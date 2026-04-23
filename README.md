# NLP_RestaurantReviews

This project utilizes natural language processing to identify restuarant customer reviews as either positive or negative reviews.

**Objective**
- Build automated system that can classify resturant reviews as positive or negative to help restaurant owners quickly understand customer sentiment.

**Technology Used**
- Python 3
- Libraries: pandas, numpy, scikit-learn, matplotlib, torch, transformers

**Dataset**
- TSV formatted file containing two attributes and 1000 records


# Repository Structure
```
NLP-RestaurantReviews/
│-- data/
│-- documentation/
│-- results/
│-- README.md
│-- RestaurantReview_NLP.ipynb
│-- requirements.txt
```

# Installation 
1. Clone repository
```
git clone https://github.com/Rymerpop03/NLP_RestaurantReviews.git
cd NLP_RestaurantReviews
```
2. Install Required Packages
```
pip install -r requirements.txt
```
3. Making predictions
```
from src.predict import predict_sentiment

# Predict sentiment for new reviews
review = "The food was amazing and service was excellent!"
sentiment = predict_sentiment(review, model, vectorizer)
print(f"Sentiment: {'Positive' if sentiment == 1 else 'Negative'}")
```
