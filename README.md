#  Personal Finance Tracker Agent 

A conversational expense tracker built with LangGraph, LangChain, and OpenAI GPT-4o-mini.

---

##  Tools

### Custom Python Tools
| Tool | What it does |
|---|---|
| `add_expense` | Adds a new expense with description, amount, and category |
| `list_expenses` | Lists all recorded expenses with IDs and total |
| `delete_expense` | Deletes an expense by ID (requires human approval) |
| `summarize_by_category` | Groups and totals spending by category |
| `get_token_usage` | Shows input/output tokens used and estimated cost |

### External API Tools
| Tool | API | What it does |
|---|---|---|
| `get_exchange_rate` | Frankfurter API (free) | Live currency exchange rates |
| `get_crypto_price` | CoinGecko API (free) | Current crypto prices with 24h change |

---

## ✨ Features
-  Add/list/delete expenses by category
-  Spending summary by category
-  Live currency rates via Frankfurter API
-  Crypto prices via CoinGecko API
-  Token usage tracking with cost estimate
-  Human approval before any deletion (interrupt)
-  Multi-turn memory with LangGraph MemorySaver
-  Interactive CLI loop for terminal chat

---

##  Setup
1. Open `Final_agent (1).ipynb` in Google Colab
2. Run Cell 2 (pip install)
3. Paste your OpenAI API key in Cell 3
4. Run all cells top to bottom

---

##  Dependencies
langgraph, langchain, langchain-openai, requests, pydantic
