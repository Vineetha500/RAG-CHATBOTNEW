# Installation
## 1.Install Python 3.11.9

## 2. Create Virtual Environment
### Windows
```bash
python -m venv venv
```

## 3. Activate Virtual Environment
### Windows
```bash
venv\Scripts\activate
```

## 4. Install Dependencies
```bash
pip install -r requirements.txt
```

# Install Ollama
Download and install Ollama:
https://ollama.com/download
After installation, pull TinyLlama model:
```bash
ollama run tinyllama
```

# Run the Application
Start Streamlit app:
```bash
streamlit run app.py
```
The application will open at:
```text
http://localhost:8501
```

# How to Use
1. Launch the application
2. Upload a PDF file
3. Wait for vector database creation
4. Ask questions related to the PDF
5. Get AI-generated answers


# Key Components
## PyPDFLoader
Loads and extracts text from PDF files.

## RecursiveCharacterTextSplitter
Splits large text into smaller chunks.

## HuggingFaceEmbeddings
Converts text chunks into embeddings.

## FAISS
Stores and retrieves vector embeddings efficiently.

## ChatOllama
Runs TinyLlama locally using Ollama.

## ConversationalRetrievalChain
Combines retrieval and conversational AI.

# Troubleshooting
## Ollama Not Found
Install Ollama and restart terminal.
## TinyLlama Model Missing
Run:
```bash
ollama run tinyllama
```
## ModuleNotFoundError
Install missing package:
```bash
pip install <package_name>
```



