
<!-- README.md is generated from README.Rmd. Please edit that file -->

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![License:
MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

# shinyrems

`shinyrems` is an app that allows you to visualize and download data
from the EMS database.

#### Follow these instructions to run the app:

First let’s install the most recent versions of `rems` and `shinyrems` R
packages. Paste the following lines into the console, one at a
time:

``` r
if(!"devtools" %in% installed.packages()[,1])  install.packages("devtools")
devtools::install_github("bcgov/rems")
if(!"drat" %in% installed.packages()[,1]) install.packages("drat")
drat::addRepo("poissonconsulting")
install.packages("shinyrems")
```

The app has 4 run modes:

  - **“demo”**
  - **“2yr”**
  - **“historic”**
  - **“all”**

Each run mode has different data requirements.

  - If using **“2yr”**, **“historic”** or **“all”** run mode, you will
    be prompted to download or update the data onto your machine prior
    to the app being launched. This requires internet\!

  - If using **“historic”** and **“all”**, the data downloaded is in
    excess of 4gb\!

  - If you only require data since 2018-01-01, the **“2yr”** run mode
    works with a smaller dataset and the app will run a little faster.

To simply run the app without having to download any data first, use the
“demo” run mode:

    shinyrems::run_app(run_mode = "demo")

For the other run modes, simply substitute “demo” with one of the other
options, e.g.:

    shinyrems::run_app(run_mode = "2yr")

## Contribution

Please report any
[issues](https://github.com/poissonconsulting/shinyrems/issues).

[Pull requests](https://github.com/poissonconsulting/shinyrems/pulls)
are always welcome.

Please note that this project is released with a [Contributor Code of
Conduct](CONDUCT.md). By participating in this project you agree to
abide by its terms
