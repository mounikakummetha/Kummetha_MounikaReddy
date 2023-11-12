## 3. Data

### Data Sources, Descriptions and Data Dictionary:

#### 1. RAW_recipes.csv:
- **Purpose:** Provides comprehensive information about each recipe, including ingredients, cooking steps, and nutritional details.
- **Columns:**
  - `recipe_id`: Integer. Unique identifier for each recipe.
  - `name`: String. The title of the recipe.
  - `minutes`: Integer. Time required to prepare and cook the recipe.
  - `contributor_id`: Integer. ID of the user who contributed the recipe.
  - `submitted`: Date. The date when the recipe was submitted.
  - `tags`: String. Categorizing tags for the recipe (e.g., "vegan").
  - `nutrition`: String. Nutritional information of the recipe.
  - `n_steps`: Integer. Number of steps in the recipe.
  - `steps`: String. Detailed cooking instructions.
  - `description`: String. A brief description of the recipe.
  - `ingredients`: String. List of ingredients used in the recipe.
  - `n_ingredients`: Integer. Number of ingredients in the recipe.

#### 2. RAW_interactions.csv:
- **Purpose:** Captures user interactions with recipes, providing insights into user preferences and behavior.
- **Columns:**
  - `user_id`: Integer. Unique identifier for each user.
  - `recipe_id`: Integer. Identifier for the interacted recipe.
  - `date`: Date. The date of the interaction.
  - `rating`: Integer. User-given rating to the recipe.
  - `review`: String. User's review or comment on the recipe.

#### 3. PP_recipes.csv:
- **Purpose:** Contains preprocessed recipe data, optimized for analysis and model training.
- **Columns:** (Similar to `RAW_recipes.csv`)

#### 4. PP_users.csv:
- **Purpose:** Includes user profile data, essential for understanding user preferences and dietary restrictions.
- **Columns:**
  - `user_id`: Integer. Unique identifier for each user.
  - `techniques`: String. Cooking techniques used or preferred by the user.
  - `items`: String. Ingredients or items used or preferred by the user.
  - `n_items`: Integer. Number of items associated with the user.
  - `ratings_count`: Integer. Total count of ratings given by the user.
  - `reviews_count`: Integer. Total count of reviews written by the user.

#### 5. interactions_train.csv, interactions_test.csv, interactions_validation.csv:
- **Purpose:** These datasets are segmented for model training, testing, and validation, containing user interactions for different phases.
- **Columns:** (Similar to `RAW_interactions.csv`)

#### 6. ingr_map.pkl:
- **Purpose:** Aids in standardizing ingredients across the datasets, ensuring data uniformity.
- **Columns:**
  - `ingredient_id`: Integer. Unique identifier for each ingredient.
  - `ingredient_name`: String. Name of the ingredient.
  - `mapped_ingredient`: String. Standardized form of the ingredient name.

### Data Size and Shape:
- The size and shape of each dataset (number of rows and columns) will be determined through data exploration.

### Time Period:
- The datasets capture recipe data and user interactions from 2010 to 2020, offering a decade's worth of culinary trends and user preferences.

### Row Representation:
- `RAW_recipes.csv`, `PP_recipes.csv`: Each row represents a unique recipe.
- `RAW_interactions.csv`, `interactions_*.csv`: Each row represents an individual user interaction.
- `PP_users.csv`: Each row represents a user profile.
- `ingr_map.pkl`: Each row represents an ingredient mapping.

### Target/Label in ML Model:
- The primary target for the machine learning models is user ratings from the interactions datasets.

### Features/Predictors for ML Models:
- Key features will include ingredients, recipe categories, user dietary restrictions, and historical interaction data.
