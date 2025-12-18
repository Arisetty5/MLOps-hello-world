# 🚀 CI/CD for Automated Model Training (MLOps Project)

This repository demonstrates a **basic MLOps CI pipeline** where model training is fully automated using **GitHub Actions**.  
The goal of this project is to show how **MLOps engineers support data scientists** by automating repetitive tasks such as environment setup, model training, and artifact management.


---

## 📌 Project Overview

Whenever code is pushed or a pull request is raised to the `main` branch, a CI pipeline is triggered that:

- Sets up a Python environment
- Installs project dependencies
- Trains the machine learning model
- Saves trained model and evaluation metrics
- Uploads these artifacts for reproducibility and traceability

This ensures that **model training is consistent, automated, and reproducible**.

---

## 🛠️ Tech Stack

- **Python**: 3.10.12  
- **CI/CD**: GitHub Actions  
- **ML Libraries**: As defined in `requirements.txt`  
- **Artifact Storage**: GitHub Actions Artifacts  

---

## 🔁 CI Workflow Details

### Workflow Trigger
The pipeline runs automatically on:
- `push` to the `main` branch
- `pull_request` to the `main` branch

### Workflow Steps
1. Checkout repository code  
2. Set up Python environment  
3. Upgrade `pip`, `setuptools`, and `wheel`  
4. Install project dependencies  
5. Train the ML model  
6. Save model artifacts  
7. Upload artifacts to GitHub Actions  

---