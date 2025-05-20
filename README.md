## 🌀 **Airflow + PostgreSQL Integration Using Docker**

This project sets up an Apache Airflow environment integrated with PostgreSQL and PgAdmin using Docker Compose. It enables you to run ETL workflows, orchestrate tasks, and monitor data pipelines in a local environment.

## 📦 **Tech Stack**

Apache Airflow

PostgreSQL

PgAdmin 4

Docker/Docker Compose

## 🚀 **Getting Started**

Follow these steps to spin up the environment and run your first Airflow DAG:

🧾 **Step 1: Fetch the Docker Compose File**

Download the official Airflow docker-compose.yaml file:

curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.8.1/docker-compose.yaml'

Alternatively, clone this repository if already included.

🛠 **Step 2: Add PostgreSQL & PgAdmin Services**

🔧 **Step 3: Initialize Airflow**

##### 📁 Create necessary directories
mkdir -p dags logs plugins

##### 🛠️ Initialize the Airflow metadata database
docker compose up airflow-init

▶️ **Step 4: Build & Run Containers**


🌐 **Step 5: Configure PgAdmin (Optional but Useful)**

🔌 **Step 6: Set Up PostgreSQL Connection in Airflow**

📅 **Step 7: Run Your DAG**

Place your DAG Python script in the dags/ folder

Open the Airflow UI and turn on your DAG

Click Trigger DAG to run

Monitor logs and status via the web UI

🧹**Clean Up**

To stop and remove containers:

docker compose down
