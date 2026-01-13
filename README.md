A Retrieval-Augmented Generation (RAG) based application that allows users to upload a PDF and ask questions, receiving accurate answers grounded in the document.

This project combines LangChain, ChromaDB, Groq LLM, and Streamlit to create a lightweight yet powerful Question-Answering system.

🚀 Features

✅ Upload any PDF document
✅ Automatic text extraction, chunking & embedding
✅ Vector database powered retrieval using ChromaDB
✅ Precise answer generation using Groq LLM models
✅ Clean & interactive Streamlit UI
✅ Reduces hallucinations by retrieving exact context from documents
rag_doc_assistant/
│
├── app.py                  # Main Streamlit application
├── requirements.txt        # Dependencies
├── README.md               # Documentation
├── .gitignore              # Ignore vector DB cache
└── data/
    └── sample_docs

requirment


cd rag_doc_assistant
pip install -r requirements.txt
set GROQ_API_KEY=your_key_here
streamlit run app.py


    💡 How It Works

User uploads a PDF

PDF is split into text chunks

Text chunks are embedded into vectors

ChromaDB stores and retrieves most relevant chunks

Groq LLM generates answers grounded in retrieved info

User sees responses instantly
