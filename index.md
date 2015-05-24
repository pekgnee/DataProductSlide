---
title       : Developing Data Products Assignment
subtitle    : Reproducible Pitch Presentation
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [quiz]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## What the app is about
- Assignment for the Coursera course "Developing Data Products" by John Hopkins Bloomberg School of Public Health
- Shiny Application hosted at shinyapps.io 
- http://pekgnee.shinyapps.io/DevelopingDataProducts/
- Display statistics from the dataset UCBAdmissions
- Aggregate data on applicants to graduate school at Berkeley for the six largest departments in 1973 classified by admission and sex.

---

## What the data looks like

```r
data(UCBAdmissions)
str(UCBAdmissions)
```

```
##  table [1:2, 1:2, 1:6] 512 313 89 19 353 207 17 8 120 205 ...
##  - attr(*, "dimnames")=List of 3
##   ..$ Admit : chr [1:2] "Admitted" "Rejected"
##   ..$ Gender: chr [1:2] "Male" "Female"
##   ..$ Dept  : chr [1:6] "A" "B" "C" "D" ...
```

---

## What the app looks like
<iframe src = 'http://pekgnee.shinyapps.io/DevelopingDataProducts/'></iframe>

--- &radio

## Quiz time
Now try selecting different inputs from the [app](http://pekgnee.shinyapps.io/DevelopingDataProducts/) and answer the following question:  
  
For all the departments A - F,  
the number male applicants is higher than the number of female applicants.  
TRUE or FALSE?

1. TRUE
2. _FALSE_

Thanks for evaluating my Shiny App & Slidify !

*** .hint 
Select each department A - F in the left hand panel and compare Male / Female number of applicants in the top bar plot in the right hand panel
