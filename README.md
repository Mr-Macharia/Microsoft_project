Sure! Here’s a draft for the README file that you can use to describe the project:

---

# IMDb Movie and Financial Data Analysis for Microsoft

## Project Overview

This project analyzes IMDb movie data and financial performance, exploring relationships between key factors like movie genres, directors, writers, ratings, production budgets, and revenue. The analysis provides insights into the correlations between movie ratings, financial success, popularity by genre, and the performance of directors and writers. The goal is to provide an understanding of what drives movie success and which genres, professionals, and budget levels are more likely to yield positive outcomes.

## Data Sources

The project involves multiple datasets that have been merged and processed to analyze:
- **IMDb People Data:** Contains information about directors, writers, and their movies.
- **IMDb Ratings Data:** Contains IMDb movie ratings and vote counts.
- **Movie Financial Data:** Includes information about production budgets, domestic and worldwide gross, release dates, and studios.

## Project Workflow

### 1. **Data Cleaning and Merging**
The project starts by cleaning and merging different datasets to align movie professionals (directors and writers) with their respective films and financial information:
- **Filtering Directors and Writers:** Extracted rows containing 'director' and 'writer' from the primary dataset and renamed columns for clarity.
- **Data Merging:** Merged the data frames for people, movies, and ratings based on `person_id` and `movie_id`, linking directors and writers to the corresponding ratings and genres.
- **Removing Unnecessary Data:** Dropped irrelevant or null values to focus on entries that had both director and writer information available.

### 2. **Financial Data Analysis**
- **Production Budget vs. Worldwide Gross:** A scatter plot was created to show the correlation between a movie's production budget and its worldwide gross, highlighting that higher-budget films generally tend to earn higher worldwide grosses.
- **Top 20 Movies by Production Budget:** Visualized the top 20 highest-budget movies and their scaled worldwide gross, showing that high-budget movies tend to be financially successful but may still risk losses.
- **Domestic Gross vs. Worldwide Gross:** Demonstrated a strong positive correlation between domestic and worldwide gross, suggesting that successful movies in domestic markets often succeed internationally as well.
- **Financial Profit Analysis:** Explored the relationship between production budget and financial profit, concluding that higher production budgets generally lead to greater profits.

### 3. **Genre Popularity Analysis**
- **Average Popularity by Genre:** Split movie genres into a manageable format and calculated the average popularity for each genre, visualizing the results. Genres like war, sports, family, music, and fantasy were found to be the most popular.
  
### 4. **Directors and Writers Performance**
- **Top 20 Directors and Writers by Rating:** Sorted directors and writers based on the average IMDb rating of their movies. Bar charts were created to visualize the top-performing directors and writers.
- **Comparison of Directors vs. Writers:** The analysis showed that directors who are also involved in writing the movie tend to produce higher-rated movies, suggesting that a closer collaboration between the director and the writer leads to better outcomes.

### 5. **Visualizations**
- **Scatter Plots and Bar Charts:** The project uses several visualizations, including scatter plots, bar charts, and horizontal bar charts, to display relationships between variables such as production budgets, revenues, and genre popularity.
- **Comparison of Top Directors and Writers:** A side-by-side plot showing the performance of the top 20 directors and writers, which emphasizes that directors involved in writing tend to produce higher-rated movies.

## Technologies Used

- **Pandas**: For data manipulation and merging.
- **Matplotlib**: For creating visualizations and charts.
- **NumPy**: For calculations and numerical operations.
- **Python**: The programming language used for the project.

## Key Insights

- **Financial Success:** Higher production budgets generally lead to greater worldwide grosses and financial profits, but there are exceptions.
- **Popularity by Genre:** The most popular genres include war, sports, family, music, and fantasy, which are more likely to attract larger audiences.
- **Director and Writer Influence:** Directors who are also writers tend to produce better-rated films, suggesting that closer involvement in the movie’s creative process yields better results.

## Conclusion

This analysis provides actionable insights for stakeholders in the film industry, such as producers and directors, to focus on high-performing genres and ensure close collaboration between directors and writers for better movie ratings. Additionally, investing in higher production budgets, while risky, is likely to result in higher worldwide gross, especially when targeting popular genres.

---
