# 🚀 E-commerce Real-Time Order Intelligence Pipeline

## 📌 Problem Statement

E-commerce platforms generate continuous order and payment data.
Traditional batch pipelines fail to process real-time updates efficiently.

👉 This project solves that using **Snowflake Streams & Tasks** for real-time data processing.

---

## 🏗️ Architecture

Raw Data → Bronze → Silver → Gold → Stream → Task → Final Table

---

## ⚙️ Tech Stack

* Snowflake
* SQL
* Streams (CDC)
* Tasks (Automation)

---

## 🔄 Pipeline Flow

1. Load raw data into Bronze layer
2. Clean & structure data in Silver layer
3. Create business-ready tables in Gold layer
4. Stream captures incremental changes
5. Task automatically updates final table

---

## ⚡ Key Features

* Real-time incremental processing
* No duplicate handling using MERGE
* Fully automated pipeline
* Scalable medallion architecture

---

## ▶️ How to Run

Run SQL files in order:

1_setup.sql
2_bronze.sql
3_silver.sql
4_gold.sql
5_streams.sql
6_tasks.sql
7_demo.sql

---

## 🎯 Demo (MOST IMPORTANT)

1. Insert new order into `clean_orders`
2. Stream captures new data
3. Task processes the stream
4. Final table (`order_master`) gets updated

---

## 🧠 Key Learnings

* Streams capture only new changes (CDC)
* Tasks automate pipelines
* MERGE prevents duplicate records
* ROW_NUMBER ensures latest records

---

## 💡 Why This Stands Out

Unlike batch pipelines, this solution:

* Processes data incrementally
* Reduces compute cost
* Enables near real-time analytics

---

## 👨‍💻 Author

Vedang Tiwari
