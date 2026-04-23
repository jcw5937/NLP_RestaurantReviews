# NLP_RestaurantReviews

This project utilizes natural language processing to identify restuarant customer reviews as either positive or negative reviews.

**Note for AI 100 Final Project Submission**

This repo contains our work and outputs as well as the final deliverables. The final deliverables specifically are as follows:

1. A Google Sheet or Microsoft Excel:  AI-100_Final.xlsx
2. A PDF report:                       AI100-Final-Report.pdf
3. Files for code:                     RestaurantReview_NLP.ipynb
                                       (Data and outputs are also provided in respective folders)

Additionally, I created a Bug Reflection Evaluator to help consolidate the steps of the final project before putting it in the spreadsheet. I will include that as well.

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
