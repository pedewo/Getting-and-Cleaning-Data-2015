# Code Book

This document describes the code inside `run_analysis.R`.
run_analysis.R take data downloaded from a website, processes the data and generates a tidy data set

# Data Source
The data comes from the accelerometers from the Samsung Galaxy S smartphone. 
A full description of the data is available at the site where the data was obtained:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
The data was obtained from:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

# Source Code
The R script is using the library reshape2.
Files activity_labels.txt, features.txt are loaded.
Data on the mean and the standard deviation are extracted using grep
Descriptive activity names are creating using gsub
Datasets are factorized using factor.
Melt function is used to transform data set from wide-format to long-format

# Output to file
Tranformed and cleaned data set is written to the file tidy.txt
