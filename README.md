# 🎙️ Pronunciation Coach

An AI-powered language pronunciation practice PWA built with a single HTML file.  
Record yourself reading example sentences, get instant feedback from Gemini AI, and build a daily speaking habit.

---

## ✨ Features

- 🌍 **5 Languages** — Mandarin, English, Japanese, German, French
- 🤖 **AI Pronunciation Scoring** — Gemini 2.5 Flash listens to your audio and scores your pronunciation with per-word feedback
- 🔊 **Natural TTS** — Gemini TTS API generates high-quality example audio for every sentence
- 🖼️ **AI Illustrations** — Context-aware images generated per sentence to reinforce memory
- 📚 **Multiple Practice Sets** — Free trial (5 sentences) + 30 Essential Phrases (Japanese & English)
- 🌐 **Native Language UI** — Full interface localisation (繁中 / English / 日本語)
- 🔁 **Retry & Best Score** — Re-record as many times as you want; best score is saved
- 🔒 **Score Gate** — Must reach 60 points to advance to the next sentence
- ⚡ **Smart Caching** — TTS audio cached in memory; images compressed to 50% JPEG and persisted in localStorage
- 📱 **Mobile-first** — Designed for iPhone/Android Chrome; works as an installable PWA

---

## 🚀 Live Demo

**[pronunciation-coach.pages.dev](https://pronunciation-coach.pages.dev)**

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Vanilla HTML / CSS / JS (single file) |
| AI Scoring | Gemini 2.5 Flash (audio input) |
| TTS | Gemini 2.5 Flash Preview TTS |
| Image Generation | Gemini 2.5 Flash Image |
| Hosting | Cloudflare Pages |
| Recording | MediaRecorder API (WebM / MP4) |
| Storage | localStorage (images), memory (TTS audio) |

---

## 📋 Requirements

- A **Gemini API Key** — free tier available at [aistudio.google.com](https://aistudio.google.com)
- Chrome or Edge browser (iOS Safari not supported due to MediaRecorder limitations)

---

## 🔧 Setup

1. Clone or download this repo
2. Open `index.html` in Chrome / Edge
3. Enter your Gemini API Key when prompted (stored locally on your device only)
4. Select a learning language and your native language
5. Start practicing!

No build step, no dependencies, no server required.

---

## 💰 Cost Estimate (Gemini API)

| Action | Cost per call | Daily (5 sentences × 3 retries) |
|--------|--------------|----------------------------------|
| Pronunciation scoring | ~$0.0005 | ~$0.008 |
| TTS generation | ~$0.002 | ~$0.01 (cached after first use) |
| Image generation | ~$0.039 | ~$0.195 (cached in localStorage) |

**Free tier (1,500 requests/day) covers all personal use — effectively free.**

---

## 📁 Project Structure

```
pronunciation-coach/
└── index.html    # Entire app in a single file
└── README.md
```

---

## 🗺️ Roadmap

- [ ] More languages (Spanish, Korean, Italian)
- [ ] More practice sets per language
- [ ] Streak tracking with localStorage
- [ ] Progress history chart
- [ ] PWA offline support (Service Worker)

---

## 📄 License

MIT — feel free to fork and extend.
