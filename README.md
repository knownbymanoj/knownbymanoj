<div align="center">

# Manoj Kumar Nagabandi

**AI Engineer · RAG & Multi-Agent Systems · LangChain · PydanticAI · FastAPI**

*Building production-grade AI systems - from architecture to deployment.*

📍 India → Italy → Stockholm, Sweden  |  🇮🇳 Indian · EU Long-Term Resident Visa

</div>

---

## Who I Am

I'm a Full-Stack AI Engineer with 3+ years of production experience building enterprise-scale AI systems. As the **sole AI engineer at SIPA SpA** (Zoppas Industries Group), I designed and productionised **AI** into **ECHO Platform**, an enterprise AI assistant ecosystem serving **3,000+ internal staff and customers globally**, that gives after sales services using ERP, CRM, PLM, ticketing, and IoT data streams through three specialised AI agents.

My work spans the full lifecycle: problem framing → system architecture → retrieval design → agent orchestration → evaluation → production deployment → LLMOps observability. I care about systems that are measurable, explainable, and maintainable at scale.

---

## What I've Built in Production

> Some projects below were built at SIPA SpA. Proprietary code lives on the company's internal GitLab.

### ECHO Platform - Enterprise AI Agent Ecosystem

**Multi-Agent multi-step real-time query system** connecting to 25+ live REST APIs (machines, orders, production data, alarms) via hierarchical intent classification → sub-agent identification parallell / sequential,  delegate / handoff → parallel function calling → parameter extraction → parallel sub-agent handoffed LLMs answer synthesis to user parallely (or) return to orchestrator for next step plan -> Final answer sysnthesis. Integrated into the platform backend via WebSockets + JavaScript front-end, with RBAC data security for 3,000+ users. Includes Langfuse observability, real-time user feedback loops, and continuous RAG evaluation.

`PydanticAI` `Django` `WebSockets` `Langfuse` `OpenAI` `PostgreSQL` `REST APIs` `RBAC`

---

### [Agentic FleetOps Copilot - Conversational Fleet Intelligence](https://github.com/knownbymanoj/agentic_fleetops_copilot)

Built a conversational fleet intelligence system that predicts truck component failures, explains risk with SHAP, and supports maintenance decisions through an agentic chat interface backed by FastAPI services. The project combines **PydanticAI, XGBoost, Langfuse, and a Scania-inspired fleet simulator**, using real predictive-maintenance patterns from the Component X dataset.

`PydanticAI` `FastAPI` `XGBoost` `SHAP` `Langfuse` `Predictive Maintenance` `Agentic Systems` `Simulator`

---

### Manuals Assistant - Hybrid RAG for Industrial PDFs

**Advanced hybrid RAG pipeline** for industrial PDF manuals (maintenance, installation, operational). Parses hierarchical document structures via Table of Contents, stores chapter/sub-chapter hierarchies in PostgreSQL with dynamic linking to pgvector embeddings (OpenAI text-embedding-3-large, dim=256) in AWS S3. Implements FTS + vector search fused with **Reciprocal Rank Fusion (RRF)**, LLM re-ranking, extractive summarisation with citations, and multi-turn query rewriting.

`RAG` `pgvector` `PostgreSQL` `AWS S3` `Hybrid Search` `RRF` `OpenAI Embeddings` `Langfuse` `Django`

---

### Customer Help Desk Assistant - Ticket Intelligence

**Data pipeline for historical service ticket retrieval**: PII removal via a domain-specific technical glossary, structured metadata extraction (alarms, machine models, issue types), and embedding-based indexing. Dual-mode retrieval: deterministic query mode (structured ticket search by parameters) + RAG semantic mode, with cited ticket references for traceability.

`RAG` `NLP` `Django` `PII Removal` `Metadata Extraction` `Semantic Search` `PostgreSQL` `LangChain` `Langfuse` `Docker`

---

### 📈 Multiple Time Series Forecasting - 4,200 Machines Simultaneously

Developed a forecasting solution predicting **alarm events and production cycle timing across 4,200 industrial machines at once**, enabling proactive maintenance scheduling. Applied **XGBoost + Transformer-based architectures (LSTM, ARIMA)** on large-scale industrial sensor data.

`XGBoost` `LSTM` `ARIMA` `Transformers` `Scikit-learn` `MLflow` `Time Series` `PySpark`

***

## 🎥 Project Architecture & Demos

###  EVA (Echo Virtual Assistant)

