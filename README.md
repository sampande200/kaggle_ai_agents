<div align="center">

# 🧠 StudyAlpha-AI-Agent  
## **Autonomous Study & Revision System**  
### *Your Personal AI Study Coach powered by Multi-Agent Intelligence*

[![Made with Python](https://img.shields.io/badge/Python-3.10-blue)]()
[![Multi-Agent System](https://img.shields.io/badge/Multi--Agent-Architecture-brightgreen)]()
[![Machine Learning](https://img.shields.io/badge/ML-Weakness%20Prediction-orange)]()
[![RAG](https://img.shields.io/badge/RAG-TF--IDF%20Memory-purple)]()
[![Streamlit](https://img.shields.io/badge/UI-Streamlit-red)]()


---

# 🚀 Google × Kaggle Agents Intensive – Capstone Project  
## 🏆 *Hackathon Writeup + Full System Documentation*

---

# 🟦 Problem Statement  

Students today struggle with **learning consistency**.  
Effective learning requires:

- 🗂️ structured planning  
- 📊 progress tracking  
- 📝 performance evaluation  
- ❗ early detection of weak topics  

Most learners **don’t know what to study next**, how long to study, or when to revise.  
Traditional AI tools simply **answer questions** — they don’t:

- plan  
- evaluate  
- remember  
- adapt  

💡 **StudyAlpha solves this** by acting as a complete, autonomous study coach that:

- plans the study roadmap  
- generates quizzes  
- evaluates understanding  
- predicts weaknesses using ML  
- adjusts future study sessions automatically  


---

# 🤖 Why I Used Agents  

Learning involves multiple interdependent tasks:

✔ planning  
✔ quizzing  
✔ evaluating  
✔ memory retrieval  
✔ weakness prediction  
✔ revision scheduling  

No single LLM call can manage this entire workflow.

### Agents enable:
- 🔹 **Modularity** — each task handled by a specialized sub-agent  
- 🔹 **Delegation** — one agent passes output to the next  
- 🔹 **Memory** — mistakes & patterns influence future learning  
- 🔹 **Multi-step reasoning** — structured learning cycles  
- 🔹 **Extensibility** — new agents or tools can be added easily  

📘 StudyAlpha behaves like a **real human tutor** — thoughtful, adaptive, and aware of past performance.


---

🌐 Deployment
Platform: Streamlit Cloud
Entry file: app.py
Auto-deploy: On every push to main



# 🏗️ Architecture Overview  

StudyAlpha is a **multi-agent learning ecosystem** orchestrated by a central StudyOrchestrator.

---

## 1️⃣ **StudyOrchestrator (Master Controller)**  
Controls the entire pipeline:

- planning  
- quiz creation  
- evaluation  
- tracking  
- revision generation  

---

## 2️⃣ **Planner Agent**  
Builds personalized study plans using:

- topics  
- priority  
- difficulty  
- available hours  
- duration  

Outputs a **multi-day optimized schedule**.

---

## 3️⃣ **Quiz Agent**  
- Generates **3 conceptual questions**  
- Uses a **TF-IDF RAG Memory**  
- Pulls context from past mistakes & logs  

---

## 4️⃣ **Revision Agent**  
Generates targeted revision tasks based on:

- past mistakes  
- predicted weaknesses  
- forgotten topics  

Optimized for **spaced repetition**.

---

## 5️⃣ **Tracker Agent**  
Evaluates quiz answers and logs:

- accuracy  
- score  
- correctness patterns  

Feeds data into the ML model.

---

## 6️⃣ **Weakness Predictor (ML Model)**  
A **GradientBoostingClassifier** predicts:

- weakness probability  
- likelihood of future mistakes  
- topics needing urgent focus  

---

## 7️⃣ **Memory Bank (RAG System)**  
Stores and retrieves:

- quizzes  
- explanations  
- errors  
- performance logs  
- improvement history  

Powered by **TF-IDF + Cosine Similarity**.

---

## 8️⃣ **Streamlit UI (Optional)**  
A simple interface to:

- generate study plans  
- take quizzes  
- see analytics  
- visualize performance  


---

# 🔄 Architecture Summary  

```
Plan → Quiz → Evaluate → Predict Weakness → Revise → Store Memory → Adapt Next
```

---

# 🖼️ Architecture Diagram  
StudyOrchestrator
                 (Master Controller Agent)
                             |
        ------------------------------------------------
        |                      |                      |
        |                      |                      |
  Planner Agent           Quiz Agent           Revision Agent
 (Create Plan)          (Generate Questions)    (Revise Topics)
        |                      |                      |
  create_plan()          generate_quiz()      generate_revision()
                               |
                         evaluate_quiz()
                               |
                         Tracker Agent
                   (Evaluation, Weakness)
                               |
                  ML Weakness Predictor
                (GradientBoostingClassifier)
                               |
                        Memory Bank (RAG)
                  (TF-IDF + Cosine Similarity)
                               |
                         Streamlit UI
                 (Optional Local Demo Frontend)
                 


---

# 🎬 Demo and Simulation  

The notebook demonstrates a **full 7-day learning simulation**:

- study plans  
- quiz generation  
- evaluation  
- ML-based weakness prediction  
- dynamic revision cycles  
- memory retrieval  
- performance graphs  
- time allocation charts  
- exported reports  


---

# 📅 Study Plan Example  

For topics:

- Arrays – Priority 2  
- Graphs – Priority 1  
- DP – Priority 2  

The planner builds a **7-day optimized schedule**.

---


## 🔄 2) WORKFLOW DIAGRAM  
> *(Insert your workflow diagram image below — drag & drop into GitHub editor and replace the link)*

User Input
(topics, priority, hours/day)
          ↓
StudyOrchestrator
(Master Controller Agent)
          ↓
Planner Agent
          ↓
Study Plan (7-Day Plan)
          ↓
Quiz Agent
          ↓
Sample Quiz (3 Questions)
          ↓
User Answers
          ↓
Tracker Agent
(Evaluation + ML Predictor)
          ↓
Weakness Probability
          ↓
Revision Agent
          ↓
Updated Revision Plan


# 📝 Quiz Generation  

Example for topic **DP**:

- 3 conceptual MCQs  
- Memory-aware grounding  


---

# 📈 Evaluation & Tracking  

Logs include:

- correct / incorrect  
- explanations  
- topic-wise accuracy  


---

# 🔮 Weakness Prediction  

ML model assigns a numerical probability:

```
Weakness Probability: 0.73  
→ High chance of confusion  
```

---

# 🔁 Revision Planning  

Revision Agent outputs:

- targeted tasks  
- recommended questions  
- spaced repetition intervals  

---

# 📊 Analytics & Visualizations  

Includes:

- study-time distribution chart  
- accuracy line graph  
- mistake clusters  
- topic dependency graph  
- memory-retrieval maps  
- revision heatmaps  

---

# 🛠️ The Build  

### ✨ Engineering Philosophy  
StudyAlpha is:

- modular  
- reproducible  
- deterministic  
- easy to test  
- extendable  

### 🧰 Technologies Used  

- Python  
- Scikit-learn  
- Pandas / NumPy  
- TF-IDF / Cosine Similarity  
- Streamlit  
- Joblib  
- Logging & Tracing  

### 🔧 Key Design Decisions  

- Deterministic mock LLM (no API keys required)  
- True multi-agent architecture  
- RAG-based quiz grounding  
- ML-based weakness prediction  
- Structured modular repository  

### 📦 Notebook Includes  

- agent modules  
- memory system  
- planner/quiz/revision pipelines  
- ML training + explainability  
- analytics & visualizations  
- reproducible tests  
- synthetic student simulation  

---

# ⏳ Future Improvements  

- Gemini Integration for richer feedback  
- Cloud deployment (API/Serverless)  
- Long-term spaced repetition pipeline  
- Daily streak tracking  
- PDF/notes ingestion  
- Leaderboards & gamification  

---

# 📝 Final Note  

**StudyAlpha acts like a real AI tutor — doing more than answering questions.**  
It thinks, plans, evaluates, adapts, and remembers.

This system combines:

- multi-agent intelligence  
- memory  
- ML prediction  
- structured planning
-  
---

# 👤 Author  
### **Samiksha Pande**  
AI & Web Developer  
*“Solve. Fail. Learn. Repeat.”*

- GitHub Repository: ****
