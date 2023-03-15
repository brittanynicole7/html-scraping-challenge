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
  - How many months exist on Mars?
  - How many Martian (and not Earth) days worth of data exist in the scraped dataset?
  - What are the coldest and the warmest months on Mars (at the location of Curiosity)?    To answer this question:
    - Find the average minimum daily temperature for all of the months.
    - Plot the results as a bar chart.
  - Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
    - Find the average daily atmospheric pressure of all the months.
    - Plot the results as a bar chart.
  - About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
    - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
    - Visually estimate the result by plotting the daily minimum temperature.
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

## Deliverable 1
- Imported dependencies
<img width="622" alt="Screenshot 2023-03-15 at 5 29 02 PM" src="https://user-images.githubusercontent.com/119909433/225457708-c196ee8f-4d92-4e6a-b046-40e2013a9dc3.png">

- Visited the Mars news site, inspect it, and connect to it using an automated browser
<img width="624" alt="Screenshot 2023-03-15 at 5 29 41 PM" src="https://user-images.githubusercontent.com/119909433/225457794-f5035647-120d-4616-8229-2bb712d6dea4.png">

- Scraped the website
<img width="623" alt="Screenshot 2023-03-15 at 5 30 19 PM" src="https://user-images.githubusercontent.com/119909433/225457882-55194e6c-8919-44de-9dc1-374465217b77.png">
<img width="634" alt="Screenshot 2023-03-15 at 5 30 49 PM" src="https://user-images.githubusercontent.com/119909433/225457962-871ba2a8-96fc-4213-8a8a-c9f940fc4b8f.png">
<img width="630" alt="Screenshot 2023-03-15 at 5 31 02 PM" src="https://user-images.githubusercontent.com/119909433/225457989-77ca9945-d5c3-4d03-b0d8-8a7835b64706.png">

- Stored the results in a dictionary and then print the list
<img width="625" alt="Screenshot 2023-03-15 at 5 31 35 PM" src="https://user-images.githubusercontent.com/119909433/225458092-6180dcbf-3ab8-4c9b-a31d-c6acb8cd0fca.png">
<img width="627" alt="Screenshot 2023-03-15 at 5 31 48 PM" src="https://user-images.githubusercontent.com/119909433/225458121-1430c10b-b924-4630-8cf8-143563183f21.png">


## Deliverable 2
- Imported dependencies
<img width="628" alt="Screenshot 2023-03-15 at 5 32 27 PM" src="https://user-images.githubusercontent.com/119909433/225458216-a6875d02-9c92-439c-9577-952d21188d27.png">

- Visited the website, connect using an automated browser, and inspect the website 
<img width="626" alt="Screenshot 2023-03-15 at 5 33 03 PM" src="https://user-images.githubusercontent.com/119909433/225458299-97cad0bc-14af-4b08-a158-1405ddeb87ce.png">

- Scraped the table on the website 
<img width="631" alt="Screenshot 2023-03-15 at 5 33 30 PM" src="https://user-images.githubusercontent.com/119909433/225458378-c7914648-b6cf-4250-99f0-4eede5114d39.png">

- Stored the data in two lists for the data and headings and printed the lists
<img width="626" alt="Screenshot 2023-03-15 at 5 34 17 PM" src="https://user-images.githubusercontent.com/119909433/225458489-fa11dc87-ec02-43d9-90fd-653407ea4bda.png">

- Created a DataFrame 
<img width="620" alt="Screenshot 2023-03-15 at 5 34 45 PM" src="https://user-images.githubusercontent.com/119909433/225458551-d319f017-fdb8-49f6-a23d-0ccd7930bc8d.png">

- Examined the datatypes, changed the datatypes, and confirmed that the changes were successful
<img width="616" alt="Screenshot 2023-03-15 at 5 36 00 PM" src="https://user-images.githubusercontent.com/119909433/225458733-392b2195-ad20-4d8d-892f-9f081f0f3681.png">
<img width="635" alt="Screenshot 2023-03-15 at 5 36 10 PM" src="https://user-images.githubusercontent.com/119909433/225458760-24865b33-e90f-4cc1-97e8-069aaa938310.png">





# Author 
-Brittany Wright github:brittanynicole7
