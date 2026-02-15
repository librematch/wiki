# Delta Patch Format

AoE2DE streams game state changes through the gRPC
[Frames](./main.md#framesrequest) RPC as binary delta patches.
This document specifies the patch format as reverse-engineered
by the
[delta-play-replay](https://github.com/librematch/delta-play-replay)
project.

The state model definition used to interpret patches can be
found in
[model.rs](https://github.com/librematch/delta-play-replay/blob/main/crates/uncage/src/model.rs).

## Overview

The format is **stack-based** and requires a pre-definition of
the state object. Instructions either modify the patcher state
(navigating the object tree) or the state object itself.

Each instruction starts with **1 byte** (the action ID),
followed by variable-length arguments. Argument sizes can only
be resolved by maintaining the current patcher state, since
field types determine how values are read.

## Actions

```
Object methods:
 1 - Pop
 2 - Assign Field
 3 - Push Field
 4 - Push, Create and Assign Field
 5 - Reset Field

Map methods (sometimes used for lists):
 6 - Assign Key
 7 - Push Key
 8 - Push, Create and Assign Key
 9 - Reset Key

List methods (sometimes used for maps):
10 - Insert
11 - Push, Create and Insert
12 - Remove
13 - Swap
14 - Resize
```

## 1. Pop

Pop an object from the stack (go to the parent object).

Takes no arguments.

## 2. Assign Field

Set a field to a value.

| Name  | Type    | Description              |
| ----- | ------- | ------------------------ |
| Field | u8      | Which field to assign to |
| Value | Dynamic | Value to assign          |

## 3. Push Field

Push the object in the given field onto the stack (make it
the current context).

| Name  | Type | Description   |
| ----- | ---- | ------------- |
| Field | u8   | Field to push |

## 4. Push, Create and Assign Field

Create a new object for the given field, assign it, and push
it onto the stack.

| Name       | Type | Description                      |
| ---------- | ---- | -------------------------------- |
| Field      | u8   | Field to assign the new model to |
| Model Type | u8   | Which model to create            |

## 5. Reset Field

Remove the object on the given field.

| Name  | Type | Description    |
| ----- | ---- | -------------- |
| Field | u8   | Field to reset |

## 6. Assign Key

Set a key in a map (or list) to a value.

| Name  | Type    | Description            |
| ----- | ------- | ---------------------- |
| Field | u8      | Field with map or list |
| Key   | i32     | Key to assign to       |
| Value | Dynamic | Value to assign        |

## 7. Push Key

Push the object at the given key onto the stack.

| Name  | Type | Description                 |
| ----- | ---- | --------------------------- |
| Field | u8   | Field with map or list      |
| Key   | i32  | Key with the object to push |

## 8. Push, Create and Assign Key

Create a new object, assign it to the given key, and push it.

| Name       | Type | Description                |
| ---------- | ---- | -------------------------- |
| Field      | u8   | Field with map or list     |
| Model Type | u8   | Which model to create      |
| Key        | i32  | Key to assign to, and push |

## 9. Reset Key

Remove the object at the given key.

| Name  | Type | Description               |
| ----- | ---- | ------------------------- |
| Field | u8   | Field with map or list    |
| Key   | i32  | Key to the value to reset |

## 10. Insert

Insert a value at the given index in a list.

| Name  | Type    | Description        |
| ----- | ------- | ------------------ |
| Field | u8      | Field with list    |
| Index | i32     | Index to insert to |
| Value | Dynamic | Value to insert    |

## 11. Push, Create and Insert

Create a new object, insert it at the given index, and push
it.

| Name       | Type | Description                  |
| ---------- | ---- | ---------------------------- |
| Field      | u8   | Field with list              |
| Model Type | u8   | Which model to create        |
| Index      | i32  | Index to insert to, and push |

## 12. Remove

Remove an object at the given index.

| Name  | Type | Description            |
| ----- | ---- | ---------------------- |
| Field | u8   | Field with list or map |
| Index | i32  | Index to remove        |

## 13. Swap

Swap two entries in a list or map.

| Name    | Type | Description                      |
| ------- | ---- | -------------------------------- |
| Field   | u8   | Field with list or map           |
| Index A | i32  | Index of value to replace B with |
| Index B | i32  | Index of value to replace A with |

## 14. Resize

Resize a list to the given length. In some cases, child
objects are expected to be created automatically.

| Name       | Type | Description        |
| ---------- | ---- | ------------------ |
| Field      | u8   | Field with list    |
| New Length | i32  | New length of list |
