Lab 03 - Nobel laureates
================
Bob D
28Mar23

### Load packages and data

``` r
library(tidyverse) 
```

``` r
nobel <- read_csv("data/nobel.csv")
```

## Exercises

### Exercise 1

``` r
#How many variables are in the dataset?
nobel %>%
  ncol()
```

    ## [1] 26

``` r
#Each row represents a winner. Number of winners?
nobel %>%
  nrow()
```

    ## [1] 935

### Exercise 2

``` r
#Create a new data frame called nobel_living that includes only observations of living people for which country data is available. 
novel_living <- nobel %>%
  filter(!is.na(country),gender != "org", is.na(died_date))
```

### Exercise 3

### Exercise 4

### Exercise 5

### Exercise 6
