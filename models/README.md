# Trained ML Models

Production-ready salary prediction models.

## Files:
salary_model.pkl ← Random Forest Regressor
label_encoder.pkl ← JobGroup encoder (Police=0, Fire=1...)


## Model Performance:
| Metric     | Test Score |
|------------|------------|
| R² Score   | 0.82       |
| MAE        | $18,500    |
| RMSE       | $24,000    |

## Load Model:
```python
import joblib
model = joblib.load('models/salary_model.pkl')
encoder = joblib.load('models/label_encoder.pkl')
