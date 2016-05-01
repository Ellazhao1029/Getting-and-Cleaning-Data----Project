# Getting and Cleaning Data - Course Project

This is the course project for the Getting and Cleaning Data Coursera course.
The R script, **run_analysis.R
88, does the following:

1. It reads the **train** and **test** data sets and appends the two datasets into one data frame. This is done using `rbind`.
2. It extracts just the *mean* and *standard deviation* from the **features** data set. This is done using `grep`.
3. After cleaning the column names, these are applied to the **x** data frame.  
4. After loading **activities** data set, it converts it to lower case using `tolower` and removes underscore using `gsub`. *activity* and *subject* column names are named for **y** and **subj** data sets, respectively.
5. The three data sets, **x**, **y** and **s**, are merged. Then, it is exported as a *txt* file into the Project folder in the same working directory, named **merged_data.txt**.
6. The *mean* of activities and subjects are created into a separate tidy data set which is exported into the Project folder as *txt* file.

The end result showns in the file **average_dateset.txt**.
