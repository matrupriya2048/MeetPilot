# 🚀 MeetPilot

Your AI-powered co-pilot for planning, managing, and extracting insights from meetings — all in one sleek, automated workspace. Built with LangChain, CrewAI, and integrated with productivity tools like Todoist and Telegram.

## 🔍 Features

- 📄 **Meeting Setup**: Define company details, objectives, attendees, and upload supporting documents.
- 🧠 **AI-Powered Analysis**:
  - Generates **contextual summaries and insights**.
  - Designs **time-optimized meeting strategies**.
  - Creates **executive briefs** for quick decision-making.
- ❓ **Q&A Assistant**: Ask contextual questions about your meeting materials using embedded knowledge.
- ✅ **Task Management**:
  - Extracts action items from transcripts.
  - Automatically creates Todoist projects and tasks.
  - Notifies your team via Telegram.

## 🛠 Tech Stack

- **Frontend**: [Streamlit](https://streamlit.io/)
- **LLM**: GPT-4 via [LangChain](https://www.langchain.com/)
- **Vector Database**: FAISS
- **Agents**: [CrewAI](https://docs.crewai.com/)
- **Integrations**:
  - [Todoist API](https://developer.todoist.com/rest/v2/)
  - [Telegram Bot API](https://core.telegram.org/bots/api)

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/matrupriya2048/MeetPilot.git
cd MeetPilot
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Make sure `requirements.txt` includes:

- streamlit
- pandas
- langchain
- langchain-openai
- faiss-cpu
- crewai
- requests

### 3. Add API Keys

In the sidebar of the app, provide:
- OpenAI API Key (required)
- Todoist API Key (optional for task creation)
- Telegram Bot Token & Chat ID (optional for notifications)

### 4. Launch the App

```bash
streamlit run Meeting_agent.py
```

## 📁 Project Structure

```
.
├── Meeting_agent.py      # Core Streamlit application
├── utils.py              # Integrations and task logic
├── requirements.txt      # Dependencies
└── README.md             # You're here!
```

## 🧠 How MeetPilot Works

1. **Configure your meeting**: Company, objective, attendees, focus areas, documents.
2. **CrewAI Agents** take over:
   - Analyze context
   - Generate strategies and briefing documents
3. **Embed everything into FAISS** for searchable Q&A.
4. **Extract tasks** using AI and assign them via Todoist.
5. **Send task summaries** on Telegram with just a click.

## 🔐 API Notes

- GPT-4 is used through LangChain’s integration with OpenAI. You need GPT-4 access.
- Google Meet, WhatsApp, and Telegram transcript fetchers are placeholder simulations. API integration can be expanded.

## 📬 Contact

For queries, improvements, or collaborations, raise an issue on GitHub or connect via [LinkedIn](https://www.linkedin.com/](https://www.linkedin.com/in/matrupriya-dibyanshu-panda-386b38251/).

---

### ⭐ Star this project if MeetPilot helped you take off 🚀
