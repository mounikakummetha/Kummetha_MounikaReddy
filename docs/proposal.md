# Personalized Recipe Recommender System

**Prepared for UMBC Data Science Master Degree Capstone by Dr. Chaojie (Jay) Wang**  
**Author**: Mounika Reddy Kummetha  
**GitHub Profile**: https://github.com/mounikakummetha/UMBC-DATA606-FALL2023-MONDAY 


---

## Background

### What is it about?
The project aims to recommend personalized recipes to users based on their dietary preferences, past ratings, and ingredient availability.

### Why does it matter?
With the rise of health consciousness and diverse dietary needs, a personalized recipe recommendation can help users find the best recipes that align with their preferences and health requirements.

### Research Questions:
- Can we provide accurate recipe recommendations based on user preferences?
- How do different ingredients and user ratings influence recipe recommendations?

---

## Data

### Data Sources:
[Kaggle's Food.com Recipes and Interactions dataset](https://www.kaggle.com/datasets/shuyangli94/food-com-recipes-and-user-interactions).

### Data Attributes:
- **Data Size**: ~500 MB
- **Data Shape**: ~230,000 recipes and 1 million interactions
- **Time Period**: Not time-bound
- **Each Row Represents**: A recipe or a user interaction

### Data Dictionary:
| Column Name      | Data Type      | Definition                                                                 |
|------------------|----------------|----------------------------------------------------------------------------|
| Recipe name      | String         | Name of the recipe                                                         |
| Ingredients      | String         | List of ingredients                                                        |
| User ratings     | Integer        | Ratings given by users                                                     |
| ...              | ...            | ...                                                                        |

**Note**: Potential values for `dietLabel` could be Vegan, Vegetarian, Gluten-Free, etc.

- **Target/Label**: User Ratings
- **Features/Predictors**: Ingredients, Dietary Labels, etc.




