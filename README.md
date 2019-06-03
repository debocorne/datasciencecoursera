==================================================================
Human Activity Recognition Using Smartphones Dataset
==================================================================
Debora Cornejo
==================================================================

Variables
======================================


Data set dowloaded from [Human Activity Recognition Using Smartphones Data Set ] (http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.

Following are the objectives:
. Merges the training and the test sets to create one data set.
. Extracts only the measurements on the mean and standard deviation for each measurement.
.Uses descriptive activity names to name the activities in the data set
.Appropriately labels the data set with descriptive variable names.
From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
.run_analysis.R has following step by step logic to produce the TidyData.txt file contains the expected data set

Load the activity label and features files.
Load the all the files belongs to both test and train.
union the test and train using rbind command.
assign respective label to activity , subject and the variable names.
filter only mean() and std() variables.
replace the activity number with respective activity label using left_join command.
column bind the activity , subject and variables tables into one single table.
calculate the mean of the each group by subject and activity using group_by and summarise_each

and also write the results in TidyData.txt file
