
# 🌱 Crop Recommendation System using Machine Learning

This project focuses on recommending the most suitable crop to plant based on soil nutrients and environmental conditions using machine learning. It aims to support farmers in making data-driven agricultural decisions.

---

## 📌 Problem Statement

Farmers often face challenges in selecting the right crop to grow for a given set of soil and climate conditions. Manual decisions can lead to inefficiencies, poor yield, or misuse of resources.

**Goal:** Build a machine learning model that predicts the optimal crop based on environmental and soil features such as nitrogen, potassium, pH, temperature, and rainfall.

---

## 🧾 Dataset Overview

- 📊 **Total Samples**: 2200
- 🌿 **Features**:
  - Nitrogen (N)
  - Phosphorus (P)
  - Potassium (K)
  - Temperature (°C)
  - Humidity (%)
  - pH
  - Rainfall (mm)
- 🎯 **Target**: Crop label (22 classes)

No missing values or duplicate entries were found.

---

## 🧪 Modeling Approach

We explored the following classification models:

| Model               | Purpose                          |
|--------------------|----------------------------------|
| Logistic Regression| Baseline interpretability        |
| Decision Tree      | Non-linear, interpretable splits |
| Random Forest      | High performance with tuning     |

- Data was standardized and split 80/20 into training and testing sets.
- Random Forest achieved the best accuracy.

---

## 📊 Key Visuals

### 🔗 Feature Correlation Heatmap
Shows how independent the features are — useful for modeling.
> Weak correlations → good for diverse model learning.

### ✅ Confusion Matrix (Random Forest)
Evaluates prediction accuracy. Most crops were correctly classified with few confusions between similar crops.

### 🌿 Feature Importance
Highlights the top contributors to model decisions:
1. **Nitrogen**
2. **Potassium**
3. **Temperature**

---

## 🎯 Final Recommendation

- ✔ Use **Random Forest** for accurate crop prediction.
- 📢 For communication with farmers, **Decision Trees** provide clear explanations.
- 🔍 Prioritize monitoring **Nitrogen**, **Potassium**, and **Temperature** in the field.
- 🧩 Combine predictions with domain knowledge for agricultural planning.

---

## 📁 Project Structure

```
Crop-Recommendation-ML/
├── data/               # Dataset file
├── notebooks/          # Analysis and modeling notebooks
├── images/             # Visual outputs
├── presentation/       # PowerPoint slides
├── models/             # Model files (optional)
├── README.md           # Project overview
```

---

## 🛠 How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Launch notebook:
   ```bash
   cd notebooks
   jupyter notebook crop_recommendation.ipynb
   ```

3. View results in:
   - `images/` (graphs)
   - `presentation/` (summary PowerPoint)

---

## 👤 Author

- Maxwell Njoroge

---

## 📜 License

This project is licensed under the MIT License.
