# 🧠 CodeMate – Offline AI Coding Assistant

**CodeMate** is a blazing-fast, privacy-first, AI-powered coding assistant built for developers who want intelligent help **without sending their code to the cloud**.

> "AI coding help without sending a byte to the cloud."

---

## 🚀 Features

- ✨ Local AI model support via [Ollama](https://ollama.com/)
- 🧠 Context-aware code suggestions and smart rewrites
- 🖥️ Electron-based desktop app with Monaco editor
- 🔒 100% offline — your code never leaves your machine
- 🛠️ Easily extensible architecture for chat, explain, autocomplete

---

## 📦 Tech Stack

| Layer          | Technology                         |
|----------------|-------------------------------------|
| UI             | Electron + React + Tailwind         |
| Code Editor    | Monaco Editor (VS Code core)        |
| AI Engine      | Local model via Ollama (Code LLaMA) |
| Context Engine | Custom prompt + tokenizer           |
| Packaging      | Electron Builder                    |

---

## 🧰 Folder Structure

codemate/ ├── src/ │ ├── main/ # Electron process │ ├── renderer/ # React UI │ └── ollama/ # Local AI client + context manager ├── public/ # Static assets ├── scripts/ # Dev scripts ├── package.json # Dependencies & scripts └── README.md