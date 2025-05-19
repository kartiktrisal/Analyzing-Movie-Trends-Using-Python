# 🎬 Analyzing Movie Trends: Genres and Ratings

This project analyzes movie trends using the MovieLens Dataset to explore genre popularity, viewer ratings, and how movie complexity has evolved over time through data cleaning and visual analysis.

## 📂 Dataset Source

- **MovieLens Dataset** by [GroupLens](https://grouplens.org/datasets/movielens/)
- Files used:
  - `movies.csv`: Contains `movieId`, `title`, and `genres`
  - `ratings.csv`: Contains `userId`, `movieId`, `rating`, and `timestamp`

## 🔍 Data Exploration & Cleaning

- Removed rows with `(no genres listed)` as they lack meaningful genre data
- Split pipe-separated genres into individual rows (one genre per row)
- Extracted release year from titles using regex and grouped by decade
- Removed duplicate entries to ensure each movie is uniquely represented
- Merged datasets on `movieId` for integrated analysis

## 📊 Analysis Performed

### 1. Genre Distribution
- Counted how many times each genre appeared across all movies
- Revealed the most and least represented genres

### 2. Single vs. Multi-Genre by Decade
- Categorized movies as single or multi-genre
- Grouped by release decade to examine genre complexity trends

### 3. Movies & Ratings by Decade
- Counted number of movies and total ratings per decade
- Highlighted user engagement and industry output over time

## 💻 Program Description

The program processes, merges, and analyzes the datasets to generate insights at:
- **Genre level**: Frequency, average ratings, and total ratings per genre
- **Decade level**: Movie count and user engagement over time
- Results are saved as `.csv` files and visualized using bar charts

## 📁 Output Files

| Filename | Description |
|----------|-------------|
| `genre_summary.csv` | Total number of movies per genre |
| `multiple_genres.csv` | Count of movies with multiple genres |
| `movies_with_max_genres.csv` | Movies with the highest number of genres |
| `movies_by_decade.csv` | Movie count per decade |
| `genre_type_ratio.csv` | Single vs multi-genre count by decade |
| `genre_comparison.csv` | Movies, average rating, and total ratings by genre |
| `decade_comparison.csv` | Movies, average rating, and total ratings by decade |

## 🛠 Tools Used

- Python
- Pandas, NumPy
- Matplotlib
- Jupyter Notebook

## 📌 How to Run

1. Clone the repository
2. Ensure `movies.csv` and `ratings.csv` are in the working directory
3. Open and run `Project.ipynb` in Jupyter Notebook

---
