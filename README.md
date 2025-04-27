# Local Chatbot with Retrieval-Augmented Generation (RAG)

**Private, Local AI Chatbot for Document-Based Question Answering**

---

## 🧠 Project Overview

This project implements a local Retrieval-Augmented Generation (RAG) chatbot, enabling users to interact with their documents through natural language queries. By leveraging local Large Language Models (LLMs) and vector databases, the chatbot ensures data privacy and efficient information retrieval without relying on external APIs. ([Local RAG Chat with Documents | Enrico Nello](https://enricollen.github.io/posts/Local-RAG-Chatbot/?utm_source=chatgpt.com), [grasool/Local-RAG-Chatbot - GitHub](https://github.com/grasool/Local-RAG-Chatbot?utm_source=chatgpt.com))

---

## ⚙️ Features

- **Local Deployment**: Runs entirely on your machine, ensuring complete data privacy.
- **Document Ingestion**: Processes various document formats, converting them into searchable embeddings.
- **Vector Database Integration**: Utilizes Chroma for efficient storage and retrieval of document embeddings.
- **Flexible LLM Support**: Compatible with models from LM Studio, allowing easy switching between different LLMs.
- **Interactive Q&A**: Engage in conversational queries, receiving contextually relevant answers based on your documents. ([Local RAG Chat with Documents | Enrico Nello](https://enricollen.github.io/posts/Local-RAG-Chatbot/?utm_source=chatgpt.com), [grasool/Local-RAG-Chatbot - GitHub](https://github.com/grasool/Local-RAG-Chatbot?utm_source=chatgpt.com))

---

## 🛠️ Technologies Used

- **Python 3.10+**
- **LangChain**: Framework for building applications with LLMs.
- **Chroma**: Open-source vector database for storing embeddings.
- **LM Studio**: Interface for running local LLMs.
- **Sentence-Transformers**: For generating embeddings from text. ([SuperEasy 100% Local RAG with Ollama + Email RAG - GitHub](https://github.com/AllAboutAI-YT/easy-local-rag?utm_source=chatgpt.com), [Local RAG Chat with Documents | Enrico Nello](https://enricollen.github.io/posts/Local-RAG-Chatbot/?utm_source=chatgpt.com), [curiousily/ragbase: Completely local RAG. Chat with your ... - GitHub](https://github.com/curiousily/ragbase?utm_source=chatgpt.com))

---

## 🚀 Getting Started

### Prerequisites

- Install [Miniconda](https://docs.anaconda.com/free/miniconda/index.html)
- Install [LM Studio](https://lmstudio.ai/) ([grasool/Local-RAG-Chatbot - GitHub](https://github.com/grasool/Local-RAG-Chatbot?utm_source=chatgpt.com))

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

4. **Set Up LM Studio**:
   - Launch LM Studio.
   - Download and load your preferred LLM (e.g., Mistral 7B, LLaMA 2).
   - Start the LM Studio server with default settings. ([grasool/Local-RAG-Chatbot - GitHub](https://github.com/grasool/Local-RAG-Chatbot?utm_source=chatgpt.com))

5. **Prepare Your Documents**:
   - Place your PDF files in a designated directory.
   - Run the following script to create the vector database:
     ```bash
     python vector-db-create.py
     ```

6. **Run the Chatbot**:
   ```bash
   python RAG-chatbot.py
   ```

---

## 📁 Project Structure

- **`RAG-chatbot.py`**: Main script to initiate the chatbot interface.
- **`qa-only.py`**: Script for testing question-answering functionalities.
- **`vector-db-create.py`**: Processes documents and creates the vector database.
- **`requirements.txt`**: List of Python dependencies. ([Local RAG Chat with Documents | Enrico Nello](https://enricollen.github.io/posts/Local-RAG-Chatbot/?utm_source=chatgpt.com), [grasool/Local-RAG-Chatbot - GitHub](https://github.com/grasool/Local-RAG-Chatbot?utm_source=chatgpt.com), [Retrieval-Augmented Generation (RAG) Chatbots: The Future of Customer ...](https://yourgpt.ai/blog/general/retrieval-augmented-generation-rag-chatbots-the-future-of-customer-support-solutions-with-yourgpt-chatbot?utm_source=chatgpt.com))

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
