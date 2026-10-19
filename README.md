# Assignment 2 - Cleaned Datasets (23L-0983)

Cleaned datasets from Assignment 2 (Exploratory Data Analysis), Data Science, FAST-NUCES Lahore. These files will be used in Assignment 3.

| File | Rows x Columns |
|---|---|
| 23L_0983_A2_netflix_cleaned.csv | 8,793 x 25 |
| 23L_0983_A2_supermarket_cleaned.csv | 1,000 x 25 |

**Version:** v1.0  
**Date:** 2026-10-19

## Original sources
- Netflix Movies and TV Shows (Kaggle): https://www.kaggle.com/datasets/shivamb/netflix-shows
- Supermarket Sales: `supermarket_Sales.csv` provided by the course instructor

## Changes made

**Netflix**
- Removed extra spaces, line breaks and stray commas in text columns
- Moved 3 durations that were in the `rating` column back to `duration`
- Removed 14 duplicate rows (same title written differently / listed twice)
- Converted `date_added` to a date (10 missing dates left empty)
- Merged UR into NR and TV-Y7-FV into TV-Y7; missing ratings set to "Unknown"
- Missing `director`, `cast` and `country` set to "Unknown"
- Added: year_added, month_added, years_to_add, movie_minutes, tv_seasons, n_countries, primary_country, n_genres, n_cast, n_directors, genre_families, maturity_group, is_short_film
- Outliers kept

**Supermarket Sales**
- No missing values, duplicates or errors found, so no rows changed or removed
- Column names changed to snake_case
- Converted `date` to a date and added `datetime`
- Added: month, month_name, weekday, weekday_num, is_weekend, hour, time_of_day

## Versions
- v1.0 (2026-10-19): first version, submitted with Assignment 2
