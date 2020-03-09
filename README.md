---
title: "Getting and Cleaning Data Assignment"
author: "Kunyu Liu"
date: "3/9/2020"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## How the script works

1. Merging the training and the test sets to create one data set.
   1.1 Download file
   1.2 Unzip file
   1.3 Load data into R
   1.4 Merge train and test data

2. Extracting only the measurements on the mean and standard deviation for each measurement
   2.1 Load feature name into R
   2.2 extract mean and standart deviation of each measurements

3. Using descriptive activity names to name the activities in the data set
   3.1 Load activity data into R
   3.2 Replace 1 to 6 with activity names
   
4. Appropriately labeling the data set with descriptive variable names

5. Creating a second, independent tidy data set with the average of each variable for each activity and each subject



## Project Code Book

1. x_train, y_train, x_test, y_test, subject_train and subject_test contain the data from the downloaded files.
2. x_data, y_data and subject_data merge the previous datasets to further analysis.
3. features contains the correct names for the x_data dataset, which are applied to the column names stored in