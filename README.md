<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=30&pause=1000&color=A78BFA&center=true&vCenter=true&width=600&lines=🤖+Personal+AI+Assistant;Voice+%7C+Chat+%7C+Smart+Commands;Powered+by+Gemini+2.5+Flash" alt="Typing SVG" />

<br/>

```
 ██████╗ ███████╗██████╗ ███████╗ ██████╗ ███╗   ██╗ █████╗ ██╗
 ██╔══██╗██╔════╝██╔══██╗██╔════╝██╔═══██╗████╗  ██║██╔══██╗██║
 ██████╔╝█████╗  ██████╔╝███████╗██║   ██║██╔██╗ ██║███████║██║
 ██╔═══╝ ██╔══╝  ██╔══██╗╚════██║██║   ██║██║╚██╗██║██╔══██║██║
 ██║     ███████╗██║  ██║███████║╚██████╔╝██║ ╚████║██║  ██║███████╗
 ╚═╝     ╚══════╝╚═╝  ╚═╝╚══════╝ ╚═════╝ ╚═╝  ╚═══╝╚═╝  ╚═╝╚══════╝
                      AI  ASSISTANT  —  ARIA
```

<br/>

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

<br/>

## 📸 Preview

```
┌─────────────────────────────────────────────────┐
│          🤖  Personal AI Assistant               │
│      Voice or type — powered by Gemini           │
│                                                  │
│  ┌───────────────────────────────────────────┐   │
│  │  Hello! Tap the mic or type a command.    │   │
│  │                                           │   │
│  │              What's the weather?   [YOU]  │   │
│  │                                           │   │
│  │  [AI]  Current weather: clear sky.        │   │
│  │        Temperature is 28°C, humidity 55%  │   │
│  └───────────────────────────────────────────┘   │
│                                                  │
│   Status: Ready                                  │
│                                                  │
│  ┌──────────────────────────┐  [➤]  [🎤]        │
│  │  Type a command...       │                    │
│  └──────────────────────────┘                    │
│                                                  │
│  ┌ TRY SAYING... ────────────────────────────┐   │
│  │ [What's the time?]  [Set a 5 min timer]   │   │
│  │ [Open YouTube]  [Tell me a joke]          │   │
│  └───────────────────────────────────────────┘   │
└─────────────────────────────────────────────────┘
```

<br/>

---

## ⚡ Features at a Glance

<br/>

```
🎤  VOICE INPUT          Real-time speech recognition (Chrome / Edge)
🔊  VOICE OUTPUT         Text-to-speech — Aria talks back to you
🧠  GEMINI AI            Handles any open-ended question intelligently
🌤️  LIVE WEATHER         GPS-based forecast — no extra API key needed
⏰  SMART TIMERS         Set countdowns with desktop push notifications
📞  CALL / SMS           Direct phone & SMS intent links
💬  WHATSAPP             Pre-filled message launcher
🐦  TWITTER / X          One-command tweet composer
🔍  WEB SEARCH           Instant Google search by voice
▶️  YOUTUBE              Search & play videos hands-free
🗺️  GOOGLE MAPS          Navigate anywhere by voice
📱  PWA READY            Installable on Android / iOS home screen
🔒  FULLY PRIVATE        No server · No storage · Runs in your browser
```

<br/>

---

## 🗂️ Project Structure

```
Nova/
│
├── 📄  index.html          ← Entire app (single self-contained file)
├── 📋  manifest.json       ← PWA manifest for mobile install
├── 🖼️  icon-192.png        ← PWA icon
└── 📖  README.md           ← You are here
```

> **No build tools. No npm. No frameworks. One file is all it takes.**

<br/>

---

## 🚀 Getting Started

### Step 1 — Get the Code

```bash
git clone https://github.com/Abd-Abdullah83/Nova.git
cd Nova
```

Or just **download `index.html`** and open it — it runs offline.

---

### Step 2 — Get a Free Gemini API Key

1. Go to **[aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)**
2. Sign in with your Google account
3. Click **"Create API Key"**
4. Copy your key

---

### Step 3 — Paste Your Key

Open `index.html` and find this line near the top of the `<script>`:

```javascript
// ── PASTE YOUR GEMINI API KEY HERE ──────────────────────────
const API_KEY = "YOUR_KEY_HERE";
// ────────────────────────────────────────────────────────────
```

Replace `YOUR_KEY_HERE` with your actual key.

---

### Step 4 — Open & Use

```bash
# Simply open in your browser:
open index.html

# Or serve locally for PWA features:
npx serve .
```

> ⚠️ **Chrome or Edge only** for voice recognition.
> Firefox does not support the Web Speech API.

<br/>

---

## 🗣️ Command Reference

<br/>

### 🕐 Time & Date
```
"What's the time?"        →  Saturday, 11 April 2026 at 3:45 PM
"What's today's date?"    →  Full localized date string
```

### 🌤️ Weather
```
"What's the weather?"     →  Live weather from your GPS location
"What's the temperature?" →  Temperature, humidity, wind speed
```

