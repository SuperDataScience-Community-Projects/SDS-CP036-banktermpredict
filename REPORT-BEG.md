# 🟢 Beginner Track

## ✅ Week 1: Setup & Exploratory Data Analysis (EDA)

### 🔑 Question 1:
**Which features contain missing or placeholder values (such as “unknown”), and how did you handle them? What impact might your chosen strategy have on downstream modeling?**  

💡 **Hint:**  
Use `.isin(['unknown']).sum()` or `.value_counts()` to detect placeholders.  
Consider replacing, imputing, grouping, or removing rows/columns depending on frequency and importance.  
Reflect on how this might affect model bias or signal loss.

✏️ *Your answer here...*


### 🔑 Question 2:
**What is the distribution of the target variable (`y`), and how imbalanced is it? How might this class imbalance affect model training and evaluation?**  

💡 **Hint:**  
Use `.value_counts(normalize=True)` and visualize with a pie chart or bar plot.  
If class 1 (“yes”) is under 20%, consider balancing techniques later.  
Mention how imbalance can mislead accuracy metrics.

✏️ *Your answer here...*


### 🔑 Question 3:
**Which numeric features (e.g., age, balance, duration, campaign) are most skewed or contain outliers, and what transformations might improve their distributions?**  

💡 **Hint:**  
Use `.describe()`, histograms, and boxplots to inspect skew.  
Consider log or square root transforms for right-skewed data.  
Outliers in `duration` or `balance` may require treatment or binning.

✏️ *Your answer here...*


### 🔑 Question 4:
**How do key categorical features like `job`, `education`, and `marital` relate to the likelihood of a client subscribing (`y`)? What patterns stand out?**  

💡 **Hint:**  
Use `groupby('job')['y'].value_counts(normalize=True)` or seaborn barplots.  
Visualize `education` vs. subscription rate using stacked bars or grouped plots.  
Comment on whether patterns make intuitive sense (e.g., students vs. retirees).

✏️ *Your answer here...*


### 🔑 Question 5:
**What are your key takeaways from the EDA that could influence your feature engineering or model design in the next phase?**  

💡 **Hint:**  
Summarize 3–5 observations: e.g., target imbalance, top predictive features, high cardinality variables, etc.  
Mention any preprocessing decisions you'll carry forward (e.g., encoding schemes, dropping `duration` if leaked).

✏️ *Your answer here...*

