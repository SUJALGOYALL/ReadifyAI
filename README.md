# 📚 ReadifyAI — Multi-PDF Question Answering App

ReadifyAI is a powerful, intuitive, and fast PDF question-answering app that allows you to **upload multiple PDFs** and **ask intelligent questions** like:
- 🔍 "Give a summary of Chapter 3"
- ❓ "Explain the concept of Quantum Entanglement"
- 📑 "What are the key takeaways from the document?"

It uses **Google's Gemini model** via **LangChain**, **FAISS vector store**, and **Streamlit** to build a conversational interface around your documents.

---

## 🚀 Features

✅ Upload **multiple PDFs**  
✅ Ask **any question** related to the documents  
✅ Get **detailed, accurate answers**  
✅ Works for **summaries, explanations, definitions, and context-based answers**  
✅ Built with **Gemini 1.5 Flash**, **FAISS**, and **LangChain**

---

## 🛠️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/SUJALGOYALL/readifyai.git
cd readifyai
```

2. **Create a virtual environment**
```bash
# If using conda:
conda create -n readify python=3.11
conda activate readify

# OR using venv:
python -m venv venv
venv\Scripts\activate  
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Set up your Google API Key**

Create a `.env` file in the root directory:
```env
GOOGLE_API_KEY=your_google_gemini_api_key_here
```

---

## 📦 Requirements

Here are the Python packages required (also present in `requirements.txt`):

```
streamlit
google-generativeai
python-dotenv
langchain
PyPDF2
faiss-cpu
langchain_google_genai
```

---

## ▶️ Usage

1. Run the app:
```bash
streamlit run app.py
```

2. In the browser:
   - Upload one or more PDF files using the sidebar
   - Click “Submit & Process”
   - Ask any question in the input field
   - View intelligent answers based on the content of your PDFs

---

## 🧠 How It Works

1. **PDF Extraction**: Extracts text from uploaded PDF(s) using `PyPDF2`.
2. **Text Chunking**: Splits the text into manageable chunks with overlap for context.
3. **Embedding**: Generates embeddings using `GoogleGenerativeAIEmbeddings`.
4. **Vector Store**: Stores embeddings in a FAISS index for fast similarity search.
5. **Q&A Chain**: Uses LangChain’s `load_qa_chain` and Gemini-1.5 Flash to generate answers from the retrieved documents.

---

## 📌 Example Use Cases

- Study notes summarizer  
- Research paper Q&A assistant  
- Legal/contract document explainer  
- Book chapter explainer  
- Technical documentation assistant  

---

## 🧾 License

This project is for **educational and research purposes** only.

---

## 🙋‍♂️ Author

**Sujal Goyal**  
Mathematics & Computing, IIIT Bhagalpur


---
