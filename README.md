# Dictate — Remote Mic Voice Dictation

**Use your laptop's microphone to type on any Mac on your network. No cloud, no subscriptions, all local.**

---

## The Problem

Mac Studios and Mac Minis don't have built-in microphones. If you work on one, you can't dictate notes, fill in search bars, or use voice typing anywhere. Dictate fixes that by borrowing the mic from any nearby laptop over WiFi.

## How It Works

```
[Your Laptop] → open a browser page → tap the mic → speak
       ↓
[Mac Studio]  → Whisper AI transcribes → auto-pastes into your active app
```

1. Run the server on the Mac you want to type on
2. Open the web page from any laptop on the same network
3. Tap the mic button, speak, tap again — text appears wherever your cursor is

## What You Get

- **Works on any laptop** — Mac, Windows, Linux. If it has a browser and a mic, it works
- **No cloud** — Whisper AI runs locally on your machine. Nothing leaves your network
- **Zero setup for clients** — no app install, no permissions. Just a browser tab
- **Auto-paste** — transcribed text is automatically Cmd+V'd into your active app
- **Self-contained** — one Python script starts the server. That's it.

## Who It's For

- **Remote workers** on Mac Studios or Minis who need voice dictation
- **DITs and editors** who want to dictate notes while keeping hands on the keyboard
- **Anyone** who prefers speaking to typing on a headless Mac

## Quick Start

```bash
# On the Mac you want to type on:
pip install -r requirements.txt
python server/listen.py

# From any other computer on the same network:
# Open https://<mac-studio-ip>:8765 in a browser
```

The server generates its own SSL certificate so browser mic access works over the network.

## License

All Rights Reserved — commercial software.

**Purchase a license: ryanwuckert@gmail.com**

---

*Built by Movie Color — AI workflow consulting and custom tooling for film and production.*
