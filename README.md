# Service Desk Assistant (Ai)
AI-powered chatbot for troubleshooting assistance (using Copilot Studio)

# Project Plan
## 1. Core Capabilities of the AI Agent
The chatbot will integrate with multiple data sources to assist in troubleshooting tasks effectively.

**Multi-Source Data Integration**
- **OneDrive/SharePoint:** For Word, Excel, and SOP documents.
- **GitHub API:** To fetch issues, project boards, and repository details.
- **Microsoft Teams API:** For retrieving chat messages and channel discussions.
- **Internal Databases:** For client details, and credentials (securely stored).

**Natural Language Understanding (NLU)**
The agent must interpret natural language queries and map them to actions, such as:
- "Share me the Client details of OMK" → Retrieve client details from CRM or Excel.
- "What is the POS pin for Subway Chur?" → Query internal database for the POS pin.
- "How to configure Nexi Terminal?" → Fetch relevant SOP from OneDrive.

**Contextual Search & Summarization**
The agent will use semantic search to find relevant documents and summarize them to provide quick answers.

## 2. Architecture Overview
The AI agent will have a multi-layered architecture:

**Frontend:**
- Web interface, Microsoft Teams Bot, or Slack Bot.

**Backend:**
- **AI Layer:** Uses an LLM (like GPT or Azure OpenAI) to understand user queries and generate responses.
- **Connector Layer:** Uses APIs to integrate with OneDrive, GitHub, Teams, and internal databases.
- **Search Engine:** Uses Azure Cognitive Search or ElasticSearch for quick document retrieval.
- **Security:** OAuth for secure connections to OneDrive, Teams, GitHub, and Azure Key Vault for storing sensitive data.

## 3. Workflow for Query Handling
The following steps define how the agent will handle user queries:
1. **User Query → Intent Detection:**
   - Example: "Share me the device list of xx location" → Intent: GetDeviceList.
3. **Source Identification:**
   - Device list → Excel in OneDrive.
   - Ticket updates → GitHub + Teams.
5. **Data Retrieval:**
   - Use Graph API to fetch data from OneDrive/Teams.
   - Use GitHub REST API to retrieve issues and project boards.
7. **Response Generation:**
   - Summarize retrieved data and present it to the user, including links to the source files if necessary.

## 4. Sample Queries and Responses
Here are examples of the types of queries the chatbot will handle and how it will respond:
- **Query 1: "Share me the Client details of OMK"**
  → Search OneDrive/Excel for "OMK Client Details" → Return structured client information.
- **Query 2: "What is the email and pass for Subway Chur?"**
  → Retrieve credentials securely from Azure Key Vault.
- **Query 3: "What is the POS pin for xx location of x client?"**
  → Query internal database or Excel sheet to get the POS pin.
- **Query 4: "How to configure Nexi Terminal?"**
  → Search SOP in OneDrive or Confluence and summarize steps.
- **Query 5: "What is the latest update of today’s ticket?"**
  → Fetch GitHub issues updated today and summarize Teams discussion threads.

## 5. Tools & Tech Stack
The chatbot will use the following technologies and APIs:
- **APIs:**
  - Microsoft Graph API (for OneDrive, Teams).
  - GitHub REST API (for repository and issue tracking).
- **AI:**
  - Azure OpenAI or OpenAI GPT for NLU and response generation.
- **Search:**
  - Azure Cognitive Search for indexing documents.
- **Integration:**
  - Power Automate for workflow automation or custom middleware.