### ⏰ Timers
```
"Set a 5 minute timer"    →  Countdown + desktop notification
"Set a 30 second timer"   →  Works with seconds, minutes, hours
"Set an alarm"            →  Defaults to 5 minutes
```

### 🔍 Search & Navigation
```
"Search for FAST University"     →  Google search
"Open YouTube"                   →  Launches YouTube
"Play lo-fi music on YouTube"    →  YouTube search query
"Open Google Maps"               →  Google Maps
"Navigate to Lahore"             →  Directions in Maps
"Open github.com"                →  Opens any website
```

### 💬 Social & Messaging
```
"Send WhatsApp message hello"    →  WhatsApp with pre-filled text
"Post on Twitter great day"      →  Twitter compose
"Open Instagram"                 →  Instagram
"Open Facebook"                  →  Facebook
```

### 📞 Communication
```
"Call +923001234567"              →  Phone dialer
"SMS +923001234567 saying hello"  →  SMS app with number and body
```

### 🧠 AI Chat — Gemini Fallback
```
"Explain machine learning"       →  Conversational AI answer
"Tell me a joke"                 →  Gemini responds with humour
"What is quantum computing?"     →  Any open-ended question
"Write a short poem"             →  Creative AI responses
```

<br/>

---

## 🏗️ How It Works

```
                    ┌──────────────────────────────┐
                    │         USER INPUT            │
                    │   (Voice mic / Text field)    │
                    └──────────────┬───────────────┘
                                   │
                    ┌──────────────▼───────────────┐
                    │        COMMAND ROUTER         │
                    │   (Pattern matching in JS)    │
                    └──┬────┬────┬────┬────┬───────┘
                       │    │    │    │    │
              ┌────────▼┐ ┌─▼──┐ │ ┌─▼──┐ │
              │ Weather │ │Maps│ │ │ TTS│ │
              │Open-    │ │Apps│ │ │Speak│ │
              │Meteo API│ │URLs│ │ └────┘ │
              └─────────┘ └────┘ │        │
                                 │        │
                    ┌────────────▼──┐  ┌──▼──────────────────┐
                    │  GEMINI AI    │  │  TIMER + NOTIF.     │
                    │  Fallback for │  │  setTimeout +       │
                    │  all unknowns │  │  Notifications API  │
                    └───────────────┘  └─────────────────────┘

        RESPONSE  →  addMessage()  →  speak()  →  User hears + reads
```

<br/>

---

## 🛠️ Customisation

### Rename the Assistant

```javascript
systemInstruction: {
  parts: [{ text: "You are a helpful assistant named Nova. Be friendly." }]
}
```

---

### Add a New Voice Command

Drop a block inside `handleCommand()`:

```javascript
// Example: "open calculator"
if (q.includes("calculator")) {
  respond("Opening calculator!");
  window.open("https://www.google.com/search?q=calculator");
  return;
}
```

---

### Change AI Personality

```javascript
"You are a sarcastic but helpful assistant. Keep it witty."
"You are a professional data science tutor."
"You only respond in Urdu."
```

---

### Switch Language

```javascript
recognition.lang = "ur-PK";   // Urdu
recognition.lang = "ar-SA";   // Arabic
recognition.lang = "fr-FR";   // French
```

<br/>

---

## 🔒 Privacy & Security

| Concern | Reality |
|---------|---------|
| **Is data stored?** | ❌ No. Nothing is ever saved anywhere. |
| **Is there a server?** | ❌ No. Runs entirely inside your browser. |
| **API key exposure** | ⚠️ Key is client-side — for personal use only. |
| **Weather & location** | GPS coords sent only to Open-Meteo's public API. |
| **Voice data** | Processed locally by your browser's speech engine. |

<br/>

---

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| Mic button does nothing | Switch to **Chrome or Edge** |
| "Mic error — check permissions" | Allow microphone in browser site settings |
| AI gives no response | Verify your `API_KEY` is valid and has quota |
| "Sorry, I couldn't connect" | Check internet connection |
| Weather not loading | Allow **location access** when browser prompts |
| Links / popups blocked | Allow popups for this page in browser settings |
| Timer notification silent | Allow **notifications** when prompted |

<br/>

---

## 📊 Tech Stack

| Layer | Technology |
|-------|-----------|
| **UI** | Vanilla HTML5 + CSS3 (dark theme, purple accent) |
| **Logic** | Vanilla JavaScript ES2020+ |
| **AI Brain** | Google Gemini 2.5 Flash Lite (REST API) |
| **Voice In** | Web Speech API — `SpeechRecognition` |
| **Voice Out** | Web Speech API — `SpeechSynthesis` |
| **Weather** | Open-Meteo (free, no key) + Geolocation API |
| **Alerts** | Notifications API + `setTimeout` |
| **Installs as App** | PWA via `manifest.json` |

<br/>

---

## 📄 License

```
MIT License — Free to use, modify, and distribute.
Give credit where it's due. ✌️
```

<br/>

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

<br/>

⭐ **Star this repo** if it helped you — it means a lot!

---

*Made with 💜 and a lot of late-night coding sessions*

</div>
