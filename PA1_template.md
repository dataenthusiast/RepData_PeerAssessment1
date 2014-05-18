# Reproducible Research: Peer Assessment 1


## Loading and preprocessing the data
activity <- read.csv("activity.csv")


## What is mean total number of steps taken per day? 
    For this part of the assignment, you can ignore the missing values in the dataset.
    Make a histogram of the total number of steps taken each day
    Calculate and report the mean and median total number of steps taken per day

    #clean the NA's
    activityClean <- activity[complete.cases(activity$steps),]
    
    # set the date variable as a proper date class
    library(lubridate)
    
    #draw histogram of total number of steps taken each day
    hist(day(activityClean$date))

    

## What is the average daily activity pattern?



## Imputing missing values



## Are there differences in activity patterns between weekdays and weekends?
