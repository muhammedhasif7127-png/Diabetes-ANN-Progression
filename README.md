# Diabetes Progression Prediction using ANN

## 📌 Objective
This project models the progression of diabetes using the sklearn dataset.  
The goal is to build, train, and evaluate an Artificial Neural Network (ANN) to predict disease progression and analyze model performance.

---

## 📂 Contents
- `Diabetes_ANN.ipynb` → Jupyter Notebook with full workflow  
- `README.md` → Project documentation  

---

## ⚙️ Workflow
1. **Data Loading & Preprocessing**
   - Loaded diabetes dataset from `sklearn.datasets`.
   - Checked for missing values (none found).
   - Normalized features using `StandardScaler`.

2. **Exploratory Data Analysis (EDA)**
   - Target distribution plot.
   - Correlation heatmap.
   - Scatter plots of features vs target.

3. **Model Building**
   - Baseline ANN: 2 hidden layers (64 → 32 neurons), ReLU activations.
   - Output layer: 1 neuron for regression.

4. **Training**
   - Train-test split (80/20).
   - 100 epochs, batch size 32.
   - Training vs validation loss plotted.

5. **Evaluation**
   - Metrics: Mean Squared Error (MSE), R² Score.

6. **Improvement Attempt**
   - Larger architecture (128 → 64 → 32).
   - Mixed activations (ReLU, Tanh).
   - 150 epochs with Adam optimizer.

---

## 📊 Results

### Baseline Model
- **MSE:** 2965.70  
- **R²:** 0.44  

### Improved Model
- **MSE:** 3801.72  
- **R²:** 0.28  

### Comparison Table

| Model Version       | MSE    | R²   | Notes                          |
|---------------------|--------|------|--------------------------------|
| Baseline ANN        | 2965.7 | 0.44 | 2 hidden layers, ReLU          |
| Improved ANN        | 3801.7 | 0.28 | Larger architecture, mixed activations |

---

## 🖼️ Visuals
- Distribution of target variable  
- Correlation heatmap  
- Feature-target scatter plots  
- Training vs Validation Loss curve  

---

## ✅ Conclusion
- The baseline ANN generalized better than the more complex model.  
- Added complexity reduced performance, showing that **simpler architectures can outperform deeper ones on small datasets**.  
- Future improvements could include:
  - Regularization (Dropout, L2).  
  - EarlyStopping to avoid overtraining.  
  - Hyperparameter tuning (learning rate, batch size).  

---

## 📌 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/muhammedhasif7127-png/Diabetes-ANN-Progression.git
