# Personalized Recipe Recommender System

This repository contains all the necessary files and documentation for the "Personalized Recipe Recommender System" project, prepared as a capstone for the UMBC Data Science Master's Degree program by Dr. Chaojie (Jay) Wang.

## Author

- **[Your Actual Name]**
  - GitHub: [Your Actual GitHub Profile](https://github.com/youractualusername)
  - LinkedIn: [Your Actual LinkedIn Profile](https://www.linkedin.com/in/youractualusername)
  - PowerPoint Presentation: [View Actual Presentation](https://linktoyouractualpresentation.com)
  - YouTube Video: [Watch Actual Video](https://linktoyouractualvideo.com)

## Background

The "Personalized Recipe Recommender System" is designed to develop a system that recommends personalized recipes to users by analyzing their dietary preferences, historical ratings, and ingredient availability. Such a system is pivotal as it aims to intelligently suggest recipes tailored to individual preferences, thus enhancing the user experience, promoting healthier eating habits, and accommodating a myriad of dietary restrictions and preferences.

### Research Questions

- Can a machine learning model be trained to accurately recommend recipes based on individual user preferences?
- What is the impact of ingredient profiles and user rating histories on the quality of recipe recommendations?

## Data

The data for this project is sourced from Kaggle's Food.com Recipes and Interactions dataset.

- **Data Size:** Approximately 500 MB
- **Data Shape:** About 230,000 recipes and 1 million user interactions
- **Each Row Represents:** Detailed information on individual recipes or user interactions with the recipes

### Data Dictionary

| Column Name     | Data Type         | Definition                                                        |
|-----------------|-------------------|-------------------------------------------------------------------|
| Recipe_ID       | Integer           | Unique identifier for each recipe                                 |
| Recipe_Name     | String            | The title of the recipe                                           |
| Ingredients     | String (List)     | Array of ingredients used in the recipe                           |
| Dietary_Labels  | String            | Classification according to dietary restrictions (e.g., Vegan)    |
| User_ID         | Integer           | Unique identifier for each user                                   |
| User_Ratings    | Float             | Ratings provided by users for the recipes                         |

### Target/Label

- The target variable is the **User Ratings**, which the recommender system aims to predict.

### Features/Predictors

- The features include **Ingredients**, **Dietary_Labels**, **User Preferences**, and **Past Ratings**.
