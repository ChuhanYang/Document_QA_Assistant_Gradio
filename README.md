# 📄 Local Document Q&A Assistant with LLM

This is a lightweight, privacy-first LLM-powered application that allows you to upload a document (PDF, TXT, or DOCX), preview its contents, and ask questions about it — all **fully offline** using open-source tools.

> 💡 Powered by a local language model (`gemm2a:2b` via [Ollama](https://ollama.com)) and fast embeddings (`MiniLM`) — no API keys, no internet required after setup.

---

## ✨ Features

- ✅ Upload documents in **PDF, TXT, or DOCX**
- 🧠 Extract key content and **ask natural language questions**
- 📸 Preview first page of PDF or snippet of text
- 🗂️ Multi-format support (UTF-8 and non-standard encodings)
- 💬 Interactive **chat history**
- 📎 Downloadable Q&A transcript

---

## 🚀 Demo

![Demo Screenshot](https://github.com/ChuhanYang/Document_QA_Assistant_Gradio/blob/756653d4823fd022ae97b8b0dfaa28d2d0afe64e/demo_preview.png)  
> *Chatting with a article and getting an instant summary + Q&A.*

---

## 🛠 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/local-doc-qa.git
cd local-doc-qa
```

### 2. Set up a virtual environment (recommended)

```bash
python -m venv .venv
source .venv/bin/activate  # or .venv\\Scripts\\activate on Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Install and run Ollama

Download [Ollama](https://ollama.com/download), then pull a lightweight local model:

```bash
ollama pull gemma2:2b
```

> ℹ️ You can also use `llama2` or `mistral` if your system has enough RAM (≥7 GB).

---

## ✅ Run the App

```bash
python doc_qa_app.py
```

Then open the local Gradio interface (usually at `http://127.0.0.1:7860`).

---

## 🧪 Requirements

- Python 3.9+
- 4 GB+ RAM (for `gemma:2b`)
- Ollama (local LLM runtime)

---

## 📂 File Structure

```
├── doc_qa_app.py          # Main app
├── requirements.txt       # Python dependencies
├── README.md              # This file
└── demo.png               # (Optional) UI screenshot
```

---

## ⚙️ Powered By

- [Gradio](https://gradio.app) – UI for ML apps
- [LlamaIndex](https://github.com/jerryjliu/llama_index) – Document indexing and vector search
- [Ollama](https://ollama.com) – Local model hosting (Mistral, Llama2, Gemma)
- [MiniLM](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) – Fast sentence embeddings

---

## 🧠 Future Improvements

- 🔄 Support multiple file uploads and cross-doc search
- 🔐 Document redaction (PII filtering)
- 📱 Mobile-friendly interface
- 🌍 Hugging Face or Docker deployment

---

## 🙋‍♂️ Author

**Chuhan Yang**  
Data Scientist · ML Enthusiast · Public Transit Analytics  
[LinkedIn](https://www.linkedin.com/in/chuhan-yang/) • [GitHub](https://github.com/ChuhanYang)


