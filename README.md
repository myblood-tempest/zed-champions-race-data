# Zed Champions Race Data Export

## Export Date: 2025-05-01 16:36:28

This directory contains data exports from Zed Champions races.

## Files

### race_results.csv
Comprehensive race results including horse details and augments used:
- `race_id` - Unique identifier for the race
- `race_name` - Name of the race
- `race_date` - When the race occurred
- `race_pots_total` - Total prize pool
- `user_id` - Unique identifier for the user/owner
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

### horse_performance.csv
Aggregated performance statistics for each horse:
- `horse_id` - Unique identifier for the horse
- `horse_name` - Name of the horse
- `bloodline` - Horse's bloodline
- `rating` - Horse's complete rating
- `speed_rating` - Horse's speed rating
- `sprint_rating` - Horse's sprint rating
- `endurance_rating` - Horse's endurance rating
- `races_count` - Number of races the horse has participated in
- `avg_position` - Average finish position
- `best_position` - Best/lowest finish position
- `total_stake` - Total amount staked across all races
- `total_earnings` - Total amount earned across all races
- `total_profit_loss` - Total profit or loss (earnings - stake)
- `avg_odds` - Average odds across all races
- `win_count` - Number of races won (1st place)
- `top3_count` - Number of races finished in top 3
- `win_rate` - Percentage of races won
- `avg_points_change` - Average change in points/rating per race

### augment_performance.csv
Analysis of augment effectiveness overall and by bloodline:
- `augment_name` - Name of the augment
- `augment_type` - Type of the augment (CPU, RAM, HYDRAULIC)
- `usage_count` - Number of times the augment was used
- `avg_position` - Average finish position when using this augment
- `avg_odds` - Average odds when using this augment
- `win_count` - Number of races won with this augment
- `win_rate` - Percentage of races won with this augment
- `win_rate_nakamoto` - Win rate when used by NAKAMOTO bloodline
- `win_rate_szabo` - Win rate when used by SZABO bloodline
- `win_rate_finney` - Win rate when used by FINNEY bloodline
- `win_rate_buterin` - Win rate when used by BUTERIN bloodline

## License
This data is shared freely for the Zed Champions community.
