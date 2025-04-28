📱 Mobile Price Predictor
This project is a machine learning-based application designed to predict the price range of mobile phones based on their specifications. It uses a Voting Classifier model, which is an ensemble method that combines multiple individual machine learning models to produce a more accurate and reliable prediction.

Table of Contents
Project Overview

Technologies Used

Model Training

Features and Inputs

How to Run the Application

Examples

License

Project Overview
The Mobile Price Predictor application predicts the price range of a mobile phone based on various specifications such as battery power, camera, RAM, processor cores, and more. The project uses a Voting Classifier, which is a machine learning technique that combines predictions from multiple models to provide a final output. This ensures the predictions are more robust and accurate.

The app allows users to input their mobile phone specifications, and based on that input, the app provides a prediction on whether the mobile phone falls into a Low, Medium, High, or Very High price range.

Objective
Predict the price range of a mobile phone (Low, Medium, High, Very High) based on its specifications.

Use ensemble learning to improve prediction accuracy.

Technologies Used
Python: The core programming language for the machine learning models and the web interface.

Gradio: A Python library for creating easy-to-use interfaces for machine learning models.

Scikit-learn: A Python library used for building machine learning models and model evaluation.

Pandas: Used for data manipulation and analysis.

NumPy: A library for numerical computations and data processing.

Model Training
Steps Involved in Training
Dataset: The dataset used contains mobile phone specifications and their corresponding price ranges. The dataset is loaded using Pandas.

Feature Selection: All columns except the target price_range are considered features (e.g., battery power, camera, RAM).

Model Definition: Multiple machine learning models are defined, including:

SVC (Support Vector Classifier)

DecisionTreeClassifier

RandomForestClassifier

LogisticRegression

KNeighborsClassifier

GaussianNB

GradientBoostingClassifier

AdaBoostClassifier

RidgeClassifier

Perceptron

SGDClassifier

MLPClassifier (Multilayer Perceptron)

ExtraTreesClassifier

Voting Classifier: A VotingClassifier is created using these models, which combines their predictions and uses hard voting to determine the final output.

Training: The model is trained using 80% of the dataset and tested on the remaining 20%.

Evaluation
After training the model, we evaluate its accuracy using the accuracy_score function from Scikit-learn.

Accuracy
The model's accuracy is printed, which gives an idea of how well the model performs on the test data.

Features and Inputs
The model takes the following inputs to predict the price range:

Battery Power (mAh)

Bluetooth (0=No, 1=Yes)

Dual SIM (0=No, 1=Yes)

4G (0=No, 1=Yes)

Internal Memory (GB)

Number of Processor Cores

Primary Camera (MP)

3G (0=No, 1=Yes)

Touch Screen (0=No, 1=Yes)

WiFi (0=No, 1=Yes)

Talk Time (hours)

Mobile Weight (grams)

Screen Height (pixels)

Screen Width (pixels)

Clock Speed (GHz)

Front Camera (MP)

RAM (MB)

Rear Camera (MP)

GPS (0=No, 1=Yes)

Edge Support (0=No, 1=Yes)

The prediction is based on these features, and the model outputs one of the following price ranges:

Low Price 💸

Medium Price 💵

High Price 💰

Very High Price 🏆
How to Run the Application
Install Dependencies:

Ensure you have Python installed.

Install the required Python libraries by running:

bash
Copy
Edit
pip install pandas numpy scikit-learn gradio
Running the Application:

Save the code in a Python file (e.g., mobile_price_predictor.py).

Run the file:

bash
Copy
Edit
python mobile_price_predictor.py
This will start the Gradio interface locally, and you can interact with the app via your browser at http://localhost:7860.

Conclusion
The Mobile Price Predictor leverages ensemble learning to create a robust and accurate model for predicting mobile price ranges. By combining the power of multiple models, it provides reliable predictions based on a variety of mobile specifications.

This version provides more details on the algorithm, the models used, and how the application works, without going into excessive detail.








