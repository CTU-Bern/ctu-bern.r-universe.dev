# CTU Berns R Package universe

[See here for details of universes](https://ropensci.org/blog/2021/06/22/setup-runiverse/)

Briefly, packages should be added to [packages.json](packages.json). They are then tracked on [r-universe](https://github.com/r-universe/ctu-bern) and built each hour. A dashboard of the included packages and build status can be found [here](https://ctu-bern.r-universe.dev/ui#builds).

To use the universe, in R, do the following...

```r
options(repos = c(CTU = "https://ctu-bern.r-universe.dev",
                  CRAN = "https://cran.rstudio.com/"))
```

