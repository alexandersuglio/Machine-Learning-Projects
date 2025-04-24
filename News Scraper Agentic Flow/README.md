# 📰 Agentic News Scraper

This project is an **Agentic Workflow** that autonomously generates a personalized news digest on a random trending topic. It simulates how AI agents can collaborate to plan, search, summarize, and compile information — all without human input after execution.

---

## 🚀 What It Does

The system consists of four agents that work together:

1. **PlannerAgent** – Randomly chooses a topic (e.g., sports, politics, or current events).
2. **SearcherAgent** – Uses Google News search and BeautifulSoup to retrieve relevant article URLs.
3. **SummarizerAgent** – Downloads and summarizes each article using a Hugging Face model (`facebook/bart-large-cnn`).
4. **CompilerAgent** – Formats the summarized content into a clean, Markdown-based newsletter.

At the end, the digest is displayed directly in the notebook using Google Colab’s `Markdown` renderer.

---

## 🧠 Agentic Workflow Example

```mermaid
graph LR
  A[PlannerAgent] --> B[SearcherAgent]
  B --> C[SummarizerAgent]
  C --> D[CompilerAgent]
  D --> E[Newsletter Output]
