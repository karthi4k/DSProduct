---
title       : Titanic Prediction Model
subtitle    : Based on Random Forest
author      : Karthikeyan Paramasivam
job         : Learner
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Agenda

1. Choosing the Shiny Project
2. Challenges Faced
3. Project Completion

---

## Choosing the Shiny Project

To choose the  shiny project I kept the below criteria.

1. It should be based on Prediction as i had taken few machine learning courses.
2. Easy to intepret by users/peers who review.
3. The model should be tested easily.

I started with searching for health related data set like effect of smoke, physical activity, eating habits, cancer etc.

But the data were measured with lot of tests/sensors which one cannot easily reporoduce at home.

So i chose to create model for Titanic data where users can enter their preferences and see if they would have survived or not!!!


---

## Challenges Faced

1. I trained the model in my system and decided to load from the shiny server in vain. Later found we can upload with the app.
2. I wanted to show the inputs selected in one place, line by line. But the PASTE method was not helpful. The cat command renders the newline but shows the result in console rather than returning it to ui as shown below.


```r
a = "Line 1"
b = "Line 2"
paste(a,b,sep="\n")
```

```
## [1] "Line 1\nLine 2"
```

```r
cat(paste(a,b,sep="\n"))
```

```
## Line 1
## Line 2
```

---
## Project Completion

1. The project was completed and was running fine in local.
2. The same project deployed in shiny apps io was throwing error.
3. It was not easy to debug as we cannot see the console.
4. Later indentified that they were due to libraries not loadiing some dependancies.
5. They were fixed and the project is ready!!!

