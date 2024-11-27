# Machine Learning for Sustainable Development Goal 3: Good Health and Well-being👩‍⚕️🫀💉💊🩸  

## Project Overview  
This repository contains the code and resources for an AI-driven solution that identifies underserved areas in healthcare by analyzing socioeconomic and healthcare infrastructure data. The project aligns with **Sustainable Development Goal 3 (Good Health and Well-being)** by ensuring equitable healthcare access and promoting community well-being.  

---

## 💡 Motivation  
> _"It is health that is real wealth and not pieces of gold and silver."_  
> – **Mahatma Gandhi**

Access to healthcare is essential for well-being. Identifying underserved areas helps ensure fair resource distribution, fostering resilience and societal prosperity.  

---

## ✨ Features  
- **Data Simulation**: Simulated healthcare accessibility data using ChatGPT.  
- **Exploratory Data Analysis (EDA)**: Statistical and visual techniques like pairplots and heatmaps.  
- **Data Preprocessing**:  
  - Categorical encoding with `LabelEncoder`.  
  - Feature scaling with `StandardScaler`.  
- **Machine Learning Implementation**: Logistic Regression for binary classification tasks.  

---

## 📊 Dataset  
- **Size**: 500 rows × 13 columns.  
- **Features**: Includes demographic data, healthcare infrastructure details, and socioeconomic indicators (e.g., population density, income levels, and doctor availability).  

---

## 🧠 Code Example  

```python
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score, classification_report

# Logistic Regression Model
model = LogisticRegression(random_state=42)
model.fit(X_train, y_train)

# Initial Evaluation
y_pred = model.predict(X_test)
print("Initial Accuracy:", accuracy_score(y_test, y_pred))
print(classification_report(y_test, y_pred))

