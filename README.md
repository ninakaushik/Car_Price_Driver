# Car_Price_Driver
Link to Jupyter notebook:

Vehicle Pricing Analysis

This project analyzes a dataset of used vehicles to identify key drivers of resale value and evaluate predictive models for vehicle pricing. The goal is to support informed decision-making for vehicle purchasing, pricing, and inventory strategy.

# Dataset

The dataset contains vehicle listings with features such as: Price, Odometer reading, Year, Manufacturer, Vehicle type, Condition

# Data Cleaning & Feature Engineering

Removed irrelevant columns: Columns with little predictive value or high missingness were dropped.

Dropped incomplete rows: Any rows missing key values like price or odometer were removed.

Outlier removal: Extreme price outliers were removed to improve model stability.

# Feature creation:

log_price and log_odometer for variance stabilization

age calculated from the vehicle year

# Exploratory Data Analysis

Key features were visualized to understand their distributions and relationships with price.

# Modeling Approach

Three models were evaluated:, Linear Regression, Lasso Regression, Ridge Regression

Models were trained to predict both price and log_price.

# Results

Test RMSE: ~$8,930

This error is reasonable given the wide price range ($1,000–$100,000).

Log-transformed models: Stabilized variance and improved interpretability

Lasso Regression: Slightly lower accuracy, indicating many small but meaningful features contribute to price prediction.

# Key Price Drivers

The models consistently identified the following as major drivers of price: Age of the vehicle, Odometer reading, Manufacturer, Condition grade, Vehicle type

# Business Insights & Recommendations

For maximizing profitability, dealers should prioritize:

Low Mileage Vehicles
Newer Models: higher ROI
Strong Manufacturers: Toyota, Honda, Lexus, Mercedes, BMW retain value better
Better Condition Grades: Good to like-new vehicles yield meaningful price increases
High-Demand Vehicle Types: Trucks and SUVs provide stronger resale values

#Next Steps:
Buy low mileage, high-condition units whenever possible
Emphasize stocking high-retention brands
Be selective with poor-condition vehicles 
Favor trucks and SUVs for stronger resale margins

Conclusion
The analysis and predictive modeling provide a stable, generalizable framework for understanding vehicle pricing. Dealers can leverage these insights to make data-driven inventory and pricing decisions.
