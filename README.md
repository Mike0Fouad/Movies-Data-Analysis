# Movies Data Analysis

A comprehensive data analysis project exploring movie statistics, focusing on the relationship between production budgets and earnings, along with detailed metadata exploration.

## Project Overview

This project analyzes a rich dataset of film statistics from Kaggle to uncover insights about how production budgets impact movie earnings and explores various metadata characteristics of films.

## Dataset

- **Source:** [The Ultimate Film Statistics Dataset for ML](https://www.kaggle.com/datasets/alessandrolobello/the-ultimate-film-statistics-dataset-for-ml)
- **File:** `movie_statistic_dataset.csv`
- **Location:** `data/` directories in both analysis folders

## Project Structure

```
Movies Data Analysis/
├── Insights/
│   ├── Analysis.ipynb           # Budget vs. Earnings correlation analysis
│   └── data/
│       └── movie_statistic_dataset.csv
├── Meta Data/
│   ├── Meta Data.ipynb          # Dataset metadata exploration
│   └── data/
│       └── movie_statistic_dataset.csv
└── README.md
```

## Analysis Notebooks

### 1. **Insights/Analysis.ipynb** - Budget Impact on Earnings
Analyzes the correlation between production budget and worldwide gross earnings.

**Key Sections:**
- Data Preprocessing
  - Loading the dataset
  - Handling missing values (replacing "-" and "\N" with NaN)
  - Dropping rows with missing budget or earnings data
  - Converting columns to appropriate numeric data types
- Exploratory Data Analysis (EDA)
  - Descriptive statistics for budget and earnings
  - Distribution visualizations
  - Budget category analysis (< $10M, $10M-$50M, $50M-$100M, $100M-$200M, > $200M)
  - Pie charts showing movie distribution by budget
  - Earnings distribution visualizations
- Statistical Analysis
  - Correlation analysis using Spearman correlation

### 2. **Meta Data/Meta Data.ipynb** - Dataset Metadata Analysis
Provides comprehensive exploration of the dataset structure and characteristics.

**Key Sections:**
- Dataset Overview
  - Dataset shape and column information
  - Missing value counts (checking for "\N" and "-" placeholders)
- Data Quality Checks
  - Uniqueness of values (nunique)
  - Duplicate movie title detection
- Descriptive Statistics
  - Summary statistics for numerical columns
- Genre Analysis
  - Genre value counts and combinations
  - Individual genre frequency analysis

## Technologies & Libraries

- **Python** - Primary programming language
- **Pandas** - Data manipulation and analysis
- **Matplotlib** - Data visualization
- **SciPy** - Statistical analysis (Spearman correlation)

## Key Features

- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA)
- Statistical correlation analysis
- Genre analysis
- Budget categorization and visualization
- Missing value handling
- Data quality checks

## Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook or VS Code with Jupyter support
- Required libraries: pandas, matplotlib, scipy

### Installation
1. Clone or download this project
2. Install dependencies:
   ```bash
   pip install pandas matplotlib scipy
   ```

### Running the Analysis
1. Open either notebook in Jupyter Notebook or VS Code
2. Ensure the CSV file is in the correct `data/` subdirectory
3. Run the cells sequentially to execute the analysis

## Key Findings

The analysis explores:
- The relationship between production budgets and movie earnings
- Distribution patterns of movies across budget categories
- Genre composition and frequency in the dataset
- Data quality and missing values

## Notes

- The dataset contains placeholder values ("-" and "\N") that are handled during preprocessing
- Both notebooks use local relative paths to the data files (`./data/movie_statistic_dataset.csv`)
- The analysis focuses on two key metrics: Production Budget ($) and Worldwide Gross ($)

## License

Dataset sourced from Kaggle - refer to the dataset's license terms.

## Future Enhancements

- Interactive visualizations using Plotly
- Machine learning models to predict earnings based on budget
- Time-series analysis of movie performance
- Director and actor influence analysis
- More advanced statistical tests
