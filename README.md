==================================================================
Human Activity Recognition Using Smartphones Dataset
==================================================================
Debora Cornejo
==================================================================

Variables
======================================


download.data = extract data

targetFolder <- contain path

test.data <- read.table
test.activities <- read.table
test.subjects <- read.table

train.data <- read.table
train.activities <- read.table
train.subjects <- read.table

data.data <- Bind the rows for each of the data sets together
data.activities <- Bind the rows for each of the data sets together
data.subjects <- Bind the rows for each of the data sets together


full_data <- Now combine all of the different columns together into one table

features <- Grab the complete list of features

requiredFeatures <- Filter to the features we want

full_data <- Extracts only the measurements on the mean and standard deviation for each measurement

activities <- Read in the activity labels

full_data[, 2] <- Update the activity name

colnames(full_data) <- Appropriately labels the data set with descriptive variable names

final.total <- Total the data so we have a unique row for each combination of subject and activites

final.mean <- Cast it getting the mean value