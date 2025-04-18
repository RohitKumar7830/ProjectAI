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

## 📁 Folder Structure

```plaintext
codemate/
│
├── public/                        # Static assets (e.g., index.html, icons)
│
├── src/
│   ├── main/                      # Electron main process
│   │   ├── electron.ts           # Electron entry point
│   │   └── preload.ts            # Preload script for context bridge
│   │
│   ├── renderer/                 # React frontend (Electron renderer)
│   │   ├── components/           # Reusable UI components
│   │   ├── editor/               # Monaco Editor setup and logic
│   │   ├── pages/                # Top-level UI views
│   │   ├── hooks/                # Custom React hooks
│   │   ├── utils/                # Helpers (tokenizer, file reader, etc.)
│   │   └── App.tsx              # Main React app
│   │
│   └── ollama/                   # Local AI integration
│       ├── promptManager.ts     # Context + prompt injection logic
│       └── ollamaClient.ts      # Interface to local model via HTTP
│
├── scripts/                      # Dev/build/start scripts
│   └── start-dev.sh             # Optional CLI start script
│
├── package.json                  # App dependencies and scripts
├── tsconfig.json                 # TypeScript config
├── electron-builder.json         # Build config for packaging app
└── README.md                     # Project overview
