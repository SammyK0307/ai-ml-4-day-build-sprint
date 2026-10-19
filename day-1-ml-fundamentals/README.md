# Exam Score Predictor using Linear Regression

A beginner-friendly Machine Learning project that predicts exam scores based on study hours using Linear Regression.

## 🎯 Objective

Understand how a regression model learns the relationship between an input feature and a numerical target, then uses that relationship to make predictions.

## 🛠️ Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 📊 Dataset

This project uses a small, illustrative dataset containing 19 observations.

- **Input feature:** Hours studied
- **Target variable:** Exam score (out of 100)

The data is synthetic and is intended for educational purposes, not real-world student performance prediction.

## ⚙️ Workflow

1. Create and inspect the dataset.
2. Visualize the relationship between study hours and scores.
3. Split the data into training and testing sets.
4. Train a Linear Regression model.
5. Evaluate predictions using MAE and R².
6. Visualize the regression line.
7. Predict the score for a new input.

## 📈 Results

The notebook reports the model's Mean Absolute Error (MAE) and R² score on the held-out test set.

Run the notebook to reproduce the results.

## 🧠 Key Learnings

- Features and target variables
- Exploratory Data Analysis
- Linear Regression and its equation
- Training vs. testing data
- Prediction errors and evaluation metrics
- The limitations of extrapolating beyond the training data

## ⚠️ Limitations

- The dataset is very small and synthetic.
- Only one feature is used for prediction.
- Evaluation metrics from four test observations are highly uncertain.
- Predictions are constrained to the 0–100 range for this demonstration; this does not guarantee accuracy.

## 🚀 Future Improvements

- Use a larger, more representative dataset.
- Compare Linear Regression with other regression algorithms.
- Add more relevant input features.
- Evaluate performance using cross-validation.
- Build a simple interactive prediction interface.

## 👨‍💻 Author

Created as part of my four-day AI/ML mini-project sprint to learn, build, and share practical Machine Learning concepts.


## Project 02: Gradient Descent Visualizer

### Overview
This project demonstrates how Gradient Descent optimizes a Linear Regression model by repeatedly updating its parameters to reduce prediction error.

### Concepts
- Linear Regression from scratch
- Mean Squared Error (MSE)
- Gradient calculation
- Learning rate
- Parameter optimization
- Convergence and divergence

### Implementation
The model uses NumPy to calculate gradients and update the slope and intercept over multiple iterations. Matplotlib visualizes the loss curve, the fitted regression line, and the effect of different learning rates.

### Visualizations
- `gradient_descent_loss.png`: Shows how the model's error changes during training.
- `gradient_descent_comparison.png`: Compares the model before and after training.
- `learning_rate_comparison.png`: Demonstrates how learning rates affect convergence.

### Key Learning
Gradient Descent can improve a model by iteratively updating its parameters in the direction that reduces the cost function. An unsuitable learning rate can make training inefficient or unstable.

### Limitations
This is an educational demonstration using a small synthetic dataset. The results illustrate optimization behavior and do not establish real-world predictive performance.

### Technologies
Python, NumPy, Matplotlib, Jupyter Notebook

## Project 03: Student Pass/Fail Predictor

### Overview
A beginner-friendly binary classification project that predicts a student's Pass/Fail label using study hours and attendance percentage.

### Technologies
- Python
- NumPy and Pandas
- Matplotlib
- Scikit-learn
- Logistic Regression

### Workflow
1. Generate and inspect a synthetic student dataset.
2. Visualize the Pass and Fail classes.
3. Split the dataset into training and testing sets.
4. Scale features and train Logistic Regression.
5. Predict class labels and estimated pass probabilities.
6. Evaluate performance using classification metrics and a confusion matrix.
7. Visualize the model's decision boundary.

### Test Results
- Test samples: 24
- Correct predictions: 21
- Incorrect predictions: 3
- Observed test accuracy: 87.50%

These results are from a small synthetic dataset and should not be interpreted as real-world academic predictions.

### Visualizations
- `student_pass_fail_distribution.png`
- `student_pass_fail_confusion_matrix.png`
- `student_pass_fail_decision_boundary.png`

### Key Learnings
- The difference between regression and classification
- Feature scaling and Logistic Regression
- Class probabilities and decision thresholds
- Accuracy, precision, recall, and F1-score
- Confusion matrices and decision boundaries

### Limitations
The dataset is synthetic and contains only 120 observations. The model uses two features and has been evaluated on just 24 test samples. Its estimated probabilities are not validated for real student outcomes.

### Future Improvements
- Experiment with different classification algorithms.
- Compare performance using cross-validation.
- Investigate incorrect predictions.
- Build an interactive interface for exploring predictions.