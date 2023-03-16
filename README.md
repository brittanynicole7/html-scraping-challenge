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

- Calculated how many months were on Mars
<img width="948" alt="Screenshot 2023-03-15 at 8 07 54 PM" src="https://user-images.githubusercontent.com/119909433/225483565-b260bc9c-a0d5-44c9-b697-5b7bf90188e3.png">

- Calculated how many Martian days' worth of data there were 
<img width="1019" alt="Screenshot 2023-03-15 at 8 08 20 PM" src="https://user-images.githubusercontent.com/119909433/225483623-0ff163ee-d57e-426e-aaca-702917ac5895.png">

- Calculated the average low temperature by month and plotted the values
<img width="1264" alt="Screenshot 2023-03-15 at 8 08 48 PM" src="https://user-images.githubusercontent.com/119909433/225483679-95754105-12c8-43e3-b9c5-93d13048a0ff.png">
<img width="974" alt="Screenshot 2023-03-15 at 8 09 00 PM" src="https://user-images.githubusercontent.com/119909433/225483702-5a03449e-4074-4fdb-9636-069f37568bb5.png">

- Calculated the lowest and highest months 
<img width="853" alt="Screenshot 2023-03-15 at 8 09 25 PM" src="https://user-images.githubusercontent.com/119909433/225483742-36502feb-eb34-4a5b-8537-801177110975.png">
<img width="1148" alt="Screenshot 2023-03-15 at 8 09 38 PM" src="https://user-images.githubusercontent.com/119909433/225483756-6f4092f3-2d06-4446-886a-9a9c18b42628.png">

- Calculated the average pressure by month and plotted the values
<img width="1056" alt="Screenshot 2023-03-15 at 8 10 06 PM" src="https://user-images.githubusercontent.com/119909433/225483813-8d36c3f5-0ab2-4c31-8f44-350052783a03.png">
<img width="945" alt="Screenshot 2023-03-15 at 8 10 17 PM" src="https://user-images.githubusercontent.com/119909433/225483834-8a16684f-ead4-48fd-b1ca-f7f354557ce7.png">

- Calculated which months had the highest and lowest average pressure
<img width="719" alt="Screenshot 2023-03-15 at 8 10 41 PM" src="https://user-images.githubusercontent.com/119909433/225483889-02a15044-5090-4089-b0f2-7550a8bbd82b.png">
<img width="1039" alt="Screenshot 2023-03-15 at 8 10 52 PM" src="https://user-images.githubusercontent.com/119909433/225483913-54664e0b-f7cd-4f91-8cdd-f4814d7de9a9.png">

- Did a rough calculation based on a plot of how many earth days there are in a Martian year
<img width="1365" alt="Screenshot 2023-03-15 at 8 11 38 PM" src="https://user-images.githubusercontent.com/119909433/225484007-c92aec4a-4a1b-4267-a13e-652eea1af3bb.png">

- Created a CSV file of the DataFrame
<img width="852" alt="Screenshot 2023-03-15 at 8 12 02 PM" src="https://user-images.githubusercontent.com/119909433/225484064-d631c504-21c1-4e5a-9d14-faf6d47d094c.png">
<img width="692" alt="Screenshot 2023-03-15 at 8 12 47 PM" src="https://user-images.githubusercontent.com/119909433/225484156-63b8badf-2839-451c-a1a3-861f61b44f2d.png">


# Author 
-Brittany Wright github:brittanynicole7
