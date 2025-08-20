## Prompt Engineering Techniques with LangChain

This project demonstrates various **prompt engineering techniques** using the **LangChain** framework to optimize interactions with language models (e.g., XAI's `grok-3`).

> The xAI APIs are used in the notebook samples - feel free to change this to your preferred API.
> 
> For more information on xAI, visit the [xAI Docs](https://docs.x.ai/docs/overview).

### Techniques and Examples
1. **Zero-Shot Prompting**  
   - Directly ask the model to perform a task without examples.  
   - **Example**: Queries the model to answer "What is the capital of France?" without prior context.  
   - **Use Case**: Quick, general-knowledge queries.

2. **Few-Shot Prompting**  
   - Provide a few examples to guide response format or style.  
   - **Example**: Classifies sentiment (positive, negative, neutral) using sample texts.  
   - **Use Case**: Tasks needing specific formats, like classification or translation.

3. **Chain-of-Thought (CoT) Prompting**  
   - Encourage step-by-step reasoning for complex tasks.  
   - **Example**: Solves "What is 15 × 8?" with detailed reasoning steps.  
   - **Use Case**: Arithmetic, logic, or multi-step problems.

4. **Self-Consistency Prompting**  
   - Generate multiple responses and select the most consistent via majority voting.  
   - **Example**: Solves "What is 15 × 8?" by aggregating five responses using `Counter`.  
   - **Use Case**: Reducing errors in variable outputs like math or ambiguous tasks.

5. **Role-Based Prompting**  
   - Assign a persona (e.g., teacher) to tailor response tone or perspective.  
   - **Example**: Explains photosynthesis as a high school science teacher.  
   - **Use Case**: Responses needing specific expertise or audience-appropriate tone.

6. **Prompt Chaining**  
   - Break tasks into sequential prompts, feeding outputs to subsequent steps.  
   - **Example**: Summarizes a text, then analyzes its sentiment.  
   - **Use Case**: Multi-stage tasks like summarization and analysis.

7. **Instruction-Based Prompting**  
   - Specify explicit instructions for format or constraints.  
   - **Example**: Describes wireless earbuds in three formal bullet points.  
   - **Use Case**: Structured outputs like lists or JSON.

8. **Contextual Prompting**  
   - Include background context to improve response accuracy.  
   - **Example**: Answers the height of the Eiffel Tower using provided context.  
   - **Use Case**: Domain-specific or document-based queries.