# Recommendation System for Amazon's Electronic Products

# Summary:

Companies leverage recommender systems to help them identify user preferences and choices of specific products. This helps companies make important decisions such as deciding how much of a certain product to produce for a given user by predicting their needs. This will not only help users get what they want, but it also helps companies boost revenue incrementally.

**Problem Statement**
The main problems customer face when trying to purchase or browse a product online are:
- the information overload
- unlimited product choices

Having a recommendations in place will help the user find relevant content to make a better purchasing decision. Moreover, recommender systems help companies like Amazon engage directly with the user and get relevant feedback for their products.

# Dataset Attributes

[Amazon Ectronic Dataset] provides the following electronic product information:

- user_id: unique id for each user
- item_id: unique id for each product
- rating: from 1.0 - 5.0
- timestamp: time of the rating
- model_attr: what gender is the product suitable for
- category: the specific class of the electronic category
- brand: the specific electronic brand
- year: year in which the electronic was purchased
- user_attr: gender specific choices
- split

In order to build the recommender models I chose: 'user_id', 'item_id', 'rating', and 'category'

# Approach Used in Analysis

- Initial Data Exploration: read the dataset, identify anomalies and features in the dataset
- Data Cleaning and Preprocessing: 
  -- Drop irrelevant features
  -- Reduce sparsity (replaced NAN values with zeros)
- Data Exploration and data visualization
- Feature Engineering: 
  -- Singular Value Decomposition: used to reduce the dimensions in the big dataset
- Model Building
- Evaluation

# Challenges

- Sparse Dataset
- Computational Time- What platform to use, whether to run things locally or on the cloud (Google Colab)
- Proper data preprocessing- carefully recognizing and choosing the methods to clean the data
- Evaluation metrics: Choosing relevant metrics to evaluate the models
