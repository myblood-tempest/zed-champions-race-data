# Zed Champions Race Data Exports

This directory contains regularly updated CSV exports of race data from the Zed Champions platform. Each file is a chunked export containing detailed information about races, participants, horses, and augments.

## File Naming Convention

- `race_data_<timestamp>_chunk<N>.csv`
  - `<timestamp>`: The UTC date and time when the export was created (format: YYYYMMDD_HHMMSS)
  - `<N>`: The chunk index (starting from 0)

## Data Columns
Each CSV file contains the following columns:

- `race_id`: Unique identifier for the race
- `race_name`: Name of the race
- `race_date`: Date and time the race started (UTC)
- `race_pots_total`: Total prize pool for the race
- `user_id`: Unique identifier for the stable owner
- `stable_name`: Name of the stable
- `gate_number`: Gate number assigned to the horse
- `horse_id`: Unique identifier for the horse
- `horse_name`: Name of the horse
- `bloodline`: Horse's bloodline
- `generation`: Horse's generation
- `rating`: Overall rating of the horse
- `speed_rating`: Speed rating
- `sprint_rating`: Sprint rating
- `endurance_rating`: Endurance rating
- `finish_position`: Final position in the race
- `finish_time`: Time taken to finish the race
- `earnings`: Earnings from the race
- `stake`: Entry stake for the race
- `profit_loss`: Net profit or loss (earnings - stake)
- `odds`: Win market odds
- `starting_points`: Points before the race
- `points_change`: Change in points after the race
- `ending_points`: Points after the race
- `cpu_augment`, `ram_augment`, `hydraulic_augment`: Names of augments equipped
- `cpu_augment_triggered`, `ram_augment_triggered`, `hydraulic_augment_triggered`: Whether the augment was triggered (1 = yes, 0 = no)

## Update Process
- Files are generated and pushed automatically in chunks, each up to 45MB, to comply with GitHub's file size limits.

---

## Support & Donations
If you find this data useful and would like to support the project, donations are greatly appreciated!

**ETH/ERC-20 Address:**
```
0x4F09B499932FF9b30C7AD408Dc0ff58756516e87
```
