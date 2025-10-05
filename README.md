# Automated-WhatsApp-Agent-LifeLift-Coach
A smart Life Coach assistant built with n8n
## Pipeline Workflow

### User Trigger
The chatbot activates automatically when user sends a message to the Whatsapp number and responds with a greeting.

### Input Handling
The system checks whether the incoming message is audio or text.

If the message is audio, it is transcribed to text using Google Gemini.

Both the transcribed text, or the user text message are stored in the same variable for unified processing.

### AI Processing
The query (text input) is passed to the AI Agent “LifeLift Coach”, which uses OpenAI’s GPT 4.1-mini for generating responses.  
It has already been given a system prompt and handles inputs accordingly.

### Memory & Tools
The agent retains a memory of the last 5 user interactions for context-aware responses.

It also has access to a Sheets tool containing Subscription data, which it can reference when needed.

### Response Generation
The agent replies to users in a friendly, motivating, and WhatsApp-style tone based on the conversation rules.

Message ends with a short thank you or positive closing line by use of prompt.


## Demo
https://github.com/user-attachments/assets/d1c8005e-3735-476a-a2ce-50f69a68df73
<img width="1043" height="499" alt="image" src="https://github.com/user-attachments/assets/c1b484da-c874-408d-92fc-1a16915d18d7" />

