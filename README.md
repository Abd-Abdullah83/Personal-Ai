<div align="center">

# 🤖 Personal AI Assistant — *Aria*

**Voice-powered · Gemini AI · 100% Free · Zero Backend**

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Gemini](https://img.shields.io/badge/Gemini_2.5_Flash-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev/)

> *A sleek, single-file personal assistant that listens to your voice, talks back, browses the web, checks the weather, sets timers, and answers anything — powered by Google Gemini AI.*

---

</div>

## ✨ Features

| Category | Capability |
|----------|-----------|
| 🎤 **Voice Input** | Real-time speech recognition via Web Speech API |
| 🔊 **Voice Output** | Text-to-speech replies using Speech Synthesis |
| 🧠 **AI Chat** | Gemini 2.5 Flash Lite for open-ended questions |
| 🌤️ **Live Weather** | GPS-based weather via Open-Meteo (no API key needed) |
| ⏰ **Timers** | Set countdowns with desktop push notifications |
| 🔗 **App Launcher** | Open YouTube, Maps, WhatsApp, Twitter, Instagram & more |
| 🔍 **Web Search** | Instant Google search from voice or text |
| 📱 **PWA Ready** | Installable on mobile via `manifest.json` |

---

## 🚀 Getting Started

### 1 — Clone or Download

```bash
git clone https://github.com/Abd-Abdullah83/Nova.git
cd Nova
```

Or just download `AI.html` — it's a **single self-contained file**, no npm, no build step.

### 2 — Add Your Gemini API Key

Open `AI.html` and find line ~13:

```javascript
// ── PASTE YOUR GEMINI API KEY HERE ──────────────────────────
const API_KEY = "YOUR_API_KEY_HERE";
```

Get your free key at → **[aistudio.google.com](https://aistudio.google.com/app/apikey)**

### 3 — Open in Browser

```bash
# Just double-click the file, or:
open AI.html
```

> ⚠️ **Use Chrome or Edge** for full voice support. Firefox does not support the Web Speech API.

---

## 🗣️ Sample Commands

```
"What time is it?"              → Shows current date & time
"What's the weather?"           → Live forecast from your location
"Set a 10 minute timer"         → Countdown with push notification
"Search for FAST University"    → Opens Google search
"Open YouTube"                  → Launches YouTube
"Play lo-fi music on YouTube"   → YouTube search for the query
"Open Google Maps"              → Launches Maps
"Navigate to Lahore"            → Directions in Google Maps
"Send WhatsApp message hello"   → Opens WhatsApp with text pre-filled
"Post on Twitter great day"     → Opens Twitter compose with text
"Explain neural networks"       → Gemini AI answers
"Tell me a joke"                → Gemini AI responds conversationally
```

---

## 🏗️ Architecture

```
AI.html  (single file)
│
├── 🎨  CSS          Dark UI — purple/indigo accent, responsive layout
├── 🎤  Speech API   Web Speech Recognition (Chrome/Edge)
├── 🔊  TTS          SpeechSynthesis API (browser native)
│
├── 🧠  Gemini AI    gemini-2.5-flash-lite via REST API
│                    → fallback for all unrecognised commands
│
├── 🌤️  Open-Meteo  Free weather API (no key required)
│                    → uses Geolocation API for coordinates
│
├── ⏰  Timer        setTimeout + Notifications API
│
└── 🔗  Intent URLs  tel:, sms:, wa.me, maps.google.com,
                     twitter.com/intent, youtube.com/results ...
```

---

## 🔒 Privacy & Security

- **No server.** Everything runs in your browser.
- **No data stored.** Conversations are never saved.
- **API key** is client-side — for personal use only. Do not publish your key publicly.
- Weather uses your GPS coordinates, which are sent only to Open-Meteo's public API.

---

## 📦 Tech Stack

| Tool | Purpose |
|------|---------|
| **Vanilla HTML/CSS/JS** | Zero dependencies, no frameworks |
| **Google Gemini 2.5 Flash Lite** | AI conversation fallback |
| **Web Speech API** | Voice recognition & synthesis |
| **Open-Meteo API** | Free weather data |
| **Notifications API** | Timer alerts |
| **PWA Manifest** | Mobile installability |

---

## 🛠️ Customisation

**Change the assistant's name or personality** — edit the system instruction in `askGemini()`:

```javascript
systemInstruction: {
  parts: [{ text: "You are a helpful assistant named Nova. ..." }]
}
```

**Add new commands** — drop a new `if` block inside `handleCommand()`:

```javascript
if (q.includes("my keyword")) {
  respond("Doing something cool!");
  return;
}
```

---

## 🐛 Troubleshooting

| Problem | Fix |
|---------|-----|
| Mic button does nothing | Use Chrome or Edge (Firefox unsupported) |
| "Mic error — check permissions" | Allow microphone access in browser settings |
| AI gives no response | Check your Gemini API key is correct and has quota |
| Weather not loading | Allow location access when prompted |
| Popups blocked | Allow popups for `file://` or your domain in browser |

---

## 📄 License

MIT — free to use, modify, and distribute.

---

<div align="center">

**Built by [Abdullah Tahir](https://github.com/Abd-Abdullah83)**
BS Data Science · FAST NUCES Lahore · 2025–2029

*"Build a company of lasting impact."*

⭐ Star this repo if you found it useful!

</div>
