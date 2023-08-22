# IBM Data Science Capstone - SpaceX Cost-Effective Rocket Launches

## Summary
In this capstone project, the objective is to predict the successful landing of the Falcon 9 first stage. As SpaceX reuses this stage to cut costs, accurate predictions are vital for estimating launch expenses and competing against SpaceX. The project encompasses data collection from SpaceX API and Wikipedia through webscraping, followed by data wrangling, exploratory data analysis (EDA) using visualizations and SQL queries, interactive map creation with Folium, and a dynamic dashboard with Plotly Dash. Predictive models were developed, including Logistic Regression, SVM, KNN, and Decision Tree, with the Decision Tree model emerging as the best performer. The conclusion highlights the Decision Tree's accuracy of 83%, improved launch success rates over time, and KSC LC 39A's notable success in launches.

## Background
In this capstone, we will predict if the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against SpaceX for a rocket launch.

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
* Isolated target variable
* Standardized training data with **StandardScalar**
* Split the data using and 80/20 split
* Created a **GridSearchCV** object using 10 folds
* Tuned 4 different classification models using GridSearchCV: Logistic Regression, SVM, KNN and Decision Tree
* Calculated the accuracy score for the test sets
* Assesed the models using a confusion looking at the True predictions
* Championed the best model based on perfomance score
  
## Conclusion
* The Decision Tree was the champion models slightly outperforming the Logistic model with a better recall score and an accuracy of **83%**
* The success of launches rates get better as time goes on
* KSC LC 39A had the most sucessfull launches out of all launch sites

