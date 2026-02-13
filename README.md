# ResearchFlow

🧠 ResearchFlow: Multi-Agent RAG Intelligence Lab
ResearchFlow is an advanced Retrieval-Augmented Generation (RAG) system that moves beyond simple "Prompt-Response" loops. It employs an Agentic Orchestration architecture where three specialized AI agents collaborate to analyze, critique, and synthesize insights from complex technical documents (PDFs).

🚀 The Problem & Solution
The Problem: Traditional RAG systems often suffer from "hallucinations" or provide surface-level summaries that miss technical nuances in large documents.
The Solution: ResearchFlow introduces a Multi-Agent Critic Loop. Instead of one LLM doing all the work, the task is split among three "experts," ensuring high-fidelity data extraction and cross-verification.

🛠 System Architecture
The system is built on a modular "Thinking Graph":

The Planner Agent: Decomposes the user’s complex query into a series of logical sub-questions.

The Researcher Agent: Performs semantic searches across a ChromaDB Vector Store using OpenAI/HuggingFace embeddings to find relevant document chunks.

The Critic Agent: Evaluates the researcher's findings. If the data is insufficient or contradicts the source, it triggers a "Re-Research" loop.

✨ Key Features
Agentic Autonomy: Agents "talk" to each other via LangGraph to resolve ambiguities.

High-End UX: Built with Streamlit, featuring a real-time "Thought Process" terminal.

Persistence: Uses ChromaDB for efficient, local vector storage and retrieval.

Hallucination Guardrails: The Critic agent performs a fact-check against the original text chunks before displaying the final output.

📦 Tech Stack
Orchestration: LangChain / LangGraph

LLM: OpenAI GPT-4o / Llama 3 (via Groq)

Vector Database: ChromaDB

Frontend: Streamlit

Document Parsing: PyMuPDF / LangChain PDF Loader

📥 Installation & Setup
Clone the Repository

Bash
git clone https://github.com/harshsaxena777/ResearchFlow.git
cd ResearchFlow
Install Dependencies

Bash
pip install -r requirements.txt
Configure Environment Variables

Run the Application
streamlit run app.py

📜 License
Distributed under the MIT License. See LICENSE for more information.
