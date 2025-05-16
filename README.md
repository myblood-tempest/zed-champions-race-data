# Zed Champions Race Data Export

This directory contains data exports from Zed Champions races.

## Export Logic

- When `race_results.csv` reaches **45MB**, it is automatically archived (renamed with a timestamp, e.g., `race_results_archive_YYYYMMDD_HHMMSS.csv`).
- The latest `race_date` in the archive is recorded in `archive_metadata.json`.
- Subsequent exports only include races with a `race_date` **after** the last archived value (incremental export).
- The `latest` directory always contains the most recent, active `race_results.csv`.

## Files

### race_results.csv
Comprehensive race results including horse details, augments used, and trigger status:
- `race_id` - Unique identifier for the race
- `race_name` - Name of the race
- `race_date` - When the race occurred
- `race_pots_total` - Total prize pool
- `user_id` - Unique identifier for the user/owner
- `stable_name` - Name of the stable/team
- `gate_number` - Starting gate position for the horse
- `horse_id` - Unique identifier for the horse
- `horse_name` - Name of the horse
- `bloodline` - Horse's bloodline (NAKAMOTO, SZABO, FINNEY, BUTERIN)
- `generation` - The breeding generation of the horse
- `rating` - Horse's complete rating
- `speed_rating` - Horse's speed rating
- `sprint_rating` - Horse's sprint rating
- `endurance_rating` - Horse's endurance rating
- `finish_position` - Position the horse finished in
- `finish_time` - Race finish time
- `earnings` - Amount won in the race
- `stake` - Amount staked/wagered
- `profit_loss` - Net profit or loss (earnings - stake)
- `odds` - Odds of winning (win_market)
- `starting_points` - Horse's points/rating before the race
- `points_change` - Change in points/rating
- `ending_points` - Horse's points/rating after the race
- `cpu_augment` - CPU slot augment used
- `ram_augment` - RAM slot augment used
- `hydraulic_augment` - HYDRAULIC slot augment used
- `cpu_augment_triggered` - Whether the CPU augment was triggered (true/false)
- `ram_augment_triggered` - Whether the RAM augment was triggered (true/false)
- `hydraulic_augment_triggered` - Whether the HYDRAULIC augment was triggered (true/false)

### archive_metadata.json
- Stores the `last_archived_race_date` to support incremental export.

## License
This data is shared freely for the Zed Champions community.
