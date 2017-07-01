
## TensorFlow for R

[![Travis-CI Build Status](https://travis-ci.org/rstudio/tensorflow.svg?branch=master)](https://travis-ci.org/rstudio/tensorflow) [![CRAN_Status_Badge](https://www.r-pkg.org/badges/version/reticulate)](https://cran.r-project.org/package=reticulate) 


[TensorFlow™](https://tensorflow.org) is an open source software library for numerical computation using data flow graphs. Nodes in the graph represent mathematical operations, while the graph edges represent the multidimensional data arrays (tensors) communicated between them. The flexible architecture allows you to deploy computation to one or more CPUs or GPUs in a desktop, server, or mobile device with a single API. 

The [TensorFlow API](https://www.tensorflow.org/api_docs/python/index.html) is composed of a set of Python modules that enable constructing and executing TensorFlow graphs. The tensorflow package provides access to the complete TensorFlow API from within R. 

## Installation

To get started, install the tensorflow R package from GitHub as follows:

```r
devtools::install_github("rstudio/tensorflow")
```

Then, use the `install_tensorflow()` function to install TensorFlow:

```r
library(tensorflow)
install_tensorflow()
```

You can confirm that the installation succeeded with:

```r
sess = tf$Session()
hello <- tf$constant('Hello, TensorFlow!')
sess$run(hello)
```

This will provide you with a default installation of TensorFlow suitable for getting started with the tensorflow R package. See the [article on installation](https://tensorflow.rstudio.com/installation.html) to learn about more advanced options, including installing a version of TensorFlow that takes advantage of Nvidia GPUs if you have the correct CUDA libraries installed.

## Documentation

See the package website for additional details on using the TensorFlow API from R: <https://tensorflow.rstudio.com>

See the TensorFlow API reference for details on all of the modules, classes, and functions within the API: <https://www.tensorflow.org/api_docs/python/index.html>

The tensorflow package provides code completion and inline help for the TensorFlow API when running within the RStudio IDE. In order to take advantage of these features you should also install the [Current Release](https://www.rstudio.com/products/rstudio/download/) of RStudio.




