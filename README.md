# Getting and Cleaning Data Project

This repository contains the work for the final project of the Getting and Cleaning Data course.

## Files
* `run_analysis.R`: The R script that performs the data preparation and cleaning.
* `CodeBook.md`: Describes the variables, the data, and any transformations performed to clean up the data.
* `FinalData.txt`: The final exported tidy dataset.
* `README.md`: This file.

## How to run the script
1. Download and unzip the data from [UCI HAR Dataset](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones).
2. Put the `run_analysis.R` script in the same parent directory as the `UCI HAR Dataset` folder.
3. Open RStudio and set your working directory to that folder.
4. Run `source("run_analysis.R")`.
5. The script will generate a file called `FinalData.txt` in your working directory.
