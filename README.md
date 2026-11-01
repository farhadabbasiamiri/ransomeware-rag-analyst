# ransomeware-rag-analyst

# Group 3b_Capstone_Project

# Manoj Bastakoti

# Diwash Raj Amatya

# Subhash Neupane

# Mandeep Giri

# Swaratmik Khanal

🛡️ Ransomware Threat Intelligence RAG Analyst

Group 3B | Applied AI Agents for Cybersecurity Operations | AI/ML in Cybersecurity (Graduate) | Laurentian University | Fall 2026

Project Overview

The Ransomware Threat Intelligence RAG Analyst is a defensive AI project designed to help security analysts understand ransomware threats using trusted cybersecurity information.

The project aims to develop a Retrieval-Augmented Generation (RAG) system using public CISA #StopRansomware advisories, MITRE ATT&CK resources, and ransomware response playbooks.

The proposed system will answer ransomware-related questions using retrieved evidence, identify relevant MITRE ATT&CK techniques, summarize threat advisories, and provide recommendations for defensive monitoring, hardening, and incident response.

The project is being developed in stages, beginning with repository setup and data collection, followed by document processing, retrieval, agent development, and evaluation.

Project Objectives

Collect and organize public ransomware threat intelligence.

Extract relevant MITRE ATT&CK techniques and ransomware behaviour information.

Prepare cybersecurity documents for retrieval and analysis.

Develop a RAG pipeline to retrieve relevant information in response to user questions.

Explore local LLM integration using Ollama.

Generate evidence-based answers with supporting citations.

Develop defensive checklists for monitoring, hardening, and containment.

Implement safety mechanisms and human approval for sensitive response actions.

Evaluate retrieval quality, answer accuracy, and system safety.

## Quick start

````bash
git clone <this-repo> && cd ransomeware-rag-analyst
python -m venv .venv && source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python scripts/build_index.py                           # builds chunks + vector index (~5 s)
python app.py

**Optional — generated answers with a free local LLM**

```bash
# install Ollama from https://ollama.com, then:
ollama pull llama3.2:3b          # or qwen2.5:3b, mistral, gemma2:2b, phi3 …
ollama serve
python app.py
````
