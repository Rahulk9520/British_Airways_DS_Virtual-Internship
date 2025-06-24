# British Airways DS Virtual Internship Programme

![British Airways](https://user-images.githubusercontent.com/68168071/208015626-505dc939-4551-4ccc-a60e-18827d60bf66.png)

**Data Science Virtual Experience Programme by British Airways (via Forage Australia)**  
*By Rahul Kumar*

---

## Table of Contents

- [Project Overview](#project-overview)
- [Motivation](#motivation)
- [Data Sources](#data-sources)
- [Directory Structure](#directory-structure)
- [Task 1: Web Scraping and Sentiment Analysis](#task-1-web-scraping-and-sentiment-analysis)
- [Task 2: Predicting Customer Buying Behaviour](#task-2-predicting-customer-buying-behaviour)
- [Results & Insights](#results--insights)
- [References](#references)
- [Contact](#contact)

---

## Project Overview

This project was completed as part of the British Airways Data Science Virtual Experience Programme (Forage Australia). The goal was to gain business insights and understand factors influencing customer buying behaviour using British Airways reviews and customer booking datasets. The project involved:

- Web scraping and sentiment analysis of customer reviews,
- Exploratory data analysis (EDA),
- Feature engineering and selection,
- Predictive modeling (Random Forest, XGBoost, CatBoost),
- Model interpretation and business recommendations.

---

## Motivation

Understanding customer sentiment and the drivers of booking completion is crucial for airlines to improve services, target marketing, and optimize customer experience. This project leverages real-world data and advanced analytics to uncover actionable insights for British Airways.

---

## Data Sources

- **British Airways Reviews Dataset:**  
  [Skytrax Reviews](https://www.airlinequality.com/airline-reviews/british-airways)  
  (Web scraped using Python and BeautifulSoup)

- **Customer Booking Dataset:**  
  Provided as `customer_booking.csv` (50,000 records, 14 features)

---

## Directory Structure
```
British-Airways-DS-Virtual-Internship/
│
├── data/                    # Raw and processed datasets
│ ├── BA_reviews.csv
│ └── customer_booking.csv
├── notebooks/               # Jupyter notebooks for EDA, modeling, and analysis
├── src/                     # Source code for scraping, sentiment analysis, modeling
├── results/                 # Visualizations, model outputs, and presentations
├── requirements.txt         # Python dependencies
├── README.md                # Project documentation
└── LICENSE
```
---

## Task 1: Web Scraping and Sentiment Analysis

- **Web Scraping:**  
  - Used Python and BeautifulSoup to collect 2,000+ customer reviews from [Skytrax](https://www.airlinequality.com/airline-reviews/british-airways).
  - Saved reviews to `BA_reviews.csv`.

- **Data Cleaning & Preprocessing:**  
  - Removed verification tags, converted text to lowercase, removed punctuation and stopwords, and tokenized reviews.

- **Sentiment Analysis:**  
  - Used NLTK and TextBlob to calculate polarity scores and tag each review as Positive, Negative, or Neutral.
  - Visualized sentiment distribution and generated word clouds for each sentiment category.

- **Key Tools:**  
  `BeautifulSoup`, `NLTK`, `TextBlob`, `WordCloud`, `matplotlib`, `pandas`

---

## Task 2: Predicting Customer Buying Behaviour

- **EDA & Data Cleaning:**  
  - Explored and cleaned the `customer_booking.csv` dataset (50,000 records, 14 features).
  - Analyzed missing values, feature distributions, and categorical variables.

- **Feature Engineering & Selection:**  
  - Used Random Forest and Ridge (L2) regularization to identify key predictors of booking completion.

- **Model Building:**  
  - Built and compared three models: Random Forest, XGBoost, and CatBoost.
  - Evaluated models using Accuracy, Recall, F1-Score, and ROC-AUC.
  - Performed hyperparameter tuning with GridSearchCV.

- **Model Interpretation:**  
  - Analyzed feature importances and model coefficients.
  - Presented findings in business-focused presentations.

- **Key Tools:**  
  `pandas`, `scikit-learn`, `xgboost`, `catboost`, `matplotlib`, `seaborn`, `GridSearchCV`

---

## Results & Insights

- **Sentiment Analysis:**  
  - ~68% of reviews were positive, ~31% negative, <1% neutral.
  - Key positive themes: friendly staff, smooth boarding, good in-flight service.
  - Negative themes: delays, cancellations, poor customer service.

- **Customer Booking Analysis:**  
  - Majority of bookings made via Internet (88.8%), rest via Mobile.
  - Most common trip type: RoundTrip (99%).
  - Top features influencing booking completion: `booking_origin`, `purchase_lead`, `length_of_stay`, `route`, `flight_duration`.
  - Only ~15% of all bookings were successfully completed.

- **Predictive Modeling:**  
  - Random Forest, XGBoost, and CatBoost models achieved accuracies in the range of 83–85%.
  - Feature selection and hyperparameter tuning improved model performance.
  - All models showed class imbalance: most bookings were not completed.

- **Business Recommendations:**  
  - Focus on improving customer experience for key routes and origins.
  - Target marketing strategies toward segments with high booking completion rates.
  - Address negative sentiment themes to reduce booking abandonment.

---

## References

1. [British Airways Reviews (Skytrax)](https://www.airlinequality.com/airline-reviews/british-airways)
2. [Forage Australia - British Airways Data Science Virtual Experience](https://www.theforage.com/virtual-internships/prototype/5b6WqTgqP4L8q7e6w)
3. [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
4. [NLTK Documentation](https://www.nltk.org/)
5. [Scikit-learn Documentation](https://scikit-learn.org/)
6. [XGBoost Documentation](https://xgboost.readthedocs.io/)
7. [CatBoost Documentation](https://catboost.ai/)

---

## Contact

**Author:** Rahul Kumar  
**Email:** kumar.rahul226@gmail.com  
**LinkedIn:** [rk95-dataquasar](https://www.linkedin.com/in/rk95-dataquasar/)

---
