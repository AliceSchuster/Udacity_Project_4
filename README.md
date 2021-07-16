# Udacity_Project_1


## Motivation

The following project has been created as part of the [Udacity Data Science Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025).

Using the Starbucks dataset, this project aims to build and evaluate different models that predict whether or not a customer will respond to an offer (binary classification). Moreover, the project provides an understanding of main features that have an influence on the success of an offer.

## Data

The following three datasets are provided by Starbucks and Udacity:

    portfolio.json: Offers sent during 30-day test period (10 offers)
        id (string): offer id
        offer_type (string): bogo, discount, informational
        difficulty (integer): money required to be spent to receive reward
        reward (integer): money awarded for completing an offer       
        duration (integer): time for offer to be open, in days
        channels (list of strings): web, email, mobile, social
        

    profile.json: Rewards program users (17000 users)
        age (integer) missing value encoded as 118
        became_member_on (integer): date when customer created an app account - format YYYYMMDD
        gender (string): gender of customer - M, F, O (other)       
        id (string): customer id        
        income (float): income of customer


    transcript.json: Event log (306534 events)
        event (string): offer received, offer viewed, transaction, offer completed
        person (string): customer id
        time (integer): hours after start of test (start: t=0)
        value (dictionary of strings):  different values (offer id or transaction amount) depending on event type
        
        
  ## Installation

For this project, I've have used Python 3.6.3 and the following Python libraries:

- seaborn==0.8.1
- pandas==0.23.3
- numpy==1.12.1
- matplotlib==2.1.0
- json5==0.8.5
- scikit-learn==0.19.1

## Results

Please find more information on this project in [my medium post] (https://medium.com/p/529fce2a9996/).

In order to predict whether an offer would be successful, I balanced the two groups and used Logistic Regression, Random Forrest Classifier, and AdaBoost Classifier for classification.

In this use case, our goal is to reduce the number of false negatives and increase the number of true positives. The reason for this is, that customers who took an offer spent twice as money as customers who do not take an offer. As sending an offer via app is not expensive for Starbucks, the number of true negatives is not of high relevance in our case.

The best model was Random Forrest with a recall 73% and a f2-Score 73,3%.