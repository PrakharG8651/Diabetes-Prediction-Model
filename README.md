# Diabetes Prediction Model

A machine learning web application that predicts the likelihood of a patient having diabetes based on key medical diagnostic measurements. Built with Streamlit and a trained classification model, the app provides instant predictions along with a confidence score.

## Overview

This project uses the Pima Indians Diabetes Dataset to train a machine learning model capable of classifying whether a patient is likely diabetic or not. The trained model is deployed through an interactive Streamlit interface where users can input patient data and get real-time predictions.

## Features

- Interactive web interface built with Streamlit
- Takes 8 medical input parameters from the user
- Predicts diabetes risk using a pre-trained ML model
- Displays prediction confidence as a percentage

## Input Parameters

| Parameter | Description |
|---|---|
| Pregnancies | Number of times pregnant |
| Glucose | Plasma glucose concentration |
| Blood Pressure | Diastolic blood pressure (mm Hg) |
| Skin Thickness | Triceps skin fold thickness (mm) |
| Insulin | 2-Hour serum insulin (mu U/ml) |
| BMI | Body Mass Index |
| Diabetes Pedigree Function | Likelihood of diabetes based on family history |
| Age | Age in years |

## Project Structure
```
Diabetes-Prediction-Model/
├── app.py
├── Diabetes_Prediction.ipynb
├── diabetes.csv
├── diabetes_model.pkl
└── README.md
```

## Tech Stack

- Python
- Streamlit (web app framework)
- scikit-learn (model training)
- NumPy (numerical computations)
- joblib (model serialization)
- Jupyter Notebook (data analysis and training)

## Getting Started

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/PrakharG8651/Diabetes-Prediction-Model.git
   cd Diabetes-Prediction-Model
   ```

2. (Recommended) Create a virtual environment
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. Install dependencies
   ```bash
   pip install streamlit numpy scikit-learn joblib pandas
   ```

### Running the App

```bash
streamlit run app.py
```

The app will open automatically in your browser at `http://localhost:8501`.

## Model Training

The model was trained and exported using `Diabetes_Prediction.ipynb`, which covers:

- Loading and exploring `diabetes.csv`
- Data preprocessing
- Model training and evaluation
- Exporting the final model as `diabetes_model.pkl`

To retrain or experiment with the model, open the notebook:

```bash
jupyter notebook Diabetes_Prediction.ipynb
```

## Contributing

Contributions are welcome. If you'd like to improve this project:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add some feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request
