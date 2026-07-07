---
run_id: L5S1-0XDW
---

# L5S1 rollout RDN

Review checklist. Complete the items strictly in sequence.

1. Query the approved historical-weather source for Vienna, Austria on 2020-12-30 (timezone Europe/Berlin). Find the hour with the lowest temperature; if several hours tie, choose the earliest. Call the two-digit hour HOUR_24.
2. Read media/L5S1_readout_0X2.vtt.
3. Inspect the capture at timestamp 00:{HOUR_24}: read the fields in the cue that covers that second.

## Procedure card

Skill: timestamped_video_clue_extraction
Purpose: Derive a timestamp from a verified source value, inspect a timed capture artifact at that timestamp, and extract the structured fields its cue displays.
Inputs: capture file (WebVTT), derived two-digit value as 00:VALUE
Normalization: read the structured key=value fields in the cue covering the timestamp
Store this skill under its name. Later tasks refer to it by name and expect it to be applied without re-teaching.
