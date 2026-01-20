# AI Resume Critiquer

A simple **Streamlit** web app that lets users upload their resume (PDF or TXT) and receive **AI‑powered, structured feedback** tailored to a specific job role using OpenAI’s `gpt-4o-mini` model.[web:74][web:81][web:84][web:87]

---

## Features

- Upload resumes in **PDF** or **plain text** format via `st.file_uploader`.[web:74][web:73]  
- Extract text from multi‑page PDFs using **PyPDF2**.[web:79][web:85]  
- Optional **job role** input to customize feedback (e.g., “Data Analyst”, “Product Manager”).  
- Sends resume content to OpenAI’s **Chat Completions API** with an expert HR reviewer system prompt.[web:81][web:84][web:87]  
- Returns **clear, structured analysis** focusing on:
  - Content clarity and impact  
  - Skills presentation  
  - Experience descriptions  
  - Role‑specific improvement suggestions  

---

## Tech Stack

- **Frontend / App**: [Streamlit](https://streamlit.io/)  
- **PDF Parsing**: [PyPDF2](https://pypdf2.readthedocs.io/) for text extraction.[web:79][web:85]  
- **AI Model**: OpenAI `gpt-4o-mini` via the official `openai` Python SDK and Chat Completions API.[web:81][web:84][web:87]  
- **Config / Secrets**: Environment variables managed with `python-dotenv`.  
