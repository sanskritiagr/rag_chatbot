# RAG Chatbot

A simple Retrieval-Augmented Generation (RAG) based chatbot that answers questions by retrieving information from documents and generating human-like responses.

## Features

- Document-based Question Answering: Ask questions based on your own documents.
- Vector Store: Store document embeddings for efficient retrieval.
- Streamlit Interface: Simple web interface for interaction.
- Modular Structure: Easy to extend and customize.

## How It Works

1. Load documents from the `docs` folder.
2. Split documents into smaller chunks.
3. Embed the chunks using a language model.
4. Store the embeddings in a FAISS vector database.
5. Retrieve relevant chunks based on user queries.
6. Generate answers using a language model.

## Project Structure

```
├── app.py            # Main Streamlit app
├── model.py          # Core logic for loading, embedding, storing, and retrieving documents
├── requirements.txt  # Required Python packages
├── docs/             # Folder containing documents
└── README.md         # Project documentation
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/sanskritiagr/rag_chatbot.git
cd rag_chatbot
```

### 2. Install dependencies

Ensure Python 3.8 or higher is installed.

```bash
pip install -r requirements.txt
```

### 3. Run the application

```bash
streamlit run app.py
```

The Streamlit app will open in your browser.

## Configuration

- Place your documents inside the `docs` folder.
- Update the model or API keys inside `model.py` if necessary.
- Customize the chunk size, retrieval method, or embedding model as needed.

## Technologies Used

- Python
- Streamlit
- FAISS
- HuggingFace Transformers or OpenAI Embeddings
- LangChain

## Future Improvements

- Add user authentication for secure access.
- Deploy to cloud platforms (AWS, Azure, HuggingFace Spaces).
