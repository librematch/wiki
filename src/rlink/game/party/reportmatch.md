### Notes

- **Every client of the match reports the result**, not just the host: in a 1v1 both peers send `reportMatch` with the same `match_id`. A server that stores or rates the match has to be idempotent per `match_id` (our implementation applies the Elo change only on the first report and ignores the duplicates).
- `results` uses `1` for the winner and `0` for the loser, aligned by index with `profile_ids`.
- The response contains the replay upload target; a local server can return the same shape with empty strings when replays are not supported.
