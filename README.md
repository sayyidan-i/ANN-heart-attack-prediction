# Heart Disease Prediction using Neural Network

## Overview
This Jupyter Notebook demonstrates the process of predicting heart disease using a neural network. The dataset used in this project is the "heart.csv" dataset.

## Dataset
The dataset is loaded from the file "/content/drive/MyDrive/BAI/heart disease dataset/heart.csv" using the pandas library. The first few rows of the dataset are displayed using `df.head()`.

## Data Preprocessing
### Categorical Variable Encoding
Categorical variables such as 'Sex', 'ChestPainType', 'RestingECG', 'ExerciseAngina', and 'ST_Slope' are one-hot encoded using the `pd.get_dummies` function.

### Feature Scaling
Numeric features including 'Age', 'RestingBP', 'MaxHR', and 'Cholesterol' are scaled to a range between 0 and 1 using Min-Max scaling.

## Data Splitting
The dataset is split into training and validation sets using the `train_test_split` function from scikit-learn. The proportions of samples in the training and validation sets are displayed.

## Neural Network Model
A neural network model is created using the Keras library. The model architecture includes multiple dense layers with dropout regularization. The model is compiled with the Adam optimizer, binary crossentropy loss, and accuracy metric.

## Training
The model is trained on the training set for 20 epochs with a batch size of 32. Training and validation metrics (accuracy) are recorded in the `hist` variable.

## Instructions to Run
1. Ensure you have the required libraries installed: pandas, scikit-learn, tensorflow, and keras.
2. Load the notebook in a Jupyter environment.
3. Run each cell sequentially to execute the code and observe the output.

## Note
This is a simplified overview, and you may need to adjust parameters, experiment with different architectures, and optimize the model for your specific requirements.

Feel free to reach out for any questions or improvements!
