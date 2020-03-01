<!-- README.md is generated from README.Rmd. Please edit that file -->

foofactors
==========

<!-- badges: start -->
<!-- badges: end -->

The goal of foofactors is to make factors less aggravating (& learn
about package development).

Installation
------------

And the development version from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("toddellis/foofactors")
```

Example
-------

This is a basic example which shows you how to solve a common problem:

### fbind()

``` r
library(foofactors)

a <- iris$Species[c(1, 51, 101)]
b <- PlantGrowth$group[c(1, 11, 21)]

fbind(a, b)
#> [1] setosa     versicolor virginica 
#> [4] ctrl       trt1       trt2      
#> 6 Levels: ctrl setosa trt1 ... virginica
```

### fcount()

``` r
fcount(iris$Species)
#> # A tibble: 3 x 2
#>   f              n
#>   <fct>      <int>
#> 1 setosa        50
#> 2 versicolor    50
#> 3 virginica     50
```
