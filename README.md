Forest Cover Type Classifier 🌳
This project is a machine learning application that predicts the forest cover type based on various geographical and environmental features. It uses a powerful Stacking Classifier model combining Random Forest and XGBoost to achieve high accuracy. The project also includes a Flask web application for making interactive predictions and viewing model performance statistics.

Features ✨
Robust Model: Utilizes a Stacking Classifier with tuned RandomForestClassifier and XGBoostClassifier to leverage the strengths of both algorithms.

Automated Training: The model training process is automated. If the trained model files (stacking_model.joblib, model_stats.json, model_columns.json) are not found, the app.py script will automatically train the model from train.csv.

Data Preprocessing: Includes automated data cleaning and feature engineering steps to prepare the data for the model.

Web Interface: A user-friendly web application built with Flask allows users to input data and get a real-time prediction.

Model Statistics: The web app features a dedicated page to display the model's performance metrics, including accuracy and a classification report.

Prerequisites 📋
This project does not require a requirements.txt file. Instead, the necessary libraries are listed below. You can install them using pip.

Bash

pip install pandas scikit-learn xgboost flask joblib
How to Run 🚀
Place the dataset: Ensure you have the train.csv dataset in the same directory as app.py.

Run the application: Execute the app.py file from your terminal.

Bash

python app.py
Access the web app: The terminal will provide a URL (e.g., http://127.0.0.1:5000). Open this link in your web browser.

The application will automatically start the training process if the model files are missing. This may take some time depending on your system's performance. Once training is complete, the web server will start.

Project Structure 📂
app.py: The main Python script containing the model training logic and the Flask web application.

templates/: A directory for the HTML files used by Flask.

index.html: The home page with the prediction form.

stats.html: The page displaying the model's performance statistics.

train.csv: The dataset used to train the machine learning model.

stacking_model.joblib: (Generated after first run) The saved trained model.

model_columns.json: (Generated after first run) A JSON file listing the input features for the model.

model_stats.json: (Generated after first run) A JSON file containing the model's accuracy and classification report.
