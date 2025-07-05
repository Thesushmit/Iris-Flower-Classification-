

````
# 🌸 Iris Flower Classification using Logistic Regression

A beginner-friendly machine learning project that classifies iris flowers into three species — **Setosa**, **Versicolor**, or **Virginica** — using **Logistic Regression**.

---

## 📁 Dataset

- **Source**: Built-in Iris dataset from `scikit-learn`
- **Features**:  
  - Sepal length  
  - Sepal width  
  - Petal length  
  - Petal width  
- **Target**: Species (`setosa`, `versicolor`, `virginica`)

---

## 🛠️ Tech Stack

- Python 3.x  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  

---

## 🚀 Workflow

1. Load and clean the Iris dataset
2. Encode categorical labels (species)
3. Split into training and testing sets
4. Standardize feature values
5. Train a Logistic Regression model
6. Predict new samples
7. Evaluate the model

---

## 🧪 Example Prediction

```python
sample = np.array([[6.7, 3.0, 5.2, 2.3]])  # Example input
sample_scaled = scaler.transform(sample)
prediction = model.predict(sample_scaled)
print("Predicted species:", le.inverse_transform(prediction)[0])
````

**Output:**

```
Predicted species: virginica
```

---

## 📊 Model Evaluation

Use these metrics from `sklearn.metrics`:

### ✅ Accuracy Score

```python
from sklearn.metrics import accuracy_score
accuracy = accuracy_score(y_test, y_pred)
print("Accuracy:", accuracy)
```

### ✅ Confusion Matrix

```python
from sklearn.metrics import confusion_matrix
print(confusion_matrix(y_test, y_pred))
```

### ✅ Classification Report

```python
from sklearn.metrics import classification_report
print(classification_report(y_test, y_pred))
```

This gives precision, recall, F1-score for each class.

---

## 📂 File Structure

```
iris_classification/
├── main.py       # Main Python script
├── README.md           # Project documentation
```

---

## ✅ How to Run

1. Install dependencies if needed:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```

2. Run the script:

```bash
python main.py
```

---

## 👨‍💻 Author

**Sushmit Partakke**
Project for learning and demonstration purposes.

---

## 🌐 References

* [Scikit-learn Iris Dataset](https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html)
* [UCI ML Repository – Iris Data](https://archive.ics.uci.edu/ml/datasets/iris)

```


