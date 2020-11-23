# Getting-and-Cleaning-Data-Course-Project

Analysis process
The analysis script, run_analysis.R reads in the processed experiment data and performs a number of steps to get it into summary form.

1. Both the processed test and training datasets are read in and merged into one data frame.
2. The data columns are then given names based on the features.txt file.
3. Columns that hold mean or standard deviation measurements are selected from the dataset, while the other measurement columns are excluded from the rest of the analysis.
4. The activity identifiers are replaced with the activity labels based on the activity_labels.txt file.
5. Invalid characters (() and - in this case) are removed from the column names. Also, duplicate phrase BodyBody in some columns names is replaced with Body.
6. The data is then grouped by subject and activity, and the mean is calculated for every measurement column.
7. Finally, the summary dataset is written to a file, tidy.txt.

Each line in run_analysis.R is commented. Reference the file for more information on this process.
