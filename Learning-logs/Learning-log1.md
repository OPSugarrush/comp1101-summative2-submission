## Learning Log – Entry 1: Project Planning and Initial Research 

### What I did 

At the start of the project, I worked with my group to plan the chatbot architecture and divide responsibilities. My role is to develop the conversation logic and AI integration, including how user input is turned into prompts, how context is managed, and how responses are returned to the frontend.  

To prepare, I researched how AI chat systems structure prompts and handle conversation history. I looked at documentation and examples of prompt design and chatbot architecture, focusing on how prompts are built dynamically using previous messages. I also reviewed AI API request examples to understand how backends communicate with language models.  

### What I learned 

I learned that prompt structure is key to how well a chatbot responds. Most systems combine system instructions, conversation history, and the current input.  

I also learned that managing conversation context is important for keeping interactions consistent across multiple messages.  

Alongside this, I began developing my understanding of how these concepts translate into a Python-based AI system, linking theoretical design to practical implementation.  

### Initial goals 

My goal is to design a chatbot that generates context-aware responses using structured prompts and conversation memory, implemented through a modular Python-based AI system.  

Specifically, I aim to:  

- Build a reusable prompt system combining instructions, input, and history  
- Implement a memory module to track previous messages  
- Integrate this into the backend so responses are dynamically generated  

I recognise this may be ambitious, so I may simplify parts of memory or prompt structure while still keeping the system functional and well designed.  

### Next steps 

My next step is to research practical implementations of prompt-building systems and begin designing the Python modules that will manage conversation history and AI requests within the backend.  
