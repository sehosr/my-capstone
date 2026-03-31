# my-capstone
A capstone project applying data cleaning, feature engineering, EDA, and math concepts on the Ames Housing dataset to understand house prices.

## Phase 1 — Data Cleaning
During this phase, I prepared the dataset for analysis by handling missing values using median for numerical columns and "Unknown" for categorical ones. I also corrected data types, such as converting categorical codes into strings. To manage extreme values, I capped outliers in SalePrice at the 99th percentile. Finally, I verified the data quality by checking for duplicates and ensuring there were no missing or invalid values in key columns.

## Phase 2 — Feature Engineering
In this phase, I enhanced the dataset by creating new features such as price_per_sqft and bathroom_ratio to provide more meaningful insights. I also created an interaction feature (quality_x_area) to capture the combined effect of size and quality. Categorical variables were encoded using one-hot and ordinal encoding. Additionally, I applied scaling to numerical features and used log transformation to reduce skewness and improve data distribution.

## Phase 3 — Exploratory Data Analysis (EDA)
During the EDA phase, I observed several important patterns in the data. The distribution of SalePrice was right-skewed, indicating that most houses are in the lower price range with a few very expensive properties. The boxplots showed that higher quality houses tend to have significantly higher prices. The scatter plot revealed a strong positive relationship between living area and SalePrice, meaning larger houses are generally more expensive. The correlation heatmap confirmed that Overall Quality and Gr Liv Area are among the most influential features affecting price. Additionally, the groupby analysis showed that houses with higher overall quality have the highest average prices.

## Phase 4 — Math Foundations
In this phase, I applied basic mathematical concepts to support the analysis. I calculated the mean and standard deviation of SalePrice manually using NumPy. Then, I standardized a numerical feature using the formula (X - mean) / std and compared the results with StandardScaler to ensure correctness. I also computed cosine similarity between the highest and lowest priced houses to measure similarity. Finally, I estimated a probability to understand how often high-quality houses exceed a certain price threshold.
