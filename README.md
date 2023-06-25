# Orchestrating-a-TFX-Pipeline-with-Airflow

Overview

This repo is designed to help you learn to create your own machine learning pipelines using TensorFlow Extended (TFX) and Apache Airflow as the orchestrator. It runs on on Vertex AI Workbench, and shows integration with TFX and TensorBoard as well as interaction with TFX in a Jupyter Lab environment.

- A TFX pipeline is a Directed Acyclic Graph, or "DAG". We will often refer to pipelines as DAGs.
- TFX pipelines are appropriate when you will be deploying a production ML application
- TFX pipelines are appropriate when datasets are large, or may grow to be large
- TFX pipelines are appropriate when training/serving consistency is important
- TFX pipelines are appropriate when version management for inference is important
- Google uses TFX pipelines for production ML

## ML development process:
- Ingesting, understanding, and cleaning our data
- Feature engineering
- Training
- Analyzing model performance
- Lather, rinse, repeat
- Ready for production
