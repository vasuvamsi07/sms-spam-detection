# SMS Spam Detection

This repository provides a complete pipeline for building, deploying, and integrating an SMS spam detection model using Natural Language Processing (NLP). The project spans model creation, API deployment, Android app integration, and includes all necessary datasets and output images.

## Repository Structure

```
sms-spam-detection/
│
├── nlp/
│   └── notebooks/
│       └── *.ipynb / *.iypy  # Jupyter Notebooks and interactive Python scripts for model creation
│   └── model.pkl             # Trained machine learning model (pickle file)
│   └── vectorizer.pkl        # Fitted vectorizer for feature extraction (pickle file)
│
├── api-creation/
│   └── ...                   # Files required for API deployment (e.g., Flask/FastAPI app)
│   └── render.yaml           # (Example) Render deployment configuration file
│
├── data-set/
│   └── ...                   # Raw and processed datasets used for training/testing the model
│
├── android-app/
│   └── ...                   # Android Studio project files for integrating model predictions
│
├── output-imgs/
│   └── ...                   # Images related to the project (visualizations, UI screenshots, etc.)
│
└── README.md
```

---

## Project Overview

This project aims to detect spam messages in SMS using machine learning and NLP techniques. The workflow involves:

1. **Data Preparation**  
   - Raw SMS data is stored in the `data-set` folder.
   - Data is cleaned and preprocessed for use in training.

2. **Model Creation (`nlp/notebooks`)**  
   - Interactive Python (`.iypy`) and Jupyter Notebook files contain all code for preprocessing, feature extraction, model training, and evaluation.
   - The trained model (`model.pkl`) and vectorizer (`vectorizer.pkl`) are serialized for reuse.

3. **API Creation (`api-creation`)**  
   - Provides an API (e.g., using Flask or FastAPI) to serve the model for inference.
   - Includes configuration for deployment on platforms like Render.

4. **Android App Integration (`android-app`)**  
   - Contains code and instructions for integrating the API with an Android app.
   - Indicates which files to modify in your Android Studio project to connect to the API and display results.

5. **Visualization & Output (`output-imgs`)**  
   - All images related to the project, including model performance graphs, confusion matrices, and app screenshots.

---

## How to Use

### 1. Train the Model

- Navigate to `nlp/notebooks` and run the `.ipynb` or `.iypy` files to preprocess data and train the model.
- The trained model and vectorizer will be saved as `model.pkl` and `vectorizer.pkl`.

### 2. Deploy the API

- Go to `api-creation` and follow the provided instructions (see `README` or comments in code).
- Deploy the API using Render or your preferred platform.

### 3. Android App Integration

- Open the `android-app` folder in Android Studio.
- Modify the necessary files as indicated in the folder to connect your app to the deployed API.
- Build and run the app to test SMS spam detection.

### 4. Explore Outputs

- All generated images, graphs, and screenshots can be found in the `output-imgs` folder.

---

## Requirements

- Python 3.x
- Jupyter Notebook
- Required libraries (see requirements.txt or notebook headers, e.g., scikit-learn, pandas, numpy, flask/fastapi, etc.)
- Android Studio (for app development)
- Render account (for API deployment, optional)
