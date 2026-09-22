# Machine Learning Experiments

A hands-on laboratory for studying **Machine Learning, model evaluation, hyperparameters, and generalization** through practical experiments.

The project uses small datasets to test different algorithms and observe how changes in models and hyperparameters affect their performance.

## Objectives

* Understand how different Machine Learning algorithms behave.
* Study and compare model evaluation metrics.
* Understand the relationship between model complexity and generalization.
* Identify **overfitting** and **underfitting**.
* Experiment with different hyperparameters.
* Compare models using consistent evaluation procedures.
* Study **cross-validation**.
* Learn hyperparameter tuning and model selection techniques.
* Develop the ability to interpret experimental results rather than simply comparing metrics.

## Experiment Workflow

Each experiment generally follows this workflow:

```text
Dataset
   ↓
Exploratory Data Analysis
   ↓
Preprocessing
   ↓
Train / Validation / Test Split
   ↓
Baseline
   ↓
Model Training
   ↓
Evaluation
   ↓
Hyperparameter Experiments
   ↓
Model Comparison
   ↓
Cross-Validation
   ↓
Model Selection
   ↓
Final Evaluation on Test Set
```

The **test set** will remain isolated during the experimentation process and will only be used for the final evaluation of the selected model.

## Models

The initial experiments will focus on classification algorithms, including:

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)

Additional algorithms may be added as the project evolves.

## Evaluation Metrics

The main evaluation metrics will include:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* ROC-AUC, when applicable

Beyond recording metric values, each experiment will include an interpretation of **why the model's performance changed**.

## Hyperparameters

Experiments will be performed by modifying relevant hyperparameters for each model.

Examples:

### KNN

* `n_neighbors`
* `weights`
* `metric`

### Decision Tree

* `max_depth`
* `min_samples_split`
* `min_samples_leaf`
* `criterion`

### Random Forest

* `n_estimators`
* `max_depth`
* `min_samples_split`
* `min_samples_leaf`
* `max_features`

### SVM

* `C`
* `kernel`
* `gamma`

### Logistic Regression

* `C`
* `penalty`
* `solver`

The goal is not simply to find the configuration with the highest score, but to understand **how each hyperparameter affects model behavior and generalization**.

## Experiment Tracking

Experiment results will be recorded in a structured table containing information such as:

| Model         | Hyperparameters | Accuracy | Precision | Recall | F1 | Observations |
| ------------- | --------------- | -------: | --------: | -----: | -: | ------------ |
| KNN           | `n_neighbors=3` |        - |         - |      - |  - | -            |
| Random Forest | `max_depth=3`   |        - |         - |      - |  - | -            |
| SVM           | `C=1`           |        - |         - |      - |  - | -            |

The experiment history will be stored in `experiments.csv`, allowing results to persist across notebook sessions.

## Datasets

### 1. Iris

The first dataset used in the project will be the **Iris dataset**, as its small size makes it suitable for quickly experimenting with different algorithms, evaluation methods, and hyperparameters.

Additional datasets will be introduced later to apply the concepts to more realistic problems.

## Technologies

* Python
* Jupyter Notebook
* NumPy
* Pandas
* Matplotlib
* Scikit-learn

## Project Structure

```text
machine-learning-experiments/
│
├── experiments.ipynb
├── experiments.csv
├── README.md
│
└── data/
    └── ...
```

## Roadmap

* [ ] Explore the Iris dataset
* [ ] Establish a baseline
* [ ] Implement initial models
* [ ] Compare evaluation metrics
* [ ] Study overfitting and underfitting
* [ ] Experiment with hyperparameters
* [ ] Add visualizations
* [ ] Study feature scaling
* [ ] Implement cross-validation
* [ ] Study Grid Search
* [ ] Study Randomized Search
* [ ] Perform final evaluation on the test set
* [ ] Repeat experiments with more complex datasets

---

> **Main goal:** not only to find which model performs better, but to understand **why** its performance changes when the model, data, or hyperparameters are modified.
