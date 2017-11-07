

# Readme for Data Visualization Video Game Ratings and Sales

## About the autor

William Fisher
Graduate Student 
Mercyhurst University
DATA 550 Data Visualization
Project #2 - Visualization of Video Game Sales and Ratings

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

The goals for this repository are:

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

Ther are several other studentsin the Fall 2017 Data Visualizatin Class doing similar projects.

## Project Explaination
Explaination of Jupyter notebook code:

Cell 1: We need to import the neccesary libraries.  For our project we need to import csv, pandas, seaborn, matplotlib, and numpy.  We can also abbreviate these to make it easier to call them later in our code.

Cell 2: We then, import our CSV file.  In this case, we use pd and the import csv method to import the data. We then assign the data to a variable.

Cell 3 and 4:  We can view just the top and bottom of the data using .head() and .tail() respectively.

Cell 5: We get some more info about our data by using type() and .shape()

Cell 6: We set our index as the "Platform" row and save this into df1

Cell 7: We can then group our data by the "Platform" index to get a more consolidated view.  We also summarize it here.  

Cell 8: Next, I chopped off some of the columns so I could get a better view of the data I wanted to use for my charts.

Cell 9: We then sort it largest to smallest using ascending = True.  We also remove the rows we do not want for our visualizations.

Cell 10: Finally, we create a stacked bar chart that shows the various amounts of sales.  The stacked chart shows an excellent job of showing it because of the multiple layers it is able to show.  It shows the breakdown of all the regions with the overarching global sales at the top.

Cell 11: Next, we get the mean of the data.  We do this to prepare for a scatter plot showing the ratio of critic scores to global sales.  We use the mean so that our data is not skewed toward one system that happens to have a lot of scores.

Cell 12:  We plot the second visualization, a scatter plot.  I expected global sales and critic scores to correlate but according to this data they do not.
                                     
## License
none
