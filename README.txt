🧠 Supervised Machine Learning Classification with Feature Selection

Implementation and comparison of supervised machine learning algorithms for classification problems with feature selection, applied to heart disease and diabetes prediction datasets.

--------------------------------------------------------------------------------
📘 Project Overview

This project explores supervised machine learning algorithms for solving binary classification problems and evaluates how feature selection impacts model performance. Two healthcare datasets — Heart Disease and Diabetes — were analyzed using six models to understand their accuracy, stability, and sensitivity to feature subsets.

--------------------------------------------------------------------------------
🎯 Objective

To understand and explore supervised machine learning algorithms for classification problems with feature selection.

--------------------------------------------------------------------------------
📂 Repository Structure

supervised-ml-classification-feature-selection/
├── P1 Part 1.ipynb              # Heart Disease: Decision Tree & Random Forest
├── P1 Part 2.ipynb              # Diabetes: Naive Bayes, kNN, Logistic Regression, SVM
└── README.txt                   # Documentation file

--------------------------------------------------------------------------------
🧠 Datasets

Heart Disease Dataset
- Samples: 918
- Attributes: 11 predictive features (Age, RestingBP, Cholesterol, MaxHR, etc.)
- Algorithms Used: Decision Tree, Random Forest
- Highlight: Random Forest achieved accuracy of 0.8657

Diabetes Dataset
- Samples: 99,805
- Attributes: 16 numerical features
- Algorithms Used: Naive Bayes, kNN, Logistic Regression, SVM
- Highlight: Gaussian NB and Logistic Regression achieved accuracy ~0.85–0.86

--------------------------------------------------------------------------------
⚙️ Algorithms Implemented

Decision Tree  | Heart Disease | Accuracy ≈ 0.82
Random Forest  | Heart Disease | Best (0.8657)
Naive Bayes (Gaussian) | Diabetes | Strong with continuous data
Naive Bayes (Multinomial) | Diabetes | Low accuracy for continuous data
kNN | Diabetes | Stable beyond k=10 (0.84)
Logistic Regression | Diabetes | Consistent (0.85)
SVM | Diabetes | Linear kernel, ~0.70 accuracy

--------------------------------------------------------------------------------
🔬 Feature Selection Study

Random subset feature experiments with m=3 and m=7 were conducted.
Findings:
- Increasing features reduced accuracy variance.
- kNN and SVM were more sensitive to feature selection.
- Gaussian NB and Logistic Regression were stable even with fewer features.
- Using 7 features improved overall accuracy.

--------------------------------------------------------------------------------
📈 Best Results Summary

Model | Max Accuracy | Best Feature Subset (Example)
Random Forest | 0.8657 | Age, Cholesterol, MaxHR
Gaussian NB | 0.8671 | glucose_fasting, hba1c, bp
Logistic Regression | 0.8595 | ldl_cholesterol, hba1c, systolic_bp
kNN | 0.8900 | hba1c, waist_to_hip_ratio, activity_minutes
SVM | 0.8937 | hba1c, insulin_level, systolic_bp

--------------------------------------------------------------------------------
🧪 Tools & Libraries

Python 3.x
scikit-learn
pandas, numpy
matplotlib, seaborn
Jupyter Notebook

--------------------------------------------------------------------------------
🚀 How to Run

1. Clone this repository:
   git clone https://github.com/upratham/supervised-ml-feature-experiments.git

2. Install dependencies:
   pip install -r requirements.txt

3. Open Jupyter Notebook:
   jupyter notebook

4. Run both parts in order:
   - P1 Part 1.ipynb
   - P1 Part 2.ipynb

--------------------------------------------------------------------------------
📜 Conclusion

This project shows how supervised ML algorithms perform on healthcare data and how feature selection improves reliability and accuracy. Ensemble methods and probabilistic models show strong generalization, while distance-based models are more sensitive to feature selection.

--------------------------------------------------------------------------------
🔮 Future Improvements

- Add ROC-AUC and precision-recall evaluation
- Implement cross-validation
- Explore deep learning models (MLP/ANN)
- Analyze feature importance and correlation

--------------------------------------------------------------------------------
👤 Author

Prathamesh Uravane
Email:upratham2002@gmail.com

⭐ If you find this project useful, please give it a star!
