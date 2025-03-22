# AI-Powered Financial Report Generator

This project is an **AI agent system** designed to automate the process of researching, analyzing, and generating insightful **financial reports** using **Streamlit**, **AutoGen**, and **OpenAI GPT-4o**.

It builds a multi-agent collaborative workflow for analyzing stock performance, extracting recent news, and generating markdown reports, complete with financial metrics, figures, and AI-driven reviews for consistency, legal compliance, and content completion.

---

## 🚀 Features

- ✅ Automatically fetches and analyzes stock price data and fundamentals (P/E, ROE, etc.)
- 📰 Extracts relevant news headlines using web scraping (no API required)
- ✍️ Generates a comprehensive markdown financial report
- 🧠 AI reviewers provide multi-perspective feedback:
  - Legal compliance
  - Data consistency
  - Textual alignment with data
  - Content completeness
- 🎯 Final meta-review aggregates all feedback to refine the report
- 📈 Visualizes normalized stock prices
- 🔐 Securely loads OpenAI API key with `.env` or Streamlit UI

---
## Deployed application: https://pratyushkr9420-ai-agents-financial-report--streamlit-app-mbsbgp.streamlit.app
---
## To set up the application locally

## 🛠️ Installation

1. **Clone the repository**:

```bash
git clone https://github.com/pratyushkr9420/AI_agents_financial_report_generator_application.git
cd AI_agents_financial_report_generator_application
```

2. **Install dependencies**:

```bash
pip install -r requirements.txt
```

3. **Set your OpenAI API Key**:

- Option 1: Add a `.env` file:
  ```env
  OPENAI_API_KEY=your_openai_key
  ```
- Option 2: Enter your API key in the Streamlit app when prompted

---

## ▶️ Usage

Run the app with:

```bash
streamlit run streamlit_app.py
```

Then:

1. Enter the **stock tickers** (e.g., `AAPL, MSFT, GOOGL`) into the input field.
2. Click the **"Start analysis"** button.
3. Wait for the agents to do their work.
4. View the generated **normalized price chart** and the full **markdown report** below it.

---

## 📂 Output

The final report includes:

- 📊 Normalized stock price chart (`normalized_prices.png`)
- 📉 Financial metric comparisons in a table
- 📚 Analysis of financial ratios and news
- 📌 Cross-stock comparisons, risk correlations
- 🔍 Potential future scenarios

---

## 🧠 AI Agents Involved

- **Financial Assistant** – Retrieves stock data and metrics
- **Researcher** – Extracts relevant news headlines
- **Writer** – Composes the markdown report
- **Critic** – Reviews the report and triggers nested reviewers:
  - Legal Reviewer
  - Consistency Reviewer
  - Text Alignment Reviewer
  - Completion Reviewer
  - Meta Reviewer

---

## 📎 Notes

- No external financial APIs are required (uses scraping where needed)
- Make sure to run in an environment with internet access
- This app is experimental and for educational/research purposes

---

## 🙏 Acknowledgments

Built using:

- [OpenAI](https://openai.com/)
- [AutoGen](https://github.com/microsoft/autogen)
- [Streamlit](https://streamlit.io/)
- [Python-dotenv](https://github.com/theskumar/python-dotenv)
