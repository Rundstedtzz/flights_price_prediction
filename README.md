# Expedia Flights Price Prediction

## Google Cloud Set-up
We have run most of our models and feature engineering on Google Cloud, so please create a Storage Bucket and create a Dataproc Cluster with the most basic setup will be fine to run our code.

## Data
Here is the link to the data: https://drive.google.com/drive/folders/1FfiXmYoKsALp3t3KFBPv7bHqpqYP0p5v?usp=sharing. Upload the files needed to the storage bucket
For testing the code, you can use the smallest data and all the following .py files have already set to run this csv: itineraries_sample_small.csv

## Step 1: feature.py
Submit the file via jobs (You can change the file and output path on line 66-67)

## Step 2: Models
Submit the file via jobs (You can change the file and output path on line 14):
- linear_regression.py
- decision_tree.py
- random_forest.py
- GBT.py
- xgboost.py
- NN.py

## Step 3: Outputs
The outputs can be viewed in the 'gs://final_project_flights/notebooks/jupyter/output/' folder.

## Step 4: Jupyter notebooks
- You can also run the jupyter notebook to see the results (milestone4_models.ipynb). 
- The XGBoost is run on Azure (milestone4_XGBoost.ipynb).
- We have also explored more on MCAR, MNAR, or MAR, predicting conditioned on ‘totalTravelDistance’ to see if within a certain ‘totalTravelDistance’ bin like flights >x # miles for example, how successful you would be in predicting the cheaper and more expensive flights within that given how important ‘totalTravelDistance’ was to RF prediction (milestone4_other.ipynb). 



