## Steps to Add a Topic in Copilot Studio:

1. **Log in to Copilot Studio**:
   - Open **Copilot Studio** and log in with your credentials.

2. **Navigate to Your Project**:
   - After logging in, select the relevant project where you want to add the new topic (e.g., your **Support Monkey AI Chatbot** project).

3. **Open the Topics Section**:
   - In the left sidebar or the main menu, look for a section labeled **Topics**, **Content**, or **Dialog Management**. This is where you can manage all your topics (the conversations, intents, or workflows your chatbot will handle).

4. **Click "Add New Topic" or "Create New"**:
   - You should see a button or option like **Add New Topic**, **Create New**, or **New Topic**. Click it to start creating a new topic for your chatbot.

5. **Define the Topic Name**:
   - You will be prompted to provide a **name** for the topic. The name should be descriptive and clearly indicate the purpose of the topic (e.g., "Client Details Query", "Troubleshooting Nexi Terminal").

6. **Add Triggers or Intents**:
   - A **trigger** is a phrase or keyword that will prompt the chatbot to use this topic. For example:
     - Trigger: "How can I get client details?"
     - Trigger: "What is the POS pin for Subway?"
   - Add a few variations of phrases (intents) users might say to trigger this topic.

7. **Define the Response**:
   - You will then need to define the **response**. This is what the chatbot will say when the topic is triggered. You can use dynamic responses such as pulling data from sources (e.g., retrieving client details from OneDrive).
   - **Example Response**: "The client details for OMK are available in OneDrive. I will retrieve them for you."

8. **Connect with Data Sources** (Optional):
   - If the topic needs to fetch information from external sources (e.g., **GitHub**, **OneDrive**, **Teams**), you will need to integrate the relevant APIs or use the predefined integrations available in **Copilot Studio**.
   - This step may involve configuring the data source within **Copilot Studio**, such as setting up access tokens or connecting with Microsoft Graph API, GitHub API, etc.

9. **Test the Topic**:
   - Once you've created the topic, it's important to test it to ensure it responds correctly to triggers.
   - Use the **test environment** or **chat interface** within **Copilot Studio** to simulate user queries and see how the chatbot responds.

10. **Save & Publish**:
   - Once you're satisfied with the topic's configuration, click on **Save** to store it.
   - If you’re ready to make it live, click **Publish** to deploy the topic in your chatbot’s active environment.

11. **Review & Iterate**:
   - After the topic is live, continue monitoring user interactions through **Copilot Studio’s analytics**.
   - If needed, refine the topic by adjusting triggers, responses, and data retrieval logic.

## Additional Tips:
- **User Intents**: Define various possible intents for a topic to handle different variations of user queries (e.g., "What is the client info?" and "Can you show me OMK details?").
- **Dynamic Responses**: Use **Copilot Studio's dynamic content features** to pull data from external sources in real-time (like pulling client details from OneDrive or fetching ticket updates from GitHub).
- **Use Variables**: If your chatbot will respond with data pulled from a database or file (like OneDrive), you can include placeholders (variables) in the response template, which will be replaced with real data when the user queries the bot.
