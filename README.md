# 🪨 Rock vs Mine Prediction using Logistic Regression

This project demonstrates a **binary classification** problem using a **Logistic Regression model** to predict whether a sonar signal indicates a **rock** or a **mine**.

---

## 📌 Project Highlights

- 📂 Dataset: Sonar signals from the UCI Machine Learning Repository
- 🤖 Model: Logistic Regression (Supervised Learning)
- 🧪 Evaluation: Accuracy on training and testing data
- 🎯 Goal: Predict if the object is a rock (R) or mine (M) based on sonar signal features

---

## 📊 Dataset Summary

- **Source**: https://drive.google.com/file/d/1pQxtljlNVh0DHYg-Ye7dtpDTlFceHVfa/view?usp=drive_link
- **Instances**: 208
- **Features**: 60 continuous values per instance (0 to 1 range)
- **Target Classes**: 
  - `R` → Rock  
  - `M` → Mine

---

## 📁 Files in the Repository

- `Rock vs Mine Prediction Using Logistic Regression Model.ipynb`: Full Jupyter notebook with code, analysis, and model
- `README.md`: This documentation file
- `sonar data.csv`: (Not included here; assumed to be added manually)

---

## 🛠 Technologies Used

- **Python**
- **Jupyter Notebook**
- **NumPy & Pandas** – Data manipulation
- **scikit-learn** – Model training & evaluation

---

## ⚙️ Workflow

1. **Import Libraries**  
2. **Load and Explore the Dataset**  
3. **Preprocess Data** – Split into features and labels  
4. **Train/Test Split** – 90% training, 10% testing  
5. **Train the Model** – Logistic Regression  
6. **Evaluate the Model** – Accuracy on both sets  
7. **Make Predictions** – Input custom data to classify as rock or mine

---

## 📈 Model Evaluation

- Training Accuracy: ~89%
- Testing Accuracy: ~81%
- Evaluation Metrics: Accuracy Score

---

## 🔮 Sample Prediction Code

```python
input_data = (0.0187,0.0346,...,0.0157)
input_data_np = np.asarray(input_data).reshape(1, -1)
prediction = model.predict(input_data_np)
print("Prediction:", "Rock" if prediction[0] == 'R' else "Mine")
