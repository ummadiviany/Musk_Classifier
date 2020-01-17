# Musk_Classifier
 This repository is created for submitting solutions to prelimenary task for  joining credicxo team.

##

### Data Pre-Processing:

1)Removed "conformation_name" column due to large number of unique values.
2)Converted "molecule_name" Categorical values to numerical encodings.
3)Removed "ID" column due to large number of unique values.
4)assigned target column vaiable to y
5)assigned feature columns to X
6)Used StandardScaler on X.It Standardize features by removing the mean and scaling to unit varianceThe standard score of a sample x is calculated as: z = (x - u) / s


### Train Test Split(80:20) :

used sklearn "train_test_split" to split it into X_train, X_test, y_train, y_test

### Kears Model:

Used Keras Sequential API to create a model.
Created with 3-dense hidden layer with 150,100,50 neurons respectively.
Used Sigmoid activation function for output layer.
#### Model Summary

Layer (type)      |          Output Shape   |           Param 

dense_5 (Dense)              (None, 150)               25200

dense_6 (Dense)              (None, 100)               15100

dense_7 (Dense)              (None, 50)                5050

dense_8 (Dense)              (None, 1)                 51

Total params: 45,401
Trainable params: 45,401
Non-trainable params: 0

### Results-Visualization:

#### Test loss: 0.0007406226365040339
#### Test accuracy: 1.0

#### Confusion_matrix
[[1116    0]
 [   0  204]]

#### Classification_report


              precision  |  recall | f1-score |  support

           0       1.00      1.00      1.00      1116
           1       1.00      1.00      1.00       204

    accuracy                           1.00      1320
   macro avg       1.00      1.00      1.00      1320
weighted avg       1.00      1.00      1.00      1320

####Train-Test Accuracy Graph:
![Train-Test Accuracy Graph](https://github.com/ummadiviany/Musk_Classifier/blob/master/acc.png)

####Train-Test Loss Graph:
![Train-Test Loss Graph](https://github.com/ummadiviany/Musk_Classifier/blob/master/loss.png)


