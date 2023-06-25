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

## Apache Airflow for Pipeline Orchestration

TFX orchestrators are responsible for scheduling components of the TFX pipeline based on the dependencies defined by the pipeline. TFX is designed to be portable to multiple environments and orchestration frameworks. One of the default orchestrators supported by TFX is Apache Airflow. This lab illustrates the use of Apache Airflow for TFX pipeline orchestration. Apache Airflow is a platform to programmatically author, schedule and monitor workflows. TFX uses Airflow to author workflows as directed acyclic graphs (DAGs) of tasks. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed. Apache Airflow workflows are defined as code. This makes them more maintainable, versionable, testable, and collaborative. Apache Airflow is suited for batch processing pipelines. It is lightweight and easy to learn.

In this example, we are going to run a TFX pipeline on an instance by manually setting up Airflow.

The other default orchestrators supported by TFX are Apache Beam and Kubeflow. Apache Beam can run on multiple data processing backends (Beam Ruunners). Cloud Dataflow is one such beam runner which can be used for running TFX pipelines. Apache Beam can be used for both streaming and batch processing pipelines.
Kubeflow is an open source ML platform dedicated to making deployments of machine learning (ML) workflows on Kubernetes simple, portable and scalable. Kubeflow can be used as an orchestrator for TFFX pipelines when they need to be deployed on Kubernetes clusters. In addition, you can also use your own custom orchestrator to run a TFX pipeline.

## Reference: https://www.tensorflow.org/tfx/tutorials/tfx/airflow_workshop
