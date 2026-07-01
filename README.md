# 🎬 Movie Industry Data Analysis
# movies-data-analysis
## About
Analysed 4,800+ movies from the TMDB dataset to uncover what drives 
movie profitability and audience ratings across decades.

## Tools Used
- Microsoft Excel (Pivot Tables, Scatter Charts, Formulas)

## Key Findings

### 💰 1. Top 3 Most Profitable Movies Ever
| Rank | Movie | Profit |
|------|-------|--------|
| 1 | Avatar | $2.55 Billion |
| 2 | Titanic | $1.64 Billion |
| 3 | Jurassic World | $1.36 Billion |

Avatar leads by a massive margin — nearly $1 billion more than 
Titanic in second place. All top 3 are franchise or event films 
with massive global appeal.

### 📅 2. Older Decades Rated Higher
The 1910s had the highest average rating (7.4), followed by the 
1950s (7.09) and 1960s (6.94). Ratings decline steadily toward 
modern decades, with 2010s scoring lowest at 5.86.

This suggests audiences rate older classics more favourably — 
likely due to survivorship bias (only the best old films are 
remembered and rated).

### 📊 3. Budget Does NOT Guarantee a Good Rating
A scatter plot of budget vs audience rating shows no clear upward 
trend. High-budget films ($200M+) still score as low as 5–6, 
while many low-budget films score 7+. 

**Insight for studios:** Spending more does not buy better 
audience reception.

## Data Cleaning Steps
- Removed corrupt and missing date entries from release_date column
- Fixed decade extraction using =LEFT(YEAR(date),3)&"0s" formula 
  to handle DD-MM-YYYY format
- Excluded rows with zero budget/revenue to avoid skewing profit 
  calculations

## Dataset
Source: [TMDB Movie Metadata — Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
