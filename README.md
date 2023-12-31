# python-api-challenge

## Background
Data's true power is its ability to definitively answer questions. So, let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"

Now, we know what you may be thinking: “That’s obvious. It gets hotter.” But, if pressed for more information, how would you prove that?

## Before You Begin
- Create a new repository for this project called python-api-challenge. Do not add this homework to an existing repository.
- Clone the new repository to your computer.
- Inside your local Git repository, create a directory for this assignment. Use a folder name that corresponds to the  Challenges, such as WeatherPy.
- Inside the folder you just created, add the files called api_keys.py, WeatherPy.ipynb, and VacationPy.ipynb that you will find in the starter code ZIP file provided. These will be the main scripts to run for each analysis.
- Before you push your changes to GitHub, add a .gitignore file.

## Add a .gitignore File
For this assignment, you will need to add a .gitignore file to your repo. Doing so will prevent the api_keys.py file that contains your API key from being shared with the public. If you skip this step, anyone using GitHub could copy and use your API key, and you may incur charges as a result.

To get started, type git status in the command line to see a list of all the untracked files that you have created so far.

To add only the WeatherPy.ipynb file to GitHub, for example, type git add WeatherPy.ipynb. Keep in mind that you would have to add each file individually when adding or updating a file. A more efficient solution is to add all of the files that you don't want to track to the .gitignore file.

Before adding your files to GitHub, add api_keys.py to the .gitignore file by following these steps:
  1. Open your python-api-challenge GitHub folder in VS Code.
  2. Open the .gitignore file and type the following code on the first line:
        Adding config.py file.
        api_keys.py

  3. In the command line, type git status and press Enter. The output should indicate that the .gitignore file has been modified and the api_keys.py file is untracked.
  4. Use git add, git commit, and git push to commit the modifications to the .gitignore, WeatherPy.ipynb and     VacationPy.ipynb files to GitHub.

On GitHub, the only new python files you should find are WeatherPy.ipynb and VacationPy.ipynb.

## Instructions
This activity is broken down into two deliverables, WeatherPy and VacationPy.

### Part 1: WeatherPy
In this deliverable, you'll create a Python script to visualize the weather of over 500 cities of varying distances from the equator. You'll use the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and your problem-solving skills to create a representative model of weather across cities.

For this part, you'll use the WeatherPy.ipynb Jupyter notebook provided in the starter code ZIP file. The starter code will guide you through the process of using your Python coding skills to develop a solution to address the required functionalities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:

- Latitude vs. Temperature
- Latitude vs. Humidity
- Latitude vs. Cloudiness
- Latitude vs. Wind Speed

### Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values as you can see in the following image:

![Screenshot 2023-09-06 at 8 46 41 PM](https://github.com/cbake105/python-api-challenge/assets/133677209/e16edc60-1630-4d3d-bc02-74b3ff29785e)

You should create the following plots:
- Northern Hemisphere: Temperature vs. Latitude
- Southern Hemisphere: Temperature vs. Latitude
- Northern Hemisphere: Humidity vs. Latitude
- Southern Hemisphere: Humidity vs. Latitude
- Northern Hemisphere: Cloudiness vs. Latitude
- Southern Hemisphere: Cloudiness vs. Latitude
- Northern Hemisphere: Wind Speed vs. Latitude
- Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.

### Part 2: VacationPy
In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

  1. Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

     ![Screenshot 2023-09-06 at 8 45 49 PM](https://github.com/cbake105/python-api-challenge/assets/133677209/d06ac48a-3f8b-45c5-9b0f-1a34fd7b375d)


  3. Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
    - A max temperature lower than 27 degrees but higher than 21
    - Wind speed less than 4.5 m/s
    - Zero cloudiness

  4. Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

  5. For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

  6. Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

     ![Screenshot 2023-09-06 at 8 47 35 PM](https://github.com/cbake105/python-api-challenge/assets/133677209/e9886989-097f-446f-9932-8d269e5938a1)


# Analysis

Summary: 

Temperature vs. Latitude Linear Regression Plot
  
  Discussion about linear relationship:
  - Northern Hemisphere: Max Temp and Latitude in the Northern Hemisphere displays a negative correlation. The r-value(0.4897) indicates a positive linear relationship but has a weaker linear relationship than the Southern Hemisphere. 

  - Southern Hemisphere: Max Temp and Latitude in the Southern Hemisphere displays a positive correlation. The r-value(0.6964) indicates a positive linear relationship and has a stronger linear relationship than the Northern Hemisphere. 

Humidity vs. Latitude Linear Regression Plot

  Discussion about linear relationship:
  - Northern Hemisphere: Humidity and Latitude in the Northern Hemisphere displays no correlation. The r-value(0.00005) indicates a very weak linear relationship and has a weaker linear relationship than the Southern Hemisphere. 

  - Southern Hemisphere: Humidity and Latitude in the Southern Hemisphere displays no correlation. The r-value(0.00587) indicates a very weak linear relationship and has a stronger linear relationship than the Northern Hemisphere. 

# Cite
AskBCS Learning Assistant

Sbu
https://smuvirtdatapt-yzn4480.slack.com/archives/C05QMFPU2SK

Luna 
https://smuvirtdatapt-yzn4480.slack.com/archives/C05R3DZC8SF

Class Office hours
