# Task 6: K-Nearest Neighbors (KNN) Classification

## 📌 Objective
The goal of this task was to understand and implement the **K-Nearest Neighbors (KNN)** algorithm for solving classification problems using the **Iris dataset**.

---

## 🧰 Tools & Libraries Used
- Python 3
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## 📁 Dataset
**Iris Dataset**  
- Features: Sepal Length, Sepal Width, Petal Length, Petal Width  
- Target: Species (`Setosa`, `Versicolor`, `Virginica`)

---

## ✅ Steps Performed

1. **Data Loading & Preprocessing**
   - Loaded `Iris.csv` using Pandas.
   - Dropped unneeded columns.
   - Normalized the feature data using `StandardScaler`.

2. **KNN Model Implementation**
   - Used `KNeighborsClassifier` from `sklearn.neighbors`.
   - Split dataset into training and testing sets (80-20).
   - Trained KNN model for different values of **K** (1 to 20).

3. **Evaluation**
   - Computed **accuracy** for each K.
   - Selected best K based on maximum test accuracy.
   - Generated and visualized the **confusion matrix** using `matplotlib`.

4. **Visualization**
   - **Accuracy vs. K plot** to understand performance trend.
   - **Decision boundary visualization** using PCA (2D projection of features).

---

## 📊 Results
- Best accuracy achieved at **K = `X`** (depends on output).
- Decision boundary clearly separates different species in 2D PCA space.
- Confusion matrix showed high accuracy with minimal misclassifications.

---

## 🧠 What I Learned

### 📌 KNN Fundamentals
- KNN is a **lazy learning** and **non-parametric** algorithm.
- It classifies based on the **majority vote** of nearest neighbors.

### 📌 Choosing K
- Small K → high variance (overfitting)  
- Large K → high bias (underfitting)  
- Optimal K is typically chosen via **cross-validation or accuracy plots**.

### 📌 Why Normalization?
- KNN relies on **distance metrics** (e.g., Euclidean).  
- Normalization ensures all features contribute equally to the distance.

### 📌 Evaluation
- **Accuracy** and **confusion matrix** give good insight into model performance.
- **Decision boundaries** help visualize how KNN separates classes.

### 📌 Time Complexity
- Training: **O(1)** (no training phase)
- Prediction: **O(n × d)** where `n` = training points, `d` = dimensions

---

## ❓ Interview Questions Tackled

1. How does KNN work?
2. How do you choose the right value of K?
3. Why is normalization important?
4. What is the time complexity of KNN?
5. Pros & Cons of KNN
6. Sensitivity to noise
7. Multi-class classification using KNN
8. Role of distance metrics (Euclidean, Manhattan, etc.)

---

## 🏁 Conclusion
This task helped solidify my understanding of KNN, its practical implementation, and evaluation. I also gained insights into model selection, hyperparameter tuning, and the importance of feature scaling.

