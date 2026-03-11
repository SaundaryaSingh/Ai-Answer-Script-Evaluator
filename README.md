# Ai-Answer-Script-Evaluator
<img width="1904" height="943" alt="image" src="https://github.com/user-attachments/assets/aa36a95d-60e1-4e08-bfeb-b099a54c1abb" />


🧠 AI Answer Script Evaluator

An AI-powered automated grading system that evaluates student answers using Large Language Models (LLMs).
The system compares student responses with reference answers and generates detailed evaluation reports including scores, feedback, strengths, and improvement suggestions.

The project uses LangChain with the DeepSeek-R1 model via Ollama to perform semantic answer evaluation rather than simple keyword matching.

🚀 Key Features
🧠 AI-Based Answer Evaluation

Uses DeepSeek-R1 LLM to analyze student answers and evaluate conceptual correctness.

📊 Automated Scoring

Generates numerical scores (0-100) for each answer using LLM reasoning.

📝 Detailed Feedback

Each evaluation includes:

Score

Feedback

Strengths

Areas for improvement

📄 Automatic Report Generation

Creates structured HTML evaluation reports for easy viewing.

🔄 Batch Student Processing

Supports evaluation of multiple students automatically from uploaded answer files.

🔒 Privacy-First Architecture

Runs LLMs locally using Ollama, ensuring:

No external API calls

Secure academic data processing

Offline evaluation capability

🏗 System Architecture
Student Answer Files (.txt)
           │
           ▼
Flask API Upload Endpoint
           │
           ▼
Evaluation Engine (LangChain + DeepSeek-R1)
           │
           ▼
AI Reasoning & Scoring
           │
           ▼
Structured Evaluation Output
           │
           ▼
HTML + JSON Report Generation
⚙️ Tech Stack
Backend

Python

Flask

AI / LLM

LangChain

Ollama

DeepSeek-R1

Data Processing

Pandas

Frontend / Output

HTML

CSS
🔄 Evaluation Workflow

1️⃣ Instructor uploads student answer files

2️⃣ Flask API triggers the AI evaluation engine

3️⃣ LangChain sends prompts to DeepSeek-R1

4️⃣ The model analyzes:

answer correctness

conceptual understanding

explanation clarity

5️⃣ AI generates structured evaluation including:

score

feedback

strengths

improvements

