#  Student Academic Stress — Data Analysis & Preprocessing Guide

This repository contains a Jupyter Notebook that analyzes a small survey dataset about **students’ academic stress** and demonstrates practical data-preprocessing steps — especially **handling categorical variables** — along with basic machine learning experiments.

---

##  Project Goals

- Perform **Exploratory Data Analysis (EDA)** on a small, real-world dataset.  
- Demonstrate how to **clean** and **encode** categorical variables using `OneHotEncoder` and `pd.get_dummies()`.  
- Apply standard preprocessing steps such as **missing value imputation** and **scaling**.  
- Discuss challenges when working with **small or imbalanced datasets**.

---

##  Notebook Overview

1. **Introduction & Purpose**  
   - Overview of dataset and objectives.

2. **Timestamp Handling**  
   - Dropped `Timestamp` column (not useful for modeling).

3. **EDA (Exploratory Data Analysis)**  
   - Summary statistics, feature distributions, and correlations.

4. **Missing Values**  
   - Mode imputation for missing categorical columns such as `Study Environment`.

5. **Categorical Encoding**  
   - Using `OneHotEncoder` (from `sklearn`)  
   - Using `pandas.get_dummies()` for quick encoding

9. **Discussion & Observations**  
   - Reflections on small dataset behavior, class imbalance, and possible improvements.

---

##  Key Learnings

- **Categorical variables**: Prefer `OneHotEncoder` for production pipelines; use `get_dummies()` for quick EDA.  
- **Missing values**: Mode imputation works for single missing entries; consider `SimpleImputer` for larger gaps.  
- **Evaluation**: On small datasets, accuracy can be misleading — check macro F1 and per-class recall instead.  

---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/StudentAcademicStress.git
   ```
2. Navigate to the project directory:
   ```bash
   cd StudentAcademicStress
   ```
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook StudentAcademicStress.ipynb
   ```

---

## Tools & Libraries

Python 3.10+

pandas, numpy

scikit-learn

matplotlib, seaborn

---

## License

This project is open-source under the MIT License.

---

##  Author & Contact

**Created by:** [Emre Yörük](https://github.com/emreyoruk64)  
**Purpose:** Educational notebook for data preprocessing and model experimentation.  
**Connect:** If you find this helpful, consider giving the repo a ⭐ and sharing your thoughts!

