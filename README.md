# 🩺 Diabetes Risk Prediction using Machine Learning

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Complete-success.svg)

*Leveraging Machine Learning to identify diabetes risk early and save lives*

[Overview](#-overview) • [Features](#-features) • [Dataset](#-dataset) • [Installation](#-installation) • [Results](#-results) • [Contributing](#-contributing)

</div>

---

## 📋 Overview

Diabetes is a growing global health crisis affecting millions worldwide. Early detection is crucial for effective management and prevention of serious complications like heart disease, nerve damage, and kidney failure. This project uses **Machine Learning** to predict diabetes risk based on key medical indicators, enabling proactive healthcare interventions.

### 🎯 Project Objectives

- Build an accurate ML model to predict diabetes risk in individuals
- Identify key medical indicators contributing to diabetes development
- Provide early warning systems for at-risk populations, especially pregnant women
- Achieve high precision and recall to minimize false negatives

### 💡 Motivation

Inspired by personal experiences with gestational diabetes, this project aims to better understand diabetes patterns and use data-driven approaches to help identify at-risk individuals before serious complications arise.

---

## ✨ Features

- 📊 **Comprehensive EDA** - In-depth exploratory data analysis with beautiful visualizations
- 🧹 **Advanced Data Preprocessing** - Handling missing values, outliers, and feature scaling
- 🤖 **Machine Learning Models** - Decision Tree classifier with hyperparameter tuning
- 📈 **Performance Metrics** - Detailed evaluation using accuracy, precision, recall, and F1-score
- 🎨 **Interactive Visualizations** - Distribution plots, correlation heatmaps, and confusion matrices
- 📝 **Comprehensive Documentation** - Well-documented code with detailed explanations

---

## 📊 Dataset

The project uses the **Pima Indians Diabetes Dataset** containing medical data from female patients.

### Dataset Features:

| Feature | Description |
|---------|-------------|
| **Pregnancies** | Number of times pregnant |
| **Glucose** | Plasma glucose concentration (2-hour oral glucose tolerance test) |
| **BloodPressure** | Diastolic blood pressure (mm Hg) |
| **SkinThickness** | Triceps skinfold thickness (mm) |
| **Insulin** | 2-Hour serum insulin (mu U/ml) |
| **BMI** | Body mass index (weight in kg/(height in m)²) |
| **DiabetesPedigreeFunction** | Family history score for diabetes likelihood |
| **Age** | Age in years |
| **Outcome** | Target variable (0 = Not Diabetic, 1 = Diabetic) |

**Dataset Size:** 768 samples  
**Source:** [Kaggle - Diabetes Dataset](https://www.kaggle.com/datasets/saurabh00007/diabetescsv)

---

## 🚀 Installation

### Prerequisites

- Python 3.8 or higher
- pip package manager
- Jupyter Notebook or JupyterLab

### Setup Instructions

1. **Clone the repository**
```bash
git clone https://github.com/uzair300303/Diabetes-Risk-Prediction-using-Machine-Learning.git
cd Diabetes-Risk-Prediction-using-Machine-Learning
```

2. **Create a virtual environment (recommended)**
```bash
python -m venv env
```

3. **Activate the virtual environment**
- Windows:
  ```bash
  env\Scripts\activate
  ```
- macOS/Linux:
  ```bash
  source env/bin/activate
  ```

4. **Install required packages**
```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

5. **Launch Jupyter Notebook**
```bash
jupyter notebook
```

6. **Open and run the notebook**
   - Open `UzairSunkad_1RVU22CSE182.ipynb`
   - Run all cells sequentially

---

## 🔍 Methodology

### 1. Data Exploration & Preprocessing
- Statistical analysis of all features
- Identification and treatment of missing values (encoded as 0)
- Outlier detection using box plots and distribution analysis
- Feature correlation analysis

### 2. Data Visualization
- Distribution plots for each feature
- Correlation heatmap to identify feature relationships
- Box plots for outlier detection
- Count plots for target variable distribution

### 3. Feature Engineering
- Standard scaling of numerical features
- Train-test split (80-20 ratio)
- Feature importance analysis

### 4. Model Building
- **Algorithm:** Decision Tree Classifier
- **Initial Training:** Baseline model evaluation
- **Hyperparameter Tuning:**
  - `max_depth = 5` - Prevents overfitting
  - `min_samples_leaf = 10` - Ensures generalization

### 5. Model Evaluation
- Accuracy, Precision, Recall, F1-Score
- Confusion matrices for both training and test sets
- Performance comparison before and after tuning

---

## 📈 Results

### Model Performance (After Hyperparameter Tuning)

| Metric | Training Set | Test Set |
|--------|-------------|----------|
| **Accuracy** | 83.43% | 72.73% |
| **Precision** | 84.00% | 73.20% |
| **Recall** | 83.40% | 72.70% |
| **F1-Score** | 83.60% | 72.90% |

### Key Insights 🔑

1. **Most Important Features:**
   - 🥇 **Glucose** - Primary indicator of diabetes risk
   - 🥈 **Age** - Significant factor, especially for women over 28
   - 🥉 **BMI** - Critical indicator, particularly when BMI > 28.5

2. **Risk Profiles Identified:**
   - **Lower Risk:** Glucose ≤ 127, Age ≤ 28
   - **Higher Risk:** Glucose > 100, Age > 28, or BMI > 28.5

3. **Model Performance:**
   - Successfully reduced overfitting through hyperparameter tuning
   - Improved generalization to unseen data
   - Balanced performance across all metrics

---

## 📁 Project Structure

```
Diabetes-Risk-Prediction/
│
├── UzairSunkad_1RVU22CSE182.ipynb    # Main Jupyter notebook
├── diabetes.csv                       # Dataset file
├── diabetes-risk-prediction.html     # HTML export of notebook
├── README.md                          # Project documentation
│
├── archive/                           # Additional datasets
│   ├── 2020-2021.csv
│   ├── 2021-2022.csv
│   ├── final_dataset.csv
│   └── Datasets/
│
└── env/                               # Virtual environment (gitignored)
```

---

## 🛠️ Technologies Used

<div align="center">

| Technology | Purpose |
|------------|---------|
| ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) | Core programming language |
| ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) | Data manipulation and analysis |
| ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white) | Numerical computations |
| ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white) | Machine learning algorithms |
| ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat&logo=python&logoColor=white) | Data visualization |
| ![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat&logo=python&logoColor=white) | Statistical visualizations |
| ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white) | Interactive development environment |

</div>

---

## 🎯 Future Enhancements

- [ ] Implement additional ML algorithms (Random Forest, Gradient Boosting, XGBoost)
- [ ] Perform ensemble learning for improved predictions
- [ ] Create a web application for real-time predictions
- [ ] Expand dataset with more diverse population samples
- [ ] Add SHAP values for better model interpretability
- [ ] Implement cross-validation for more robust evaluation
- [ ] Create a REST API for model deployment
- [ ] Add feature for personalized health recommendations

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve this project:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Uzair Sunkad**  
Roll No: 1RVU22CSE182

- GitHub: [@uzair300303](https://github.com/uzair300303)
- Project Link: [Diabetes Risk Prediction](https://github.com/uzair300303/Diabetes-Risk-Prediction-using-Machine-Learning)

---

## 🙏 Acknowledgments

- Dataset source: [Kaggle - Diabetes Dataset](https://www.kaggle.com/datasets/saurabh00007/diabetescsv)
- Inspired by the need to better understand and predict diabetes in at-risk populations
- Special thanks to all healthcare professionals working on diabetes research

---

## 📞 Contact

For questions or suggestions, please open an issue or reach out via GitHub.

---

<div align="center">

**⭐ If you found this project helpful, please consider giving it a star!**

Made with ❤️ and Python

</div>
