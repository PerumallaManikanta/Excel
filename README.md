# 🏥 Healthcare Data Analysis and Insights

## 📌 Project Introduction

**Healthcare Data Analysis and Insights** is an Excel-based data analytics project focused on analyzing healthcare data to identify meaningful patterns related to patient health profiles, medical history, hospitalization information, and healthcare costs.

The project applies **data cleaning, data transformation, exploratory analysis, pivot tables, visualization, and dashboard development** to convert raw healthcare data into actionable insights.

The analysis is designed to support healthcare stakeholders in understanding patient characteristics, health conditions, healthcare charges, and relationships between different health metrics.

---

## 🎯 Problem Statement

The healthcare industry generates large amounts of data from medical examinations, hospitalization records, and customer profiles.

However, raw healthcare data often contains missing values, inconsistent formats, non-numeric values, and information that requires transformation before meaningful analysis can be performed.

This project focuses on cleaning and transforming healthcare data and analyzing relationships between:

* Patient demographics
* BMI and weight status
* HbA1C and diabetes status
* Smoking behavior
* Cancer history
* Heart issues
* Major surgeries
* Transplants
* Hospital tier
* City tier
* State
* Healthcare charges

The ultimate objective is to identify trends and patterns that can support informed healthcare decision-making.

---

## 🎯 Business Objectives

The major objectives of this project are:

1. Clean and prepare the healthcare dataset for analysis.
2. Identify and handle missing values.
3. Standardize inconsistent healthcare-related fields.
4. Transform raw fields into meaningful analytical categories.
5. Create patient-level health indicators.
6. Analyze healthcare charges across different patient groups.
7. Understand relationships between age, BMI, HbA1C, and healthcare charges.
8. Compare healthcare charges across hospital tiers and states.
9. Analyze health conditions based on smoking and transplant history.
10. Build an interactive healthcare dashboard for decision-making.

---

# 📂 Dataset Information

The project uses healthcare data consisting of three primary tables:

* **Medical Examinations**
* **Hospitalization Details**
* **Customer Names**

The three tables are connected using **Customer ID** as the common field.

### Dataset Download

The original project source provides the dataset through Google Drive.

---

# 🗂️ Data Preparation

## 1. Data Cleaning

The following cleaning activities were performed/planned as part of the project:

### Missing Value Treatment

Missing values represented by `?` were identified in:

* Medical Examinations table
* Hospitalization Details table

The project specifies the following treatment strategies:

| Column        | Treatment                                                                 |
| ------------- | ------------------------------------------------------------------------- |
| Month         | Fill missing values with `Sep`                                            |
| Year          | Fill missing values using the average year rounded to the nearest integer |
| Smoker        | Fill missing values using the most frequent value                         |
| Hospital Tier | Fill missing values using the most frequent value                         |
| City Tier     | Fill missing values using the most frequent value                         |
| State ID      | Use `Unknown` or another appropriate treatment                            |

---

# 🔄 Data Transformation

Several transformations were performed to make the raw healthcare data suitable for analysis.

## Customer Name Transformation

The `Names` column was split into:

* Title
* First Name
* Last Name

## Major Surgeries

The `NumberOfMajorSurgeries` column was converted into numerical data by replacing non-numeric values with meaningful numerical representations.

## Data Consistency

Potential inconsistencies in:

* Heart Issues
* Smoker

were checked and corrective actions were considered.

---

# ⚖️ Feature Engineering

## Weight Status

A new calculated field named **Weight Status** was created using BMI.

|            BMI | Weight Status |
| -------------: | ------------- |
|     Below 18.5 | Underweight   |
|    18.5 – 24.9 | Normal Weight |
|    25.0 – 29.9 | Overweight    |
| 30.0 and Above | Obesity       |

## Diabetes Status

A new field named **Diabetes Status** was created using HbA1C values.

|         HbA1C | Diabetes Status |
| ------------: | --------------- |
|     Below 5.7 | Normal          |
|     5.7 – 6.4 | Prediabetes     |
| 6.5 and Above | Diabetes        |

## Date of Birth

The following fields were combined:

* Year
* Month
* Date

into a single **Date of Birth** field.

The resulting date was formatted as:

`DD-MMM-YYYY`

## Age Calculation

Customer age was calculated using the Date of Birth and the dataset collection date:

**8 June 2023**.

