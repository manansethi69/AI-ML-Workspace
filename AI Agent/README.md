# LangGraph ReAct CLI Agent

A minimal command-line AI assistant built with **LangChain** and **LangGraph**.  
It demonstrates how to wire a ReAct-style agent to Python tools (a calculator and a greeter) and stream responses in the terminal.[web:3][web:16][web:26][web:36]

---

## Features

- ReAct-style agent created via `create_react_agent` from LangGraph.[web:3][web:16][web:36]  
- Two built-in tools using the `@tool` decorator:
  - `calculator(a: float, b: float) -> str` for simple arithmetic on two numbers.
  - `say_hello(name: str) -> str` for returning a greeting.[web:19][web:26]  
- Streaming CLI loop that:
  - Reads user input continuously.
  - Streams model responses chunk-by-chunk.
  - Exits cleanly when the user types `quit`.[web:3][web:16]

---

## Tech Stack

- Python 3.9+  
- [LangChain](https://docs.langchain.com/) (`langchain-core`, `langchain-openai`)[web:26]  
- [LangGraph](https://langchain-ai.github.io/langgraph/)[web:3][web:16]  
- [python-dotenv](https://pypi.org/project/python-dotenv/) for loading environment variables.  

---

## Getting Started

### Prerequisites

- Python 3.9 or later installed.  
- An OpenAI-compatible API key (for example, `OPENAI_API_KEY`).[web:20][web:22]

### Installation

Clone your repository and install dependencies:

```bash
git clone <your-repo-url>.git
cd <your-repo-name>

pip install langchain-core langchain-openai langgraph python-dotenv
