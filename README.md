# Getting-and-Cleaning-Data
This is the course project for getting and cleaning data.

One of the most exciting areas in all of data science right now is wearable computingThe data linked to from the course website represent data collected from the accelerometers from the Samsung Galaxy S smartphone. A full description is available at the site where the data was obtained: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

The project is to create one R script called run_analysis.R that does the following:	
1. Merges the training and the test sets to create one data set.	
2. Extracts only the measurements on the mean and standard deviation for each measurement.	
3. Uses descriptive activity names to name the activities in the data set	
4. Appropriately labels the data set with descriptive variable names.	
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.	

The gitfolder of this repo contains the run_analysis.R source code and a CodeBook describing the steps to clean up the data. To run the analysis:	
1. Copy the run_analysis.R into your current working directory of R.	
2. Download and unzip the dataset into your current working directory.	
3. Source the run_analysis.R. It will give you a tidy dataset in the UCI HAR Dataset folder.	
4. Use read.table("run_analysis.txt") to read the tidy dataset.	
