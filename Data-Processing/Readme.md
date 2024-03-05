Program Documentation
Overview
This program is designed to process and analyze tabular data stored in a CSV (Comma-Separated Values) file format. It offers various functionalities such as data cleaning, exploratory data analysis (EDA), visualization, and data manipulation.

Dependencies
pandas: A powerful data manipulation library used for data manipulation and analysis.
scikit-learn: A machine learning library providing tools for data preprocessing and modeling. Used here for data imputation (SimpleImputer), standardization (StandardScaler), and outlier detection (IsolationForest).
numpy: A library for numerical computing, used primarily for array manipulation.
seaborn: A statistical data visualization library based on matplotlib. Used for generating heatmaps.
matplotlib: A comprehensive plotting library for Python, used for creating various types of plots such as histograms, bar charts, and scatter plots.
tkinter: Python's de-facto standard GUI (Graphical User Interface) package, used for simple file selection through a dialog box.
Functionality

1. Loading Data
   The program loads the data from a CSV file specified by the user. The file path is hardcoded but can be modified as needed.
2. Data Cleaning
   Missing values in the dataset are handled using mean imputation for numerical columns and most frequent imputation for categorical columns.
   Duplicate rows are removed to ensure data integrity.
3. Exploratory Data Analysis (EDA)
   Users can check for missing values in the dataset.
   Summary statistics like mean, median, and standard deviation can be calculated for numerical columns.
   Data can be filtered based on a specific column and criteria.
4. Visualization
   Histograms, bar charts, scatter plots, and heatmaps can be generated to visualize the data distribution and relationships between variables.
5. Saving Data
   Processed data can be saved back to a CSV file with a specified name.
6. Exiting Program
   Users can choose to exit the program when finished with their analysis.
   Usage
   Run the program.
   Choose an option from the menu to perform the desired operation.
   Follow the prompts and input any required information.
   Analyze the results or save the processed data as needed.
   Exit the program when finishe

Example
CSV file loaded successfully.

Choose an option:

1. Check missing values
2. Clean data
3. Remove duplicates
4. Calculate summary statistics
5. Filter data
6. Generate histogram
7. Generate bar chart
8. Generate scatter plot
9. Generate heat map
10. Save DataFrame to CSV
11. Exit

Enter your choice: 2
Data cleaned successfully.

Choose an option:

1. Check missing values
2. Clean data
3. Remove duplicates
4. Calculate summary statistics
5. Filter data
6. Generate histogram
7. Generate bar chart
8. Generate scatter plot
9. Generate heat map
10. Save DataFrame to CSV
11. Exit
