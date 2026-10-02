# Task 1 Report – Netflix Data Cleaning & Preparation

**Intern:** Mohamed Faizal Fathima Zainab
**Offer Letter ID:** AT/INT/2037034
**Program:** Data Analysis Using Python Internship – Auspify Technologies

## 1. Objective
Prepare and organize the Netflix dataset so it is ready for business analytics and reporting in the later tasks.

## 2. Dataset overview
- **Source file:** `Dataset.csv` (raw)
- **Size:** 8,790 rows × 10 columns
- **Columns:** show_id, type, title, director, country, date_added, release_year, rating, duration, listed_in

## 3. Tools used
Python, Pandas, NumPy, Jupyter Notebook

## 4. Process and findings

| Step | What I checked | Finding | Action taken |
|------|----------------|---------|--------------|
| 1. Import | Shape, data types | 8,790 rows, 10 columns; dates and duration stored as text | Loaded with Pandas |
| 2. Missing values | True NaN values and hidden placeholders | 0 true NaN, but "Not Given" in `director` (2,588) and `country` (287) | Converted to NaN, filled with "Unknown" |
| 3. Duplicates | Exact duplicates and duplicates ignoring `show_id` | 0 exact; 4 hidden duplicates (15-Aug, 22-Jul, 9-Feb, Consequences). 'Consequences' was only detected after trimming extra whitespace | Removed, keeping the first record |
| 3. Formatting | Date and duration columns | `date_added` was text; `duration` mixed minutes and seasons | Converted to datetime; split duration into value and unit; added `year_added`, `month_added` |
| 4. Standardization | Type, Country, Rating | Labels needed trimming and consistency checks | Standardized all three; added `rating_group` (Kids, Older Kids, Teens, Adults, Unrated) |
| 5. Export | Final quality check | 0 missing values, 0 duplicates | Saved `netflix_cleaned.csv` |

## 5. Results
- Rows: **8,790 → 8,786** (4 duplicate records removed)
- Missing values after cleaning: **0**
- Duplicate rows after cleaning: **0**
- Content types: **6,123 Movies** and **2,663 TV Shows**
- Unique countries (including "Unknown"): **86**
- Columns: 10 → **15** (added `year_added`, `month_added`, `duration_value`, `duration_unit`, `rating_group`)

## 6. Conclusion
The dataset is now clean, consistent and correctly typed. `netflix_cleaned.csv` is the input for the analysis tasks that follow.

## 7. Files
- `Task1_Netflix_Data_Cleaning.ipynb`: full code and outputs
- `Dataset.csv`: raw data
- `netflix_cleaned.csv`: cleaned data
- `screenshots/`: screenshots of key outputs
