## NYC Taxi Fare Prediction Analysis
Overview
This project analyzes NYC Yellow Taxi trip data to predict fare amounts using AutoML and traditional machine learning approaches. We explore trip patterns, fare relationships, and predictive modeling through comprehensive data analysis and visualization.
Dataset
We used the NYC Yellow Taxi Trip Data sample containing:

Pickup/dropoff timestamps
Trip distances
Fare amounts
Passenger counts
Payment types
Rate codes

Analysis Pipeline
1. Exploratory Data Analysis & Visualization
Created comprehensive visualizations to understand patterns in:
Basic Trip Metrics

Trip distance vs fare amount relationships
Average fare variation by hour
Trip duration distributions
Payment type breakdowns

Temporal Patterns

Trip frequency by day of week
Average fare patterns by day
Hourly demand variations
Monthly trends

Fare Analysis

Overall fare distribution
Impact of passenger count on fares
Rate code influence
Cost per mile patterns

Distance and Duration Analysis

Trip distance patterns
Speed variations
Duration trends by time of day

2. Data Preprocessing
Implemented comprehensive data preparation:

Feature engineering from timestamps
Trip duration calculations
Outlier removal
Feature scaling and normalization
Categorical variable encoding

3. AutoML Implementation
Used PyCaret for automated machine learning:

Automated feature selection
Model comparison and selection
Hyperparameter tuning
Ensemble model creation
Performance evaluation

Results
Model Performance
The analysis generated multiple models with:

Comparison of regression algorithms
Cross-validation results
Feature importance rankings
Prediction accuracy metrics

Key Findings

Trip Patterns:

Identified peak hours and busy days
Found common trip durations
Analyzed speed patterns


Fare Insights:

Strong correlation between distance and fare
Time of day impact on pricing
Payment method preferences


Model Performance:

Achieved competitive RMSE scores
Identified most important predictive features
Successfully handled categorical variables



Dependencies

pandas
numpy
scikit-learn
matplotlib
seaborn
pycaret 
