# 💳 Loan Default Prediction Using Decision Trees

## 📌 Project Overview

This project develops a Decision Tree Classification model to predict whether a customer will default on a loan. The project explores the challenges of class imbalance in credit risk modelling and demonstrates how class weighting can improve the detection of defaulting customers.

---

## 📂 Dataset

### 📥 Data Source

Dataset obtained from Kaggle:

Loan Default Prediction Dataset

* Size: 255,347 entries, 18 columns
* Target Variable: Default

  * 0 = No Default
  * 1 = Default

### Class Distribution

* No Default: 225 694 (88.4%)
* Default: 29 653 (11.6%)

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Pydotplus
* Graphviz

---

## 📊 Approach

* Performed data preprocessing and train-test split
* Built a baseline Decision Tree Classifier
* Evaluated model performance using:

  * Accuracy Score
  * Confusion Matrix
  * Classification report
* Identified class imbalance as a cause for on model predictions
* Applied class weighting to improve the identification of default cases
* Visualized the decision tree structure
* Visualised feature importance



---

## 🔍 Key Decisions

### Initial Model

* DecisionTreeClassifier(max_depth=5)
* Accuracy: 88.3%
* Correctly identified only 103 default cases
* Predicted the majority class (No Default) most of the time

### Balanced Model

* DecisionTreeClassifier(max_depth=5, class_weight='balanced')
* Accuracy: 66.9%
* Correctly identified 3,885 default cases
* Significantly improved detection of defaulting customers

---

## 📈 Results

### Initial Model

* Accuracy: 88.3%
* Recall (Default): 1.7%

### Balanced Model

* Accuracy: 66.9%
* Precision (Default): 21%
* Recall (Default): 65%
* F1-Score (Default): 32%

✔️ Class weighting substantially improved the model's ability to identify defaulting customers, despite reducing overall accuracy.

---

## ⚠️ Considerations

* The dataset is moderately imbalanced (88.4% vs 11.6%)
* Accuracy alone can be misleading in credit risk classification
* The balanced model produces more false positive predictions
* There is a trade-off between identifying defaulters and incorrectly flagging low-risk customers

---

## 💡 Key Insights

* High accuracy does not necessarily indicate a useful classification model
* Confusion matrices and classification reports provide deeper insights than accuracy alone
* Class imbalance can significantly affect model performance


  👤 Author
Tebogo Mosehle

📫 [tebogomosehle10@gmail.com]

Linkedin: www.linkedin.com/in/tebogo-mosehle-1806b319b
