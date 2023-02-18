# Vehicle-Insurance
If a customer has life insurance will he be interested in vehicle insurance? What are chances?


To predict whether a Health Insurance owner is interested in vehicle insurance, we can build a binary classification model using deep learning. Here are the steps to build the model:

Data Preprocessing: We will start by loading the train and test datasets and do some basic preprocessing. The steps include:

  Drop the 'id' column as it is not useful for our analysis.
  
  Convert categorical variables ('Gender', 'Vehicle_Age', 'Vehicle_Damage') into numeric form.
  
  Scale the numerical variables ('Age', 'Region_Code', 'Annual_Premium', 'Policy_Sales_Channel', 'Vintage') to have zero mean and unit variance.
  
  Model Building: We will build a deep learning model using Keras API in TensorFlow. The model will have 7 layers:
  
  Input layer: Input layer will have 11 neurons (one for each input feature).
  
  Hidden Layers: We will add 5 hidden layers with 128 neurons each. Each layer will use ReLU activation function and dropout regularization to prevent overfitting.
  
  Output layer: Output layer will have 1 neuron with sigmoid activation function as we are doing binary classification.
  
  Model Training and Evaluation: We will train the model on the preprocessed train data and evaluate its performance on the test data. We will use binary cross-entropy   as the loss function, Adam optimizer, and accuracy as the evaluation metric.
  
  Results and Visualization: Finally, we will visualize the results using a confusion matrix and a ROC curve.
