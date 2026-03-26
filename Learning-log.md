## Learning Log – Entry 1: Project Planning and Initial Research

### What I did

At the beginning of this project I worked with my group to plan the architecture of our chatbot application and divide the responsibilities between team members. My role in the project is to develop the conversation logic and AI integration for the chatbot system. This involves designing how user messages are converted into prompts for the AI model, how conversation context is managed, and how responses are processed before being returned to the user interface.

To prepare for this role I began researching how AI chat systems structure prompts and manage conversation history. I explored documentation and tutorials related to prompt design and chatbot architectures, focusing on how prompts can be dynamically constructed based on previous messages. I also reviewed examples of AI API requests to understand how backend systems communicate with language models.

### What I learned

From this initial research I learned that prompt structure plays a major role in how effectively a chatbot responds. Many systems use a combination of system instructions, conversation history, and the current user message to construct prompts. I also learned that managing conversation context is important for maintaining coherent interactions across multiple messages.

### Initial goals

At the start of the project, my overall goal is to design and implement a chatbot system that can generate context-aware responses by combining structured prompt engineering with conversation memory.

Specifically, I aim to:

Build a reusable prompt generation system that combines system instructions, user input, and conversation history
Implement a conversation memory module that tracks previous messages and feeds them into the AI model
Integrate this system into the backend so that responses are dynamically generated rather than hardcoded

At this stage, I expect to implement a relatively complete system that maintains multi-turn conversation context and produces consistent, relevant responses.

However, I recognise that this goal may be somewhat ambitious given time constraints and the complexity of managing conversation state effectively. As I progress, I may need to simplify aspects of memory handling or prompt structure while still maintaining a functional and well-designed system.

### Next steps

My next step is to research practical implementations of prompt-building systems and begin designing the Python modules that will manage conversation history and AI requests within the backend.
