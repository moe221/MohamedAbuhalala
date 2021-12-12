---
date: 2020-12-11T11:13:32-04:00
description: "Predicting the rental price of an apartment based on
 it's features."
featured_image: "/images/Berlin-map1.png"
tags: []
title: "Apartment Rental Price Predictor"
---

looking for an apartment in berlin is so annoyingly hard and competitive that
it feels like it should be an olympic sport. Everyone knows that finding the perfect apartment
isn't easy, but being well prepared by doing some research on the renting market in Berlin
before jumping in and trying your luck, could improve your chances. Recently, I was thinking about moving myself 
and wanted to get an idea of what I should expect, so I decided to do this project to help
me with my apartment hunt!   

## Project Overview

* Analyzed two different datasets scrapped from Immobilienscout24.de. 

* The raw data consisted of rental offers posted on Immobilienscout24.de
 in Sep 2018, May 2019, Oct 2019, Feb 2020 and Apr 2020. 
 
* Cleaned and joined the two datasets as well as created new
 features from the description of each listing.
 
* Conducted an extensive EDA in order to develop insight on the
 rental market in Berlin.
 
* Implemented three different Machine learning models that could 
estimate the total rent price (Warmmiete) of an apartment in berlin.

* Used GridsearchCV to find the best hyperparameters for a Random 
Forest Regression.

* Serialized the RF model using pickle and created a simple UI.

{{< figure src="/images/Berlin-map1.png"  width="850" >}}

## Results
   
| Evaluation Metric  | Multiple linear Regression| Lasso Regression| Random Forest     |
|--------------------|:-------------------------:|:----------------:|:----------------:|
| **MAE  [€]**       |          194.92           |     194.92      |    166.94         |
| **RMSE [€]**       |          277.76           |     277.76      |    259.80         |
| **R²   [-]**       |           0.85            |      0.85       |     0.87          |

   

[GitHub repo](https://github.com/moe221/Apartment_price_ML)