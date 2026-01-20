# AI News Aggregator

An end‑to‑end **GenAI application** that collects AI news from multiple sources (YouTube, blogs, RSS), summarizes it with LLMs, stores everything in Postgres, and sends you a personalized daily email digest.[web:63][web:70]

---


## Features

- **Multi‑source scraping pipeline**  
  - YouTube channels via RSS + `youtube-transcript-api` for transcripts.  
  - AI blogs (e.g., OpenAI, Anthropic) and custom RSS feeds.[web:63]  

- **LLM‑powered summarization and ranking**  
  - Uses OpenAI models to summarize articles and rank them based on a user profile / system prompt.[web:63][web:69]  

- **Postgres‑backed storage**  
  - Stores sources, articles, transcripts, and generated digests using SQLAlchemy models.[web:63]  

- **Daily digest email**  
  - Scheduled job runs every 24 hours, builds a digest in Markdown/HTML, and emails it to the configured recipients.[web:63]  

- **Docker & production‑ready deployment**  
  - Docker Compose for local dev and a Render‑compatible setup for production hosting and scheduling.[web:63][web:70]  

---

## Architecture

At a high level, the system:

1. **Scrapes sources** (YouTube, blogs, RSS) and normalizes them into `Article` objects.[web:63]  
2. **Stores raw and processed content** in Postgres (via SQLAlchemy).[web:63]  
3. **Runs an LLM “aggregator agent”** that:
   - Clusters and ranks articles.
   - Produces a personalized daily digest.[web:63]  
4. **Sends the digest via email** through a simple email service abstraction.[web:63]  
5. **Runs on a schedule** (cron / Render job) for full automation.[web:63][web:70]  

---

## Tech Stack

- **Language**: Python  
- **AI / LLMs**: OpenAI API (chat + embeddings).[web:63][web:69]  
- **Database**: Postgres (local Docker container + managed DB in production).[web:63][web:70]  
- **ORM**: SQLAlchemy.[web:63]  
- **Scraping**: RSS feeds, HTTP clients.[web:63]  
- **Infra & Dev**: Docker, Docker Compose, uv / pyproject‑based dependency management.[web:63][web:69]  
- **Deployment**: Render Web Service + Render Cron Job.[web:63][web:70]  


**The most valuable learning happens when you struggle, reference the code, and push through to the next checkpoint.**
