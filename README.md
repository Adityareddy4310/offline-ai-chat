# offline-ai-chat
Native Windows installation guide for Ollama and Open-WebUI: Offline, lightweight AI chat interface without Docker or WSL
Here is your **complete, polished, professional, engaging, and copy-paste-ready README.md**
— perfect for your GitHub repository **offline-ai-chat**.

Just copy → paste into your `README.md`.

---

# 📌 **offline-ai-chat**

A fully **offline, self-hosted AI chat system** built using **Ollama**, **Open WebUI**, and **Llama 3.1**.
Designed for privacy-focused users, secure workplaces, and environments without internet access — this project demonstrates how to run a modern LLM completely **locally**, with a smooth web interface and no external dependencies.

---

## 🎥 **Project Demo**

```md
<video src="https://raw.githubusercontent.com/Adityareddy4310/offline-ai-chat/main/demo.mp4" controls width="650"></video>
```

---

## 🚀 **Overview**

**offline-ai-chat** gives you a powerful, private AI assistant that runs entirely on your machine:

* No API keys
* No cloud services
* No data leaving your device
* Full control over your models and storage

Using **Ollama** as the backend and **Open WebUI** as the frontend, the system provides an intuitive chat interface powered by the **Llama 3.1** model.

---

## ✨ **Features**

* 🧠 **Offline LLM Execution** using Ollama
* 🌐 **Beautiful Chat UI** powered by Open WebUI
* 🔒 **100% Private & Secure** – works without internet
* ⚡ **Fast Local Inference** on supported hardware
* 🔌 **Easy Setup** with simple commands
* 🖥️ **Cross-Platform**: Windows / Linux / macOS
* 🧩 **Extendable** to other models (Gemma, Mistral, Phi, etc.)

---

## 🧱 **Tech Stack**

| Tool               | Purpose                                |
| ------------------ | -------------------------------------- |
| **Ollama**         | Local backend for running LLMs offline |
| **Open WebUI**     | Browser-based chat interface           |
| **Llama 3.1 (8B)** | The model used for this project        |
| **Docker**         | Runs the Open WebUI container          |
| **Local Machine**  | No external dependencies               |

---

## 🛠️ **Installation & Setup**

### **1️⃣ Install Ollama**

Download and install Ollama:

```sh
https://ollama.com/download
```

---

### **2️⃣ Pull the Llama 3.1 Model**

```sh
ollama pull llama3.1
```

---

### **3️⃣ Run Open WebUI (Docker Recommended)**

```sh
docker run -d \
  -p 3000:8080 \
  -v open-webui:/app \
  --name open-webui \
  ghcr.io/open-webui/open-webui:main
```

---

### **4️⃣ Open the Web Interface**

Visit:

```
http://localhost:3000
```

Select your model → Start chatting offline.

---

## 📂 **Project Structure**

```
offline-ai-chat/
├── demo.mp4        # Project demonstration video
├── README.md       # Project documentation
└── (additional files in future updates)
```

---

## 🤖 **How It Works**

1. **Ollama** hosts the Llama model locally
2. **Open WebUI** connects to Ollama through API
3. You interact with the UI
4. All responses are generated on your machine
5. No data is sent to external servers

You get complete privacy + great performance.

---

## 📌 **Use Cases**

* Offline AI development
* Secure enterprise environments
* Personal AI assistant
* Research projects
* Learning how LLMs work behind the scenes

---

## 🚧 **Planned Improvements**

* Add support for multiple models
* Provide a setup script for automation
* Include screenshots section
* Add custom tools/extensions for Open WebUI

---

## 🤝 **Contributing**

Contributions are always welcome 😊
If you’d like to improve the documentation, add features, or optimize performance — feel free to open an issue or pull request.

---


