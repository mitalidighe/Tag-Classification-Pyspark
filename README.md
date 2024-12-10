# Tag-Classification-Pyspark


**Built a Tag Recommendation System for the top 50 tags to tag Stack Overflow posts**

*Feature Engineering*
Extracted Top 50 tags based on their frequency in the dataset
Processed tokens by tokenizing text, removing stop words, and applying TF-IDF to generate features

*Model Development*
Trained 50 logistic regression models, one for each tag, using SparkML
Models predict whether a tag applies to a post based on the TF-IDF scores

*Model Storage*
Saved the trained models to Google Cloud Storage for efficient access during inference

*Inference*
Loaded models to predict tags from sample data
Combined the predictions to form a list of recommended tags for each post


**Data Source**
https://console.cloud.google.com/bigquery?ws=!1m4!1m3!3m2!1sbigquery-public-data!2sstackoverflow
