# 🎬 Top 10,000 IMDb Movies — Exploratory Data Analysis

A beginner-friendly EDA project exploring a dataset of the top 10,000 movies on IMDb — covering data cleaning, univariate/bivariate analysis, correlations, outliers, and feature engineering.

## 📊 Overview

This project walks through a complete, step-by-step exploratory data analysis of an IMDb movies dataset using **Python, Pandas, and Seaborn/Matplotlib**. It's structured in clear phases so it's easy to follow even for those new to data analysis.

## 🔍 Phases Covered

1. **Load the Data** — Import the dataset (`Top_10000_Movies_IMD.csv`) with Pandas
2. **Understand the Data** — Shape, structure, and summary statistics
3. **Check Data Quality** — Missing values and duplicate rows
4. **Clean the Data** — Convert `Runtime` from text to numeric, fill missing `Metascore` values with the median, simplify `Genre` into a `Main Genre` column
5. **Univariate Analysis** — Distribution of ratings, runtime, and most common genres
6. **Bivariate Analysis** — Rating vs. Votes, Rating by Genre, Runtime vs. Rating
7. **Correlation Analysis** — Heatmap of relationships between Rating, Runtime, Metascore, Votes, and Gross
8. **Outlier Detection** — Boxplots for Votes and Gross, and identifying top-grossing blockbusters
9. **Feature Engineering** — New `Popularity` category (Low/Medium/High) based on vote count, and average rating by popularity group
10. **Final Summary** — Key takeaways from the analysis

## 🔑 Key Insights

- The dataset contains **9,999 movies** with Rating, Genre, Runtime, Votes, and Gross earnings.
- Only the `Metascore` column had missing values — filled with the median.
- Most movies are rated between **7 and 8.5**, since the dataset only includes top-rated films.
- **Drama** is the most common genre, followed by Comedy and Action.
- **Votes and Gross earnings are strongly correlated** — more popular movies tend to earn more.
- Rating doesn't correlate strongly with any single numeric column, suggesting it depends on qualitative factors like story or direction.
- Outliers in Votes and Gross are real blockbuster movies, not data errors.

## 🛠️ Tools & Libraries

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📁 Repository Contents

| File | Description |
|------|--------------|
| `Top10000_movies_EDA.ipynb` | Jupyter notebook containing the full step-by-step EDA |
| `Top_10000_Movies_IMD.csv` | Raw input dataset |
| `Top_10000_Movies_IMD_cleaned_simple.csv` | Cleaned dataset exported at the end of the notebook |
| `README.md` | Project documentation (this file) |

## 🚀 How to Use

1. Clone or download this repository.
2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Top10000_movies_EDA.ipynb
   ```
4. Run the cells in order — each phase includes markdown explanations and insights alongside the code.

## 📌 Notes

- This notebook is designed as a learning resource, with clear phase-by-phase commentary explaining *why* each step is done, not just *how*.
- The cleaned dataset (`_cleaned_simple.csv`) can be reused for further analysis or modeling.

## 📄 License

This project is open for educational and portfolio use.
