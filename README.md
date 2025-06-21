<h1 align="center">🚢 Titanic Dataset – Exploratory Data Analysis (EDA)</h1>

<p align="center">The notebook analyzes different patterns from the infamous titanic datatset. It includes finding survival rates based on factors like sex, age, passenger class, etc.</p>

---

## 📄 Overview

This notebook performs an in-depth Exploratory Data Analysis (EDA) on the Titanic dataset to understand how different factors such as **sex**, **age**, **passenger class**, **fare**, and **embarkation point** influenced survival.

---

## 📓 This notebook contains the following

### 1. 📊 Dataset Metadata Exploration

-   Preview of the first 5 rows with `titanic.head()`
-   Basic dataset info: shape, column types, and column names
-   Descriptive statistics using `describe(include="all")`

---

### 2. 🧼 Missing Values Analysis

-   Visualized missing data using a **heatmap**

<p align="center">
    <img src="images/missing_values_heatmap.png" alt="missing values heatmap" width="600"/>
</p>

-   Missing values imputed using:
    -   `IterativeImputer` with `RandomForestRegressor` for numerical features
    -   Mode imputation for categorical features

---

### 3. 📈 Univariate analysis:

#### 🚶‍♂️ Survival count (`countplot`)

<p align="center">
    <img src="images/survival_count.png" alt="survival count" width="600"/>
</p>

#### 🛏️ Passenger Class Distribution (`countplot`)

<p align="center">
    <img src="images/passenger_class.png" alt="passenger class distribution" width="600"/>
</p>

#### 🧭 Age Distribution (`histplot`)

<p align="center">
    <img src="images/age_distribution.png" alt="age distribution" width="600"/>
</p>

#### 🧬 Sex Distribution (`countplot`)

<p align="center">
    <img src="images/sex_distribution.png" alt="sex distribution" width="600"/>
</p>

---

### 4. 📊 Bivariate analysis:

#### 🚶‍♂️ Survival rate **v/s** 🧬 Sex (`countplot`)

<p align="center">
    <img src="images/survival_rate_vs_sex.png" alt="survival rate vs sex" width="600"/>
</p>

#### 🚶‍♂️ Survival rate **v/s** 🛏️ Passenger Class (`countplot`)

<p align="center">
    <img src="images/survival_rate_vs_pclass.png" alt="survival rate vs passenger class" width="600"/>
</p>

#### 🚶‍♂️ Survival rate **v/s** 🧭 Age Group

<p align="center">
    <img src="images/survival_rate_vs_age.png" alt="survival rate vs age group" width="600"/>
</p>

---

### 5. 🔀 Multivariate Analysis

#### 🚶‍♂️ Survival rate **v/s** 🧬 Sex **v/s** 🛏️ Passenger Class (`catplot`)

<p align="center">
    <img src="images/multivariate_analysis.png" alt="survival rate vs sex vs passenger class" width="1000"/>
</p>

---

### 6. ❤️‍🩹 Survival Analysis

#### ⚓ Survival rate based on Embarkment point (`countplot`)

<p align="center">
    <img src="images/embarkment_point.png" alt="embarkment point" width="600"/>
</p>

#### 💵 Survival rate based on Fare charges (`histplot`)

<p align="center">
    <img src="images/fare_charges.png" alt="fare charges" width="600"/>
</p>

#### 👨‍👩‍👧‍👦 Survival rate based on Family size (`countplot`)

<p align="center">
    <img src="images/family_size.png" alt="family size" width="600"/>
</p>

#### 🧭 Survival rate based on Age group (`countplot`)

<p align="center">
    <img src="images/age_group.png" alt="age group" width="600"/>
</p>

---

### 7. 🔎 Advanced visualization (Correlation Heatmap)

-   Pearson correlation matrix for numerical features

<p align="center">
    <img src="images/correlation_heatmap.png" alt="correlation heatmap" width="1000"/>
</p>

---

## ✅ Conclusion

This visual analysis helps us understand what factors matter the most in the game of survival. The notebook delved deeper into the correlations between various factors like _age_, _sex_, _passenger class_, _embarkment points_, etc to evaluate survival rates.
