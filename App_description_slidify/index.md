---
title       : Daily Calories Intake Calculator
subtitle    : Description of the application of the same name
author      : L. Stepanek
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---


## About the application

- the app can be used to estimate averagely daily intake of calories [in kCal]
- average calories intake depends primarily on

1. age of a person
2. weight of a person
3. height od a person
4. and a gender of a person

- and other factors not included in estimation


--- .class #id

## Formula of the estimation

- the estimation is based on Harris - Benedict equation

- for females it is

$$BMR = 655.1 + 9.6 * weight [kg] + 1.8 * height [cm] - 4,77 * age [years]$$

- for males it is

$$BMR = 66.5 + 13.8 * weight [kg] + 5.0 * height [cm] - 6.8 * age [years]$$

- where $BMR$ is basal metabolic rate $[kCal]$

--- .class #id

## An example

- for a male with $weight = 70$ $kg$, $height = 175$ $cm$ and $age = 30$ $years$, we get $BMR = 1668.2$ $kCal$

- for a female with $weight = 65$ $kg$, $height = 170$ $cm$ and $age = 30$ $years$, we get $BMR = 1427.5$ $kCal$



--- .class #id


## Some discussion

- for extreme values the estimation gives unexpected results (and is not so reliable)

- when other variables are fixed, females generally should take less calories than males

- more activities a person do during a day, more calories shoul he or she take - there is a coefficent $>1$ which should be $BMR$ multiplied by


