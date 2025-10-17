# 🩺 Osteoporosis Prediction Dataset Description

The dataset used in this project is a **modified version of a publicly available medical dataset** curated for educational and research purposes related to **osteoporosis risk prediction**.
It contains anonymized patient-level health, lifestyle, and clinical attributes relevant to bone density and fracture risk assessment.
All personal identifiers have been removed to maintain confidentiality and compliance with ethical data use standards.

---

## 📊 Data Fields

| **Column Name**         | **Type**   | **Description**                                                                                 |
| ----------------------- | ---------- | ----------------------------------------------------------------------------------------------- |
| **Id**                  | Identifier | Unique patient identifier                                                                       |
| **Age**                 | Attribute  | Patient’s age in years                                                                          |
| **Gender**              | Attribute  | Biological sex of the patient (Male/Female)                                                     |
| **Hormonal Changes**    | Attribute  | Indicates presence or absence of hormonal changes (e.g., postmenopausal status)                 |
| **Family History**      | Attribute  | Whether the patient has a family history of osteoporosis or fractures (Yes/No)                  |
| **Race/Ethnicity**      | Attribute  | Patient’s racial or ethnic background                                                           |
| **Body Weight**         | Attribute  | Weight classification (Underweight / Normal / Overweight / Obese)                               |
| **Calcium Intake**      | Attribute  | Daily calcium intake level (Low / Adequate / High)                                              |
| **Vitamin D Intake**    | Attribute  | Estimated Vitamin D intake or sufficiency level                                                 |
| **Physical Activity**   | Attribute  | Activity level (Sedentary / Moderate / Active)                                                  |
| **Smoking**             | Attribute  | Smoking habit indicator (Yes/No)                                                                |
| **Alcohol Consumption** | Attribute  | Frequency or intensity of alcohol intake (None / Moderate / High)                               |
| **Medical Conditions**  | Attribute  | Pre-existing conditions affecting bone metabolism (e.g., Rheumatoid Arthritis, Hyperthyroidism) |
| **Medications**         | Attribute  | Medications currently in use that may influence bone density (e.g., Corticosteroids)            |
| **Prior Fractures**     | Attribute  | History of prior bone fractures (Yes/No)                                                        |
| **Osteoporosis**        | **Target** | Binary indicator of osteoporosis diagnosis (1 = Positive, 0 = Negative)                         |

---

### ⚠️ Missing Attribute Values

Yes — some attributes contain missing or `NaN` values due to incomplete medical histories or unavailable records.

---

### 💡 Usage

This dataset is intended for **predictive modeling and analysis** of osteoporosis risk using machine learning techniques such as logistic regression, random forests, and gradient boosting.
It supports feature engineering, exploratory data analysis (EDA), and model evaluation focused on understanding the relationship between lifestyle, hormonal, and medical factors with bone health outcomes.
