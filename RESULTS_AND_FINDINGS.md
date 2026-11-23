Instagram User Analytics Using Machine Learning

Project Objective

The primary objective of this project was to analyze Instagram user engagement data and develop a machine learning model capable of predicting the number of likes a post may receive based on account characteristics and posting behavior.

Dataset Analysis Findings

After examining the dataset, several important observations were identified:

• User engagement is directly influenced by follower count.

• Posts from accounts with higher followers generally receive more likes.

• Post timing impacts engagement levels.

• Frequently used hashtags contribute to increased visibility.

• Certain keywords appear repeatedly in high-performing posts.

These findings indicate that both audience size and content strategy play significant roles in Instagram engagement.

Word Cloud Analysis

Caption Word Cloud Findings

The caption analysis revealed frequently occurring words used in Instagram posts.

Observations:

• Common keywords appeared repeatedly across multiple posts.

• Popular content themes became visible through word frequency.

• High-frequency terms highlighted user interests and posting trends.

Benefits:

• Understanding audience preferences.

• Identifying trending content topics.

• Improving content planning.

Hashtag Word Cloud Findings

The hashtag analysis revealed the most frequently used hashtags in the dataset.

Observations:

• Several hashtags appeared significantly more often than others.

• Frequently used hashtags were associated with better engagement.

Benefits:

• Better hashtag selection.

• Improved content discovery.

• Increased audience reach.

Exploratory Data Analysis Findings

Follower vs Likes Relationship

Regression analysis demonstrated a positive correlation between followers and likes.

Key Finding:

As follower count increases, the expected number of likes also increases.

Conclusion:

Follower count is one of the most influential features in engagement prediction.

Time Since Posted Analysis

Analysis of posting time revealed engagement patterns over time.

Key Finding:

Likes accumulate gradually as more time passes after publishing a post.

Conclusion:

Post age is an essential factor affecting engagement levels.

Machine Learning Results

Model Used

Gradient Boosting Regressor

Reason for Selection

Gradient Boosting was chosen because it can learn complex relationships between variables while maintaining strong prediction performance.

Input Features

• Followers

• Time Since Posted

Output Prediction

• Likes

Model Training Process

• Dataset preprocessing

• Missing value handling

• Feature scaling

• Train-test split

• Model learning

• Prediction generation

Prediction Results

The trained model successfully generated engagement predictions for different follower counts.

Example Scenarios Tested

Scenario 1

Followers: 100

Expected Result:

Moderate engagement growth over time.

──────────────────────────

Scenario 2

Followers: 200

Expected Result:

More engagement compared to 100 followers.

──────────────────────────

Scenario 3

Followers: 1000

Expected Result:

Significantly higher likes progression.

──────────────────────────

Observation

The prediction trend consistently showed increasing engagement with increasing follower counts.

Visualization Results

The following visual outputs were successfully generated:

✓ Caption Word Cloud

✓ Hashtag Word Cloud

✓ Followers vs Likes Regression Plot

✓ Predicted vs Actual Likes Scatter Plot

✓ Likes Progression Curves

These visualizations made engagement trends easier to understand and interpret.

Business Insights

The project generated several practical insights:

For Influencers

• Understand factors affecting engagement.

• Improve content planning strategies.

• Choose effective posting times.

For Marketers

• Estimate expected campaign performance.

• Identify audience engagement patterns.

• Optimize advertising decisions.

For Businesses

• Improve brand visibility.

• Create data-driven social media strategies.

• Increase audience interaction.

Challenges Encountered

During development, several challenges were identified:

• Small dataset size.

• Limited engagement metrics.

• Missing and inconsistent data.

• Restricted feature availability.

However, preprocessing and feature engineering techniques helped improve model effectiveness.

Project Achievements

Successfully accomplished:

✓ Data preprocessing

✓ Engagement analysis

✓ Word cloud generation

✓ Feature engineering

✓ Machine learning model development

✓ Likes prediction

✓ Visual analytics creation

✓ Insight generation

Conclusion

The project successfully demonstrated how machine learning can be applied to Instagram analytics. The analysis revealed meaningful engagement patterns, while the Gradient Boosting Regressor provided effective likes prediction based on follower count and posting time. The generated insights can support influencers, marketers, and businesses in making data-driven decisions to improve their Instagram performance.
