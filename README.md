# Local Chatbot with Retrieval-Augmented Generation (RAG)

**Private, Local AI Chatbot for Document-Based Question Answering**

---

## 🧠 Project Overview

This project implements a local Retrieval-Augmented Generation (RAG) chatbot, enabling users to interact with their documents through natural language queries. By leveraging local Large Language Models (LLMs) and vector databases, the chatbot ensures data privacy and efficient information retrieval without relying on external APIs.

---

## ⚙️ Features

- **Local Deployment**: Runs entirely on your machine, ensuring complete data privacy.
- **Document Ingestion**: Processes various document formats, converting them into searchable embeddings.
- **Vector Database Integration**: Utilizes Chroma for efficient storage and retrieval of document embeddings.
- **Flexible LLM Support**: Compatible with models from LM Studio, allowing easy switching between different LLMs.
- **Interactive Q&A**: Engage in conversational queries, receiving contextually relevant answers based on your documents.

---

## 🛠️ Technologies Used

- **Python 3.10+**
- **LangChain**: Framework for building applications with LLMs.
- **Chroma**: Open-source vector database for storing embeddings.
- **Sentence-Transformers**: For generating embeddings from text.

---

## 🚀 Getting Started

### Prerequisites

- Install [Miniconda](https://docs.anaconda.com/free/miniconda/index.html)

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ainulyaqinmhd/Local-Chabot-RAG.git
   cd Local-Chabot-RAG
   ```

2. **Create and Activate Conda Environment**:
   ```bash
   conda create --name local-rag-chatbot python=3.10
   conda activate local-rag-chatbot
   ```

3. **Install Required Packages**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Prepare Your Documents**:
   - Place your PDF files in a designated directory.
   - Run the following script to create the vector database:
     ```bash
     python vector-db-create.py
     ```

5. **Run the Chatbot**:
   ```bash
   python RAG-chatbot.py
   ```

---

## 📁 Project Structure

- **`RAG-chatbot.py`**: Main script to initiate the chatbot interface.
- **`qa-only.py`**: Script for testing question-answering functionalities.
- **`vector-db-create.py`**: Processes documents and creates the vector database.
- **`Chatbot_RAG.ipynb`**: Jupyter notebook demonstrating RAG concepts.
- **`requirements.txt`**: List of Python dependencies.

---

## 🔄 Workflow Architecture

The chatbot operates through the following workflow:

1. **Document Loading**: PDF documents are loaded and processed.
2. **Text Splitting**: Documents are split into manageable chunks.
3. **Embedding Generation**: Each chunk is converted into a vector embedding using Sentence-Transformers.
4. **Vector Storage**: Embeddings are stored in Chroma, a vector database.
5. **User Query Processing**: User inputs a question.
6. **Similarity Search**: The system retrieves relevant document chunks from Chroma based on the query.
7. **Response Generation**: The retrieved context is passed to the LLM to generate a response. 

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
