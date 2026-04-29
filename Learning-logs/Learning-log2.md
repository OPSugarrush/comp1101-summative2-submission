## Learning Log – Entry 2: Initial AI Logic Implementation (29/03) 

### What I did 

I moved from research to implementing the core AI logic using Python, which I had limited experience with. I also spent time improving my understanding through a short AI fundamentals course, helping me make more informed decisions.  

I created a standalone module (`ai_logic.py`) that handles the full response pipeline. I structured it into functions: `process_input` to standardise input, `build_prompt` to format it, and `generate_response` to control the flow. Although responses are rule-based, the structure reflects real AI systems.  

I also separated logic from output to improve modularity and designed the code with future expansion in mind, including clear points to add conversation memory later.  

To test it, I built a simple terminal loop to repeatedly input messages and check responses. I also ensured the module can integrate with Jimi’s backend by making `generate_response` usable within an API endpoint.  

### What I learned 

I learned that good AI systems rely on both prompt structure and clear code organisation. Breaking the system into stages made it easier to understand and extend.  

Applying prompt structuring in code helped reinforce my understanding beyond theory. Testing also showed the limits of rule-based responses, highlighting the need for future improvements.  

I also developed practical experience in building a Python-based AI logic pipeline, strengthening my ability to translate system design into working code.  

### Changes to goals 

I originally planned to implement memory at this stage, but realised it was too ambitious. I instead focused on building a clean, modular foundation first.  

### Next steps 

Next, I will integrate the module into Jimi’s FastAPI backend and ensure responses work through an API endpoint. After that, I will implement conversation memory and refine the prompt structure.  
