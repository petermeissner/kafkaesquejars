This is a resubmission


## Test environments
* local R installation, R 3.6.3
* ubuntu 16.04 (on travis-ci), oldrel, release, devel
* win-builder (devel)
* win-builder (release)


## R CMD check results

0 errors | 0 warnings | 1 note

* This is a new release.


## Your Comments

Thanks, we see:

   Package has FOSS license, installs .class/.jar but has no 'java'
directory.

   Size of tarball: 10025277 bytes

Not more than 5 MB for a CRAN package, please.

Please fix and resubmit.



## My Comments and Actions Taken

- Directory ./inst/java created and file sources.md added. sources.md contains 
a list of URLs where any user can download the source code of the jar files 
contained in ./inst/java and distributed with the package.

- Since the Java dependencies make the package tarbal larger than 5 MB only 
dependencies essential for running have been included and the 
package has been split into two packages. This package "kafkaesqujars" only 
contains the dependency jars while the kafkaesque package to be published 
later on will contain the actual Java code. I think this is in line with 
common practice and advice for packages making use of Java code. 