# Rainfall Prediction Project

## Project Description

This project focuses on predicting rainfall in Austin, Texas using machine learning techniques. The goal is to analyze weather patterns and create a model that can predict precipitation levels based on various weather parameters.

## Dataset

- **File:** austin_weather.csv
- **Location:** Austin, Texas
- **Records:** 1,319 weather observations
- **Features:** 21 weather parameters
- **Target:** PrecipitationSumInches

## Features Used

The model uses the following weather parameters:
- Temperature (High, Average, Low)
- Dew Point (High, Average, Low) 
- Humidity (High, Average, Low)
- Sea Level Pressure (High, Average, Low)
- Visibility (High, Average, Low)
- Wind Speed (High, Average, Gust)

## Methodology

### Data Preprocessing
1. **Data Loading:** Imported the CSV file using pandas
2. **Data Cleaning:** 
   - Handled missing values
   - Converted special characters ('T' for trace, '-' for missing)
   - Converted string columns to numeric
3. **Feature Selection:** Selected 18 relevant weather features
4. **Data Scaling:** Applied StandardScaler for normalization

### Model Development
- **Algorithm:** Linear Regression
- **Data Split:** 80% training, 20% testing
- **Cross-validation:** Random state = 42

### Evaluation Metrics
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE) 
- R-squared (R²) Score

## Analysis Steps

1. **Data Exploration**
   - Checked data types and missing values
   - Analyzed unique values in precipitation column
   - Examined dataset structure

2. **Data Visualization**
   - Precipitation trends over time
   - Distribution of precipitation values
   - Scatter plots of weather parameters vs precipitation
   - Monthly precipitation patterns
   - Correlation matrix heatmap

3. **Model Training**
   - Split data into training and test sets
   - Scaled features using StandardScaler
   - Trained Linear Regression model
   - Generated predictions

4. **Model Evaluation**
   - Calculated performance metrics
   - Created actual vs predicted plots
   - Analyzed residuals
   - Identified feature importance

## Results

### Model Performance
- Training R² Score: [Your Value]
- Test R² Score: [Your Value]
- Test RMSE: [Your Value] inches

### Key Findings
- [Your findings about feature importance]
- [Your findings about correlations]
- [Your findings about seasonal patterns]

## Files Included

- `rainfall_prediction.ipynb` - Main Jupyter notebook with complete analysis
- `1.ipynb` - Alternative implementation
- `austin_weather.csv` - Dataset file
- `README.md` - Project documentation

## How to Run

1. Install required libraries:
```bash
pip install pandas numpy matplotlib scikit-learn
```

2. Download all files to the same directory

3. Open `rainfall_prediction.ipynb` in Jupyter Notebook

4. Run all cells sequentially

## Visualizations

The project includes the following visualizations:
- Time series plot of precipitation
- Histogram of precipitation distribution
- Scatter plots of weather parameters vs precipitation
- Monthly precipitation bar chart
- Correlation matrix heatmap
- Actual vs predicted plots
- Residuals plot
- Feature importance bar chart

## Technical Details

### Libraries Used
- pandas - Data manipulation
- numpy - Numerical operations
- matplotlib - Data visualization
- scikit-learn - Machine learning

### Data Processing
- Missing value imputation using mean
- Special character handling
- Feature scaling
- Data type conversion

## Conclusions

This project successfully demonstrates:
- Data preprocessing techniques
- Exploratory data analysis
- Linear regression modeling
- Model evaluation and interpretation
- Weather pattern analysis

The Linear Regression model provides a baseline understanding of rainfall prediction using weather parameters. The model can be improved with more advanced algorithms and additional features.

## Future Improvements

1. **Advanced Models:** Try Random Forest, XGBoost, or Neural Networks
2. **Feature Engineering:** Add lag features and seasonal indicators
3. **Hyperparameter Tuning:** Use grid search for optimization
4. **Ensemble Methods:** Combine multiple models
5. **Real-time Data:** Integrate with live weather APIs

## Author

[Your Name]
Module 13 - Rainfall Prediction Project
[Your Institution]

---

*This project was created for educational purposes as part of the Module 13 assignment.* 