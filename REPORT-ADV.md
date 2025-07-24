# 🔴 Advanced Track

## ✅ Week 1: Setup & Exploratory Data Analysis (EDA)


### 🔑 Question 1:
**Which features contain high proportions of “unknown” values (e.g., in `job`, `education`, `contact`, `poutcome`), and how did you decide whether to impute, encode, or discard them?**  

💡 **Hint:**  
Use `.isin(['unknown']).sum()` and `.value_counts(normalize=True)` for affected columns.  
Consider frequency, distribution, and impact on the target.  
Think: could "unknown" hold implicit meaning in real marketing contexts?

✏️ *Your answer here...*


### 🔑 Question 2:
**How imbalanced is the target variable (`y`), and what strategies might you consider to address this imbalance in a deep learning context?**  

💡 **Hint:**  
Use `.value_counts(normalize=True)` and bar plots.  
If "yes" is heavily underrepresented, consider:  
- Weighted loss functions  
- Oversampling (SMOTE)  
- Stratified batching or data augmentation  
Explain pros/cons of each in deep learning.

✏️ *Your answer here...*


### 🔑 Question 3:
**Which categorical features are high-cardinality, and how will this influence your encoding strategy (e.g., embeddings vs. one-hot)?**  

💡 **Hint:**  
Use `.nunique()` and `value_counts()` to inspect cardinality.  
Variables like `job`, `education`, `contact`, or `poutcome` may benefit from learned embeddings.  
Reflect on how this affects model complexity and generalization.

✏️ *Your answer here...*


### 🔑 Question 4:
**Which continuous features (e.g., `balance`, `duration`, `campaign`, `pdays`) are most skewed or contain extreme outliers? What preprocessing might help improve numerical stability during training?**  

💡 **Hint:**  
Use `.describe()`, `.skew()`, and histograms or boxplots.  
Use log-transform or normalization (`StandardScaler`, `MinMaxScaler`).  
Consider clipping or binning rare/extreme values.

✏️ *Your answer here...*


### 🔑 Question 5:
**What feature-to-target interactions stood out during EDA (e.g., `previous` contacts vs. subscription, or `month` vs. `y`)? How might these inform future feature engineering or model attention?**  

💡 **Hint:**  
Use heatmaps or grouped bar plots to visualize interactions like:  
- `previous` vs. `y`  
- `month` vs. `y`  
- `contact` method vs. `poutcome`  
Explain which interactions appear strongest and how they could shape feature engineering.

✏️ *Your answer here...*

