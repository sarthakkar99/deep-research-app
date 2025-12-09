🚀 Deep Research Assistant — AI-Powered Multi-Agent Research System

In today’s information-rich world, conducting deep, focused research across the web can be time-consuming and overwhelming.

This project implements an AI-powered research assistant that automates this process using CrewAI multi-agent workflows, real-time web search, and advanced language models. The system simulates how a human researcher iteratively explores a topic by:

Asking refined questions

Searching multiple sources

Summarizing insights

Cleaning and structuring content

Generating polished research reports

🧠 What the System Does
✅ 1. Perform Deep Topic Research

Users can:

Enter any research topic

Configure breadth (number of sub-queries) and depth (recursion levels)

Trigger an automated multi-step research process

Behind the scenes:

A Research Agent performs web searches via Firecrawl

A Summarizer Agent condenses findings

A Presenter Agent organizes the insights into a structured report

The system orchestrates this via CrewAI + LangChain + OpenAI GPT models.

✅ 2. Generate and View Research Reports

Users can:

View cleaned and structured research summaries inside the Streamlit UI

Download a professional PDF report generated using ReportLab

Reports include:

Topic overview

Summaries

Extracted web sources

Structured insights

🏗️ Tech Stack
🔹 Frontend

Streamlit: Interactive UI for entering topics, configuring parameters, and viewing outputs

🔹 Backend

Python (MVC structure)

CrewAI: Multi-agent orchestration

LangChain: LLM tool integration

OpenAI GPT Models: Research reasoning + summarization

Firecrawl API: Search + metadata extraction

ReportLab: Dynamic PDF generation


Project Architecture
deep_research_app/
├── main.py                        # Streamlit entry point
├── controllers/
│   └── research_controller.py     # Orchestrates entire research workflow
├── services/
│   └── agents_service.py          # CrewAI agent setup & task creation
├── models/
│   └── pdf_generator.py           # Generates PDF reports using ReportLab
└── utils/
    └── markdown_cleaner.py        # Cleans & preprocesses markdown output



