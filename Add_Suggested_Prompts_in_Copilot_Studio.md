
# Guide to Add Suggested Prompts in Copilot Studio

## Steps to Add Suggested Prompts in Copilot Studio

1. **Log into Copilot Studio**:
   - Open **Copilot Studio** and log in with your credentials.

2. **Navigate to Topics or Intent Management Section**:
   - In **Copilot Studio**, go to the section where you manage **Topics** or **Intents**. This is where you define what the chatbot should do when it receives a specific input from the user.

3. **Create or Edit a Topic**:
   - Either **create a new topic** or **edit an existing topic** that you want to add suggested prompts to.
   - Click on **Add New Topic** or select an existing topic to edit.

4. **Define Suggested Prompts (Predefined User Choices)**:
   - **Suggested prompts** are typically predefined options that the chatbot can display as buttons or quick replies.
   - You can define these prompts as **buttons**, **cards**, or **quick replies** that the user can choose from during the conversation.
   - For example:
     - “Here are a few things you can do next:”
       - Button 1: “Show OMK client details”
       - Button 2: “View latest ticket”
       - Button 3: “Get troubleshooting guide”

5. **Customize the Appearance of Suggested Prompts**:
   - Customize the appearance of the prompts as **buttons** or **cards** to make them visually appealing. Most chatbot platforms allow you to design how the prompts look to users.
   - You can:
     - Use **buttons** for clickable options.
     - Use **cards** to provide richer content (text, images, and buttons).

6. **Define Actions for Each Prompt**:
   - After defining the prompts, specify what actions the chatbot should take when a user selects one of the options.
     - **Example**: If the user selects “Show OMK client details,” the bot fetches client data from **OneDrive** or the database and displays it.

7. **Test the Suggested Prompts**:
   - After adding the suggested prompts, test them by simulating user input in **Copilot Studio’s test environment**.
   - Ensure that the chatbot is displaying the correct prompts and triggering the right actions based on user selection.

8. **Publish the Changes**:
   - Once you are satisfied with the suggested prompts and have tested them, **save** and **publish** the changes within **Copilot Studio** to make them live for users.

## Example of Suggested Prompts

Let’s say you are adding suggested prompts to a **Client Details Query** topic:

1. **Topic Name**: **Client Details Query**
2. **Triggers**:
   - “Show me the client details for OMK”
3. **Suggested Prompts**:
   - “Here’s what I can do for you with the client data:”
     - **Button 1**: “Show OMK client details”
     - **Button 2**: “View client’s last ticket”
     - **Button 3**: “Get troubleshooting guide”
4. **Response**:
   - After the user selects one of the buttons, the chatbot fetches the relevant data and provides it as a response.

## Best Practices for Suggested Prompts

- **Provide Clear Options**: Make sure the prompts are clear and actionable so users can easily understand and choose what they want.
- **Use Context**: The suggested prompts should be context-aware, offering choices that are relevant to the current conversation or user intent.
- **Keep It Short**: Limit the number of suggestions to 3-4 choices at a time to avoid overwhelming the user.
- **Personalization**: If possible, personalize the prompts based on user behavior or data (e.g., “Hello, John! Would you like to see the latest ticket for Subway?”).

## Conclusion

Adding **suggested prompts** in **Copilot Studio** helps improve the chatbot’s user experience by providing predefined options that guide users through a conversation. It makes interactions smoother and more efficient, especially for repetitive tasks like retrieving client details or ticket updates.
