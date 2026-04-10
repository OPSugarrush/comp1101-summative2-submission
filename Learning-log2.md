## Learning Log – Entry 2: Initial AI Logic Implementation (29/03)

### What I did

During this stage I moved from research into implementing the core AI logic for the chatbot using Python. Between this and my previous entry, I spent additional time strengthening my understanding of Python in AI contexts by completing a short course focused on AI fundamentals. This helped ensure that my implementation decisions were more informed rather than rushed.

I then created a standalone module (`ai_logic.py`) that handles the full response pipeline.

I structured the system into separate functions: `process_input` to standardise user input, `build_prompt` to format the input, and `generate_response` to coordinate the flow and return a response. Although the responses are currently rule-based, the structure reflects how real AI systems process prompts.

I also added a `format_response` function to separate logic from output, improving modularity. The code was intentionally designed with future expansion in mind, including clear points where features such as conversation memory can be introduced in later stages.

To test the system, I implemented a terminal-based loop which allowed me to repeatedly input messages and observe responses. This helped verify that each part of the pipeline was functioning correctly.

I also ensured that the `generate_response` function can be easily integrated into the backend being developed by Jimi, allowing it to be imported and used directly within an API endpoint.


### What I learned

I learned that effective AI systems rely not only on prompt structure but also on clear separation of responsibilities within the code. Breaking the system into stages made it easier to understand, test, and extend.

I also developed my understanding of prompt structuring by applying it in code rather than just researching it. This showed me how even simple structural decisions can influence how a chatbot behaves.

Testing the system locally highlighted limitations in the current rule-based responses and reinforced the importance of designing the system in a way that supports future improvements.


### Changes to goals

My initial goal was to build both prompt structuring and conversation memory early on. However, I realised this was slightly too ambitious for this stage. I adjusted my approach to prioritise building a clean, modular foundation before introducing more advanced features.

This refinement does not change my overall goal of developing a structured and reusable AI logic system, but it changes the order of implementation, focusing on incremental and testable progress.


### Next steps

Next, I will work with Jimi to integrate this module into the FastAPI backend. This will involve ensuring that responses are correctly returned through an API endpoint.

After integration, I plan to implement a basic conversation memory system and refine the prompt structure to improve response quality and consistency across interactions.