## Healthcare Charges

The `charges` field was formatted as currency in **USD ($)**.

---

# 📊 Data Integration

A new Excel sheet named **Healthcare** was created to consolidate relevant information from the three source tables.

The tables were combined using:

**Customer ID**

The project specifies the use of **VLOOKUP** for integrating the required fields.

### Final Analytical Fields

The consolidated Healthcare dataset contains the following important fields:

* Customer ID
* First Name
* BMI
* HBA1C
* Heart Issues
* Any Transplants
* Cancer History
* Number of Major Surgeries
* Smoker
* Weight Status
* Diabetes Status
* Date of Birth
* Charges
* Hospital Tier
* City Tier
* State ID
* Age

---

# 🔍 Exploratory Data Analysis

The analysis focuses on understanding healthcare patterns and identifying relationships between patient health characteristics and healthcare costs.

## Key Analytical Questions

### Smoking & Cancer

**How does cancer history differ between smokers and non-smokers?**

A Pie/Donut chart can be used to compare cancer-history distribution between smoking groups.

---

### Transplants & Medical Conditions

**How do total major surgeries and average HbA1C differ between patients with and without a history of transplants?**

This analysis helps compare medical complexity and HbA1C levels across transplant groups.

---

### Weight Status & Diabetes

**How do healthcare charges vary across different Weight Status and Diabetes Status categories?**

This analysis helps identify differences in healthcare costs across patient health categories.

---

### Hospital Tier & State

**How does the average healthcare charge vary by Hospital Tier across different states?**

This analysis provides a comparison of healthcare costs across geographic and hospital-level categories.

---

### Age & Health Metrics

The project explores whether there is a relationship between:

* Age and BMI
* Age and HbA1C
* Age and healthcare charges

Scatter plots can be used to identify potential relationships and patterns.

---

# 📈 Visualizations

The project uses different chart types according to the analytical question.

| Visualization      | Purpose                                      |
| ------------------ | -------------------------------------------- |
| Pie / Donut Chart  | Cancer history among smokers and non-smokers |
| Pie / Donut Chart  | Transplant-related comparison                |
| Column / Bar Chart | Charges by Weight Status                     |
| Column / Bar Chart | Charges by Diabetes Status                   |
| Bar Chart          | Average charges by Hospital Tier and State   |
| Scatter Plot       | Age vs BMI                                   |
| Scatter Plot       | Age vs HbA1C                                 |
| Scatter Plot       | Age vs Healthcare Charges                    |

These visualizations are designed to make healthcare trends and cost patterns easier to interpret.

---

# 📊 Dashboard Design

An interactive **Healthcare Dashboard** was designed to consolidate the major analytical findings into a single view.

### Dashboard Components

The dashboard focuses on:

* Patient health profile
* Weight Status
* Diabetes Status
* Smoking behavior
* Cancer history
* Transplant history
* Major surgeries
* Hospital tier
* State-level healthcare charges
* Age-related health patterns
* Healthcare charges

---

# 🎛️ Interactive Filters

Two important slicers are included:

### 1. Weight Status

Users can filter the dashboard based on:

* Underweight
* Normal Weight
* Overweight
* Obesity

### 2. Diabetes Status

Users can filter the dashboard based on:

* Normal
* Prediabetes
* Diabetes

These slicers allow users to compare health outcomes and healthcare charges dynamically.

---

# 💡 Key Insights

The project is designed to identify insights around:

* Cancer history among smokers and non-smokers.
* Differences in major surgeries between transplant and non-transplant patients.
* Differences in average HbA1C across transplant groups.
* Healthcare charges across different weight categories.
* Healthcare charges across diabetes categories.
* Differences in average charges between hospital tiers.
* State-level healthcare charge variations.
* Relationships between age and BMI.
* Relationships between age and HbA1C.
* Relationship between age and healthcare charges.

> **Note:** Specific numerical findings should be added after the final Excel analysis is completed. The source project defines the analytical questions but does not provide the resulting numerical findings.

---

# 💼 Business Recommendations

Based on the analytical framework of the project, healthcare stakeholders can use the dashboard to:

1. Monitor healthcare cost differences across patient health categories.
2. Identify patient groups associated with higher healthcare charges.
3. Compare healthcare costs across hospital tiers.
4. Investigate geographic differences in healthcare expenditure.
5. Monitor relationships between age and important health metrics.
6. Use patient health indicators to support resource planning.
7. Use interactive filtering to investigate specific patient segments.

