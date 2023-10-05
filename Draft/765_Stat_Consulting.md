Data analysis for detroit
================

# Stat_consulting_76 with Anna Bauer and Geo Jeong

### 1. Exploration Data Analysis

    The raw data for Detroit has 1923012 rows and 51 columns. To understand the variables, we should reference link : [census_data_911](https://github.com/tsdataclinic/Vera)

#### 1. Let’s see the number of call_type with bar plot

![](765_Stat_Consulting_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

    Based on the graph, We can see the variance of the number of calls by call_types. There were many NA datas, so to do the analysis corretly, I need the exact dataset, which I will receive from Anna. 

### 2. Analysis

#### The first goal of this analysis is to find out if there is differences of the number of calls, which will be decided by the actual dataset, throughout weekly, month, hours. To see the differnce, I will show the histogram first and do the analysis.

<img src="765_Stat_Consulting_files/figure-gfm/setup-1.png" width="50%" /><img src="765_Stat_Consulting_files/figure-gfm/setup-2.png" width="50%" /><img src="765_Stat_Consulting_files/figure-gfm/setup-3.png" width="50%" />

    There are three plots and we can easily tell that, accroding to th e plot, the difference of the number of calls is the most distingishable in hourly plots. We can assume that the hypothesis 'H0: there is no difference' would be rejected.
