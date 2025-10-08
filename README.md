## CSCN8030 – Assignment 2

## Rapid Prototyping With and Without Generative AI Tools

---

## Project Overview

Hospitals face major challenges in managing Operating Room (OR) schedules due to unpredictable surgery durations, emergencies, and growing backlogs.  
This project uses AI to **predict actual surgery duration** based on booked time, service type, and other operational features.

Two AI prototypes were built and compared:

1. **Prototype A – Without Generative AI**

   - Traditional machine learning pipeline
   - Features: `Booked Time (min)`, `Service`, `OR Suite`
   - Model: `RandomForestRegressor`

2. **Prototype B – With Generative AI**
   - Incorporates _Generative-AI-assisted_ feature engineering and synthetic data augmentation
   - Added features: `weekday`, `month`, `is_morning`, `setup_minutes`, `exit_minutes`
   - Uses synthetic “long-surgery” samples inspired by AI-assisted data expansion

---

## 📂 Project Structure

# Assignment 2 Directory Structure

```plaintext
assignment2/
│
├── 2022_Q1_OR_Utilization.csv       # OR dataset (Q1 2022)
├── notebooks/
│   ├── Prototype_A_WithoutGenAI.ipynb   # Traditional ML notebook
│   └── Prototype_B_WithGenAI.ipynb # GenAI-assisted notebook
├── models/
│   ├── prototype_A_no_genai_model.pkl
│   └── prototype_B_with_genai_model.pkl
└── README.md                        # Project documentation
│
├── requirements.txt
├── .gitignore

```

---

## Setup Instructions

### 1️. Create and activate a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate   # (Linux/Mac)
```

### 2. Install the requirements

```bash
pip install -r requirements.txt
```
