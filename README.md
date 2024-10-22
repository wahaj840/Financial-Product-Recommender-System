# Personalized Financial Products Recommendations

This project explores the development of various recommender systems for personalized financial product recommendations. The goal is to suggest products such as credit cards, loans, savings accounts, and insurance options based on customer data. We implemented and compared three recommendation approaches: rule-based, machine learning classification, and content-based filtering, and analyzed their performance.

## Project Overview

- **Project Name**: Personalized Financial Products Recommendations
- **Authors**: Ali Wahaj 

## Abstract

This project implements and compares three different recommender system approaches for financial products:

1. **Rule-Based Recommendation**: Uses predefined business rules to provide recommendations.
2. **Machine Learning (ML) Classification**: Applies classification algorithms to predict relevant financial products.
3. **Content-Based Filtering**: Analyzes product and customer attributes to recommend similar products.

We found that rule-based recommendations work best in controlled environments, while ML models (specifically Random Forest and SVM) provide a more flexible approach for diverse data patterns. Content-based filtering performed well in aligning products with individual customer profiles.

## Colab Notebook

You can access the full implementation of the models in the following Google Colab notebook:  
[Colab Notebook Link Here]

## Project Objective

The primary objectives of this project are:
- Develop a recommender system that provides personalized financial product recommendations (credit cards, loans, savings accounts, insurance).
- Implement and compare rule-based, machine learning classification, and content-based approaches.
- Evaluate the performance of each method and identify the most effective system for financial product recommendations.

## Dataset

- **Source**: [Kaggle - Credit Card Customers](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers/data)
- **Number of Customers**: 10,000
- **Features**: 18 columns, including demographic information and financial status, such as credit limits, spending behavior, and payment habits.

## Methodology

The project follows a structured process, including:

1. **Business Understanding**: Define business goals for personalized recommendations.
2. **Data Understanding**: Perform exploratory data analysis (EDA) to uncover patterns in the customer data.
3. **Data Preparation**: Clean the data, apply scaling, and handle imbalances.
4. **Modeling**: Implement and train the models (rule-based, ML classification, and content-based).
5. **Evaluation**: Compare the models using relevant metrics.
6. **Deployment**: Propose integration of the best-performing model.

## Recommendation Methods

### 1. Rule-Based Recommendation
A set of predefined business rules is used to recommend financial products. For example, users with high transaction amounts may be suggested cashback or rewards cards, while users with stable incomes may be suggested investment or savings products. 

### 2. Machine Learning Classification
We evaluated multiple classifiers: Random Forest, Logistic Regression, Support Vector Classification (SVC), Gradient Boosting, and k-Nearest Neighbors (k-NN). Random Forest and SVC achieved the best performance in predicting relevant financial products.

### 3. Content-Based Filtering
Content-based filtering uses cosine similarity to match financial products to customer profiles based on features such as income, spending patterns, and marital status. Products with the highest similarity to a user's profile are recommended.

## Results

### Rule-Based Recommendation
- **Accuracy**: 1.0 in a controlled environment.
- **Limitation**: While it works well under specific conditions, it may miss more complex real-world scenarios.

### Machine Learning Models
- **Best Model**: Random Forest
- **Cross-validation Score**: Random Forest achieved a score of 0.888, followed closely by SVC. Gradient Boosting and Logistic Regression performed well, while k-NN had the lowest performance.

### Content-Based Filtering
- **Top Recommendations**: Products like 'Personal Loan' and 'Life Insurance' showed high relevance to user profiles with similarity scores close to 1.

## Findings and Discussion

- **Rule-Based Approach**: Effective for straightforward scenarios but lacks adaptability for complex customer profiles.
- **Machine Learning Approach**: Random Forest and SVC are best suited for handling diverse data and customer behavior patterns.
- **Content-Based Filtering**: Highly effective for personalizing recommendations by analyzing customer attributes.

## Conclusion

This project demonstrates that integrating rule-based, machine learning, and content-based filtering approaches can significantly improve the effectiveness of personalized financial product recommendations. Each method has its strengths, with rule-based systems being efficient in predefined scenarios, while ML and content-based methods are better suited for personalized, data-driven recommendations.

### Future Work
Future improvements could include the integration of deep learning models and the adaptation of these systems to evolving customer expectations and financial landscapes.

## How to Run the Project

1. Download the notebook file `CA1_Report_Ali_Wahaj.ipynb` or access it via the Colab link.
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt



### Key Sections:
- **Project Overview**: Summarizes the project and its objectives.
- **Dataset**: Describes the data used for the project.
- **Methodology and Approaches**: Provides details about the recommendation methods implemented.
- **Results and Findings**: Summarizes the outcomes and the effectiveness of each approach.
- **How to Run the Project**: Explains how to run the project locally or in Colab.
- **Future Work and Conclusion**: Highlights possible extensions and summarizes key insights.

This `README.md` will present your project in a professional manner, providing clarity for anyone reviewing it on GitHub.
