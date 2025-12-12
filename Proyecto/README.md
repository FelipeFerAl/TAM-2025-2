# 📘 Machine Learning Theory Project — Predicting UITI in Electrical Distribution Networks
## 📌 Overview

This project applies Machine Learning techniques—specifically TabNet and RAG/Agentic RAG workflows—to analyze an electrical distribution system dataset and predict the Unified Index of Tension and Interruptions (UITI).
UITI is a metric that integrates voltage stability, interruption frequency, and duration, and serves as an indicator of service quality across points in a power distribution network.

The project is structured as a research-oriented exploration for a machine learning theory course.

## 📂 Dataset Description

This project uses a dataset from Kaggle containing technical, structural, operational, and meteorological data related to equipment and nodes in an electrical distribution grid.

📎 Dataset link: (https://www.kaggle.com/datasets/felipef2/chec-dataset/data)

## 🔍 Purpose of the Dataset

The goal is to predict the UITI for each point in the network. This value summarizes aspects such as:
* Voltage stability
* Frequency of service interruptions
* Duration of outages

By predicting UITI, engineers and operators can:
* Evaluate equipment performance
* Identify critical points in the distribution network
* Prioritize maintenance tasks
* Support decision-making for system reliability

## 📊 Reliability Indices Included

The dataset provides several industry-standard reliability metrics:

* SAIFI (System Average Interruption Frequency Index):
Average number of interruptions per customer.

* SAIDI (System Average Interruption Duration Index):
Average total outage time per customer.

* CAIDI (Customer Average Interruption Duration Index):
Average duration of a single outage.

* UITI (Unified Index of Tension and Interruptions):
Composite indicator integrating voltage stability, frequency, and duration.

**UITI is the target variable for prediction tasks in this project.**

# 🤖 Machine Learning Approach
## 1️⃣ TabNet for Tabular Deep Learning

The project implements multiple TabNet architectures to explore:

Feature representation learning

Different hyperparameter configurations

Classification or regression (depending on UITI formulation)

Comparative evaluation against baseline models

TabNet was selected due to its:

Interpretability (feature masks)

Suitability for high-dimensional tabular data

Efficient sparse representation learning

The main notebook details the training workflow, model selection, and performance visualization.

## 🔍 RAG and Agentic RAG Integration

The main .ipynb notebook includes an experimental section using:
* RAG (Retrieval-Augmented Generation)
* Agentic RAG (Self-directed retrieval + reasoning chains)

These components were used to:
* Generate explanations for model behavior
* Automate documentation and insights generation
* Validate predictions using external knowledge
* Create agent-like pipelines supporting iterative refinement

This demonstrates the theoretical integration of LLM retrieval systems into traditional machine learning workflows.
