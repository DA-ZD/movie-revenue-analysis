# Movie Revenue and IMDb Ratings Analysis

An exploratory data analysis and data wrangling project combining Kaggle's Movies Dataset and OMDb API data to uncover the relationship between financial success and audience appreciation.

## Overview

This project investigates and wrangles two distinct datasets to answer a key research question:
* Do movies with the highest revenue tend to have the best IMDb ratings?

The analysis involved gathering data manually and programmatically via API, cleaning structural and quality issues (such as parsing JSON-formatted strings and fixing mixed data types), and conducting exploratory analysis using Python in a Jupyter Notebook environment.

## Key Findings

* **Revenue vs. Ratings:** High revenue does not necessarily guarantee the absolute highest IMDb ratings. Most high-revenue movies cluster around average IMDb ratings between 6 and 8.
* **Top Earners:** The top 10 highest-grossing movies in the dataset all hold strong IMDb ratings between 7 and 9, suggesting that while financial success aligns with positive audience reception, revenue alone is not the sole indicator of a highly-rated film.

## Technologies Used

* Python 3
* Pandas
* NumPy
* Matplotlib
* Requests (API Integration)
* Jupyter Notebook

## Project Structure

├── Data_Wrangling_Project_Starter.ipynb   # Main analysis and wrangling notebook
├── movies_metadata.csv                    # Raw dataset 1 (Kaggle)
├── omdb_data.csv                          # Raw dataset 2 (OMDb API)
├── cleaned_movies_combined.csv            # Final cleaned and merged dataset
└── README.md                              # Project documentation

## Limitations

* **Sample Size:** Due to API constraints and processing time, only a subset of movies (the first 1,000) was queried from the OMDb API.
* **Missing Data:** Movies with missing `BoxOffice` values were dropped during the cleaning phase, which reduced the final dataset size.
* **Scope:** The analysis is exploratory only — no strict statistical hypothesis testing was performed. Results describe patterns and should not be interpreted as evidence of causation.

## How to Run

Clone the repository:
```bash
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
