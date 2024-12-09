# **Student Performance Prediction**

## **Project Overview**
This project investigates the factors influencing student performance in secondary education and builds predictive models for final grades (G3). Using datasets from two Portuguese schools, the analysis focuses on academic, demographic, and behavioral variables to derive actionable insights for educators and policymakers.

---

## **Research Question**
What factors most influence student performance, and can we accurately predict students' final grades using behavioral and academic variables?

---

## **Dataset**
- **Source:** Two datasets from Portuguese schools (`student-mat.csv` and `student-por.csv`) containing academic, demographic, and behavioral features.
- **Target Variable:** `G3` (final grade), ranging from 0–20.

### **Key Features**
1. **Demographic Variables:** `age`, `sex`, `guardian`
2. **Academic Variables:** `G1`, `G2`, `failures`, `studytime`
3. **Parental Involvement:** `Medu`, `Fedu`, `Pstatus`
4. **Behavioral Variables:** `goout`, `activities`
5. **School Support:** `schoolsup`, `famsup`, `internet`, `higher`, `paid`

---

## **Methods**
1. **Data Preprocessing**:
   - Handling missing data (none found in the dataset).
   - Encoding categorical variables using `LabelEncoder`.
   - Scaling numerical variables for consistent range.

2. **Exploratory Data Analysis (EDA)**:
   - Heatmaps to explore correlations.
   - Histograms and boxplots to visualize feature distributions and their relationships with final grades.

3. **Modeling**:
   - **Linear Regression**: Provides baseline performance.
   - **Random Forest**: Captures complex relationships in the data.

4. **Evaluation Metrics**:
   - **R² Score**: Explains variance in final grades.
   - **Mean Absolute Error (MAE)**: Measures average error.
   - **Root Mean Squared Error (RMSE)**: Penalizes larger errors.

---

## **Results**
1. **Model Performance**:
   - **Random Forest** slightly outperforms **Linear Regression** in explanatory power (R² = 0.7678 vs. 0.7646).
   - Linear Regression shows slightly lower error metrics (MAE = 1.0508 vs. 1.0915).

2. **Feature Importance**:
   - **Top Predictors**:
     - Academic: `G1`, `G2`
     - Behavioral: `goout`
     - Parental: `Medu`, `Fedu`

---

## **Key Insights**
- Academic history (G1, G2) is the strongest predictor of final grades.
- Behavioral factors like going out (goout) also significantly affect performance.
- Random Forest captures non-linear relationships, while Linear Regression provides interpretability.

---

## **Future Directions**
- Implement cross-validation for better model generalization.
- Perform feature selection to refine predictors.
- Extend analysis to validate findings on additional datasets.

---

## **How to Run the Code**
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd <repository_name>
