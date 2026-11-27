# Data Preparation and Cleaning Log

## Original Data

Source: UCI Bike Sharing Dataset

Files:
- `hour.csv`: Hourly bike rental observations.
- `day.csv`: Daily bike rental observations.

The original CSV files are stored in `data/raw/` and are not modified.

## Cleaning and Transformations

The following transformations were applied to both datasets:

1. Converted `dteday` from string format to pandas datetime format.
2. Sorted observations chronologically.
3. Added `season_name` to convert numerical season codes into readable labels.
4. Added `weather_name` to convert numerical weather codes into readable labels.
5. Added `month_name` to convert numerical month codes into readable labels.
6. Preserved all original columns and numerical category codes.

## Data Quality Checks

The following checks were performed:
- Missing values.
- Duplicate rows.
- Negative rental counts.
- Date range and observation counts.

No observations were intentionally removed during initial preparation.

## Dataset Selection

The hourly dataset is the primary dataset for analyses involving:
- Hourly rental patterns.
- Time-of-day behavior.
- Detailed demand prediction.

The daily dataset is used for:
- Long-term rental trends.
- Monthly and seasonal comparisons.
- Daily rental distributions.

## Output Files

- `hour_clean.csv`: Prepared hourly dataset.
- `day_clean.csv`: Prepared daily dataset.

Both datasets retain their original variables, with additional readable categorical labels and converted date columns.