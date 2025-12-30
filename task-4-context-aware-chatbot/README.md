# Task 4: Context-Aware Chatbot (RAG)

## Objective
Build a context-aware chatbot that answers user queries based on external documents using a Retrieval-Augmented Generation (RAG) approach.

---

## Methodology
1. Load textual documents as a knowledge base
2. Split documents into manageable chunks
3. Convert text chunks into vector embeddings
4. Store embeddings in a FAISS vector database
5. Retrieve relevant context for each user query
6. Generate answers grounded in retrieved context

---

## Technologies Used
- LangChain
- FAISS
- Sentence-Transformers
- HuggingFace Embeddings
- Python

---

## Example Query
**Question:** What is a context-aware chatbot?

**Answer:**  
A context-aware chatbot uses external documents as a knowledge source and retrieves
relevant information before answering. This approach, known as Retrieval-Augmented
Generation (RAG), reduces hallucinations and ensures responses are grounded in real data.

---

## Conclusion
This project demonstrates how Retrieval-Augmented Generation can be used to build
reliable and context-aware chatbots. Such systems are widely used in enterprise
search, documentation assistants, and AI-powered customer support.
