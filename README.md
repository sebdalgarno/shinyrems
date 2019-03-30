
<!-- README.md is generated from README.Rmd. Please edit that file -->

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![License:
MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

# shinyrems

`shinyrems` provides an app which serves as an interface to the `rems` R
package and ems database.

#### To run the app, paste the following into an R console

``` r
# install.packages("drat")
drat::addRepo("poissonconsulting")
devtools::install_github("poissonconsulting/shinyrems")
# you can now run the app with.
shinyrems::run_app()
# by default the above runs the app in 'demo' mode using a small dataset that doesn't require downloading.
# to access the '2 year' dataset (data from 2018-01-01 to present), use:
shinyrems::run_app(run_mode = "2yr")
# to access the 'historic' dataset (data from 1964-01-01 to 2018-01-01), use:
shinyrems::run_app(run_mode = "historic")
# to access all data (data from 2018-01-01 to present), use:
shinyrems::run_app(run_mode = "2yr")
```

## Contribution

Please report any
[issues](https://github.com/poissonconsulting/shinyrems/issues).

[Pull requests](https://github.com/poissonconsulting/shinyrems/pulls)
are always welcome.

Please note that this project is released with a [Contributor Code of
Conduct](CONDUCT.md). By participating in this project you agree to
abide by its terms
