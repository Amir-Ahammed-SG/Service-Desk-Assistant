
# How to Add Flows in Copilot Studio and Link with Your Support Monkey Agent

## 1. Log into Copilot Studio
   - Open **Copilot Studio** and log in using your credentials.

## 2. Navigate to the "Flows" Section
   - In the **Copilot Studio** interface, locate and open the **Flows** section. This is where you can create and manage the flow of conversations for your chatbot.
   - **Flows** can be used to guide users step-by-step through interactions, gathering information, or providing responses.

## 3. Click "Add New Flow"
   - Look for an option like **"Add New Flow"**, **"Create New Flow"**, or **"Create Flow"** and click on it to start the process of adding a new flow.

## 4. Define the Flow’s Purpose
   - **Flow Name**: Name the flow based on its purpose. For example, **Client Info Flow**, **Ticket Update Flow**, or **Troubleshooting Flow**.
   - **Description**: Provide a brief description of what the flow will accomplish. For example: "This flow helps users retrieve client details and provide troubleshooting steps."

## 5. Design the Flow
   - **Step-by-Step Interaction**: 
     - Use **Copilot Studio’s Flow Builder** to design the conversation steps. Each step can represent a user prompt, a bot response, or an action (like retrieving data).
     - For example, the flow can ask the user for a client name, fetch client details, and return the results.

   - **Variables**: Define variables that will store user input or dynamic data fetched from external sources (e.g., client name, POS details).
     - Example: Create a variable `client_name` to store the name the user provides when asking for client details.

   - **Conditions**: Use conditional logic to handle different branches in the conversation. For example:
     - If the user asks for **client details**, show the **Client Info Flow**.
     - If the user asks for **ticket updates**, show the **Ticket Update Flow**.

   - **Suggested Prompts**: You can add **suggested prompts** (e.g., buttons or quick replies) within the flow to guide the user’s next steps.

   - **External Actions**: Integrate **API calls** or **data retrieval actions** within the flow. For example:
     - Retrieve client details from **OneDrive**.
     - Fetch ticket updates from **GitHub**.

## 6. Link Flow with Your Support Monkey Agent
   - Once you’ve created the flow, link it with the **Support Monkey Agent** by:
     - **Mapping Topics to Flows**: Define which topics (e.g., Client Info Query, Ticket Updates) will trigger specific flows.
     - For instance, if the user asks about **client details**, the flow for **Client Info Retrieval** should be triggered.

   - **Link to Agent**: In the agent configuration, you can specify that the agent should use the newly created flow when specific triggers or topics are matched.

## 7. Test the Flow
   - Use **Copilot Studio’s testing environment** to simulate the user interactions and verify that the flow behaves as expected.
     - Test scenarios like asking for **client details**, **ticket updates**, and running through **troubleshooting steps** to ensure the flow handles all cases correctly.

## 8. Publish the Flow and Agent
   - Once you are satisfied with the flow, **save and publish** it within **Copilot Studio** to make it live.
   - The flow will now be linked to your **Support Monkey Agent** and will be active for users interacting with the agent.

---

## Example of Creating a Client Info Flow

1. **Flow Name**: **Client Info Flow**
2. **Trigger**: When the user asks, "What are the client details for OMK?"
3. **Flow Steps**:
   1. **Step 1**: Ask the user for the **client name** (e.g., “Which client’s details do you need?”).
   2. **Step 2**: Use **Copilot Studio’s dynamic response feature** to retrieve the client’s details from **OneDrive**.
   3. **Step 3**: Display the retrieved client data (e.g., name, contact details).
4. **Variables**: 
   - **client_name**: Stores the name of the client entered by the user.
5. **Action**: Call the **OneDrive API** to fetch client details based on the **client_name**.

## Best Practices for Creating Flows in Copilot Studio

- **Keep Flows Modular**: Break complex workflows into smaller, manageable steps. Each flow should ideally cover a specific use case (e.g., retrieving client details or providing troubleshooting help).
- **Use Conditional Logic**: Handle different user inputs with branching paths based on responses (e.g., "Yes" or "No").
- **Test Thoroughly**: Always test the flow to ensure that it behaves correctly under all possible scenarios.
- **Personalization**: Use user data or contextual variables to personalize the flow (e.g., “Hello, John! Let’s check the client details for you.”).

## Conclusion

By creating and linking **flows** with your **Support Monkey AI Chatbot Agent**, you can build dynamic, multi-step conversations that can handle a variety of user interactions. Flows provide a structured way to guide users through tasks such as retrieving client details, providing ticket updates, or troubleshooting system issues.
