---
date: 2020-10-09T10:58:08-04:00
description: "An algorithm that can estimate the retention time in pressure pipes
using waste-water temperature time series."

featured_image: "/images/h2s & art scatter plot - complete dataset2.png"

tags: []
title: "Temperature-based Retention Time"
---

Most sewer networks consist of gravity pipes, which rely on the natural slope
of the landscape to convey waste-water, and pressure pipes, which are driven by
a pump that pushes waste-water to higher located collection points. Anaerobic
retention time (ART) is defined as the amount of time a given volume of waste-water
resides in a pressure pipe before being discharged. Long retention times have been
linked to an increase in the occurrence of unwanted biological and chemical
processes, such as the formation of hydrogen sulfide (H2S) which is associated
with odor, corrosion, and health problems. Retention time is most commonly
determined using flow meters which can be very costly. In this project, I present a
new method for determine retention times using temperature data.

## Project Overview

* Collected waste-water temperature data using a SulfiLogger sensor from two different pressure pipes.

* Cleaned and analyzed the data.

* Found correlation between temperature changes and flow rate.

* Calculated reference retention times using flow meter data.

* Created an algorithm that could determine the retention times
 of a waste-water parcel in a pressure pipe using temperature data


{{< figure src="/images/ART-flow & temp - complete.png" width="1000" >}}

## Results

| Evaluation Metric:  |---Dataset A                 | ---Dataset B       |
|:--------------------|:-------------------------:|:---------------:|
| RMSPE           |          11%              |     14%         |
| R²             |          0.97             |      0.75       |


[GitHub repo](https://github.com/moe221/Temperature-based_RT_project)
