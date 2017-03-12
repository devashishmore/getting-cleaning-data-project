# getting-cleaning-data-project
## Download the file
File was downloaded using the download.file() function.

## Read the Activity,Subject and Test files
The following files were read into tables:
* features.txt
* activity_labels.txt
* subject_train.txt
* x_train.txt
* y_train.txt
* subject_test.txt
* x_test.txt
* y_test.txt

## Concatenate the data tables by rows
* Using the **rbind()** function the activity, features and subject tables were concatenated.

## Set names and merge columns
* Using the **names()** function the variable names were changed
* Using the **cbind()** function the columns were merged

## Extract the standard deviation and mean
* The standard deviation and mean were extracted using the **grep()** function

## Change the activity names in an easily understandable form
* The **gsub()** function was used to change activity names

## Average the data and create an independent tidy dataset
* The **plyr** package was used
* Using the **aggregate()** average was calculated and using **write.table()** function the data was put into tidyData.txt
