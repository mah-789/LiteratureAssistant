##Literature Assistant Agent

## Overview

Literature Assistant is an AI-powered research assistant built using LangGraph and Groq LLM. The agent helps users explore academic topics by searching for relevant information, summarizing findings, identifying research gaps, and generating a structured literature review report.

## Workflow Type

Conditional Workflow with Iterative Query Refinement

The workflow evaluates search results and decides whether enough information has been gathered. If the information is insufficient, the agent automatically refines the query and performs another search before proceeding.

## Features

* Literature search using DuckDuckGo Search
* Wikipedia-based knowledge retrieval
* Automatic search result evaluation
* Query refinement loop
* Literature summarization
* Research gap identification
* Final literature review report generation
* Persistent state management
* Workflow visualization using Mermaid diagrams

## LangGraph Features Used

* StateGraph
* Nodes
* Edges
* Conditional Edges
* Typed State
* Tool Integration
* Checkpointing with InMemorySaver
* Graph Compilation
* Workflow Visualization using draw_mermaid_png()

## Workflow

1. Analyze Research Topic
2. Search Literature Sources
3. Evaluate Search Results
4. Refine Query if Needed
5. Summarize Findings
6. Identify Research Gaps
7. Generate Final Report

### Configure Environment Variables

Create a `.env` file and add:

env
GROQ_API_KEY=your_api_key_here

## Running the Notebook

Open the notebook in Google Colab and run all cells sequentially.

Ensure that:

- Required packages are installed
- GROQ API key is configured
- All outputs are visible
- Graph visualization generated using draw_mermaid_png()

## Running the Streamlit App

streamlit run app.py

## Project Structure

LiteratureAssistant/
│
├── agent.ipynb
├── app.py
├── README.md
├── requirements.txt
├── .env.example
│
├── flowchart/
│   └── workflow.png
│
└── slides/
    └── presentation.pdf
