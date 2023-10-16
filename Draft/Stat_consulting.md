Stat_consulting
================

# Behavioral Health 911 Call Notes(Draft)

## Instruction

In real-life situations, people call 911 for various reasons, including
accidents, violence, or fire emergencies. For our analysis, we will
specifically focus on the call type ‘Behavioral Health,’ which can be
categorized into ‘Mental Health Crisis,’ ‘Suicidal Threats or Attempts,’
or ‘Emotional Distress.’ The objective is to understand the
characteristics of calls falling under this category.

Firstly, we will concentrate on the distribution of ‘Behavioral Health’
calls over time, considering factors such as hours, months, and
weekdays. This will provide insights into when these calls are more
likely to occur.

Secondly, employing spatial analysis, we aim to unveil patterns, trends,
and relationships that may not be immediately apparent. This analysis
will help in understanding the geographical aspects of ‘Behavioral
Health’ calls, offering a comprehensive view beyond temporal
considerations.

## Exploration data Analysis

Data consists of 48318 \* 23 matrix and there are some NA values in some
columns. If I need to adjust NA values, I will mention it if necessary.

## Analyses

### Time series of counts

First of all, we will see the glimpse of difference of the number of
calls with several barplots.

![Barplots](/image/number_hourly_monthly_weekly.png)

Based on the plots, we can see there are some difference of frequencies
between each months, hours, and weekday. To see it is a statistically
significant difference, I would like to use Chisq.test.

``` r
# chisq.test for month
chisq.test(data_bar_month$sum , p = month_prop )
```

    ## 
    ##  Chi-squared test for given probabilities
    ## 
    ## data:  data_bar_month$sum
    ## X-squared = 348.52, df = 11, p-value < 2.2e-16

``` r
# chisq.test for month
chisq.test(data_bar_weekday$sum , p = weekday_prop )
```

    ## 
    ##  Chi-squared test for given probabilities
    ## 
    ## data:  data_bar_weekday$sum
    ## X-squared = 31.597, df = 6, p-value = 1.95e-05

``` r
# chisq.test for month
chisq.test(data_bar_hour$sum , p = hour_prop )
```

    ## 
    ##  Chi-squared test for given probabilities
    ## 
    ## data:  data_bar_hour$sum
    ## X-squared = 4800, df = 23, p-value < 2.2e-16

### Spatial Analysis

Let’s see the hit map first to see what area has the most calls.

![Mapview](/image/map_view.png)



