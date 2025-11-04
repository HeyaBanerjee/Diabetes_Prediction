# Diabetes_Prediction
A machine-learning web application that predicts whether a patient is likely to develop diabetes, based on health indicators.

🧾 Overview

This project uses a health-indicator dataset (from the BRFSS 2015 survey) to train a classification model for diabetes risk. A web application (built with Streamlit) provides a user-friendly interface to input features and get a prediction.

📁 Project Structure
├── app.py                     # Main Streamlit application  
├── model.py                   # Model training and evaluation code  
├── model.pkl                  # Trained model (pickle format)  
├── scaler.pkl                 # Scaler used on feature data  
├── diabetes_012_health_indicators_BRFSS2015.csv  # Dataset used for training  
├── patients_records.csv       # Example/ad hoc patient records  
├── correlation_heatmap.png    # Correlation analysis visualization  
├── boxplot_bmi.png            # Box-plot for BMI feature  
├── boxplot_menthlth.png       # Box-plot for mental health feature  
├── boxplot_physhlth.png       # Box-plot for physical health feature  
├── screenshot_app.png         # Screenshot of the running app  
├── requirements.txt           # Python dependencies  
├── README.md                  # This file  
└── diabetes_report_cd31a1e6.pdf  # Full report / documentation  

🔧 Setup & Installation

Clone the repository:

git clone https://github.com/HeyaBanerjee/Diabetes_Prediction.git  
cd Diabetes_Prediction  


Create and activate a virtual environment (optional but recommended):

python -m venv venv  
source venv/bin/activate     # Mac/Linux  
.\venv\Scripts\activate      # Windows  


Install the dependencies:

pip install -r requirements.txt  

🚀 Running the App

Once dependencies are installed, you can start the application:

streamlit run app.py  


Open the provided local URL in your browser. Input your health-indicator values and click “Predict” to see whether the model predicts diabetes risk.

🧠 Model & Methodology

The dataset used: diabetes_012_health_indicators_BRFSS2015.csv.

Data exploration and visualization steps include: correlation heatmap, box plots of key features (BMI, mental health, physical health).

Data preprocessing: feature scaling (hence scaler.pkl), train-test split, model training (details in model.py).

The model: (e.g., logistic regression / random forest / whichever you used) saved as model.pkl.

The app uses the scaler and model to process user input and output prediction.

✅ Features

Easy web-based interface for inputting health features.

Backend uses a trained ML model for prediction.

Visualizations and EDA results included in the repo for transparency.

Modular structure: you can retrain the model, replace it, or extend the app.

🔄 Retraining / Customization

To retrain or modify the model:

Open model.py and adjust preprocessing, model type, hyperparameters etc.

Run the training code to produce a new model.pkl and scaler.pkl.

Update app.py if any new input features are added.

Test locally, then push to GitHub (or deploy).

👥 Contributing

Contributions are welcome! Whether it’s:

Improving the UI/UX of the Streamlit app

Enhancing model performance (feature engineering, hyper-tuning)

Deploying the app (Heroku, AWS, etc)

Adding new visualizations, documentation, or test data
Feel free to fork the repo, make changes, and submit a pull request.
