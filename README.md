# AI-Driven PDF Interaction Platform

This project is a **Streamlit** application that empowers users to have dynamic conversations with multiple PDF documents simultaneously. By leveraging **Google Generative AI (Gemini)**, the system processes uploaded files, generates vector embeddings via **FAISS**, and provides precise, context-aware answers to user inquiries.

---

## Key Functionalities

* **Multi-Document Support:** Seamlessly upload and analyze several PDF files at once.
* **Text Extraction & Processing:** Automated parsing of raw text from document pages.
* **Vector Search Engine:** High-performance similarity searches using **FAISS** embeddings.
* **Contextual Q&A:** Intuitive chat interface to query document data.
* **Advanced LLM Integration:** Powered by **Google Generative AI (Gemini Pro)** for high-quality synthesis.

---

## Getting Started

### System Requirements

* **Python:** Version 3.8 or higher.
* **Google API Key:** Required to access **Google Generative AI** services.
* **Conda:** For isolated environment management.

### Setup Instructions

1.  **Download the Source Code**
    ```bash
    git clone https://github.com/nathania-rachael/Chat-with-Multiple-PDFs.git
    cd chat-with-multiple-pdfs
    ```

2.  **Initialize the Environment**
    ```bash
    conda create --name chatpdf-env python=3.8
    conda activate chatpdf-env
    ```

3.  **Deploy Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure Environment Variables**
    Create a file named `.env` in the root folder and insert your credentials:
    ```text
    GOOGLE_API_KEY=your_google_api_key
    ```

---

## How to Use

1.  **Launch the Interface:** Execute `streamlit run app.py` in your terminal.
2.  **Ingest Documents:** Use the sidebar utility to select and upload your PDF files.
3.  **Interact:** Enter your questions into the chat box to retrieve insights directly from your uploaded content.

---

## Technical Architecture

| Technology | Purpose |
| :--- | :--- |
| **Streamlit** | Powers the front-end web interface and user experience. |
| **Google Generative AI (Gemini Pro)** | The core language model for interpreting and answering queries. |
| **PyPDF2** | Handles the extraction of text data from PDF structures. |
| **FAISS** | Manages vector storage and efficient similarity retrieval. |
| **LangChain** | The orchestration framework connecting the AI models and data pipeline. |

Technology,Purpose
Streamlit,Powers the front-end web interface and user experience.
Google Generative AI (Gemini Pro),The core language model for interpreting and answering queries.
PyPDF2,Handles the extraction of text data from PDF structures.
FAISS,Manages vector storage and efficient similarity retrieval.
LangChain,The orchestration framework connecting the AI models and data pipeline.
