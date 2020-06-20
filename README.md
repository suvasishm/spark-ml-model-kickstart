# Spark ML Model Kickstart



#### Initial Setup

1. [PySpark In Jupyter](https://github.com/suvasishm/pyspark-in-jupyter)
2. Install NumPy: `$ pip3 install numpy`


##### !! Exception: Java gateway process exited before sending its port number !!
If the above error occurs make sure $JAVA_HOME is either set globally or [for the project](https://github.com/suvasishm/pyspark-in-jupyter/#note-jupyter-might-fail-to-work-on-a-system-with-java-18-i-had-java-1130-and-i-was-getting-error-exception-java-gateway-process-exited-before-sending-its-port-number-multiple-jdks-can-be-managed-the-following-way).

### What I did here

#### titanic_survival_model
Build a model to predict survival on the Titanic based on the training data (`data/training.csv`) only. A subset of traning data are used to train the model and remaing data are used as test data.

The notebook contains steps:
1. Load the training data
1. Prepare the dataset for Spark ML library
1. Split the dataset into training_data and test_data
1. Build the model and fit the training dataset into the model
1. Use the test dataset against the model to get the predictions
1. Finally calculate accuracy of the predictions

#### titanic_kaggle_prediction
This is similar to the above model. Only difference is here two seperate datasets are used - training data (`data/training.csv`) to train the model. Then using that model to predict survival of the passengers in the test data (`data/test.csv`).

The notebook contains steps:
1. Load the training & test data
1. Prepare both the datasets for Spark ML library
1. Build the model and fit the training dataset into the model
1. Use the test dataset against the model to get the predictions

Ref: 
1. https://www.kaggle.com/c/titanic/overview
2. https://towardsdatascience.com/your-first-apache-spark-ml-model-d2bb82b599dd

