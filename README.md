# Service Desk Assistant (Ai)
AI-powered chatbot for troubleshooting assistance (using Copilot Studio)

# Project Plan
## 1. Core Capabilities of the AI Agent
The chatbot will integrate with multiple data sources to assist in troubleshooting tasks effectively.
### Multi-Source Data Integration
- **OneDrive/SharePoint:** For Word, Excel, and SOP documents.
- **GitHub API:** To fetch issues, project boards, and repository details.
- **Microsoft Teams API:** For retrieving chat messages and channel discussions.
- **Internal Databases:** For client details, and credentials (securely stored).
### Natural Language Understanding (NLU)
The agent must interpret natural language queries and map them to actions, such as:
- "Share me the Client details of OMK" → Retrieve client details from CRM or Excel.
- "What is the POS pin for Subway Chur?" → Query internal database for the POS pin.
- "How to configure Nexi Terminal?" → Fetch relevant SOP from OneDrive.
### Contextual Search & Summarization
The agent will use semantic search to find relevant documents and summarize them to provide quick answers.
