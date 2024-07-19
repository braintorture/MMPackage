# MMPackage
Contains the function to sag "Let's see whats is your BMI!" and create BMI groups.


# Instalation
You can install the development version of regexcite from GitHub with:
``` r
#install.packages("remotes")
remotes::install_github("braintorture/MMPackage")
```

## Usage
```{r}
library(MMPackage)
```
```{r}
Start <- function() {
  print("Let's see whats is your BMI!")
}
```

```{r}
bmi3 <- function(x) {
  bmi.groups <- cut(x, breaks = c(0, 25, 30, Inf), right = FALSE)
  return(bmi.groups)
}

```
