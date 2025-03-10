# LLM_Chatbot

An LLM RAG Chatbot With LangChain and Neo4j

# [reference](https://realpython.com/build-llm-rag-chatbot-with-langchain/#demo-an-llm-rag-chatbot-with-langchain-and-neo4j)

## DAY01-LangChain

### 1. ChatModel

- HumanMessage: A message from the user interacting with the language model.
- AIMessage: A message from the language model.
- SystemMessage: A message that tells the language model how to behave. Not all providers support the SystemMessage.

### 2. Prompt Templates

you can think of prompt templates as predefined recipes for generating prompts for language models.

### 3. Chains and LangChain Expression Language

In general, the LCEL allows you to create arbitrary-length chains with the pipe symbol (|).
``
review_chain = review_prompt_template | chat_model | output_parser
``

### 4. RAG retriever

you can pass the content to the chart_model. but it can not be scale well. To overcome this,
you need a retriever, The process of retrieving The process of retrieving relevant documents and passing them to
a language model to answer questions is known as retrieval-augmented generation (RAG).

### 5. Agents

An agent is a language model that decides on a sequence of actions to execute. Unlike chains where the sequence of actions is hard-coded, agents use a language model to determine which actions to take and in which order.
