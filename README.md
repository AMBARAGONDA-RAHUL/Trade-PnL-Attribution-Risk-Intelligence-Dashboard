
# Trade PnL Attribution & Risk Intelligence Dashboard

[![Python](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)  [![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-green)(https://powerbi.microsoft.com/)  [![AWS](https://img.shields.io/badge/AWS-Cloud-orange)](https://aws.amazon.com/)  
[![Apache Airflow](https://img.shields.io/badge/Apache-Airflow-blue)](https://airflow.apache.org/)  [![dbt](https://img.shields.io/badge/dbt-Data%20Transformation-lightgrey)](https://www.getdbt.com/)
---

## 🚀 Project Overview

Trade PnL Attribution & Risk Intelligence Dashboard is a professional-grade solution designed to simulate real-world hedge fund and banking workflows by breaking down trade gains and losses across multiple dimensions—trader, instrument, strategy, and asset class.  

It provides actionable portfolio-level insights by integrating multi-asset trade data, automated ETL pipelines, and anomaly detection for suspicious trade patterns. The solution is built using industry-standard tools to demonstrate strong domain knowledge and technical depth.

---

## 🛠️ Tech Stack

- **Data Engineering & Orchestration:** Apache Airflow, dbt, Python (Pandas, SQLAlchemy)  
- **Cloud:** AWS (Redshift, S3, Lambda)  
- **Visualization:** Power BI  
- **Databases & Storage:** AWS Redshift, S3  
- **Programming Languages:** Python, SQL  

---

## ⚙️ Features

- **Multi-Asset Trade Data Simulation:** Generate realistic trade datasets covering market movement, FX, execution slippage, and strategy logic.  
- **PnL Attribution Pipelines:** Automated ETL pipelines break down PnL by key factors such as trader, desk, asset class, and strategy.  
- **Dynamic Power BI Dashboards:** Interactive dashboards with filtering capabilities for portfolio-level trade and risk insights.  
- **Anomaly Detection:** Integrated machine learning models to flag suspicious trade patterns and performance outliers.  
- **Pipeline Automation:** Fully orchestrated workflows using Apache Airflow and version-controlled transformations via dbt.  

---

## 🎯 Getting Started

### Prerequisites

- Python 3.8+  
- Access to AWS services (Redshift, S3)  
- Power BI Desktop or Power BI Service  
- Apache Airflow installed and configured  
- dbt CLI installed  

---

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/trade-pnl-dashboard.git
cd trade-pnl-dashboard
````

---

### Step 2: Set Up Python Environment

```bash
# (Optional) Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install required Python packages
pip install -r requirements.txt
```

---

### Step 3: Configure AWS and Database Access

* Configure AWS CLI with your credentials:

```bash
aws configure
```

* Ensure you have access and credentials set for AWS Redshift and S3 buckets used in the project.
* Update Airflow connection details (`airflow.cfg` or via UI) with your AWS and database credentials.

---

### Step 4: Initialize dbt Models

```bash
cd dbt
dbt deps         # Install dependencies
dbt seed         # Load seed data (if any)
dbt run          # Run data transformations
dbt test         # Run tests to verify models
```

---

### Step 5: Set Up Airflow Pipelines

* Place the DAG files located in `/airflow/dags` into your Airflow DAGs folder.
* Start Airflow scheduler and webserver:

```bash
airflow scheduler
airflow webserver
```

* Trigger DAGs manually or schedule automated runs via the Airflow UI.

---

### Step 6: Load Power BI Dashboard

* Open `powerbi/Trade_PnL_Dashboard.pbix` in Power BI Desktop.
* Connect to your Redshift data source using appropriate credentials.
* Use filters and slicers to explore PnL attribution by asset class, trader, and strategy.

---

### Step 7: Monitor and Analyze

* Use the dashboard for real-time trade PnL insights and risk anomaly detection.
* Review Airflow logs and dbt runs regularly to ensure smooth pipeline operation.

---

## 📊 Project Structure

```
trade-pnl-dashboard/
├── airflow/                  # Apache Airflow DAGs and configs
│   └── dags/
├── dbt/                      # dbt project files (models, seeds, tests)
├── powerbi/                  # Power BI dashboard files (.pbix)
├── scripts/                  # Python scripts for data simulation & ETL
├── requirements.txt          # Python dependencies
├── README.md                 # This file
└── .gitignore
```

---

## 🤝 Contributions

Contributions, suggestions, and improvements are welcome! Feel free to open an issue or submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

