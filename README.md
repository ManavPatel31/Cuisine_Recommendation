# Cuisine Recommendation Using Association Rules
This is the code to recommend different cuisines using Association Rules

Recommender App for Top Ingredients in a Cuisine Type

This project is about building a small recommender app that recommends the top ingredients used in a certain cuisine type based on recipe data collected from the web. The app uses the Apriori algorithm to come up with the rules and is implemented in Python.

Data Analysis and Exploration
Before building the app, some basic data analysis and exploration were carried out on the recipe data provided in the "recipes.Json" file. The following information was noted:

Total number of instances of recipes: 39774
Number of cuisines available in the data: 20
Table illustrating each cuisine type and the number of recipes available in the file related to that cuisine:
| Cuisine Type | Number of Recipes |
|--------------|-------------------|
|greek | 1175 |
|southern_us | 4320 |
|filipino	|755|
|indian |	3003 |
|jamaican	| 526 |
|spanish |	989 |
|italian | 7838 |
|mexican|	6438|
|chinese|	2673|
|british|	804|
|thai|	1539|
|vietnamese|	825|
|cajun_creole|	1546|
|brazilian|	467|
|french|	2646|
|japanese	|1423|
|irish	|667|
|korean|	830|
|moroccan|	821|
|russian	|489|

# App Functionality
The app receives a cuisine type as input from the user and uses the Apriori algorithm to analyze all the ingredients available under the inputted cuisine type. The support value is set to 100/total number of recipes for the selected cuisine, and the confidence value is set to 0.5.

If the cuisine type is not available, the app replies with "We don't have recommendations for XXX", where XXX is the inputted cuisine type, and prompts the user to enter a different cuisine type.

After analyzing the ingredients, the app presents back to the user the top group of ingredients calculated by the algorithm for the inputted cuisine type, i.e., the most frequent dataset, and all rules with lift value greater than two.

The app continues to accept input from the user and respond until the user enters an "exit" text.

# Running the App
To run the app, download the "recipes.Json" file and the Python script "firstname_cusine_recommender.py" and run the script from the command prompt without errors. The script will prompt the user to enter a cuisine type and display the recommendations as described above.

# Conclusion
The Recommender App for Top Ingredients in a Cuisine Type is a useful tool for those looking to discover popular ingredients in different cuisines. With the ability to analyze large recipe datasets, the app provides valuable insights into the most frequently used ingredients and offers recommendations to users based on their inputted cuisine type.
