# Building Energy Consumption Anomaly Detection

## Overview

This project analyzes large-scale building electricity consumption data from the Building Data Genome Project 2 (BDG2) dataset. The objective is to identify abnormal energy consumption patterns using machine learning and time-series analysis techniques.

The project includes data preprocessing, feature engineering, anomaly detection, visualization, and business-oriented analysis to better understand building energy behavior.

**Note:** This was a team project. My primary contribution was implementing the machine learning–based anomaly detection component using the Isolation Forest algorithm and analyzing abnormal energy consumption patterns.

---

## Dataset Information

* Dataset: Building Data Genome Project 2 (BDG2)
* Time Period: 2016–2017
* Frequency: Hourly readings
* Buildings: 1,500+
* Total Records: 17,544 timestamps
* Type: Multivariate Time-Series Data

Each row represents a timestamp and each column represents the electricity consumption of a building.

---

## Project Workflow

1. Data Loading
2. Data Cleaning
3. Missing Value Handling
4. Feature Engineering
5. Anomaly Detection
6. Visualization and Analysis
7. Business Insights

---

## Feature Engineering

The following features were generated to capture temporal consumption patterns:

* Hour of Day
* Day of Week
* Weekend Indicator
* 1-Hour Lag Feature
* 24-Hour Lag Feature
* 24-Hour Rolling Mean
* 24-Hour Rolling Standard Deviation

---

## Machine Learning Approach

### Isolation Forest

Isolation Forest was used as the primary anomaly detection model.

Key characteristics:

* Unsupervised learning approach
* Detects unusual consumption behavior without labeled anomaly data
* Efficient for large-scale datasets
* Suitable for complex and seasonal energy usage patterns

The model identifies abnormal spikes and drops in electricity consumption that may indicate operational inefficiencies, equipment issues, or unusual building activity.

---

## Results

* Anomalies Detected: 175
* Anomaly Percentage: Approximately 1%

Detected anomalies were visualized and analyzed to understand abnormal energy consumption behavior across buildings.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Git
* GitHub

---

## Repository Structure

```text
Building-Energy-Analysis
│
├── src/
├── results/
├── main.py
├── Energy_Anomaly_Detection_FULL_Project.ipynb
└── README.md
```

---

## Contribution

Team Project

My contribution focused on:

* Machine learning–based anomaly detection
* Isolation Forest implementation
* Anomaly visualization
* Interpretation of abnormal energy consumption patterns
