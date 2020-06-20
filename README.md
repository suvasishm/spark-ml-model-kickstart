# Spark ML Model Kickstart



#### Initial Setup

1. [PySpark In Jupyter](https://github.com/suvasishm/pyspark-in-jupyter)
2. Install NumPy: `$ pip3 install numpy`


##### !! Exception: Java gateway process exited before sending its port number !!
If the above error occurs make sure $JAVA_HOME is either set globally or [for the project](https://github.com/suvasishm/pyspark-in-jupyter/#note-jupyter-might-fail-to-work-on-a-system-with-java-18-i-had-java-1130-and-i-was-getting-error-exception-java-gateway-process-exited-before-sending-its-port-number-multiple-jdks-can-be-managed-the-following-way).

#### What I did here

In this learning process, I am trying to predict survival on the Titanic as described in the below Ref #1.

The notebook contains steps:
1. load the training data
1. prepare the data for Spark ML library
1. build the model and fit the training dataset into the model
1. use the test dataset against the model to get the predictions
1. finally calculate accuracy of the predictions

Ref: 
1. https://www.kaggle.com/c/titanic/overview
2. https://towardsdatascience.com/your-first-apache-spark-ml-model-d2bb82b599dd

