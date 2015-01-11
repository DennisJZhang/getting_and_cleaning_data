## Codebook for full_data.csv and tidy.csv

### Data Cleaning for full_data.csv

The original data is from Human Activity Recognition Using Smartphones Dataset Version 1.0. More information can be found on http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The process of generating full_data.csv from Human Activity Recognition Using Smartphones Dataset:
*Combine the feature and label data from both test and train groups in the original data set.
*Pick variables related to mean and standard deviatoins of measurements in the original data set.
*Remane variable names to reflect activity, subject, and measures. 

### Data Cleaning for tidy.csv
tidy.csv is generated from full_data.csv
The process of generating tidy.csv:
*tidy.csv contains the mean of all measurements in full_data.csv for each subject and each activity.

### Variable Names:
activity:
*The activity that subject is performing. The activity includes "WALKING", "WALKING_UPSTAIRS", "WALKING_DOWNSTAIRS", "SITTING", "STANDING", "LAYING".

subject:
*The number of subjects that perform those activities.

other measures:
These measures includes "tBodyAcc-mean()-X, tBodyAcc-mean()-Y, tBodyAcc-mean()-Z, tBodyAcc-std()-X, tBodyAcc-std()-Y, tBodyAcc-std()-Z, tGravityAcc-mean()-X, tGravityAcc-mean()-Y, tGravityAcc-mean()-Z, tGravityAcc-std()-X, tGravityAcc-std()-Y, tGravityAcc-std()-Z, tBodyAccJerk-mean()-X, tBodyAccJerk-mean()-Y, tBodyAccJerk-mean()-Z, tBodyAccJerk-std()-X, tBodyAccJerk-std()-Y, tBodyAccJerk-std()-Z, tBodyGyro-mean()-X, tBodyGyro-mean()-Y, tBodyGyro-mean()-Z, tBodyGyro-std()-X, tBodyGyro-std()-Y, tBodyGyro-std()-Z, tBodyGyroJerk-mean()-X, tBodyGyroJerk-mean()-Y, tBodyGyroJerk-mean()-Z, tBodyGyroJerk-std()-X, tBodyGyroJerk-std()-Y, tBodyGyroJerk-std()-Z, tBodyAccMag-mean(), tBodyAccMag-std(), tGravityAccMag-mean(), tGravityAccMag-std(), tBodyAccJerkMag-mean(), tBodyAccJerkMag-std(), tBodyGyroMag-mean(), tBodyGyroMag-std(), tBodyGyroJerkMag-mean(), tBodyGyroJerkMag-std(), fBodyAcc-mean()-X, fBodyAcc-mean()-Y, fBodyAcc-mean()-Z, fBodyAcc-std()-X, fBodyAcc-std()-Y, fBodyAcc-std()-Z, fBodyAccJerk-mean()-X, fBodyAccJerk-mean()-Y, fBodyAccJerk-mean()-Z, fBodyAccJerk-std()-X, fBodyAccJerk-std()-Y, fBodyAccJerk-std()-Z, fBodyGyro-mean()-X, fBodyGyro-mean()-Y, fBodyGyro-mean()-Z, fBodyGyro-std()-X, fBodyGyro-std()-Y, fBodyGyro-std()-Z, fBodyAccMag-mean(), fBodyAccMag-std(), fBodyBodyAccJerkMag-mean(), fBodyBodyAccJerkMag-std(), fBodyBodyGyroMag-mean(), fBodyBodyGyroMag-std(), fBodyBodyGyroJerkMag-mean(), fBodyBodyGyroJerkMag-std()".

Each variable has original measurement name ('-XYZ' is used to denote 3-axial signals in the X, Y and Z directions):
*tBodyAcc-XYZ
*tGravityAcc-XYZ
*tBodyAccJerk-XYZ
*tBodyGyro-XYZ
*tBodyGyroJerk-XYZ
*tBodyAccMag
*tGravityAccMag
*tBodyAccJerkMag
*tBodyGyroMag
*tBodyGyroJerkMag
*fBodyAcc-XYZ
*fBodyAccJerk-XYZ
*fBodyGyro-XYZ
*fBodyAccMag
*fBodyAccJerkMag
*fBodyGyroMag
*fBodyGyroJerkMag

Each variable also has a part ('mean()' or 'std()') indicates estimation procedure of it:
mean(): Mean value of all signals for that subject for each subject and each activity.
std(): Mean value of the standard deviations of signals in one time window for each subject and each activity.
