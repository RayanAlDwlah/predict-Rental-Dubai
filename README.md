# Predict Rental Dubai

## Project Overview
This project aims to analyze and predict rental prices for properties in Dubai using machine learning techniques. The data consists of various property details, including address, rent, number of bedrooms and bathrooms, type of property, area in square feet, rent per square foot, and more.

## Dataset
The dataset `dubai_properties.csv` contains information about properties in Dubai, including:
- Address
- Rent
- Beds
- Baths
- Type
- Area_in_sqft
- Rent_per_sqft
- Rent_category
- Frequency
- Furnishing
- Purpose
- Posted_date
- Age_of_listing_in_days
- Location
- City
- Latitude
- Longitude

## Data Preprocessing
- Loaded the dataset using Pandas.
- Checked for missing values and data types.
- Converted the `Posted_date` column to datetime and extracted `Year`, `Month`, and `Day`.
- Dropped unnecessary columns like `Frequency`, `Purpose`, and `Address`.

## Exploratory Data Analysis (EDA)
- Performed basic data exploration using `df.head()`, `df.tail()`, and `df.info()`.
- Visualized the distribution of rent categories using pie charts and count plots.
- Examined the value counts for categorical columns.

## Data Cleaning
- Handled missing values in the `Latitude` and `Longitude` columns.
- Encoded categorical columns using one-hot encoding.

## Visualization
- Plotted the distribution of rent categories.
- Created a count plot for rent categories with respect to the rent values.

## Model Building and Evaluation
- Utilized various machine learning models, including Random Forest, for predictions.
- Random Forest was found to be the best-performing model.
- Trained the Random Forest model and evaluated its performance.

## Random Forest Model Performance
The Random Forest model provided the best results among the tested models, showing high accuracy and robustness in predicting rental prices based on the provided features. Details of the model's performance can be found in the `model.ipynb` notebook.

## Future Work
- Further tuning of hyperparameters for better model performance.
- Deploy the model for real-time predictions.

## Conclusion
This project provides a comprehensive overview of the rental market in Dubai and sets the foundation for building predictive models to estimate rental prices based on various property features.

## Code
The code for data preprocessing, visualization, and initial exploration is provided in the `model.ipynb` notebook. Further steps for model building and evaluation are to be added.

## Repository
You can find the complete project repository [here](https://github.com/RayanAlDwlah/predict-Rental-Dubai).

## Author
- LinkedIn: [Rayan Saleh](https://www.linkedin.com/in/rayan-saleh-b12a3132a)
- GitHub: [RayanAlDwlah](https://github.com/RayanAlDwlah)

Feel free to explore the notebook and contribute to the project!
