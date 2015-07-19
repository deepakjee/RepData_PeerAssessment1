# Reproducible Research: Peer Assessment 1

## Load Libraries

```r
library(ggplot2)
```



##Load the data 

```
##   steps       date interval
## 1    NA 2012-10-01        0
## 2    NA 2012-10-01        5
## 3    NA 2012-10-01       10
## 4    NA 2012-10-01       15
## 5    NA 2012-10-01       20
## 6    NA 2012-10-01       25
```
##Process/transform the data 

```
##   steps       date interval
## 1    NA 2012-10-01        0
## 2    NA 2012-10-01        5
## 3    NA 2012-10-01       10
## 4    NA 2012-10-01       15
## 5    NA 2012-10-01       20
## 6    NA 2012-10-01       25
```

##Calculate the total number of steps taken per day

```
## 'data.frame':	53 obs. of  2 variables:
##  $ date : Date, format: "2012-10-02" "2012-10-03" ...
##  $ steps: int  126 11352 12116 13294 15420 11015 12811 9900 10304 17382 ...
```

##Histogram of total number of steps taken each day
![](figure/unnamed-chunk-5-1.png) 

##Calculate the mean the total number of steps taken per day

```
## [1] 10766.19
```

##Calculate the  median of the total number of steps taken per day

```
## [1] 10765
```

##What is the average daily activity pattern?
![](figure/unnamed-chunk-8-1.png) 

##Which 5-minute interval, on average across all the days in the dataset, contains the maximum number of steps?

```
## [1] 835
```

##Imputing Missing Values

Calculate and report the total number of missing values in the dataset (i.e. the total number of rows with NAs)

```
## [1] 2304
```

Replacement data is the number of steps per interval averaged over all days


A new dataset that is equal to the original dataset but with the missing data filled in.

Histogram of the total number of steps taken each day
![](figure/unnamed-chunk-13-1.png) 

Calculate and report the mean number of steps taken per day. 

```
## [1] 10766.19
```
Calculate and report the median total number of steps taken per day. 

```
## [1] 10766.19
```

Do these values differ from the estimates from the first part of the assignment?

We see that the mean is the same

We see the median is slightly higher 

##Are there differences in activity patterns between weekdays and weekends?
replace the data with the week day name


pluck out the days that being with 'S' (Saturday & Sunday) and add a column for a weekend or weekday flag


average number of steps taken, averaged across all weekday days or weekend days (y-axis)
![](figure/unnamed-chunk-18-1.png) 
