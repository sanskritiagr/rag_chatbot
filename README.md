RAG Chatbot
===========

A simple Retrieval-Augmented Generation (RAG) based chatbot that answers questions by retrieving information from a set of documents and using a language model to generate human-like responses.

✨ Features
----------

*   **Document-based Question Answering:** Ask questions based on your documents.
    
*   **Vector Store:** Store document embeddings for fast and efficient retrieval.
    
*   **Streamlit Interface:** User-friendly web interface for interaction.
    
*   **Modular Structure:** Easy to extend and customize.
    

🛠️ How It Works
----------------

1.  **Load Documents:**
    
    *   Documents are loaded from the docs folder.
        
2.  **Chunking:**
    
    *   Documents are split into smaller chunks for better embedding and retrieval.
        
3.  **Embedding:**
    
    *   Chunks are converted into embeddings using a model (like OpenAI Embeddings or HuggingFace models).
        
4.  **Store in Vector Database:**
    
    *   Embeddings are stored in a FAISS vector store for similarity search.
        
5.  **RAG Pipeline:**
    
    *   Retrieve relevant chunks based on user query.
        
    *   Generate answer using a language model (LLM).
        

📂 Project Structure
--------------------

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   plaintextCopyEdit├── app.py            # Main Streamlit app  ├── model.py          # Contains core logic for loading, embedding, storing, and retrieving documents  ├── requirements.txt  # Required Python packages  ├── docs/             # Folder containing the documents  └── README.md         # Project documentation   `

🚀 Getting Started
------------------

### 1\. Clone the repository

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   bashCopyEditgit clone https://github.com/sanskritiagr/rag_chatbot.git  cd rag_chatbot   `

### 2\. Install dependencies

Make sure you have Python 3.8+ installed.Then install the required packages:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   bashCopyEditpip install -r requirements.txt   `

### 3\. Run the application

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   bashCopyEditstreamlit run app.py   `

This will start a local Streamlit server. Open the link shown in the terminal to interact with your chatbot!

⚙️ Configuration
----------------

*   Place your documents inside the docs folder.
    
*   Update model and API keys (if needed) inside model.py.
    
*   Customize chunk size, retrieval method, or embedding model as per your needs.
    

📚 Technologies Used
--------------------

*   **Python**
    
*   **Streamlit** – for the web UI
    
*   **FAISS** – for vector storage
    
*   **HuggingFace Transformers / OpenAI Embeddings** – for embedding
    
*   **LangChain** – to streamline the RAG pipeline
    

💡 Future Improvements
----------------------

*   Add authentication for secure access.
    
*   Support for multi-document types (PDF, txt, etc.).
    
*   Option to upload documents directly from the UI.
    
*   Deployment on cloud platforms (like AWS, Azure, or HuggingFace Spaces).
    

🙌 Acknowledgements
-------------------

*   [LangChain](https://github.com/langchain-ai/langchain)
    
*   [FAISS by Facebook AI](https://github.com/facebookresearch/faiss)
    
*   [Streamlit](https://streamlit.io/)
