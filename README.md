# 🌸 Iris Flower Classification

## 📌 Project Overview

This project demonstrates a complete **Machine Learning classification workflow** using the famous **Iris Flower dataset**.

The objective is to build a machine learning model that can predict the species of an iris flower based on its physical measurements.

The three target species are:

* **Setosa**
* **Versicolor**
* **Virginica**

The project uses Python and popular machine learning and data visualization libraries.

---

## 🎯 Objective

The main objective is to train and evaluate machine learning classification models that can identify the species of an iris flower using:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

---

## 🛠️ Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**
* **UV** for Python environment and dependency management

---

## 📂 Project Structure

```text
iris-flower-classification/
│
├── iris_classification.ipynb
├── requirements.txt
├── README.md
└── .venv/
```

> `.venv/` is the local virtual environment and normally should not be uploaded to GitHub.

---

## 📊 Dataset

The Iris dataset is built directly into **scikit-learn**, so no external dataset download is required.

The dataset contains:

* **150 samples**
* **4 numerical features**
* **3 target classes**
* **50 samples per species**

### Features

| Feature      | Description         |
| ------------ | ------------------- |
| Sepal Length | Length of the sepal |
| Sepal Width  | Width of the sepal  |
| Petal Length | Length of the petal |
| Petal Width  | Width of the petal  |

### Target Classes

| Value | Species    |
| ----: | ---------- |
|     0 | Setosa     |
|     1 | Versicolor |
|     2 | Virginica  |

---

## 🔍 Exploratory Data Analysis

The notebook performs the following EDA:

* Dataset shape
* Column information
* Data types
* Missing/null value checking
* Descriptive statistics
* Species distribution

### Visualizations

The project includes:

* Species distribution plot
* Pairplot showing relationships between features
* Box plots for individual features

These visualizations help understand the distribution of the data and identify relationships between features and species.

---

## 🔬 Feature Selection

The EDA indicates that **petal length** and **petal width** are among the most discriminative features.

They provide strong separation between the three Iris species.

However, all four available features are used for model training:

```text
Sepal Length
Sepal Width
Petal Length
Petal Width
```

---

## 🤖 Machine Learning Models

Two classification algorithms are trained and evaluated.

### 1. Logistic Regression

Logistic Regression is used as a baseline classification model.

The features are standardized using `StandardScaler` before training.

### 2. K-Nearest Neighbours (KNN)

KNN classifies an observation based on the classes of its nearest training samples.

Feature scaling is also applied before training the KNN model.

### Optional Model

A **Decision Tree Classifier** can also be included for additional model comparison.

---

## 🧪 Train/Test Split

The dataset is divided into:

* **80% training data**
* **20% testing data**

The split uses `random_state=42` for reproducibility and `stratify=y` to maintain the class distribution.

---

## 📈 Model Evaluation

Each model is evaluated using:

### Accuracy

Measures the percentage of correctly classified samples.

### Confusion Matrix

Shows the number of correct and incorrect predictions for each species.

### Classification Report

The classification report provides:

* Precision
* Recall
* F1-score
* Support

---

## 🏆 Best Model

The best-performing model is selected based on its performance on the **test dataset**.

The notebook compares the accuracy of the trained models and identifies the model with the highest test accuracy.

The final model should not be declared in advance. It should be selected based on the actual evaluation results produced when the notebook is executed.

---

## 🚀 Installation

This project uses **UV** to manage the Python environment.

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd iris-flower-classification
```

### 2. Create a virtual environment

```bash
uv venv
```

### 3. Activate the environment

On Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```bash
uv pip install -r requirements.txt
```

### 5. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
iris_classification.ipynb
```

---

## 📦 Requirements

The project dependencies are listed in `requirements.txt`.

```text
numpy
pandas
scikit-learn
matplotlib
seaborn
jupyter
notebook
ipykernel
```

---

## ▶️ How to Run

1. Create and activate the UV environment.
2. Install the required dependencies.
3. Start Jupyter Notebook.
4. Open `iris_classification.ipynb`.
5. Run the notebook cells from top to bottom.
6. Review the EDA visualizations.
7. Compare the machine learning models.
8. Identify the best-performing model.

---

## 📚 Machine Learning Workflow

```text
Load Iris Dataset
       ↓
Data Exploration
       ↓
Check Missing Values
       ↓
Descriptive Statistics
       ↓
Data Visualization
       ↓
Feature Analysis
       ↓
Train/Test Split
       ↓
Feature Scaling
       ↓
Train Models
       ↓
Make Predictions
       ↓
Evaluate Models
       ↓
Compare Performance
       ↓
Select Best Model
```

---

## 💡 Key Findings

* The Iris dataset contains **150 samples**.
* There are **three flower species**.
* The dataset contains **four numerical features**.
* There are no missing values.
* Petal measurements provide particularly strong separation between species.
* Logistic Regression and KNN can both perform very well on this dataset.
* The final model is selected based on test-set performance.

---

## 👨‍💻 Author

**Naveed Anwer Khan**

Machine Learning / AI Project

---

## 📄 License

This project is created for **educational and learning purposes**.
