# Html Scraping Challenge

# Project Description 

## Deliverable 1: Scrape Titles and Preview Text from Mars News
- Inspect the Mars news site and connect to it using automated browsing
- Create a BeautifulSoup object and extract the text elements
- Extract the titles and preview texts for each of the articles, create a title and preview dictionary, store the dictionaries in a Python list, and print the list. 



## Deliverable 2: Scrape and Analyze Mars Weather Data
- Inspect the Mats Temperature Data Site and connect to it using automated browsing
- Create a BeautifulSoup object and extract the data from the table
- Create a DataFrame with the extracted table/data that reflects the columns on the website
- Examine the data types and convert data types into datetime, int, or float data types
- Analyze the dataset by answering the following questions:
How many months exist on Mars?
How many Martian (and not Earth) days worth of data exist in the scraped dataset?
What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
Find the average minimum daily temperature for all of the months.
Plot the results as a bar chart.
Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
Find the average daily atmospheric pressure of all the months.
Plot the results as a bar chart.
About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
Consider how many days elapse on Earth in the time that Mars circles the Sun once.
Visually estimate the result by plotting the daily minimum temperature.
- Export the DataFrame to a CSV

# Software and Files
## Deliverable 1
- from splinter import Browser
- from bs4 import BeautifulSoup
- url = https://static.bc-edx.com/data/web/mars_news/index.html

## Deliverable 2
- from splinter import Browser
- from bs4 import BeautifulSoup as soup
- import matplotlib.pyplot as plt
- import pandas as pd
- import datetime as date
- url = https://static.bc-edx.com/data/web/mars_facts/temperature.html

# Output/Analyses

## Part 1: Analyze and Explore Climate Data

### Connect Jupyter Notebook to Database

- Reflected Tables into SQLAlchemy ORM
<img width="1121" alt="Screenshot 2023-03-14 at 12 08 21 PM" src="https://user-images.githubusercontent.com/119909433/225083599-7b2a10b6-ed15-4266-a96e-13736ba18110.png">

### Precipitation Analysis

- Found the most recent date in the dataset 
<img width="1112" alt="Screenshot 2023-03-14 at 12 09 00 PM" src="https://user-images.githubusercontent.com/119909433/225083734-fe67a9ee-10f7-495a-b828-7a495eb6ffea.png">

- Designed a query to retrieve the last 12 months of precipitation data and plotted dates and inches of precipitation 
<img width="1108" alt="Screenshot 2023-03-14 at 12 10 11 PM" src="https://user-images.githubusercontent.com/119909433/225084038-42997baf-ef5d-4f62-9339-44d4ebb4e917.png">
<img width="714" alt="Screenshot 2023-03-14 at 12 10 24 PM" src="https://user-images.githubusercontent.com/119909433/225084086-d721168e-1009-454b-bd66-ff0116ef7615.png">

- Caculated summary statistics for the precipitation data
<img width="1092" alt="Screenshot 2023-03-14 at 12 10 51 PM" src="https://user-images.githubusercontent.com/119909433/225084200-7fed973e-037b-449a-93b5-a9ea71107c2c.png">

### Station Analysis

- Queried the total number of stations in the dataset
<img width="1112" alt="Screenshot 2023-03-14 at 12 12 37 PM" src="https://user-images.githubusercontent.com/119909433/225084671-f2ae26ee-5082-4d33-896d-87f0ffa95aaa.png">

- Queried the stations and observation counts in descending order 
<img width="1112" alt="Screenshot 2023-03-14 at 12 13 08 PM" src="https://user-images.githubusercontent.com/119909433/225084796-93f2b397-54cf-4c22-aaab-7e1724ae971c.png">

- Queried the lowest, highest, and average temperature observations from the most active station
<img width="1111" alt="Screenshot 2023-03-14 at 12 14 06 PM" src="https://user-images.githubusercontent.com/119909433/225085046-8ae0bde6-0f82-4529-b9f6-0e25977aa783.png">