#### **Version 1: Workflow Based Single AI Agent**

[▶ Watch the demo video](https://drive.google.com/file/d/1e7ynm-rBylvi4d1bKy44CK4vWUCnThaM/view?usp=sharing)

[![Watch the demo](./assets/workflow_based_agent.png)](https://drive.google.com/file/d/1e7ynm-rBylvi4d1bKy44CK4vWUCnThaM/view?usp=sharing)

##### **Architecture**

<p align="center">
<img src="./assets/echo-platform-v1-architecture.png">
<img src="./assets/echo-platform-architecture-integration.png">
</p>

---

#### **Version 2: Planning based Multi-step Multi-agents using delagation/handoff to sub-agents using Orchestrator**

[▶ Watch the demo video](https://drive.google.com/file/d/19vl0LPuBBumn2boE3RaQKM7z5Oonic9R/view?usp=sharing)

[![Watch the demo](./assets/multi-agents-orchestration.png)](https://drive.google.com/file/d/19vl0LPuBBumn2boE3RaQKM7z5Oonic9R/view?usp=sharing)

### Manuals Assistant - Hybrid RAG for Industrial PDFs

[▶ Watch the demo video](https://drive.google.com/file/d/1welDVC23dEJkBv5_cCFPDoSCqXW7Xltw/view?usp=sharing)

[![Watch the demo](./assets/manuals-assistant.png)](https://drive.google.com/file/d/1welDVC23dEJkBv5_cCFPDoSCqXW7Xltw/view?usp=sharing)

**Architecture**

<p align="center">
  <img src="./assets/manuals-assistant-architecture-1.png">
  <img src=".assets/manuals-assistant-architecture-2.png">
</p>

### Customer Help-Desk Assistant

[▶ Watch the demo video](https://drive.google.com/file/d/1pXB03IaWDlg9wmInGfZE0UNhU_yFDoIw/view?usp=sharing)

[![Watch the demo](./assets/customer_help_desk_assistant.png)](https://drive.google.com/file/d/1pXB03IaWDlg9wmInGfZE0UNhU_yFDoIw/view?usp=sharing)

**Architecture**

<p align="center">
  <img src="./assets/helpdesk-assistant-architecture-1.png">
  <img src="./assets/helpdesk-assistant-architecture-2.png">
</p>

### Agentic FleetOps Copilot - Conversational Fleet Intelligence

[**Architecture**](https://github.com/knownbymanoj/agentic_fleetops_copilot/blob/main/README.md#-web-ui-demo--3-simple-tools-walkthrough)

**Screenshots**

<img width="1024" height="750" alt="image" src="https://github.com/user-attachments/assets/fd9e1c71-52ce-4684-953b-970020993731">
<img width="776" height="717" alt="image" src="https://github.com/user-attachments/assets/8ce86810-c990-4f01-b476-7957340b2574" />


***

## 🛠 Tech Stack

**Generative AI & LLMs**

![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)

**Agentic & LLMOps**

![PydanticAI](https://img.shields.io/badge/PydanticAI-E92063?style=for-the-badge&logo=pydantic&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Langfuse](https://img.shields.io/badge/Langfuse-000000?style=for-the-badge&logo=langfuse&logoColor=white)

**Backend & APIs**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

**ML & Data Science**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-1A9AC9?style=for-the-badge&logo=xgboost&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)

**Databases & Storage**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![AWS S3](https://img.shields.io/badge/AWS_S3-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?style=for-the-badge&logo=postgresql&logoColor=white)
---

## 🎓 Education

|Degree|Institution|Year|
|-|-|-|
|[M.Sc. Data Science](https://www.unipd.it/en/corsi-di-laurea/data-science) (Dep. of Mathematics)|University of Padova, Italy|2021 - 23|
|[B.Sc. Engineering Sciences](https://engineering-sciences.uniroma2.it/)|University of Rome Tor Vergata, Italy|2017 - 21|

---

## 🌍 Currently

* 🏢 Full-Stack AI Engineer @ **SIPA SpA** (Zoppas Industries Group) - Italy
* 🎯 Open to senior AI/ML Engineer roles in **Stockholm, Sweden** or any other location in **Sweden**
* 🌐 Languages: English · Italian · Hindi · Telugu
---

<div align="center">

**[View & Download Resume](https://flowcv.com/resume/0e4p317okj)**

**Let's connect →** [**LinkedIn**](https://www.linkedin.com/in/manoj-nagabandi/)

</div>

