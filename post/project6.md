---
date: 2021-12-03T11:14:48-04:00
description: "Detect and classify faces in movie frames and generate diversity statistics."
featured_image: "/images/diversity_in_hollywood_banner.png"
tags: []
title: "Diversity in Hollywood (Le wagon final project)"
---
Movies have a big impact on our lives. They can influence the way we see the world
around us. Diversity on the big screen is extremely important since it
allows a much wider audience to see what diversity looks like outside of their
own communities and become more familiar and accepting of it.

This project was meant to put Hollywood under the lens and analyze gender and race
representation in a selection of movies spanning from the 1920s to 2021 using
deep learning.

{{< figure src="/images/diversity_stats2.png" >}}


## Project Overview
* Built pipeline for movie frame retrieval from [movie-screencaps.com](https://movie-screencaps.com/)

* Scanned movie frames for faces using MTCNN framework

* Used an ensemble of CNN models to estimate race and gender of detected faces

* Calculated different diversity statistics for each movie

* Used face averaging techniques to create a composite face for each movie based
on all detected faces

* Built and deployed a web application using Heroku and Streamlit to host the results of
the analysis

[Diversity in Hollywood App](https://diversity-in-hollywood.herokuapp.com/)

[GitHub repo](https://github.com/moe221/diversity_in_cinema)

Collaborators:
[Gabi Otero](https://github.com/goGabiO)
