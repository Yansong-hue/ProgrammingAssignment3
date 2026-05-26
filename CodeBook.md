# Code Book

## Data Source
The original data comes from the "Human Activity Recognition Using Smartphones Data Set" provided by UCI. 

## Transformation Steps
1. Merged the training and the test sets to create one data set.
2. Extracted only the measurements on the mean and standard deviation for each measurement using `grep`.
3. Replaced activity codes (1-6) with descriptive names (WALKING, etc.).
4. Labeled the data set with descriptive variable names:
    * All abbreviations like `Acc`, `Gyro`, `Mag` were expanded to `Accelerometer`, `Gyroscope`, `Magnitude`.
    * Prefixes `t` and `f` were replaced by `Time` and `Frequency`.
5. Created a second, independent tidy data set with the average of each variable for each activity and each subject.

## Variables
* `subject`: The ID of the participant (1 to 30).
* `activity`: The type of activity performed (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING).
* `TimeBodyAccelerometerMeanX`: Mean time-domain body acceleration in X direction.
* ... (列出主要变量即可，或说明所有变量遵循此命名规则)

## Units
All measurement variables are normalized and bounded within [-1, 1], thus they are unitless.
