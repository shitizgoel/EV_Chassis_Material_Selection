# 🚘 Material Selection for EV Chassis using Machine Learning

This project explores the suitability of various materials for Electric Vehicle (EV) Chassis using Supervised Machine Learning techniques. By analyzing material properties, the project identifies which materials are most appropriate for EV chassis applications as per the industry standards.

## 📌 Project Overview

🔍 The primary goal of this project is to determine the best materials suitable for EV chassis using their physical and mechanical properties. We apply several supervised machine learning algorithms to classify and evaluate materials for their viability in EV chassis design.

### Workflow:
1. **Data Analysis**  
   - Exploratory Data Analysis (EDA) to understand and visualize material properties  
   - Data cleaning and preprocessing  

2. **Modeling**  
   Applied multiple supervised ML models:
   - Artificial Neural Networks (ANN)
   - Support Vector Machines (SVM)
   - Decision Tree
   - Bagging
   - Random Forest
   - Adaboost    
   - K-Nearest Neighbors (KNN)  
   - Naive Bayes
   - Logistic Regression

3. **Evaluation**  
   Models were evaluated using key metrics:  
   - Accuracy  
   - Precision  
   - Recall  
   - F1 Score  
   - AUC (Area Under the Curve)

---

## 📊 Dataset

The dataset has 1552 rows consisting **material properties** that affect the suitability for EV chassis construction, such as:
- Density
- Ultimate Tensile Strength (UTS)
- Yield Strength
- Elastic Modulus
- Shear Modulus
- Poisson's Ratio

*(We downloaded the dataset from Kaggle - [Dataset Download link](https://www.kaggle.com/datasets/purushottamnawale/materials))*

---

## 🛠️ Libraries Used

- [Pandas](https://pandas.pydata.org/) — for data manipulation and analysis  
- [Matplotlib](https://matplotlib.org/) — for visualizations  
- [Scikit-learn](https://scikit-learn.org/stable/) — for implementing machine learning models and evaluation metrics

---

## 📈 Results

The analysis was performed on a significantly imbalanced dataset (with only 8.69% of data labelled as 'True' materials). Decision tree-based methods, along with ensemble methods like Random Forest and AdaBoost, exhibited robust performance despite this imbalance, showcasing their resilience to skewed class distributions.

Results Table:

| Classifier          | Accuracy | Precision | Recall | F1-Score | ROC AUC |
| ------------------- | -------- | --------- | ------ | -------- | ------- |
| ANN                 | 0.98     | 0.89      | 0.86   | 0.88     | 0.93    |
| SVM                 | 0.96     | 0.77      | 0.69   | 0.73     | 0.84    |
| Decision Tree       | 1.00     | 1.00      | 0.97   | 0.98     | 0.98    |
| Bagged Trees        | 1.00     | 1.00      | 0.97   | 0.98     | 0.98    |
| Random Forest       | 1.00     | 1.00      | 0.97   | 0.98     | 0.98    |
| DT with AdaBoost    | 1.00     | 1.00      | 0.97   | 0.98     | 0.98    |
| KNN                 | 0.98     | 0.87      | 0.90   | 0.88     | 0.94    |
| Naive Bayes         | 0.84     | 0.31      | 0.93   | 0.47     | 0.88    |
| Logistic Regression | 0.88     | 0.39      | 0.93   | 0.55     | 0.91    |


---

## 📂 Project Structure

```plaintext
├── Final_Code.ipynb          # Full Python Code
├── Project_Report.pdf        # Project Report
├── README.md                 # Project documentation
└── requirements.txt          # List of dependencies
```

---

## 🚀 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/shitizgoel/ev-chassis-material-ml.git
   cd ev-chassis-material-ml
   ```

2. (Optional) Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # or venv\Scripts\activate on Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Open the notebooks or run the scripts:
   ```bash
   jupyter notebook
   ```

---

## 🤝 Contributions

Pull requests and suggestions are welcome!  
For major changes, please open an issue first to discuss what you would like to change.
