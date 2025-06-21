# 🧠 Autonomous News Agent (n8n Workflow)

This project is an **autonomous news agent** designed using [n8n](https://n8n.io). It automatically fetches, analyzes, filters, and emails the **top 10 AI and technology news stories** relevant to users in India — without any manual input or prompting.

---

## 🚀 Features

- ⏰ **Scheduled Execution** – Runs daily at 9 AM IST
- 🔍 **Dynamic Query Generation** – Searches multiple relevant topics like `AI India`, `Robotics`, `Startup`
- 🗞️ **News Sourcing** – Fetches real-time Google News via [SerpAPI](https://serpapi.com)
- 🧠 **Intelligent Filtering** – Filters based on user-defined interests like "AI", "technology", "India"
- 🏆 **Ranking System** – Ranks and formats top 10 news items
- 📬 **Email Delivery** – Sends a well-designed HTML digest to the user via Gmail

---

## 📁 Workflow Contents

| Node Name            | Purpose                                      |
|----------------------|----------------------------------------------|
| `Daily Trigger`      | Initiates workflow every morning             |
| `Generate Queries`   | Produces topic-based queries                 |
| `Fetch Google News`  | Uses SerpAPI to get news for each topic      |
| `Check for Error`    | Routes API failures to a fallback node       |
| `Fallback News`      | Provides sample content if API fails         |
| `Filter by Interests`| Extracts articles based on relevance         |
| `Summarize & Rank`   | Formats and ranks top stories                |
| `Send Gmail`         | Delivers the news via Gmail in HTML format   |

---

## 📦 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/autonomous-news-agent.git
