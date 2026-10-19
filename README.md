# AI/ML: 4-Day Build Sprint 🚀

A hands-on Machine Learning learning series focused on building small projects, understanding algorithms, and visualizing how models learn.

This repository documents my journey from fundamental Machine Learning algorithms to neural networks and modern deep learning.

## 📅 Day 1 — Machine Learning Fundamentals

### Project 1: Exam Score Predictor
**Algorithm:** Linear Regression

Predicts exam scores from study hours using a simple regression model.

**Concepts:** Features, targets, train/test splitting, predictions, MAE, and R².

### Project 2: Gradient Descent Visualizer
**Algorithm:** Gradient Descent implemented using NumPy

Demonstrates how a model learns its slope and intercept by repeatedly reducing its prediction error.

**Concepts:** Cost functions, gradients, learning rates, parameter updates, and convergence.

The training MSE decreased from approximately 519.85 to 0.75 on the illustrative dataset.

### Project 3: Student Pass/Fail Predictor
**Algorithm:** Logistic Regression

Classifies synthetic student records using study hours and attendance.

**Concepts:** Classification, feature scaling, class probabilities, precision, recall, F1-score, confusion matrices, and decision boundaries.

The model achieved 87.5% accuracy on a held-out test set of 24 synthetic observations.

## 🛠️ Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- VS Code

## 📂 Repository Structure

- `day-1-ml-fundamentals/` — Regression, optimization, and classification
- `day-2-classical-ml/` — Classical Machine Learning experiments
- `day-3-neural-networks/` — Clustering, dimensionality reduction, and neural networks
- `day-4-advanced-deep-learning/` — CNNs, sequence models, and transformers

The later phases are planned and will be added as they are completed.

## 🚀 Getting Started

Clone the repository, create a virtual environment, and install the dependencies.

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

Open a project notebook in VS Code and select the Python environment for your Jupyter kernel.

## 📌 Important Note

The initial projects use small synthetic datasets for educational purposes. Their results illustrate how the algorithms work and should not be interpreted as validated real-world predictions.

## 🎯 Goal

Learn Machine Learning by building, experimenting, visualizing results, documenting limitations, and sharing each project.

More projects will be added throughout the four-day sprint.