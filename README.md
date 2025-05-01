# Zed Champions Race Data

This repository contains race results data from Zed Champions, automatically updated every 2 hours.

## Data Structure

The `race_results.csv` file contains the following columns:

- `race_id` - Unique identifier for the race
- `race_name` - Name of the race
- `race_date` - When the race occurred
- `race_pots_total` - Total prize pool
- `horse_id` - Unique identifier for the horse
- `horse_name` - Name of the horse
- `bloodline` - Horse's bloodline (NAKAMOTO, SZABO, FINNEY, BUTERIN)
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

Data is automatically updated every ~2 hours.