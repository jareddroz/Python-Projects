# App Rating Prediction



### Table of contents
   
   - [Project Overview](#project-overview)
   - [Data Sources](#data-sources)
   - [Tools](#tools)
   - [Data Cleaning and Preparation](#data-cleaning-and-preparation)
   - [Exploratory Data Analysis](#exploratory-data-analysis)
   - [Results and Findings](#results-and-findings)
   - [Recommendations](#recommendations)
   - [Limitations](#limitations)
   - [Conclusion](#conclusion)


### Project Overview

The "App Rating Prediction" project endeavors to develop a model capable of predicting app ratings based on diverse app attributes sourced from Google Play Store data. Addressing challenges such as inconsistent data formatting, outlier treatment, and the exploration of relationships between app ratings and factors like price, size, reviews, and content categories, the project employs thorough analysis and linear regression modeling to gain insights into the influential factors affecting app ratings.


### Data Sources
 The primary dataset used for this project is the "googleplaystore.csv", containing app attributes sourced from the Google Play Store.

### Tools
    
   - Python - Data Cleaning, Data Visualization, Exploratory Data Analysis (EDA), Data Preprocessing, Model Building
   


### Data Cleaning and Preparation 
    
   - Drop Duplicates rows
   - Handling null Values
   - Data formatting
   - Data Transformation
   - Dropping Columns

### Exploratory Data Analysis
    
- Are there any outliers? Think about the price of usual apps on Play Store.
- Are there any apps with very high number of reviews? Do the values seem right?
- How are the ratings distributed? Is it more toward higher ratings?
- How are the size for apps distributed?
- What pattern do you observe? Does rating increase with price?
- Are heavier apps rated better?
- Does more review mean a better rating always?
- Is there any difference in the ratings when it comes to content rating? Are some types liked better?
- Which genre has the best ratings?

  
### Results and findings 

- Over 95% of apps are priced under $50, suggesting that a vast majority of apps have relatively affordable prices, with only a small fraction exceeding this threshold.
- Majority of reviews are under 2 million indicating reviews for apps greater than 2 million can be considered as outliers.
- The left-skewed distribution of app ratings indicates a prevalent trend where most apps receive higher ratings, with only a minority receiving lower ratings.
- A right-skewed distribution in app sizes suggests that the majority of apps have smaller file sizes, with fewer apps having larger sizes.
- There is a negative correlation between app price and review counts, implying that as app prices increase, the number of reviews tends to decrease.
- Higher-priced apps may experience lower user engagement, resulting in fewer installations and subsequently fewer reviews.
- Larger app sizes may lead to decreased user satisfaction, especially for users with limited storage or processing capabilities on their devices.
- A higher number of reviews typically indicates greater user engagement, reflecting user satisfaction and positive experiences with the app.
- Apps with content ratings such as "Everyone" and "Teen" are likely to appeal to a broader audience, potentially contributing to higher ratings.
- Categories such as Beauty, Education, Events, and Personalization exhibit higher average ratings, indicating that apps within these categories tend to be better received by users.
- The developed model indicated moderate predictive performance with room for improvement.

### Recommendations 

- Consider pricing apps competitively below $50 to align with the majority of apps in the market and appeal to a broader audience.
- Pay attention to apps with exceptionally high review counts or prices, as they may skew the overall dataset and require special consideration.
- Focus on strategies to increase user engagement, such as offering affordable pricing, optimizing app size, and encouraging user reviews through incentives or engagement campaigns.
- Invest in developing high-quality content, particularly in categories like Beauty, Education, Events, and Personalization, to enhance user satisfaction and ratings.
- Consider exploring advanced machine learning algorithms, feature engineering techniques, or incorporating additional relevant features to improve model performance and achieve a higher R2 score.

### Limitations

Lack of consideration for temporal dynamics or trends in user preferences and app ratings over time, which could potentially impact the predictive accuracy of the model, especially if user preferences evolve significantly over the dataset's duration.


### Conclusion 

The "App Rating Prediction" project successfully navigates challenges related to data inconsistencies, outlier treatment, and attribute exploration. Despite a moderate R2 score, the linear regression model provides valuable insights into the relationships between app attributes and ratings. The project significantly contributes to the understanding and prediction capabilities for app performance on the Google Play Store, offering a foundation for future improvements and refinements in predicting app ratings based on key attributes. This work serves as a valuable resource for stakeholders in the app development and marketing domain seeking to optimize their strategies for enhanced app performance and user satisfaction.
