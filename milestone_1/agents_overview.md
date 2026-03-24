# Agents Overview

## Why 3 Agents?
To simplify the system design while maintaining clear separation of responsibilities and reducing orchestration complexity.

---

## 1. Candidate Intelligence Agent
Responsible for:
- Parsing CV
- Extracting structured data (skills, tools, projects, experience)
- Inferring target role

Output:
Structured candidate profile

---

## 2. Interview Orchestrator Agent
Responsible for:
- Planning interview flow
- Selecting/generating questions (RAG + LLM)
- Managing interview state
- Handling conversation logic

Output:
Next question + interview state

---

## 3. Evaluation & Reporting Agent
Responsible for:
- Evaluating answers
- Scoring responses
- Generating feedback
- Producing final report

Output:
Scores + feedback + final report

---

## Framework Choice
LangGraph is used to:
- Manage stateful workflows
- Control execution flow
- Support multi-agent orchestration

---

## LLM Choice
Groq API is used due to:
- Fast inference
- Free-tier availability
- Suitable for real-time applications