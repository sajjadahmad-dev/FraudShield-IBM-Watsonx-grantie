# FraudShield: AI-Powered Financial Risk Assessment and Fraud Detection

> An intelligent financial crime analysis platform that leverages Large Language Models (IBM Granite), interactive analytics, and explainable AI to assist with transaction risk assessment and fraud monitoring.

---

## Overview

FraudShield is a research-oriented prototype designed to demonstrate how Large Language Models (LLMs) can support financial fraud detection and risk assessment through natural language reasoning.

The system combines:

- AI-assisted transaction analysis
- Customer risk assessment
- Interactive analytics dashboard
- Report generation
- Conversational AI assistant
- Explainable risk scoring

The application is implemented using **Python** and **Streamlit**, with **IBM Granite** serving as the reasoning engine for risk analysis. :contentReference[oaicite:0]{index=0}

---

## Motivation

Traditional fraud detection systems primarily rely on manually engineered rules or supervised machine learning models.

FraudShield explores an alternative approach where modern Large Language Models assist analysts by:

- Interpreting transaction descriptions
- Estimating fraud risk
- Supporting compliance analysis
- Explaining suspicious financial activities
- Providing conversational assistance

This project investigates how foundation models can complement traditional financial crime detection pipelines.

---

# Features

## Transaction Risk Analysis

Analyze individual financial transactions using IBM Granite.

Input includes:

- Sender
- Receiver
- Amount
- Currency
- Transaction description

The LLM estimates a fraud risk score between **0 and 1**, which is converted into an interactive risk gauge. :contentReference[oaicite:1]{index=1} :contentReference[oaicite:2]{index=2}

---

## Customer Risk Assessment

Evaluate customer profiles using business characteristics such as:

- Business type
- Transaction volume
- Country risk

The system prompts the LLM to estimate an overall customer risk score. :contentReference[oaicite:3]{index=3}

---

## Interactive Dashboard

Visual dashboard includes:

- Transaction statistics
- Risk summaries
- Risk trend visualization
- Interactive charts

Built with Plotly for exploratory analysis. :contentReference[oaicite:4]{index=4}

---

## Report Generation

Generate multiple report types:

- Transaction Summary
- Risk Analysis
- Suspicious Activity Report

Includes:

- Interactive charts
- Tables
- Geographic visualization

:contentReference[oaicite:5]{index=5}

---

## AI Chat Assistant

FraudShield includes an integrated chatbot powered by IBM Granite that allows users to ask questions related to fraud detection and financial analysis. :contentReference[oaicite:6]{index=6}

---

# System Architecture

```
                User
                  │
                  ▼
          Streamlit Web UI
                  │
      ┌───────────┴────────────┐
      │                        │
      ▼                        ▼
Transaction Analysis      Risk Assessment
      │                        │
      └───────────┬────────────┘
                  ▼
         Prompt Construction
                  ▼
         IBM Granite LLM API
                  ▼
        Risk Score Generation
                  ▼
      Visualization & Reports
```

---

# Technology Stack

| Category | Technologies |
|----------|--------------|
| Language | Python |
| Frontend | Streamlit |
| AI Model | IBM Granite 3 8B Instruct |
| Visualization | Plotly |
| Data Processing | Pandas, NumPy |
| API | IBM Watsonx |
| HTTP | Requests |

---

# AI Workflow

1. User submits transaction details.
2. A structured prompt is created.
3. IBM Granite analyzes the transaction.
4. The generated response is parsed.
5. A numerical fraud risk score is extracted.
6. The score is visualized through dashboards and indicators.
---

# Installation

Clone the repository

```bash
git clone https://github.com/yourusername/FraudShield.git

cd FraudShield
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# Configure IBM Watsonx

Set your API key as an environment variable:

```bash
export YOUR_KEY=YOUR_API_KEY
```

Configure:

- IBM Cloud API Key
- Project ID
- Watsonx endpoint

before launching the application.

---

# Run

```bash
streamlit run app.py
```

---

# Research Directions

This prototype can be extended with:

- Graph Neural Networks for transaction networks
- Retrieval-Augmented Generation (RAG)
- Hybrid LLM + traditional fraud classifiers
- Explainable AI (XAI)
- Agentic AI workflows
- Knowledge Graph reasoning
- Multi-agent financial investigation
- Real-time streaming transaction analysis
- Temporal fraud pattern modeling

---

# Future Improvements

- Live banking APIs
- AML compliance integration
- SAR generation
- Role-based authentication
- Audit logging
- Multi-LLM support
- Database integration
- Model benchmarking
- Explainable reasoning traces

---
