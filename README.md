###  Analysis Movies Performance

#### Objective
The primary objective of this project is to analyze the key factors that influence a movie's box office performance, with a focus on understanding those which would assist the company start planning for its new studio.

#### Data Sources
1. **Rotten Tomatoes Reviews** (`rt.reviews.tsv.gz`)
2. **The Numbers Movie Budgets** (`tn.movie_budgets.csv.gz`)
3. **Box Office Mojo Movie Gross** (`bom.movie_gross.csv.gz`)
4. **Rotten Tomatoes Movie Information** (`rt.movie_info.tsv.gz`)

#### Data Cleaning and Preparation
- **Handling Missing Values:** Removed or imputed missing values.
- **Data Type Conversions:** Ensured appropriate data types for all columns.
- **Merging Datasets:** Combined datasets based on common keys (e.g., movie titles) to create a comprehensive dataset for analysis.
- **Removing Duplicates:** Ensured no duplicate entries existed in the merged dataset.

#### Exploratory Data Analysis (EDA)
- **Visualization:**
  - **Distribution of Production Budgets:** Visualized to understand the spread and central tendencies.
  - **Domestic gross vs Worldwide gross:** To determine the market focus.
  - **Correlation Analysis:** Assessed the relationship between production budgets and worldwide gross.

#### Regression Analysis
Performed Ordinary Least Squares (OLS) regression to quantify the relationship between production budget and worldwide gross revenue.
- **R-squared:** 0.560, indicating that 56% of the variance in worldwide gross is explained by the production budget.
- **Key Coefficients:**
  - **Production Budget:** Positive significant impact on worldwide gross (coefficient = 3.1269).
  - **Intercept:** Negative, indicating potential baseline costs or factors not captured by the model.

#### Recommendations
**Optimal Budget:** Invest in movies within the optimal budget range that yields the highest return on investment.
**Genre Focus:** Prioritize genres that consistently perform well at the box office. This can include genres like action,adventure, or family movies.
**Quality Over Quantity:** Focus on improving both audience and critic ratings as higher ratings correlate with higher revenue.

#### Next Steps
1. **Data Collection:** Gather more data on other influencing factors like marketing budgets and release strategies.
2. **Advanced Modeling:** Utilize more sophisticated modeling techniques, including robust regression and machine learning, to capture complex relationships.
.
