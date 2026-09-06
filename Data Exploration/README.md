# 📊 Product Data Analysis Workbook

## 👋 Overview

This workbook provides a structured approach to analyzing product information using Microsoft Excel. It combines product details, calculated values, conditional analysis, and Product ID text extraction in a clear and organized format.

The workbook contains the following sheets:

- **Instructions**
- **Dataset**

---

## 📋 Workbook Contents

The main data sheet contains product-related fields such as:

- 🆔 **Product ID**
- 📦 **Product Name**
- 🏷️ **Brand Name**
- 💲 **Price ($)**
- 🔢 **Quantity**
- 🗂️ **Category**
- 💰 **Total Price**
- 📊 **Price Range**
- 💻 **Category-based calculations**
- 🔎 **Conditional counts**
- 📅 **Day, Month, and Country Code** extracted from Product ID

> **Note:** The exact column names and layout are retained from the workbook so the README can be used alongside the spreadsheet without changing its structure.

---

## 🧮 Calculations & Analysis

The workbook demonstrates practical Excel data-analysis techniques, including:

### 💰 Total Price

The total value for each product is calculated using:

`Total Price = Price × Quantity`

This makes it possible to evaluate the overall value associated with each product record.

### 📈 Summary Statistics

The workbook includes calculations for key price statistics, such as:

- 💵 Total value
- 🔢 Product count
- 📊 Average price
- ⬇️ Minimum price
- ⬆️ Maximum price

### 🏷️ Price Range Classification

Products are categorized according to their price using conditional logic. This makes it easier to distinguish higher-priced products from standard-priced products.

### 🔎 Conditional Analysis

Functions such as `SUMIF` and `COUNTIF` are used to analyze the dataset based on specific conditions, including product category and price thresholds.

### ✂️ Product ID Extraction

The Product ID contains multiple pieces of information. Excel text functions are used to extract individual components such as:

- 📅 Day
- 🗓️ Month
- 🌍 Country Code

Common functions used for this type of extraction include:

`LEFT()` · `MID()` · `RIGHT()`

---

## 🛠️ Excel Functions Demonstrated

The workbook demonstrates the practical use of:

| Function | Purpose |
|---|---|
| `SUM()` | Adds numerical values |
| `COUNT()` | Counts numerical records |
| `AVERAGE()` | Calculates the average |
| `MIN()` | Finds the minimum value |
| `MAX()` | Finds the maximum value |
| `IF()` | Applies conditional logic |
| `SUMIF()` | Calculates totals based on a condition |
| `COUNTIF()` | Counts records based on a condition |
| `LEFT()` | Extracts characters from the beginning of text |
| `MID()` | Extracts characters from a specified position |
| `RIGHT()` | Extracts characters from the end of text |

---

## 📊 Data Analysis Workflow

```text
📥 Product Data
      │
      ▼
🧹 Structured Dataset
      │
      ▼
🧮 Excel Formulas
      │
      ├── 💰 Total Price
      ├── 🏷️ Price Classification
      ├── 🔎 Conditional Analysis
      └── ✂️ Product ID Extraction
      │
      ▼
📈 Summary & Insights
```

---

## 🚀 How to Use This Workbook

1. Open the workbook in **Microsoft Excel**.
2. Review the instructions and dataset sheets.
3. Explore the original product information.
4. Review the calculated columns and formulas.
5. Examine the summary results to understand the overall dataset.
6. Modify or extend the source data when required, ensuring formulas are copied correctly for new records.

---

## ✨ Key Features

- 📊 Structured product dataset
- 🧮 Formula-based calculations
- 🔎 Conditional data analysis
- 🏷️ Automated price classification
- ✂️ Text extraction from Product IDs
- 📈 Summary statistics
- 📋 Clear spreadsheet organization
- 💼 Suitable for demonstrating practical Excel data-analysis skills

---

## 📁 File Structure

```text
📊 Product Data Analysis Workbook
│
├── 📋 Instructions
│   └── Reference information and required analysis
│
└── 📊 Dataset
    ├── Product information
    ├── Calculated values
    ├── Conditional analysis
    ├── Price classification
    └── Product ID components
```

---

## 💡 Purpose

This workbook is designed to demonstrate how raw product information can be organized, calculated, and analyzed using standard Excel functions. The combination of formulas and structured data provides a simple foundation for understanding spreadsheet-based data analysis.

---

## 📝 Notes

- Keep the original data structure intact when adding new records.
- Verify that formulas are extended to any newly added rows.
- Use consistent formats for prices, quantities, categories, and Product IDs.
- Review calculated results after making changes to the source data.

---

### 🌟 Professional Spreadsheet Reference

A well-structured workbook makes data easier to understand, analyze, and maintain. This README provides a quick reference to the workbook's purpose, organization, calculations, and Excel techniques used throughout the file.
