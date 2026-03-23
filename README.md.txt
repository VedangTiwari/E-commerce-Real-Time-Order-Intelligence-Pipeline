# Snowflake Data Pipeline (Hackathon Project)

## 📌 Overview

This project implements a complete **data pipeline using Snowflake** following the Medallion Architecture:

* Bronze → Raw ingestion
* Silver → Data cleaning & transformation
* Gold → Business-ready tables
* Streams → Change Data Capture
* Tasks → Automation

---

## 🏗️ Architecture

Raw Data → Bronze → Silver → Gold → Stream → Task → Final Table

---

## ⚙️ Tech Stack

* Snowflake
* SQL
* Streams & Tasks

---

## 📂 Project Structure

```
sql/
 ├── 1_setup.sql
 ├── 2_bronze.sql
 ├── 3_silver.sql
 ├── 4_gold.sql
 ├── 5_streams.sql
 ├── 6_tasks.sql
 └── 7_demo.sql
```

---

## 🔄 Pipeline Flow

1. Load raw data into Bronze layer
2. Clean and transform into Silver layer
3. Create final analytical tables in Gold layer
4. Use Streams to track new data
5. Use Tasks to automate incremental processing

---

## ⚡ Key Features

* Incremental data processing
* No duplicate handling using MERGE
* Real-time automation with Streams & Tasks
* Scalable architecture

---

## ▶️ How to Run

Run SQL files in order:

1 → 2 → 3 → 4 → 5 → 6 → 7

---

## 🎯 Demo

Insert new data into `clean_orders`
Stream captures change → Task processes → Final table updates

---

## 🧠 Key Learnings

* Streams track only new changes (CDC)
* Tasks automate pipelines
* MERGE prevents duplicate records
* Separation of layers improves scalability