- Queried the last 12 months of temperature observations from the most active station and plotted the data
<img width="1106" alt="Screenshot 2023-03-14 at 12 15 01 PM" src="https://user-images.githubusercontent.com/119909433/225085292-0e27a304-0e71-40ae-ad9e-55131bb464b5.png">

- Closed the session
<img width="1109" alt="Screenshot 2023-03-14 at 12 15 19 PM" src="https://user-images.githubusercontent.com/119909433/225085356-1ec8d556-f04e-4fb8-9fe4-7d58ca01866a.png">

## Part 2: Design a Climate App

- Set up the Database and Flask 
<img width="587" alt="Screenshot 2023-03-14 at 12 16 20 PM" src="https://user-images.githubusercontent.com/119909433/225085587-b66e1a20-bd0a-4057-be8e-24555b52312a.png">

- Set up routes
<img width="447" alt="Screenshot 2023-03-14 at 12 16 43 PM" src="https://user-images.githubusercontent.com/119909433/225085687-7a191ec2-6436-4aea-ab05-68f9278a7f6b.png">
<img width="361" alt="Screenshot 2023-03-14 at 12 17 11 PM" src="https://user-images.githubusercontent.com/119909433/225085786-54cb05fb-c17c-48b5-9690-b38bfdc59e63.png">

- Created a route for precipitation data, queried dates and precipitation observations within a specified year, and returned a JSON list of those observations 
<img width="905" alt="Screenshot 2023-03-14 at 12 18 38 PM" src="https://user-images.githubusercontent.com/119909433/225086145-3aa85407-6bfd-4964-8173-2a64f05cb995.png">
<img width="1033" alt="Screenshot 2023-03-14 at 12 19 03 PM" src="https://user-images.githubusercontent.com/119909433/225086320-00d03473-ebd6-424c-a1cc-6a7c98acac23.png">

- Created a route for stations and returned a JSON list of all the stations in the dataset 
<img width="552" alt="Screenshot 2023-03-14 at 12 19 49 PM" src="https://user-images.githubusercontent.com/119909433/225086478-9940bd3a-c475-4d54-92d0-f3fc6afb080b.png">
<img width="526" alt="Screenshot 2023-03-14 at 12 20 05 PM" src="https://user-images.githubusercontent.com/119909433/225086545-431949a0-04ce-4846-b907-5b0c74699eca.png">

- Created a route for temperature observations, queried dates and temperature observations for the most active station, and returned a JSON list of those observations
<img width="960" alt="Screenshot 2023-03-14 at 12 21 09 PM" src="https://user-images.githubusercontent.com/119909433/225086809-6ca2e57e-0f6c-4a16-bd13-6afa1df8cbbe.png">
<img width="873" alt="Screenshot 2023-03-14 at 12 21 29 PM" src="https://user-images.githubusercontent.com/119909433/225086897-591de768-b24a-42cd-85f2-e665f7d0c0ef.png">

- Created a route for observations before a specified start date
- Queried for min, max, and average temperatures prior to that start date
- Returned a JSON list of the min, max, and average temperatures 
<img width="912" alt="Screenshot 2023-03-14 at 12 23 27 PM" src="https://user-images.githubusercontent.com/119909433/225087386-98650d26-bfca-4f6c-9456-01a2174cbe16.png">
<img width="476" alt="Screenshot 2023-03-14 at 12 23 51 PM" src="https://user-images.githubusercontent.com/119909433/225087502-d1549c4b-71ce-4669-84c0-761422c03c78.png">

- Created a route for observations between a specified start and end date
- Queried for min, max, and average temperatures between the specified start and end dates
- Returned a JSON list of the min, max, and average temperatures
<img width="893" alt="Screenshot 2023-03-14 at 12 24 57 PM" src="https://user-images.githubusercontent.com/119909433/225087768-3a7502c4-a8c3-40c7-86fa-4861ba147177.png">
<img width="568" alt="Screenshot 2023-03-14 at 12 25 18 PM" src="https://user-images.githubusercontent.com/119909433/225087852-82e365dd-7ccc-4307-809e-d435db349c79.png">



# Author 
-Brittany Wright github:brittanynicole7
