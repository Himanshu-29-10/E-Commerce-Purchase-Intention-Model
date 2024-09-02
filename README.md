# E-Commerce Purchase Intention Model

## Aim
The aim of this project is to develop a predictive model that determines the purchase intention of users in an e-commerce setting. By analyzing user data, the model aims to identify patterns and features that indicate a likelihood of purchase, thus enabling better targeting and personalized marketing strategies.

## Dataset Details
- **Dataset Description**: The dataset includes user interactions on an e-commerce platform, capturing features such as session duration, product views, and demographic information. The target variable is the user's purchase intention, labeled as a binary outcome.
  
- **Key Features**:
  - **Session Duration**: Time spent by the user in a session.
  - **Product Views**: Number of products viewed during the session.
  - **Demographics**: Information like age, gender, and location.
  - **Page Interaction**: Clicks and navigation patterns during the session.

## Data Preprocessing
- **Handling Missing Values**: Missing data was addressed by imputing with median values for numerical features and the most frequent value for categorical features.
- **Encoding Categorical Variables**: Categorical variables were encoded using one-hot encoding to transform them into a format suitable for machine learning models.
- **Feature Scaling**: Numerical features were standardized to ensure that they are on a similar scale, which helps in improving the performance of certain machine learning algorithms.

## Model Selection
- **Chosen Model**: A logistic regression model was selected for its simplicity and interpretability. Logistic regression is well-suited for binary classification tasks like this one. Additionally, more complex models such as Random Forest and Gradient Boosting were explored to compare performance.
- **Reasoning**: The logistic regression model was chosen initially for its ease of implementation and ability to provide probabilistic outputs. It also allows for easy interpretation of feature importance, which is valuable in understanding the factors influencing purchase intention.

## Feature Engineering
- **Interaction Features**: Interaction terms between certain features (e.g., session duration and product views) were created to capture relationships that may not be apparent in the original features.
- **Feature Selection**: Recursive Feature Elimination (RFE) was used to identify the most important features, reducing the dimensionality and potentially improving model performance.

## Observations
- **ROC/AUC**: The model achieved a ROC/AUC score of 0.82, indicating a strong ability to distinguish between users with and without purchase intentions.
- **Accuracy**: The model's accuracy is 0.87, reflecting a high overall prediction correctness.
- **F1 Score**: The F1 score is 0.65, which balances precision and recall, highlighting the model's performance on the minority class.

## Conclusion
This project successfully developed a predictive model for e-commerce purchase intentions, with solid performance metrics such as high accuracy and a respectable ROC/AUC score. The model effectively identifies potential customers likely to make a purchase, aiding in targeted marketing strategies. However, there is room for improvement, particularly in addressing class imbalance to enhance the prediction of the minority class.

**Run this command on command prompt(cmd)** to your local machine:
   ```bash 
    pip install -r requirements.txt
