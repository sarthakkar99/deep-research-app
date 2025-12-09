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


📦 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/sarthakkar99/deep-research-app.git
cd deep-research-app

2️⃣ Create a virtual environment (optional but recommended)
python3 -m venv venv
source venv/bin/activate

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Add your .env file

Create a .env file in the project root:

OPENAI_API_KEY=your-openai-key
FIRECRAWL_KEY=your-firecrawl-key


(Do NOT commit this file.)

▶️ Running the App
streamlit run main.py


Streamlit will open at:
http://localhost:8501

🛠️ How It Works — Under the Hood
🔍 Step 1 — Input

User enters a topic + breadth + depth.

🤖 Step 2 — Agents Activate

Research Agent generates sub-queries and fetches relevant content via Firecrawl

Summarizer Agent condenses findings into structured markdown

Presenter Agent formats insights into a coherent narrative

🧹 Step 3 — Markdown Cleaning

Custom cleaning functions remove noise, artifacts, broken symbols, etc.

📄 Step 4 — PDF Generation

ReportLab compiles the cleaned content into a downloadable PDF.

📘 Future Enhancements (Planned)

Add vector search for storing/retrieving insights

Add citation extraction

Add multiple rendering themes for PDFs

Add knowledge graph generation

Enable multi-step conversational research

