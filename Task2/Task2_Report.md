# Task 2 Report – Content Type Analysis Dashboard

**Intern:** Mohamed Faizal Fathima Zainab
**Offer Letter ID:** AT/INT/2037034
**Program:** Data Analysis Using Python Internship – Auspify Technologies

## 1. Objective
Analyze the distribution of Movies and TV Shows available on Netflix.

## 2. Data and tools
- **Input:** `netflix_cleaned.csv` from Task 1 (8,786 titles, 15 columns, no missing values)
- **Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## 3. Workflow
| Step | What I did |
|------|------------|
| 1. Load | Loaded the cleaned dataset from Task 1 and checked its shape and missing values |
| 2. Count | Calculated the number and percentage of Movies and TV Shows |
| 3. Visualize | Bar chart, donut chart, titles added per year, movie duration histogram, TV Show seasons chart |
| 4. Compare | Share by release decade, rating group by type, TV Show share of new titles over time |
| 5. Summarize | Combined 2x2 dashboard and key findings calculated from the data |

## 4. Key findings
1. Netflix has **8,786 titles**: **6,123 Movies (69.69%)** and **2,663 TV Shows (30.31%)**.
2. There are about **2.3 Movies for every TV Show**.
3. Movie additions peaked in **2019 (1,422 titles)**. TV Show additions peaked in **2020 (595 titles)**.
4. The median movie runs **98 minutes**, and **67% of TV Shows have only 1 season**.
5. Adult-rated content is **47% of Movies and 43% of TV Shows**. Content for kids and older kids is **21% of Movies and 29% of TV Shows**.
6. TV Shows made up **32% of titles added in 2020**, compared with **41% in 2016**.

## 5. Business insights
- **Movies dominate the catalogue** (about 7 in 10 titles), so the library's depth is mostly film.
- **Most TV Shows have one season**, which suggests many limited series or shows that were not renewed.
- **Additions grew sharply from 2016 to 2019.** Movie additions dipped in 2020, while TV Show additions kept rising until 2020.
- **Adult content is the largest audience group** for both types. TV Shows lean a little more toward kids and older kids than Movies do.
- **Recommendation:** keep investing in movies for catalogue breadth, and track TV Show renewals, since returning series drive long-term engagement.

## 6. Limitations
- The dataset ends in **September 2021**, so 2021 is a partial year.
- It describes the catalogue, not viewing numbers, so it cannot show which titles are most watched.

## 7. Files
- `Task2_Content_Type_Analysis.ipynb`: full code and outputs
- `charts/`: 8 PNG charts, including `08_dashboard.png`
- `screenshots/`: screenshots of key outputs
