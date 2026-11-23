#  Customer Review Sentiment Analysis & Recommendation Prediction Using NLP

##  Project Overview

Customer reviews are one of the most valuable sources of feedback for e-commerce businesses. They help companies understand customer satisfaction, identify product-related issues, and improve the overall shopping experience.

In this project, I analyzed **22,000+ customer reviews** from a Women's Clothing E-Commerce dataset using Natural Language Processing (NLP), Machine Learning, and Topic Modeling techniques.

The main objective was to extract meaningful insights from customer feedback, identify unhappy customers, predict product recommendations, and discover the major topics influencing customer satisfaction.

##  Business Objectives

- Analyze customer reviews to understand overall customer sentiment.
- Identify negative reviews and potentially dissatisfied customers.
- Predict whether a customer would recommend a product based on review text.
- Discover common themes and topics discussed by customers.
- Understand the relationship between customer feedback, product categories, and recommendations.
- Provide actionable insights to help improve product quality and customer experience.

##  Project Workflow

The project follows an end-to-end NLP and Machine Learning workflow:

1. **Data Understanding**
   - Explored dataset dimensions, columns, data types, and statistical summaries.
   - Analyzed customer ratings, recommendations, and review distribution.

2. **Data Cleaning & Preprocessing**
   - Handled missing values and duplicate records where applicable.
   - Cleaned review text and prepared it for NLP processing.
   - Applied text preprocessing techniques using NLTK.

3. **Exploratory Data Analysis (EDA)**
   - Analyzed customer ratings and recommendation patterns.
   - Examined positive, neutral, and negative review distributions.
   - Compared customer feedback across product categories and age groups.

4. **Sentiment Analysis**
   - Classified customer reviews into positive, neutral, and negative sentiment categories.
   - Identified patterns in customer satisfaction and dissatisfaction.

5. **Text Vectorization**
   - Applied TF-IDF (Term Frequency–Inverse Document Frequency).
   - Used unigram and bigram features to capture important words and phrases.

6. **Machine Learning Model Development**
   - Trained and compared multiple classification algorithms.
   - Applied class balancing to improve the detection of negative reviews.
   - Evaluated models using accuracy, recall, and ROC-AUC.

7. **Topic Modeling**
   - Implemented Latent Dirichlet Allocation (LDA).
   - Identified five major themes from customer reviews.

8. **Business Insights & Recommendations**
   - Converted analytical findings into actionable business insights.

##  Technologies & Libraries

| Category | Tools & Technologies |
|---|---|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn, WordCloud |
| NLP & Text Processing | NLTK |
| Text Vectorization | TF-IDF |
| Machine Learning | Scikit-learn |
| Classification Models | Logistic Regression, Random Forest, Naive Bayes |
| Topic Modeling | Latent Dirichlet Allocation (LDA) |
| Development Environment | Jupyter Notebook |

##  Machine Learning Model Performance

### 1. Negative Review Classification

The objective was to identify negative customer reviews accurately. Since negative reviews represented a smaller portion of the dataset, detecting dissatisfied customers was particularly important.

| Model | Accuracy | Negative Review Recall |
|---|---:|---:|
| Naive Bayes | 87% | 49% |
| Random Forest | 87% | 52% |
| Logistic Regression (Class Balanced) | **88%** | **86%** |

**Best Performing Model: Logistic Regression with Class Balancing**

- Achieved 88% accuracy.
- Improved negative review recall to 86%.
- Achieved a ROC-AUC score of 0.94.

The class-balanced Logistic Regression model performed best at identifying negative customer feedback compared with the other tested models.

### 2. Product Recommendation Prediction

A separate TF-IDF-based Logistic Regression model was developed to predict whether a customer would recommend a product based on review text.

- Accuracy: **89%**
- ROC-AUC: **0.947**

### 3. Rating Prediction

An additional model was developed to predict customer ratings from review text.

- Accuracy: **62%**
- Average prediction error: Approximately **0.56 stars**

##  Topic Modeling – Customer Review Themes

Using Latent Dirichlet Allocation (LDA), five major themes were identified from customer reviews.

| Topic | Key Findings |
|---|---|
| Fabric & Comfort | 93% positive sentiment and 96% recommendation rate |
| Size & Fit | 84% positive sentiment and 89% recommendation rate |
| Look & Style | 29% negative reviews, 3.39 average rating |
| Occasion & Gifting | Mixed customer feedback, with a 3.49 average rating |
| Quality Complaints | Identified as a separate theme in customer feedback |

These topics helped identify which product attributes were associated with positive and negative customer experiences.

##  Key Business Insights

### 1. Customer Sentiment Distribution
- Positive reviews: 77%
- Neutral reviews: 12.5%
- Negative reviews: 10.5%

The majority of customers expressed positive experiences, but negative reviews provided important opportunities for improvement.

### 2. Customer Recommendation Behaviour
- Among 17,448 positive reviewers, 17,261 recommended the product.
- Among 2,370 negative reviewers, only 109 recommended the product.

This highlights a strong relationship between customer sentiment and product recommendation behaviour.

### 3. Product Category Analysis
- The Trend subcategory recorded approximately 18% negative reviews.
- Other categories recorded approximately 9–11% negative reviews.

This indicates that the Trend subcategory deserves further investigation to identify potential product-related issues.

### 4. Recommendation Across Channels
- Web recommendation rate: 81.7%
- Mobile recommendation rate: 82.2%

Recommendation behaviour was nearly similar across both shopping channels.

### 5. Customer Age Groups
Recommendation rates across customer age groups were approximately 81–85%, indicating relatively consistent recommendation behaviour across age segments.

##  Business Recommendations

Based on the analysis, the following actions can help improve customer satisfaction:

- **Improve Product Quality:** Investigate recurring quality complaints and prioritize products receiving negative feedback.
- **Optimize Size & Fit Information:** Improve size charts and product descriptions to reduce sizing-related dissatisfaction.
- **Review Product Styling:** Analyze negative feedback related to look and style to understand customer expectations.
- **Monitor High-Negative Categories:** Pay closer attention to the Trend subcategory due to its higher negative review share.
- **Use NLP for Feedback Monitoring:** Implement automated review classification to identify dissatisfied customers more efficiently.
- **Improve Product Recommendations:** Use customer review insights to understand the factors influencing recommendation decisions.

##  Project Outcomes

- Analyzed more than 22,000 e-commerce customer reviews.
- Performed sentiment analysis to understand customer satisfaction.
- Built and compared multiple Machine Learning classification models.
- Achieved 86% recall for negative reviews using class-balanced Logistic Regression.
- Developed a product recommendation prediction model with 89% accuracy.
- Identified five major customer feedback themes using LDA.
- Extracted actionable business insights related to product quality, fit, style, and customer recommendations.



**Note:** Place the dataset in the appropriate project directory and update the dataset file path in the notebook before running it. The dataset is not included in this repository unless separately uploaded.

##  Author

**Data Analytics & Machine Learning Project**

Interested in Data Analytics, Natural Language Processing, Machine Learning, and transforming raw data into meaningful business insights.

---

 If you find this project useful, feel free to explore the repository and share your feedback!
