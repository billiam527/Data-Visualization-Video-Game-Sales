

# Readme for Data Visualization Video Game Ratings and Sales

## About the autor

William Fisher
Graduate Student 
Mercyhurst University
DATA 620 Data Visualization
Project 2 - Visualization of Video Game Sales and Ratings

## This repository contains:

1. The Jupyter notebook containing code
2. Data Visualization Video Game Sales and Rating CSV
3. The redame file

## Table of Contents

- [Background](#background)
- [Install](#install)
- [Usage](#usage)
- [Related Efforts](#related-efforts)
- [Project Explaination](#Project-explaination)
- [License](#license)

## Background

The dataset consists of an excel file.  The columns consist of the name of the game, the platform it was realeased on, the year of the release, the genre, the publisher, the sales from various regions and the global sales, ratings from critics and users,the developer, and the rating of the games.  The data contains 31 different consoles and 13 different genres.  These will be the main focus of our analysis.  The various sales recorded are North American sales, European sales, Japanese Sales, other and global sales.

#### Wii
<img src="Wii.jpg" width="200"/> 

#### PS3
<img src="PS3.jpg" width="200"/> 

#### Xbox 360
<img src="X360.jpg" width="200"/> 


Please follow the following for the second project:
1) Select a dataset of your own choice (simple, complicated, whatever your level of comfort is)
2) Chop the dataset using pandas to fit whatever visualization you have in mind.
3) Clean the dataset and drop missing values - if needed
4) Create two different types of visualization - minimum. Your choice, just make sure they are different kinds - (for example a bar chart and a pie, but not two pies).
5) You can have more visualizations if you want
6) Make sure your readme file is perfect!
7) Submit on github and kaggle (if using kaggle datasets), just github if you are using data from other sources like drivedata.org or other census data.

## Install

This project uses Python & the following python packages:

csv
pandas
seaborn
matplotlib
numpy

## Usage

This is a class project.

## Related Efforts

There are several other students in the Fall DATA 620: Data Visualization class working on similar projects.  Students were supposed to choose different data sets so while content may be similar, the topics should be broadly ranged.

## Project Explaination
Explaination of Jupyter notebook code:

Cell 1: We need to import the neccesary libraries.  For our project we need to import csv, pandas, seaborn, matplotlib, and numpy.  We can also abbreviate these to make it easier to call them later in our code. "A lazy coder is a successful coder."

Cell 2: We then, import our CSV file.  In this case, we use pd and the import csv method to import the data. We then assign the data to the variable data.

Cell 3 and 4:  We can view just the top and bottom of the data using .head() and .tail() respectively.  We do this to get an idea of what all our data contains. In this case we are just looking at the beginning and end but we will do more to see what other values our in our data.

Cell 5: We get some more info about our data by using type() and shape().  Again, if we are going to make effective visualizations we need to understand the data and figuring out what it contains is step one to that.

Cell 6: We set our index as the "Platform" row and save this into df1.  I chose to designate "Platform" as the index because I wanted to explore the sales based on their consoles.

Cell 7: We can then group our data by the "Platform" index to get a more consolidated view.  We also summarize it here.  

Cell 8: Next, I chopped off some of the columns so I could get a better view of the data I wanted to use for my charts.

Cell 9: We then sort it largest to smallest using ascending = True.  We also remove the rows we do not want for our visualizations.

Cell 10: Then, we create a stacked bar chart that shows the various amounts of sales.  The stacked chart does an excellent job of displaying sales because of the multiple layers it is able to show.  It shows the breakdown of all the regions with the overarching global sales at the top.

Cell 11:  In addition to a bar chart, a pie chart is another excellent way to show which console had the most global sales.  I also wanted to switch up the color scheme as the bar chart using "Winter" was too bright and the colors ran together.

Cell 12:  Finally, I used an area chart to also show which consoles have had the most market share.  After plotting the data on these three chart types it is clear (if it was not already from reading the numbers) that the PS2 is the highest selling console in the data as of 2016.  The graphics also show that the Playstation brand as a whole has done well as the PS3 and the PS are also featured amongst the top of the charts.

Cell 12: I then wanted to view sales from the three main generation 7 consoles: the Wii, the PS3, and the Xbox 360.  These 3 consoles were revolutionary and were big competitors at the times of their releases. In order to display them properly on their respective charts, I first wanted to isolate their specific rows and columns, and summarize by the yearly global sales.  Once the data was ready, I was able to produce bar charts to show these sales by their year.

Cell 13: After comparing global sales amongst the consoles, I wanted to look at some of the gaming "scores" and how those correlate with eachother and sales.  In Cell 13, we created a heat map after first converting any float values to numbers.  The heatmap shows us that critic and user scores correlate pretty well which should be expected.

Cell 14 and 15: These cells are regression plots to see if scores also correlate to higher sales.  Although it can be hard to see, there is an uptick in sales as critic and user scores go up.
                                     
## License
none
