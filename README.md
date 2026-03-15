# 🏠 House Price Prediction – Lahore, Pakistan

**AI/ML Engineering Internship – Task 6**  
**Developer:** [Your Name]  
**Organization:** Developers Hub Corporation  

---

## 📌 Project Overview

This project focuses on predicting residential property prices in **Lahore, Pakistan** using the **Zameen Lahore Dataset**. The regression pipeline analyzes how features like **location, size, and utility ratios** impact market valuation in the current 2026 real estate landscape.  

---

## 📊 Dataset Specifications

- **Source:** Zameen Lahore Real Estate Data (CSV)  
- **Target Variable:** `Price_thnds` (Converted to PKR Millions for evaluation)  
- **Key Features:**
  - `Area_sqft`: Total land/built-up area  
  - `Beds` & `Baths`: Total room count  
  - `locality_enc`: Label-encoded geographical sectors  
  - `bath_bed_ratio`: Engineered feature highlighting luxury utility  
  - `area_log`: Log-transformed area to handle outliers and variance  

---

## 🛠️ Models & Methodology

Two models were implemented for comparative analysis:

### 1. Linear Regression (LR)
- Baseline model  
- Features scaled via `StandardScaler`  
- Captures linear trends in housing prices  

### 2. Gradient Boosting Regressor (GBR)
- Non-linear ensemble model  
- Tuned with **300 estimators** and **max depth 4**  
- Captures complex market patterns and non-linear interactions  

---

## 📈 Model Performance

| Metric | Linear Regression | Gradient Boosting |
|--------|-----------------|-----------------|
| **R² Score** | 0.5234 | 0.7652 |
| **MAE** | PKR 32.36 Million | PKR 16.96 Million |
| **RMSE** | PKR 53.56 Million | PKR 37.59 Million |
| **MAPE** | 87.4% | 24.4% |

> Gradient Boosting Regressor clearly outperforms the linear model, capturing the nuances of Lahore's property market.  

---

## 💡 2026 Lahore Market Insights

- **Top Performing Localities:**
  - **DHA Lahore (Phases 5, 6, & 8):** High-value zones due to modern infrastructure and strong rental demand  
  - **Gulberg:** Luxury high-rise and vertical living driving prices  
  - **Bahria Town / Orchard:** Hotspots for high ROI with new skyscraper developments  

- **Shift to "On-Ground" Assets:** Possession-ready properties favored over speculative files  

- **Infrastructure Impact:** Proximity to **Lahore Ring Road** and **Orange Line Metro** significantly increases property values  

- **Construction Costs:** Rising cement and steel costs have increased the base price of new constructions  

---

## 📂 Submission Requirements & Metadata

- **Internship:** AI/ML Engineering (Developers Hub Corporation)  
- **Task:** 6 of 6 (House Price Prediction)  
- **Due Date:** April 3rd, 2026  
- **Tools Used:** Python, Scikit-Learn, Pandas, Matplotlib, Seaborn  

---

## 🚀 How to Use

```bash
# Clone the repository
git clone https://github.com/yourusername/DH-Internship-Tasks.git

# Navigate to project directory
cd DH-Internship-Tasks

# Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn

# Run the Jupyter Notebook
jupyter notebook Untitled.ipynb
