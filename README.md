This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

This problem set is based on the content of the paper "How Are You, My Dearest Mozart? Well-Being and Creativity of Three Famous Composers Based on Their Letters." and the corresponding replication data written by Karol Jan Borowiecki (2017). 
Its aim is to investigate if (negative)emotions influenced the creativity of three world-famous composers Wolfgang Amadeus Mozart, Ludwig van Beethoven and Franz Liszt.  In addition to the interactive econometric analysis of Borowiecki's results, it also considers a growing economic analysis method - automated text analysis - with the package [*quanteda*](https://quanteda.io/) The interactive structure of the problemset together with descriptions of economic theory and explanations of R commands grant a diversified and informative journey through the topic.

The paper can be found online at https://doi.org/10.1162/REST_a_00616 .

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.

```s
install.packages("RTutor",repos = c("https://skranz-repo.github.io/drat/",getOption("repos")))

if (!require(devtools))
  install.packages("devtools")

devtools::install_github("DKlinke/RTutorCreativity")
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.

```s
library(RTutorCreativity)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorCreativity")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorCreativity",
       auto.save.code=TRUE, clear.user=FALSE)
```

If everything works fine, a browser window should open, in which you can start exploring the problem set.