These recommendations are intended as analytical use cases; specific recommendations should be finalized after reviewing the actual numerical results.

---

# 📌 Business Impact

The project demonstrates how healthcare data can be transformed into an analytical decision-support solution.

Potential business impact includes:

* Better understanding of healthcare cost patterns.
* Improved visibility into patient health profiles.
* Identification of important health-related trends.
* Improved comparison of hospital and geographic costs.
* More effective healthcare resource planning.
* Faster access to meaningful healthcare information.
* Improved data-driven decision-making.

---

# ⚠️ Challenges Faced

The major challenges addressed in this project include:

* Handling missing values represented by `?`.
* Converting inconsistent data into usable formats.
* Cleaning non-numeric surgery values.
* Splitting customer names correctly.
* Creating meaningful BMI categories.
* Creating diabetes categories from HbA1C.
* Combining multiple date fields.
* Calculating customer age.
* Integrating multiple tables using Customer ID.
* Selecting appropriate visualizations for each analytical question.
* Designing an interactive dashboard that remains easy to interpret.

---

# ⚠️ Limitations

The project has several limitations:

* The analysis is dependent on the quality of the provided dataset.
* Missing or inconsistent values may affect analytical accuracy.
* Healthcare charges alone may not explain the complete cost structure.
* Correlation analysis does not establish causation.
* The dataset may not represent the entire healthcare population.
* The analysis is based on the available fields and historical dataset information.

---

# 🚀 Future Scope

The project can be further enhanced by:

* Automating the data-cleaning process.
* Adding more advanced statistical analysis.
* Performing predictive healthcare-cost analysis.
* Developing patient-risk segmentation.
* Adding time-based healthcare trend analysis.
* Building the solution in Power BI or Tableau.
* Adding automated KPI monitoring.
* Developing machine-learning models for healthcare cost prediction.
* Creating more advanced geographic analysis.

---

# 🛠️ Tools & Skills Demonstrated

### Tools

* Microsoft Excel
* Excel Pivot Tables
* Excel VLOOKUP
* Excel Charts
* Excel Slicers

### Technical Skills

* Data Cleaning
* Data Transformation
* Data Integration
* Feature Engineering
* Exploratory Data Analysis
* Pivot Table Analysis
* Data Visualization
* Dashboard Development
* Healthcare Data Analysis

### Analytical Skills

* Problem Solving
* Data Interpretation
* Pattern Identification
* Business Question Development
* Insight Generation
* Data-Driven Decision Making

---

# 📁 Project Structure

```text
Healthcare-Data-Analysis/
│
├── Dataset/
│   └── Healthcare Dataset.xlsx
│
├── Dashboard/
│   └── Healthcare Dashboard.xlsx
│
├── Documentation/
│   └── Healthcare Analysis Report.pdf
│
├── Screenshots/
│   └── Healthcare Dashboard.png
│
└── README.md
```

---

# 📷 Dashboard Preview

Add your final dashboard screenshot here:

```markdown
![Healthcare Dashboard](Screenshots/Healthcare-Dashboard.png)
```

---

# 🎓 Project Outcome

This project demonstrates an end-to-end **Excel Data Analytics workflow**, starting from raw healthcare data and progressing through:

**Raw Data → Data Cleaning → Data Transformation → Feature Engineering → Data Integration → EDA → Visualization → Dashboard → Business Insights**

The project highlights the ability to transform complex healthcare data into a structured and interactive analytical solution.

---

# 👨‍💻 Author

**Manikanta**

Aspiring **Data Analyst** with a focus on developing practical skills in:

* Excel
* SQL
* Power BI
* Python
* Data Visualization
* Business Analytics

This project is part of my data analytics portfolio and demonstrates my ability to work with real-world-style datasets, clean and transform data, perform exploratory analysis, create dashboards, and communicate analytical findings.

---

# 📌 Final Project Statement

> **Healthcare Data Analysis and Insights** demonstrates how raw healthcare data can be cleaned, transformed, analyzed, and visualized to uncover meaningful patterns in patient health profiles and healthcare costs.

The project combines **Excel data preparation, analytical techniques, visualization, and interactive dashboard design** to create a practical healthcare analytics solution for data-driven decision-making.
