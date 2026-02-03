PharmaMind — Agentic AI System for Drug Repurposing Research
Overview

PharmaMind is an agent-based artificial intelligence system developed to automate drug repurposing research. Drug repurposing focuses on discovering new therapeutic applications for existing drugs or chemical compounds. Traditionally, this process requires manual exploration of multiple biomedical databases and research sources. PharmaMind eliminates this manual effort by coordinating multiple AI agents that independently collect, analyze, and summarize biomedical and market intelligence.

The system integrates information from clinical trials, research publications, patent databases, and healthcare datasets, and converts it into meaningful insights presented through visual dashboards and downloadable reports.

Objective

The primary objective of PharmaMind is to design an intelligent system capable of automatically researching, analyzing, and presenting potential new medical uses for any given molecule using real-world biomedical data and AI reasoning.

When a molecule name is provided, the system gathers relevant evidence from multiple domains and compiles the findings into a structured summary.

System Architecture

PharmaMind follows a multi-agent architecture composed of a central coordinating agent and multiple specialized worker agents.

Master Agent (Coordinator)

The master agent interprets the user query and distributes tasks to appropriate worker agents. It then aggregates the outputs into a coherent final response.

Worker Agents
Agent	Responsibility	Data Source
Clinical Trials Agent	Retrieves data about ongoing and completed trials	ClinicalTrials.gov API
Research Agent	Collects research papers and trends	PubMed API, Semantic Scholar
Patent Agent	Searches patents involving the molecule	Lens.org, Google Patents
Market Agent	Evaluates disease demand and market potential	OpenFDA, WHO, Kaggle datasets
Report Agent	Generates charts and structured PDF reports	Plotly, ReportLab
Technology Stack
Frontend

React.js for user interface

Tailwind CSS / Material UI for design

Chart.js / Recharts / Plotly for visualizations

Framer Motion for interface interactions

Backend

FastAPI (Python) for API handling

LangChain / CrewAI / LlamaIndex for multi-agent orchestration

AsyncIO / Celery for parallel execution

Pandas and Plotly for data processing

AI and NLP Layer

OpenAI language models for reasoning and summarization

BioBERT / PubMedBERT for biomedical understanding

SciSpacy for entity extraction

Database

MongoDB for storing results

Redis for optional caching

Data Sources

PharmaMind collects data from reliable biomedical and public datasets including:

ClinicalTrials.gov

PubMed Central

Semantic Scholar

PubChem

Lens.org

Kaggle datasets

OpenFDA API

System Workflow

The user provides the name of a molecule.

The master agent assigns tasks to worker agents.

Each worker agent retrieves and summarizes domain-specific information.

The report agent combines the results into structured JSON data, charts, and a PDF report.

The frontend dashboard displays the final output.

Output Provided

For a given molecule, PharmaMind generates:

Drug overview

Ongoing and completed clinical trials with new indications

Key research publications

Relevant patents

Market analysis and visual charts

Downloadable structured report
