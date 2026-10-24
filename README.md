# 🤖 AI Study Buddy

**An AI-powered learning assistant built with Streamlit and Google Gemini to make learning simpler, smarter, and more interactive.**

AI Study Buddy helps students understand complex concepts through AI-generated explanations, interactive question answering, and revision support. With a simple chat-based interface and a modular Python architecture, it provides an accessible learning experience tailored to students' questions.

## ✨ Features

- 🧠 **AI-Powered Explanations** — Understand complex topics through clear, student-friendly explanations.
- 💬 **Interactive Q&A** — Ask questions and receive AI-generated answers in a conversational interface.
- 📚 **Concept Breakdown** — Explore difficult topics step by step.
- 🔄 **Revision Support** — Revisit concepts and reinforce your understanding.
- 🎨 **Simple User Interface** — Interact with the assistant through a clean Streamlit interface.
- 🔗 **Google Gemini Integration** — Generate responses using Google's Gemini API.
- 🧩 **Modular Architecture** — Separate UI components, core logic, and API utilities for easier maintenance.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core application logic |
| Streamlit | Interactive web interface |
| Google Gemini API | AI-powered responses and explanations |
| python-dotenv | Environment variable management, if used |

## 📂 Project Structure

```text
AI_STUDY-BUDDY/
│
├── main.py                  # Streamlit application entry point
├── components/
│   └── chat_ui.py           # Chat interface components
├── core/
│   └── explainer.py         # Concept explanation logic
├── utils/
│   └── gemini_helper.py     # Gemini API integration
├── requirements.txt         # Python dependencies
├── .env                     # Local environment variables (not committed)
├── .gitignore               # Files excluded from version control
└── README.md                # Project documentation
```

## ⚙️ Installation and Setup

### Prerequisites

- Python 3.10 or a compatible version supported by your dependencies
- pip package manager
- A Google Gemini API key

### 1. Clone the repository

```bash
git clone https://github.com/Aayush-Rasaily/AI_STUDY-BUDDY.git
cd AI_STUDY-BUDDY
```

### 2. Create a virtual environment (recommended)

**Windows:**

```bash
python -m venv .venv
.venv\Scripts\activate
```

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Configure your Gemini API key

Create a `.env` file in the project's root directory:

```env
GEMINI_API_KEY=your_api_key_here
```

Replace `your_api_key_here` with your actual API key. Obtain a key through [Google AI Studio](https://aistudio.google.com/).

**Important:** Never commit your API key to GitHub. Add `.env` to your `.gitignore` file and use environment variables or your deployment platform's secrets manager to store credentials securely.

Ensure your Gemini integration reads the `GEMINI_API_KEY` environment variable and that your installed SDK supports the Gemini model configured in your application.

### 5. Run the application

```bash
streamlit run main.py
```

Streamlit will display a local URL in the terminal, usually:

```text
http://localhost:8501
```

Open the URL in your browser to start using AI Study Buddy.

## 🚀 Deployment

You can deploy AI Study Buddy using a supported hosting platform, such as:

- **[Streamlit Community Cloud](https://streamlit.io/cloud)** — A convenient option for Streamlit applications.
- **[Hugging Face Spaces](https://huggingface.co/spaces)** — Host the application using an appropriate Streamlit-compatible setup.
- **[Render](https://render.com/)** — Deploy with a suitable Python environment and start command.

### Deployment checklist

1. Push your project code to GitHub.
2. Configure the required Python dependencies.
3. Add `GEMINI_API_KEY` to the platform's secrets or environment-variable settings.
4. Set the application start command to `streamlit run main.py` where applicable.
5. Deploy and verify that the application can communicate with the Gemini API.

Never include API credentials directly in source code or public repository files.

## 🏗️ Architecture

AI Study Buddy follows a modular architecture to keep the application organized and maintainable.

- **Presentation Layer (`components/`)** — Handles chat interface components.
- **Core Logic Layer (`core/`)** — Manages concept explanation and learning-related processing.
- **Integration Layer (`utils/`)** — Handles communication with the Google Gemini API.
- **Application Entry Point (`main.py`)** — Connects the components and runs the Streamlit application.

This separation makes the project easier to understand, debug, test, and extend.

## 🔮 Future Enhancements

Potential improvements include:

- 📝 Automatic quiz and practice-question generation
- 📄 PDF and document-based question answering
- 🗂️ Personalized study notes and summaries
- 🎯 Topic-based learning plans
- 📈 Learning progress tracking
- 🧠 Flashcards and spaced-repetition revision
- 🌐 Support for additional languages

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Implement and test your changes.
4. Commit your changes with a descriptive message.
5. Open a pull request describing your contribution.

## 🔐 Security

- Keep API keys and other credentials private.
- Use environment variables or deployment secrets.
- Avoid committing `.env`, virtual environments, or generated files.
- Handle API errors and rate limits gracefully.

## 📜 License

This project is open-source and intended for educational use. A specific license has not been identified in this README. Consider adding a `LICENSE` file, such as the MIT License, if you intend to distribute the project under those terms.

## 👨‍💻 Author

**Aayush Rasaily**

GitHub: [@Aayush-Rasaily](https://github.com/Aayush-Rasaily)

## ⭐ Support

If you find AI Study Buddy useful:

- ⭐ Star the repository.
- 🍴 Fork it and experiment with new features.
- 🐛 Report issues or suggest improvements.
- 🤝 Contribute to making learning more accessible.

---

*Making learning simpler, one question at a time. 📚🤖*
