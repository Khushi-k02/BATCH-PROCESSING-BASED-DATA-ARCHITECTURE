Streaming Data Pipeline with Kafka, Airflow, and Spark
Project Overview
This project sets up a streaming data pipeline using Apache Kafka, Apache Airflow, and Apache Spark. The pipeline fetches user data from an external API, processes it, and streams it to Kafka for batch processing analytics.
Components
1.	Apache Airflow: Orchestrates the data pipeline.
2.	Kafka: Handles real-time data streaming.
3.	Spark: Processes and writes data to storage.
4.	Docker Compose: Manages containerized services.
Files
•	.env: Environment variables for services.
•	docker-compose.yml: Configuration for Kafka, Airflow, and Spark.
•	airflow.sh: Script to run Airflow commands.
•	kafka_stream_dag.py: Airflow DAG to trigger Kafka streaming.
•	kafka_streaming_service.py: Kafka producer fetching and streaming data.
•	spark_processing.py: Spark job for data transformation.
Setup
1.	Run docker-compose up -d to start services.
2.	Access Airflow at http://localhost:8080 (User: admin, Pass: admin).
3.	Monitor Kafka UI at http://localhost:8888.
4.	Verify data processing using Spark logs.


