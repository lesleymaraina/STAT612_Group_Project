---
title       : Air Quality and COVID-19 Mortality and Incidence Rates 
subtitle    : 
author      : Courtney Stoner, Katherine Lee, Steven Tomey, Lesley Chapman
job         : STAT612 Group Project
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
ext_widgets : {rCharts: [libraries/nvd3]}
output:
  flexdashboard::flex_dashboard:
    orientation: rows

---









---

---
## Introduction

**Project Aim**
> - Compare the average percentage of unhealthy air quality days of each county to its COVID-19 mortality and incidence rates

**Data**
> - Annual summaries of recorded Air Quality Index (AQI) for each county within the United States from the years 2015-2019 
> - COVID-19 mortality and incidence rates per country as of June 6th, 2020
> - Unhealthy days are defined as days where the AQI is greater than 101

---


---
## Research Questions

> - Are counties with poorer air quality more likely to have higher COVID-19 mortality and incident rates? 
>- Do the effects of specific air pollutants on COVID-19 mortality and incident rates vary?

---


---
## Hypotheses

> - **H1**: A higher percentage of bad air quality (AQI) days is associated with a higher mortality rate 
> - **H2**: A higher percentage of bad air quality days is associated with a higher incident rate (Kat)
> - **H3**: Each pollutant (CO, NO2, Ozone, SO2, PM2.5, PM10, Air Quality Index) has a different (or same) effect on mortality rate
> - **H4**: Each pollutant (CO, NO2, Ozone, SO2, PM2.5, PM10, Air Quality Index) has a different (or same) effect on incident rate? 

---


--- &twocol

## Exploratory Data Analysis

Distribution of mortality rate and the average percent of unhealthy days counted

*** =left

![plot of chunk unnamed-chunk-5](assets/fig/unnamed-chunk-5-1.png)

*** =right

![plot of chunk unnamed-chunk-6](assets/fig/unnamed-chunk-6-1.png)

---


--- &twocol
*** =right
Nationwide avg pct unhealthy days over 5 years and incidence rate, mortality rate

*** =left

![plot of chunk unnamed-chunk-7](assets/fig/unnamed-chunk-7-1.png)

---

--- .class #id

---

--- &twocol

## Data-driven Hypotheses

#### Evaluation of sampled states

*** =right

> - Pennyslvania, California, and Washington have positive correlations in incidence rate and average percent unhealthy days, while
> - Texas and New York have negative correlations

*** =left

![plot of chunk unnamed-chunk-9](assets/fig/unnamed-chunk-9-1.png)




---




--- 


> - PA, CA, and WA linear regression results
> - not enough evidence to say that the pct unhealthy days is associated with an increased case fatality ratio (p value .839)
> - There may be enough evidence to say that the pct unhealthy days is associated with the incidence rate (infections per 100,000 people)
> - Pvalue for California is: 0.029



---

--- &twocol
*** =right
When plotting average of the median aqi against mortality rate. More states seem to have a positive correlation

*** =left
![plot of chunk unnamed-chunk-12](assets/fig/unnamed-chunk-12-1.png)
---

--- .class #id 

---

--- &twocol
*** =right
> - Checked the same association with the average of the 90th percentile AQI over 5 yrs
> - For all states, this one has a slight positive correlation but high p-value .187 

*** =left

![plot of chunk unnamed-chunk-14](assets/fig/unnamed-chunk-14-1.png)


---


--- .class #id 

## Conclusions

> - There could be enough evidence to say that the 5-year average of the median air quality is associated with higher mortality rates 

> - This association could be true when considering every 1 additional increase to the avg of the 5yr med AQI is associated with a 0.000178 increase in the mortality rate

> - The statistical tests as well as caveates within the data could also have influenced the results

---

