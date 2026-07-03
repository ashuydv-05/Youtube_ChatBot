# 🤖 YouTube RAG Chatbot

An AI-powered chatbot that allows users to interact with any YouTube video's content by simply providing its **Video ID**. The application fetches the video's transcript, converts it into semantic embeddings, stores them in a FAISS vector database, and answers user questions using **Google Gemini 2.5 Flash** through a Retrieval-Augmented Generation (RAG) pipeline.

---

## ✨ Features

- 🎥 Fetch transcripts directly from any YouTube video using its Video ID
- 📝 Automatically split transcripts into meaningful chunks
- 🧠 Generate semantic embeddings using Hugging Face Sentence Transformers
- ⚡ Store embeddings efficiently in a FAISS Vector Database
- 🔍 Retrieve the most relevant transcript chunks using semantic similarity search
- 🤖 Generate accurate, context-aware answers using Google Gemini 2.5 Flash
- 🔗 Built with LangChain Expression Language (LCEL) for a modular AI pipeline

---

# 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Core Programming Language |
| LangChain | Building the RAG Pipeline |
| Google Gemini 2.5 Flash | Large Language Model |
| Hugging Face Sentence Transformers | Text Embeddings |
| FAISS | Vector Database |
| YouTube Transcript API | Transcript Extraction |
| python-dotenv | Environment Variable Management |
| Jupyter Notebook | Development Environment |

---

# ⚙️ Project Workflow

```text
                     User
                       │
                       ▼
            Enter YouTube Video ID
                       │
                       ▼
        YouTube Transcript API Fetches Transcript
                       │
                       ▼
         Recursive Character Text Splitter
                       │
                       ▼
     Hugging Face Sentence Transformer Embeddings
                       │
                       ▼
             FAISS Vector Database
                       │
                       ▼
              User asks a Question
                       │
                       ▼
       Semantic Search retrieves relevant chunks
                       │
                       ▼
             Prompt Template (LangChain)
                       │
                       ▼
             Google Gemini 2.5 Flash
                       │
                       ▼
             Context-Aware AI Response
```

---

# 📂 Project Structure

```bash
Youtube_ChatBot/
│
├── YT_RAG.ipynb          # Complete RAG Pipeline
├── requirements.txt      # Project Dependencies
├── .env                  # API Keys (Ignored)
├── .gitignore
└── README.md
```

---

# 🚀 Installation

### Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/Youtube_ChatBot.git
```

### Navigate to the project

```bash
cd Youtube_ChatBot
```

### Create a Virtual Environment

```bash
python -m venv venv
```

### Activate Virtual Environment

#### Windows

```bash
venv\Scripts\activate
```

#### macOS/Linux

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file in the project root.

```env
GOOGLE_API_KEY=YOUR_GEMINI_API_KEY
```

---

# ▶️ Run the Project

Open

```
YT_RAG.ipynb
```

Run all notebook cells.

Provide any YouTube Video ID and start asking questions.

Example:

```
Video ID:
AJtDXIazrMo
```

Example Questions

```
Summarize the video.

Who is the speaker?

What are the main topics discussed?

Explain the conclusion.

What technologies are mentioned?
```

---

# 📦 Requirements

```
langchain
langchain-community
langchain-core
langchain-google-genai
langchain-huggingface
google-generativeai
youtube-transcript-api
sentence-transformers
faiss-cpu
python-dotenv
tiktoken
ipykernel
```

---

# 💡 Future Improvements

- Streamlit Web Interface
- Support YouTube URLs directly
- Multi-language Transcript Support
- Chat History
- PDF Export
- Docker Deployment
- Memory Support
- Multiple LLM Support (OpenAI, Claude, Gemini)

---

# 👨‍💻 Author

**Ashu Yadav**

If you found this project helpful, consider giving it a ⭐ on GitHub!
