---
title       : Energy Consumption
author      : Sulchan Yoon
job         : R student
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      #
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Description

The Shiny App written displays energy consumption information for the years of 2012 2013 and 2014:

- gas
- electricity
- water

---
## Details

For the years of 2012, 2013, 2014, every Sunday, data is gathered from the meters. 

The values are subtracted from each other to get the week's usage. 

Finally, with electric prices in the local area, use a formula to gather the estimated price for the week. 

---
## Example

Here are the first 10 lines of the Excel file:


```
##          Date PriceGas PriceElec PriceWater
## 1  2012-01-01    55.51     22.14       2.96
## 2  2012-01-08    57.22     23.67       3.30
## 3  2012-01-15    62.07     23.29       3.26
## 4  2012-01-22    56.59     23.67       3.02
## 5  2012-01-29    63.63     23.86       3.12
## 6  2012-02-05    83.32     24.43       4.61
## 7  2012-02-12    83.80     25.39       5.03
## 8  2012-02-19    59.13     23.29       5.62
## 9  2012-02-26    54.13     21.00       5.40
## 10 2012-03-04    40.49     21.38       3.66
```

---
## Lessons learned

- It is necessary to use reactive functions when there are 2 or more inputs. 

- In the renderPlot function, dataframe name needs parenthesis.

---
## Conclusion

- Writing the application does not take long, and thus we know that large projects are all doable. 
