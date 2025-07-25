# 📊 Trade PnL Attribution & Risk Intelligence Dashboard

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)  
[![SQL](https://img.shields.io/badge/SQL-blue)](https://www.sql.org/)  
[![Power BI](https://img.shields.io/badge/Power%20BI-Data%20Visualization-yellow)](https://powerbi.microsoft.com/)  
[![AWS](https://img.shields.io/badge/AWS-Cloud-orange)](https://aws.amazon.com/)  
[![Apache Airflow](https://img.shields.io/badge/Apache%20Airflow-Workflow-blueviolet)](https://airflow.apache.org/)  
[![dbt](https://img.shields.io/badge/dbt-Data%20Transformation-lightgrey)](https://www.getdbt.com/)

---

## 🚀 Project Overview

This enterprise-grade dashboard simulates **trade Profit & Loss (PnL) attribution** workflows used by hedge funds and banks. It breaks down trade performance by **instrument, trader, and strategy**, providing detailed insights into key drivers such as market movement, FX impacts, execution slippage, and strategy logic.  

The dashboard integrates **anomaly detection** to flag unusual trade patterns, enabling risk and compliance teams to proactively monitor portfolio health and potential risks.

---

## 🛠️ Tech Stack

- **Python** (Pandas, NumPy) for data processing & modeling  
- **SQL** for data querying and transformation  
- **Power BI** for interactive, dynamic visualizations  
- **Apache Airflow** for orchestration and pipeline automation  
- **AWS Redshift & S3** for scalable cloud data storage and querying  
- **dbt** for modular, version-controlled data transformations  

---

## ⚙️ Key Features

- **Comprehensive PnL Attribution:** Break down trade PnL into Market Movement, FX, Execution Slippage, and Strategy Logic components  
- **Dynamic Drill-Down Dashboards:** Filter views by asset class, desk, trader, and timeframe for granular analysis  
- **Automated ETL Pipelines:** Data ingestion, transformation, and loading orchestrated via Airflow and dbt  
- **Anomaly Detection Module:** Identify and flag suspicious trade patterns and performance outliers leveraging statistical methods  
- **Scalable Cloud Architecture:** Utilizes AWS Redshift and S3 for handling multi-asset, large-scale datasets  

---

## 🎯 Getting Started

### Prerequisites

- Python 3.8+  
- Access to AWS services (Redshift, S3)  
- Power BI Desktop or Power BI Service  
- Apache Airflow setup  
- dbt CLI installed  

### Installation & Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/trade-pnl-dashboard.git
cd trade-pnl-dashboard

# Install Python dependencies
pip install -r requirements.txt

# Configure AWS credentials and Redshift access
# Set up Airflow connections and variables
# Initialize dbt models
dbt deps
dbt run

# Trigger Airflow DAGs to start pipelines

