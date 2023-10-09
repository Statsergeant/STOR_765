765_consuling_project
================

# Behavioral Health 911 Call Notes(Draft)

Using detroit_analysis data, we will find out a meaningful observation.
The things we will do includes hypothesis test of null no difference of
the number of calls based on hour, month, weekday. Also, since we have
census track data, we will do spatial analysis to see the feature of
location of calls.

## Exploration data Analysis

Data consists of 48318 \* 23 matrix and there are some NA values in some
columns. If I need to adjust NA values, I will mention it if necessary.

## Analyses

### Time series of counts

First of all, we will see the glimpse of difference of the number of
calls with several barplots.

<img src="real_analysis_files/figure-gfm/setup-1.png" width="50%" /><img src="real_analysis_files/figure-gfm/setup-2.png" width="50%" /><img src="real_analysis_files/figure-gfm/setup-3.png" width="50%" />

### Spatial Analysis

Let’s see the hit map first to see what area has the most calls.

<!-- ```{r, echo = F} -->
<!-- data_long_lati <- data %>%  -->
<!--   group_by(longitude,latitude) %>%  -->
<!--   summarise(n = n()) -->
<!-- mapviewOptions(maxpoints = 300) # diamonds has some 53000 rows -->
<!-- my_sf <- st_as_sf(data_long_lati, coords = c('longitude', 'latitude')) -->
<!-- my_sf <- st_set_crs(my_sf, 4326) -->
<!-- mapview(my_sf, map.types = mapviewGetOption("basemaps"))@map -->
<!-- ```{r} -->
<!-- ggmap::register_google(key = "AIzaSyDSjw6COMi28nOOPXWdQyu3XCmwY7-CQU4", write = TRUE) -->
<!-- lon_mean <- data_long_lati$longitude %>% mean() -->
<!-- lat_mean <- data_long_lati$latitude %>% mean() -->
<!-- get_googlemap(center = c(lon = lon_mean , lat = lat_mean),zoom = 11, markers =  data_long_lati[,1:2], scale = 2) %>% ggmap() -->
<!-- ?get_googlemap -->
<!-- ``` -->
