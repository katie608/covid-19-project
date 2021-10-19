# COVID-19 Data Science Project
Repository for Team Delta Data Science Project 1

Team Delta: Jen, Shamama, Hazel, Sydney, Katie


## Data Setup

### Census Data
**Steps**: Our objective is to find the 2018 American Community
Survey\[1\] (ACS) Total Population estimates, disaggregated by counties.
To check your results, this is Table `B01003`.

1.  Go to [data.census.gov](data.census.gov).
2.  Scroll down and click `View Tables`.
3.  Apply the following filters to find the ACS **Total Population** estimates,
    disaggregated by counties.

-   `Topics > Populations and People > Counts, Estimates, and Projections > Population Total`
-   `Geography > County > All counties in United States`

1.  Select the **Total Population** table and click the `Download`
    button to download the data; make sure to select the 2018 5-year
    estimates. (2019 data should also be fine in this instance)
2.  Unzip and move the data to your `/data` folder.
3. Rename the .csv file to census.csv


### Weather Data

To set up, follow instructions here:
https://docs.ropensci.org/rnoaa/articles/rnoaa.html

Make sure to remember to get an API key!

Docs:
* https://docs.ropensci.org/rnoaa/
* https://cran.r-project.org/web/packages/rnoaa/rnoaa.pdf


# Report
**What question did you set out to answer?**

We set out to answer the question of whether the outside temperature affects COVID cases.

**What is the relevant background on your question?**

We decided on this question because we hypothesized that comfortable weather would allow people to hold more outdoor gatherings than indoor gatherings. Since COVID and other viruses spread more indoors[^1], outdoor social gatherings are less likely to spread the virus compared with indoor gatherings.

**What data did you find to help answer that question?**

We used the [rOpenSci rnoaa package](https://docs.ropensci.org/rnoaa/). This package serves as an R interface to several different NOAA data sources, including historical weather data.

**What is the quality of those data?**

As a national administration, NOAA's data can be assumed to be accurate, and generally unbiased. However, there are certain places where data are incomplete, or not in an ideal format. The most recent date of the dataset varies a lot by county. For example, Orleans Parish, LA has very recent historical data, ending about a week ago. However, Middlesex, CT data ends about a year ago. Additionally, in the daily temperature dataset, some locations have data for maximum temperature, some have data for minimum temperature, and some have data for average temperature. This makes it difficult to compare weather between locations.

**What conclusions did you come to?**


**What questions do you have remaining?**


[^1][cdc.gov](https://www.cdc.gov/coronavirus/2019-ncov/daily-life-coping/outdoor-activities.html)
