# Video_Games_Rating

**Machine Learning Problem: Video Games Rating Prediction**

This machine learning problem focuses on predicting video game ratings based on various features. These features include the year of release, genre, platform, publisher, global sales, critic score, critic count, user score, and user count.

**Model Details:**

The model used for this task is the XGBClassifier, which is a type of gradient boosting algorithm known for its effectiveness in handling complex datasets and providing accurate predictions.

**Pipeline for Categorical Feature Processing:**

To ensure accurate predictions, a pipeline was constructed to preprocess categorical features before feeding them into the XGBClassifier model. This preprocessing step is crucial for handling categorical data effectively and improving the overall model performance.

**Deployment on Streamlit:**

The trained XGBClassifier model has been successfully deployed on Streamlit, allowing users to input relevant data such as the year of release, genre, platform, publisher, global sales, critic score, critic count, user score, and user count. The model then processes this input to predict the video game rating, providing valuable insights for decision-making purposes.
