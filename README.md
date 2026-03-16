# Bias Buster – Fairness & Bias Detection in Machine Learning

Bias Buster is a **Responsible AI project** that evaluates and detects **algorithmic bias in machine learning models**. The system analyzes model predictions across sensitive attributes (such as gender or age) and measures fairness using statistical metrics.

The goal is to help developers identify **hidden discrimination in AI systems** and improve fairness without significantly reducing model performance.


# Overview

Machine learning models trained on real-world data can unintentionally learn biased patterns. Bias Buster provides a **fairness evaluation pipeline** that analyzes model outputs across demographic groups and highlights disparities.

The project measures fairness metrics and compares **model performance before and after bias mitigation techniques**.

This project demonstrates the importance of **ethical AI and responsible machine learning deployment**.


# Key Features

- Detects **algorithmic bias in classification models**
- Evaluates predictions across **sensitive attributes**
- Computes fairness metrics such as:
  - **Disparate Impact Ratio**
  - **Group Prediction Rates**
  - **Representation Imbalance**
- Compares **model performance vs fairness trade-offs**
- Supports **bias mitigation techniques**


# Technologies Used

## Programming
- Python

## Machine Learning
- Scikit-learn
- Logistic Regression
- Decision Trees

## Data Processing
- Pandas
- NumPy

## Visualization
- Matplotlib
- Seaborn


# Project Workflow

    Dataset
        │
        ▼
    Data Preprocessing
        │
        ▼
    Train Classification Models
    (Logistic Regression / Decision Tree)
        │
        ▼
    Evaluate Model Performance
    (Accuracy, Precision, Recall)
        │
        ▼
    Fairness Evaluation
    (Disparate Impact, Group Prediction Rates)
        │
        ▼
    Bias Mitigation Techniques
    (Re-sampling / Feature Auditing)
        │
        ▼
    Compare Fairness vs Performance

 # How It Works

### 1. Load Dataset
The dataset includes features along with a **sensitive attribute** such as gender or age.

### 2. Data Preprocessing
- Handle missing values
- Normalize data
- Identify protected attributes

### 3. Model Training
Train baseline models such as:

- Logistic Regression
- Decision Trees

### 4. Fairness Evaluation
Measure fairness using metrics such as:

**Disparate Impact Ratio**

    DI = P(outcome | unprivileged group) / P(outcome | privileged group)


If **DI < 0.8**, the model may be biased.


# Bias Mitigation

Apply techniques such as:

- **Re-sampling** – balance the dataset by increasing samples from underrepresented groups or reducing overrepresented ones.
- **Feature auditing** – analyze and remove features that may indirectly introduce bias.
- **Balanced training datasets** – ensure fair representation of demographic groups during model training.


## Result Comparison

Evaluate the model after mitigation by comparing:

- **Model accuracy**
- **Fairness metrics**
- **Bias reduction effectiveness**

This helps understand the **trade-off between model performance and fairness**.


# Installation

### Clone the repository

```bash
git clone https://github.com/yourusername/bias-buster.git
cd bias-buster
```
### Install dependencies

    pip install pandas
    pip install numpy
    pip install scikit-learn
    pip install matplotlib
    pip install seaborn
### Run the project

    python main.py

## Applications

Bias Buster can be used in industries where **fair decision making is critical**, such as:

- Hiring and recruitment systems
- Credit scoring models
- Insurance risk assessment
- Loan approval systems
- Healthcare predictions


## Future Improvements

- Integrate **Fairlearn** or **IBM AI Fairness 360**
- Add support for **deep learning models**
- Build a **visual fairness dashboard**
- Automate **bias detection pipelines**
- Deploy **fairness monitoring for production AI systems**
