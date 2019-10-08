# Module 4 Project - Predicting House Prices Using Data From Zillow

## Background

Following a recent funding round a property start-up, *Investate*, have raised $100 million.  To ensure that this money is invested wisely, we have been appointed to **identify the top 5 best zipcodes in which to invest**. 

## Data

To investigate this problem, data has been sourced from *Zillow*.  *Zillow* is the leading real estate and rental marketplace in the US.  It maintains a database of 110 million properties across the country.  From this, they are able to provide zipcode-level sales and rental price history dating back to 1996.  

## Approach

To provide recommendations to Investate, the following approach has been employed:
- The data is imported and pre-processed to remove missing values and identify outliers
- Exploratory data analysis is performed to identify:
    - high growth states
    - high growth counties within the high growth states
- Data for selected counties is extracted
- Each county dataset is split into a training and test set
- Each dataset is assessed for evidence of stationarity, seasonality and autocorrelation.  This assists with model selection
- Alternative models compared.  Model with best performance is selected
- Predictions are run to calculate growth
- Zipcodes with highest forecast growth, and excellent model performance are identified as investable


## Requirements

These instructions will guide you through the technical requirements that will need to be fulfilled, before running this project on your machine.

Before getting started, you will need to have Python installed on your machine. We recommend using Anaconda for this purpose, as it is delivered with more than 1,500 packages/libraries pre-installed.

## Libraries
To run these projects, you will first need to install the following libraries. If you have chosen to run Python through Anaconda, there is no need to individually install the below:

- **Pandas**: Used for data manipulation and analysis
- **Numpy**: Supports multi-dimensional matrices and arrays, provides a large number of mathematical functions
- **Matplotlib**: A 2D graphical plotting library
- **Seaborn**: Another data visualisation libary, based on Matplotlib
- **Statsmodels**: Enables the conduct of statistical analysis
- **Sklearn**: Provides tools for data analysis
- **Itertools**: Implements a number of interator building blocks (e.g. permutations, combinations etc.)
- **Folium**: Supports the creation of interactive maps
- **Ast**:  Helps Python applications to process trees of the Python abstract syntax grammar.


## Forking & Cloning the Repository onto your Local Machine

1. Within Github, click 'Fork'
2. Once Forked, copy the link https://github.com/[YOUR NAME]/dsc-mod-4-project-online-ds-ft-071519
3. Open the command line and navigate to the folder you wish to save the projec to
4. Type 'git clone https://github.com/[YOUR NAME]/dsc-mod-4-project-online-ds-ft-071519'
5. Open a new command line window, type 'jupyter notebook'
6. A Jupyter notebook will open. Navitage to the folder in which your project is located, open the Jupyter notebook. You are ready to get started.


## Files
The relevant files within this repository are as follows:

- **README.md**: The file you're reading now.
- **zillow_data.csv**: This is the dataset that will be used for the investigation.  Contains median house prices for each zipcode 1996 to 2018.
- **mod_4_project.ipynb**: This is the Jupyter notebook that contains the statistical analysis
- **states.json**: A JSON file containing the geometry of each state.  This is used with Folium to create data maps
- **denver_zipcodes.csv**: Contains the latitude and longitude of each zipcode in Denver.  Used with Folium to map data.
- **california_zipcodes.csv**: Contains the latitude and longitude of each zipcode in California.  Used with Folium to map data.
- **Presentation.pdf**: This is a set of slides which provides a non-technical overview of the project's findings
