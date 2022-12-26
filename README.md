# Natural Language Processing with Reviews from International Hotel brands in Europe

## INTRODUCTION
Natural language processing (NLP) is a subfield of linguistics, artificial intelligence, and machine learning concerned with the interaction between computers and human languages. In the context of hotel reviews on Booking.com, NLP techniques can be used to extract valuable insights and information from the large volume of guest reviews written in various natural languages. 

NLP techniques can be used to automatically classify reviews as positive, negative, or neutral, or to extract specific topics or themes mentioned in the reviews. This can be useful for hotel owners and managers to understand what guests like or dislike about their property, and to identify areas for improvement. NLP can also be used to translate reviews written in different languages, making it easier for hotels to analyze and understand feedback from a diverse group of guests. Overall, NLP can help hotels make more informed decisions based on the insights and information extracted from guest reviews.

The data was provided from https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe

## Pre-proccessing
K-means Clustering is an unsupervised machine-learning (ML) model that groups cryptocurrencies based on the similarity of their price-volume movement. The model recommended 5 clusters which are found at the elbow in the Inertia plot and the highest of the Silhouette Score. Based on the model and domain knowledge, the following clusters are below (Plot attached below for reference):

### Dataset features

The csv file contains 17 columns and 515,738 rows. The description of each columns is below:

* Hotel_Address: Address of hotel.
* AdditionalNumberof_Scoring: There are also some guests who just made a scoring on the service rather than a review. This number indicates how many valid scores 
* Review_Date: Date when reviewer posted the corresponding review.
* Average_Score: Average Score of the hotel, calculated based on the latest comment in the last year.
* Hotel_Name: Name of Hotel
* Reviewer_Nationality: Nationality of Reviewer
* Negative_Review: Negative Review the reviewer gave to the hotel. If the reviewer does not give the negative review, then it should be: 'No Negative'
* ReviewTotalNegativeWordCounts: Total number of words in the negative review.
* Positive_Review: Positive Review the reviewer gave to the hotel. If the reviewer does not give the negative review, then it should be: 'No Positive'
* ReviewTotalPositiveWordCounts: Total number of words in the positive review.
* Reviewer_Score: Score the reviewer has given to the hotel, based on his/her experience
* TotalNumberofReviewsReviewerHasGiven: Number of Reviews the reviewers has given in the past.
* TotalNumberof_Reviews: Total number of valid reviews the hotel has.
* Tags: Tags reviewer gave the hotel.
* dayssincereview: Duration between the review date and scrape date.
* without review in there.
* lat: Latitude of the hotel
* lng: longtitude of the hotel


![](assets/CLUSTERING%20-%20Map.png)



## Conclusion


# Citation
Use this bibtex to cite this repository:

```
@misc{thai22011_NLP_Hotel_Review_2022,
  title={Natural Language Processing with Reviews from International Hotel brands in Europe},
  author={Thai Nguyen},
  year={2022},
  publisher={Github},
  journal={GitHub repository},
  howpublished={\url{https://github.com/thai22011/NLP_Hotel_Review}},
}
```

# Contributing

No contribution is required.       

# Requirements

`geopy` isnt available in conda so needs to create the `nlp_env` first then `pip install geopy` inside the environment

```
conda create -n nlp_env python=3.8 numpy pandas matplotlib seaborn statsmodels scikit-learn==0.24.1 jupyter jupyterlab nltk geopandas plotly

conda activate nlp_env

pip install geopy
```
