# Mid_Price_Prediction
## Description
In this project, our goal is to predict the best mid price based on the best bid/ask volume and the bid/ask depth for a point in time. 
When starting this project, I noticed the files provided were very large and in .gz format. Thus, I used gzip, wget, and dask to open and store these files in a dask dataframe with 1 partion per dataframe. I would then concatenate the dataframes, creating a dask dataframe with 9 partitions. 
After visualing the data and organizing/preparing the data for machine learning, I created a local dask cluster to train my models in parallel. Although the models I used were relatively simple, if I were to use deep learning, training in parallel would almost be necessary.
I trained my model on both a Decision Tree and a Linear Regression. Testing my model on 2021-02-10T00:02:28.02819	yieled a prediction of 36148. The correct value for that time is 46997.119999999995.

#### View file and results here: https://github.com/jovuribe/Mid_Price_Prediction/blob/08ce0274df30f3c4a6716b26a207e5ea1346cb00/Mid-Price%20Prediction.ipynb
