# Deforestation_Fire_Classification
##_AICTE_Internship_##

# 🔥 Classification of Fire Types in India Using MODIS Satellite Data

This project focuses on classifying different types of fire events in India using MODIS satellite data. It combines rule-based preprocessing with machine learning techniques to categorize fire events into vegetation fires, industrial fires, and offshore sources.

---

## 🎯 Objectives

- Analyze thermal anomaly data from NASA MODIS (FIRMS).
- Clean and preprocess multi-year fire datasets.
- Visualize spatial and statistical trends in fire events.
- Train and evaluate multiple machine learning classifiers.
- Classify fire events into meaningful categories using location and intensity features.

---

## 🛰️ Data Source

- **MODIS Fire Data** (2021–2023): Downloaded from [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/)
- Includes fields like `latitude`, `longitude`, `brightness`, `confidence`, `type`, and `acq_date`.

---

## 📂 Dataset Structure

- `modis_2021_India.csv`
- `modis_2022_India.csv`
- `modis_2023_India.csv`

Each file includes:
- Latitude, Longitude
- Brightness and Confidence
- Acquisition Date and Time
- Fire Type (labeled)

---

## 📊 Project Workflow

### 1. 🔹 Data Loading & Merging

Multiple yearly CSV files are loaded and concatenated into a single dataset using `pandas`.

### 2. 🔍 Exploratory Data Analysis (EDA)

- Inspected data types and statistics
- Checked missing and duplicate entries
- Visualized:
  - Fire type distribution (`countplot`)
  - Confidence scores (`histplot`, `boxplot`)

### 3. ⚙️ Preprocessing

- Label encoding of fire type (`LabelEncoder`)
- Feature scaling using `StandardScaler`

### 4. 🧠 Model Training

Trained multiple models using:
- **Random Forest Classifier**
- **K-Nearest Neighbors (KNN)**
- **XGBoost Classifier**

### 5. 📈 Evaluation

- Accuracy and F1-score reported
- Confusion matrix displayed to show performance by class

---

## 🔬 Key Features Used

- `latitude`
- `longitude`
- `brightness`
- `confidence`

---

## 🧠 ML Techniques Used

- Label encoding for target variable
- Feature scaling for model compatibility
- Classification models: RandomForest, XGBoost, KNN
- `train_test_split` from Scikit-learn

---

## 📌 Results

- Random Forest produced the most stable and interpretable results.
- Spatial features combined with brightness and confidence are strong predictors of fire type.
- Visualization confirmed model separation and label consistency.

---

## 🚀 Future Enhancements

- Integrate temporal features (month, hour).
- Apply GridSearchCV for hyperparameter optimization.
- Use satellite imagery (HDF/GeoTIFF) for deeper insights.
- Add region-specific rules or crop calendar for context-aware classification.

---

## 🧰 Tech Stack

- **Language**: Python
- **Notebook**: Jupyter / Google Colab
- **Libraries**:
  - `pandas`, `numpy`
  - `scikit-learn`
  - `matplotlib`, `seaborn`
  - `xgboost`
  - `LabelEncoder`, `StandardScaler`

---


