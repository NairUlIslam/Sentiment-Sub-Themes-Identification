# Sentiment-Sub-Themes-Identification
Subtheme Sentiment Analysis Task
Subtheme Sentiment Analysis Task
Take the following example:
“One tyre went missing, so there was a delay to get the two tyres fitted. The way garage dealt
with it was fantastic.”
In this review there are numerous insights, insights we call “subtheme sentiments”. A Subtheme
sentiment is generally a sentiment towards an aspect or a problem.
If we look at the subtheme sentiments of the above review we will get a clearer sense what these
generally are.
incorrect tyres sent negative garage service positive wait time negative
The main difference between these subthemes is that Garage Service and Wait Time are aspects
of the service that can be positive or negative while
Incorrect Tyres Sent denotes a problem, something inherently negative.
Task
The task is to develop an approach that given a sample will identify the subthemes along with
their respective sentiments

Approach:

1. Use, the top 5 Insights from each kind of sentiment (posotive or negative). Positive sentiments are in majority, but we want the model to identify every kind of sentiment.
2. Use BERT model, and teach the model to identify the insights and associated sentiments.
3. 20% of the data is held-out for testing, and 10% data from the training set is used for model validation as it is being trained.
4. Strarified spilitting was employed to ensure proper distribution.
5. After successful training, test the performance of the model on the held out set.
6. Generate a CSV file that contains where we match the actual insights and sentiments with those of the predicted insights and associated sentiments.

Performance on the held-out set:

+-----------+---------------+
| Metric    | Value in %age |
+-----------+---------------+
| accuracy  | 97.38         |
| f1        | 97.38         |
| precision | 97.38         |
| recall    | 97.38         |
+-----------+---------------+

    
