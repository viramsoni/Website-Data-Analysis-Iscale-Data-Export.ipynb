# 🌐 Web Traffic Channels & User Engagement Analytics

An end-to-end exploratory data analysis (EDA) pipeline engineered in Python to process multi-channel web export traffic data, parse structural datetimes, and map user behavior distributions.

## 📊 Project Artifacts & Reports
* 🚀 **Interactive Analysis:** [View Jupyter Notebook](./Website-Data-Analysis-Project.ipynb)
* 📄 **Executive Document:** [Download Complete PDF Report](./Website-Data-Analysis-Project.pdf) *(Visual Export Mirror)*

## ⚙️ Dataset Architecture & Setup
The repository contains web traffic granular logs provided by the iScale curriculum. Mirror this directory layout to execute code locally:

```text
├── data/
│   └── Website- Data Analysis - Iscale data-export.csv <-- raw data here
├── Website-Data-Analysis-Project.ipynb
├── Website-Data-Analysis-Project.pdf
└── README.md
```

## ⚙️ Data Engineering & Pipeline Steps

### 1. Data Ingestion & Schema Correction
* **Header Alignment:** Cleaned corrupted structural grids by dynamically mapping implicit row headers (`df.columns = df.iloc[0]`).
* **Type Casting & Optimization:** Converted raw sequence tracking indexes into explicit `datetime64` vector blocks (`%Y%m%d%H`) and isolated hours.强制 mapped numeric string vectors into optimized float variables.

### 2. Exploratory Data Analysis (EDA)
* **Traffic Volatility Monitoring:** Evaluated overall `Sessions` and `Users` timelines to spot conversion spikes.
* **Engagement Evaluation:** Calculated metric summary frames across categorical channels to trace engagement rates and mean interaction frequencies.

## 📊 Core Data Insights & Visualizations
* **Volume Leader:** **Organic Social** commands the absolute highest volume of total users, closely followed by Direct and Organic Search traffic.
* **Engagement Winner:** **Referral and Organic Video channels** drive the highest median engagement times per session, indicating exceptionally high traffic quality.
* **Hourly Spikes:** Developed an absolute traffic density **Heatmap (Hour vs Channel)** proving performance peak clusters between 10:00 AM and 11:00 PM.
* **Metric Interaction:** Tracked continuous **Engagement Rate % vs Total Sessions** profiles to isolate growth patterns over time.

---
*Completed as a hands-on portfolio piece via the iScale Data Analytics Program.*
