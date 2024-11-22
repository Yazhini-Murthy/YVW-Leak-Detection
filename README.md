# Leak Management System for YVW Team

This repository contains code and datasets developed for leak management in a water distribution network. The project includes two key components: leak detection and leak localization, implemented using RNN models and various visualization techniques.

---

## 📁 Project Structure

### 1. **Leak Detection**
- **Description**: Detects leaks in the water distribution network using sensor data.
- **Folder Contents**:
  - **`leak_detection.ipynb`**:  Python Notebook containing the code for training, testing, and visualizing leak detection results.
  - **Dataset**: Raw data for the leak detection task.
  
- **Features**:
  - Binary classification of leak vs. non-leak conditions.
  - RNN-LSTM model implementation.
  - Visualizations to evaluate detection performance.

### 2. **Leak Localization**
- **Description**: Localizes the position of detected leaks using sensor coordinates and other data.
- **Folder Contents**:
  - **`All_Sensors_Leak_Localisation.ipynb`**: Code for the baseline approach using sensor readings from all 5 sensors for leak localization.
  - **`SensorX_Leak_Localisation.ipynb`**: Codes for analysing the impact of each sensor on localization accuracy.
  - **`Closest_Sensor_Approach.ipynb`**: Approach that effectively anchors the localization estimate to the sensor closest to the leak.
  - **`Non_Linear_Weighting_Ensemble_Leak_Localisation_Approach.ipynb`**: Propsoed methodology that exploits the proximity advantage of sensors closer to the leak site using Non-Linear Weighting.
  - **Datasets**: Includes all necessary data files for training and evaluation.
  
- **Features**:
  - Predicts latitude and longitude of leaks.
  - Utilizes RNN models and hyperparameter tuning.
  - Visualization of predicted vs. actual leak locations.

---

## 🛠️ Requirements

- Python 3.x
- Libraries:
  - Tensorflow
  - Pandas
  - Matplotlib
  - Scikit-learn
  - Geopy (for geographic calculations)
  - NumPy

---
