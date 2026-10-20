# 🚀 AI/ML: 4-Day Build Sprint

A hands-on Machine Learning project series focused on understanding algorithms through implementation, experimentation, and visualization.

The goal is to strengthen my foundations in AI/ML by building small, practical projects — progressing from regression and optimization to ensemble learning and model evaluation.

## 📚 Project Roadmap

| Day | Focus | Projects | Status |
|---|---|---:|---|
| Day 1 | ML Fundamentals | 3 | ✅ Completed |
| Day 2 | Classical Machine Learning | 3 | ✅ Completed |
| Day 3 | Neural Networks | 3 planned | 🔜 Upcoming |
| Day 4 | Advanced Deep Learning | 3 planned | 🔜 Upcoming |

---

## 📅 Day 1 — ML Fundamentals

**Focus:** Regression, optimization, and classification.

| Project | Algorithm | What It Covers |
|---|---|---|
| [01. Exam Score Predictor](day-1-ml-fundamentals/01_linear_regression_exam_score.ipynb) | Linear Regression | Prediction, features, targets, MAE, and R² |
| [02. Gradient Descent Visualizer](day-1-ml-fundamentals/02_gradient_descent_visualizer.ipynb) | Gradient Descent | Gradients, cost functions, learning rates, and convergence |
| [03. Student Pass/Fail Predictor](day-1-ml-fundamentals/03_logistic_regression_pass_fail.ipynb) | Logistic Regression | Classification, probabilities, evaluation metrics, and decision boundaries |

### Highlights

- Reduced training Mean Squared Error from approximately **519.85 to 0.75** in the Gradient Descent experiment.
- Achieved **87.5% test accuracy** with Logistic Regression on 24 held-out observations from a synthetic dataset.

📖 **[Explore Day 1 projects and details](day-1-ml-fundamentals/README.md)**

---

## 📅 Day 2 — Classical Machine Learning

**Focus:** Hyperparameter optimization, ensemble learning, and classification evaluation.

| Project | Techniques | What It Covers |
|---|---|---|
| [04. KNN Hyperparameter Lab](day-2-classical-ml/04_knn_hyperparameter_lab.ipynb) | KNN, GridSearchCV, PCA | Feature scaling, cross-validation, and hyperparameter selection |
| [05. Ensemble Learning Benchmark](day-2-classical-ml/05_ensemble_learning_benchmark.ipynb) | Decision Tree, Random Forest, Gradient Boosting | Model comparison, confusion matrices, and feature importance |
| [06. Classification Threshold Dashboard](day-2-classical-ml/06_classification_threshold_dashboard.ipynb) | Random Forest, ROC-AUC, precision–recall analysis | Threshold selection and precision–recall trade-offs |

### Highlights

- Achieved **100% test accuracy** on 36 held-out samples in the KNN experiment.
- Compared three tree-based algorithms using five-fold stratified cross-validation.
- Explored how changing a classification threshold affects precision, recall, and F1-score.

📖 **[Explore Day 2 projects and results](day-2-classical-ml/README.md)**

*All results reflect specific experimental setups and data splits; they are not guarantees of performance on unseen datasets.*

---

## 🛠️ Tech Stack

- **Language:** Python
- **Data Handling:** NumPy, Pandas
- **Visualization:** Matplotlib
- **Machine Learning:** Scikit-learn
- **Environment:** Jupyter Notebook, VS Code
- **Version Control:** Git and GitHub

## 📂 Repository Structure

```text
ai-ml-4-day-build-sprint/
├── README.md
├── requirements.txt
├── .gitignore
│
├── day-1-ml-fundamentals/
│   ├── README.md
│   └── 3 project notebooks and visualizations
│
├── day-2-classical-ml/
│   ├── README.md
│   └── 3 project notebooks and visualizations
│
├── day-3-neural-networks/
│
└── day-4-advanced-deep-learning/
```

The Day 3 and Day 4 folders represent upcoming phases and will be populated as those projects are completed.

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/SammyK0307/ai-ml-4-day-build-sprint.git
cd ai-ml-4-day-build-sprint
```

### 2. Create and activate a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Run the notebooks

Open the repository in VS Code, install the Python and Jupyter extensions if needed, and select the virtual environment as your notebook kernel.

Open any project notebook and run its cells sequentially.

## 🎯 Learning Goals

Through this sprint, I aim to:

- Strengthen my understanding of core ML algorithms.
- Implement models and evaluate them using appropriate metrics.
- Understand optimization, hyperparameter tuning, and generalization.
- Visualize model behavior and communicate experimental findings.
- Progress toward neural networks and modern deep learning.

## 📌 Notes and Limitations

The projects use small public or synthetic datasets for educational experimentation. Performance metrics are specific to the experiments conducted and should not be interpreted as guarantees of real-world performance.

The breast cancer classification projects are educational demonstrations, not clinically validated diagnostic systems.

---

**Learning by building. Improving through experimentation. One project at a time. 🚀**