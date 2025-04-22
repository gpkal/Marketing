# Marketing Analytics

A comprehensive analytical system to optimize marketing strategies through churn, repurchase, market basket, and sentiment analysis.

## Overview
This project implements various analytical models to support data-driven marketing strategic decisions. Starting from raw business data, we performed extensive preprocessing and analysis to develop targeted strategies for customer retention, product cross-selling, and feedback management.

## Dataset
The raw dataset consisted of seven interconnected tables:
- **Customers**
- **Customer accounts**
- **Addresses**
- **Orders** (transaction history including purchases and refunds)
- **Products** (product catalog information)
- **Customer reviews** (unstructured feedback)
- **Labelled reviews** (sentiment-labelled review subset)

## Project Scope
We established three core business objectives:
1. **Customer Focus**: Prevent high-value customer churn through targeted retention marketing campaigns
2. **Product Focus**: Increase profit through strategic product cross-selling initiatives
3. **Feedback Focus**: Address detractors and promoters through loyal engagement marketing to manage sentiment impact

## Methodology & Results

### Customer Segmentation and Churn Analysis
We developed:
- **RFM Analysis** segmenting customers into 7 value categories (Cheap, Tin, Copper, Bronze, Silver, Gold, Diamond)
- **Churn prediction models** with XGBoost achieving best performance (AUC 0.88)
- **Repurchase models** for one-shooter customers (AUC 0.91)

### Market Basket Analysis
We applied Apriori algorithm (min support 0.5%) to identify product associations with confidence ≥ 0.5.

### Sentiment Analysis
We implemented:
- Text preprocessing pipeline (tokenization, lemmatization, TF-IDF vectorization)
- Classification models with Logistic Regression achieving 72% accuracy

## Business Applications

### Customer Retention Strategy
- Target high-value segments with personalized retention offers
- Implement early intervention for customers showing churn indicators
- Design specific reactivation campaigns for dormant customers

### Cross-Selling Optimization
- Create bundled offerings based on discovered product associations
- Implement recommendation systems at checkout
- Optimize product catalog based on sales performance

### Sentiment-Based Engagement
- Develop response protocols for negative feedback
- Leverage promoters for advocacy and testimonials
- Address recurring themes in product development

---
Project by Giorgia Prina and Enrico Mannarino

*Marketing Analytics course project, 2024*  
*Master Degree in Data Science - University of Milano-Bicocca*
