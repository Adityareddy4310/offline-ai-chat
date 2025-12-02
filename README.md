# 🚀 Offline AI Chat – Your Local ChatGPT Alternative

**Run Llama models 100% offline with a sleek web UI.** No cloud, no Docker bloat, no internet after setup. Perfect for privacy pros, devs, and offline warriors.

## 🎥 Demo Video

[![Watch Demo](https://github.com/Adityareddy4310/offline-ai-chat/raw/main/thumbnail.png)](https://user-images.githubusercontent.com/12345678/98765432/11223344/demo%20video.mp4)

*Watch the full setup & offline chat demo – 100% local!*

> 💡 **Quick Win**: Get chatting in 2 mins. Fork this repo, star it ⭐, and share your custom model tweaks!

---

## ✨ Why This Project Rocks
Tired of Docker eating your RAM or cloud APIs spying on your prompts? This setup delivers **fast, private AI** on any machine. Built on Ollama's rock-solid local inference + Open-WebUI's intuitive chat.

- **🔒 Ultra-Private**: Everything stays on your device – zero data leaks.
- **⚡ Blazing Fast**: Starts in seconds, no VM overhead.
- **🧩 Extensible**: Swap models, add RAG, or integrate tools like LangChain.
- **🌍 Cross-Platform**: Windows/Linux/macOS ready (Windows-native focus).
- **📱 Offline-First**: Pull once, chat forever – even on a plane.

> Inspired by [Ollama](https://ollama.com) and [Open-WebUI](https://openwebui.com). Join the local AI revolution!

---

## 🛠 Quick Start – From Zero to Chat in 2 Mins

### 1. Grab Ollama (The Brain)
Download the native installer:  
[Windows](https://ollama.com/download/windows) | [macOS](https://ollama.com/download/macos) | [Linux](https://ollama.com/download/linux)

### 2. Pull Your First Model (One-Time Magic)
Open terminal/cmd and run:
```bash
ollama pull llama3.1:8b
```
*Test it*: `ollama run llama3.1:8b` → Ask: "What's the meaning of life?" → `/bye` to exit.

### 3. Fire Up the UI (Python Power)
```bash
# Create project space
mkdir offline-ai-chat && cd offline-ai-chat

# Set up venv (isolated & clean)
python -m venv venv
source venv/bin/activate  # Linux/macOS
# or on Windows: venv\Scripts\activate

# Install & launch
pip install --upgrade pip
pip install open-webui
open-webui serve --port 3000
```

Boom! Head to [http://localhost:3000](http://localhost:3000) → Select your model → Chat away!

> ⚠️ **Pro Tip**: For offline model glitches, hit Settings > Connections > Test Ollama link. Fixed in seconds!

### Docker Lovers? (Optional, Low-Overhead)
```bash
docker run -d -p 3000:8080 -v open-webui:/app/backend/data --add-host=host.docker.internal:host-gateway -e WEBUI_AUTH=False ghcr.io/open-webui/open-webui:main
```

---

## 🤖 Model Showdown – Pick Your Power Level

Compare models like a boss. All pull with `ollama pull [name]` – choose based on your hardware!

| Model              | Size   | Speed 🚀 | Smarts 🧠 | Vibe                          | Pull Command                  |
|--------------------|--------|----------|-----------|-------------------------------|-------------------------------|
| **llama3.1:8b**   | 4.9 GB | ⭐⭐⭐⭐  | ⭐⭐⭐⭐⭐ | Balanced chat king            | `ollama pull llama3.1:8b`    |
| **llama3.2:3b**   | 2.0 GB | ⭐⭐⭐⭐⭐| ⭐⭐⭐⭐  | Speedy for low-RAM laptops    | `ollama pull llama3.2:3b`    |
| **mistral:7b**    | 4.1 GB | ⭐⭐⭐⭐  | ⭐⭐⭐⭐⭐ | Creative & witty responses    | `ollama pull mistral:7b`     |
| **phi3:medium**   | 2.3 GB | ⭐⭐⭐⭐⭐| ⭐⭐⭐⭐  | Code/debugging whiz           | `ollama pull phi3:medium`    |

> 🔍 **Try This**: Start with llama3.1:8b, then remix with a custom Modelfile for your style (e.g., "Act like a pirate coder").

---

## 🎮 Hands-On Demos – See It in Action

Beyond the video thumbnail above, here's what you'll build:

- **Basic Chat**: Prompt: "Plan a vegan dinner party for 4 – keep it under $50." → Gets a full menu + shopping list.
- **Reasoning Test**: "Solve: Bat + ball = $1.10, bat $1 more than ball?" → Step-by-step logic (spoiler: $0.05!).
- **Creative Spark**: "Write a haiku about quantum cats." → Poetic AI magic.

Upload your own demo GIFs/PRs to `/demos/` – let's crowdsource epic examples!

---

## 🧑‍💻 Project Structure (Keep It Tidy)
```
offline-ai-chat/
├── demo video.mp4      # Your full setup walkthrough
├── thumbnail.png       # Clickable preview (grab a frame from your vid!)
├── README.md           # This file – your project's front door
├── setup-notes.md      # Custom tweaks & troubleshooting
└── .gitignore          # Ignore venv & temp files
```

> 📂 **Hack It**: Add a `scripts/` folder for auto-launch (e.g., PowerShell one-liner). PRs welcome!

---

## 🚧 Troubleshooting – Common Wins
- **Models Vanish Offline?** Refresh Settings > Ollama > Test Connection. (GitHub issue #1 vibes – fixed!)
- **Slow on CPU?** Drop to 3B model or enable GPU (NVIDIA/AMD auto-detects).
- **Port Clash?** Swap `--port 3000` to 8080.
- **Stuck?** Ping me in Issues or join [Ollama Discord](https://discord.gg/ollama).

---

## 🌟 Join the Fun – Let's Build Together!
- ⭐ **Star** this repo to fuel the local AI fire.
- 🍴 **Fork** & tweak – add voice mode? RAG docs? Your call!
- 💬 **Chat** in Issues/Discussions – share your wildest prompts.
- 🤝 **Contribute**: Docs, models, or UI skins. See [CONTRIBUTING.md](CONTRIBUTING.md) for the lowdown.

> 💭 **What's Next?** Roadmap: Auto-model switching, mobile PWA support. Vote in Issues!

**Made with ❤️ for offline dreamers. License: MIT – Use freely, credit kindly.**

---

[Ollama Docs](https://ollama.com/docs) | [Open-WebUI Guide](https://docs.openwebui.com) | [Your Feedback Here](https://github.com/Adityareddy4310/offline-ai-chat/issues/new)
````

---
