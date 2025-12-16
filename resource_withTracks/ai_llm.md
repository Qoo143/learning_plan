# AI & LLM 應用學習資源

> 最後更新: 2025-12-16
> 這是你的興趣路線！

---

## 免費資源

### 🐍 Python 基礎

| 資源 | 說明 | 連結 |
|------|------|------|
| **Python 官方教程** | 官方入門 | https://docs.python.org/3/tutorial/ |
| **Real Python** | 高品質 Python 教程 | https://realpython.com/ |
| **Codecademy Python** | 互動學習 (部分免費) | https://www.codecademy.com/learn/learn-python-3 |

### 🤖 LangChain & RAG

| 資源 | 說明 | 連結 |
|------|------|------|
| **LangChain 官方文檔** | 最權威的 LangChain 教學 | https://python.langchain.com/docs/ |
| **freeCodeCamp - Learn RAG From Scratch** | LangChain 工程師教的 RAG 課程 | https://www.youtube.com/watch?v=... (搜尋 "freeCodeCamp RAG LangChain") |
| **LangChain Master Class 2024** | 20+ 程式碼範例 + 免費原始碼 | 搜尋 "LangChain Master Class Beginners 2024" |
| **LangChain Build RAG Agent** | 官方 RAG Agent 教學 | https://python.langchain.com/docs/tutorials/rag/ |

### 🧠 AI Agent

| 資源 | 說明 | 連結 |
|------|------|------|
| **LangGraph 官方教學** | Agent 進階框架 | https://langchain-ai.github.io/langgraph/ |
| **DEV Community - Building LangChain Agent** | 從零建立 Agent | https://dev.to/ |
| **KDnuggets - Agentic RAG** | Agent + RAG 整合 | https://www.kdnuggets.com/ |

### 🏠 本地 AI (Ollama)

| 資源 | 說明 | 連結 |
|------|------|------|
| **freeCodeCamp - Local AI with Qwen & Ollama** | 免費本地 AI 建置 | https://www.freecodecamp.org/ |
| **YouTube - Local RAG with Ollama** | 免費本地 RAG | 搜尋 "Local RAG Ollama LangChain" |

---

## 學習路線建議

```
1. Python 基礎 (1-2 週)
   ↓
2. OpenAI API 基礎 (1 週)
   ↓
3. LangChain 基礎 (1-2 週)
   ↓
4. RAG 系統建置 (2-3 週)
   ↓
5. AI Agent 開發 (持續)
```

---

## 推薦的第一個專案

**CLI Chatbot**: 用 Python + OpenAI API 做一個命令列聊天機器人

```python
# 簡單範例
from openai import OpenAI

client = OpenAI()
response = client.chat.completions.create(
    model="gpt-3.5-turbo",
    messages=[{"role": "user", "content": "Hello!"}]
)
print(response.choices[0].message.content)
```

---

## 我的學習紀錄

(學完後回來評價哪個資源最有用)

