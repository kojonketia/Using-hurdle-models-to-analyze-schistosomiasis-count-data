# Using-hurdle-models-to-analyze-schistosomiasis-count-data
The model codes and analysis for the paper "Using hurdle models to analyze schistosomiasis count data of school children in the southern areas of Ghana" are presented here. It is a combination of Python and R codes.

# Files

The Rmd file contains the model codes used. Six distinct models under different scenarios were used.

The python (jupyter) file contains codes used for slicing dataframes, descriptive statistics and fugure plotting

## Methods

### Rmd

The standard Poisson, negative binomial (NB), zero-inflated Possion (ZIP), zero-inflated negative binomial (ZINB), hurdle Poisson (HP), hurdle negative binomial (HNB) models are the various models used.

Their corresponding R syntax is 

```
Poisson = "glm("dependent variable ~ x1 + x2 + ... + xn", family = 'poisson', data = count_data)"

NB = "glm("dependent variable ~ x1 + x2 + ... + xn", family = negative.binomial(1), data = count_data"

ZIP = "zeroinfl(dependent variable ~ x1 + x2 + ... + xn, data = count_data, dist = "poisson")"

ZINB = "zeroinfl(dependent variable ~ x1 + x2 + ... + xn, data = count_data, dist = "negbin")"
```

