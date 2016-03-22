---
title       : Spatial Simulated Annealing
subtitle    : Developing Data Products - Reproducable Pitch
author      : IJDalrymple
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

--- .class #id

## The problem

We want to understand the spatial distribution of some characteristic of a soil around the Meuse River.
We know that the distribution of soil characteristics is a function of  

1. Distance to the river
2. Soil type
3. Frequency of flooding

Where is the best place to put the samples in order to maximise the amount of information?

Spatial Simulated Annealing is a process that minimises a geostatistical variable in order to optimally arrange a given number of samples in an area. While considering the criteria above, we can choose to optimise the design for different outcomes, such as:   

> * Trend identification
> * Variogram estimation
> * Spatial interpolation

--- bg:#EEE

## Limited Example

The following is a worked example of a design for 30 samples in the defined catchment area, optimised for the estimation of a variogram. Note that because this criterion was chosen, the spatial coverage may be incomplete. 

<img src="figure/unnamed-chunk-1-1.png" title="plot of chunk unnamed-chunk-1" alt="plot of chunk unnamed-chunk-1" style="display: block; margin: auto;" />

---

## Spatial Simulated Annealing Application


This application at https://ijdalrymple.shinyapps.io/Spatial_Simulated_Annealing/ has the ability to choose the number of samples to be added and the intention of the optimisation design. Please wait while the link below has time to upload. 

<iframe src='https://ijdalrymple.shinyapps.io/Spatial_Simulated_Annealing/' width = '80%' height = '400px'></iframe>

---

## Where to find more information

For more information on the Meuse data package in R, type help(meuse) and help(meuse.grid) into the prompt.

This application uses functions within the spsann package available on CRAN. For more information, please follow [this link.](https://cran.r-project.org/web/packages/spsann/)

For more infomration on fundamental geostatistics, try [this link.](https://en.wikipedia.org/wiki/Geostatistics)




