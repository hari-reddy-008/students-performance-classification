**Students Performance Classification**

## **Overview:**

This capstone project focuses on students academic prediction using machine learning techniques. 
The goal is to understand how various factors—such as previous grades, study time, failures, demographics, alcohol consumption, and absences—impact the final grade (G3).

## **The project includes:**

* End-to-end ML workflow
* Exploratory data analysis
* Outlier handling
* Feature engineering & preprocessing
* SMOTE-based class balancing
* Training and comparing 7 supervised learning models
* GridSearch hyperparameter tuning
* Detailed evaluation metrics

## **The dataset used in this project is Student Performance Dataset, specifically:**

* student-mat.csv — Math students dataset
* Contains demographic, social, academic, and behavioral attributes

## **Key feature groups:**

**Demographics:** age, gender, address
**Academics:** previous grades (G1, G2), G3 (target)
**Behavioral:** study time, alcohol consumption (Walc & Dalc), absences
**Family:** parental job, family support, internet, nursery, reason for choosing school

## **Project Workflow**

* Importing libraries & loading datasets
* Dataset exploration (shape, types, missing values, duplicates)
* Exploratory Data Analysis (visualizations + numerical insights)
* Outlier detection & treatment using IQR
* Train-test split
* Preprocessing pipeline (scaling + encoding)
* Handling class imbalance with SMOTE
* Model training (Logistic Regression, Decision Tree, RF, SVM, KNN, GB, XGBoost)
* Hyperparameter tuning using GridSearchCV
* Evaluation & comparison
* Final insights & conclusion

## **Exploratory Data Analysis**

**EDA includes:**
* Gender distribution
* Address: urban vs rural
* Relationship between study hours & grades
* Failures distribution
* Alcohol consumption (Dalc, Walc) across age groups
* Scatterplots: G1→G2→G3 correlation
* Boxplots for numerical feature outliers
* Distribution of continuous variables

## **Key insights:**

* G1 & G2 have strong positive correlation with G3
* Alcohol consumption slightly increases with age
* Higher study time aligns with better final grades
* Absences show heavy right skew and required outlier handling

## **Data Preprocessing Outlier Treatment**

**Applied IQR method on:**
* Age
* Absences
* G1, G2, G3
* Replaced extreme values with median.
* Categorical Encoding
* Used OneHotEncoder for non-numerical features.
* Scaling
* Applied StandardScaler to continuous features.
* Train-Test Split
* test_size = 20%
* random_state = 42
* SMOTE for Class Balancing
* Balanced final grade classes to prevent bias and improve model learning.

## **Modeling & Evaluation**

* **Logistic Regression** -  **GridsearchCV** Accuracy improved from 67% → 75%.
* **Decision Tree** - **GridsearchCV**  Accuracy 76%  Best Performer.
* **Random Forest** - **RandomizedsearchCV** Accuracy 66% → 71%
* **SVC** - **RandomizedsearchCV** Accuracy 66% → 73%
* **KNN** - **RandomizedsearchCV** Accuracy 52% → 65%
* **Gradient Boosting** - **RandomizedsearchCV** Accuracy 67% → 71%
* **X Gradient Boosting** - **RandomizedsearchCV** Accuracy 61% → 71%

## **Evaluations include:**

* Accuracy
* Precision
* Recall
* F1-score
* Classification reports

## **Results**

* Logistic Regression accuracy improved from 67% → 75% after preprocessing + tuning
* Logistic Regression & Random Forest delivered the best results overall
* SMOTE significantly improved minority class recalls

## **Technologies Used**

* Python
* Pandas
* NumPy
* Matplotlib & Seaborn
* Scikit-learn
* SMOTE (Imbalanced-learn)
* XGBoost
* Google Colab Notebook




