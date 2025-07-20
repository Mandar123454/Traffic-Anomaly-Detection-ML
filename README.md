# 🚗 Traffic Anomaly Detector + Self-Improving Model

A smart machine learning system built with Python and Google Colab to detect unusual traffic patterns (anomalies) using a custom dataset. The model self-improves over time by learning from new data and updating itself.

---

## 📌 Project Overview

This project uses a **Random Forest Classifier** to classify traffic as **Normal** or **Anomalous**. It simulates real-world traffic behavior, performs automated retraining on new data, and visualizes performance metrics.

---

## 📁 Dataset

- **Format**: CSV  
- **Size**: 1000 entries  
- **Features**: `vehicle_speed`, `vehicle_count`, `accident_flag`, `time_of_day`, `weather_condition`, `traffic_label`

Example:

| vehicle_speed | vehicle_count | location | time_of_day | is_anomaly |
|---------------|---------------|----------|-------------|------------|
| 35.6          | 45            | Highway  | Morning     | 0          |

---

## 🧠 Steps & Workflow

### ✅ Step 1: Data Generation & Loading
- Created a synthetic traffic dataset with labeled entries.
- Stored in CSV format for easy loading in Colab.

### 🔍 Step 2: Exploratory Data Analysis (EDA)
- Analyzed feature distributions.
- Visualized categorical variables like time of day and weather.

### 🧼 Step 3: Data Preprocessing
- Applied Label Encoding to categorical columns.
- Checked for nulls and cleaned dataset.

### 🤖 Step 4: Model Training
- Trained a **RandomForestClassifier** on 80% of the data.
- Achieved **initial accuracy of 1.0**.

### 📉 Step 5: Performance Visualization
- Generated learning curves and accuracy drift plots.
- Tracked model performance before and after retraining.

### 🔁 Step 6: Self-Improving Model
- Accepted new entries dynamically.
- Detected anomalies and updated the model using new samples.
- Achieved updated accuracy of **0.993** after retraining.

### 🚨 Step 7: Real-time Prediction
- Detected traffic as either:
  - 🔴 **"Anomaly Detected!"**
  - ✅ **"Normal Traffic"**

---

## 📊 Visuals

- Learning Curve
- Accuracy Drift
- Feature Importance (optional)

*Visuals generated using matplotlib and seaborn.*

---

## 🔮 Future Scope

1. **Integration with Live Traffic APIs** for real-time monitoring.  
2. **Deployment on Edge/IoT Devices** for smart city use cases.  
3. **Multi-Class Anomaly Detection** for deeper traffic insights.

---

## 📌 Tech Stack

- **Language**: Python  
- **Platform**: Google Colab  
- **Libraries**: pandas, scikit-learn, matplotlib, seaborn, numpy

---

## 🚀 Output Example

```bash
✅ Normal Traffic
🚨 Anomaly Detected!
