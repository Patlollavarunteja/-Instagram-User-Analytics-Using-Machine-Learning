DATA_PREPROCESSING

Instagram User Analytics Using Machine Learning

Version: 1.0

Data Preprocessing Documentation

──────────────────────────

Introduction

Data preprocessing is one of the most important stages of the machine learning workflow. Raw Instagram data often contains inconsistencies, missing values, and non-numeric information that cannot be directly processed by machine learning algorithms.

The purpose of preprocessing is to transform raw data into a clean and structured format suitable for analysis and model training.

──────────────────────────

Preprocessing Objectives

The main objectives of preprocessing in this project are:

• Improve data quality

• Remove inconsistencies

• Handle missing values

• Convert text-based information into usable formats

• Normalize numerical features

• Prepare machine learning input variables

──────────────────────────

Dataset Loading

The Instagram dataset is loaded into a Pandas DataFrame.

Purpose:

• Read CSV file

• Store records in a structured format

• Enable data manipulation and analysis

Output:

Dataset available for preprocessing.

──────────────────────────

Dataset Inspection

The dataset structure is inspected before performing any transformations.

Inspection Activities

• Check column names

• Identify data types

• Verify record count

• Detect missing values

• Understand feature distribution

Purpose

To understand the quality and structure of available data.

──────────────────────────

Missing Value Handling

Problem

Datasets may contain empty or null values.

Examples

Missing likes

Missing posting time

Missing engagement information

Solution

The project identifies missing values and replaces them using Mean Imputation.

Method Used

SimpleImputer

Strategy

Mean

Benefits

• Prevents model failure

• Maintains dataset completeness

• Improves prediction quality

──────────────────────────

Time Conversion Process

Problem

The "Time Since Posted" column contains text values.

Examples

1 hour

2 hours

1 day

2 weeks

1 month

Machine learning models cannot directly process text-based time values.

Solution

Convert time information into numeric values.

Conversion Logic

1 Hour = 1

1 Day = 24

1 Week = 168

1 Month = 720

Examples

2 Hours → 2

3 Days → 72

2 Weeks → 336

1 Month → 720

Benefits

• Converts categorical data into numerical format

• Enables machine learning processing

• Creates measurable engagement features

──────────────────────────

Feature Selection

Not all columns contribute equally to prediction.

Selected Features

Followers

Time Since Posted

Reason

These features showed strong relationships with engagement metrics.

Benefits

• Reduces complexity

• Improves model performance

• Eliminates unnecessary variables

──────────────────────────

Target Variable Preparation

Target Variable

Likes

Purpose

The machine learning model learns patterns to predict the number of likes.

Role

Dependent Variable

Benefits

Provides measurable engagement output.

──────────────────────────

Target Scaling

Purpose

Normalize like values before training.

Procedure

Maximum likes value is identified.

Every record is divided by the maximum value.

Formula

Normalized Likes = Likes ÷ Maximum Likes

Benefits

• Improves model stability

• Prevents large value dominance

• Better numerical representation

──────────────────────────

Feature Matrix Construction

Input Matrix

X

Contains:

• Followers

• Time Since Posted

Output Vector

Y

Contains:

• Likes

Purpose

Prepare data for machine learning training.

Structure

X → Independent Variables

Y → Dependent Variable

──────────────────────────

Data Splitting

Purpose

Evaluate machine learning performance using unseen data.

Method

Train-Test Split

Distribution

Training Data: 90%

Testing Data: 10%

Benefits

• Prevents overfitting

• Measures generalization ability

• Improves evaluation quality

──────────────────────────

Feature Scaling

Problem

Followers and time values exist on different numerical scales.

Example

Followers = 1000

Time = 24

These differences may negatively affect model performance.

Solution

Standardization

Method Used

StandardScaler

Transformation Formula

Z = (X − Mean) / Standard Deviation

Benefits

• Consistent feature ranges

• Improved learning process

• Higher model performance

──────────────────────────

Data Validation

Quality checks performed after preprocessing.

Validation Steps

✓ Missing value verification

✓ Data type verification

✓ Feature scaling verification

✓ Shape consistency checks

✓ Train-test split verification

Purpose

Ensure reliable training data.

──────────────────────────

Process Flow

Raw Dataset

↓

Dataset Inspection

↓

Missing Value Detection

↓

Missing Value Imputation

↓

Time Conversion

↓

Feature Selection

↓

Target Preparation

↓

Feature Matrix Creation

↓

Train-Test Split

↓

Feature Scaling

↓

Validated Dataset

↓

Machine Learning Training

──────────────────────────

Benefits of Preprocessing

The preprocessing pipeline provides several advantages.

• Improved data quality

• Reduced noise

• Consistent feature representation

• Better machine learning performance

• More reliable predictions

• Increased model stability

• Faster model training

──────────────────────────

Challenges Addressed

Challenge

Missing Values

Solution

Mean Imputation

──────────────────────────

Challenge

Text-Based Time Information

Solution

Numeric Conversion

──────────────────────────

Challenge

Feature Scale Differences

Solution

StandardScaler

──────────────────────────

Challenge

Data Inconsistency

Solution

Data Validation

──────────────────────────

Impact on Model Performance

Proper preprocessing significantly improved the effectiveness of the Gradient Boosting Regression model by providing:

• Cleaner input data

• Better feature representation

• Reduced training noise

• Improved prediction accuracy

• Enhanced model reliability

──────────────────────────

Conclusion

Data preprocessing serves as the foundation of the Instagram User Analytics project. Through cleaning, transformation, scaling, and validation, raw Instagram engagement data is converted into a machine-learning-ready format that supports accurate analysis and prediction of post engagement metrics.
