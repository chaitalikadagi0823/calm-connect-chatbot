# 🌿 Calm Connect — Chat Assistant for Health & Calming Suggestions

A web-based chat assistant that offers grounding techniques, mood tracking, and wellness suggestions to support users through moments of stress, anxiety, or low energy.

## 📌 Overview

Calm Connect is a chat interface where users can talk about how they're feeling and receive supportive responses — including grounding exercises, sleep tips, study tips, and anxiety-relief suggestions. It combines a custom front end with a connected backend service for generating chat replies.

## ✨ Features

- **Chat interface** with a clean, dark-themed UI and bot/user message bubbles
- **Mood detection** — automatically detects mood (happy, sad, stressed, anxious, angry, okay) from keywords in user messages
- **Mood tracking & history** — logs daily mood and renders a trend chart using HTML5 Canvas, stored locally via `localStorage`
- **Grounding techniques** — quick-access tools like 4-2-6 breathing, 5-4-3-2-1 grounding, and a 5-second reset
- **Voice input & output** — speech-to-text using the Web Speech API (`webkitSpeechRecognition`) and text-to-speech playback of the assistant's replies
- **Contextual wellness suggestions** — keyword-triggered tips for anxiety, sleep, study pressure, tension, and low motivation
- **Daily motivational quote** shown on load
- **Connected backend service** — chat messages are sent to a hosted backend API which returns the assistant's reply

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Front-end | HTML, CSS, JavaScript |
| Voice | Web Speech API (Speech Recognition & Speech Synthesis) |
| Data (client-side) | Browser `localStorage` for mood history |
| Visualization | HTML5 Canvas (custom-drawn mood chart) |
| Backend | Hosted API service (returns chat replies) |
| Hosting | Netlify (front-end) |

## 🚀 How It Works

1. The user types (or speaks) a message describing how they're feeling.
2. The front end scans the message for mood-related keywords and logs the detected mood.
3. The message is sent to a backend API, which returns a reply that's displayed in the chat.
4. Based on keywords in the message (or detected mood), the assistant also offers relevant suggestions — breathing exercises, sleep tips, study tips, or motivational messages.
5. Mood history is tracked over time and visualized as a simple trend line.

## 📄 My Contribution

- Built the front-end chat interface, including layout, styling, and message flow.
- Implemented keyword-based mood detection and the mood-history trend chart.
- Added voice input/output using the Web Speech API.
- Designed the rule-based wellness suggestion system (grounding techniques, sleep/study/anxiety tips).
- Connected the front end to a hosted backend service for generating chat replies.

## 🔮 Future Improvements

- Expand backend reply generation with more advanced natural-language understanding
- Add user accounts to sync mood history across devices
- Weekly/monthly mood summary reports

---
*This project was developed as a personal/academic project to explore practical, supportive applications of web technology in mental wellness.*
