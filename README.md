# Stock Price Direction Prediction Using Alternative Asset Information

This repository contains the source code and dataset for the thesis project titled:

"The Inclusion of Alternative Asset Information Improves Model Performance in Stock Direction Prediction"

conducted as part of the Master's program in Data Science and Business Analytics at the University of Amsterdam.

---

## Repository Overview

This study investigates whether incorporating alternative asset data—specifically interest rates, Bitcoin prices, and gold prices—can improve the prediction of stock price direction using various machine learning models. The models evaluated include Logistic Regression, Support Vector Machine (SVM), Random Forest, XGBoost, and Multi-layer Perceptron (MLP).

The project assesses both short-term (1-day ahead) and medium-term (20-day ahead) stock movement predictions. Evaluation metrics include macro F1-score and Area Under the Curve (AUC), with feature contributions analyzed through SHAP values.

---

## Contents

| File                  | Description                                           |
|------------------------|------------------------------------------------------|
| `DATA (1).csv`          | Main dataset containing stock and alternative asset features |
| `collect.ipynb`         | Data collection and preprocessing notebook           |
| `WXH_logistic.ipynb`    | Logistic Regression model training and analysis      |
| `WXH_SVM.ipynb`         | Support Vector Machine model implementation          |
| `WXH_random.ipynb`      | Random Forest model experiments                      |
| `WXH_Boost.ipynb`       | XGBoost model experiments                            |
| `WXH_MLP.ipynb`         | Multi-layer Perceptron (Neural Network) experiments  |

---

## Usage

1. Clone the repository:

   git clone https://github.com/XinhuiWang1992/stock-prediction-thesis.git
   cd stock-prediction-thesis

2. Run the notebooks using Jupyter:

   jupyter notebook

   Open any of the notebooks to reproduce the experiments:
   - WXH_logistic.ipynb : Logistic Regression
   - WXH_SVM.ipynb      : Support Vector Machine
   - WXH_random.ipynb   : Random Forest
   - WXH_Boost.ipynb    : XGBoost
   - WXH_MLP.ipynb      : Multi-layer Perceptron

---

## Summary of Findings

- Adding interest rate data significantly improved medium-term (20-day) prediction performance, especially with XGBoost, which achieved a 9.1% improvement in F1-score and a 16.0% improvement in AUC.
- Bitcoin prices enhanced AUC in linear models and MLP, indicating improved discrimination ability, though classification thresholds needed adjustment for optimal F1 performance.
- Gold prices did not show substantial predictive value under the tested framework.

SHAP analysis provided insights into how alternative assets contributed to model predictions, revealing complex nonlinear effects and conditional dependencies.

---

## Citation

If you use this repository or find it helpful for your research, please cite:

Xinhui (2025). The Inclusion of Alternative Asset Information Improves Model Performance in Stock Direction Prediction. Master’s Thesis, Faculty of Economics and Business, University of Amsterdam. Available at: https://github.com/XinhuiWang1992/stock-prediction-thesis

---

## License

This project is licensed under the MIT License.

---

## Contact

For any questions or collaboration inquiries, please contact:

Xinhui  
Email: xinhuiwang251@gmail.com
