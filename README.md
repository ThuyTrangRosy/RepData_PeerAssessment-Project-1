# RepData_PeerAssessment-Project-1
**Loading and preprocessing the data**
Show any code that is needed to

Load the data (i.e. 
read.csv()
read.csv())

Process/transform the data (if necessary) into a format suitable for your analysis
library("tidyr");library("stringr");library("plyr");library("dplyr");library("knitr")
library(lattice)
ctivity <- read.csv("activity.csv")
activity_na_false <- na.omit(activity)
activity_na_true <- subset(activity,is.na(activity$steps) == TRUE)
nrow(activity)
## [1] 17568
nrow(activity_na_false) + nrow(activity_na_true)
## [1] 17568
