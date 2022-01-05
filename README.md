# Time-Series-Forcasting-in-R
This repository introduces common techniques to analyse time series data and make predictions.

## Replication Requirements
The following R packages outside of the base set of functions that will be used in this time series data analytics:
- library(skimr)          # data summary and description
- library(tidyverse)      # data manipulation and visualization
- library(ggplot2)        # data visualization
- library(lubridate)      # easily work with dates and times
- library(fpp2)           # working with time series data
- library(zoo)            # working with time series data

## Introduction
Moving average is one of smoothing methods (i.e., a family of forecasting methods) that average values over multiple periods in order to reduce the noise and uncover patterns in the data. This method averages values from a window of consecutive time periods, thereby generating a series of averages. The approaches primarily differ based on the number of values averaged, how the average is computed, and how many times averaging is performed. This repo will walk you through the basics of performing moving averages.

### Learning objectives:
1. Centered Moving Averages
2. Trailing Moving Average for Forecasting
3. Moving Averages of Moving Averages

## Centered Moving Averages
The centered moving averages is a most straightforward simple moving average method. For this method, we choose a number of neighbourhood points and average them to estimate the trend. To keep the calculation symmertic, it is beneficial to use an odd number of points.

## Trailing Moving Average for Forecasting
For purposes of forecasting, we use trailing moving averages, where the window of k periods is placed over the most recent available k values of the time series.

## Moving Averages of Moving Averages
The concept of simple moving averages can be extended to taking moving averages of moving averages. This method is often employed with an even number of time series data points so that the final product is symmetric around each point.

## References
1. UC Business Analytics R Programming Guide.
2. Hyndman, R.J., & Athanasopoulos, G. (2021) Forecasting: principles and practice, 3rd edition, OTexts: Melbourne, Australia. OTexts.com/fpp3.
