# Project Scope — AI Mock Interview Platform

## 1. Project Vision

The project aims to develop an **AI-powered mock interview platform** that simulates realistic interview experiences using a **multi-agent system**, **real-time voice interaction**, **CV understanding**, and an **interactive avatar with lip sync**.

The system is designed to help students and job seekers practice interviews in a structured and intelligent environment while receiving automated feedback on their performance.

---

## 2. MVP Scope

### A. CV Analysis and Role Inference

The interview process begins with uploading the user’s CV.  
A dedicated **Candidate Intelligence Agent** analyzes the CV and extracts structured information such as:

- skills  
- tools/technologies  
- projects  
- experience level  

Based on this information, the system **infers a suggested target role**, which the user can review and modify before starting the interview.

---

### B. Multi-Agent Interview System

The system follows a **multi-agent architecture** composed of three main agents:

#### 1. Candidate Intelligence Agent
- Parses the CV
- Extracts structured candidate information
- Infers target role

#### 2. Interview Orchestrator Agent
- Plans the interview flow
- Selects/generates questions (RAG + LLM)
- Manages interview state
- Handles interaction logic

#### 3. Evaluation & Reporting Agent
- Evaluates answers
- Generates scores
- Produces feedback
- Creates final report

---

### C. Real-Time Voice Interview (Streaming-Based)

The system provides a **real-time voice-based interview experience**:

- Questions are delivered using **Text-to-Speech (TTS)**  
- The user responds via microphone  
- Speech is converted to text using **Speech-to-Text (STT)**  
- The system processes responses dynamically during the session  

This creates a live interview experience rather than a text-based interaction.

---

### D. Interview Question Pipeline

The system generates interview questions based on:

- extracted CV information  
- inferred or user-selected role  
- predefined question bank  
- LLM-generated follow-up questions  

The platform supports:
- technical questions  
- HR questions  
- project-based questions  
- adaptive follow-up questions  

---

### E. AI-Based Answer Evaluation

Each user response is evaluated using AI models based on:

- relevance  
- technical correctness  
- clarity  
- completeness  

The system generates:
- score per answer  
- feedback per answer  
- aggregated evaluation  

---

### F. Avatar with Lip Sync (Prototype)

The system includes a **simple interviewer avatar** that:

- presents questions visually  
- synchronizes basic lip movement with generated speech  
- enhances realism and user engagement  

This feature is implemented as a **lightweight prototype**.

---

### G. Final Interview Report

At the end of the interview, the system generates a report including:

- overall score  
- category-based performance  
- strengths  
- weaknesses  
- improvement recommendations  

---

### H. Web Interface

The system includes a web interface that allows users to:

- upload CV  
- review/edit inferred role  
- start interview  
- interact during the session  
- view final report  

---

## 3. In-Scope Summary

The MVP includes:

- CV upload and parsing  
- role inference with user adjustment  
- multi-agent system (3 agents)  
- question bank integration  
- LLM-based question generation  
- real-time voice interaction  
- STT and TTS integration  
- avatar with lip sync (prototype)  
- answer evaluation system  
- final report generation  
- web interface  

---

## 4. Out of Scope

The following features are excluded from the current version:

- emotion detection using facial analysis  
- body language analysis (computer vision)  
- multi-language support  
- production-scale deployment  
- long-term user analytics  

---

## 5. Constraints

- The system must rely on **free or open-source tools**  
- The project is developed by a **team of 5 students**  
- Real-time processing must be optimized for limited hardware  
- Some features may be implemented in simplified form  

---

## 6. Assumptions

- Users provide CVs in supported and readable formats  
- Users have access to a microphone  
- Selected models can run locally or via free-tier APIs  
- A sufficient question bank is available  

---

## 7. Identified Risks

### 1. Real-Time Voice Complexity
Implementing real-time streaming and maintaining low latency may be challenging.

### 2. Lip Sync Integration
Synchronizing avatar movement with speech may require optimization.

### 3. Multi-Agent Coordination
Managing communication between agents may introduce complexity.

### 4. Free Model Limitations
Free/open-source models may have limitations in accuracy or availability.

---

## 8. Risk Mitigation Strategies

- Start with simplified pipelines and iterate  
- Use lightweight and efficient models  
- Design modular architecture  
- Perform incremental testing and integration  

---

## 9. Target Users

- University students  
- Fresh graduates  
- Job seekers preparing for interviews  

---

## 10. Summary

This project delivers a practical AI-driven mock interview platform that combines:

- CV understanding  
- multi-agent systems  
- real-time voice interaction  
- AI-based evaluation  

The system is designed to be **cost-efficient**, **modular**, and **scalable**, making it suitable as a graduation project with strong technical depth and real-world applicability.