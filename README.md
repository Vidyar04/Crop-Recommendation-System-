# Crop-Recommendation-System-
A web-based crop recommendation system using Python, Flask, and machine learning. It predicts the best crop to grow based on soil and weather factors like nitrogen, phosphorus, potassium, temperature, humidity, and pH. Powered by a trained Random Forest model, it delivers recommendations via a simple web interface.
Features
Accepts six key input features:

Nitrogen (N)
Phosphorus (P)
Potassium (K)
Temperature (°C)
Humidity (%)
pH value
Predicts the optimal crop based on trained machine learning model

Provides a user-friendly web interface using HTML templates

Built using Flask and scikit-learn

Requirements
Install the required Python libraries:

pip install flask pandas scikit-learn
Make sure the following files are present:

Crop_Recommendation.csv — Dataset used for training
index.html — Form to input parameters
result.html — Displays prediction result
How to Run
Ensure the dataset (Crop_Recommendation.csv) and HTML templates (index.html, result.html) are in the correct locations.
Run the application using the command:
python app.py
Open your browser and go to:
http://localhost:8080/
Enter the required inputs and click submit to get the crop recommendation.
Dataset
The model is trained on the Crop_Recommendation.csv dataset.
Features used: Nitrogen, Phosphorus, Potassium, Temperature, Humidity, pH_Value
Target: Crop (name of the recommended crop)
Machine Learning Model
Model: RandomForestClassifier from scikit-learn
Data split: 80% training, 20% testing
The model is trained each time the server is started
File Structure
app.py — Main Flask application with model logic
Crop_Recommendation.csv — Dataset file
templates/index.html — Input form page
templates/result.html — Output display page
Notes
Model retrains on every run; for large datasets, consider pre-saving the model using joblib.
Accuracy may vary depending on input and dataset quality.
Ensure input values are realistic for optimal predictions.
