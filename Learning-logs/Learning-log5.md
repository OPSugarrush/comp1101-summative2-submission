# Learning Log – Entry 5: Prompt Evaluation and AI Integration (22/04)

## What I did  

I introduced a Gemini AI fallback within `generate_response`, allowing the system to produce dynamic responses when no rule matches. This created a hybrid system combining rule-based logic with AI-generated output, without altering the existing structure.  

To support this, I implemented `.env` usage to securely store the API key, using `load_dotenv()` and environment variables.  

I also worked with Jimi and Joshua to ensure the full system operated correctly end-to-end, confirming that the backend API, AI logic, and frontend requests all worked together consistently.  

## What I learned  

I learned how hybrid chatbot systems function in practice, combining rule-based responses with external AI models. Integrating the Gemini API helped me understand how real AI services are used within applications, including how prompts are passed to a model and how responses are returned.  

Additionally, I gained experience using `.env` files to manage API keys securely. This is an important development practice, as it separates configuration data from code and prevents sensitive information from being exposed.  


## Changes to goals  

My initial goal was to design a chatbot that generates context-aware responses using structured prompts and conversation memory. While this remains the overall aim, I realised that fully dynamic responses depend on integrating external AI models rather than relying solely on internal Python logic.  

As a result, my focus shifted towards building a well-structured AI system that accurately represents how real chatbot pipelines operate. This includes clear input processing, prompt construction, memory handling, and backend integration. The addition of the Gemini AI fallback allows the system to begin producing dynamic responses while still maintaining the structured design I developed.  


## Final reflection  

The system is now complete and functioning as intended. 

While I originally aimed for conversation memory to have a stronger influence on responses, the current implementation is sufficient and demonstrates the intended design clearly.
