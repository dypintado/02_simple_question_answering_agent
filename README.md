# 🤖 Simple Question-Answering Agent

My own implementation of a simple QA agent using LangChain and OpenAI — part of my ongoing series building AI agents from scratch.

> Based on the agent pattern from [NirDiamant/GenAI_Agents](https://github.com/NirDiamant/GenAI_Agents), rebuilt and customized independently.

---

## What It Does

A conversational question-answering agent that takes any user question and returns a clear, concise answer using OpenAI's `gpt-4o-mini` model, orchestrated through LangChain's prompt + chain architecture.

---

## Tech Stack

| Tool | Purpose |
|---|---|
| `LangChain` | Chain orchestration and prompt templating |
| `langchain-openai` | OpenAI model integration |
| `OpenAI gpt-4o-mini` | Language model for Q&A |
| `python-dotenv` | Secure API key management |
| `Jupyter Notebook` | Interactive development environment |

---

## Project Structure

```
02_simple_question_answering_agent/
├── simple_question_answering_agent.ipynb   # Main notebook
├── .env                                     # API key (not committed)
├── .gitignore                               # Ignores .env and .venv
└── README.md
```

---

## Setup & Run

### 1. Clone the repo
```bash
git clone https://github.com/dypintado/02_simple_question_answering_agent.git
cd 02_simple_question_answering_agent
```

### 2. Create a virtual environment
```bash
python -m venv .venv

# Windows
.venv\Scripts\Activate.ps1

# Mac/Linux
source .venv/bin/activate
```

### 3. Install dependencies
```bash
pip install langchain langchain-openai python-dotenv jupyter openai
```

### 4. Add your OpenAI API key
Create a `.env` file in the root directory:
```
OPENAI_API_KEY=your-key-here
```

### 5. Launch the notebook
```bash
jupyter notebook
```

Open `simple_question_answering_agent.ipynb` and run all cells.

---

## How It Works

```
User Question
     ↓
PromptTemplate  →  Formats the question into a structured prompt
     ↓
ChatOpenAI      →  Sends prompt to gpt-4o-mini
     ↓
LLMChain        →  Returns the model's response
     ↓
Answer
```

---

## Example Output

```
Question: What is the capital of France?
Answer: The capital of France is Paris.
```

---

## Part of a Series

This is **Build #02** in my AI Agents implementation series. Each build explores a different agent pattern with my own implementation twist.

| Build | Agent Type | Status |
|---|---|---|
| 01 | *(coming soon)* | 🔜 |
| 02 | Simple Q&A Agent | ✅ Done |
| 03 | *(coming soon)* | 🔜 |

---

## Author

**Dylan Pintado** — AI Automation Engineer & Founder of [FlowForge AI](https://dylanpintado.com)

Building voice receptionists, workflow automations, and custom AI solutions for businesses.

- 🌐 [dylanpintado.com](https://dylanpintado.com)
- 💼 [LinkedIn](https://linkedin.com/in/dylanpintado)
- 🐙 [GitHub](https://github.com/dypintado)
