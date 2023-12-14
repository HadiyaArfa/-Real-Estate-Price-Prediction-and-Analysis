# -Real-Estate-Price-Prediction-and-Analysis
**Project Title: Real Estate Price Prediction and Analysis**
**Objective:**
The primary goal of this project is to develop a multi-model machine learning approach to predict real estate prices based on various features. Additionally, the project aims to conduct a thorough analysis of real estate data, providing valuable insights for potential buyers, sellers, and investors.

**Summary:**
This project follows a systematic process, starting from data collection and preprocessing to building predictive models and conducting exploratory data analysis (EDA). The outcome includes predictive models for estimating housing prices and insightful analyses to empower stakeholders in making informed decisions.

Tools and Libraries: pandas: Data manipulation and analysis. seaborn: Data visualization. numpy: Numerical operations. matplotlib: Plotting visualizations. scikit-learn: Machine learning models and tools.

Data Loading and Preprocessing: Loaded real estate data from the provided CSV file. Removed unnecessary columns, such as 'Property ID'. Handled missing values, replacing them in the 'Amenities' column with 'None'.

Feature Engineering: Transformed the 'Location' and 'Amenities' text-based features into a structured format using one-hot encoding. Created binary columns for each unique location and amenity. Addressed the dummy variable trap by dropping one column for each feature.

Model Building: Extracted features (X) and the target variable (y). Split the data into training and testing sets. Utilized a RandomForestRegressor for initial model fitting. Assessed the model's performance using the R-squared score.

Cross-Validation: Employed K-Fold cross-validation to measure the accuracy of the Linear Regression model. Utilized ShuffleSplit to randomize folds equally for each sample.

Model Comparison: Employed GridSearchCV to find the best hyperparameters for various regression models (Linear Regression, Lasso, Decision Tree, and Random Forest). Created a bar plot to visually compare the best scores achieved by each model.

Best Model Selection: Determined that the RandomForestRegressor yielded the highest score. Concluded to use the RandomForestRegressor for further analysis.

Property Price Prediction: Created a function to predict property prices based on location, square footage, bathrooms, bedrooms, and amenities. Tested the prediction function on different property scenarios.
