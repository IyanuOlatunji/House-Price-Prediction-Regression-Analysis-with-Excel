# House-Price-Prediction-Regression-Analysis-with-Excel

## Introduction
Being able to predict house prices accurately is really important for everyone involved. People looking to buy can make smart offers, and sellers can feel confident about setting the right price for their home. By studying all these different factors using a method called regression analysis, we can learn important things and stay on top of how the housing market is changing.
In this project, I would be using excel to perform a regression analysis on US housing dataset. The aim of this project is to predict the "price" based on other house features in the US.

## Dataset Preparation
- The dataset was gotten from Kaggle, and it contains 5000 records and 7 fields namely price, Avg. Income, Avg. Area House Age, Avg. Area Number of Rooms, Area Population, Avg. Area Number of Bedrooms, and Address.
- Before conducting the regression analysis, the dataset was examined for null values and blanks, and none were found.
- Descriptive statistics were computed for all variables to gain insights into their distributions. It provided valuable information about the central tendency, dispersion, and shape of each variable's distribution.
- Overall, the descriptive statistics indicated that the variables in the dataset exhibit relatively symmetrical distributions, with skewness values close to zero. The standard deviations and variances vary across variables, suggesting differing levels of dispersion in the data.

![image](https://github.com/IyanuOlatunji/House-Price-Prediction-Regression-Analysis-with-Excel/assets/135010390/3473a9a7-b59e-4aaf-9915-18f5a3b7f050)

- Further analysis involved checking for linearity between the dependent variable (Price) and independent variables (Avg. Income, Avg. Area House Age, Avg. Area Number of Rooms, Area Population, Avg. Area Number of Bedrooms) using scatter plot charts. It was observed that only Avg. Area Number of Bedrooms did not exhibit a linear relationship with the dependent variable and was consequently dropped from the analysis.

![image](https://github.com/IyanuOlatunji/House-Price-Prediction-Regression-Analysis-with-Excel/assets/135010390/5cdb15de-5b51-4bdb-a23f-40eb946b68a9)

![image](https://github.com/IyanuOlatunji/House-Price-Prediction-Regression-Analysis-with-Excel/assets/135010390/346b4d74-12a7-426e-a8f0-175afd4a0cac)
![image](https://github.com/IyanuOlatunji/House-Price-Prediction-Regression-Analysis-with-Excel/assets/135010390/e288395c-aec8-4ca9-86ad-6025d56d5519)


## Multicollinearity Check
To ensure the independence of predictors, multicollinearity was assessed using the Variance Inflation Factor (VIF). VIF values were calculated for each independent variable, with all values falling within acceptable ranges, indicating no significant multicollinearity issues.

![image](https://github.com/IyanuOlatunji/House-Price-Prediction-Regression-Analysis-with-Excel/assets/135010390/36857020-81e3-4f5d-9870-f46934514711)

## Regression Analysis Interpretation 
The regression analysis revealed
- Multiple R value of 0.95 which indicates a strong positive relationship between housing prices and the independent variables, with an R-squared value of 0.918, indicating that approximately 91.8% of the variability in housing prices can be explained by the independent variables. 
- All independent variables included in the model, Average Income, Average Area House Age, Average Area Number of Rooms, and Area Population were found to be statistically significant predictors of housing prices. Therefore, this model can be utilized to predict housing prices based on these factors.
- The Linear Regression Model Equation is given as Dependent variable Price = -2637560.673 + 21.58274357(Avg. Area Income) + 165657.8724(Avg. Area House Age) + 121598.1646(Avg. Area Number of Rooms) + 15.19611982(Area Population) 
- Upon application of the regression model, The actual housing prices were found to be lower than the predicted prices. This suggests potential limitations or inaccuracies in the regression model's predictive capabilities. It indicates that the model may have overestimated the value of the houses based on the independent variables considered.

## Recommendation
Further analysis should be pursued to uncover additional variables or data sources that could more effectively capture the nuances of the housing market. Moreover, validating the model through alternative methodologies using appropriate metrics, such as mean squared error (MSE) can enhance its reliability and applicability.
