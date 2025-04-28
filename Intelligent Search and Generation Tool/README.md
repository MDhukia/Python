#Intelligent Search using LangChain, ChromaDB, OpenAI, and Tavily APIs
##**Overview**
This project demonstrates how to build an intelligent search system that decides between querying a vectorstore (internal database) or performing a web search, based on the user question.

It uses LangChain, OpenAI, ChromaDB, and Tavily services.

#**Features**
Routing: Determines if the question needs web search or internal database search.

Retrieval: Searches internal documents using vectorstore (ChromaDB).

Relevance Grading: Filters retrieved documents based on their relevance to the question.

Question Rewriting: If no relevant documents are found, the system rewrites the question.

Answer Generation: Generates answers using retrieved data.

Hallucination Checking: Ensures that the generated answers are based on real data.

Final Decision: Only outputs answers that are both grounded and solve the original question.

#**Technologies Used**
Python

LangChain

OpenAI API

ChromaDB

Tavily API

LangGraph

#**Installation**

pip install langchain langchain-openai langchain-community langchain-chroma tavily-python langgraph

#**How It Works**
Routing
If the question is about "Viswanathan" or "chess", it searches the vectorstore. Otherwise, it performs a web search.

Retrieve Documents
If vectorstore is selected, it searches internal documents.

Grade Documents
Checks if retrieved documents are relevant to the user question.

Rewrite Question (if needed)
If no good documents are found, the system rewrites the question to improve retrieval.

Answer Generation
Uses LangChain's RAG to generate an answer.

Hallucination Check
Confirms the answer is based on real documents.

Final Decision
If everything is correct, outputs the answer. Otherwise, it rewrites the question or retries.

#**Example Inputs**
"Tell me about Viswanathan's achievement in 2003?"

"Tell me about Viswanathan's achievements?"

"Tell me about recent baseball events?"
