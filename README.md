# Hit_Song_Science
This project creates a custom dataset using the Spotify API and Billboard Hot 100 Data, ultimately creating a random forest that achieved 97% precision.

The first file (Hit_Prediction_Data_Creation) uses the Spotify API to retrieve 500,000+ songs and their associated acoustic features. I then joined this dataset to a dataset of Billboard Hot 100 annual lists. Songs that appeared on a Billboard Hot100 list were labeled as 'hits,' and songs not found on the Billboard Hot100 were labeled as 'non-hits.' The dataset ended up with 500,000+ non-hits and 2,700+ hits.

The second file contains EDA, data preprocessing, and model creation. I created several visualizations to explore the data, including correlation heat maps for both hits and non-hits and scatterplots showing the relationship between features color-coded by whether or not the instance was a hit. To compensate for the wildly unbalanced dataset, I used Synthetic Minority Oversampling Technique (SMOTE).

I created several models. The best performing was a Random Forest. I created random forests using both Scikit-Learn and TensorFlow's RandomForest estimator. 
