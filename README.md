# Vignette-Simulating-a-minimal-SPSS-dataset-from-R

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.


Getting started
=================

To run this example, we’ll need to load {tidyverse}, {surveytoolbox}, and {haven}. Specifically, I’m using {tidyverse} for its data manipulation functions, {surveytoolbox} for functions to set up variable/value labels, and finally {haven} to export the data as a .SAV file.

Note that {surveytoolbox} is currently not available on CRAN yet, but you can install this by running devtools::install_github("martinctc/surveytoolbox"). You’ll need {devtools} installed, if you haven’t got it already.

In addition to loading the packages, we will also set the seed2 with set.seed() to make the simulated numbers reproducible:

library(tidyverse)
library(surveytoolbox) 
library(surveytoolbox)
library(haven)

set.seed(100) # Enable reproducibility - 100 is arbitrary

