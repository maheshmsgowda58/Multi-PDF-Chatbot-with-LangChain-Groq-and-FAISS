# Multi-PDF-Chatbot-with-LangChain-Groq-and-FAISS

A Streamlit-based chatbot that allows users to ask questions across multiple PDF documents. Powered by LangChain for document processing, HuggingFace embeddings for semantic search, FAISS for efficient vector storage, and Groq LLMs for high-quality responses.

---

## How to Run?

### STEPS:

Clone the repository

```bash
git clone https://github.com/maheshmsgowda58/Multi-PDF-Chatbot-with-LangChain-Groq-and-FAISS.git
```

### STEP 01 - Create a conda environment after opening the repository

```bash
conda create -n multidocsrag python=3.10 -y
```

```bash
conda activate multidocsrag
```

### STEP 02 - Install the requirements

```bash
pip install -r requirements.txt
```

### STEP 03 - Create a `.env` file in the root directory and add your credentials as follows:

```ini
GROQ_API_KEY="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```

---

### STEP 04 - Process PDFs and store embeddings locally

```bash
# Upload your PDF files and run the Streamlit app to process them
python app.py
```

---

### STEP 05 - Run the application

```bash
streamlit run app.py
```

Open your browser at:

```bash
http://localhost:8501
```

---

## Techstack Used:

- Python
- Streamlit
- LangChain
- Groq LLM
- HuggingFace embeddings
- FAISS (Vector Database)
- PyPDF2

---

## Optional: Dockerize the Application

1. Build Docker image:

```bash
docker build -t multi-pdf-qna-groq-chatbot .
```

2. Run Docker container:

```bash
docker run -p 8501:8501 multi-pdf-qna-groq-chatbot
```

