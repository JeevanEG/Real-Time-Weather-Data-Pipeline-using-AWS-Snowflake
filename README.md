# Real-Time-Weather-Data-Pipeline-using-AWS-Snowflake

## 📌 Overview

This project implements a **real-time weather data pipeline** leveraging **AWS Lambda**, **DynamoDB**, **DynamoDB Streams**, **S3**, and **Snowflake**. It fetches hourly weather data for 10 Indian cities using the WeatherAPI, processes and stores it in DynamoDB, streams it for transformation into CSV, and loads it into Snowflake for analytics.

---

## 🛠 Architecture

```
WeatherAPI → Lambda (Data Collector) → DynamoDB → Lambda (Stream Processor) → S3 → Snowflake
```

---

## 📂 Project Structure

| File                           | Description                                                                               |
| ------------------------------ | ----------------------------------------------------------------------------------------- |
| `weather_lamda_fun1.py`        | AWS Lambda function to collect weather data from WeatherAPI and insert into DynamoDB      |
| `W_Ddb_to_streamlamda_fun2.py` | Stream-triggered Lambda function to transform new DynamoDB records and store as CSV in S3 |
| `Final_Report_FDE.docx`        | Detailed project report outlining objectives, architecture, implementation, and results   |

---

## 🌐 Technologies Used

* **AWS Lambda**: Serverless compute to run Python code
* **AWS DynamoDB**: NoSQL database for real-time storage
* **DynamoDB Streams**: To trigger transformations on new records
* **AWS S3**: Storage for transformed CSV files
* **Snowflake**: Cloud data warehouse for analytics
* **WeatherAPI**: External API for real-time weather data
* **Python & Pandas**: Data processing and transformation

---

## 📊 Cities Monitored

* Bangalore
* Delhi
* Mumbai
* Chennai
* Kashmir
* Dehradun
* Kochi
* Kerala
* Hyderabad
* Sikkim

---

## 📈 Key Features

* ⏱ Hourly weather data collection
* ☁️ Serverless architecture (AWS Lambda)
* 📦 NoSQL data storage (DynamoDB)
* 🔁 Stream processing (Lambda + Pandas)
* 💾 CSV export to S3
* ❄️ Snowflake integration for analytics

---

## 📌 Sample Analytics in Snowflake

* **Average Temperature per City**
* **Maximum Wind Speed per City**
* **Daily Temperature Range**
* **Wind Direction Patterns**
* **Time of Highest Temperature**

---

## 🚀 Future Work

* Add more cities and weather parameters
* Introduce data validation layers
* Create real-time visualization dashboards
* Integrate ML models for weather forecasting

---

## 📑 Author

**Jeevan EG**
`1RVU22CSE069`
RV University, Bengaluru
Academic Year: 2024–2025

---

