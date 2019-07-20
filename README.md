
# noiris <img src="data-raw/noiris.png" style="margin: 0 auto; width: 10%">

This package is primarily to provide data that is more similar to what
many people would typically come across in the wild, or is simply more
interesting or accessible (in my opinion), and more useful for
instruction and workshops. Far too often examples use `iris`, `mtcars`,
etc. for convenience, but these are actually inconvenient for
demonstrating common data and modeling problems, or are too small to
even be realistic.

This package will provide larger and at some point messier data. The
bias is towards data that could be understood regardless of
discipline/background. In addition, it should have minimally several
hundred observations, and often much larger, but not so large that
analysis or data processing demonstration would take an inordinate
amount of time. However, it should have relatively few columns (unless
for demonstration of a ‘large p’ type of problem/analysis,
e.g. penalized regression.).

## Data

In most cases the data has been cleaned up to make it easier to use and
understand.

Right now it has:

  - `gapminder_2019`: a 2019 pull from
    [gapminder.org/data](http://www.gapminder.org/data/).
      - A nice longitudinal/time-series data set suitable for a wide
        range of standard and more complex mixed models, spatial
        visualization and analyses, etc.
  - `star_wars`: several data sets based on the [Star Wars
    API](https://swapi.co/).
      - Mostly just for fun, but it demonstrates usage of list columns
        and otherwise could be good for demonstrating joins.
  - `instructor_evaluations`: a nice-sized data set for
    mixed/multi-level modeling taken from the `lme4` package.
      - Good for mixed models and similar.
  - `fish`: Number of fish caught on camping trips.
      - An accessible data set useful for demonstrating count models
        including zero-inflated/hurdle models.
  - `pisa`: OECD’s Programme for International Student Assessment with
    international scores for math, science, and reading, covering years
    2000-2015.
      - Potentially good for demonstrating nonlinear relationships
        (e.g. GAM), imputing missing data, longitudinal/spatial
        analyses.
  - `world_happiness`: Multiyear data set with country level scores of
    ‘happiness’. From 2019 World Happiness Report, and includes data
    from 2005-2018.
      - Similar to Gapminder and PISA, this could be used for a variety
        of standard statistical models.
  - `sp500`: Daily S & P 500 data for a 10 year period covering +- 5
    years before and after the Great Recession low.
      - Good for time series and related analyses. Includes industry
        classifications.
  - `wine_reviews`, `wine_quality`: Two data sets regarding wine reviews
    that can be used for a wide range of standard statistical and
    machine learning.
      - Can be used for standard regression and classification, ordinal
        regression, text analysis, sentiment analysis.
  - `google_apps`: Ratings and other information for Google Play Store
    apps.
      - Text & sentiment analysis, standard regression, etc.
  - `fashion_train`, `fasion_test`: The ‘Fashion MNIST’. Image data for
    clothing items.
      - Image classification, cluster analysis
  - `gender_gap`, `gender_gap_2018`: Country level data regarding the
    World Bank Gender Gap Index.
      - Longitudinal analysis, geospatial analysis, etc.

## Installation

This package is not on CRAN. To install:

``` r
devtools::install_github('m-clark/noiris')
```

## Other

To do:

  - \[X\] Data for basic classification
  - \[X\] Data for basic machine learning (reg and class)
  - \[X\] Data for text analysis (more to come)
  - \[X\] Data for image classification
  - \[ \] Data for survival analysis
  - \[ \] Data for factor analysis/SEM (PCA?)
  - \[ \] Data Non-obvious cluster analysis (no iris\! and no old
    faithful either\!)
