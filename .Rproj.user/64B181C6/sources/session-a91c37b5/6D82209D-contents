library(tidyverse)
library(readr)

# load heart disease data from data raw
HeartDisease <- read_csv("data_raw/heart-disease.csv")

# change column name 'sex' to 'gender'
colnames(HeartDisease)[colnames(HeartDisease) == 'sex'] <- 'gender'

# remove duplicate rows
HeartDisease <- unique(HeartDisease)

# change columns from integers to factors
change_col <- c('gender','target', 'cp', 'fbs', 'restecg', 'exang', 'slope', 'ca', 'thal')
HeartDisease[change_col] <- lapply(HeartDisease[change_col], as.factor)

# save to data file
usethis::use_data(HeartDisease)

