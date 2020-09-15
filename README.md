# KNN Classifier Model

### Objective

A project to build a KNN classifier to find whether a patient would have diabetes or not.

### Feature and the target varaible

X- The feature variables :
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

y - Target variable
- Outcome

### Determining n_neighbours 

- From a range of 1 to 9 , the n_neighbors are selected passing them through a for loop to test each case and then the training accuracy and testing accuracy graph is plotted along with Number of neighbors with respective to accuracy. Vizualising the graph neighbor havingb the value 4 has a greater testing accuracy and when fitted to the model it gives 72.7% accuracy.

- Another method to determine n_neighbors is to tune the hyper parameters to choose the best best value. Grid search cv method is also used here to determine the best value for neighbor from the range of 1 to 50 . The best score with n_neighbors = 14 gives 75.78% accuracy.

### Accuracy prediction
- Classification report 
- Confusion matrix : True positive = 86     True negative = 14
                     False positive = 31    False negative = 23

### Plotting the ROC Curve
- Plotting the true positive rates with respective to false positive rates for different possible cut points of a diagonstic point 
- Finding the area under ROC curve and thus predicting the score which is equal to 74.6%

### Passing a new data to predict whether a patient has diabetes or not

 Two new data's were passed for prediction and the model predicted that patient 1 has no diabetes and patient 2 has diabetes .

