
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer

<!-- badges: start -->
<!-- badges: end -->

The goal of libminer is to help you understand how many packages you
have and where they are, and how much space they take up.

## Installation

You can install the development version of libminer from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("EricKrantz/libminer")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(libminer)

lib_summary()
#>                                                                      Library
#> 1                                         C:/Program Files/R/R-4.3.1/library
#> 2 C:/Users/ERic.Krantz/AppData/Local/Temp/RtmpobcB9n/temp_libpath552ce4d7303
#> 3                                             C:/Users/ERic.Krantz/R_Library
#>   n_packages
#> 1         30
#> 2          1
#> 3        476

# Also can calculate sizes
lib_summary(size = TRUE)
#>                                                                      Library
#> 1                                         C:/Program Files/R/R-4.3.1/library
#> 2 C:/Users/ERic.Krantz/AppData/Local/Temp/RtmpobcB9n/temp_libpath552ce4d7303
#> 3                                             C:/Users/ERic.Krantz/R_Library
#>   n_packages   lib_size
#> 1         30   68858812
#> 2          1      13023
#> 3        476 1457191452
```

What is special about using `README.Rmd` instead of just `README.md`?
You can include R chunks like so:

``` r
summary(cars)
#>      speed           dist       
#>  Min.   : 4.0   Min.   :  2.00  
#>  1st Qu.:12.0   1st Qu.: 26.00  
#>  Median :15.0   Median : 36.00  
#>  Mean   :15.4   Mean   : 42.98  
#>  3rd Qu.:19.0   3rd Qu.: 56.00  
#>  Max.   :25.0   Max.   :120.00
```

You’ll still need to render `README.Rmd` regularly, to keep `README.md`
up-to-date. `devtools::build_readme()` is handy for this.

You can also embed plots, for example:

<img src="man/figures/README-pressure-1.png" width="100%" />

In that case, don’t forget to commit and push the resulting figure
files, so they display on GitHub and CRAN.
