---
title       : Relocating in the Capital of Iceland 
subtitle    : Predicting relocation cost
author      : gnusi100
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- .class #id 

## What does the app do

This data product helps you out in the beginning of the process of finding a new appartment

1. It gives you an price estimate on your appartment

2. It estimates the price of your desired appartment, given the size and location

3. It gives you an impression of the prices in different areas of the capital of Iceland

---
## The data
I got the data from this webpage [http://www.skra.is/markadurinn/talnaefni/](http://www.skra.is/markadurinn/talnaefni/)

The data is a summary from all the real estate contracts for appartments in 34 different areas in Reykjavik Iceland in 2013

The values that my prediction model is built on is the average square meter price in each area




```r
str(data2)
```

```
## 'data.frame':	34 obs. of  6 variables:
##  $ type         : Factor w/ 1 level "appartment": 1 1 1 1 1 1 1 1 1 1 ...
##  $ neighbourhood: Factor w/ 34 levels "Akrar  Gardabaer",..: 18 20 10 13 11 29 34 12 14 25 ...
##  $ year         : int  2013 2013 2013 2013 2013 2013 2013 2013 2013 2013 ...
##  $ count        : int  391 106 76 113 33 96 36 74 91 84 ...
##  $ size         : int  86 108 89 97 106 100 99 105 101 110 ...
##  $ price        : num  2524 2331 2185 2166 1826 ...
```

---
  
## Limitations

1. It expects that the square meter price is the same for all appartment sizes in a neighbourhood

2. It´s probably only useful if you are interested in an average quality appartment for each neighbourhood



---
## Next step

Buy the the real estate contracts from Registers Iceland and build á real regression model with more parameters to estimate appartment prices.

Add a map to the app for better understanding of the neighbourhoods



