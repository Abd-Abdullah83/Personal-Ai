<div align="center">

# 🤖 Personal AI Assistant — *Aria*

### Voice · Chat · Smart Commands · Powered by Gemini 2.5 Flash

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](.)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](.)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](.)
[![Gemini](https://img.shields.io/badge/Gemini_2.5_Flash-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev/)
[![PWA](https://img.shields.io/badge/PWA-5A0FC8?style=for-the-badge&logo=pwa&logoColor=white)](.)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](.)

<br/>

> **"Talk to it. It listens. It thinks. It acts."**
>
> A zero-dependency, single-file personal AI assistant that understands your voice,
> answers your questions with Gemini AI, checks live weather, sets timers,
> opens apps, searches the web — and talks back.

<br/>

[🚀 Live Demo](https://abd-abdullah83.github.io/Nova/) &nbsp;·&nbsp;
[🐛 Report Bug](https://github.com/Abd-Abdullah83/Nova/issues) &nbsp;·&nbsp;
[💡 Request Feature](https://github.com/Abd-Abdullah83/Nova/issues)

</div>

---

## ⚡ Features at a Glance

| Feature | Description |
|--------|-------------|
| 🎤 Voice Input | Real-time speech recognition (Chrome / Edge) |
| 🔊 Voice Output | Text-to-speech — Aria talks back to you |
| 🧠 Gemini AI | Handles any open-ended question intelligently |
| 🌤️ Live Weather | GPS-based forecast — no extra API key needed |
| ⏰ Smart Timers | Set countdowns with desktop push notifications |
| 📞 Call / SMS | Direct phone & SMS intent links |
| 💬 WhatsApp | Pre-filled message launcher |
| 🐦 Twitter / X | One-command tweet composer |
| 🔍 Web Search | Instant Google search by voice |
| ▶️ YouTube | Search & play videos hands-free |
| 🗺️ Google Maps | Navigate anywhere by voice |
| 📱 PWA Ready | Installable on Android / iOS home screen |
| 🔒 Fully Private | No server · No storage · Runs in your browser |

---

## 🗂️ Project Structure

```
Nova/
├── index.html       ← Entire app (single self-contained file)
├── manifest.json    ← PWA manifest for mobile install
├── icon-192.png     ← PWA icon
└── README.md        ← You are here
```

> **No build tools. No npm. No frameworks. One file is all it takes.**

---

## 🚀 Getting Started

### Step 1 — Get the Code

```bash
git clone https://github.com/Abd-Abdullah83/Nova.git
cd Nova
```

Or just **download `index.html`** and open it — it runs offline.

### Step 2 — Get a Free Gemini API Key

1. Go to **[aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)**
2. Sign in with your Google account
3. Click **"Create API Key"** and copy your key

### Step 3 — Paste Your Key

Open `index.html` and find this line near the top of the `<script>`:

```javascript
const API_KEY = "YOUR_KEY_HERE";
```

Replace `YOUR_KEY_HERE` with your actual key.

### Step 4 — Open & Use

```bash
# Simply open in your browser:
open index.html

# Or serve locally for full PWA features:
npx serve .
```

> ⚠️ **Chrome or Edge only** — Firefox does not support the Web Speech API.

---

## 🗣️ Command Reference

### 🕐 Time & Date
| Say | Result |
|-----|--------|
| "What's the time?" | Current time in your locale |
| "What's today's date?" | Full localized date string |

### 🌤️ Weather
| Say | Result |
|-----|--------|
| "What's the weather?" | Live weather from your GPS location |
| "What's the temperature?" | Temperature, humidity, wind speed |

### ⏰ Timers
| Say | Result |
|-----|--------|
| "Set a 5 minute timer" | Countdown + desktop notification |
| "Set a 30 second timer" | Works with seconds, minutes, hours |
| "Set an alarm" | Defaults to 5 minutes |

### 🔍 Search & Navigation
| Say | Result |
|-----|--------|
| "Search for FAST University" | Google search |
| "Open YouTube" | Launches YouTube |
| "Play lo-fi music on YouTube" | YouTube search query |
| "Navigate to Lahore" | Google Maps directions |
| "Open github.com" | Opens any website |

### 💬 Messaging & Social
| Say | Result |
|-----|--------|
| "Send WhatsApp message hello" | WhatsApp with pre-filled text |
| "Post on Twitter great day" | Twitter compose |
| "Open Instagram" | Opens Instagram |

### 📞 Communication
| Say | Result |
|-----|--------|
| "Call +923001234567" | Phone dialer |
| "SMS +923001234567 saying hello" | SMS with number and body |

### 🧠 AI Chat — Gemini Fallback
| Say | Result |
|-----|--------|
| "Explain machine learning" | Conversational AI answer |
| "Tell me a joke" | Gemini responds with humour |
| "Write a short poem" | Creative AI response |

---

## 🛠️ Customisation

### Rename the Assistant
```javascript
systemInstruction: {
  parts: [{ text: "You are a helpful assistant named Nova. Be friendly." }]
}
```

### Add a New Voice Command
```javascript
if (q.includes("calculator")) {
  respond("Opening calculator!");
  window.open("https://www.google.com/search?q=calculator");
  return;
}
```

### Change AI Personality
```javascript
"You are a sarcastic but helpful assistant. Keep it witty."
"You are a professional data science tutor."
"You only respond in Urdu."
```

### Switch Language
```javascript
recognition.lang = "ur-PK";   // Urdu
recognition.lang = "ar-SA";   // Arabic
recognition.lang = "fr-FR";   // French
```

---

## 🔒 Privacy & Security

| Concern | Reality |
|---------|---------|
| Is data stored? | ❌ No — nothing is ever saved anywhere |
| Is there a server? | ❌ No — runs entirely inside your browser |
| API key exposure | ⚠️ Key is client-side — for personal use only |
| Weather & location | GPS coords sent only to Open-Meteo's public API |
| Voice data | Processed locally by your browser's speech engine |

---

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| Mic button does nothing | Switch to **Chrome or Edge** |
| "Mic error — check permissions" | Allow microphone in browser site settings |
| AI gives no response | Verify your `API_KEY` is valid and has quota |
| Weather not loading | Allow **location access** when browser prompts |
| Links / popups blocked | Allow popups for this page in browser settings |
| Timer notification silent | Allow **notifications** when prompted |

---

## 📊 Tech Stack

| Layer | Technology |
|-------|-----------|
| UI | Vanilla HTML5 + CSS3 (dark theme, purple accent) |
| Logic | Vanilla JavaScript ES2020+ |
| AI Brain | Google Gemini 2.5 Flash (REST API) |
| Voice In | Web Speech API — `SpeechRecognition` |
| Voice Out | Web Speech API — `SpeechSynthesis` |
| Weather | Open-Meteo (free, no key) + Geolocation API |
| Alerts | Notifications API + `setTimeout` |
| Installs as App | PWA via `manifest.json` |

---

## 📄 License

MIT License — Free to use, modify, and distribute. Give credit where it's due. ✌️

---

<div align="center">

**── Built by ──**

### Abdullah Tahir

*BS Data Science · FAST NUCES Lahore · 2025–2029*

[![GitHub](https://img.shields.io/badge/GitHub-Abd--Abdullah83-181717?style=for-the-badge&logo=github)](https://github.com/Abd-Abdullah83)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-abdullah--tahir--ds-0A66C2?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/abdullah-tahir-ds)
[![Portfolio](https://img.shields.io/badge/Portfolio-abd--abdullah83.github.io-A78BFA?style=for-the-badge&logo=githubpages&logoColor=white)](https://abd-abdullah83.github.io)

<br/>

*"Build a company of lasting impact."* 🚀

⭐ **Star this repo** if it helped you — it means a lot!

*Made with 💜 and a lot of late-night coding sessions*

</div>
