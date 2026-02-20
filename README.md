# BEES Data Engineering – Breweries Case

## 📌 Overview
This project implements a resilient and scalable Data Lake architecture consuming data from the Open Brewery DB API.

The solution follows the Medallion Architecture pattern with Bronze, Silver, and Gold layers.

## 🏗️ Architecture

### Data Flow

1. Data ingestion from Open Brewery API
2. Raw data persisted in Bronze layer
3. Data transformation and partitioning in Silver layer (Parquet format)
4. Aggregated data in Gold layer

## 🥉 Bronze Layer
Stores raw API data in its original JSON format.

## 🥈 Silver Layer
- Converts data to columnar format (Parquet)
- Applies data cleaning and transformation
- Partitions data by brewery location

## 🥇 Gold Layer
Aggregated dataset containing brewery count by type and location.

## 🛠️ Technologies
- Python
- Pandas / PySpark (depending on scalability needs)
- Parquet
- Apache Airflow (orchestration)
- Docker (containerization)

## 🚀 How to Run
Instructions will be provided after implementation.