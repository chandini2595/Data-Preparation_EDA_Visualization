## Air Quality Prediction Project

## Project Overview

This project aims to predict air quality by modeling CO(GT) levels based on environmental factors and pollutant levels in a public air quality dataset. Using AutoML tools, feature engineering, and advanced machine learning models, this project explores relationships among pollutants, meteorological data, and other air quality indicators.

## Dataset

The dataset includes air quality measurements, collected hourly from a city monitoring station. It includes the following key features:

	•	Date and Time: Timestamp information for each measurement.
	•	CO(GT): Target variable representing CO levels in mg/m³.
	•	Pollutant Sensors: Various sensor measurements for compounds such as NOx, NMHC, and O3.
	•	Meteorological Variables: Environmental measurements like temperature (T), relative humidity (RH), and absolute humidity (AH).

## Data Source

	•	The dataset was sourced from Kaggle, provided in CSV format.

## Data Preprocessing

	1.	Date-Time Parsing: Combined Date and Time columns into a single datetime index.
	2.	Missing Value Handling: Used forward fill and interpolation to handle minor missing data.
	3.	Unit Conversion: Converted European-style decimal commas to periods for numerical processing.
	4.	Filtering: Removed rows with negative CO(GT) values, which represent erroneous data.

## Exploratory Data Analysis (EDA)

EDA included visualizations such as time series plots, scatter plots, and correlation heatmaps to understand relationships among pollutants and meteorological conditions.

## Automated Machine Learning with AutoViML

For this project, AutoViML (Automated Variant Interpreter and Machine Learning) was used to automate key parts of the machine learning workflow:

	1.	Feature Selection: AutoViML automatically selected relevant features, reducing redundancy and improving model efficiency.
	2.	Model Training: Trained and compared various machine learning models, ultimately selecting the best-performing model.
	3.	Hyperparameter Tuning: Used RandomizedSearchCV for efficient tuning, optimizing model performance without extensive manual tuning.
	4.	Feature Reduction and Engineering: Employed feature engineering techniques and reduced the feature space based on importance.

AutoViML Parameters

	•	hyper_param: Set to ‘RS’ (Random Search) for efficient hyperparameter tuning.
	•	feature_reduction: Enabled to reduce the feature set and improve model performance.
	•	scoring_parameter: RMSE was chosen to prioritize models that minimize prediction error.

Using AutoViML allowed for streamlined model development, providing quick insights into the best-performing features and models.

## Modeling

The modeling process included various machine learning models tested through AutoViML, with performance evaluated using key metrics.

## Key Models Explored

	•	Linear Models
	•	Gradient Boosting Models (e.g., XGBoost, LightGBM)
	•	Ensemble Methods

## Evaluation

Model performance was evaluated with:

	•	Root Mean Squared Error (RMSE)
	•	Mean Absolute Error (MAE)
	•	R-squared (R²)
