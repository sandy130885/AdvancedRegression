House Price Prediction Using Advanced Regression
> Outline a brief description of your project.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.
- The company wants to know:

Which variables are significant in predicting the price of a house, and

How well those variables describe the price of a house.
- Data set train is used

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- CMonth (House) Sold: June, followed by July and May
MSSubClass: Most preferred type of dwelling involved is 20 i.e. 1-Story 1946 & Newer All Styles, followed by 60 i.e. 2-Story 1946 & Newer.
Overall Quality (material and finish): Average and Above Average
Overall Condition: Mostly Average, followed by Above Average
(i) Basement Full Bathrooms: Maximum 0(None), followed by 1.
(ii) Full Bathrooms: Preferred 2, followed by 1 and (iii) Half Bathrooms: Preferred 0(None), followed by 1.
Bedrooms Above Ground:3, followed by 2.
Total Rooms Above Ground: 6, followed by 7.
No significant preferences for Fireplaces (0 0r 1) and WhetherRemodelled (House) or not.
GarageCars space: 2 car spaces, followed by 1 car space
- '1stFlrSF','GrLivArea' show a positive correlation with the SalePrice.
Other continuous variables are too scattered. Let's understand them from further analysis.
SalePrice vs ('LotFrontage', 'MasVnrArea', '1stFlrSF', and 'GarageArea' scatterplots do have some datapoints with some eccentric values/outliers. Let's eliminate them first.
- (1)The predictors 'GrLivArea' and 'TotRmsAbvGrd' shows (0.83) strong positive correlation. Hence, dropping 'TotRmsAbvGrd'. (2)The predictors 'GarageCars' and 'GarageArea' shows (0.89) strong positive correlation. Hence, dropping 'GarageCars'. (1)The predictors 'GrLivArea' and '2ndFlrSF' shows (0.72) strong positive correlation. Hence, dropping '2ndFlrSF'. (2)The predictors '1stFlrSF' and 'TotalBsmtSF' shows (0.77) strong positive correlation. Hence, dropping '1stFlrSF'.
- Ridge and Lasso Regression both perform well on the model

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- library - version 1.0
- library - version 2.0
- library - version 3.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->