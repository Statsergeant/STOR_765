# STOR_765_911_calls_ Detroit

   Thanks for all the informations! ^^

   @@ Meeting note : [Behavioral Health 911 Calls Notes - Google Docs](https://docs.google.com/document/d/18fq7AWVNhskYoM3dm362KyvO4PeQoHaOWQn040oQyCA/edit)

1. In the attached zip file, you will find:

   - *detroit_analysis.csv*: The analysis-ready dataset containing only behavioral health calls from the city of Detroit, with relevant variables (time, date, lat/long coordinates for census tract centroid, population, demographics)
   - *detroit_analysis.Rdata*: Same as above but as an R dataset instead of csv.
   - *vera911data.R*: R script used to derive the city-level tables and attach x-y coordinates to census tracts

    

   The raw csv file I downloaded from GitHub that contains all data for all cities is located here: https://dcvera.s3.amazonaws.com/all.zip

    

   A few notes:

   - You will see that I have provided a data file for the city of Detroit instead of New Orleans. After more careful inspection of the data, it appears that New Orleans had a very large proportion of their calls coded as “other”, which is why the number of behavioral health calls was so small. Detroit has a more calls and they seem to be appropriately coded.
   - The GitHub site for the original data and data descriptions is located here: https://github.com/tsdataclinic/Vera
   - There were a series of blogs on Medium about this consolidated 911 data. They may be helpful to give more context.
   
   1. [Announcing a Consolidated Dataset of 911 Calls for Five US Cities (Part 1)](https://medium.com/dataclinic/announcing-a-consolidated-dataset-of-911-calls-for-five-us-cities-part-1-4320a1a31a88)
   2. [Creating a consolidated taxonomy for 911 call data across different US Cities (Part 2)](https://medium.com/dataclinic/creating-a-consolidated-taxonomy-for-911-call-data-across-different-us-cities-part-2-9600cb09abfd)
   3. [Exploring Temporal and Geographic Patterns of 911 Calls within US Cities (Part 3)](https://medium.com/dataclinic/exploring-temporal-and-geographic-patterns-of-911-calls-within-us-cities-part-3-980c858ff646)

​	Variables :

| Name of variable |         Actual name          |
| :--------------: | :--------------------------: |
|    B01003_001    |          total_pop           |
|    B01002_001    |          median_age          |
|    B03002_003    |          white_pop           |
|    B03002_004    |          black_pop           |
|    B03002_005    |        amerindian_pop        |
|    B03002_006    |          asian_pop           |
|    B03002_008    |        other_race_pop        |
|    B03002_012    |         hispanic_pop         |
|    B11001_003    |      married_households      |
|    B14001_002    |          in_school           |
|    B15003_017    |     high_school_diploma      |
|    B07009_003    |  high_school_including_ged   |
|    B17001_002    |           poverty            |
|    B19013_001    |        median_income         |
|    B19083_001    |          gini_index          |
|    B25002_001    |        housing_units         |
|    B25002_003    |     vacant_housing_units     |
|    B25003_001    |    occupied_housing_units    |
|    B25058_001    |         median_rent          |
|    B25071_001    | percent_income_spent_on_rent |
|    B23025_002    |      pop_in_labor_force      |
|    B23025_004    |         employed_pop         |
|    B23025_005    |        unemployed_pop        |
|                  |                              |

