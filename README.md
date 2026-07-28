# Weather Condition Classification using Support Vector Machine (SVM)

## Objective

The objective of this project is to classify weather conditions as **Warm** or **Cool** using a Support Vector Machine (SVM) classifier. Weather data is collected from the Open-Meteo API and preprocessed before training the machine learning model.

---

## API Documentation

Open-Meteo API:
https://open-meteo.com/

---

## Dataset

The dataset is generated using the Open-Meteo Weather API by collecting hourly weather information from multiple cities.

### Features

- Temperature
- Relative Humidity
- Surface Pressure
- Wind Speed

### Target Variable

- Warm → Temperature ≥ 25°C
- Cool → Temperature < 25°C

---

## Libraries Used

- Python
- Pandas
- NumPy
- Requests
- Matplotlib
- Scikit-learn

---

## Methodology

1. Fetch weather data using the Open-Meteo API.
2. Convert JSON data into a Pandas DataFrame.
3. Create the Weather_Class target variable.
4. Perform data preprocessing:
   - Remove unnecessary columns
   - Encode target labels
   - Split dataset into training and testing sets
   - Standardize feature values
5. Train an SVM classifier using the RBF kernel.
6. Evaluate the model using:
   - Accuracy
   - Precision
   - Recall
   - F1-Score
   - Confusion Matrix

---

## Results

The Support Vector Machine successfully classified weather conditions into Warm and Cool categories using meteorological features. The trained model demonstrated good classification performance on the testing dataset.

---

## Conclusion

The project demonstrates the use of Support Vector Machines for weather classification using real-time weather data from the Open-Meteo API. Feature scaling improved the model's performance, making SVM effective for this classification task. While SVM provides strong predictive accuracy, it may become computationally expensive for very large datasets.