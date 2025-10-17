# 🧠 Osteoporosis Risk Prediction – Full Stack ML Pipeline

## Predicting Osteoporosis Risk through End-to-End Machine Learning with FastAPI Deployment

---

## 🚀 Overview

This repository contains a **complete end-to-end machine learning pipeline** for **osteoporosis risk prediction**, built with a focus on **feature engineering before preprocessing**, **reproducible environments**, and **deployment-ready architecture**.

The project leverages **Python**, **scikit-learn**, and **FastAPI**, using **`uv`** for environment management and dependency locking.

---

### Notebook size too big for GitHub?

- Preview here on Google Collab [osteoporosis.ipynb](https://colab.research.google.com/github/D0nG4667/osteoporosis_prediction_full_stack/blob/main/dev/notebooks/osteoporosis.ipynb)

## 🧩 Key Features

* 🔬 **Feature Engineering before Preprocessing**

  * Domain-driven feature creation and transformation before scaling or encoding.
  * Handles categorical, numerical, and derived medical indicators for enhanced model accuracy.

* ⚙️ **Preprocessing & Modeling**

  * Modular data pipeline with standardization, encoding, and imputation.
  * Multiple model benchmarking with F1-score, precision, and recall comparisons.

* 🧱 **Clean Project Architecture**

  * Clear separation of data, models, utils, and API.
  * Environment-specific configuration for offline/online and notebook use.

* ⚡ **FastAPI Integration**

  * Real-time model inference API with async endpoints.

* 📦 **Reproducible Dependency Management** with `uv`

  * Fast installs, isolated environments, and lockfile tracking (`uv.lock`).

---

## 🗂️ Project Folder Structure

```markdown
### Project folder structure

- .venv/
- data/
  └── README.md
- models/
  └── notebooks/
- plots/
- env/
  ├── .online.env
  ├── .offline.env
  └── .notebook.env
- src/
  ├── api/
  └── client/
- utils/
- LICENSE
- pyproject.toml
- README.md
- requirements.txt
- uv.lock
```

### 🧱 Folder Responsibilities

| Folder / File         | Description                                                              |
| --------------------- | ------------------------------------------------------------------------ |
| **data/**             | Raw and cleaned datasets, including structured data for experimentation. |
| **models/**           | Trained model binaries and saved weights.                                |
| **models/notebooks/** | Jupyter notebooks for EDA and feature exploration.                       |
| **plots/**            | Saved visualizations for reports and presentations.                      |
| **env/**              | Environment-specific configuration files (.env variants).                |
| **src/api/**          | FastAPI app for model inference and deployment.                          |
| **src/client/**       | API client or frontend integration utilities.                            |
| **utils/**            | Helper scripts for preprocessing, logging, and metrics.                  |
| **main.py**           | Project entry point for orchestration or CLI.                            |
| **pyproject.toml**    | Project metadata and dependency definitions (for uv).                    |
| **requirements.txt**  | Backward-compatible dependency list.                                     |
| **uv.lock**           | Frozen dependency lockfile for reproducibility.                          |

---

## 🧪 Pipeline Architecture

### 1️⃣ Feature Engineering

* Generate medically relevant features before preprocessing.
* Handle compound variables (e.g., hormonal changes, calcium intake, family history).
* Encode derived binary or continuous features for better signal capture.

### 2️⃣ Preprocessing

* Imputation of missing values.
* Encoding categorical variables.
* Standardization and scaling.
* Splitting into training, validation, and test sets.

### 3️⃣ Modeling

* Model training using Logistic Regression, Random Forest, and XGBoost.
* Grid search and cross-validation for hyperparameter optimization.
* Evaluation using F1-score and confusion matrix analysis.

### 4️⃣ Deployment

* Model serialized with `joblib`.
* Exposed via FastAPI endpoints for inference.
* Ready for containerization (Docker optional).

---

## ⚙️ Environment Setup (Using `uv`)

### 🧰 Prerequisites

* Python ≥ 3.10
* [`uv`](https://github.com/astral-sh/uv) – a fast, modern Python package manager

### 🪄 Setup Steps

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/osteoporosis-prediction.git
cd osteoporosis-prediction

# 2. Create and activate the environment
uv venv
source .venv/bin/activate  # or .venv\Scripts\activate on Windows

# 3. Install dependencies
uv sync
or
uv pip install .
or 
uv pip install -r requirements.txt
```

## 🧠 Evaluation Metrics

| Metric        | Description                                                        |
| ------------- | ------------------------------------------------------------------ |
| **Precision** | Correctly predicted positive cases out of all predicted positives. |
| **Recall**    | Correctly predicted positives out of all actual positives.         |
| **F1-Score**  | Harmonic mean of precision and recall for balanced evaluation.     |
| **Accuracy**  | Overall correctness of the model predictions.                      |

---

## 📊 Visualization Samples

* Correlation heatmaps for feature relationships
* Age distribution vs. risk
* Confusion matrix visualization for model comparison

All plots are stored in the `/plots` directory.

---

## 🧾 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more information.

---

## 🤝 Contributions

Contributions, bug reports, and feature suggestions are welcome!
To contribute:

```bash
# Create a new branch
git checkout -b feature/your-feature-name

# Commit your changes
git commit -m "feat: add new preprocessing feature"

# Push and open a pull request
git push origin feature/your-feature-name
```

---

## 📬 Contact

**Author:** Gabriel Okundaye

**Role:** Data & AI Consultant

**LinkedIn:** [Gabriel Okundaye](https://www.linkedin.com/in/dr-gabriel-okundaye/)

---

## ⭐️ Show your support

If you like this project kindly show some love, give it a 🌟 **STAR** 🌟. Thank you!

## 📝 License

This project is [MIT](/LICENSE) licensed.
