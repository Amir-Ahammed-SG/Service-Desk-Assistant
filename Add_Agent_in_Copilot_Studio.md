
# How to Add the Support Monkey AI Chatbot Agent in Copilot Studio

## 1. Log into Copilot Studio
   - Open **Copilot Studio** and log in with your credentials.

## 2. Navigate to the "Agents" Section
   - In **Copilot Studio**, go to the section labeled **Agents** or **AI Models**. This is where you can create and manage the agents that will assist users.

## 3. Click "Add New Agent"
   - Once you’re in the **Agents** section, look for an option to **Add New Agent** and click on it to begin the process of creating your new agent.

## 4. Define the Agent’s Purpose
   - **Agent Name**: Name your agent something descriptive, such as **Support Monkey Agent**.
   - **Description**: Provide a brief description of the agent’s role. For example, “The Support Monkey AI Chatbot assists support agents by retrieving client information, managing support tickets, and offering troubleshooting guidance.”

## 5. Choose Agent Type
   - **AI-Powered Assistant**: Select **AI-Powered Assistant** to use the **GPT** or **Azure OpenAI** model for understanding user queries and generating responses.
   - **Integration Type**: Specify which platforms or tools the **Support Monkey Agent** will interact with. For example:
     - **GitHub**: To retrieve and show the latest support tickets.
     - **OneDrive**: To fetch client details and documents.
     - **Microsoft Teams**: For real-time support interaction with agents.

## 6. Define the Agent’s Capabilities
   - **Core Functionalities**:
     - **Retrieve Client Details**: Fetch client data from **OneDrive** or another cloud storage service.
     - **Support Ticket Updates**: Retrieve the latest support tickets from **GitHub**.
     - **Troubleshooting Guidance**: Provide step-by-step troubleshooting guidance from documents stored in **SharePoint** or **OneDrive**.

   - **Define Topics/Intents**: In this section, specify which queries or topics the agent should handle. For example:
     - **Client Info Query**: “What are the client details for OMK?”
     - **Ticket Update Query**: “What is the latest ticket for Subway Chur?”
     - **Troubleshooting Query**: “How do I configure the Nexi Terminal?”

## 7. Connect Data Sources & External Integrations
   - **OneDrive/SharePoint**: Integrate **OneDrive** to retrieve client details, troubleshooting guides, and documents. Set up the necessary **Microsoft Graph API** access.
   - **GitHub**: Integrate **GitHub** to fetch ticket updates or issues. Provide **Personal Access Tokens (PAT)** for authentication.
   - **Teams**: Integrate **Microsoft Teams** to allow real-time interactions and retrieve chat messages or history.

## 8. Set Up Trigger Actions
   - For each **topic** or **intent**, define **triggers**. These triggers will be used to activate specific responses from the agent.
     - **Example Trigger 1**: “Show me the client details for OMK.”
     - **Example Trigger 2**: “What is the latest ticket for Subway Chur?”

   - **Response Actions**: Specify what happens when a trigger is detected. For example:
     - If the query asks for **client details**, the agent should fetch the data from **OneDrive**.
     - If the query asks for **ticket updates**, the agent should retrieve the latest issues from **GitHub**.

## 9. Test the Agent
   - **Test Interactions**: After setting up the agent, use **Copilot Studio’s testing tools** to simulate queries and ensure the agent responds correctly.
   - For example, test queries like “What is the client info for OMK?” to verify the bot fetches data from **OneDrive** correctly.
   - Refine the agent based on any issues or feedback.

## 10. Publish the Agent
   - Once you are satisfied with the agent’s capabilities and behavior, **publish** the agent in **Copilot Studio** to make it available for use.
   - This will deploy the agent and make it operational in the chosen environment (e.g., **Microsoft Teams**, **Web Chat**).

---

## Example: Creating the Support Monkey Agent

1. **Agent Name**: **Support Monkey AI Chatbot**
2. **Description**: “An AI-powered assistant that assists support agents by retrieving client details, managing support tickets, and providing troubleshooting guidance.”
3. **Trigger Example 1**: “What are the client details for OMK?”
4. **Trigger Example 2**: “Fetch the latest ticket for Subway Chur”
5. **Actions**:
   - **Client Info**: Retrieves data from **OneDrive**.
   - **Ticket Updates**: Fetches data from **GitHub** issues.
   - **Troubleshooting**: Provides troubleshooting steps from **SharePoint** or other documents.

### Testing Example:
   - Test input: “Show me the client details for OMK.”
   - Expected action: The agent will query **OneDrive** for client details and return the data.

---

## Best Practices for Adding Agents:
- **Use Clear Intent Names**: When defining topics, give each one a clear, concise name (e.g., **Client Info Query**, **Ticket Update**).
- **Modularize Topics**: Keep topics modular by defining specific, limited actions. For example, one topic for fetching **client data** and another for **retrieving ticket updates**.
- **Regular Testing**: Test agent behavior with different user queries to ensure proper functionality before going live.
- **Personalize Responses**: If possible, personalize responses by using variables (e.g., “Hello [UserName], here are the details for OMK”).

---

## Conclusion

Adding an agent in **Copilot Studio** allows you to create an AI-powered assistant to automate tasks and help support teams with faster data retrieval and troubleshooting. By following the steps above, you can create an agent that integrates with various tools like **OneDrive**, **GitHub**, and **Teams**, while defining clear triggers and responses to streamline operations.
