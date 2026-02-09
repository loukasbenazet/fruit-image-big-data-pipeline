# Fruit Image Big Data Pipeline 🍎☁️

Big Data project to build the first version of a scalable image processing pipeline for a fruit recognition mobile application.

The goal is **not to train a model yet**, but to prepare the **data processing architecture** that will support future large-scale machine learning.

---

## Project context

A young AgriTech startup wants to launch a mobile app that allows users to take a photo of a fruit and get information about it.

Before deploying a full ML system, the company needs a **scalable Big Data pipeline** capable of processing large volumes of images in the cloud.

This project simulates the creation of this first production-ready pipeline.

---

## Objectives

Build the first bricks of a Big Data architecture:

- Deploy a cloud environment using **AWS EMR**
- Process images at scale using **PySpark**
- Distribute TensorFlow model weights for inference
- Reduce image dimensionality using **PCA**
- Store processed outputs in the cloud

---

## Tech stack

- Python
- PySpark
- AWS EMR
- AWS S3
- TensorFlow / Keras
- Big Data distributed processing

---

## Pipeline overview

The pipeline performs the following steps:

1. Load raw fruit images from cloud storage  
2. Distribute model weights across Spark workers  
3. Extract image features using TensorFlow  
4. Apply dimensionality reduction (PCA) in PySpark  
5. Save processed data back to cloud storage

This prepares the data for future large-scale ML training.

---

## Output data

The pipeline generates:

- Distributed parquet files containing extracted image features
- CSV files containing PCA-reduced features

These outputs are ready for future machine learning workflows.

---

## Key learning outcomes

- Designing a Big Data architecture
- Using PySpark for distributed processing
- Deploying and using AWS EMR
- Scaling image processing pipelines
- Preparing ML pipelines for production
