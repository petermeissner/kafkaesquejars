
<!-- README.md is generated from README.Rmd. Please edit that file -->

<!-- -->

<!-- FILL OUT OPTIONS !!! -->

<!-- -->

<!-- -->

<!-- -->

# Java Jars for the Package ‘kafkaesque’

**Status**

<a href="https://travis-ci.org/petermeissner/kafkaesquejars"><img src="https://api.travis-ci.org/petermeissner/kafkaesquejars.svg?branch=master"><a/>
[![AppVeyor build
status](https://ci.appveyor.com/api/projects/status/github/petermeissner/kafkaesquejars?branch=master&svg=true)](https://ci.appveyor.com/project/petermeissner/kafkaesquejars)
<a href="https://codecov.io/gh/petermeissner/kafkaesquejars"><img src="https://codecov.io/gh/petermeissner/kafkaesquejars/branch/master/graph/badge.svg" alt="Codecov" /></a>
<a href="https://cran.r-project.org/package=kafkaesquejars">
<img src="http://www.r-pkg.org/badges/version/kafkaesquejars"> </a>
<img src="http://cranlogs.r-pkg.org/badges/grand-total/kafkaesquejars">
<img src="http://cranlogs.r-pkg.org/badges/kafkaesquejars">

*lines of R code:* 5, *lines of test code:* 2

**Version**

2.3.1-2 ( 2020-03-04 23:37:30 )

**Description**

Contents of ‘Kafka-clients’ & supporting Java archives
(<https://github.com/apache/kafka>). The version number of the package
reflects the version number of the included ‘JAR’ file.

**License**

Apache License (\>= 2.0) | file LICENSE <br>Peter Meissner \[aut, cre\],
Marius Pirv \[aut\], virtual7 \[cph\], Apache Software Foundation
\[cph\] (Kafka), Facebook \[cph\] (For Zstandard software, BSD License),
Luben Karavelov \[cph\] (Zstd-jni: JNI bindings to Zstd Library, BSD
2-Clause License)

**Citation**

``` r
citation("kafkaesquejars")
```

``` r
Meissner P, Pirv M (2020). kafkaesquejars: Java Jars for the Package 'kafkaesque'. R package version 2.3.1-2.
```

**BibTex for citing**

``` r
toBibtex(citation("kafkaesquejars"))
```

    @Manual{,
      title = {kafkaesquejars: Java Jars for the Package 'kafkaesque'},
      author = {Peter Meissner and Marius Pirv},
      year = {2020},
      note = {R package version 2.3.1-2},
    }

**Installation**

Stable version from CRAN:

``` r
install.packages("kafkaesquejars")
```

Latest development version from Github:

``` r
devtools::install_github("petermeissner/kafkaesquejars")
```

# Content

## Not much R to see

``` r
library(kafkaesquejars)
```

    ## Loading required package: rJava

``` r
ls("package:kafkaesquejars")
```

    ## character(0)

## Its all about the Java

This package has all the Java dependencies needed for the {kafkaesque}
package.

``` r
system.file(package = "kafkaesquejars", "java") %>% 
  list.files() %>% 
  cat(sep="\n")
```

    ## gson-2.8.6.jar
    ## kafka-clients-2.3.1.jar
    ## logback-classic-1.2.3.jar
    ## logback-core-1.2.3.jar
    ## lz4-java-1.6.0.jar
    ## slf4j-api-1.7.26.jar
    ## snappy-java-1.1.7.3.jar
    ## zstd-jni-1.4.0-1.jar
