# PREDICTING VISITOR PURCHASES WITH BIGQUERY ML

This project was done under a Google Cloud Course.

In this project, I have harnessed the power of Google Cloud's BigQuery, a fully-managed, serverless data warehouse that enables lightning-fast SQL queries using the processing power of Google's infrastructure. The primary objective of this project is to predict the likelihood of a visitor making a purchase during a subsequent visit to the Google Merchandise Store website - https://shop.googlemerchandisestore.com/

The first critical step involves gathering and processing the relevant data. BigQuery, with its scalability and flexibility, proves instrumental in handling large datasets efficiently. The platform allows seamless integration with various data sources, ensuring that diverse and comprehensive information about user interactions, preferences, and historical behavior is captured.

# DATA

The dataset can  be found at- https://www.blog.google/products/marketingplatform/analytics/introducing-google-analytics-sample

The dataset definitons can be found at- https://support.google.com/analytics/answer/3437719?hl=en

Data Dimensions- 970,532 rows

# BUILDING AND EVALUATING ML MODEL 

Once the data is ingested into BigQuery, the focus shifts to preparing it for analysis. Through structured SQL queries, I've crafted a dataset that serves as the foundation for training a **Logistic Machine Learning model.** This model, designed to predict binary outcomes (purchase or no purchase), is trained on historical data, learning patterns and relationships within the dataset.

The **logistic regression model**, a popular choice for binary classification tasks, is chosen for its simplicity and interpretability. Its ability to provide probability scores aids in fine-tuning the prediction threshold, ensuring a balanced approach based on the project's specific requirements.

For classification problems in ML, we need to minimize the False Positive Rate (predict that the user will return and purchase and they don't) and maximize the True Positive Rate (predict that the user will return and purchase and they do).

This relationship is visualized with a ROC (Receiver Operating Characteristic) curve , where we try to maximize the area under the curve or AUC:

![GNW5Bw+8bviep9OK201QGPzaAEnKKyoIkDChUHeVdFw=](https://github.com/Sniperex/Predicting-Visitor-Purchases-with-BigQuery-ML/assets/52499633/55a7a4cb-e71c-44d8-b689-7b0c3e6d7a0f)

# PREDICTION AND ANALYSIS

- Of the top 6% of first-time visitors (sorted in decreasing order of predicted probability), more than 6% make a purchase in a later visit.
- These users represent nearly 50% of all first-time visitors who make a purchase in a later visit.
- Overall, only 0.7% of first-time visitors make a purchase in a later visit.
- Targeting the top 6% of first-time increases marketing ROI by 9x vs targeting them all.


The insights derived from this predictive analysis can empower the website's decision-makers to tailor their approach, allocating resources more effectively. Whether it's optimizing the user interface, refining marketing campaigns, or tailoring promotions, the predictive model provides a valuable tool for enhancing the overall user experience and maximizing revenue potential.

