# DLPR Requirements

Requirements analysis for the delta-snapshot-based replay
format (`*.dlpr`) developed by the
[delta-play-replay](https://github.com/librematch/delta-play-replay)
project.

## Background

The existing CaptureAge (CA) replay system utilizes an internal
format (`*.carz`) to play recorded games. This format supports
backward compatibility with older recorded games, allowing them
to be replayed without running the original AoE2DE simulation.
However, the `*.carz` format is primarily designed for internal
debugging purposes and in-memory use, and not for long-term
storage.

The goal is to create a new, standardized replay format that
accommodates the requirements for efficient storage, improved
replay functionalities, and broader community support.

## Current System Overview

### Existing CaptureAge Replay Format

- **Format**: `*.carz` (CaptureAge Replay Format)
- **Purpose**: Internal debugging, live spectating
- **Limitations**: Not optimized for long-term storage,
  primarily intended for in-memory use
- **Features**:
  - Backward compatibility with older games
  - Instant navigation to any point in the replay
  - No need for an AoE2DE instance to replay games

## Functional Requirements

1. **Backward Compatibility** - Support existing replays
   recorded in previous versions of AoE2DE. Ensure
   compatibility with the internal `*.carz` format used by
   CaptureAge.

2. **Delta-Snapshot System** - Implement a delta-snapshot-based
   approach to efficiently capture game state changes. Generate
   patches representing state differences at fixed intervals
   (snapshots) and on-demand (events).

3. **Conversion and Compatibility Tools** - Develop a converter
   to transform existing recorded games into the new replay
   format. Update gRPC definitions to accommodate new replay
   functionalities.

4. **Long-Term Storage** - Optimize the format for persistent
   storage, ensuring that replays are compact and easily
   shareable. Include metadata for versioning and compatibility
   checks.

5. **Improved Navigation and Spectator Features** - Enable
   quick navigation to any point in the replay, both forwards
   and backwards. Integrate spectator tools to allow live game
   viewing without running the AoE2DE simulation.

6. **Support for Live Games** - Explore server-side conversion
   for live games to facilitate real-time spectating without
   AoE2DE instances. Stream delta-patch files to spectators to
   reduce local processing requirements.

7. **Open Source and Community Support** - Make the new replay
   format open source and freely available to the community.

8. **Security and Integrity** - Implement encryption and
   integrity checks to protect replay files from tampering.

9. **Game Independence** - Evaluate how far the existing
   delta-snapshot-based replay formats are game-independent.
   Consider making the format support other games in the Age of
   Empires franchise (AoE4, AoM:R, AoE3DE).

## Non-Functional Requirements

1. **Performance** - Minimize overhead when generating and
   storing replays. Ensure smooth and responsive playback.

2. **Scalability** - Handle a wide range of game scenarios,
   from short matches to extensive tournaments. Support
   concurrent access by multiple tools.

3. **Extensibility** - Allow for future extensions without
   breaking existing compatibility.

## Comparison to Existing Format

| Feature                    | `*.carz`  | `*.dlpr`  |
| -------------------------- | --------- | --------- |
| **Backward Compatibility** | Partial   | Full      |
| **Long-Term Storage**      | Limited   | Optimized |
| **Instant Navigation**     | Supported | Supported |
| **Performance**            | ?         | Optimized |

## Future Considerations

- **Community Involvement**: Engage with the AoE2DE community
  to gather feedback and suggestions for the new replay format.
- **Integration with Other Platforms**: Explore opportunities
  to integrate with platforms like Twitch or YouTube for
  enhanced content creation and sharing.
- **Further Optimizations**: Continue researching ways to reduce
  the size of delta-snapshot files while maintaining rich
  functionality.
