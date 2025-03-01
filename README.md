# Asteroid Classification Data Analytics Report
## Introduction
This report explores the data preprocessing, feature engineering, and analysis techniques used to classify asteroid data. The key focus is on preparing the data, handling missing values, performing feature engineering, and validating data conversions.
## Handling Missing Values
Missing values are handled by conversions and backtracking. Various imputation methods, such as interpolation, are used to fill gaps in the dataset. For example, relative velocities in kilometers per hour were filled using corresponding values in miles per hour.
## Feature Engineering
Several features were engineered from the original dataset. One key example is the "time until approach," which was calculated by converting the epoch date close approach into a datetime format and finding the difference between the current date and the approach date.
## Data Validation
To ensure the accuracy of unit conversions, the dataset was validated by comparing calculated values for relative velocity in different units. Any discrepancies were found to have a negligible error margin.
## Data Exploration
During the initial exploration of the dataset, summary statistics such as mean, median, and standard deviation were calculated for key numerical features like "Miss Distance", "Relative Velocity", and "Semi-major Axis". Feature distributions were visualized using 'histograms and box plots to gain an understanding of the spread and skewness of the data. 'Additionally, correlations between features were calculated using Pearson correlation coefficients to identify relationships between variables.
## Model Performance
Several machine learning models were tested to classify asteroids based on the provided features. These models included Logistic Regression, Decision Trees, and Random Forests. Performance metrics such as accuracy, precision, recall, and F1-score were used to evaluate the models. Among the tested models, Random Forest achieved the best performance, with an accuracy of over 90% and a balanced precision and recall score. Feature selection and hyperparameter tuning further improved the model’s performance.

## Visualizations
The relationship between key features, such as miss distance and semi-major axis, was explored using visualizations like scatter plots and pair plots. These plots help understand the correlations between different orbital properties.
 
This is the correlation matrix of different columns for extraction of features and establishing relations to fill in more missing values.
BoxPlots were also plotted to detect outliers in different columns.
 
This is the pairplot that relates different features using scatter plots and also shares information regarding skewness and normalization values.
## Conclusion
In conclusion, the preprocessing and feature engineering steps ensure the dataset is ready for classification. Further steps include applying machine learning models to classify asteroids based on their potential hazard level.
