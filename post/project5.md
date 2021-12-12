---
date: 2021-02-17T11:14:48-04:00
description: "Classifying construction contractors based on work description."
featured_image: "/images/piechart.png"
tags: []
title: "NLP Contractor Classification"
---
I've made it a habit to always look back at my previous work experiences
and think about how what I'm learning now could have helped me do my job better or automate
some tasks. Recently, I've been learning about Natural Language Processing, which involves
transforming text data into a format that a machine learning algorithm can understand.
After learning some of the basics of NLP I was eager to try out this concept
on some data that I collected myself during my time as a construction manager.

The data contained information on extra construction work that was needed to complete a project.
My goal was to classify contractors based on the description of the work that they have done.

{{< figure src="/images/dataset_head.png" >}}
 

## Project Overview 
* Cleaned the raw data and checked for null values

* Explored and visualized the data

* prepared the 'work_description' column by:

    - Removing common words and punctuation
    - Tokenizing the descriptions (convert each description into a list of words)
    - Performing vectorization: use SciKit Learn's bag-of-words model

* Ensemble testing with Multiple Linear Regression, Random Forest, K-NN, and Naive Bayes classifier

{{< figure src="/images/color_barplot.png" >}}

## Results

|Classifier                  | accuracy |
|:---------------------------|----------|
| Multiple Linear Regression | 0.90     |
| Random Forest              | 0.88     |
| K-NN                       | 0.75     |
| Naive Bayes                | 0.89     |

[GitHub repo](https://github.com/moe221/NLP_Contractor_Classification)

