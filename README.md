# Predict Rental Prices in Dubai

## Project Overview
This project focuses on analyzing and predicting rental prices for properties in Dubai using advanced machine learning techniques. The dataset includes detailed property information such as location, rent, property type, and other relevant features. The goal is to provide insights into the rental market and build a predictive model for estimating rental prices.

## Dataset Description
The dataset `dubai_properties.csv` contains the following features:
- **Address**: Property address.
- **Rent**: Rental price of the property.
- **Beds**: Number of bedrooms.
- **Baths**: Number of bathrooms.
- **Type**: Type of property (e.g., Apartment, Villa).
- **Area_in_sqft**: Property area in square feet.
- **Rent_per_sqft**: Rent per square foot.
- **Rent_category**: Categorized rent levels (Low, Medium, High).
- **Frequency**: Payment frequency (e.g., Yearly).
- **Furnishing**: Furnishing status (Furnished/Unfurnished).
- **Purpose**: Purpose of the listing (e.g., For Rent).
- **Posted_date**: Date the property was listed.
- **Age_of_listing_in_days**: Age of the listing in days.
- **Location**: Specific location of the property.
- **City**: City where the property is located.
- **Latitude**: Latitude coordinates of the property.
- **Longitude**: Longitude coordinates of the property.

## Key Steps in the Project

### Data Preprocessing
- Loaded the dataset using Pandas and performed initial exploration.
- Checked for missing values and handled them appropriately.
- Converted the `Posted_date` column to datetime format and extracted `Year`, `Month`, and `Day`.
- Dropped irrelevant columns such as `Frequency`, `Purpose`, and `Address`.

### Exploratory Data Analysis (EDA)
- Conducted a detailed analysis of the dataset using descriptive statistics.
- Visualized the distribution of rental categories using pie charts and count plots.
- Analyzed categorical features and their relationships with rental prices.

### Feature Engineering
- Created new features from existing ones, such as extracting date components.
- Encoded categorical variables using techniques like one-hot encoding and binary encoding.
- Scaled numerical features using robust scaling to handle outliers.

### Model Building and Evaluation
- Split the dataset into training and testing sets.
- Trained multiple machine learning models, including:
    - **Linear Regression**
    - **Decision Tree Regressor**
    - **Random Forest Regressor**
- Evaluated model performance using metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), and R² Score.
- The **Random Forest Regressor** outperformed other models, providing the most accurate predictions.

### Visualization
- Plotted histograms and box plots to analyze numerical features.
- Visualized outliers and distributions of key features.
- Created count plots to explore categorical data.

## Results
The **Random Forest Regressor** demonstrated the best performance, achieving high accuracy and robustness in predicting rental prices. The model effectively utilized the provided features to estimate rental values.

## Future Enhancements
- Perform hyperparameter tuning to further improve model accuracy.
- Explore additional machine learning models and ensemble techniques.
- Deploy the model as a web application for real-time rental price predictions.

## Repository
The complete project, including the dataset and code, is available in the [GitHub repository](https://github.com/RayanAlDwlah/predict-Rental-Dubai).

## Author
- **LinkedIn**: [Rayan Saleh](https://www.linkedin.com/in/rayan-saleh-b12a3132a)
- **GitHub**: [RayanAlDwlah](https://github.com/RayanAlDwlah)

Feel free to explore the repository, review the code, and contribute to the project!
