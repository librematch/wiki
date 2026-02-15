# gRPC API

Documentation for the gRPC API exposed by Age of Empires II:
Definitive Edition (AoE2DE) during replay playback, as
reverse-engineered by the LibreMatch project.

## Overview

AoE2DE exposes a gRPC endpoint when watching replays. This
allows external tools to receive game state updates in real-time
without running the game simulation themselves. The API streams
delta patches representing frame-by-frame state changes, along
with game events and player commands. It is used by
[CaptureAge](https://captureage.com/) for spectating.

The protocol buffer definitions and format specification
documented here are the result of reverse engineering the
`*.caderec` format as part of the LibreMatch
[delta-play-replay](https://github.com/librematch/delta-play-replay)
project.

## Protocol Buffers

The API is defined using three proto files:

- **[CadeRemote Service](./main.md)** (`cade_api.proto`) - The
  main gRPC service with RPCs for game info, pause control, fog
  of war, perspective switching, and frame streaming
- **[Atlas Data](./atlas_data.md)** (`atlas_data.proto`) -
  Sprite and asset information for rendering
- **[File Metadata](./file_metadata.md)**
  (`file_metadata.proto`) - Metadata for graphics files

## Delta Play Replay (DLPR)

[delta-play-replay](https://github.com/librematch/delta-play-replay)
is the LibreMatch project for creating a specification and
tooling around a new open replay format (`*.dlpr`) for AoE2DE,
based on the reverse-engineered `*.caderec` format:

- **[Delta Patch Format](./delta_format.md)** - Specification of
  the stack-based delta patch format used in frame data
- **[DLPR Requirements](./dlpr_requirements.md)** - Requirements
  analysis for the new replay format
