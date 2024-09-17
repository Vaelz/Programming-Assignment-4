# Programming-Assignment-3

## Item #1
#### Function/s Used:
  - import pandas as pd
  - pd.read_csv()
  - x.mean()

#### Documentation:
a. Importing Pandas as pd
  - Initially import the pandas Library using import pandas as pd to access pandas functions.

b. Read the CSV file
  - Using the function pd.read_csv('board2.csv'), the program then reads the CSV file "board2". from the repository

c. Setting up the Average
  - Using data['Average'] = data[['GEAS','Electronics','Math', 'Communication']].mean(axis=1), this look for the average mean from the 4 Subject found at board2.csv file.
  - The average can now be stored as data['Average']
    
d. Condition A 
  - Given with a condition, Filename: Instru = [“Name”, “GEAS”, “Electronics >70”]; where the track is constant as "Instrumentation" and hometown "Luzon".
  - Using this line of code, Instru = data[(data['Track'] == 'Instrumentation') & (data['Hometown'] == 'Luzon') & (data['Electronics'] > 70)], the data can now be sliced to the given condition.
  - Now to Collate the data I use, Instru = Instru[['Name','GEAS','Electronics']], then print Instru.
    
d. Condition B
  - Given with a condition, Filename: Mindy = [ “Name”, “Track”, “Electronics”, “Average >=55”]; where hometown is constant as "Mindanao" and gender "Female"
  - Using this line of code, Mindy = data[(data['Hometown'] == 'Mindanao') & (data['Gender'] == 'Female') & (data['Average'] >= 55)], using the average from letter c for reference, the data can now be sliced to the given condition.
  - Now to Collate the data I use, Mindy = Mindy[['Name','Track','Electronics','Average']], then print Mindy.
    
Note: 
  - The board2.csv is an external file located at this heres repository

## Item #2
#### Function/s Used:
  - import matplotlib.pyplot as plt
  - x.mean()
  - x.unique()
  - plt.figure()
  - plt.boxplot()
  - plt.title()
  - plt.x,ylabel()
  - plt.show()

#### Documentation:
a. Importing matplotlib.pyplot as plt
  - Added an import for matplotlib Library using import matplotlib.pyplot as plt to access matplotlib plot functions.

b. Setting the Plot size
  - By using the function plt.figure(x,y). The plot size changes its figure to a desirable one (here, I used x = 20, y = 4).

c. Unique Variables
  - Using X_unique = X.unique(), the desired variable can now be used as a separate variable to use for loops.
    
d. Calculate the Average for the different features
  - Using X_Ave = [data[data['X'] == track]['X'] for X in X_unique], the average of the targeted features can now be stored and used for comparing in the plot.
  - In this assignment, the features used are Track, Gender and Hometown.

e. Set up to plot
  - According to what I know you can use any plotting tools but in here I used plt.boxplot(y-axis, x-axis).
  - To create the plot the x and y axis is changed to the desired feature (Track, Gender or Hometown) as x-axis, and the average of each desired feature calculated from before as y-axis.
    
f. Edit and show the plot
  - Using the following functions:
  - plt.title(): Edit and reveal the "Title" of the boxplot located at the middle top.
  - plt.xlabel(): Edit and reveal the "Label" for the x-axis located at the middle bottom.
  - plt.ylabel(): Edit and reveal the "Label" for the y-axis located at the left side.
  - plt.show(): This shows the whole boxplot

Note:
- The capital letter 'X' used here are any desired variables
- Some of the funtion of plot used here are searched online.

## Updates:
- Posted Programming Assignment 4.ipynb File
- Added board2.csv File
- Added ReadMe File
-
