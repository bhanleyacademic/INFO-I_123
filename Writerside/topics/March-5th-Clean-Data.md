# March 5th - Preparation/Cleaning Data

## Canvas
INTRODUCTION

Data preparation, or data cleaning, occurs after collecting and storage of data. It might include tasks such as: removing duplicates, assigning unique identifiers to each observation, ensuring homogeneity, resolving missing values, and ensuring that data types are correct.

Icons-Gray_target.png  LEARNING OBJECTIVES

Students will be able to:

1) Understand data preparation/cleaning tasks

2) Define tidy data

OFFICE HOURS

Joshua Nunley (joshnunl@iu.edu): Wednesdays, 5-6 pm on Zoom or email for appointment

Staša Milojević (smilojev@indiana.edu): Thursdays, 3-4 pm, Luddy Center for Artificial Intelligence (1015 E. 11th St.) 2032 or email for appointment

Devin Wright  (devrwrig@iu.edu): Fridays 11am-12pm, Zoom

Links to an external site.Links to an external site. or email for appointment

Icons-Gray_clipboard.png  TO-DO

1) Watch the videos below (in the Resources - Video section) prior to coming to class. Be sure to take notes as you watch.

2) Join us in class on Tuesday to expand your understanding of these concepts and practice applying them.

RESOURCES - VIDEO
[](https://www.youtube.com/watch?v=DJr4zRG0O9Y)

RESOURCES - MAJOR CONCEPTS

A dataset is a collection of values, usually either numbers (if quantitative) or strings (if qualitative). Values are organized in two ways. Every value belongs to a variable and an observation. A variable contains all values that measure the same underlying attribute (like height, temperature, duration) across units. An observation contains all values measured on the same unit (like a person, or a day) across attributes.

Tidy data is a way of presenting a matrix of data. There are three interrelated rules that make a dataset tidy: each variable must have its own column, each observation must have its own row, and each value must have its own cell.

## Class Notes
- Slides are missing so they will be reposted
- 50 questions on exam
- Identify Fallacy, valid/invalid, prepositions & conclusions
- Sampling (snowball, etc.)
- Algorithms (bubble sort, binary sort, etc.)
- SQL/Database
  - Understand difference between entity vs. attribute
  - Inner and Outer Join
  - SELECT, ON, WHERE, FROM

## Lecture
- Missing values/null/empty cells are a big problem for analysis
- Primary keys on unique identifiers are ways to stop duplicate data
- 70-90% of time spent on data cleaning
  - Can cost a lot when using low quality/uncleaned data
### Tidy Data
- Values
  - Numbers or Strings
- Variables
  - All of the values that measure a single attribute
  - Are in columns
- Observation
  - All of the values of the same unit across all variables
  - Are in rows
- Tidy format means variables in columns and observations in rows
- Tidy data is a format not a synonym for clean data
### Unique ID
- Unique Identify each observation
### Homogeneity
- Data should have the same standard
### Missing Data
- Listwise Deletion
- Dropping Variables
- Imputation with central tendency ( mean, median, mode)
- Imputation using other variables (estimated value)
- Why is the data missing
  - Completely at Random
  - Missing at Random
  - Not at Random

## Aside
Aside: Is there an algorithm/math formula that identifies if outliers are causing too much of a skew on the mean of the data? Is that the log-likelihood function? Is it just confidence intervals?

Something along the lines of:

Mean of data

\# of entries above vs. number of entries below
Adjust until entries are ~ even 

```tex 
\underset{\text{# of entries lower than mean}}{A}<\frac{\sum_{i=0}^n n_i}{n}<\underset{\text{# of entries higher than mean}}{B}
```