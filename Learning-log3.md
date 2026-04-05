## Learning Log – Entry 3: Backend Integration and System Structuring (05/04)

### What I did
During this stage I focused on refining my AI logic module so that it could be more effectively integrated into the backend API being developed by Jimi. Rather than adding new features such as conversation memory at this point, I prioritised improving the structure and usability of the existing system.

I updated the code to better reflect how it will function within a larger application. The main change was introducing a clear interface function, `handle_message`, which acts as the entry point between the backend and the AI logic. This function takes user input and returns a structured response in a JSON-friendly format, making it suitable for use within a FastAPI endpoint.

I also improved input handling by adding basic type checking to ensure the system behaves more reliably when receiving unexpected data. The prompt-building function was refined to include a simple system instruction, making the structure more aligned with how real AI prompts are designed.

Although the response system is still rule-based, I ensured that the internal pipeline (processing → prompt building → response generation) is now clearly defined and modular. This makes it easier to extend in later stages without needing to rewrite the system.

I updated the local testing system to use the new `handle_message` function, ensuring that testing reflects how the backend will actually interact with the module.

### What I learned
Through this stage I developed a better understanding of how different parts of a software system connect together, particularly how internal logic must be designed with external use in mind. Designing a clear interface function highlighted the importance of separating internal processing from how data is exposed to other parts of the application.

I also learned that improving structure and reliability is just as important as adding new features. By refining the existing system, I made it more maintainable and easier to integrate, which is essential in a collaborative project.

Additionally, I gained further insight into how prompt structure can be gradually developed. Even though the system is not yet using an external AI model, the way prompts are constructed now better reflects how such integration would work in the future.

### Changes to goals
My original plan was to begin implementing conversation memory at this stage. However, after reviewing the system and considering integration requirements, I decided to focus first on ensuring that the module is cleanly structured and fully compatible with the backend.

This adjustment improves the overall quality of the system and reduces the risk of issues during integration. My goal of implementing conversation memory remains, but it has been moved to the next stage so that it can be built on top of a stable foundation.

### Next steps
Next, I will implement a basic conversation memory system that stores recent messages and incorporates them into the prompt structure. This will allow the chatbot to handle multi-turn interactions more effectively.

Following that, I plan to further refine the prompt construction to include this conversation history, improving the consistency and relevance of responses.
