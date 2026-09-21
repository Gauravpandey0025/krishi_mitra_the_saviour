# krishi_mitra_the_saviour
# 🌱 Krishi Mitra

AI-Powered Crop Prediction & Smart Agriculture Assistant






🌾 Overview

Krishi Mitra is an AI-based crop recommendation system designed to help farmers identify a suitable crop based on agricultural and environmental conditions.

The system uses soil and weather parameters such as:

Nitrogen (N)

Phosphorus (P)

Potassium (K)

Temperature

Humidity

Soil pH

Rainfall

The project combines Machine Learning, weather data, satellite information and IoT-based agricultural data to support crop recommendation.

<details>
<summary>📑 <b>Table of Contents</b></summary>

Overview

Key Features

System Architecture

Prediction Workflow

Input Parameters

Machine Learning Model

Data Sources

Technologies

Project Structure

Deployment

Future Improvements

</details>

✨ Key Features

🌱 AI-based crop recommendation

🧪 Soil nutrient analysis

🌦️ Weather-based prediction

🛰️ Satellite-data integration

📡 IoT sensor integration

🌧️ Rainfall and environmental parameter analysis

🤖 Machine Learning prediction

🌐 Web-based interface

☁️ Cloud deployment

🧠 System Architecture

                 ┌─────────────────────┐
                 │     User / Farmer   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   Input Parameters  │
                 │ N, P, K, pH, etc.   │
                 └──────────┬──────────┘
                            │
                            ▼
        ┌────────────────────────────────────┐
        │        Data & Environment          │
        │                                    │
        │  🌦️ Weather APIs                   │
        │  🛰️ Satellite Data                 │
        │  📡 IoT Sensors                    │
        └────────────────┬───────────────────┘
                         │
                         ▼
                 ┌─────────────────────┐
                 │ Data Preprocessing  │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Machine Learning    │
                 │ Crop Prediction     │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Recommended Crop    │
                 └─────────────────────┘

🔄 Prediction Workflow

Farmer Input
     │
     ▼
Soil Parameters
(N, P, K, pH)
     │
     ▼
Environmental Parameters
(Temperature, Humidity, Rainfall)
     │
     ▼
Preprocessing
     │
     ▼
Trained ML Model
     │
     ▼
Crop Prediction
     │
     ▼
🌾 Recommended Crop

🧪 Input Parameters

Parameter

Description

N

Nitrogen level in soil

P

Phosphorus level in soil

K

Potassium level in soil

Temperature

Environmental temperature

Humidity

Environmental humidity

pH

Soil acidity/alkalinity

Rainfall

Rainfall condition

🤖 Machine Learning Model

The project uses a Decision Tree-based Machine Learning approach for crop recommendation.

Model Pipeline

Agricultural Data
       ↓
Data Cleaning
       ↓
Feature Preparation
       ↓
Model Training
       ↓
Decision Tree
       ↓
Crop Prediction

The trained model and preprocessing components can be saved and loaded for inference.

Typical model files include:

dtr.pkl
preprocessor.pkl

<details>
<summary>🛰️ <b>Data Sources & Integrations</b></summary>

ISRO Satellite Data

Satellite information can provide agricultural/environmental information useful for understanding field conditions.

IMD Weather Data

Weather information can be used to incorporate environmental conditions into the crop recommendation process.

OpenWeatherMap

Weather API integration can provide parameters such as temperature, humidity and rainfall-related information.

Tomorrow.io

Additional weather information can be integrated for environmental analysis.

IoT Sensors

Agricultural sensors can provide real-time field/soil information.

Communication

IoT devices can use technologies such as:

IoT Sensor
    ↓
LoRaWAN / GSM
    ↓
Data Collection
    ↓
Prediction System

</details>

🛠️ Technologies Used

Technology

Purpose

Python

Core development

Pandas

Data processing

NumPy

Numerical operations

Scikit-learn

Machine Learning

Decision Tree

Crop prediction

Joblib / Pickle

Model persistence

Flask

Backend/API

HTML/CSS

Frontend

Tailwind CSS

UI styling

JavaScript

Frontend interaction

Render

Deployment

Git & GitHub

Version control

Jupyter Notebook

Model development

📁 Project Structure

Krishi-Mitra/
│
├── model/
│   ├── dtr.pkl
│   └── preprocessor.pkl
│
├── notebooks/
│   └── model_training.ipynb
│
├── app.py
├── requirements.txt
├── README.md
└── frontend/
    ├── index.html
    ├── style.css
    └── script.js

Adjust the structure above if your actual repository uses different filenames or folders.

🔌 Backend Workflow

Frontend
   │
   │ HTTP Request
   ▼
Flask API
   │
   ▼
Load Preprocessor
   │
   ▼
Transform Input
   │
   ▼
Load Trained Model
   │
   ▼
Predict Crop
   │
   ▼
JSON Response
   │
   ▼
Frontend Result

<details>
<summary>☁️ <b>Deployment</b></summary>

The crop prediction backend can be deployed using Render.

Typical deployment flow:

GitHub Repository
       ↓
Render
       ↓
Flask Application
       ↓
Trained ML Model
       ↓
API Endpoint
       ↓
Frontend

</details>

<details>
<summary>📊 <b>Example Prediction</b></summary>

Input
────────────────────────
N            → Soil value
P            → Soil value
K            → Soil value
Temperature  → °C
Humidity     → %
pH           → Soil pH
Rainfall     → mm
────────────────────────
             ↓
       ML Prediction
             ↓
      🌱 Recommended Crop

</details>

🎯 Project Objective

The objective of Krishi Mitra is to combine agricultural data and Machine Learning to provide a data-driven crop recommendation system.

       🌱 FARM DATA
            │
     ┌──────┴──────┐
     ▼             ▼
   SOIL          WEATHER
     │             │
     └──────┬──────┘
            ▼
      MACHINE LEARNING
            │
            ▼
      CROP PREDICTION
            │
            ▼
       🌾 FARMER

🔮 Future Improvements

📍 Location-based crop recommendations

🌦️ Real-time weather integration

🛰️ More satellite-derived features

📡 Real-time IoT sensor data

💰 Market-price integration

📈 Crop yield prediction

🌾 Crop disease detection

📱 Mobile application

🌐 Multilingual farmer interface

🧠 Comparison of multiple ML algorithms

👨‍💻 Author

Gaurav Pandey

B.Tech CSE (Data Science)
Chandigarh Group of Colleges, Landran
Session: 2023–2027
