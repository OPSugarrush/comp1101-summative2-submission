## Learning Log – Entry 4: Conversation Memory Implementation (14/04)

### What I did 

In this stage, I implemented a basic conversation memory system within my AI logic module. I introduced a global `history` list to store recent interactions and limited it to the last 3 messages to keep it lightweight and manageable.  

I updated the `build_prompt` function to include this history, allowing previous messages to be structured alongside the current user input. I also modified `generate_response` so that each interaction updates the memory after a response is produced.  

Alongside this, I worked with Jimi to ensure the system remained fully integrated with the backend. This included confirming correct imports between folders and adding the required `__init__.py` files so Python treats the directories as packages.  

### What I learned 

I developed my understanding of how state can be managed in a Python-based AI system, particularly how conversation history can be stored and reused across interactions.  

I also learned more about integration challenges, especially how file structure and imports affect collaboration between different parts of a system.  

### Changes to goals 

The memory system is now implemented, but it does not yet significantly influence response generation, as responses are still rule-based.  

My next goal is to make responses more dynamic by using this memory more effectively, or by introducing a fallback to a real AI model.  

### Next steps 

Next, I will refine how memory is used within the prompt so it has a clearer impact on responses.  

Following this, I may explore integrating an external AI model as a fallback to move beyond fully hardcoded responses while keeping the current system structure.
