# IBM_DataScience_Capstone

## Introduction
### Background
In this capstone, we will predict if the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against SpaceX for a rocket launch.

### Summary

## Methodology

### Data Collection
* Request data from SpaceX API
* Convert .json to dataframe
* Request information about launches from API using custom functions
* Create a dictionary from the data
* Implement dictionary into Pandas Dataframe
* Filter dataframe to only contain Falcon 9 launches
* Export to .csv file
  
#### API
* Request data from Wikipedia
* Create BeautifulSoup object from HTML response
* Extract column names from HTML tables
* Collected data from parsing HTML tables
* Created dictionary from the data
* Created dataframe from dictionary
* Export data to .csv file
  
#### Webscraping
* Checked for null values
* Calculated the number of launches at each site
* Calculated the number of orbit occurences
* Created a binary label column from the outcomes
* Handled null values
  
### Data Wrangling

### EDA with Visualizations
* Scatterplot looking at relationshipb between flight numbers and launch sites
* Scatterplot looking at relaitonship between payload mass and launch sites
* Bar chat looking at the success rate of each orbit
* Scatter plot looking at relationship between flight number and orbit type
* Scatter plot looking at relationship between payload mass and orbit type
* Line chart looking at trend of success by year
  
### EDA with SQL
* Queried the data to understand more about the data

### Maps with Folium
* Created dynamic interactive maps using Folium to visualize launch sites across the country, launch outcomes and some local proximites
  
### Dashboard with Plotly Dash
* Created dynamic dashboard hosted on local server
* Included piechart show successful launches
* Included Scatter plot showing Payload Mass vs Launch Outcomes with adjustable payload slider
  
### Predictive Models
* Split 
## Conclusion
