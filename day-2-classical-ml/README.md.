# Day 2 — Classical Machine Learning

Three hands-on projects exploring **hyperparameter optimization, ensemble learning, and classification evaluation** using Python and Scikit-learn.

## Projects at a Glance

| Project | Key Concepts | Dataset |
|---|---|---|
| [04. KNN Optimization](#project-04-knn-hyperparameter-optimization) | GridSearchCV, cross-validation, PCA | Wine |
| [05. Ensemble Benchmark](#project-05-ensemble-learning-benchmark) | Decision Trees, Random Forest, Gradient Boosting | Breast Cancer Wisconsin |
| [06. Threshold Evaluation](#project-06-classification-threshold-dashboard) | ROC-AUC, precision–recall, threshold tuning | Breast Cancer Wisconsin |

---

## Project 04: KNN Hyperparameter Optimization

**Notebook:** [`04_knn_hyperparameter_lab.ipynb`](04_knn_hyperparameter_lab.ipynb)

### Objective
Investigate how the number of neighbors, distance metric, and neighbor weighting affect a K-Nearest Neighbors classifier.

### Methodology
- Explored the Wine dataset containing 178 samples, 13 features, and 3 classes.
- Standardized features using `StandardScaler`.
- Used PCA to visualize the dataset in two dimensions.
- Tuned hyperparameters using `GridSearchCV` with five-fold stratified cross-validation.
- Evaluated the selected model on a held-out test set.

### Results

| Metric | Result |
|---|---:|
| Optimal neighbors (K) | 7 |
| Distance metric | Manhattan |
| Neighbor weighting | Uniform |
| Cross-validation Macro F1 | 0.9789 |
| Test accuracy | 100% |
| Test Macro F1 | 1.0000 |

The selected configuration achieved perfect classification on the 36-sample test set in this experiment.

**Key learning:** Feature scaling and hyperparameter selection can significantly influence distance-based models. A perfect score on a small test set does not guarantee equally strong performance on new data.

### Visualizations
- [Class distribution](wine_class_distribution.png)
- [PCA projection](wine_pca_visualization.png)
- [Confusion matrix](wine_knn_confusion_matrix.png)
- [Hyperparameter comparison](knn_hyperparameter_comparison.png)

---

## Project 05: Ensemble Learning Benchmark

**Notebook:** [`05_ensemble_learning_benchmark.ipynb`](05_ensemble_learning_benchmark.ipynb)

### Objective
Compare Decision Tree, Random Forest, and Gradient Boosting classifiers using the same data split and validation strategy.

### Methodology
- Used the Breast Cancer Wisconsin Diagnostic dataset: 569 samples and 30 numerical features.
- Applied a stratified 80/20 train/test split.
- Compared the models using five-fold stratified cross-validation.
- Evaluated accuracy, Macro F1, and malignant recall.
- Analyzed test-set confusion matrices and Random Forest feature importance.

### Results

| Model | CV Macro F1 | Test Accuracy | Test Macro F1 | Malignant Recall |
|---|---:|---:|---:|---:|
| Random Forest | 0.9602 | 0.9561 | 0.9526 | 0.9286 |
| Gradient Boosting | 0.9483 | 0.9561 | 0.9521 | 0.9048 |
| Decision Tree | 0.9119 | 0.9123 | 0.9075 | 0.9286 |

Random Forest achieved the highest cross-validation and test Macro F1 scores. Gradient Boosting produced a very similar test result, while the single Decision Tree performed less well overall.

### Top Random Forest Features

| Feature | Importance |
|---|---:|
| `worst perimeter` | 0.1331 |
| `worst area` | 0.1281 |
| `worst concave points` | 0.1081 |
| `mean concave points` | 0.0944 |
| `worst radius` | 0.0906 |

Feature importance reflects how the fitted model uses features for its predictions; it does not establish causation or clinical significance.

### Visualizations
- [Class distribution](cancer_class_distribution.png)
- [Cross-validation comparison](ensemble_cv_comparison.png)
- [Confusion matrices](ensemble_confusion_matrices.png)
- [Random Forest feature importance](random_forest_feature_importance.png)

---

## Project 06: Classification Threshold Dashboard

**Notebook:** [`06_classification_threshold_dashboard.ipynb`](06_classification_threshold_dashboard.ipynb)

### Objective
Explore how classification probability thresholds affect precision, recall, F1-score, and the resulting predictions.

### Methodology
- Used the Breast Cancer Wisconsin Diagnostic dataset.
- Split the data into training, validation, and test sets.
- Trained a Random Forest classifier on the training data.
- Evaluated probability rankings using ROC-AUC and Average Precision.
- Selected a threshold by maximizing validation-set F1-score.
- Compared the default 0.50 threshold with the selected threshold on the held-out test set.

**Positive class:** Malignant  
**Negative class:** Benign

### Validation Results

| Metric | Score |
|---|---:|
| ROC-AUC | 0.992 |
| Average Precision | 0.990 |

These metrics indicate strong class-ranking performance on the validation set for this experiment. Final test-set results are reported separately in the notebook.

### Visualizations
- [ROC curve](threshold_roc_curve.png)
- [Precision–recall curve](threshold_precision_recall_curve.png)
- [Threshold metric comparison](threshold_metric_comparison.png)
- [Test-set confusion matrix comparison](threshold_confusion_matrix_comparison.png)

**Key learning:** The default classification threshold is not always the best choice for a particular objective. Threshold selection changes the balance between false positives and false negatives, so it should reflect the requirements of the application.

---

## Technologies

- Python
- NumPy and Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- VS Code

## How to Run

From the repository root, activate the existing Python virtual environment and install the dependencies:

```bash
source .venv/bin/activate
python -m pip install -r requirements.txt
```

Open the required notebook in VS Code and select the **Python (AI-ML Sprint)** Jupyter kernel.

Run the cells sequentially to reproduce the experiments and visualizations.

## Key Takeaways

Through these projects, I explored:

- Hyperparameter tuning and cross-validation
- Distance-based learning and feature scaling
- Ensemble methods and model comparison
- Feature importance and model interpretation
- ROC-AUC and precision–recall analysis
- Classification threshold selection
- The importance of separating validation from final test evaluation

## Limitations

The results depend on the datasets, random splits, and model configurations used in these experiments. A single test split does not guarantee performance on other data.

The Breast Cancer Wisconsin experiments are for educational model evaluation only. They are **not clinically validated diagnostic systems**.

---

*Part of the [AI/ML 4-Day Build Sprint](../README.md) — learning through implementation, experimentation, and visualization.*