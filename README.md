
## `drat` Repository for `Neuronorm` dependencies!

`drat` ([CRAN](https://cran.r-project.org/package=drat), [GitHub](https://github.com/eddelbuettel/drat), [docs](https://eddelbuettel.github.io/drat)) makes it easy to host your own CRAN-like repositories for packages (or [data](https://journal.r-project.org/archive/2017/RJ-2017-026/index.html)).

## R Packages in this drat

This repository contains the dependencies version of the [`NeuroNorm`](https://github.com/DavidPayares/neuronorm) package.
- [x] [NeuroData](https://github.com/DavidPayares/neurodata)
- [x] [ANTsR](https://github.com/stnava/ANTsR/releases/)
- [x] [ITKR](https://github.com/stnava/ITKR)
- [x] [extrantsr](https://github.com/muschellij2/extrantsr/releases/)
- [x] [MNITemplate](https://github.com/Jfortin1/MNITemplate)
- [x] [RAVEL](https://github.com/Jfortin1/RAVEL)

## Installation

You can install all the packages in this repo by using the standard R function `install.packages`. In case a package does not install correctly, please refer to its corresponding GitHub page. Make sure the packages `ANTsRCore` and `fslr` are already installed. 

``` r
# Install ANTsCore
devtools::install_github('stnava/ANTsRCore')
# Install FSLR
devtools::install_github('muschellij2/fslr')

# Install drat with packages
packages = c("ITKR", "ANTsR","extrantsr","RAVEL","MNITemplate","neurodata")
install.packages(packages, repos = 'https://davidpayares.github.io/drat', type = "source")
```
