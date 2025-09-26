# 🚀 Big Data Lab with Spark, Hadoop & Jupyter (Dockerized)

This repository provides a **ready-to-use environment** for experimenting with  
**Apache Spark**, **Hadoop HDFS**, and **Jupyter Notebook** – all inside Docker containers.  
Perfect for **learning, practicing, and running PySpark code** locally.

---

## 🛠️ Stack

- **Apache Spark 3.5.0**
  - Spark Master + Worker(s)  
- **Hadoop HDFS 3.2.1**
  - Namenode + Datanode  
- **Jupyter Notebook** (with PySpark pre-configured)  

All services are orchestrated via **Docker Compose**.

---

## 🌐 Exposed Ports

| Service          | Port | Description           |
|------------------|------|-----------------------|
| Spark Master     | 8082 | Spark Web UI          |
| Spark Worker     | 8081 | Worker UI             |
| Jupyter Notebook | 8888 | Interactive notebooks |
| HDFS Namenode    | 9870 | Namenode Web UI       |
| HDFS Datanode    | 9864 | Datanode Web UI       |

---

## 📂 Project Structure

```plaintext
spark-docker-lab/
│
├── docker-compose.yml     # Docker services definition
├── shared/                # Shared folder between containers
│   ├── NullData.csv
│   ├── russia.txt
│
├── notebooks/
│   └── pyspark_lab.ipynb  # PySpark experiments
│
└── README.md
```
---

## ▶️ How to Run

Clone the repository

git clone https://github.com/saeed-3laa/spark-docker-lab.git
cd spark-docker-lab


Start the environment

docker compose up -d


Access services

Jupyter Notebook → http://localhost:8888

Spark Master UI → http://localhost:8082

HDFS Namenode UI → http://localhost:9870

