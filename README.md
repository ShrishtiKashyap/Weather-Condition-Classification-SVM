# Weather Condition Classification using Support Vector Machine (SVM)

## Project Overview

This project implements a **Support Vector Machine (SVM)** classifier to classify weather conditions as **Warm** or **Cool** using real-time weather data collected from the **Open-Meteo API**. The dataset is preprocessed, standardized, and used to train an SVM model with the **RBF kernel**. The model is evaluated using multiple classification metrics and a confusion matrix.

---

## Objective

The objective of this project is to build a machine learning model that predicts whether a weather condition is **Warm** or **Cool** based on meteorological observations such as temperature, humidity, pressure, and wind speed.

---

## Data Source

**Open-Meteo Weather API**

- Website: https://open-meteo.com/
- No API key required
- Weather data collected from multiple Indian cities

---

## Features Used

- Temperature (°C)
- Relative Humidity (%)
- Surface Pressure (hPa)
- Wind Speed (km/h)

### Target Variable

| Weather Class | Condition |
|---------------|-----------|
| Warm | Temperature ≥ 25°C |
| Cool | Temperature < 25°C |

---

## Technologies Used

- Python
- Pandas
- NumPy
- Requests
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Project Workflow

1. Fetch weather data from the Open-Meteo API.
2. Convert the JSON response into a Pandas DataFrame.
3. Create the **Weather_Class** target variable.
4. Perform data preprocessing:
   - Remove unnecessary columns
   - Check for missing values
   - Encode the target variable
   - Split the dataset into training and testing sets
   - Standardize feature values using StandardScaler
5. Train an **SVM Classifier** using the **RBF kernel**.
6. Predict weather conditions for the test dataset.
7. Evaluate the model using:
   - Accuracy
   - Precision
   - Recall
   - F1-Score
   - Confusion Matrix

---

## Results

The Support Vector Machine classifier successfully learned to distinguish between **Warm** and **Cool** weather conditions using meteorological features. After feature scaling and training with the RBF kernel, the model achieved reliable classification performance on the test dataset.

---

## Conclusion

This project demonstrates the practical implementation of the Support Vector Machine algorithm for weather condition classification using real-time weather data. Feature scaling played an important role in improving the model's performance because SVM is sensitive to the magnitude of input features. An important advantage of SVM is its ability to perform well on complex classification problems, while a limitation is that training can become computationally expensive for very large datasets.

---

## Repository Structure

```
Weather-Condition-Classification-SVM/
│── Assignment-6.ipynb
│── weather_data.csv
│── README.md
│── requirements.txt
└── .gitignore
```

---
