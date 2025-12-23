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

### 9. String Output Parser.ipynb
Learn to parse model outputs into plain strings. Shows how to use StrOutputParser to extract text content from ChatOpenAI responses, chain parsers with model invocations, handle complex response objects, and clean output for downstream processing or display.

### 10. Comma-Separated List Output Parser.ipynb
Demonstrates list parsing from model outputs. This notebook teaches how to use CommaSeparatedListOutputParser to automatically split responses into list items, format instructions for models, parse structured comma-separated data, and work with the parsed list output programmatically.

### 11. Datetime Output Parser.ipynb
Covers specialized parsing for temporal data. Learn to use DatetimeOutputParser for extracting dates and times from model responses, format datetime instructions for prompts, parse natural language dates, and convert model outputs into Python datetime objects for calculations and comparisons.

## 🔗 External Resources

- [LangChain Documentation](https://python.langchain.com/)
- [LangGraph Documentation](https://langchain-ai.github.io/langgraph/)
- [OpenAI API Documentation](https://platform.openai.com/docs)

## 📝 Notes

- Ensure you have a valid OpenAI API key before running the notebooks
- Use a virtual environment to avoid dependency conflicts
- Some notebooks may consume OpenAI API credits

## 📄 License

This project is provided as educational material.

---

**Author:** Júlio César  
**Last updated:** December 2025
