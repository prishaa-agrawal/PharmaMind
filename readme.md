# PharmaMind: Agentic AI for Drug Repurposing Research

## Overview
PharmaMind is an agent-based AI platform built to automate drug repurposing research by identifying new therapeutic uses for existing molecules. The system uses multiple AI agents to collect, analyze, and present biomedical and market data in a structured and meaningful way.

## Objective
To develop an AI system capable of researching, analyzing, and summarizing potential new medical applications for any given molecule using real-world biomedical sources and AI reasoning.

## Architecture
A master agent coordinates several specialized worker agents responsible for gathering information from clinical trials, research papers, patents, and market datasets. Their outputs are combined into a unified summary and report.

## Technology Stack
- Frontend: React.js
- Backend: FastAPI (Python)
- AI/NLP: Language models and biomedical NLP tools
- Database: MongoDB with optional Redis caching

## Workflow
1. User enters a molecule name.
2. Agents collect domain-specific data from multiple sources.
3. Results are processed into summaries, charts, and a structured report.
4. Dashboard displays the final insights.

## Output
- Drug overview
- Clinical trials and new indications
- Research papers and patents
- Market analysis
- Downloadable report
