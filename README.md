


# **# What’s Cooking**
_**Prepared for: Foundations of DataScience, Capstone Project**_

_**Prepared by: Durgamallesh Sunkara**_

_**December 20, 2015**_




## Objective
This project has been picked from one of the Kaggle competitions. Even though this might not address a real problem (or may be it does?), it has a lot of scope for learning and similar principles can be applied to several other classification problems. 
The primary objective of the project is to predict the type of cuisine based on the list of ingredients used in the dish. A classification model will be developed based on a training dataset and then be used to product the cuisines in a test dataset. 


## Data Sources

The Data source for this project is provided by Yummly on Kaggle here. The data is in JSON format with the attributes: Dish ID, Cuisine and Ingredients list in the training set. In test dataset cuisine is excluded (as expected, isn’t it?). Sample data shown below:

 {
 "id": 24717,
 "cuisine": "indian",
 "ingredients": [
     "tumeric",
     "vegetable stock",
     "tomatoes",
     "garam masala",
     "naan",
     "red lentils",
     "red chili peppers",
     "onions",
     "spinach",
     "sweet potatoes"
 ]
 },

##  Project Outline:
The project would be executed in three different steps. 

Data Ingestion: Read the JSON data and format it in a way, so that we can build a matrix with the list of all the ingredients against all the dishes and cuisines.

Data Exploration and cleansing: Once the JSON data is read, different ingredients will be analyzed and cleansed as required. For. e.g, coconut/ shredded coconut/frozen shredded coconut will all be considered as coconut. Any common ingredients found across all the cuisines or majority of cuisines will not be considered while building the model.

Build the Model: Once the data is ready for model, it will be split into a test and training. Once the model is built on training part, we will use test dataset to verify the accuracy of our model, before trying it on the final test dataset. 


## Deliverables:
The deliverables for this project would include the following: 
 R markdown file including the code for data ingestion, data exploration, cleansing and model building.
Cookbook to explain the variables in the dataset.
training and test datasets.
Submission file with the predicted values.
