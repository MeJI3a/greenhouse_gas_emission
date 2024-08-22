# Greenhouse Gas Emissions Analysis for New Zealand

## Project Overview
This project focuses on analyzing and visualizing greenhouse gas emissions data across different regions and sectors in New Zealand. The analysis is structured into four main chapters, each addressing a specific aspect of the dataset.

## Chapter 1: Data Cleaning and Preprocessing
- **Data Loading:** 
  - Loaded the raw greenhouse gas emissions data for New Zealand into a pandas DataFrame.
  
- **Data Cleaning:**
  - Converted data types where necessary (e.g., converting the `year` column to numeric).
  - Removed unnecessary or irrelevant columns.
  - Handled missing values and outliers using the Interquartile Range (IQR) method.
  - Used boxplots to identify and visualize outliers, then removed them based on a defined threshold to ensure data integrity.

- **Data Export:**
  - Cleaned data was saved to a CSV file for use in subsequent chapters.

## Chapter 2: Statistical Analysis
- **Descriptive Statistics:**
  - Calculated key statistical metrics (mean, median, standard deviation, etc.) for the dataset.
  - Generated descriptive statistics for each region in New Zealand over the years to understand emission patterns.

- **Data Visualization:**
  - Created histograms and boxplots to visualize the distribution of emissions across regions and years.
  - Developed a correlation matrix to explore relationships between variables, visualized through a heatmap.
  - Conducted a detailed analysis of emissions by ANZSIC descriptors (industrial sectors) and regions.

- **Regional Analysis:**
  - Visualized trends in emissions by region and sector in New Zealand, including bar charts and pie charts.

## Chapter 3: Advanced Visualizations
- **Multi-Visualization Dashboards:**
  - Developed comprehensive dashboards combining multiple charts (line plots, bar charts, pie charts, and heatmaps) to present a holistic view of the data.
  - Focused on highlighting regional emissions trends, sector contributions, and progress towards emission reduction goals in New Zealand.

- **Pairplot and Jointplot Visualizations:**
  - Utilized seaborn’s pairplot and jointplot functions to explore relationships between multiple variables.
  - Applied binning techniques to create more granular visualizations, enhancing insights into data distribution.

## Chapter 4: Advanced Analysis and Modeling
- **Time Series Analysis:**
  - Performed time series decomposition on regional emissions data to extract trend, seasonal, and residual components.
  - Visualized decomposed components to understand underlying patterns in emissions over time.
  - **Outcome:** The decomposition results showed no significant seasonal or residual components, indicating a lack of seasonal patterns or random fluctuations in the data.

- **Regression Modeling:**
  - Built a linear regression model to predict future emissions based on historical data.
  - Evaluated the model's performance using metrics such as Mean Absolute Error (MAE) and R-Squared.
  - **Outcome:** The model performed poorly, with a high MAE (148.66) and a negative R-Squared value (-0.004), suggesting that the linear model is not suitable for predicting emissions based solely on the year. This poor fit indicates that the emissions data may exhibit non-linear patterns or complexities not captured by a simple linear regression.

- **K-Means Clustering:**
  - Applied K-Means clustering to group regions in New Zealand based on their average emissions.
  - **Outcome:** The clustering identified three groups, but the differences between clusters were not as distinct as anticipated, indicating limited variation in emission levels across regions.

## Future Work
Potential extensions include exploring other machine learning models, conducting more advanced cluster analysis, and performing more granular sectoral analyses, particularly focusing on specific industries within New Zealand.
