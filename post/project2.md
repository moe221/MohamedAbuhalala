---
date: 2021-02-08T10:58:08-04:00
description: "A model that can predict the daily power demand of a building."

featured_image: "/images/comparing_floors_kWh.png"

tags: []
title: "Building Power Demand Prediction"
---

Office buildings have an important role in shaping electricity demand
in modern societies. Their energy demand patterns account in some countries
for up to 45 % of the primary energy consumption. Monitoring the energy consumption
of buildings and appliances using smart meters allows for a better understanding of 
specific energy needs and patterns, as well as enables locating peak demand times 
which can help decision-makers and planners to improve electricity consumption.


## Project Overview 

* Cleaned and restructured smart power meter time series data into 
a multi-index data frame. 

* Conducted an extensive EDA to locate trends in the power demand.

* Used hierarchical agglomerative clustering to cluster building 
floors based on similarities. 

* Calculated and compared the average annual electricity cost of
 the building in different countries.

* Trained a SARIMA model to predict daily power demand 
taking into account weekends and national holidays.


---

{{< figure src="/images/comparing_floors_kWh.png"  width="850" >}}
{{< figure src="/images/SARIMA_results.png" width="850" >}}  

## Results

| Evaluation Metric||SARIMA||SARIMA with external regressors|
:---:|:---|:---:|:---:|:---:|
| RMSPE|       | 26% |   | 12%                         |
| R²  |        | 0.52 |  | 0.82                        |
   

[GitHub repo](https://github.com/moe221/SARIMA_Power_Demand_Prediction)