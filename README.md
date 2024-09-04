<img src="boombox.png"> <br>
<b>Notebook by Ritwik Raj</b>

## Focus Area
BoomBikes, a US-based bike-sharing provider, has experienced significant revenue declines due to the COVID-19 pandemic. With the easing of lockdown restrictions, the company seeks to regain its market position and boost profits by understanding and predicting the demand for shared bikes. To achieve this, BoomBikes has partnered with a consulting firm to analyze the factors influencing bike demand in the American market.

## Table of Contents
* [Objective](#Objective)
* [Steps Followed](#Stepsfollowed)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
* [License](#License)

### Objective
The primary objective of this analysis is to identify the key variables that significantly impact bike demand and to quantify their effects. By modeling these relationships, BoomBikes aims to gain insights into how different factors—such as weather conditions, seasonal trends, and user behavior—influence the daily demand for bikes. This understanding will enable the company to adjust its business strategies to better align with customer needs and optimize bike availability.

<b>About the dataset</b>
The dataset provided for this analysis contains extensive daily records of bike demand, along with various independent variables such as temperature, humidity, wind speed, and other meteorological data. The goal is to develop a predictive model that accurately captures the dynamics of bike demand, allowing BoomBikes to make data-driven decisions as they navigate the post-pandemic market.

A detailed Data dictionary is attached with the rest of the files . 

### Steps followed

1. Before building the model, convert numeric values like 'weathersit' and 'season' into categorical string values to avoid implying order where none exists. Consider retaining the 'yr' column, as it captures increasing demand trends over 2018 and 2019. The model should use 'cnt' as the target variable, representing total bike rentals, including both casual and registered users.

2. After model building and residual analysis, evaluate the model using the R-squared score on the test set with r2_score(y_test, y_pred). This step is crucial for assessing the model's performance.

## Conclusions

The model reveals that temperature, humidity, and windspeed are significant predictors of bike demand, with temperature having a strong positive effect and humidity and windspeed having negative effects. 

Seasonal and weather conditions also significantly impact bike demand.

Based on the analysis of the regression model, the company should focus on the following features to optimize bike-sharing operations:

Temperature (temp):
Focus: Implement strategies to maximize bike availability and marketing efforts during warmer temperatures, as higher temperatures significantly boost bike demand.

Humidity (hum):
Focus: Monitor humidity levels and adjust bike-sharing operations accordingly. Since higher humidity negatively impacts demand, the company might consider promoting bike-sharing options or providing amenities to mitigate the effects of high humidity.

Windspeed (windspeed):
Focus: Be aware of the impact of windspeed on bike demand. During high wind conditions, demand decreases, so the company could consider special promotions or operational adjustments on windy days.

Seasonal Variations (summer, winter):
Focus: Adjust bike availability and marketing strategies based on the season. The model indicates higher demand during summer and winter, so the company should ensure adequate bike supply and tailored marketing during these seasons.

Weather Conditions (mist, snow or rain):
Focus: Prepare for lower bike demand during misty or snowy/rainy weather by optimizing bike distribution and implementing targeted promotions to encourage usage despite adverse conditions.

By focusing on these features, BoomBikes can better align their operations with factors that influence bike demand, improving service efficiency and potentially increasing revenue.

## Technologies Used
- Pandas - version 2.2.2
- NumPy - version 1.26.4
- Seaborn - version 0.13.2
- MatplotLib - version 3.9.1

## Acknowledgements
This project was inspired by UpGrad and IIITB Programme as a case study for the Machine Learning and Artificial Intelligence course.

### License

Use of this dataset in publications must be cited to the following publication:

[1] Fanaee-T, Hadi, and Gama, Joao, "Event labeling combining ensemble detectors and background knowledge", Progress in Artificial Intelligence (2013): pp. 1-15, Springer Berlin Heidelberg, doi:10.1007/s13748-013-0040-3.

@article{
	year={2013},
	issn={2192-6352},
	journal={Progress in Artificial Intelligence},
	doi={10.1007/s13748-013-0040-3},
	title={Event labeling combining ensemble detectors and background knowledge},
	url={http://dx.doi.org/10.1007/s13748-013-0040-3},
	publisher={Springer Berlin Heidelberg},
	keywords={Event labeling; Event detection; Ensemble learning; Background knowledge},
	author={Fanaee-T, Hadi and Gama, Joao},
	pages={1-15}
}

Contact	
For further information about this dataset please contact Hadi Fanaee-T (hadi.fanaee@fe.up.pt)
