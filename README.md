# 📊 Data Observability & Source ROI SDK

A modular, cloud-agnostic Python SDK designed to monitor, validate, and evaluate the health and ROI of data sources across any data pipeline — batch or streaming, pandas or Spark, on-prem or cloud.

---

## 🚀 Features

### 🔍 Data Observability
Implements the five pillars of observability:
- **Freshness** – Is the data arriving on time?
- **Volume** – Are we receiving the expected amount?
- **Schema** – Has the structure changed?
- **Distribution** – Are values within expected ranges?
- **Lineage** – Where does the data come from?

### 📈 Source ROI Framework
Quantifies vendor/source performance using:
- Freshness, Completeness, Usability
- Cost-efficiency, Error Rate, Rework Time
- Product Impact
- **ROI Score** = `w₁*(Usable%) + w₂*(Coverage%) - w₃*(Error%) - w₄*(Cost/GB)`

### 🧩 Plug-and-Play SDK
- Works with **pandas** and **Spark DataFrames**
- Supports **YAML-based rule configs**
- Emits metrics to any collector endpoint
- Easily integrates with **Airflow DAGs**

---

## 🗂️ Project Structure
data_observability_sdk/ 
├── config.py # Environment config 
├── emitter.py # Metric emission logic 
├── metrics.py # Observability metric computation 
├── roi.py # ROI score calculation 
├── rule_engine.py # YAML-based rule evaluation 
├── utils.py # Schema extraction, helpers 
├── sample_usage.py # Example with pandas 
├── spark_support.py # Spark DataFrame support 
├── airflow_dag.py # Airflow DAG integration 
└── rules.yaml # Sample rule definitions


