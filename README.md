# Hospital Inpatient Charges & Efficiency Analysis (NY SPARCS 2022)

## **📌 Project Overview**

This project presents an in-depth analysis of the 2022 New York State SPARCS inpatient dataset. Using Python, I examined over 1 million discharge records to understand what drives hospital charges and operational efficiency.

The objective was to understand what actually drives hospital charges and how operational efficiency varies across different patient groups and clinical categories.

Instead of focusing only on visualizations, I aimed to extract practical business insights related to cost structure and hospital performance.

## **📂 Dataset Information**
* **Size:** 1M+ records
* **Source:** [New York State Department of Health (Health Data NY)] - (https://health.data.ny.gov/)
* [NY State Health Data Portal] - (https://health.data.ny.gov/Health/Hospital-Inpatient-Discharges-SPARCS-De-Identified/5dtw-tffi/about_data)
* **Key Features Used:** Facility Name, Age Group, Length of Stay (LOS), APR DRG (Diagnosis Groups), Severity of Illness, Total Costs, and Total Charges.

> [!IMPORTANT]  
> **Data Access:** Due to GitHub's file size limitations (the dataset exceeds 900MB), the raw CSV file is not included in this repository. To replicate this analysis, please download the 2022 SPARCS dataset directly from the official portal and place it in the project root.

## **🛠Tech Stack**
Language: Python 3.x

Libraries: Pandas, NumPy, Matplotlib, Seaborn

Dataset: 2022 NY State Statewide Planning and Research Cooperative System (SPARCS)

## **🚀 Key Analysis Phases**
Data Integrity & Cleaning: Handled missing values and standardized financial columns.

Filtering Strategy: Isolated core patient populations (e.g., stays < 30 days) to mitigate the "long-tail" effect of outliers.

Clinical Deep-Dive: Analyzed APR DRG and Severity of Illness (SOI) impact on total charges.

Efficiency Metrics: Engineered and tracked the Cost-to-Charge Ratio (CCR) as a KPI for operational performance.

Correlation Mapping: Quantified the relationship between Length of Stay (LOS) and financial outcomes.

## **📊 Key Business Insights**
Clinical Intensity vs. Volume: Identified that financial performance is driven more by the complexity of cases (Severity) than by the sheer number of patients.

The Efficiency Gap: Discovered that as patients age (50+), the Cost-to-Charge Ratio tightens, indicating higher operational costs relative to billed charges.

Revenue Drivers: Proved that managing procedural efficiency in high-acuity DRGs (Cardiac, Neonatology) is more impactful for margins than focusing solely on bed occupancy.

## 📈 Visualizations

### 1. Distribution of Total Charges (Histogram)
This histogram shows how total charges are distributed across all inpatient stays, helping to identify common billing ranges and outliers.  
![Total Charges Histogram](images/Distribution_of_Total_Charges_with_KD_Histogram.png)

### 2. Efficiency Trends by Age Group (Line Plot)
The line plot highlights the tightening of the Cost-to-Charge Ratio (CCR) in older demographics, signaling potential margin pressure and operational inefficiencies.  
![CCR by Age](images/Cost_to_Charge_Ratio_(CCR)_Trends_LinePlot.png)


### 3. Financial & Operational Correlation (Heatmap)
This heatmap illustrates the strong dependency between Length of Stay (LOS) and Total Costs, validating LOS as a primary operational lever.  
![Correlation Heatmap](images/Financial_Operational_Correlation_Heatmap.png)

## 🏁 Conclusion
The findings suggest that hospital margins are highly sensitive to case complexity, Length of Stay, and severity levels. Financial sustainability depends less on admission volume and more on managing high-cost, high-acuity populations efficiently.

Strategic focus on procedural efficiency and cost monitoring in complex DRGs may yield stronger financial improvements than volume-based growth strategies.
