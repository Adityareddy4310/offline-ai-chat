# 📌 offline-ai-chat

A fully offline, self-hosted AI chat system using **Ollama**, **Open WebUI**, and **Llama 3.1**.  
This project demonstrates how to run a modern LLM completely **locally**, without any cloud or API dependencies — ideal for secure or offline environments.

---

## 🎥 Demo Video

Since GitHub does not support playing MP4 directly inside a README,  
click the image below to watch the full demo:

[![Demo Video](thumbnail.png)](https://raw.githubusercontent.com/Adityareddy4310/offline-ai-chat/main/demo%20video.mp4)

> 🔹 Replace `thumbnail.png` with any screenshot from your demo video.  
> Upload a PNG/JPG image and rename it to **thumbnail.png**.

---

## 🚀 Overview

**offline-ai-chat** allows you to run Llama models completely offline:

- No API keys  
- No cloud  
- No data leaving your machine  
- Fast, private inference  
- Clean web UI via Open WebUI  

---

## ✨ Features

- 🧠 Run Llama 3.1 fully offline  
- 🌐 Chat UI with Open WebUI  
- 🔒 Privacy-first (no internet required)  
- ⚡ Fast inference via Ollama backend  
- 🖥️ Works on Windows / Linux / macOS  
- 🔌 Simple setup, easy to extend  

---

## 🧱 Tech Stack

| Tool | Purpose |
|------|---------|
| **Ollama** | Local model runtime |
| **Open WebUI** | Browser-based chat interface |
| **Docker** | Containerized deployment |
| **Llama 3.1 (8B)** | Main model used |

---

## 🛠 Installation & Setup

### 1️⃣ Install Ollama  
Download Ollama from: https://ollama.com/download

### 2️⃣ Pull the model  
```bash
ollama pull llama3.1
3️⃣ Run Open WebUI
bash
Copy code
docker run -d \
  -p 3000:8080 \
  -v open-webui:/app \
  --name open-webui \
  ghcr.io/open-webui/open-webui:main
4️⃣ Open the UI
Visit:

arduino
Copy code
http://localhost:3000
📂 Project Structure
bash
Copy code
offline-ai-chat/
├── demo video.mp4    # Demo video
├── thumbnail.png      # Thumbnail image used in README
├── README.md
🤖 How It Works
Ollama hosts the model locally

Open WebUI connects to Ollama

You chat through the browser

All processing happens on your device

📌 Use Cases
Private AI assistant

Offline labs

Secure enterprise setups

Machine learning practice

Research experiments

🤝 Contributing
Pull requests are welcome!
Feel free to improve documentation, add features, or optimize the setup.
