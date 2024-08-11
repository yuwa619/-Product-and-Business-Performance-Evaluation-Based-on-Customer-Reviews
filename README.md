# -Product-and-Business-Performance-Evaluation-Based-on-Customer-Reviews


## Project Overview

This project aims to evaluate ASDA's business performance by analyzing customer reviews from Trustpilot. Through sentiment analysis and various machine learning models, the project provides insights into customer sentiment and identifies key areas of commendation and concern. The goal is to leverage these insights to improve customer satisfaction and business operations.

## Methodology

### 1. **Data Collection**
   - **Source**: Customer reviews were scraped from Trustpilot using Python and the BeautifulSoup library.
   - **Data Range**: The dataset includes reviews from January 1, 2017, to September 30, 2023, consisting of 11,009 reviews.
   - **Challenges**: Pagination and potential IP blocking were handled using VPN for IP rotation.

### 2. **Exploratory Data Analysis (EDA)**
   - **Objectives**: Identify patterns, trends, and key topics in customer reviews.
   - **Techniques Used**:
     - Word counts per review.
     - Distribution of review ratings over time.
     - Sentiment analysis using TextBlob and VADER.
     - Topic modeling through Latent Semantic Analysis (LSA).
     - Aspect-based sentiment analysis using spaCy.
     - WordCloud generation to visualize common terms in positive and negative sentiments.

### 3. **Data Preprocessing**
   - **Text Processing**: Includes lowercase conversion, punctuation removal, stop word elimination, lemmatization, and stemming.
   - **Feature Engineering**: Analysis of stop word percentages, positive word percentages, and polarity/subjectivity using TextBlob.
   - **Data Imbalance Handling**: Reviews were categorized into positive and negative sentiments, addressing the imbalance with a predominance of negative sentiments.

### 4. **Model Building**
   - **Models Tested**: Logistic Regression, Random Forest, Support Vector Classification, Gradient Boosted Classifier.
   - **Optimization**: GridSearch was used to fine-tune hyperparameters. Standard scaling ensured uniform feature scales.
   - **Performance Metrics**: Accuracy, Precision, Recall, Specificity, F1 Score.

## Results

### **Performance Metrics**
   - **Average Rating**: The average rating identified was 1.459 stars, with significant fluctuations observed around the COVID-19 lockdown period.
   - **Customer Feedback**: Key themes identified include customer service, delivery issues, product quality, and refund processes.

### **Sentiment Analysis**
   - **Sentiment Distribution**: Over 60% of reviews expressed negative sentiments, consistently observed across different time periods.
   - **Topic Modeling**: Common topics identified include delivery and ordering processes, customer service, product issues, and app functionality.

### **Machine Learning Model**
   - **Best Model**: The Gradient Boosted Classifier emerged as the best-performing model for predicting customer sentiment.
   - **Feature Importance**: The percentage of positive words was identified as the most distinguishing feature between positive and negative reviews.

## Conclusion

This project provides a comprehensive analysis of ASDA's business performance through customer reviews. The insights gained can inform strategies to enhance customer satisfaction and business operations.

## Future Work
- **Expand Dataset**: Incorporate more recent reviews and other sources like social media.
- **Refine Models**: Explore advanced models and ensemble methods.
- **Deploy Models**: Implement the models in a real-time sentiment analysis system for ongoing feedback and business improvement.

