# Team2_Python_Pioneers_PythonHackathon_Sep_2026

**Cardiac Failure Analytics**

Our Research Question
Can a hospital identify high-risk heart failure patients using information available when they are admitted?
We used patient demographic, cardiac, medical history, laboratory, medication, and hospitalization data to find patterns related to mortality and readmission.

**Team Members**
- Aditi Mishra
- Saranya Shanmugam
- Sashi Laguduva
- Sudha Madhuri Basa
- 
**About the Dataset**
The dataset contains information from **2,008 hospitalized heart failure patients**.
The data was organized into different hospital tables and linked using:” inpatient_number”
The main areas of the data include:
- Demography
- Cardiac information
- Patient history
- Hospitalization and discharge
- Laboratory results
- Responsiveness
- Prescriptions
The final cleaned dataset contains:
**2,008 rows × 210 columns**


**Our project was divided into four main parts:**
1. **Data Cleaning**: We first cleaned and prepared the raw data.
We cleaned the data and few feature engineering fro the model performance
**Some features we created include:**
-	BMI categories
-	Obesity flag
-	NLR
-	Comorbidity count
-	CCI groups
-	Medication burden
-	Kidney function groups
-	Other clinical groups
2. **Descriptive Analysis**: We explored the patient data to understand the population.
3. Prescriptive Analysis: We then looked at relationships between clinical variables and patient outcomes.Here We used statistical tests such as:
-	Fisher's Exact Test
-	Chi-Square Test
-	Spearman Correlation
-	Mann-Whitney U Test
-	Kruskal-Wallis Test
4. **Predictive Analysis**
We also tested whether patient information could be used to predict outcomes.
The models we tested were:
-	Logistic Regression
-	Random Forest
-	Artificial Neural Network (ANN)
We looked at:-
-	ROC-AUC
-	PR-AUC
-	Recall
-	Precision

The main outcomes included:
-	28-day mortality
-	6-month mortality
-	6-month readmission
We used cross-validation to evaluate the models.


**Streamlit Dashboard**:
We created an interactive Streamlit dashboard to bring our analysis together.The dashboard has the following sections:
**Introduction**:Shows our research question, project purpose, and team members.
**Data Overview**:Shows the size and structure of our dataset and the main types of information included.
**Data Cleaning & Features**:Shows the main cleaning and feature-engineering steps we performed.
**Interactive Clinical Insights**:This is the main interactive section of our dashboard.
Users can select:
1. An insight area
2. A clinical marker
3. An outcome
The dashboard then shows the related chart, outcome rate, statistical evidence, and a short explanation.This allows users to explore different clinical questions without having to run the analysis themselves.

**Model Performance**:Shows the performance of our predictive models and allows users to explore model-based risk results.
**Key Takeaways & Conclusion**:Summarizes the main findings from our analysis.

**Some of Our Findings**
A few of the patterns we found in the dataset were:
About **38.5%** of patients were readmitted within 6 months.
- About **2.8%** of patients died within 6 months.
- Higher Killip grades were associated with higher mortality.
- Higher creatinine levels were associated with higher 6-month readmission.
- Kidney function markers showed differences between patient outcome groups.
- Higher troponin levels were associated with higher mortality.
- NLR and other inflammation-related markers showed differences across outcome groups.
These are associations found in our dataset and do not mean that one factor directly caused an outcome.
**Predictive Model Results**
Some of the Logistic Regression results from our analysis were:
| Outcome | ROC-AUC | Recall |
| 28-day death | 0.89 | 78% |
| 6-month death | 0.82 | 70% |
| 6-month readmission | 0.61 | 56% |

We also compared Logistic Regression with Random Forest and ANN.

------------------


