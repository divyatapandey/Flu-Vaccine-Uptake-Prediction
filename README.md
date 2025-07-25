# 🧬 Flu Vaccine Prediction

A multilabel classification machine learning project to predict whether individuals received **seasonal** and **xyz (H1N1)** flu vaccines. The model uses behavioral, demographic, and opinion-based features to estimate the probability of vaccination.

---

## 📌 Problem Description

The goal is to predict how likely individuals are to receive their **xyz** and **seasonal flu** vaccines. Specifically, you'll be predicting **two probabilities**:
- One for `xyz_vaccine`
- One for `seasonal_vaccine`

### 🎯 Labels

There are two binary target variables:
- `xyz_vaccine`: Whether the respondent received the xyz (H1N1) flu vaccine (0 = No, 1 = Yes)
- `seasonal_vaccine`: Whether the respondent received the seasonal flu vaccine (0 = No, 1 = Yes)

This is a **multilabel classification problem**, not multiclass. A respondent may receive:
- None
- One
- Or both vaccines.

---

## 🧾 Dataset

⚠️ **Note:** The dataset used in this project is **not publicly available online** and was provided as part of a private hackathon. Therefore, it is not included in this repository.

### 💡 Features

The dataset contains **36 columns**:
- `respondent_id`: Unique identifier
- 35 features including:
  - Levels of concern, knowledge, and opinions about flu
  - Behavioral habits (mask usage, hand washing, social distancing, etc.)
  - Doctor recommendations
  - Health status and chronic conditions
  - Demographic data (age, sex, race, income, employment, education, etc.)

Example variables:
- `xyz_concern` (0–3): Level of concern about xyz flu
- `xyz_knowledge` (0–2): Level of knowledge about xyz flu
- `behavioral_avoidance`, `behavioral_face_mask` (binary)
- `opinion_xyz_vacc_effective`, `opinion_seas_vacc_effective` (1–5)
- `age_group`, `education`, `race`, `income_poverty`, etc.

---

## 🛠️ System Requirements

Python 3.7 or above. Install dependencies using:

```bash
pip install -r requirements.txt
