
# CTU Berns R Package universe <a href="https://ctu-bern.r-universe.dev/"><img src='logo.png' align="right" height="200"></a>

R package universes are similar a bit like mini-CRANs. ‘The system
automatically tracks registered git repositories containing R packages,
builds binaries for Windows and MacOS, renders vignettes, and makes all
data available through dashboards, feeds and APIs on personal
subdomains’.

CTU Berns universe is [here](https://ctu-bern.r-universe.dev).

## Packages in the universe

| package                                                                    | status                                                  |
| :------------------------------------------------------------------------- | :------------------------------------------------------ |
| [accrualPlot](https://github.com/CTU-Bern/accrualPlot)                     | ![](https://ctu-bern.r-universe.dev/badges/accrualPlot) |
| [btabler](https://github.com/CTU-Bern/btabler)                             | ![](https://ctu-bern.r-universe.dev/badges/btabler)     |
| [CTUtemplate](https://github.com/CTU-Bern/CTUtemplate)                     | ![](https://ctu-bern.r-universe.dev/badges/CTUtemplate) |
| [HSAr](https://github.com/aghaynes/HSAr)                                   | ![](https://ctu-bern.r-universe.dev/badges/HSAr)        |
| [kpitools](https://github.com/CTU-Bern/kpitools)                           | ![](https://ctu-bern.r-universe.dev/badges/kpitools)    |
| [presize](https://github.com/CTU-Bern/presize)                             | ![](https://ctu-bern.r-universe.dev/badges/presize)     |
| [secuTrialR](https://github.com/SwissClinicalTrialOrganisation/secuTrialR) | ![](https://ctu-bern.r-universe.dev/badges/secuTrialR)  |
| [SwissASR](https://github.com/CTU-Bern/SwissASR)                           | ![](https://ctu-bern.r-universe.dev/badges/SwissASR)    |

## For users…

All vignettes are accessible via the [articles
button](https://ctu-bern.r-universe.dev/ui#articles) on the universe
page.

To use the universe, in R, do the following, which adds the universe to
your list of repos (when installing packages, R will cycle through the
repos until it finds the appropriate package)…

``` r
options(repos = c(CTU = "https://ctu-bern.r-universe.dev",
                  CRAN = "https://cran.rstudio.com/"))
```

It is then possible to install universe packages as if they were CRAN
packages…

``` r
install.packages("accrualPlot")
```

Alternatively, you can install without setting the option:

``` r
install.packages("accrualPlot", repos = "https://ctu-bern.r-universe.dev")
```

## For maintainers…

A dashboard of the included packages and build status can be found
[here](https://ctu-bern.r-universe.dev/ui#builds).

Briefly, packages should be added to [packages.json](packages.json).
They are then tracked on
[r-universe](https://github.com/r-universe/ctu-bern) and built each
hour. [See here for further details of
universes](https://ropensci.org/blog/2021/06/22/setup-runiverse/)

### Acknowledgements

The package logo was created with
[`ggplot2`](https://ggplot2.tidyverse.org/) and
[`hexSticker`](https://github.com/GuangchuangYu/hexSticker).
