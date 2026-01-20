A curated **workspace of AI and ML projects** built while learning modern data science, ML engineering, and GenAI.  
Each folder or script in this repo is a self‑contained project that can go into your portfolio.

> This workspace currently includes:  
> - AI Agent (LangChain / LangGraph style tools)  
> - AI News Aggregator (GenAI end‑to‑end app)  
> - Cold Email Generator – GenAI  
> - Resume Critiquer (Streamlit + OpenAI)  
> - ZenML & MLflow – Price Prediction System  
> - Stand‑alone Python projects: AI Discord ChatBot, AI Voice Assistant, Image Classifier, Recommendation system, Sentiment Analysis.[file:113]

---

## Repository Layout

From the root of the repo:[file:113]

- `.idea/` – IDE configuration (PyCharm/IntelliJ, safe to ignore for usage).  
- `AI Agent/` – CLI or app showcasing tool‑calling agents (e.g., calculator, greeting, etc.).  
- `AI News Aggregator/ai-news-aggregator/` – GenAI project that scrapes AI content, summarizes with LLMs, and sends digests.  
- `Cold Email Generator - GenAI/` – Project for generating tailored cold emails using LLM prompts.  
- `Resume Critiquer/` – Streamlit app that uploads a resume (PDF/TXT) and returns AI‑powered feedback.  
- `ZenML & MLFlow - Price Prediction System/` – End‑to‑end MLOps house‑price prediction pipeline with ZenML + MLflow.  
- `AI Discord ChatBot.py` – Script for building a Discord bot powered by an LLM.  
- `AI Voice Assistant.py` – Voice assistant script (speech‑to‑text + LLM + TTS).  
- `Image Classifier.py` – Basic computer‑vision classification project.  
- `Recommendation.py` – Recommender system (e.g., content‑based or collaborative filtering).  
- `Sentiment Analysis.py` – Text sentiment classifier.  

(See individual project folders for more detailed READMEs and code.)

---

## Tech Stack

Most projects use a similar core stack:

- **Language**: Python 3.x  
- **Data / ML**: `pandas`, `numpy`, `scikit-learn`, plus domain‑specific libs (e.g., CV, NLP).  
- **GenAI / LLMs**: OpenAI API (chat/completions) and LangChain / LangGraph where applicable.  
- **MLOps**: ZenML and MLflow in the price‑prediction system.  
- **Apps & UI**: Streamlit, Discord.py, and other lightweight frameworks depending on the project.  

Each sub‑project may define its own dependencies via `requirements.txt` or `pyproject.toml`.

