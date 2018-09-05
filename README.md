# data_analysis_911_calls_dataset
This project demonstrate data analysis and visualization of some 911 call dataset from Kaggle using Pandas, Numpy, Matplotlib and Seaborn.

#### Dataset source: https://www.kaggle.com/mchirico/montcoalert

# Objective:

* Read in the csv file as a dataframe called df and check the info and head of the df.
* What are the top 5 zipcodes for 911 calls?
* What are the top 5 townships (twp) for 911 calls?
* Take a look at the 'title' column, how many unique title codes are there?
* In the titles column there are "Reasons/Departments" specified before the title code. These are EMS, Fire, and Traffic. Create a new column called "Reason" that contains this string value.
* What is the most common Reason for a 911 call based off of this new column?
* Now use seaborn to create a countplot of 911 calls by Reason.
* Now use seaborn to create a countplot of 911 calls by Township.
* Now let us begin to focus on time information. What is the data type of the objects in the timeStamp column?
* Timestamps are still strings. Use pd.to_datetime to convert the column from strings to DateTime objects.
* Now that the timestamp column are actually DateTime objects, use .apply() to create 3 new columns called Hour, Month, and Day of Week. You will create these columns based off of the timeStamp column.
* Use the .map() with this dictionary to map the actual string names to the day of the week.
* Use seaborn to create a countplot of the Day of Week column with the hue based off of the Reason column.
* Now create a simple plot off of the dataframe indicating the count of calls per month.
* Now see if you can use seaborn's lmplot() to create a linear fit on the number of calls per month. 
* Create a new column called 'Date' that contains the date from the timeStamp column.
* Now groupby this Date column with the count() aggregate and create a plot of counts of 911 calls.
* Now recreate this plot but create 3 separate plots with each plot representing a Reason for the 911 call.
* Now let's move on to creating heatmaps with seaborn and our data. We'll first need to restructure the dataframe so that the columns become the Hours and the Index becomes the Day of the Week. 
* Now create a HeatMap using this new DataFrame.
* Now create a clustermap using this DataFrame.
* Now repeat these same plots and operations, for a DataFrame that shows the Month as the column.

# Steps To Run:
For this demonstration, I am using the Jupyter Notebook, open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text.

### Step 1:
Create a virtual enviroment and install dependencies by running requirements.txt.

$ pip install virtualenv env

$ source env/bin/activate

$ pip install -r requirements.txt

### Step 2:
Run the script.

$ jupyter notebook
