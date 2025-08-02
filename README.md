
# LG Summer Internship – Robust Classification of Semi-Structured Textual Data

**Internship Project at LG Electronics**  
**Title:** Robust Classification of Semi-Structured Textual Data Using Random Forests and AI-Augmented Features  
**Intern:** Taru Bhargava , Kanishk Mehta 
**Tools Used:** Python, Scikit-learn, Pandas, NumPy, Excel, Mostly AI

---

## 📌 Objective

Build a robust multi-class classification pipeline to categorize semi-structured textual data into:
- **0 → Name**
- **1 → Email**
- **2 → Address**

using AI-synthesized data, noise injection, feature engineering, and Random Forest classifier with fine-tuning.

---

## 🧪 Workflow Overview

1. **Data Collection**
   - First names from Kaggle
   - Last names, emails, addresses generated via Mostly AI

2. **Data Preparation**
   - Combined and labeled data stored in Excel

3. **Data Cleaning**
   - Null removal, whitespace trimming, and preservation of noisy formats

4. **Data Manipulation (Noise)**
   - 5% of each class augmented with controlled noise (e.g., typos, spacing issues)

5. **Feature Engineering**
   - 20 handcrafted features: string length, pattern presence, digit/special char count, case flags, etc.

6. **Exploratory Data Analysis**
   - Class balance, feature distributions, ANOVA, Chi-Square tests

7. **Label Encoding**
   - Encoded categorical features for modeling

8. **Model Fitting**
   - RandomForestClassifier with `bootstrap=True`, `oob_score=True`

9. **Hyperparameter Tuning**
   - GridSearchCV for finding best combination

10. **Feature Selection**
    - Tested models with top 5, 10, and 16 important features

11. **Model Validation**
    - Used a completely unseen dataset of 75 samples

12. **ROC Curve Analysis**
    - Evaluated model performance using ROC curves and AUC scores

---

## 📂 Repository Structure

```
LG_Summer_Internship/
│
├── Python Code/
│   └── LG_Internship.ipynb         # Complete Jupyter notebook for pipeline
│
├── Report/
│   └── Final Report_LG.docx        # Internship report in Word format
│
├── Sheets/
│   ├── Data/
│   │   ├── Original_data.xlsx      # Clean original data
│   │   ├── Noisy_Data.xlsx         # Data with injected noise
│   │   └── Validation_data.xlsx    # Final validation set (unseen)
│   │
│   └── Output/
│       ├── categorical_feature_eda.xlsx  # Categorical feature analysis
│       ├── continuous_feature_eda.xlsx   # Continuous feature analysis
│       ├── Noisy.xlsx                    # Feature output of noisy data
│       └── Validation.xlsx               # Model predictions on validation data
```

---

## 📈 Key Outputs

- Confusion Matrices (train & validation)
- Feature Importance Plots
- ROC Curves (macro & per-class)
- Classification Reports
- Excel outputs for feature sets & predictions

---

## 🧠 Learnings

- Hands-on experience with AI-generated data
- Advanced feature engineering
- Real-world noise robustness
- End-to-end model building, tuning & evaluation

---

