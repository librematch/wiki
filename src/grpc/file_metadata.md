# File Metadata

Metadata for SMX graphics files used by AoE2DE.

- **Package**: `renderer.smx.metadata`
- **Source**:
  [file_metadata.proto](https://github.com/librematch/delta-play-replay/blob/main/crates/uncage-client/proto/file_metadata.proto)

## Proto File

```protobuf
syntax = "proto3";

package renderer.smx.metadata;

option optimize_for = SPEED;

message FileMetadata {
  string name = 1;
  int64 lastModified = 2;
  int32 version = 3;
  uint32 fileSize = 4;
  repeated uint32 frameOffsets = 5;
  bytes sldFrames = 6;
  uint32 globalAlpha = 7;
}

message DirectoryMetadata {
  string path = 1;
  repeated FileMetadata files = 2;
}

message MetadataStore {
  repeated DirectoryMetadata directories = 1;
  int32 version = 2;
}
```

## Messages

### FileMetadata

Metadata for a single graphics file: name, modification
timestamp, version, file size, frame offsets for random
access, SLD frame data, and global alpha value.

### DirectoryMetadata

Groups file metadata entries under a directory path.

### MetadataStore

Top-level container holding all directory metadata with a
store-wide version number.
