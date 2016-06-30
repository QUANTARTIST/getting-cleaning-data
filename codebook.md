#Getting and Cleaning Project Codebook
QUANTARTIST | 30 June, 2016

###Data Source

A full description of the data used in this project can be found at The UCI Machine Learning Repository.
The source data for this project can be found at:

https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

###Dataset

Eah record in the dataset contains the following attributes:

1. Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration
2. Triaxial Angular velocity from the gyroscope
3. A 561-feature vector with time and frequency domain variables
4. Its activity label
5. An identifier of the subject who carried out the experiment

###Load Files

Read the following files into R, assign column names and combine into one dataset:

features.txt
activity_labels.txt
subject_train.txt
x_train.txt
y_train.txt
subject_test.txt
x_test.txt
y_test.txt

###Extract mean, standard deviation for each measurement

Form a logcal vector that contains TRUE values for the ID, mean and stdev columns and FALSE values for the remaining columns.
Subset this data to keep only the required columns.

###Use descriptions to name the activities in the dataset

Merge data subset with activityType table in order to inlude the descriptive activity descriptor

###Create a second, independent tidy dataset with the average of each variable for each activity and each subject

Produce one data set with the average of each veriable for each activity and subject



