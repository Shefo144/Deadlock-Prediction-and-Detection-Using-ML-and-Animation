# Deadlock-Prediction-and-Detection-Using-ML-and-Animation

## Overview
This project combines the traditional Banker’s Algorithm with Machine Learning techniques to detect and predict deadlock conditions in operating systems.

The system generates different resource allocation states, analyzes them using Banker’s Algorithm, extracts important numerical features, and trains multiple machine learning models to classify system states as either SAFE or DEADLOCK.

The project also includes animated visualization of the Resource Allocation Graph (RAG).

---

# Features
- Banker’s Algorithm implementation
- Deadlock detection
- Safe sequence generation
- Automatic dataset generation
- Machine Learning deadlock prediction
- Resource Allocation Graph visualization
- Animated graph simulation
- Multiple ML model comparison
- User custom input testing
- ROC Curve and Confusion Matrix visualization

---

# Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- NetworkX
- Joblib
- Imbalanced-learn

---

# Machine Learning Models
The following models are trained and evaluated:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)
- XGBoost Classifier

The best-performing model is automatically saved for future predictions.

---

# Project Workflow

## 1. Dataset Generation
The project generates:
- Random system states
- Safe states
- Deadlock-prone states

---

## 2. Banker’s Algorithm
The algorithm checks whether the current system state is:
- SAFE
- DEADLOCK

It also generates the safe sequence if one exists.

---

## 3. Feature Extraction
Important extracted features include:
- Total allocated resources
- Total needed resources
- Resource pressure
- Allocation variance
- Need variance
- Unsafe ratio
- Available resource statistics

---

## 4. Dataset Balancing
The dataset is balanced using:
bash
RandomOverSampler


---

## 5. Model Training and Evaluation
Each model is evaluated using:
- Accuracy Score
- Classification Report
- Confusion Matrix
- ROC Curve
- AUC Score

---

## 6. User Input Testing
Users can manually enter:
- Allocation Matrix
- Maximum Matrix
- Available Resources

The system then:
1. Runs Banker’s Algorithm
2. Predicts deadlock using ML
3. Displays graph visualization

---

# Example Input

## Allocation Matrix
text
P0: 1 0 1
P1: 0 2 0
P2: 1 1 0


## Maximum Matrix
text
P0: 2 1 1
P1: 1 3 1
P2: 2 1 1


## Available Resources
text
1 1 0


---

# Example Output
text
Banker Result: SAFE
Safe Sequence: [0, 2, 1]

ML Prediction: SAFE
Probability: 96.4%


---

# Visualization
The project visualizes:
- Processes
- Resources
- Allocation edges
- Request edges
- Animated graph movement

### Graph Colors
- Green → Allocated resources
- Red → Requested resources

---

# Installation

Install the required libraries:

bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost networkx joblib imbalanced-learn


---

# Run The Project

Start Jupyter Notebook:

bash
jupyter notebook


Then open the notebook file and run all cells.

---

# Generated Files

| File Name | Description |
|---|---|
| best_deadlock_model.pkl | Saved trained ML model |
| scaler.pkl | Saved feature scaler |

---

# Future Improvements
- GUI Application
- Real-time system monitoring
- Deep Learning integration
- Better graph animation
- Larger training dataset
- Live deadlock prediction

---

# Author
Mohammed Sherif

Operating Systems and Machine Learning Project for Deadlock Detection and Prediction.
