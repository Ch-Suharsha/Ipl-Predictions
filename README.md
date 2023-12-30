# Ipl-Predictions

**Project Overview: IPL Score Prediction**

**Objective:**
The project aims to predict the total score in an Indian Premier League (IPL) cricket match based on various features, including venue, batting team, bowling team, striker, and bowler. The prediction is made using a neural network regression model trained on historical IPL match data.

**Key Steps in the Project:**

1. **Data Preparation:**
   - Loading the dataset containing IPL match data.
   - Dropping unnecessary features like date, runs, wickets, overs, runs_last_5, wickets_last_5, mid, striker, and non-striker.
   - Separating features (X) and the target variable (total runs).

2. **Label Encoding:**
   - Applying label encoding to categorical features (venue, batting team, bowling team, striker, and bowler).
   - Using sklearn's LabelEncoder for each categorical feature.

3. **Train-Test Split:**
   - Splitting the dataset into training and testing sets.

4. **Feature Scaling:**
   - Scaling the numerical features using Min-Max scaling to bring them into a common range.

5. **Neural Network Model:**
   - Defining a neural network model using Keras with three layers (input, hidden, and output).
   - Using Huber loss as the loss function for regression.

6. **Model Training:**
   - Training the neural network model on the training set for 50 epochs.
   - Monitoring and visualizing the training and validation losses.

7. **Model Evaluation:**
   - Making predictions on the test set.
   - Evaluating the model's performance using mean absolute error.

8. **Interactive Prediction Widget:**
   - Creating an interactive widget using ipywidgets for users to input match details (venue, batting team, bowling team, striker, bowler).
   - Using the trained model to predict the total score based on user inputs.
   - Displaying the predicted score.

**Outcome:**
The project provides a tool for cricket enthusiasts to get an estimate of the total score in an IPL match based on historical data and machine learning. The neural network model learns patterns and relationships from past matches to make predictions, enhancing the excitement and engagement of cricket fans. The interactive widget adds a user-friendly aspect, making it accessible to a broader audience.
