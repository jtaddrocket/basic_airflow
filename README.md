# Apache Airflow 

Apache Airflow is an open-source platform used to programmatically author, schedule, and monitor workflows.
It allows you to define complex workflows as code and manage their execution. Airflow is commonly used for data
pipeline, where tasks like data extraction, transformation, and loading (ETL) are orchestrated across multiple systems.

# Key Concepts In Apache Airflow 

## 1. DAG (Directed Acyclic Graph): 

DAG: connection of tasks that you want to schedule and run.

- Directed: Task must have a specific seq.
- Acyclic: No task should be depend on itself.

## 2. Tasks:

Task represent the individual unit of work in a DAG. 

- Python function. 
- Querying a database. 
- Sending an HTTP request.

## 3. Dependencies

Task in a DAG have dependencies, meaning one task might need to finish before another task can start.
These dependencies allow you to control the order in which tasks are executed. Airflow provides mechanisms like 
set_upstream and set_downstream to define these dependencies between tasks.

# Why Airflow for MLOps

In MLOps, orchestrating ML workflows efficiently is crucial for ensuring that data pipelines, model training, 
and deployment tasks happen smoothly and in an automated manner. Airflow is well-suited for this purpose because it
allows you to define, automate, and monitor every step in an ML pipeline.

## 1. Orchestrating ML Pipeline And ETL Pipeline

Data Ingestion ==> Data Preprocessing ==> Model Training and Eval ==> Model Deployment

## 2. Task Automation

## 3. Monitoring And Alert

- Real Time Monitoring -> Airflow UI
- Task Logs
- Alert And Notifications -> Emails
- Retry Mechanism -> Retry Task -> Pre define Rules



