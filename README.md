# AgriPredict 🌾
## 📋 Overview

AgriPredict is a simple, end-to-end agricultural price prediction system built with Python and Flask. The project uses historical mandi data and a trained LSTM model to forecast crop prices. With a clean HTML/CSS/JavaScript frontend and a Flask backend serving predictions, it aims to help users explore price trends and forecast future commodity prices.

## ✅ Key Features

Time-series forecasting of agricultural commodity prices using an LSTM neural network.

Web-based user interface (built with HTML, CSS, JavaScript) — no heavy front-end frameworks.

Flask backend handles data processing, model loading, and serving predictions.

Easy-to-use pipeline: upload or use available dataset → predict future prices.

Saved model and data preprocessing ensure reproducible predictions without retraining.

## 📁 Repository Structure
AgriPredict/
│
├── app.py               # Flask backend application  
├── Agri.ipynb           # Notebook used during development / analysis  
├── data/                # Folder for datasets (historical mandi data)  
│   └── total1.csv 
├── models/              # Saved trained model (LSTM) and related artifacts  
│   └── all saved models and encoders  
├── static/              # Static files (CSS, JS, frontend resources)  
│   └── index.html
│   └── script.js
│   └── styles.css
├── README.md            # This file  
└── LICENSE              # MIT license  


You can see the same structure on GitHub under the “Files” tab. 
GitHub

## 🛠️ Getting Started — Installation & Running Locally
Prerequisites

Python 3.x

pip

Installation steps
#Clone the repository
git clone https://github.com/SaloniKhare/AgriPredict.git
cd AgriPredict

#(Optional) Create and activate a virtual environment
python -m venv venv
source venv/bin/activate      # on Linux/macOS
#venv\Scripts\activate       # on Windows

#Install dependencies (if requirements.txt available; else manually install Flask, numpy, pandas, keras etc.)
pip install -r requirements.txt

Running the application
python app.py


Once the server is running, open your browser and navigate to:

http://127.0.0.1:5000/


You should see the web interface where you can upload data or select existing datasets to predict future prices.

## 🧠 How It Works

The backend loads a pre-trained LSTM model (stored under models/).

When the user submits a request via the frontend UI, the Flask backend preprocesses the input data (normalization, windowing, etc.).

The LSTM model predicts future price values.

Predictions are returned to the frontend and displayed to the user (via charts or tables, depending on your implementation).

This makes it easy for users to get predictions without having to retrain the model themselves.

## 💡 Usage Example

Navigate to the homepage in browser.

Upload mandi (price) data or choose existing data (if provided).

Select the crop/commodity and any filters (as per your UI).

Click “Predict” (or equivalent button) — the system returns price forecasts.

View predicted price trends (e.g., future 7-day or monthly forecasts) on the UI.

## 🧠 Machine Learning Model

The project uses an LSTM (Long Short-Term Memory) neural network for forecasting agricultural price trends.

Model pipeline includes:

Data cleaning

MinMax scaling

Sequence generation

LSTM training

Saving trained model and scaler

The saved model enables predictions without retraining.

## 📥 Outputs

Future price predictions

Graph-based output (if implemented)

Preprocessed dataset

Prediction results rendered on the frontend

## 📄 License

This project is licensed under the MIT License (see LICENSE file). 
GitHub

## 🙋 Contributing & Improvements

Feel free to contribute! Here are some ways to get involved:

Extend the project by adding more crops or commodities.

Improve the UI: add charts, better styling, responsive design.

Add data validation and error handling for uploads.

Incorporate additional features: seasonal analysis, comparison across years/states, user accounts, etc.

Retraining: update and retrain LSTM model with more data to improve accuracy.

If you make improvements, please open a Pull Request, or raise an Issue to discuss before implementing large changes.

## 🎓 About & Author

AgriPredict was developed by Saloni Khare as a machine-learning and data-science project.
It demonstrates use of time-series forecasting (LSTM), data preprocessing, and web deployment via Flask, with a minimal but functional frontend.
### Saloni Khare
B.Tech CSE-AIML | AI/ML & Data Science Enthusiast
