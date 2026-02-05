# AI Engineering - LangChain and LangGraph Projects

This repository contains a collection of educational notebooks exploring the fundamental concepts of **LangChain** and **LangGraph** for AI engineering, with a focus on integration with the OpenAI API.

## 📚 Project Contents

### Initial Setup
- **Setting Up the Env 03.ipynb** - Environment configuration, dependency installation, and credential validation

### OpenAI API
- **The OpenAI API 01.ipynb** - Introduction and basic usage of the OpenAI API with LangChain

### AI Messages
- **AI Messages.ipynb** - Exploration of AI message structures
- **System and Human Messages.ipynb** - Differences and usage of system and user messages

### Prompt Templates
- **Prompt Templates and Prompt Values.ipynb** - Fundamental concepts of prompt templates
- **Chat Prompt Templates and Chat Prompt Values.ipynb** - Chat-specific templates
- **Few-Shot Chat Message Prompt Templates.ipynb** - Few-shot examples in chat templates

### Output Parsers
- **String Output Parser.ipynb** - Parsing string-formatted outputs
- **Comma-Separated List Output Parser.ipynb** - Parser for comma-separated lists
- **Datetime Output Parser.ipynb** - Specialized parser for dates and times

### Chat Model
- **ChatOpenAI.ipynb** - Working with the ChatOpenAI model

### Chains and Runnables
- **The Runnable and RunnableSequence Classes.ipynb** - Foundation of LangChain's functional composition model
- **Piping a Prompt Model and an Output Parser.ipynb** - Composing chains using the pipe operator
- **Piping Chains and the RunnablePassthrough Class.ipynb** - Advanced piping patterns with passthrough functionality
- **Streaming.ipynb** - Real-time streaming of responses from chains
- **Batching.ipynb** - Batch processing multiple inputs efficiently

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- OpenAI API key

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd AI-Engineering-LangChain-And-LangGraph-Projects
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install the dependencies:
```bash
pip install -r requirements.txt
```

4. Configure your environment variables in the `.env` file:
```
OPENAI_API_KEY=your_api_key_here
```

### Running the Notebooks

1. Start Jupyter:
```bash
jupyter notebook
```

2. Open `Setting Up the Env 03.ipynb` first to validate the configuration
3. Execute the notebooks in the suggested order for optimal progressive learning

## 📓 Detailed Notebook Descriptions

### 1. Setting Up the Env 03.ipynb
This foundational notebook covers environment configuration essentials. Learn how to load environment variables using the `dotenv` extension, set up your OpenAI API key programmatically, manage OS environment variables, and securely handle credentials for LangChain projects.

### 2. The OpenAI API 01.ipynb
An introduction to using the OpenAI API through LangChain. This notebook demonstrates how to initialize the OpenAI client, create completion requests with the GPT-4 model, configure parameters like temperature and seed for reproducibility, and implement streaming responses for real-time output.

### 3. AI Messages.ipynb
Explores how to work with AI-generated messages in LangChain. Learn to construct HumanMessage and AIMessage objects, build conversation histories, invoke the ChatOpenAI model with message sequences, and understand how context from previous messages influences model responses.

### 4. System and Human Messages.ipynb
Demonstrates the role of system messages in controlling chatbot behavior. This notebook shows how to use SystemMessage to set personality and instructions, combine SystemMessage with HumanMessage for better control over model responses, and achieve consistent behavior patterns like sarcasm or specific tones.

### 5. Prompt Templates and Prompt Values.ipynb
Introduces templating for dynamic prompt construction. Learn to create reusable prompt templates with variable placeholders, invoke templates with different parameter values, understand the PromptTemplate class and its methods, and generate formatted prompts programmatically.

### 6. Chat Prompt Templates and Chat Prompt Values.ipynb
Extends prompt templates specifically for chat-based interactions. Covers SystemMessagePromptTemplate and HumanMessagePromptTemplate creation, ChatPromptTemplate composition, invoking chat templates with variable substitution, and passing formatted chat prompts to the ChatOpenAI model.

### 7. Few-Shot Chat Message Prompt Templates.ipynb
Covers few-shot learning techniques in LangChain. Learn to define example conversations, use FewShotChatMessagePromptTemplate to guide model behavior through examples, compose examples with human and AI messages, and improve response consistency through demonstrated patterns.

### 8. ChatOpenAI.ipynb
A comprehensive guide to the ChatOpenAI wrapper in LangChain. Demonstrates how to instantiate the ChatOpenAI model, configure model parameters (temperature, seed, max_tokens), invoke the model with simple prompts, and access response content for further processing.

### 9. The Runnable and RunnableSequence Classes.ipynb
Introduces the core building blocks of LangChain's compositional system. Learn how Runnable objects enable functional composition, understand RunnableSequence for chaining operations, invoke multiple steps in sequence, and leverage the invoke() and batch() methods for both single and batch processing.

### 10. Piping a Prompt Model and an Output Parser.ipynb
Demonstrates the elegant pipe operator syntax for composing chains. This notebook shows how to use the LCEL (LangChain Expression Language) | operator to connect prompts, models, and parsers, create reusable pipeline components, and simplify chain definitions compared to RunnableSequence.

### 11. Piping Chains and the RunnablePassthrough Class.ipynb
Covers advanced piping patterns and the RunnablePassthrough utility. Learn to use RunnablePassthrough for conditional pipeline logic, compose complex chains with multiple branches, pass through data unchanged in specific pipeline stages, and build sophisticated data processing workflows.

### 12. Streaming.ipynb
Explores real-time streaming capabilities for chain outputs. This notebook demonstrates how to use the stream() method for progressive token-by-token responses, integrate streaming with different components, monitor real-time progress in long-running operations, and optimize user experience with immediate feedback.

### 13. Batching.ipynb
Covers efficient batch processing of multiple inputs. Learn to use the batch() method for parallel processing multiple prompts, optimize throughput for bulk operations, handle batch results efficiently, and compare performance between single, streaming, and batch execution modes.

### 14. String Output Parser.ipynb
Learn to parse model outputs into plain strings. Shows how to use StrOutputParser to extract text content from ChatOpenAI responses, chain parsers with model invocations, handle complex response objects, and clean output for downstream processing or display.

### 15. Comma-Separated List Output Parser.ipynb
Demonstrates list parsing from model outputs. This notebook teaches how to use CommaSeparatedListOutputParser to automatically split responses into list items, format instructions for models, parse structured comma-separated data, and work with the parsed list output programmatically.

### 16. Datetime Output Parser.ipynb
Covers specialized parsing for temporal data. Learn to use DatetimeOutputParser for extracting dates and times from model responses, format datetime instructions for prompts, parse natural language dates, and convert model outputs into Python datetime objects for calculations and comparisons.

## 🔗 External Resources

- [LangChain Documentation](https://python.langchain.com/)
- [LangGraph Documentation](https://langchain-ai.github.io/langgraph/)
- [OpenAI API Documentation](https://platform.openai.com/docs)

## 📝 Notes

- Ensure you have a valid OpenAI API key before running the notebooks
- Use a virtual environment to avoid dependency conflicts
- Some notebooks may consume OpenAI API credits

**Author:** Júlio César
**Last updated:** February 2026
