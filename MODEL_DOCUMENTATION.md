MODEL DOCUMENTATION

Instagram User Analytics Using Machine Learning

Version: 1.0

Machine Learning Model Documentation

──────────────────────────

Model Overview

The Instagram User Analytics project uses a supervised machine learning regression model to predict the number of likes an Instagram post may receive.

The model learns patterns from historical Instagram engagement data and generates predictions using selected engagement-related features.

Model Goal:

Predict the number of likes on Instagram posts.

Problem Type:

Regression

Learning Type:

Supervised Machine Learning

──────────────────────────

Algorithm Used

Model Name:

Gradient Boosting Regressor

Library:

Scikit-Learn

Category:

Ensemble Learning

Regression Algorithm

Reason for Selection:

• Handles non-linear relationships effectively

• Provides strong predictive performance

• Works well with small and medium datasets

• Reduces prediction errors through boosting

• Generates stable predictions

──────────────────────────

Data Source

Dataset Name:

Instagram_dataset.csv

Dataset Source:

Kaggle

Dataset Type:

Structured Social Media Dataset

Purpose:

To analyze Instagram engagement and train a predictive model.

──────────────────────────

Input Features

The model is trained using the following variables.

Feature 1

Followers

Description:

Total number of followers of the Instagram account.

Data Type:

Numeric

Role:

Independent Variable

──────────────────────────

Feature 2

Time Since Posted

Description:

Amount of time passed since the post was published.

Examples:

1 Hour

1 Day

1 Week

1 Month

Data Type:

Numeric

Role:

Independent Variable

──────────────────────────

Target Variable

Target:

Likes

Description:

The total number of likes received by an Instagram post.

Data Type:

Numeric

Role:

Dependent Variable

Purpose:

Prediction Output

──────────────────────────

Data Preprocessing Before Training

The following preprocessing operations are performed before training.

Missing Value Handling

Missing values are identified and replaced using mean value imputation.

Benefits:

• Improved dataset quality

• Better prediction performance

──────────────────────────

Time Conversion

Instagram posting time data is converted into numerical values.

Examples:

1 Hour = 1

1 Day = 24

1 Week = 168

1 Month = 720

Purpose:

Allow machine learning algorithms to process time information.

──────────────────────────

Feature Scaling

Method Used:

StandardScaler

Purpose:

Normalize numerical values before model training.

Benefits:

• Better feature consistency

• Improved training performance

• Reduced bias caused by feature magnitude

──────────────────────────

Train-Test Split

Dataset Division

Training Data:

90%

Testing Data:

10%

Function Used:

train_test_split()

Random State:

42

Purpose:

Evaluate model performance using unseen data.

──────────────────────────

Model Training Workflow

Step 1

Load Dataset

↓

Step 2

Preprocess Data

↓

Step 3

Handle Missing Values

↓

Step 4

Convert Time Data

↓

Step 5

Select Features

↓

Step 6

Scale Features

↓

Step 7

Split Dataset

↓

Step 8

Train Gradient Boosting Regressor

↓

Step 9

Generate Predictions

↓

Step 10

Evaluate Model

──────────────────────────

Prediction Process

The trained model receives:

Input:

Followers

Time Since Posted

Processing:

Feature Scaling

↓

Gradient Boosting Prediction

↓

Output Generation

Output:

Predicted Likes

──────────────────────────

Evaluation Method

The model is evaluated using:

Actual Values

vs

Predicted Values

Visualization:

Scatter Plot

Performance Metric:

R² Score

Purpose:

Measure how accurately the model predicts Instagram likes.

──────────────────────────

Example Prediction Scenarios

Scenario 1

Followers: 100

Expected Outcome:

Lower engagement level

──────────────────────────

Scenario 2

Followers: 200

Expected Outcome:

Moderate engagement level

──────────────────────────

Scenario 3

Followers: 1000

Expected Outcome:

Higher engagement level

──────────────────────────

Model Strengths

• Fast training process

• Good regression performance

• Handles complex patterns

• Suitable for social media datasets

• Easy to interpret results

• Reliable prediction capability

──────────────────────────

Model Limitations

• Small dataset size

• Limited feature availability

• No real-time Instagram data

• No sentiment analysis data

• Dependent on historical records

──────────────────────────

Potential Improvements

Future model enhancements may include:

• XGBoost

• Random Forest

• LightGBM

• Deep Neural Networks

• LSTM Networks

• Transformer-Based Models

These models may improve prediction accuracy and scalability.

──────────────────────────

Business Applications

The trained model can be used for:

• Influencer Analytics

• Social Media Marketing

• Content Optimization

• Engagement Forecasting

• Campaign Planning

• Audience Growth Analysis

──────────────────────────

Conclusion

The Gradient Boosting Regressor successfully serves as the core predictive engine of the Instagram User Analytics project. By utilizing follower count and posting time information, the model estimates post engagement levels and provides valuable insights that can support better content strategy and social media decision-making.
