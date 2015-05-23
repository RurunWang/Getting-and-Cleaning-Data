## The attached R script (run_analysis.R) performs the following to clean up the data:

1. Read all the txt files and save them to variables called X_train, X_test, Y_train, Y_test, features, activity_labels, subject_train, subject_test. 

2. Combine the training and testing data set using rbind and save them to variables called X_all, Y_all, subject_all

3. Merge Y_all data to activity labels by the common column "V1". In order not to confuse latter performance, change the column name of activity_labels to Activity and subject column to subject. Use cbind to combine Y_all data and subject_all to generate a dataset called Y_subject. Then use merge to combine the Y_subject and activity_labels by the common column "V1", resulting a dataset called Y_merge. 

4. Then combine the Y_merge data with X_all data to get a complete dataset containing all the measurements, subjects, activity labels. First give X_all dataset the variable names using the names in feasure. Then use cbind to combine the Y_merge and X_all to generate a dataset called data_all. 

5. Last use the select function to select the data_all dataset any columns that contans "means" or "std" to a selected dataset called data_select. Group the dataset by subject and activity labels, generating data_group. Finally get the mean of each group and generate a tidy dataset, data_final. Write it to a txt file called run_analysis.txt using write.table function. 
