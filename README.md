# 🤖 Agentic AI Workspace

A collection of hands-on projects built using **LangGraph**, **LangChain**, **Groq**, and **LangSmith** to learn Agentic AI concepts from beginner to advanced.

## 🚀 What You'll Learn

- Basic Chatbots with LangGraph
- Human-in-the-Loop Workflows
- Tool Calling Agents
- LangGraph Debugging
- Multi-Agent Systems
- Supervisor-Based Agent Architectures
- LangSmith Tracing & Monitoring

---

## 📁 Project Structure

```bash
1-BasicChatbot/
│
├── 1-basicChatbot.ipynb
├── human in the loop.ipynb
│
├── 3-Debugging/
│   ├── debugging.ipynb
│   ├── agent.py
│   └── langgraph.json
│
└── Agents/
    └── Multiagents.ipynb
```

---

## ⚙️ Setup

### Clone Repository

```bash
git clone <repo-url>
cd AgenticAIWorkspace
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Install Dependencies

```bash
pip install langgraph langchain langchain-groq langsmith tavily-python python-dotenv
```

### Configure Environment Variables

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key
LANGCHAIN_API_KEY=your_langsmith_api_key
LANGSMITH_TRACING=true
```

---

# 📚 Modules

## 1️⃣ Basic Chatbot

**File:** `1-basicChatbot.ipynb`

Learn:

- StateGraph
- MessagesState
- LLM Invocation
- Graph Visualization

Architecture:

```text
START → Chatbot → END
```

---

## 2️⃣ Human-in-the-Loop

**File:** `human in the loop.ipynb`

Learn:

- Interrupts
- Human Approval
- Command Resume
- MemorySaver

Architecture:

```text
User
 ↓
Agent
 ↓
Human Review
 ↓
Agent
 ↓
END
```

---

## 3️⃣ Tool Calling & Debugging

**Folder:** `3-Debugging`

Learn:

- ToolNode
- Tool Binding
- Conditional Routing
- LangGraph Debugging

Example Tool:

```python
@tool
def add(a: float, b: float):
    return a + b
```

Architecture:

```text
START
 ↓
LLM
 ↓
Tool
 ↓
LLM
 ↓
END
```

---

## 4️⃣ Simple Multi-Agent System

**File:** `Agents/Multiagents.ipynb`

Agents:

- Researcher
- Writer

Workflow:

```text
Researcher → Writer → END
```

---

## 5️⃣ Supervisor Multi-Agent System

Agents:

- Supervisor
- Researcher
- Analyst
- Writer

Workflow:

```text
Supervisor
    ↓
Researcher
    ↓
Analyst
    ↓
Writer
```

The Supervisor dynamically decides which agent should work next based on the current state.

---

## 🛠 Tech Stack

- LangGraph
- LangChain
- Groq LLM
- LangSmith
- Tavily Search
- Python

---

## 🎯 Learning Outcomes

After completing these notebooks you'll understand:

- Agentic AI Fundamentals
- Graph-Based Workflows
- Tool Calling
- Human-in-the-Loop Systems
- Debugging LangGraph Applications
- Multi-Agent Collaboration
- Supervisor Agent Patterns

---

## ⭐ Future Improvements

- RAG Pipelines
- Vector Databases
- Long-Term Memory
- MCP Integration
- FastAPI Deployment
- Production Agent Monitoring

---

Built as part of my Agentic AI learning journey using LangGraph, LangChain, Groq, and LangSmith. 🚀