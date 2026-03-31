# 📊 Student Productivity & Burnout Predictor
> **Course:** Fundamentals of AI and ML  
> **Author:** Arun Kumar | **Reg No:** 25BAI10984  
> **Department:** CSE (AI ML)

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![ML](https://img.shields.io/badge/Model-Random%20Forest-green.svg)]()
[![Accuracy](https://img.shields.io/badge/Accuracy-90%25-orange.svg)]()

## 🎯 Project Overview
In today’s academic world, digital fatigue is real. This project addresses the "Bring Your Own Project" challenge by analyzing how daily lifestyle habits—like sleep and screen time—directly influence productivity levels.

The goal is to predict whether a student will have **Low, Medium, or High** productivity based on their daily habits, helping in better time management and burnout prevention.

---

## 🛠 Methodology & Pipeline
I implemented a robust Machine Learning pipeline to ensure reliable predictions:

1.  **Data Acquisition:** Developed `step1_generate_data.py` to simulate a synthetic dataset of **500 days** of student activity (addressing privacy concerns of real-world logging).
2.  **Feature Engineering:** Tracked key metrics including:
    * **Independent:** Sleep Hours, Study Hours, Screen Time, Exercise, and Weekend status.
    * **Target:** Productivity Level (0: Low, 1: Med, 2: High).
3.  **Exploratory Data Analysis (EDA):** Leveraged **Seaborn** to visualize correlations. 
    * *Insight:* Study hours show the strongest positive correlation, while screen time is the primary negative driver.

---

## 🤖 Model Selection
After testing, the **Random Forest Classifier** was selected for the following reasons:
* **Non-linearity:** Excellent at handling complex relationships between features.
* **Robustness:** Highly resistant to overfitting compared to standard Decision Trees.
* **Performance:** Achieved a validation accuracy of **~90%** on an 80/20 train-test split.

---

## 💡 Key Challenges & Decisions
* **The Weekend Effect:** Included a "Weekend" binary variable to account for the drastic shift in student habits on Saturdays and Sundays.
* **Optimization:** Improved initial low accuracy by implementing **Feature Scaling** and refining the data generation logic to weigh "burnout factors" (like high screen time) more heavily.

---

## 📈 Learning & Reflections
* **Data > Models:** Cleaning and preparing data takes 80% of the effort; the model is only as good as the data it's fed.
* **Efficiency:** A well-tuned Random Forest often outperforms a complex Neural Network for tabular datasets.
* **DevOps:** Version control via GitHub was crucial for documenting the development lifecycle and tracking progress.

---

## 🚀 How to Run
1. Clone the repo:
   ```bash
   git clone [https://github.com/yourusername/productivity-predictor.git](https://github.com/yourusername/productivity-predictor.git)


## Install dependencies:

Bash
pip install pandas seaborn scikit-learn

## Generate data and train:
Bash
python step1_generate_data.py
python train_model.py

## Developed as part of the AI & ML Fundamentals coursework.
