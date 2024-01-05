# Predicting-Visitor-Purchases-with-BigQuery-ML

This project was done under a Google Cloud Course.

In this project, I have harnessed the power of Google Cloud's BigQuery, a fully-managed, serverless data warehouse that enables lightning-fast SQL queries using the processing power of Google's infrastructure. The primary objective of this project is to predict the likelihood of a visitor making a purchase during a subsequent visit to the Google Merchandise Store website - https://shop.googlemerchandisestore.com/

The first critical step involves gathering and processing the relevant data. BigQuery, with its scalability and flexibility, proves instrumental in handling large datasets efficiently. The platform allows seamless integration with various data sources, ensuring that diverse and comprehensive information about user interactions, preferences, and historical behavior is captured.

# DATA

The dataset can  be found at- https://www.blog.google/products/marketingplatform/analytics/introducing-google-analytics-sample

The dataset definitons can be found at- https://support.google.com/analytics/answer/3437719?hl=en

Once the data is ingested into BigQuery, the focus shifts to preparing it for analysis. Through structured SQL queries, I've crafted a dataset that serves as the foundation for training a Logistic Machine Learning model. This model, designed to predict binary outcomes (purchase or no purchase), is trained on historical data, learning patterns and relationships within the dataset.

The logistic regression model, a popular choice for binary classification tasks, is chosen for its simplicity and interpretability. Its ability to provide probability scores aids in fine-tuning the prediction threshold, ensuring a balanced approach based on the project's specific requirements.

Google Cloud's ML Engine facilitates the deployment and management of the trained model, allowing seamless integration with the existing infrastructure. The model is then put to the test using real-time or batch predictions, depending on the project's needs. This predictive capability opens avenues for targeted marketing strategies, personalized user experiences, and optimized conversion rates.

The insights derived from this predictive analysis can empower the website's decision-makers to tailor their approach, allocating resources more effectively. Whether it's optimizing the user interface, refining marketing campaigns, or tailoring promotions, the predictive model provides a valuable tool for enhancing the overall user experience and maximizing revenue potential.

In essence, this project represents a synergy between Google Cloud's BigQuery and Logistic Machine Learning, offering a robust framework for predicting user behavior and driving informed decision-making within the context of e-commerce or any online platform.
