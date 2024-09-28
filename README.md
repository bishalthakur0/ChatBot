This chatbot project is a simple graphical user interface (GUI) application built using Java's `Swing` library. It simulates basic interactions between a user and a chatbot. Here's a breakdown of how it works:

### Key Components:
1. **JFrame (Main Window)**: The application window is created using the `JFrame` class. It holds all the elements like text areas, buttons, and labels.
2. **JTextArea (Chat Area)**: This is a non-editable area where the conversation between the user and the chatbot is displayed. The background is black, and the text color is set to green for the user.
3. **JTextField (Input Field)**: This is where the user types their messages.
4. **JButton (Send Button)**: A button labeled "SEND" which, when clicked, processes the user's input and generates a chatbot response.

### Layout:
- The `JTextArea` (chat area) is placed at the top to display the conversation.
- The `JTextField` (input field) is at the bottom where the user types their messages.
- The `JButton` (send button) is next to the input field to trigger the message sending.

### Functionality:
- **Event Handling (ActionListener)**: When the user clicks the "SEND" button, the `ActionListener` checks the source of the action (the button) and processes the user's input text from the `JTextField`.
- The input text is converted to lowercase for easy comparison.
- Based on certain keywords (like "hi," "how are you," "what is your name," etc.), the chatbot replies with predefined responses.
- If none of the keywords match, the chatbot responds with "I can't understand."

### Chatbot Logic:
- **Keywords**: The chatbot checks for specific keywords in the user's input, such as:
  - **"hi"**: The bot replies with "Hi there."
  - **"how are you"**: The bot responds, "I'm Good :). Thank you for asking."
  - **"what is your name"**: The bot says, "I'm Tumhara Chatbot."
  - **"gender"**: The bot responds humorously about being female.
  - **"love you"**: The bot responds playfully with, "I'm Feeling Shy :) Love you too."
  - **"bye"**: The bot says, "Too Soon :( Anyways, STAY HOME STAY SAFE."

- **Default Reply**: If the input does not match any of the predefined keywords, the bot replies with, "I can't understand."

### Interaction Flow:
1. The user types a message in the `JTextField`.
2. Upon clicking the "SEND" button, the chatbot processes the input.
3. The input is displayed in the `JTextArea` with a prefix "You-->".
4. Based on the input, the chatbot provides a relevant response or a default message.
5. The bot's response is displayed in the `JTextArea` with a prefix "ChatBot-->".

### GUI Design:
- The chatbot window is fixed in size (400x400) with a cyan background for the frame.
- The chat area is black with green text to mimic a terminal-style conversation.
- The input field and button are neatly aligned below the chat area.

### Additional Points:
- The `replyMeth` method is used to append the bot's response to the chat area, simplifying the code structure by separating the logic for displaying chatbot messages.
- The chatbot is simple, with fixed responses for specific keywords, and serves as a basic demonstration of how to create a GUI-based chatbot in Java.
