# GlobalRetail Databricks Data Lakehouse Project

This project is based on a case study of GlobalRetail, a multinational retail corporation with operations in 27 countries. GlobalRetail generates massive amounts of data across various channels and faces challenges with data consolidation, quality, and analytics. This project aims to address these challenges by implementing a modern data lakehouse architecture using Databricks and Delta Lake.

## Table of Contents

- [Project Overview](#project-overview)
- [Architecture](#architecture)
- [Data Sources](#data-sources)
- [Objectives](#objectives)
- [Layers](#layers)
  - [Raw Data Layer](#raw-data-layer)
  - [Master Data Layer](#master-data-layer)
  - [Reporting Layer](#reporting-layer)
- [Technologies Used](#technologies-used)
- [Setup Instructions](#setup-instructions)
- [Project Components](#project-components)

## Project Overview

GlobalRetail faces challenges in managing and analyzing data effectively due to varying data formats, large volumes of historical data, and complex ETL requirements. This project builds a data lakehouse on Databricks to improve data processing times, forecast accuracy, and customer personalization, while providing near-real-time financial reporting across regions.

## Architecture

The project follows a multi-layer architecture, consisting of three primary layers: Bronze, Silver, and Gold. Data flows through these layers to enhance quality, enrich content, and prepare for business intelligence.

![Architecture Diagram](link_to_diagram.png)

1. **Raw Data Layer:** Ingests raw data from multiple sources (CSV, JSON, Parquet).
2. **Master Data Layer:** Processes and cleanses data to address quality issues and aligns formats.
3. **Reporting Layer:** Creates a unified customer view and prepares data for analytics.

## Data Sources

- **Customer Data:** CSV format from CRM, ~500 million records.
- **Product Catalog:** JSON format from the inventory system, ~500,000 SKUs.
- **Transaction History:** Parquet format from POS and e-commerce, ~10 billion transactions annually.

## Objectives

- **Reduce Data Processing Time:** From 72 hours to under 6 hours.
- **Improve Forecasting Accuracy:** Enhance inventory forecasting by 25%.
- **Boost Customer Personalization:** Target a 15% increase in repeat purchases.
- **Enable Real-Time Reporting:** Support near real-time financial reporting.

## Layers

### Raw Data Layer
The Raw Data Layer ingests raw data in its original format (CSV, JSON, Parquet) to the Databricks File System (DBFS).

### Master Data Layer
The Master Data layer standardizes, cleans, and transforms data based on business rules to improve data quality and format consistency.

### Reporting Layer
The Reporting Layer provides a unified customer view across regions and channels, enabling company-wide analytics and reporting.

## Technologies Used

- **Databricks**: Unified data analytics platform for big data and machine learning.
- **Delta Lake**: Open-source storage layer providing ACID transactions.
- **Power BI**: Visualization tool for reporting and dashboards.

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/kandelsatish/GlobalRetail.git
   cd GlobalRetail-DataLakehouse
