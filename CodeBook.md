Code Book :
===========

This code book includes information about the source data, the transformations performed post collection of the data and some information about the variables of the resulting data sets.

Coding Details :
----------------

The source data was collected from the [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones) to complete an assignment for a Coursera course named Getting and Cleaning Data instructed by Prof.Jeff Leek. The assignment involves working with the [UCI HAR Dataset](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) and producing a tidy data representation of the source data. A Detailed list of the tasks performed to arrive at the tidy data are enlisted as below.

1. Download the [UCI HAR Dataset](https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip) file as mentioned in the discription above
2. Unzip the data set into the chosen working directory
3. Set your working directory to the respective path where the dataset has been unzipped.
3. Load test and training data labels y_train.txt to b_train and y_test.txt to b_test
4. Load the text files, features.txt to features and activity_labels.txt to activity_labels which is the  list all the features and the text file that Links the class labels with their activity name
5. Load the text files that contain the datasets ie., subject_train.txt to subject_train  and subject_test.txt subject_test
6. Now,Load the Test and Training Data Sets X_train.txt to a_train and X_test.txt to a_test

Now the analysis will be done in two parts:
     Part1 : Analysis of 70% of the Volunteer select for generating the training data
     Part2 : Analysis of 30% of the Volunteer select for generating the test data 
    
Part1 : Analysis of 70% of the Volunteer select for generating the training data

    1. Nominate the columnnames
8. Replace the activity IDs with the activity labels to render readability
9. Combine the Test and Training data frames to produce one data frame containing the subjects, measurements and activities
10. Arrive at the "mergedtidydata.txt" with the combined data frame as the first expected output
11. Create one more data set using the data.table library of R thereby grouping the tidy data by subject and activity
12. Apply the mean and standard deviation calculations across all the groups
13. Arrive at the final "calculatedtidydata.txt" as the final required output to complete the assignment.

Please refer to run_analysis.R for implementation details.

Variables Involved: 
-------------------

- subjectId: 1 to 30 each representing a participant in the study
- activity: the activity that the subject was doing at the time of the measurement
- tBodyAcc-mean-X        
- tBodyAcc-mean-Y
- tBodyAcc-mean-Z
- tBodyAcc-std-X
- tBodyAcc-std-Y
- tBodyAcc-std-Z
- tGravityAcc-mean-X
- tGravityAcc-mean-Y
- tGravityAcc-mean-Z
- tGravityAcc-std-X
- tGravityAcc-std-Y
- tGravityAcc-std-Z
- tBodyAccJerk-mean-X
- tBodyAccJerk-mean-Y
- tBodyAccJerk-mean-Z
- tBodyAccJerk-std-X
- tBodyAccJerk-std-Y
- tBodyAccJerk-std-Z
- tBodyGyro-mean-X
- tBodyGyro-mean-Y
- tBodyGyro-mean-Z
- tBodyGyro-std-X
- tBodyGyro-std-Y
- tBodyGyro-std-Z
- tBodyGyroJerk-mean-X
- tBodyGyroJerk-mean-Y
- tBodyGyroJerk-mean-Z
- tBodyGyroJerk-std-X
- tBodyGyroJerk-std-Y
- tBodyGyroJerk-std-Z
- tBodyAccMag-mean
- tBodyAccMag-std
- tGravityAccMag-mean
- tGravityAccMag-std
- tBodyAccJerkMag-mean
- tBodyAccJerkMag-std
- tBodyGyroMag-mean
- tBodyGyroMag-std
- tBodyGyroJerkMag-mean
- tBodyGyroJerkMag-std
- fBodyAcc-mean-X
- fBodyAcc-mean-Y
- fBodyAcc-mean-Z
- fBodyAcc-std-X
- fBodyAcc-std-Y
- fBodyAcc-std-Z
- fBodyAccJerk-mean-X
- fBodyAccJerk-mean-Y
- fBodyAccJerk-mean-Z
- fBodyAccJerk-std-X
- fBodyAccJerk-std-Y
- fBodyAccJerk-std-Z
- fBodyGyro-mean-X
- fBodyGyro-mean-Y
- fBodyGyro-mean-Z
- fBodyGyro-std-X
- fBodyGyro-std-Y
- fBodyGyro-std-Z
- fBodyAccMag-mean
- fBodyAccMag-std
- fBodyBodyAccJerkMag-mean
- fBodyBodyAccJerkMag-std
- fBodyBodyGyroMag-mean
- fBodyBodyGyroMag-std
- fBodyBodyGyroJerkMag-mean
- fBodyBodyGyroJerkMag-std
