# 💸 Broke No More 2.0 — AI-Powered Personal Finance Agent

> A smart, modular, agent-based personal finance assistant built using **LangChain**, **LangGraph**, **Gemini Pro**, and **FAISS**.  
> From tracking expenses to offering contextual financial advice — your AI wallet just got an upgrade.

---

### 📌 Overview

**Broke No More 2.0** is a multi-agent, AI-powered personal finance assistant that uses natural language to manage and analyze your financial data. It builds on the earlier version with major architectural upgrades, including:

- 🧠 **LLM-powered agents** using Google Gemini
- 🔄 **LangGraph memory & tool chaining**
- 🗂️ **FAISS vector store** for semantic financial document retrieval
- 📊 **Expense tracker agent** with dynamic state tracking
- 💬 **General financial advisor agent** with LangChain tools
- ⚛️ **React-style dynamic agent flow**

---

### 🧩 Key Features

| Feature | Description |
|--------|-------------|
| **🧾 Expense Tracker Agent** | Parses and logs expenses via natural language |
| **💡 Financial Advisor Agent** | Gives personalized advice based on prior data |
| **🧠 LangGraph Agents** | Modular multi-agent flow with reactive state |
| **🔍 Vector Search** | FAISS-powered semantic retrieval for receipts, docs |
| **🔗 LangChain Tool Use** | Tool calling enabled (e.g., conversion, date parsing) |
| **🪄 Gemini Pro LLM** | Fast, smart, multi-turn conversation support |
| **📦 Local & Cloud Mode** | Works offline with FAISS or cloud Gemini API |
| **🧱 Frontend Ready** | Easy to extend into a Streamlit or web dashboard |

---

### 🤖 Agent Architecture

   +---------------------+
   |  User Input (Chat)  |
   +---------------------+
             |
             v
  +------------------------+
  | LangGraph Agent Router |
  +------------------------+
     /             \
    /               \
+------------------+ +---------------------+
| Expense Tracker | | Financial Advisor |
| - Logs spending | | - Gives insights |
| - Summarizes | | - Suggests action |
+------------------+ +---------------------+
\ /
\ /
+------------------------+
| Vector Search & Memory |
+------------------------+


---

### ⚙️ Tech Stack

- **LLM:** Gemini Pro via Google Generative AI SDK  
- **Framework:** LangChain + LangGraph  
- **Vector Store:** FAISS (custom embeddings for receipts + advice)  
- **Backend:** Python, FastAPI (optional)  
- **Frontend:** (Pluggable: Streamlit or React)  
- **Tools:** tiktoken, pydantic, dateparser, numexpr  

---

### 📦 Example Prompts

```txt
"Log $32 spent on dinner yesterday at Olive Garden"
"How much did I spend on food this week?"
"Am I saving enough compared to last month?"
"Summarize my subscriptions"
"Based on my rent, how much should I spend on groceries?"

🚀 Getting Started
Clone the repo:

git clone https://github.com/<your-username>/BrokeNoMore2.git
cd BrokeNoMore2
Install dependencies:

pip install -r requirements.txt
Configure your env.json:

{
  "GEMINI_API_KEY": "your-api-key",
  "VECTOR_DB_PATH": "./faiss_index/"
}

Run the app:

python main.py

🎯 Use Cases
🧾 Automate and understand your personal spending

📚 Retrieve financial insights from unstructured documents

🧠 Integrate with budgeting goals or salary tracking

📈 Research finance agents, LLM-driven decision flows

👤 Author
Divyansh Pradhan
📧 divyansh.pradhan@stonybrook.edu
