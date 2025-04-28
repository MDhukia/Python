Intelligent Search using LangChain, ChromaDB, OpenAI, and Tavily APIs
This project demonstrates how to build an intelligent search system that decides between querying a vectorstore (internal database) or performing a web search, based on the user question.
It uses LangChain, OpenAI, ChromaDB, and Tavily services.

🚀 Features
Routing: Determines if the question needs web search or internal database search.

Retrieval: Searches internal documents using vectorstore (ChromaDB).

Relevance Grading: Filters retrieved documents based on their relevance to the question.

Question Rewriting: If no relevant documents are found, the system rewrites the question.

Answer Generation: Generates answers using retrieved data.

Hallucination Checking: Ensures that the generated answers are based on real data.

Final Decision: Only outputs answers that are both grounded and solve the original question.

🛠️ Technologies Used
Python 

LangChain

OpenAI API

ChromaDB

Tavily API

LangGraph

📦 Installation
bash
Copy
Edit
pip install langchain langchain-openai langchain-community langchain-chroma tavily-python langgraph
⚙️ How It Works
Routing

If the question is about "Viswanathan" or "chess" ➔ Search in vectorstore.

Otherwise ➔ Perform web search.

Retrieve Documents

If vectorstore is selected, search internal documents.

Grade Documents

Check if retrieved documents are relevant to the user question.

Rewrite Question (if needed)

If no good documents are found, rewrite the question to improve retrieval.

Answer Generation

Use LangChain's RAG to generate an answer.

Hallucination Check

Confirm the answer is based on real documents.

Final Decision

If everything is correct ➔ Output the answer.

Else ➔ Rewrite or retry.

📄 Example Inputs
"Tell me about Viswanathan's achievement in 2003?"

"Tell me about Viswanathan's achievements?"

"Tell me about recent baseball events?"


