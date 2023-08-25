# CDGE_modelling
Our Sponsor, ComfortDelGro Engineering Pte Ltd (CDGE) is Singapore’s largest one-stop vehicle maintenance and repair workshop that offers services such as car maintenance, manufacturing, and delivery of vehicle parts for both private and partnered vendors.

## Table of Contents
- [Project Overview](#project-overview)
- [Tools and Techniques](#tools-and-techniques)
- [References](#references)


## Project Overview

This project has 3 main goals:
1) Route optimization to ensure best fuel efficiency
2) Visibility over delivery status for both internal tracking and external clients
3) Fuel prediction to facilitate resource planning

Data Privacy Statement: This project repository contains essential documents intended for demonstration purposes. To safeguard sensitive information, the original data has been replaced with dummy data. This measure ensures that no confidential data is accessible within this repository. The analysis presented here is conducted using the substitute dummy data for illustrative purposes.

### Tools and Techniques

| Feature | Tools & Techniques | Data |
|------------|-----------------------------|------------------------------|
|Route Planner   |Techniques: Dijkstra, Rule-based Approach, Routing problem solution methods  <br> Tools: Google OR-Tools |Real delivery location history and/or simulated data of locations in Singapore. |
|Fuel Consumption Model|Techniques: Multiple regression, Ridge regression, Lasso regression <br> Tools: R-studio |Detailed historical delivery data|
|Telegram Chatbot  |Techniques: Data cleaning and visualisation <br>Tools: Telegram Bot API, pandas, numpy, sklearn |Driver’s location |
|Driver Performance Dashboard  |Tools: Power BI  |Detailed Trip reports, Movement Reports |
|Microsoft Power Application |Tools: Microsoft Power Application, Python, Flask, ReactJs, Docker, Ms Azure | |

### References

Microsoft Power Application https://docs.microsoft.com/en-us/powerapps/
<br>Pandas https://pandas.pydata.org/pandas-docs/version/0.15/tutorials.html
<br>NLP - NLTK Python Programming Tutorials https://www.datacamp.com/community/tutorials/text-analytics-beginners-nltk
<br>Telegram Bot Framework https://core.telegram.org/bots
<br>Creating Dashboard using Power BI Tool https://docs.microsoft.com/en-us/power-bi/desktop-getting-started
