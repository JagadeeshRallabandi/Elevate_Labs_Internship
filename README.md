# Task 1: Data Cleaning and Preprocessing

## Dataset Used:
Netflix Movies and TV Shows  
Source: https://www.kaggle.com/datasets/shivamb/netflix-shows

## Summary of Changes Made:

1. **Missing Values:**
   - Filled missing `director`, `cast`, `country`, `rating`, and `duration` with "Unknown".
   - Converted `date_added` to datetime format, handling missing values.

2. **Duplicate Rows:**
   - Removed all duplicate rows using `.drop_duplicates()`.

3. **Text Standardization:**
   - Lowercased and stripped spaces in `type`.
   - Title-cased `country` and uppercased `rating` values.

4. **Date Format Conversion:**
   - Converted `date_added` to standard `datetime` format using Pandas.

5. **Column Renaming:**
   - Renamed all column headers to lowercase with underscores (e.g., `show_id`, `date_added`).

6. **Data Types Fix:**
   - Ensured `show_id` is of string type.
   - Verified that `release_year` is already integer.

## Output:
- Cleaned dataset: `cleaned_netflix_dataset.csv`

## Tools Used:
- Python
- Pandas

