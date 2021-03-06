---
title       : Data Products 
subtitle    : Shiny Application for Motorcars
author      : M. Jung
job         :  
framework   : io2012   # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []   # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Shiny Application "Analysis Mtcars"

The Application "Analysis Mtcars" helps to analyse the  "Motor Trend Car Road Tests" dataset (mtcars).

Functionality:
- web based
- interactive: you choose which attributes you want to analyse
- nice "Scatterplot Matrices"
- possibility to build a simple linear model for mpg
- embedded detailed documentation
- for free

--- .class #id 

## Example for choosen attributes hp and wt

The Scatterplot Matrices show the correlation between the choosen variables. For the Transmission (am) there are different colors used. Green are the cars with automatic transmission, blue the cars with manual transmission. 

```r
pairs(mtcars[,c("mpg", "hp", "wt")], panel = panel.smooth,
                       col = 3 + mtcars$am)
```

<img src="assets/fig/simple-plot-1.png" title="plot of chunk simple-plot" alt="plot of chunk simple-plot" style="display: block; margin: auto auto auto 0;" />

Linear model for the choosen Attributes:
fit <- mpg ~ hp + wt

--- .class #id

##  Prospects

The following features are in planning for the next releases:
- load your own dataset for the analyse
- possibility to change the type of variables in factors
- selection of different plots
- choose the variable for which you want to build a linear model
- predictive Analysis based on the linear model

--- .class #id

## Links

Shiny Application "Analysis Mtcars" 
- https://mjung4.shinyapps.io/Analysis_Mtcars/

Code on my github Account:
- https://github.com/mjung4/ShinyAppCode 

These Slides on my github Account:
- http://mjung4.github.io/ShinyApp/index.html 
         
              
                  
Note: These slides are done with Slidify. 
Slidify was created by [Ramnath Vaidyanathan](https://github.com/ramnathv) in order to streamline the process of creating and publishing `R` driven presentations.



