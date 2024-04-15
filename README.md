# Build and Run a Docker Container for your Machine Learning Model  


I am reproducing this from a github. I am rebuilding a simple machine learning model in a docker container and running it. The following files will be in it.


- Dockerfile
- train.py 
- inference.py 

The train.py is  a python script that ingest and normalize EEG data in a csv file (train.csv) and train two models to classify the data (using scikit-learn). The script saves two models: Linear Discriminant Analysis (clf_lda) and Neural Networks multi-layer perceptron (clf_NN). 

The inference.py will be called to perform batch inference by loading the two models that has been previously created. The application will normalize new EEG data coming from a csv file (test.csv), perform inference on the dataset and print the classification accuracy and predictions. 