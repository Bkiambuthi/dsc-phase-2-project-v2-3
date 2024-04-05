# UNDERSTANDING KING COUNTY’S HOUSING MARKET

## Introduction

The project aims to find important insights as we explore the huge world of real estate that will aid in the comprehension of the dynamics of the housing market in King County.
We will walk you through each step of the process of developing and assessing our linear regression model and go over the main factors that affect home values, talk about the issues with linear regression, and use analysis and visualizations to show off our model's ability to predict outcomes.By the end of the presentation, we hope to provide insights that can  be used in similar datasets , in addition to demystifying the complexity of real estate prediction. 

![WhatsApp Image 2024-04-05 at 21 50 57_c564785e](https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/assets/151352438/9de60684-8a05-454a-9b2a-ecb800401b73)


### Business Problem
The management of a startup real estate company seeks to understand the key factors influencing housing prices in King County. Their capacity to develop focused actions and activities to support housing affordability and fair access to housing is limited by a lack of data-driven insights.

### The Data

This project uses the King County House Sales dataset, which can be found in  `kc_house_data.csv` in the data folder in this project's GitHub repository. The description of the column names can be found in `column_names.md` in the same folder. 


### Project Goals
The project aims to use CRISP-DM data science methodology to fit and select the best regression model that will predict housing prices. The resultant model will be used by the real estate company to price housing units so as to attract customers and optimize their sales.

### Methods
Linear regression analysis will be used to find the relationship between sales prices and various house features other factors.

![image](https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/assets/151352438/8cafe8af-4b2b-4644-b6e1-02d5fb3f20ca)

### Results
When using linear regression there are four assumptions that need to be followed:

      .Linearity - relationship between predictor and target should be linear.

      .Independence - Observations are independent from each other, low or no multicollinearity.

      .Normality - Errors should be normally distributed.

      .Homoscedasticity - variance or the errors is the same.

1.Checking the relationships amongst all the variables in our data set

<img width="579" alt="image" src="https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/assets/151786633/4521570b-0ca8-4ea9-a236-ddb596d6eb2c">

2. Fitting our baseline model using sqft_living as the independent variable and price as the dependent variable.
Sqft_living has the highest correlation with price.

<img width="294" alt="image" src="https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/assets/151786633/51669624-a8c0-4b39-ab0f-a5ae47c9cf84">

The model is explaining 49.3% of the change in price.

Equation for our model Price = 280.86X - 43988.89

<img width="431" alt="image" src="https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/assets/151786633/5dc87bb1-d1ab-4460-bf2c-d9d1283b86c1">

<img width="437" alt="image" src="https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/assets/151786633/0c36eef8-132d-41d2-8ec5-203ed3916e45">

3. Multiple linear regression
 <img width="269" alt="image" src="https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/assets/151786633/4a1345d5-d76b-4656-b521-771064ec43f7">
 
 The model is explaining 64% of the change in price.

 <img width="577" alt="image" src="https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/assets/151786633/b450f7ef-0307-41dd-99be-1bd44deb8d68">

 4. Polynomial regression
Using 3-degree polynomial regression, the model yielded the highest score.
The results were as below:

      Mean Squared Error (MSE)  192833.78

      R-squared (training)  0.738

      R-squared (testing)  0.731

### Conclusion

Square footage of living space in the home is the highest determinant in house pricing.

The other factors included

Construction and design of the house

Number of floors

Number of bedrooms

Quality of view from house

Location

### For More Information
Please review our full analysis in our [Jupyter Notebook](https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/blob/main/student.ipynb) or our [presentation](https://github.com/Bkiambuthi/dsc-phase-2-project-v2-3/blob/main/Understanding%20King%20County's%20Housing%20Market.pdf).




   






