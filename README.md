# Environmental Informatics

## Assignment 08 - Time Series Analysis with Pandas

### Lab Objectives

On completion of this lab, students will be able to:

1. Use Time and Date functions with pandas DataFrames to conduct time series analysis of a dataset.
2. 
3. 

### Reading Assignment

Data Analysis with Open Source Tools:

- Chapter 4: Two Variablesime as a Variable: Time Series Analysis

### The Lab Assignment

1. Start by cloning this assignment to the folder where you have been completing assignments.

2. Next, complete the tutorial [Time Series Analysis with Pandas](http://earthpy.org/pandas-basics.html), but include all of the tutorial code in a Python program called **PandasDatesDemo.py** that is included in this repository.

(15 pts) Complete the tutorial Time series analysis with Pandas, with the following modifications:
You can copy commands from the browser using  -  , and paste them into spyder by clicking (not rolling) the middle button.  If you accidentally roll the middle button instead of clicking it, select another window (a Microsoft window, not another X11 window) to get out of scroll mode for X-windows.
The "set_printoptions()" function does not appear to work with the current version of pandas.
Do not set your graphics to inline(see "ln[7]:"),graphics are already prepared in the spyder interface.
The !wget command will download the data file from within the console in spyder, but can also be run directly from the Linux prompt (drop the "!" from the start of the command, this is telling the Python interpretor that the command should be run at the Linux shell and not interpreted as a Python statement).
If you started spyder without a file, then it will default to using your home directory as its working directory.  So when you download the data file from the Python prompt it will be written to your home directory, not the new course directory.
From the Linux prompt, use "head" and "tail" to determine the start and end dates for your file (the tutorial was written in 2013, but the data file continues to be updated).  What dates should you use to define the correct record length?
The length of record for the AO and NAO files may not be the same, despite what the tutorial document says.  If they are not the same length, what happens when they are combined into a single DataFrame?
Submit the following plots for evaluation (5 pts each plot): 
(5 pts) Daily Atlantic Oscillation (AO) plot (Out [23]:)
(5 pts) Annual median values for AO (Out [48]:)
(5 pts) Rolling mean for both AO and NAO (Out [52]:)
Download the attached file, which is daily discharge for the Wabash River at the Lafayette, Indiana gauge from March 17, 2015 through March 24, 2016.
(35 pts) Write a Python script that will do the following:
(10 pts) Read the contents of the file into a Pandas series using Columns 3 and 4 for a single Date-Time element, and Column 6 (discharge in cubic feet per second) for the value.
The Pandas documentation on the read_table function will be helpful.
More information can also be found at the IO Tools page, in particular help on how to get the read function to parse the date for you automatically can be found here.
Information on how to get read_tables to handle variable white space as a separator can be found at this discussion page.
This does not have to all be done in a single line, you may find it easier to import the data in a more raw format, and then work it into a usable final format.
(5 pts) Create a plot of daily average streamflow for the period of record, written to a PDF or PS file.
(5pts) Using the daily average flow data, identify and plot the 10 days with highest flow, written to a PDF or PS file.  Use symbols to represent the data on the same time axis used for the full daily flow record.
(5 pts) Create a plot of monthly average streamflow for the period of record, written to a PDF or PS file.
(5 pts) Submit all input and output files.
(5 pts) Submit a well documented script that works with the provided files.
Bundle all files into a directory and submit through Blackboard.


4. Be sure that the script has a complete header comment block, appropriate in-line comments, and runs without intervention.

#### What to turn in...

The following should be included in your GitHub repository:

1. A working tutorial solution file called **PandasDatesDemo.py**.

2. The data file downloaded from the [USGS earthquake hazards web site](http://earthquake.usgs.gov/earthquakes/feed/).

2. A working program called **program-08.py**.

5. A metadata file called **Metadata.pdf**:
   - Use Word or similar word processing program (Open Office, `openoffice.org`, is available on all of the clusters and does many of the same things as Microsoft Office).
   - Describe the source and format of the input data (not more than half a page),
   - Describe the types of analysis conducted by your script (not more than half a page),
   - Import the graphical analysis figures your developed in the previous section, and write a caption that describes the figure and addresses the hints provided for each figure.
   - Captions should be consecutively numbered.
   - Convert the Metadata file into a PDF file prior to submission.

7. Put your input file, processing script and metadata file in the assignment repository and push to GitHub to submit.

#### Grading Rubric (50 pts Total)

| Question | Description | Score |
| -------- | ----------- | ----- |
| 1. |Complete the tutorial Time series analysis with Pandas, with the required modifications | 15 pts |
| 3. | Submit the following plots for evaluation || 
| 3.1. | Daily Atlantic Oscillation (AO) plot (Out [23]:) | 5 pts |
| 3.2 | Annual median values for AO (Out [48]:) | 5 pts |
| 3.3 | Rolling mean for both AO and NAO (Out [52]:) | 5 pts |
Download the attached file, which is daily discharge for the Wabash River at the Lafayette, Indiana gauge from March 17, 2015 through March 24, 2016.
(35 pts) Write a Python script that will do the following:
(10 pts) Read the contents of the file into a Pandas series using Columns 3 and 4 for a single Date-Time element, and Column 6 (discharge in cubic feet per second) for the value.

(5 pts) Create a plot of daily average streamflow for the period of record, written to a PDF or PS file.
(5pts) Using the daily average flow data, identify and plot the 10 days with highest flow, written to a PDF or PS file.  Use symbols to represent the data on the same time axis used for the full daily flow record.
(5 pts) Create a plot of monthly average streamflow for the period of record, written to a PDF or PS file.
(5 pts) Submit all input and output files.
(5 pts) Submit a well documented script that works with the provided files.
