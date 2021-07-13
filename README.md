Congress by Election Year
================
Jeremiah Cha

A simple dataset that pairs each session of the U.S. Congress with their
election years. Additional variables include the start and end of the
term.

# Installing

Start by downloading the `.csv`, `.dta` or `.rds` file in this
repository. Importing the `.dta` format into R requires external
packages, such as
[`haven`](https://cran.r-project.org/web/packages/haven/haven.pdf). The
`.rds` file can be read into R with the following code.

``` r
df <- readRDS("congyear.rds")
```

Reading in the `.rds` file imports a tibble, which is compatible with
the `tidyverse` suite. A preview of the data is featured below.

``` r
library(tidyverse)
df
```

    ## # A tibble: 117 x 4
    ##    congress e_year term_start term_end
    ##       <int>  <int>      <int>    <int>
    ##  1        1   1788       1789     1791
    ##  2        2   1790       1791     1793
    ##  3        3   1792       1793     1795
    ##  4        4   1794       1795     1797
    ##  5        5   1796       1797     1799
    ##  6        6   1798       1799     1801
    ##  7        7   1800       1801     1803
    ##  8        8   1802       1803     1805
    ##  9        9   1804       1805     1807
    ## 10       10   1806       1807     1809
    ## # … with 107 more rows
