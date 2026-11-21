# 📘 Product Manual AI – Smart Troubleshooting Assistant

An AI-powered Product Manual Assistant that allows users to upload appliance manuals in PDF format and ask questions in natural language. The application uses **Retrieval-Augmented Generation (RAG)** to retrieve relevant information from uploaded documents and generate context-aware answers using Google's Gemini API.

## 🚀 Project Overview

Reading lengthy product manuals to find troubleshooting instructions can be time-consuming. Product Manual AI simplifies this process by allowing users to upload a product manual and ask questions directly.

The system retrieves relevant document content and generates easy-to-understand answers with troubleshooting steps, safety warnings, and source information.

## ✨ Features

- 📄 **PDF Upload:** Upload product manuals in PDF format.
- 🤖 **AI-Powered Q&A:** Ask questions in natural language.
- 🔍 **RAG Pipeline:** Retrieve relevant information from uploaded documents.
- 🧠 **Semantic Search:** Find relevant content using HuggingFace embeddings.
- 💬 **Conversational Interface:** Interact with the uploaded document.
- 🛠️ **Troubleshooting Assistance:** Generate step-by-step instructions based on manual content.
- ⚠️ **Safety Guidance:** Highlight relevant safety precautions.
- 📚 **Context-Based Responses:** Generate answers using retrieved document content.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Programming language |
| Streamlit | Web application interface |
| LangChain | RAG orchestration |
| Google Gemini API | LLM-based answer generation |
| HuggingFace | Text embeddings |
| FAISS | Vector similarity search |
| PyMuPDF / PDF loader | PDF text extraction |

## 🏗️ Project Architecture

```text
User
 |
 v
Streamlit Web Interface
 |
 v
Upload Product Manual (PDF)
 |
 v
PDF Text Extraction
 |
 v
Text Chunking
 |
 v
HuggingFace Embeddings
 |
 v
FAISS Vector Database
 |
 v
User Question
 |
 v
Relevant Context Retrieval
 |
 v
Google Gemini API
 |
 v
AI-Generated Answer
```

## 📂 Project Structure

```text
pdf-chatbot-rag-main/
│
├── app.py
├── src/
│   └── chat.py
├── requirements.txt
├── README.md
├── .gitignore
└── ...
```

*Note: The structure above is illustrative. Refer to the actual repository for the complete project structure.*

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Product-Manual-AI-Roll40.git
```

### 2. Navigate to the project directory

```bash
cd Product-Manual-AI-Roll40
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the virtual environment

**Windows:**

```bash
venv\Scripts\activate
```

### 5. Install dependencies

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

### 6. Configure Gemini API Key

Create a `.env` file in the project root:

```env
GEMINI_API_KEY=your_gemini_api_key
```

Get your API key from:

https://aistudio.google.com/apikey

Never upload your `.env` file or expose your API key publicly.

### 7. Run the application

```bash
streamlit run app.py
```

Open the application at:

```text
http://localhost:8501
```

## 🧪 How to Use

1. Start the Streamlit application.
2. Upload a product manual in PDF format.
3. Wait for the document processing and embedding generation.
4. Enter a question related to the uploaded product
