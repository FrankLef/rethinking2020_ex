# rethinking2020

[![Lifecycle: stable](https://img.shields.io/badge/lifecycle-stable-brightgreen.svg)](https://lifecycle.r-lib.org/articles/stages.html) [![R 4.2.1](https://img.shields.io/badge/R-4.2.1-blueviolet.svg)](https://cran.r-project.org/bin/windows/base/)

`rethinking2020_ex` is a set of solutions fro the practices found in 
*Statistical Rethinking*, second edition, by Richard McElreath.

These solutions are home-made and have not been reviewed or approved in any way.

## Aknowledgement

Many thanks to Richard McElreath who wrote *Statistical Rethinking* to make Bayesian statistics so interesting.

This study project is inspired by *Solomon Kurtz* who did wonderful work. It can be found at [Solomon Kurtz](https://bookdown.org/content/3890/).

## Packages

The packages used in this project are as follows.

### Modelizations and data processing

| Package                                                                | Comment                                                                                                                                                                                        |
|--------------------|----------------------------------------------------|
| [rethinking](https://github.com/rmcelreath/rethinking)                 | This R package accompanies a course and book on Bayesian data analysis: McElreath 2020. Statistical Rethinking, 2nd edition.                                                                   |
| [brms](https://paul-buerkner.github.io/brms/)                          | Used to do pretty much all models and computations.                                                                                                                                            |
| [loo](http://mc-stan.org/loo/index.html)                               | Used by both `rethinking` and `brms` to compute WAIC and LOO. See section 7.5 in chapter for more details.                                                                                     |
| [posterior](https://mc-stan.org/posterior/)                            | Used to work with the output of Bayesian models.                                                                                                                                               |
| [tidybayes](http://mjskay.github.io/tidybayes/articles/tidybayes.html) | Bayesian statistics do require a lot of data processing. `tidybayes` is incredibly helpful in providing a constant and efficient way of coding the data processing.                            |
| [bayestestR](https://easystats.github.io/bayestestR/)                  | A comprehensive and consistent set of functions to analyze and describe posterior distributions.                                                                                               |
| [tidyverse](https://www.tidyverse.org)                                 | **The** package for data science in general.                                                                                                                                                   |
| [extraDistr](https://github.com/twolodzko/extraDistr)                  | has many extra distributions such as BetaBinom, NegBetaBinom, HalfCauchy, ZIP, Pareto, etc. which are useful in real-world applications and usually dispersed amongst many different packages. |

### Visualizations

| Package                                                 | Comment                                                                                                                                                                    |
|-------------------|-----------------------------------------------------|
| [ggdist](https://mjskay.github.io/ggdist/)              | `tidybayes` relies heavily on the `ggdist` and reexport very many of it's functions. In addition `ggdist` is useful for both a frequencist as well as a bayesian approach. |
| [bayesplot](https://mc-stan.org/bayesplot/)             | Used as complement when `ggdist` and `tidybayes` do not provide a satisfactory solution.                                                                                   |
| [ggplot2](https://ggplot2.tidyverse.org)                | Vizualisations using the grammar of graphics.                                                                                                                              |
| [scales](https://scales.r-lib.org)                      | Provide the internal scaling infrastructure used by `ggplot2`                                                                                                              |
| [paletteer](https://github.com/EmilHvitfeldt/paletteer) | A nice package to manage color and shape palettes.                                                                                                                         |

### Miscellaneous

| Package                                                                  | Comment                                                                                                 |
|------------------------------|------------------------------------------|
| [xfun](https://cran.r-project.org/web/packages/xfun/vignettes/xfun.html) | The function `xfun::cache_rds` is used for caching which is used several times in almost every chapter. |
