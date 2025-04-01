# Customer Churn Prediction Using Machine Learning

## Overview
This project predicts customer churn for a telecommunications company using machine learning techniques. The model identifies key factors influencing churn and helps improve customer retention strategies.

## Features and Approach
- **Dataset:** Contains customer features such as revenue, call data, customer service interactions, and account details.
- **Preprocessing:**
  - Missing values filled using the **median**.
  - **RobustScaler** used for scaling due to skewed data.
  - Feature engineering includes derived metrics like `revenue_usage_ratio`, `recurring_charge_gap`, and `eqpdays`.
- **Model Used:** `KNeighborsClassifier (KNN)`, optimized with `k=3` and distance-based weighting.
- **Evaluation Metrics:**
  - Accuracy: **0.8283**
  - Precision: **0.8283**
  - Recall: **0.8283**
  - F1 Score: **0.8282**
  - ROC-AUC Score: **0.9082**

## Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/OlaSuaifan93/SDG_Telecom_Cust_churn.git
cd your-repo
pip install -r requirements.txt

```

## Running the Model
```bash
DataAnalysis.py
```

## Saving and Loading the Model
The trained model is saved using `joblib`:
```python
from joblib import dump, load
# Save model
dump(model, 'Best_model.joblib')
# Load model
model = load('Best_model.joblib')
```

## Key Features by Importance
1. `revenue_usage_ratio` - **10.27%**
2. `eqpdays` - **9.11%**
3. `rev_usage_change_ratio` - **8.13%**
4. `income_underutilization` - **8.02%**
5. `recurring_charge_gap` - **5.88%**

## Contributors
- [Ola Suaifan](https://github.com/OlaSuaifan93)

## License
This project is licensed under the MIT License.

