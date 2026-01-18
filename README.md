# D.C_Bike_Rental_Data

📊 Description of the Bike Rental Analysis Code
This Jupyter Notebook performs an exploratory data analysis (EDA) on the Bike Sharing Demand dataset (from Kaggle) to understand patterns and trends in bike rentals over time, user types, weather, and working days.
1. Data Acquisition
Uploads a Kaggle API token and configures the environment.
Downloads the Bike Sharing Demand competition dataset from Kaggle.
Unzips the dataset and loads the train.csv file into a Pandas DataFrame.
2. Data Preparation & Cleaning
Converts the datetime column into a proper datetime format.
Checks:
Data types
Number of rows
Missing values
Extracts new time-based features from datetime, including:
year
month
day
dayofweek
hour
Converts numeric season codes into readable labels:
Spring, Summer, Fall, Winter
3. Exploratory Data Analysis (EDA)
The notebook answers a series of analytical questions using grouping, aggregation, and visualization:
🔹 Rental Trends
Total rentals by year
Monthly rental patterns for 2011 vs 2012
Daily rental trends over time (line plot)
🔹 User Behavior
Compares casual vs registered users
Shows that:
Registered users dominate rentals on working days
Casual users rent more on non-working days
Analyzes hourly rental behavior for both user types
🔹 Seasonal & Weather Insights
Identifies Fall as the season with the highest average rentals
Analyzes rentals by weather condition to find:
Highest rental weather
Lowest rental weather
🔹 Hourly Patterns
Determines:
Busiest hours (e.g., 5 PM, likely commuting time)
Quietest hours of the day
Creates pivot tables to compare rentals by:
Hour
Working vs non-working days
4. Correlation Analysis
Computes correlations between numerical features and total rental count.
Identifies which variables most strongly influence bike rentals.
5. Visualizations
Line plots for:
Daily rental trends
Hourly rental patterns by user type
These plots help highlight commuting behavior and long-term usage trends.
✅ Overall Purpose
The notebook is designed to:
Understand when and why bikes are rented
Compare behavior across time, seasons, weather, and user types
Provide data-driven insights useful for demand forecasting or model building later
