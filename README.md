# -Fintech-Inclusion-FAQ-Assistant-LLM-based-
💡 Fintech Inclusion FAQ Assistant (LLM-based)
This project builds a large language model (LLM)-driven FAQ assistant for financial inclusion using a CSV of frequently asked questions and answers — without needing a traditional database.

It uses LlamaIndex, Hugging Face LLMs and embeddings to provide semantic search and natural language responses from a static CSV file.

🧰 Features
✅ Uses HuggingFace’s Meta-LLaMA-3-8B-Instruct for generation
✅ Uses BAAI/bge-small-en-v1.5 for semantic embedding
✅ LlamaIndex VectorStoreIndex powers the search
✅ Returns top 5 relevant Q&A pairs for any query
✅ Completely stateless — no database required
✅ Simple CSV-based document ingestion
⚙️ How It Works
Tokenizer and LLM Initialization

Uses Meta-LLaMA-3 with HuggingFace token.

Embedding & Indexing

The CSV is parsed into Document objects and indexed with VectorStoreIndex.

Query Engine

LlamaIndex's query engine ranks similar documents using embedding similarity and returns top 5 matches.

Answering Questions

The top matches are returned in question + answer format.
📈 Potential Extensions
Deploy as a Streamlit or Gradio app

Replace CSV with Google Sheets or Airtable

Add chat history tracking

Integrate with WhatsApp/Telegram bots

📎 References
LlamaIndex

Meta-LLaMA-3

HuggingFace BGE Embeddings
