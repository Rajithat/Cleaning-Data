<H1> Code Book for Run Analysis

The dataset is based on data from [1], downloaded from here

The goal of the project is to  prepare tidy data that can be used for later analysis. 
The Train and Test data sets are downloaded and merged to create one data set

<h3> The following files were merged into test data table
* test\X_test.txt
* test\y_test.txt, 
* test\subject_test.txt 

<h3> The following files were merged into test data table
* test\X_train.txt 
* test\y_train.txt 
* test\subject_train.txt 

The features corresponding to the variables are extracted from features.txt

Only the measurements on the mean and standard deviation for each measurement were extracted from both training and test data tables and combined into a single table (also including columns with corresponding subject ids and activity labels).

A second, data set with the average of each variable for each activity and each subject was created. The rows were reodered so that activities performed by each subject are in adjacent rows.
Each activity label was replaced with corresponding activity name from activity_labels.txt.

Column names:

Subject: .. range of values [1:30] .. id of a subject performing ther activity
Activity: .. Name of activity performed
Rest of the coluns corespond to averaged variables describing mean/std measurements. E.g. tGravityAcc-mean()-X tGravityAcc-mean()-Y tGravityAcc-mean()-Z tGravityAcc-std()-X tGravityAcc-std()-Y tGravityAcc-std()-Z

Names of these variables are same as in features.txt but the values are averages of each variable for each activity and each subject.
