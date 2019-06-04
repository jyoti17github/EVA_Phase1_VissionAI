## Assignmnet 5 

Change the code 8 or your own 4th Code from Assignment 4 to include:
1. Image normalization
2. L2 regularization
3. ReLU after BN
Run your new code for 40 epochs and save the model with highest validation accuracy
Find out 25 misclassified images from the validation dataset and create an image gallery
Submit

### Used my own network of Assignmnet 4 ( 8372 parameters with 9948 accuracy)

### key observations 
### Image Normalization 
     Validation accuracy achieved 0.9939 over 40 epochs but without this it was 0.9949 on running same no of epochs.Speculation is around number of parameters as code 8 has 16k parameters but network used had 8k approx parameters.Observation - accuracy decreased  by less than 1 percent.
### L2 regulrization , val accuracy 9937 over 40 epochs
 nothing much observe on val accuracy  side just drop or near same val accuracy resulted after adding per layers l2 regularization 
 But overfitting was improved while training model.Observation - accuracy decreased  by 0.02 percent.
 
### Relu before BN and generated missclassifield images. 
It made network to drop val accuracy by 2.4 percent.Seems now network will discard the negative values and not passing all info for batch normalization.Observation - accuracy decreased  by 2.4 percent from original model.

On this model Images which are miss classified can be seen.
