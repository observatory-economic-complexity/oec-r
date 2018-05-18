
<!-- README.md is generated from README.Rmd. Please edit that file -->
OEC R package <img src="http://pacha.hk/oec-r-package/observatory.png" width=150 align="right" alt="sticker"/>
==============================================================================================================

[![mitlicense](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) [![Build Status](https://travis-ci.org/pachamaltese/oec-r-package.svg?branch=master)](https://travis-ci.org/pachamaltese/oec-r-package) [![Build status](https://ci.appveyor.com/api/projects/status/5xvlffxy8ro4wc34?svg=true)](https://ci.appveyor.com/project/pachamaltese/oec) [![cran checks](https://cranchecks.info/badges/summary/oec)](https://cran.r-project.org/web/checks/check_results_oec.html) [![CRAN downloads](http://cranlogs.r-pkg.org/badges/oec)](http://cran.rstudio.com/web/packages/oec/index.html) [![CRAN downloads](http://cranlogs.r-pkg.org/badges/grand-total/oec)](http://cran.rstudio.com/web/packages/oec/index.html)

`oec` provides an easy way to obtain data from the [Observatory of Economic Complexity](http://atlas.media.mit.edu/en/) by accessing its API.

Installation
------------

``` r
# Install release version from CRAN
install.packages("oec")

# Install development version from GitHub
devtools::install_github("pachamaltese/oec-r-package")
```

Usage
-----

Please read the vignette for a detailed user guide.

``` r
library(oec)

# What does Chile export to China?  
# year 2015 - SITC (4 characters)
getdata("chl", "chn", 2015)

# What does Chile export to China?  
# years 2010 to 2015 - SITC (4 characters)
getdata_batch("chl", "chn", 2010, 2015)
```

The MIT License
---------------

Copyright (c) 2016, Mauricio "Pachá" Vargas

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
