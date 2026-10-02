# Auspify Technologies – Data Analysis Using Python Internship

**Intern:** Mohamed Faizal Fathima Zainab
**Program:** 4-Week Data Analysis Using Python Internship
**Dataset:** Netflix titles dataset (8,790 records, 10 columns)
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## Tasks Completed

| Task | Title | Level | Status | Folder |
|------|-------|-------|--------|--------|
| 1 | Netflix Data Cleaning & Preparation | Easy | Completed | [Task1](./Task1) |
| 2 | Content Type Analysis Dashboard | Easy | Completed | [Task2](./Task2) |
| 3 | Country-Wise Netflix Content Analysis | Medium | In progress | Task3 |
| 4 | Trend Analysis by Release Year | Medium | In progress | Task4 |

## Repository Structure

```
auspify-data-analysis-internship/
├── README.md
├── Task1/
│   ├── Task1_Netflix_Data_Cleaning.ipynb
│   ├── Dataset.csv               (raw data)
│   ├── netflix_cleaned.csv       (cleaned output, used by Tasks 2-4)
│   └── screenshots/
├── Task2/
├── Task3/
└── Task4/
```

## Task 1 – Data Cleaning Summary

| Issue found | Action taken |
|---|---|
| "Not Given" placeholders in `director` (2,588) and `country` (287) | Converted to NaN, then filled with "Unknown" |
| 4 duplicate titles with different `show_id` | Removed (8,790 → 8,786 rows) |
| `date_added` stored as text | Converted to datetime; added `year_added`, `month_added` |
| `duration` mixed minutes and seasons | Split into `duration_value` and `duration_unit` |
| Inconsistent Type / Country / Rating | Standardized; added `rating_group` |

## How to Run

```bash
pip install pandas numpy matplotlib seaborn jupyter
cd Task1
jupyter notebook Task1_Netflix_Data_Cleaning.ipynb
```

## Demo Video

Task 1 demo: PASTE YOUR VIDEO LINK HERE

#Auspify #AuspifyTechnologies #AuspifyInternship #AuspifyProjects

