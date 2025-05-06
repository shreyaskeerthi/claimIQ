# ClaimIQ: RAG-Based Insurance Assistant

ClaimIQ is a Retrieval-Augmented Generation (RAG) application designed to simulate an AI-powered assistant for insurance-related queries. It helps users explore policy details, understand coverage, and analyze claims data using public, structured datasets.

## 🚀 Features

- 📄 **Semantic Q&A over insurance documents** (e.g. policy coverage, claim steps)
- 🤖 **LLM-based natural language interface**
- 🧠 **Fraud risk classifier** using structured claim data
- 🧮 **Simulated quote estimation tool**
- 🗂️ **Chunked document retrieval with vector search**
- 🖥️ **Streamlit front-end for user interaction**

## 📦 Tech Stack

- **Language Model**: GPT-4 / HuggingFace Transformers
- **RAG Framework**: LangChain or LlamaIndex
- **Embeddings**: Sentence-Transformers (`all-MiniLM-L6-v2`)
- **Vector Store**: FAISS / Chroma
- **Frontend**: Streamlit
- **Backend (optional)**: FastAPI
- **ML Tools**: Scikit-learn, Pandas

## 📚 Datasets Used

| Dataset | Source | Usage |
|--------|--------|--------|
| Allstate Claims Severity | [Kaggle](https://www.kaggle.com/c/allstate-claims-severity) | Claims metadata for loss prediction |
| Insurance Fraud Detection | [Kaggle](https://www.kaggle.com/datasets) | Fraud classification demo |
| NJ Auto Insurance Guide | [NJ.gov](https://www.state.nj.us/dobi/division_consumers/insurance/autoguide.htm) | RAG document base |
| CMS Medicare Claims | [data.cms.gov](https://data.cms.gov/) | Optional health claims dataset |

## 🛠️ Setup

1. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

2. **Prep Data**
  * Place PDFs or CSVs in the /data directory
  * Use preprocessing scripts to embed and index
    
3. **Run Streamlit app**
 ```bash
   streamlit run app.py
   ```

