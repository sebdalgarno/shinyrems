
<!-- README.md is generated from README.Rmd. Please edit that file -->

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![License:
MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

# shinyrems

`shinyrems` is an app that allows you to visualize and download data
from the EMS database.

#### Follow these instructions to run the app:

First let’s install the package\! Paste the following into the console:

``` r
if(!"drat" %in% installed.packages()[,1]) install.packages("drat")
drat::addRepo("poissonconsulting")
install.packages("shinyrems")
```

The app can be run in 4 modes:

  - “demo”
  - “2yr”
  - “historic”
  - “all”

Each mode has different data requirements. If running app in “2yr”,
“historic” or “all” mode, you will be prompted to download or update
the data onto your machine prior to the app being launched. This
requires internet\! In the case of “historic” and “all”, the data
downloaded is in excess of 4gb\!

To simply run the app without having to download any data first, use
“demo” mode:

    shinyrems::run_app(run_mode = "demo")

For the other modes, simply substitute “demo” with another run\_mode,
e.g.:

    shinyrems::run_app(run_mode = "2yr")

## Contribution

Please report any
[issues](https://github.com/poissonconsulting/shinyrems/issues).

[Pull requests](https://github.com/poissonconsulting/shinyrems/pulls)
are always welcome.

Please note that this project is released with a [Contributor Code of
Conduct](CONDUCT.md). By participating in this project you agree to
abide by its terms
