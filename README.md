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

This is an R library that has the stuff that we need, but unless I am missing
something obvious, there will be much difficulty getting this data into a
usable format. See more specific notes as comments in the project.rmd file.

To set up, follow instructions here:
https://docs.ropensci.org/rnoaa/articles/rnoaa.html

Make sure to remember to get an API key!

Docs:
* https://docs.ropensci.org/rnoaa/
* https://cran.r-project.org/web/packages/rnoaa/rnoaa.pdf
