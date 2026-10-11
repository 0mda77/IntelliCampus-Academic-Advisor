# 🎓 Academic Assistant (Intelligent Systems Engineering)

**Developed by:** Mohamed Emad Eldin Asaad

**Student ID:** 514

## 📌 About the Project

The Academic Assistant for Helwan National University is a smart chatbot specifically designed to serve students of the Intelligent Systems Engineering program. The system leverages Retrieval-Augmented Generation (RAG) technology to accurately answer student inquiries regarding academic regulations, graduation requirements, and the specific locations of halls and classrooms. The project is fully configured to run on a Google Colab environment, utilizing GPU resources to ensure rapid response times.

## ✨ Key Features

* **Interactive User Interface:** Built using `Streamlit` to provide a seamless and user-friendly chat experience.

* **Personalized Responses:** Includes a sidebar to input the student's name and current academic level, allowing the assistant to tailor its advising precisely to the student's status.

* **Local AI Processing:** Runs the `qwen2.5:7b` language model locally using `Ollama` for fast and private text generation.

* **Advanced RAG System:** Extracts and processes information from syllabus files (PDF) and text files (TXT) to provide reliable answers based on official sources.

* **Hardcoded Knowledge Base:** Integrated with a detailed map of classrooms, labs, and lecture halls in "Engineering Building 1", along with core graduation conditions (e.g., completing 148 credit hours).

* **Arabic Language Support:** Automatically adjusts text direction (RTL/LTR) to perfectly accommodate Arabic queries and responses.

## 🛠️ Tech Stack & Libraries

This project relies on modern AI and web development technologies:

* **LangChain:** For building the RAG pipeline and managing prompts.

* **Ollama:** To host and run the Large Language Model (LLM) locally.

* **FAISS:** Used as a fast vector store for document retrieval.

* **Google Generative AI Embeddings:** To convert text chunks into vector embeddings.

* **Streamlit:** For building the interactive web application.

* **pdfplumber / PyPDF:** For parsing and extracting text from PDF documents.

* **Pyngrok:** To create a secure tunnel and expose the local Streamlit app to the public internet.

## 🚀 How to Run (on Google Colab)

Since the project requires specific environments and GPU computing, it is designed to be executed via a Google Colab notebook. The provided script automates the following steps:

1. **Mount Google Drive:** Sets up directories and saves the downloaded Ollama models directly to Google Drive.

2. **Install Dependencies:** Installs `Ollama`, pulls the `qwen2.5:7b` model, and installs all required Python libraries.

3. **Prepare Files:** Creates the necessary knowledge base files (`general_info.txt`) and writes the main application code to `app.py`.

4. **Launch Application:** Starts the Streamlit server in the background and uses Ngrok to generate a public URL for easy access.

## 💡 Example Questions

* "Where is Lecture Hall 1 or the section classrooms located?"

* "What are the first-level courses and their prerequisites?"

* "What are the graduation requirements for the Intelligent Systems Engineering program?"