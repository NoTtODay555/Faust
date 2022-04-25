# Faust



The main frameworks that we will use are:

 - Faust: stream processing library, using the async/away paradigm and requires python 3.6+
 - Kafka: we will use the confluent version for kafka as our streaming platform
 - MLFlow: an open-source platform used to monitor and save machine learning models after training
 - Jupyter lab: 
 - docker-compose : 
 - Miniconda3 : 

download : data (creditcard.csv)  
with https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud


RUN Jupyter Notebook :
 - fraud_detection_training.ipynb(For create Model)
 - message_sender.ipynb(For send Data To Kafka)

Run Server With MLFlow
mlflow models serve -m <Model Filename> --host 0.0.0.0 --port 5010


Run Server With Fraud
faust -A <FileFraud Python> worker -l info