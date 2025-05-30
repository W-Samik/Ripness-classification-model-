# Ripness-classification-model
# 🥑 Avocado Ripeness Predictor using Random Forest

This machine learning project uses a **RandomForestClassifier** to predict whether an **avocado is ripe or not** based on its physical and chemical properties.

## 📂 Dataset

The dataset `avocado_ripeness_dataset.csv` contains features such as:

- Weight
- Firmness
- Skin color
- Oil content
- Sugar level
- Acidity
- Storage days
- Temperature (optional)

The **target variable** is:
- `ripeness` (Binary: `Ripe` or `Unripe`)

## 🧠 Model

A **Random Forest Classifier** is used due to its robustness and ability to handle both linear and non-linear data effectively. It also reduces overfitting and improves accuracy through ensemble learning.

### Model Highlights:
- Ensemble of Decision Trees
- Handles feature interactions well
- Offers feature importance insights

### Example Code Snippet:
```python
from sklearn.ensemble import RandomForestClassifier
model = RandomForestClassifier(n_estimators=100, random_state=42)
model.fit(X_train, y_train)
