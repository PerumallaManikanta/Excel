# 📊 Data Cleaning & Transformation Guide

> A professional reference for preparing, standardizing, transforming, and presenting the dataset.

---

## 🎯 Overview

This workbook focuses on improving the **quality, consistency, structure, and presentation** of the data.

The cleaning process covers:

- 🧹 Missing-value handling
- ✏️ Data standardization
- 🗑️ Duplicate removal
- 🔄 Data splitting and merging
- 💵 Number and date formatting
- 🎨 Conditional formatting

---

## 📁 Workbook Structure

| Worksheet | Purpose |
|---|---|
| `Instructions` | Provides the required data-cleaning and transformation guidelines |
| `Dataset` | Contains the data to be cleaned, transformed, and formatted |

---

# 🧹 1. Missing Values

### 💰 Price

Review the **Price ($)** column for missing values and apply an appropriate, consistent method for handling them.

The selected approach should maintain the reliability of the dataset and avoid introducing arbitrary information.

### 🏷️ Category

Review the **Category** column for missing values.

Use an appropriate strategy to impute or otherwise handle missing category information consistently.

---

# ✏️ 2. Data Standardization

### 📝 Product Name

Review the **Product Name** column for inconsistencies such as:

- Capitalization
- Spacing
- Text variations
- Other formatting differences

Use **Find and Replace** where appropriate to standardize the product names.

### 🏷️ Category

Review the **Category** column for:

- Spelling mistakes
- Typos
- Inconsistent category names

Use **Find and Replace** to correct identified issues and ensure equivalent categories are represented consistently.

---

# 🗑️ 3. Duplicate Records

Check the dataset for duplicate records.

### 🔎 Duplicate-checking rule

A duplicate should be evaluated using the **entire row**, rather than relying on only one field.

Remove complete duplicate rows where applicable and verify that valid unique records remain unchanged.

---

# 🔄 4. Data Transformation

## 🆔 Product ID

Separate the information contained in **Product ID** into two dedicated fields:

- 📅 **Manufacturing Date**
- 🌍 **Country Code**

Remove unnecessary characters as part of the transformation and verify that the extracted values are accurate and consistently structured.

---

## 🏢 Product Brand

Combine:

**Brand Name + Product Name**

into a single column named:

**Product Brand**

The combined value should clearly preserve both the brand and product information.

---

# 💵 5. Number & Date Formatting

### 💰 Price

Format the **Price ($)** column as **Currency**.

Use a consistent currency presentation across the dataset.

### 📅 Manufacturing Date

Format **Manufacturing Date** using:

**DD-MM-YYYY**

Example:

`25-08-2026`

Consistent date formatting improves readability and makes the dataset easier to analyze.

---

# 🎨 6. Conditional Formatting

## 💰 Price Visualization

Apply either:

- 📊 **Data Bars**, or
- 🌈 **Color Scales**

to the **Price ($)** column.

This provides a quick visual representation of differences in product prices.

---

## 🔌 Electronics Highlighting

Create a **custom conditional-formatting rule** for the **Category** column.

The rule should highlight every cell where the category is:

**Electronics**

This makes the selected category immediately visible within the dataset.

---

# 🔍 Final Review Checklist

Before finalizing the cleaned dataset, confirm that:

- [ ] 🧹 Missing `Price ($)` values have been reviewed and handled appropriately.
- [ ] 🏷️ Missing `Category` values have been reviewed and addressed appropriately.
- [ ] 📝 Inconsistent `Product Name` values have been standardized.
- [ ] ✏️ Category typos and spelling inconsistencies have been corrected.
- [ ] 🗑️ Complete duplicate rows have been checked and removed where applicable.
- [ ] 🆔 `Product ID` has been separated into `Manufacturing Date` and `Country Code`.
- [ ] 🧹 Unnecessary characters have been removed from the transformed data.
- [ ] 🏢 `Brand Name` and `Product Name` have been combined into `Product Brand`.
- [ ] 💵 `Price ($)` is displayed in Currency format.
- [ ] 📅 `Manufacturing Date` is displayed as `DD-MM-YYYY`.
- [ ] 📊 Data Bars or a Color Scale have been applied to `Price ($)`.
- [ ] 🔌 `Electronics` entries are highlighted using a custom conditional-formatting rule.
- [ ] ✅ The complete dataset has been reviewed for accuracy and consistency.

---

# 🏆 Expected Outcome

The final dataset should be:

**🧹 Clean → 📋 Consistent → 🔄 Well-structured → 🎨 Visually clear → 📊 Ready for analysis**

A properly prepared dataset should contain standardized values, appropriately handled missing information, no complete duplicate records, correctly transformed fields, consistent formatting, and useful visual indicators.

---

## 📌 Data Quality Principle

> **Clean accurately. Transform carefully. Format consistently.**

Every change should improve the usability and consistency of the data while preserving valid underlying information.

---

### ✨ Data Preparation Workflow

**🔍 Inspect → 🧹 Clean → ✏️ Standardize → 🗑️ Deduplicate → 🔄 Transform → 💵 Format → 🎨 Visualize → ✅ Review**
