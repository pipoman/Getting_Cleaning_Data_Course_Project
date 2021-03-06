{\rtf1\ansi\ansicpg1252\deff0\deflang3082{\fonttbl{\f0\froman\fprq2\fcharset0 Times New Roman;}{\f1\fnil\fcharset2 Symbol;}{\f2\fnil\fcharset0 Courier New;}}
{\*\generator Msftedit 5.41.21.2510;}\viewkind4\uc1\pard\nowidctlpar\lang1033\b\f0\fs28 Getting and Cleaning Data Project\lang1023\b0\fs24\par
\lang1033\b\fs28 CodeBook.MD\lang1023\b0\fs24\par
\par
\lang1033 Author: Pipoman\lang1023\par
\par
\lang1033 Date: 2014-11-17\lang1023\par
\par
\par
\lang1033\b Description\lang1023\b0\par
\par
\pard\nowidctlpar\sl360\slmult1\lang1033 This report provided additional information about variables, data, and transformations used in the course project for the Johns Hopkins Getting and Cleaning Data course.\lang1023\par
\pard\nowidctlpar\par
\lang1033\b Source Data\lang1023\b0\par
\par
\pard\nowidctlpar\sl360\slmult1\lang1033 A full description of the data used in this project can be found at The UCI Machine Learning Repository.\lang1023\par
\lang1033 The source data for this project can be found here:\lang1023\par
\lang1033 https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip. \lang1023\par
\par
\pard\nowidctlpar\lang1033\b Data Set Information\lang1023\b0\par
\par
\pard\nowidctlpar\sl360\slmult1\qj\lang1033 The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.\lang1023\par
\lang1033 The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.\lang1023\par
\par
\pard\nowidctlpar\lang1033\b Attribute Information\lang1023\b0\par
\par
\pard\nowidctlpar\sl360\slmult1\qj\lang1033 For each record in the dataset it is provided:\lang1023\par
\pard\nowidctlpar\fi-360\li720\sl360\slmult1\qj\f1\'b7\tab\lang1033\f0 Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.\lang1023\par
\f1\'b7\tab\lang1033\f0 Triaxial Angular velocity from the gyroscope.\lang1023\par
\f1\'b7\tab\lang1033\f0 A 561- feature vector with time and frequency domain variables.\lang1023\par
\f1\'b7\tab\lang1033\f0 Its activity label.\lang1023\par
\f1\'b7\tab\lang1033\f0 An identifier of the subject who carried out the experiment.\lang1023\par
\pard\nowidctlpar\par
\lang1033\b Section 1. Merge the training and the test sets to create one data set\lang1023\b0\par
\par
\lang1033 After setting the source directory for the files, the data located in\lang1023\par
\lang1033\tab features.txt\lang1023\par
\lang1033\tab activity_labels.txt\lang1023\par
\lang1033\tab subject_train.txt\lang1023\par
\lang1033\tab x_train.txt\lang1023\par
\lang1033\tab y_train.txt\lang1023\par
\lang1033\tab subject_test.txt\lang1023\par
\lang1033\tab x_test.txt\lang1023\par
\lang1033\tab y_test.txt\lang1023\par
\pard\nowidctlpar\sl360\slmult1\lang1033 were read into tables and names were assigned to the columns and the files were merged to create one data set.\lang1023\par
\pard\nowidctlpar\par
\lang1033\b Section 2. Extract only the measurements on the mean and standard deviation for each measurement\lang1023\b0\par
\par
\pard\nowidctlpar\sl360\slmult1\lang1033 Create a logical vector that contains TRUE values for the ID, mean and stdev columns and FALSE values for the others. Subset this data to keep only the necessary columns.\lang1023\par
\pard\nowidctlpar\par
\lang1033\b Section 3. Use descriptive activity names to name the activities in the data set\lang1023\b0\par
\par
\lang1033 Merge data subset with the activityType table to include the descriptive activity names.\lang1023\par
\par
\lang1033\b Section 4. Appropriately label the data set with descriptive activity names.\lang1023\b0\par
\par
\lang1033 Use gsub function for pattern replacement to clean up the data labels.\lang1023\par
\par
\pard\pagebb\nowidctlpar\par
\pard\nowidctlpar\lang1033\b Section 5. Create a second, independent tidy data set with the average of each variable for each activity and each subject.\lang1023\b0\par
\par
\pard\nowidctlpar\sl360\slmult1\lang1033 According to the project instructions, we need to produce only a data set with the average of each variable for each activity and subject,\lang1023\par
\pard\lang11274\f2\fs22\par
}
 