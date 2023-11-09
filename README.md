
<!-- README.md is generated from README.Rmd. Please edit that file -->

# `pifpaf`: Estimation of Potential Impact Fractions (pif) and Population Attributable Fractions (paf) <img src="man/figures/logo.png"  style="float:right; height:135px;" alt="" />

**THIS IS STILL A WORK IN PROCESS**

<!-- badges: start -->

[![Project Status: Active – The project has reached a stable, usable
state and is being actively
developed.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
[![metacran
downloads](https://cranlogs.r-pkg.org/badges/last-week/pifpaf)](https://cran.r-project.org/package=pifpaf)
[![Codecov test
coverage](https://codecov.io/gh/RodrigoZepeda/pifpaf/branch/main/graph/badge.svg)](https://app.codecov.io/gh/RodrigoZepeda/pifpaf?branch=main)
[![CRAN
status](https://www.r-pkg.org/badges/version/pifpaf)](https://CRAN.R-project.org/package=pifpaf)
<!-- badges: end -->

> The `pifpaf` package corresponds to an **update** on the previous
> [homonimous package](https://github.com/INSP-RH/pifpaf) developed at
> INSP.

# Installation

You can install the development version of `pifpaf` from
[GitHub](https://github.com/pifpaf) with:

``` r
#install.packages("remotes")
remotes::install_github("RodrigoZepeda/pifpaf", dependencies = TRUE)
```

# Usage

The main purpose of the package is to calculate **potential impact
fractions** and **population attributable fractions** for a specific
case: when the exposure information comes from cross-sectional studies
(in particular, surveys) and the relative risk information from the
literature (*e.g.* metanalysis).

In our package we assume the user has access to the data either as
**individual-level** exposure (*e.g.* the user has access to the survey)
or the user has access to **aggregated data** on the exposure (*e.g.*
the user has the population-mean exposure and its confidence interval).
The following table shows which function to use depending on the case:

| **Exposure data**                          | Population Attributable Fraction           | Potential Impact Fraction           |
|--------------------------------------------|--------------------------------------------|-------------------------------------|
| [Individual-level](#individual-level-data) | [`paf`](#population-attributable-fraction) | [`pif`](#potential-impact-fraction) |
| [Aggregated](#aggregated-data)             | `paf_approximate`                          | `pif_approximate`                   |

> **Note** If the user has available both **individual-level** and
> **aggregated data** they should prefer the **individual-level**
> information as it captures better the sample’s variability. The
> population attributable fraction and potential impact fractions
> estimated from **aggregated data** are only approximations and are
> biased estimates.

## Individual-level data

### Population Attributable Fraction

### Potential Impact Fraction

### Model’s diagnostics

## Aggregated data

**WORK IN PROGRESS**
