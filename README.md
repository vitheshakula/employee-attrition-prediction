Employee-Attrition-Prediction
Employee exit prediction via Random Forest on HR dataset

Open In Colab - https://colab.research.google.com/drive/1SCdOMPOsVxOHGVvhR7ew4W9M_Hdj298g?usp=sharing

This project leverages machine learning to predict whether an employee is likely to leave a company, based on factors such as satisfaction level, salary, promotions, and working hours. The model aims to help HR departments identify at-risk employees and reduce attrition rates through data-driven decision-making.

Dataset

  - Source: Offered as part of the *Infosys Springboard – Machine Learning Foundations* course.
  - Format: CSV (`HR_comma_sep.csv`)
  - Size: ~15,000 records
  - Target Variable: `left` (1 = Left the company, 0 = Stayed)

Note: Because of licensing issues, the data is not available in this repository.
      If you are enrolled in the course, you may obtain it from the Springboard course portal.
      Or if you executed the notebook, you can also upload it manually with `files.upload()` in Google Colab.

Technologies Used

  - Python
  - Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
  - Platform: Google Colab

---

Features Used

    | Feature                | Description                                  |
    |------------------------|----------------------------------------------|
    | `satisfaction_level`   | Worker's satisfaction rating (0 to 1)         |
    | `average_monthly_hours`| Monthly average working hours                      |
    | `salary`               | Salary level (Low, Medium, High)             |
    | `promotion_last_5years`| Promoted in last 5 years         |
    | `number_project`       | Number of projects treated                   |
    | `time_spend_company`   | Time spent in company                   |

---

Model Overview

  - Algorithm*: Random Forest Classifier
  - Train-Test Split: 80% training, 20% testing
    - Preprocessing:
    - Categorical attribute encoding
    - Feature scaling
  - Evaluation Metrics:
    - Accuracy: 85%
    - F1 Score: 0.78

---

Key Insights

  - Low satisfaction is the best predictor of turnover.
  - Low pay and no promotion have strong exit correlations.
  - Working hours did not have any effect.
  
---

Future Improvements

  - Try other models (e.g., XGBoost, Logistic Regression)
  - Conduct higher-level feature engineering (e.g., department, performance ratings)
  - Use hyperparameter tuning to achieve higher accuracy

---

Project Files

  - `employee_attrition_prediction.ipynb` – Sanitized Colab notebook with complete code and analysis
  - _Dataset not included (see Dataset section above)_

---

License

  This project is purely academic in scope and follows usage guidelines offered by Infosys Springboard.
