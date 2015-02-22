---
title       : Exploratory Data Analysis for Regression Model Development
subtitle    : Data Product Pitch
author      : kylase-coursera
job         : MOOC Student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Data analysis life cycle

1. Formulate question
2. Gather data
3. **Exploring data (Time-consuming)**
4. Develop model to answer question
5. Document steps and analysis for publication

---
## Exploring data

As we are in an era which the amount of data are growing exponentially, exploring data needs to be easier and less tedious. 

Exploring data needs the following skillsets:

1. Data wrangling
2. Data visualisation
  - Programming-based such as MATLAB, Matplotlib (Python), ggplot (R)
  - HTML/CSS/JS such as [D3.js](http://d3js.org)
  - Software like Tableau, etc

---
## App

The [data product app that I have developed](https://kylase-coursera.shinyapps.io/Project/) is a simple data visualisation tool that helps to develop linear model in an agile fashion.

Making use of the `mtcars` data as an example, one can easily manipulate 3 variables (x axis, colour and size of the points on scatter plot) at one to visualise the data to develop regression models.

So you can easily develop a linear regression:

```r
lm(mpg ~ factor(cyl) + hp + wt, data = mtcars)
```

```
## 
## Call:
## lm(formula = mpg ~ factor(cyl) + hp + wt, data = mtcars)
## 
## Coefficients:
##  (Intercept)  factor(cyl)6  factor(cyl)8            hp            wt  
##     35.84600      -3.35902      -3.18588      -0.02312      -3.18140
```

---
## Sample Screenshot of app

![sample screenshot from app](assets/img/ss.png)