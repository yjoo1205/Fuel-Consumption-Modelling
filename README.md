# Fuel Efficiency Analysis and Prediction for CDGE

ComfortDelgro Engineering (CDGE) is a subsidiary of ComfortDelgro, the largest vehicle maintenance and repair workshop in Singapore. CDGE offers services such as car maintenance, manufacturing, and vehicle parts delivery to private and partnered vendors. This project explores data related to their deliveries.

## Table of Contents

- [Project Overview](#project-overview)
- [Tools and Techniques](#tools-and-techniques)
- [Introduction](#introduction---fuel-consumption-model)
- [Datasets](#datasets)
- [Limitations](#limitations)
- [References](#references)

## Project Overview

This project has three main objectives:
1. Route optimization for enhanced fuel efficiency.
2. Enhanced visibility over delivery status for internal tracking and external clients.
3. Fuel consumption prediction to facilitate resource planning.

**Data Privacy Statement:** This project repository contains essential documents for demonstration purposes. To protect sensitive information, the original data has been replaced with dummy data. This ensures that no confidential data is exposed within this repository. The analysis presented here utilizes substitute dummy data for illustrative purposes.

**In light of confidentiality concerns, this repository exclusively showcases the application of predictive modeling techniques to a fuel consumption model.**

### Tools and Techniques

| Feature            | Tools & Techniques                      | Data                                 |
|-------------------|-----------------------------------------|--------------------------------------|
| Route Planner     | Techniques: Dijkstra, Rule-based Approach, Routing problem solution methods  <br> Tools: Google OR-Tools | Real delivery location history and/or simulated data of locations in Singapore. |
| Fuel Consumption Model | Techniques: Multiple regression, Ridge regression, Lasso regression <br> Tools: R-studio | Detailed historical delivery data |
| Telegram Chatbot  | Techniques: Data cleaning and visualization <br> Tools: Telegram Bot API, pandas, numpy, sklearn | Driver’s location |
| Driver Performance Dashboard | Tools: Power BI | Detailed Trip reports, Movement Reports |
| Microsoft Power Application | Tools: Microsoft Power Application, Python, Flask, ReactJs, Docker, Ms Azure | |

### Introduction - Fuel Consumption Model

Our analysis takes a two-pronged approach to the fuel consumption of trucks. The first model seeks relationships between independent variables affecting fuel consumption, providing actionable insights for better efficiency. The second model aims to predict future truck fuel consumption based on identified independent variables, enabling effective resource planning.

### Datasets

The dataset, provided by our sponsor, consists of truck data from February 2020 to February 2021. The dataset includes several reports:
- Detail Trip Report
- Movement Report
- Refuel Report
- Fuel Efficiency Report

While the data was user-friendly in Excel, data cleaning was necessary due to its interface origin. The dataset's limitations stem from the number of trucks and available metrics, making it suitable for fundamental analysis but limited in visualization and deeper insights.

### Limitations

1. The system only allows extraction of data from the past year, limiting our duration.
2. There are only four trucks, with three of the same make and model, and one smaller truck.
3. Some metrics are monthly, resulting in only 39 rows of data.
4. Many variables in different reports are repeated and irrelevant.

The provided data answers basic queries such as monthly fuel consumption or delivery events. However, it offers limited visualization and deeper insights.

## Analysis

### Summary Statistics & Findings

The project begins with summary statistics to provide an overview. Key findings include insights into fuel consumption patterns, idling time, and offense counts. Google Data Studio was used for intuitive data visualization. Notable findings include:

1. Fuel Consumption Patterns: Analysis shows specific vehicles with higher fuel consumption, guiding fuel management strategies.
2. Idling Time Impact: A significant historical spike in idling time was observed, suggesting operational improvements.
3. Offense Counts: A particular vehicle consistently recorded the most offenses, indicating the need for driver behavior interventions.

These insights lay the foundation for further investigations into relationships between fuel consumption and factors, along with predictive model development.

### Relationship Between Fuel Consumption and Independent Variables

This section explores the intricate relationship between fuel consumption and independent variables. Multivariate regression analysis identifies key variables significantly influencing fuel consumption. Notable findings include:

1. Total Duration Impact: Longer trip durations correlate with higher fuel consumption, emphasizing the need for optimized routing.
2. Offenses and Fuel Efficiency: Offenses like speeding and braking correlate with elevated fuel consumption rates.
3. Car Type Distinction: Vehicle type emerges as a significant variable, suggesting fuel efficiency varies with different car types.

These insights suggest strategies to enhance fuel efficiency within CDGE's fleet, including reducing trip durations, addressing driver behavior, and considering vehicle choices.

### Predictive Fuel Consumption Regression

This section delves into predictive modeling for fuel consumption. Techniques including best subset selection, cross-validation, and regularization were used to create a robust model. The primary goal is to equip CDGE with tools for informed decision-making and resource planning.

1. Variable Selection: Best subset selection identifies influential predictor variables for model construction.
2. Cross-Validation: Cross-validation refines and validates the model's ability to generalize to new data.
3. Regularization: Ridge and lasso regression prevent overfitting and fine-tune model performance.
4. Outcome: A multilinear equation decodes independent variables' relationships with fuel consumption, enabling proactive decisions.

An interactive Shiny application enhances accessibility, enabling dynamic engagement with the predictive model for strategic resource allocation.

## Limitations and Future Work

We acknowledge limitations, including dataset size, potential interaction effects, and the need for additional variables. Future work involves more data gathering, exploring predictor variables, and refining the model for increased accuracy.

### References

Microsoft Power Application: https://docs.microsoft.com/en-us/powerapps/
<br>Pandas: https://pandas.pydata.org/pandas-docs/version/0.15/tutorials.html
<br>NLP - NLTK Python Programming Tutorials: https://www.datacamp.com/community/tutorials/text-analytics-beginners-nltk
<br>Telegram Bot Framework: https://core.telegram.org/bots
<br>Creating Dashboard using Power BI Tool: https://docs.microsoft.com/en-us/power-bi/desktop-getting-started
<br>Optimization of Thermal Insulation and Regression Analysis of Fuel Consumption: https://www.sciencedirect.com/science/article/pii/S1877705814003154
