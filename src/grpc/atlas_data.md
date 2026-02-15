# Atlas Data

Sprite and asset information used for rendering game graphics.

- **Package**: `renderer.atlas.collector.ser`
- **Source**:
  [atlas_data.proto](https://github.com/librematch/delta-play-replay/blob/main/crates/uncage-client/proto/atlas_data.proto)

## Proto File

```protobuf
syntax = "proto3";

package renderer.atlas.collector.ser;

option optimize_for = SPEED;

message Options {
  uint32 exploredMask = 1;
  uint32 dopplegangerMask = 2;
  bool enhancedGraphics = 3;
  repeated string enabledMods = 4;
}

message ExtraAssetFrameInfo { bool used = 1; }

message AssetInfo {
  int32 id = 1;
  string fileName = 2;
  bool used = 3;
  bool broken = 4;
  repeated bytes headers = 5;
  SpriteInfo spriteInfo = 6;
  repeated ExtraAssetFrameInfo extraFrameInfo = 7;
}

message SpriteInfo {
  string name = 1;
  int32 facetNum = 2;
  int32 frameNum = 3;
}

message FrameInfo {
  uint32 frame = 1;
  uint32 time = 2;
  repeated Frames remove = 3;
  repeated Frames add = 4;
  repeated Frames once = 5;
}

message Frames {
  int32 assetId = 1;
  repeated int32 frames = 2;
}

message AtlasData {
  Options options = 1;
  repeated AssetInfo assets = 2;
  repeated FrameInfo frames = 3;
}
```

## Messages

### Options

Rendering options including explored/doppelganger masks,
enhanced graphics toggle, and enabled mod list.

### AssetInfo

Describes a sprite asset: its ID, file name, usage status,
and per-frame information via `SpriteInfo` and
`ExtraAssetFrameInfo`.

### SpriteInfo

Sprite metadata with name, number of facets (rotation
angles), and number of frames (animation steps).

### FrameInfo

Per-frame changes to the atlas. Each frame can add, remove,
or play-once specific sprite frames.

### AtlasData

Top-level container combining rendering options, all asset
definitions, and frame-by-frame atlas changes.
