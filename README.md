# ANN Car Price Prediction

Artificial Neural Network (ANN) with Tensorflow to estimate the correct selling price to customers based on multiple variables:
- Name
- Email
- Country
- Gender
- Age
- Annual Salary
- Credit Card Debt (Could be Credit Score)
- Net Worth

## Highlights
- Keras and Tensorflow used to predict
- Sequential Model Used:
```
Model: "sequential_1"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
dense_1 (Dense)              (None, 5)                 30        
_________________________________________________________________
batch_normalization_1 (Batch (None, 5)                 20        
_________________________________________________________________
dense_2 (Dense)              (None, 15)                90        
_________________________________________________________________
dense_3 (Dense)              (None, 1)                 16        
=================================================================
Total params: 156
Trainable params: 146
Non-trainable params: 10
_________________________________________________________________
```
- Results: 
```
Model Evaluation 
--- Train MSE: 0.003
--- Test MSE: 0.003

Gender = 1 # Male
Age = 50
Annual_Salary = 50000
Credit_Card_Debt = 10000
Net_Worth = 600000

Suggested Price for Customer  [[45407.695]]
```

## Potential Improvements
- Use Country as a variable (Transforming categorical to be used in ANN is needed)

## Demo Images

### Variable Pair-Plot to "Car Purchase Amount"
![image](https://user-images.githubusercontent.com/87340855/219026703-511cebc9-c3d3-4e83-a996-f1727dd24165.png)

### Train and Validation Loss Plots
![image](https://user-images.githubusercontent.com/87340855/219026810-24104371-1eb9-4241-95f7-3284e3d4ca4e.png)

