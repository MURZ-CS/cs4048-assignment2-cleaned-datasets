# CS4048 Assignment 2 - Cleaned Datasets

Cleaned datasets for CS4048 Data Science, Assignment 2 (FAST-NU Lahore).
Author: Muneeb Ur Rehman, Roll No. 23L-0511
Version: v1.0
Date: 18 October 2026

## 1. Netflix Movies and TV Shows
File: 23L_0511_A2_netflix_cleaned.csv (8,807 rows, 20 columns)

Original source: Kaggle dataset "Netflix Movies and TV Shows" by shivamb
https://www.kaggle.com/datasets/shivamb/netflix-shows
The original data belongs to its authors; please credit the source and respect its licence.

What I changed:
- Stripped extra spaces in text columns (88 date_added values, 1 title).
- Moved 3 durations that were typed into the rating column (Louis C.K. titles) back into duration; their rating became Unknown.
- Merged NR and UR into "Unrated"; merged TV-Y7-FV into TV-Y7.
- Filled missing director, cast and country with "Unknown"; left 10 missing date_added empty.
- Converted date_added to a date; split duration into movie_minutes and seasons.
- Added: year_added, month_added, movie_minutes, seasons, num_countries, num_genres, primary_country, release_to_added_gap.
- No rows removed; all outliers kept.

## 2. Supermarket Sales
File: 23L_0511_A2_supermarket_cleaned.csv (1,000 rows, 21 columns)

Original source: supermarket_Sales.csv, provided by the course instructor, used exactly as supplied.

What I changed:
- Found no missing values, duplicates, inconsistent labels or invalid values, so nothing was removed or corrected.
- Converted Date to a date type.
- Added: Month, Weekday, Hour, Is_weekend.
- All original columns kept (some are redundant, see the notebook handoff note); all outliers kept.

## Versioning
v1.0 is the version used in Assignment 2. Any later change to the cleaning will be published as a new version and will not overwrite v1.0.
