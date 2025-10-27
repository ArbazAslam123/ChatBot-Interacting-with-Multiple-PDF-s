Multiple PDF Chatbot 

Overview 

Multiple PDF Chatbot is an intelligent RAG-based AI assistant built using LangChain, Hugging Face embeddings, and the Groq API. 
It enables users to upload multiple PDF files and ask natural language questions related to their combined content. The chatbot processes all uploaded PDFs, extracts their text, and provides relevant, context-aware answers drawn from across all documents. 

This project demonstrates the power of Retrieval-Augmented Generation (RAG), allowing the model to reason over large documents while maintaining speed and accuracy using Groq’s optimized inference technology. 

 

Tools & Technologies Used 

    LangChain – Framework for building retrieval-based conversational agents 

    Hugging Face Embeddings – To transform document text into numerical vector representations 

    Groq API – For fast and efficient large language model inference 

    Python – Main programming language for development 

    FAISS  – Vector databases for storing and retrieving embeddings 

    Gradio – To build an interactive chatbot interface 

 

How It Works 

    PDF Upload: 
    Users can upload multiple PDF files through the interface. 

    Text Extraction: 
    The system extracts textual data from all uploaded PDFs using LangChain’s document loaders. 

    Embedding Generation: 
    Each chunk of extracted text is converted into numerical embeddings using Hugging Face sentence-transformers. 

    Vector Storage: 
    These embeddings are stored in a vector database (like FAISS or Chroma) for quick retrieval. 

    Question Answering: 
    When a user asks a question, the query is also embedded and compared against the stored document vectors to find relevant context. 

    Answer Generation (via Groq API): 
    The relevant text chunks are passed to a Groq-powered LLM, which generates a natural, contextually accurate response. 

 

Example Use Case 

Suppose a user uploads multiple PDF files such as: 

    A research paper, 

    A financial report, and 

    A technical whitepaper. 

They can then ask questions like: 

“What are the key findings in the research paper?” 
“Summarize the financial performance mentioned in the reports.” 
“Explain the technical methods discussed across the PDFs.” 

The chatbot intelligently searches across all uploaded PDFs and returns coherent, well-structured answers. 


Conclusion 

The Multiple PDF Chatbot combines the strengths of Hugging Face embeddings and the Groq API to deliver a fast, context-aware conversational experience. 
By leveraging LangChain’s modular architecture, it enables efficient document retrieval and interactive AI-based question answering across multiple PDF files — all within a simple and user-friendly interface. 

 
