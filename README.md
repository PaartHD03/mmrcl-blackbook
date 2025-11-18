# mmrcl-blackbook
Final year black book for MMRCL internship - submitted at DY Patil University (2025)

# 🤖 MMRCL AI Chatbot (LLM-Powered)
This project involves the design, development, and deployment of a sophisticated, AI-powered conversational agent (chatbot) for the **Mumbai Metro Rail Corporation Limited (MMRCL)** website. Leveraging advanced **Large Language Models (LLMs)** and a robust **Django** backend, the chatbot provides real-time, context-aware answers to commuters' queries regarding routes, ticketing, schedules, and general information.

## ✨ Key Features

* **Real-time Information:** Provides instant, accurate information on MMRCL services.
* **LLM Integration:** Utilizes the **Mistral 7B** model for high-quality Natural Language Understanding (NLU) and response generation.
* **Retrieval-Augmented Generation (RAG):** Employs **FAISS** (Facebook AI Similarity Search) and **HuggingFace Embeddings** for efficient semantic search against a curated knowledge base, ensuring grounded and factual responses.
* **Multimodal Support:** Supports query input via **text**, **voice**, and **image**.
* **Multilingual Capability:** Supports interactions in **English**, **Hindi**, and **Marathi** to cater to Mumbai's diverse commuter base.
* **Robust Backend:** Built with **Django** for a secure, scalable, and manageable application environment.
* **Interactive Frontend:** Deployed using **Streamlit** for a rapid and user-friendly interface.

## ⚙️ Technologies Used

| Category | Technology | Purpose |
| :--- | :--- | :--- |
| **Backend Framework** | **Python, Django** | Core web framework, session management, and resource handling. |
| **LLM** | **Mistral 7B** | Conversational AI and text generation. |
| **Vector Database/Search** | **FAISS** | Fast similarity search for RAG implementation. |
| **Embeddings** | **HuggingFace Embeddings** | Generating semantic representations of text. |
| **Frontend/UI** | **Streamlit** | Rapid application deployment and user interface. |
| **Deployment** | Netlify | Containerization and hosting. |

## 🚀 Installation and Setup

### Prerequisites

* Python 3.10+
* pip (Python package installer)
* Virtual environment tool (e.g., `venv` or `conda`)

### Step-by-Step Guide

1.  **Clone the Repository:**
    ```bash
    git clone <Your-Repository-URL>
    cd <project-directory>
    ```

2.  **Create and Activate a Virtual Environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Linux/macOS
    # venv\Scripts\activate   # On Windows
    ```

3.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure Environment Variables:**
    Create a `.env` file in the root directory and add necessary variables (e.g., API keys, database configuration).

5.  **Prepare the Knowledge Base (for RAG):**
    * Place your MMRCL-specific data/documents in the designated knowledge base directory (e.g., `data/`).
    * Run the script to generate and index the vector store:
        ```bash
        python manage.py build_vector_index
        ```

6.  **Run the Django Backend:**
    ```bash
    python manage.py runserver
    ```

7.  **Run the Streamlit Frontend:**
    (If the frontend is separate from Django)
    ```bash
    streamlit run app.py
    ```

## 📝 Project Details

This project was developed as a requirement for the degree of **B.Tech in Computer Science and Business Systems** at the **Ramrao Adik Institute of Technology** (Under the ambit of D. Y. Patil Deemed to be University).

* **Student:** Paarth Parag Doshi (21CE2022)
* **Academic Year:** May 2025
* **Supervisors:** Mr. Chaitanya Jage (Project Co-ordinator), Mr. Sumit Patil (Industry Mentor), Mrs. Bhavana Alte (Supervisor).

## 🤝 Contributing

We welcome contributions! Please feel free to submit issues or pull requests to improve the chatbot's functionality, accuracy, or language support.

## ⚖️ License

This project is licensed under the **Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License** - see the [LICENSE](LICENSE) file for details.
