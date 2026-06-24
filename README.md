# Multi-Agent Research Assistant

An AI-powered research assistant that uses a multi-agent workflow to gather information from the web, analyze sources, generate structured reports, and provide automated feedback on the quality of the generated content.

## Overview

This project demonstrates how multiple specialized AI agents can collaborate to perform complex research tasks. Instead of relying on a single LLM call, the system breaks the problem into smaller stages handled by dedicated agents.

### Agent Workflow

1. **Search Agent**

   * Searches the web for relevant and recent information.
   * Identifies high-quality sources related to the user's query.

2. **Reader Agent**

   * Selects the most relevant source.
   * Extracts and summarizes detailed content from web pages.

3. **Writer Agent**

   * Synthesizes gathered information.
   * Generates a structured research report.

4. **Critic Agent**

   * Reviews the generated report.
   * Provides feedback on clarity, completeness, and quality.

## Architecture

User Query
↓
Search Agent
↓
Reader Agent
↓
Writer Agent
↓
Critic Agent
↓
Final Research Report

## Features

* Multi-agent AI workflow
* Web search integration
* Automated content extraction
* Research report generation
* Report quality evaluation
* FastAPI backend
* Interactive frontend dashboard
* Real-time research pipeline visualization

## Tech Stack

### Backend

* Python
* FastAPI
* LangChain
* Mistral AI
* Tavily Search API
* BeautifulSoup

### Frontend

* HTML
* CSS
* JavaScript

### AI Components

* Search Agent
* Reader Agent
* Writer Agent
* Critic Agent

## Installation

Clone the repository:

```bash
git clone <repository-url>
cd multi-agent-research
```

Create a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create a `.env` file:

```env
MISTRALAI_API_KEY=your_api_key
TAVILY_API_KEY=your_api_key
```

Run the application:

```bash
uvicorn api:app --reload
```

Open:

```text
http://localhost:8000
```

## Future Improvements

* Parallel agent execution
* LangGraph-based orchestration
* Source credibility scoring
* Citation generation
* PDF export
* Research memory and caching
* Multi-model support (OpenAI, Gemini, Claude, Mistral)

## Project Motivation

The goal of this project is to explore agentic AI systems where multiple specialized agents collaborate to solve complex research tasks. It demonstrates practical applications of tool calling, web search, content extraction, and automated report generation using modern LLM frameworks.

## Author

**Divyam Saraf**

B.Tech Computer Science & Engineering
Indian Institute of Information Technology (IIIT) Kota
