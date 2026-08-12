# 🚀 My Info AI

An AI-powered, interactive resume parser and candidate chatbot. This application extracts structured professional data from a PDF resume and deploys an intelligent assistant capable of answering interview and HR questions on behalf of the candidate.

## ✨ Features

* **Intelligent PDF Parsing:** Reads and extracts information based on semantic meaning, not just strict headings.
* **Structured Data Output:** Automatically categorizes experience, skills, education, and projects into a clean JSON format.
* **AI Candidate Representative:** An interactive chat interface where users (like HR or recruiters) can ask contextual questions about the candidate's background.
* **Modern Interface:** A sleek, dark-mode frontend built with Tailwind CSS for a seamless user experience.

## 🛠️ Tech Stack

* **Backend:** Python, FastAPI, Uvicorn, PyPDF, Pydantic
* **AI Engine:** Groq API (`openai/gpt-oss-120b` model)
* **Frontend:** HTML5, Vanilla JavaScript, Tailwind CSS, Axios
* **Environment Management:** `uv` (as per `pyproject.toml` and `uv.lock`)

## 📂 Project Structure

```text
My-Info-AI/
├── backend/
│   ├── main_backend.py      # FastAPI server and AI logic
│   └── [Resume].pdf         # The candidate's resume to be parsed
├── frontend/
│   └── index.html           # UI for data visualization and chat
├── .env                     # API keys and secrets (Git ignored)
├── .gitignore               # Ignored files/folders
├── pyproject.toml           # Project dependencies
├── uv.lock                  # Dependency lockfile
└── README.md                # Project documentation
```

## 🚀 Installation & Setup

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/my-info-ai.git](https://github.com/your-username/my-info-ai.git)
cd my-info-ai
```

### 2. Set Up the Environment
Make sure you have your dependencies installed. Since this project uses `uv`, you can sync your environment:
```bash
uv sync
```

### 3. Configure Environment Variables
Create a `.env` file in the root directory and add your Groq API key:
```env
GROQ_API_KEY=your_groq_api_key_here
```

### 4. Add the Resume
Ensure the resume you want to parse is placed directly inside the `backend/` folder.

## 💻 Running the Application

### Start the Backend Server
Run the FastAPI backend using Uvicorn from the root directory:
```bash
uvicorn backend.main_backend:app --reload
```
The API will be available at `http://127.0.0.1:8000`.

### Open the Frontend
Open `frontend/index.html` in your web browser, or use the **Live Server** extension in VS Code.

## 🕹️ Usage

1. Open the UI in your browser.
2. Click **Parse Resume** in the top right corner.
3. Use the **Chat with Candidate AI** window to ask specific questions about the candidate's skills, work history, or project experience. 

---

## Author Details

**Name:** Raj Fatehveer Singh Brar<br>
**Roll No.:** 102317090<br>
**Email ID:** rbrar_be23@thapar.edu<br>
**University:** Thapar Institute of Engineering and Technology
