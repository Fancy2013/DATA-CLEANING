#Coursera-Getting-and-Cleaning Data Assignment 

Criteria
1.	The submitted data set is tidy.
2.	The Github repo contains the required scripts.
3.	GitHub contains a code book that modifies and updates the available codebooks with the data to indicate all the variables and summaries calculated, along with units, and any other relevant information.
4.	The README that explains the analysis files is clear and understandable.
5.	The work submitted for this project is the work of the student who submitted it.
Instructions

The run_analysis.R script aims to accomplish the following goals:
1.	Merges the training and the test sets to create one data set.
2.	Extracts only the measurements on the mean and standard deviation for each measurement.
3.	Uses descriptive activity names to name the activities in the data set
4.	Appropriately labels the data set with descriptive variable names.
5.	From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

Data set: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

Analysis Script
Please see the run_analysis.R script for a detailed description of the implementation of each step used to accomplish the goals. Here is a high level description of the steps in the script used to accomplish each goal.

1	Merges the training and the test sets to create one data set.
  1.1	Download the file and put the file in the data folder
  1.2	Unzip the file
  1.3	unzipped files are in the folderUCI HAR Dataset. Get the list of the files
  1.4	Read data from the activity, subject, and features files into the variables
  1.5	Concatenate the data tables by rows
  1.6	set names to variables
  1.7	Merge columns to get the data frame Data for all data

2	Extracts only the measurements on the mean and standard deviation for each measurement.
  2.1	Subset Name of Features by measurements on the mean and standard deviation
  2.2	Subset the data frame Data by seleted names of Features

3	Uses descriptive activity names to name the activities in the data set
  3.1	Read descriptive activity names from “activity_labels.txt”
  3.2	facorize Variale activity in the data frame Data using descriptive activity names

4	Appropriately labels the data set with descriptive variable names.
  4.1	In the former part, variables activity and subject and names of the activities have been labelled using descriptive names. In this part, Names of Features will labelled using descriptive variable names.

5	From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.
  5.1	In this part,a second, independent tidy data set will be created with the average of each variable for each activity and each subject based on the data set in step 4.

Output
Tidy dataset: tidy.txt

Code Book
CodeBook.md: describes the variables, the data, and any transformations or work performed to clean up the data

