# Mobile Price Range Predictor 📱

This project uses machine learning to predict the price range of a mobile phone based on its specifications. The model leverages a **Voting Classifier** that combines multiple algorithms to make predictions. The app is built with **Gradio** to provide a simple user interface for making predictions.

## Technology Stack 🚀

- **Python**: The primary programming language used for building the model and app.
- **Machine Learning Libraries**:
  - **Scikit-learn**: For building and training the classifiers.
  - **Voting Classifier**: Combines several models to make predictions.
  - **Classifiers Used**:
    - Support Vector Classifier (SVC)
    - Decision Tree Classifier
    - Random Forest Classifier
    - Logistic Regression
    - K-Nearest Neighbors (KNN)
    - Gaussian Naive Bayes (NB)
    - Gradient Boosting Classifier
    - AdaBoost Classifier
    - Ridge Classifier
    - Perceptron
    - Stochastic Gradient Descent (SGD) Classifier
    - Multi-layer Perceptron (MLP)
    - Extra Trees Classifier
- **Gradio**: For creating an interactive web interface where users can input mobile specifications and receive price predictions.
- **Pandas & Numpy**: For data manipulation and handling.
  
## Features 🛠️

- Predict the price range of a mobile phone based on various specifications.
- Mobile price prediction is categorized into 4 ranges:
  - Low Price 💸
  - Medium Price 💵
  - High Price 💰
  - Very High Price 🏆
  
## How It Works 🧠

1. **Model**: 
   The model uses a **Voting Classifier** that combines various classifiers such as SVC, Decision Tree, Random Forest, KNN, and others. The input features include specifications like battery power, screen size, RAM, camera quality, etc.
   
2. **User Input**: 
   Users can provide specifications for a mobile phone, and the model will predict the price range based on those features.
   
3. **Prediction**: 
   The result is displayed as a text message, showing the predicted price range of the mobile phone (Low, Medium, High, Very High).

## Installation Instructions 💻

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/mobile-price-predictor.git
cd mobile-price-predictor
2. Install Dependencies
Make sure you have Python 3.7+ installed on your machine.

Create a virtual environment:

bash
Copy
Edit
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
Install the required dependencies:

bash
Copy
Edit
pip install -r requirements.txt
The requirements.txt should include:

nginx
Copy
Edit
pandas
numpy
gradio
scikit-learn
3. Dataset
Make sure the dataset.csv is located in the specified directory:

swift
Copy
Edit
C:/Users/mohan/OneDrive/Desktop/Modile Procing Predictor/dataset.csv
If you're running this on a different machine, update the file path in the code accordingly.

4. Run the App
Start the Gradio app by running:

bash
Copy
Edit
python app.py
The app will start running on http://127.0.0.1:7866. You can access the interface in your browser by navigating to this URL.

5. Usage
Once the app is running, you can input the mobile phone specifications, and the model will predict the price range. The input includes fields like battery power, RAM, screen size, camera quality, etc.

Example Inputs:
Battery Power: 1500 mAh

Bluetooth: Yes (1)

Dual SIM: Yes (1)

4G: Yes (1)

Internal Memory: 16 GB

Number of Processor Cores: 4

Primary Camera: 12 MP

Talk Time: 12 hours

Weight: 150 grams

RAM: 2000 MB

And more...

Example Outputs:
Low Price 💸

Medium Price 💵

High Price 💰

Very High Price 🏆

Gradio Link 🔗
You can access the web interface for predictions at:

http://127.0.0.1:7866

Contributing 🤝
If you want to contribute to the project, feel free to fork the repository, make changes, and submit a pull request.

License 📜
This project is licensed under the MIT License - see the LICENSE file for details.

Note: This project is for educational purposes and may require further optimization for production use.

markdown
Copy
Edit

### Key Sections:
- **Technology Stack**: Explains the tools and libraries used.
- **Features**: Lists what the app can do.
- **Installation Instructions**: How to get the project up and running.
- **Gradio Link**: Provides a direct link to the app once it's running locally.
- **Contributing**: Encourages others to contribute.

Feel free to update the repository link, dataset path, or any other specific details.








