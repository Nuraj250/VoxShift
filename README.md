# 🎙️ VoxShift

**VoxShift** is a modern, expressive text-to-speech web app that lets you generate lifelike voice clips in multiple styles and languages. Whether you’re making content, experimenting with AI, or just having fun — VoxShift brings your words to life.

---

## 🚀 Features

- 🎤 Convert any text into lifelike speech
- 🎭 Choose from expressive voice tones (neutral, calm, angry, etc.)
- 🌍 Support for multiple languages (English, Hindi, Spanish, etc.)
- 🎧 Play, preview, and download generated audio
- 🌓 Toggle between light & dark mode
- 💡 Built with clean, modular architecture

---

## 🧱 Tech Stack

| Layer     | Tooling           |
|-----------|-------------------|
| Frontend  | React + Bootstrap |
| Backend   | Flask (Python)    |
| TTS Engine| gTTS (Google TTS) |
| Styling   | Custom CSS / Neumorphism |
| API Comm. | Axios             |

---

## 🏗 Project Structure

```
voxshift/
├── backend/                ← Flask + gTTS
│   ├── app/
│   │   ├── __init__.py
│   │   ├── config.py
│   │   ├── routes/
│   │   │   └── tts.py
│   │   └── services/
│   │       └── tts_service.py
│   ├── audio_output/
│   ├── run.py
│   ├── requirements.txt
│   └── .env
│
├── frontend/               ← React + Bootstrap
│   ├── public/
│   └── src/
│       ├── components/
│       │   ├── VoiceForm.jsx
│       │   └── AudioPlayer.jsx
│       ├── App.jsx
│       ├── index.js
│       └── custom.css
│   └── package.json
```

---

## ⚙️ Getting Started

### 1️⃣ Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate         # or venv\Scripts\activate on Windows
pip install -r requirements.txt
```

Add a `.env` file in `/backend`:

```env
AUDIO_FOLDER=audio_output
DEBUG=true
TTS_PROVIDER=gtts
```

Run the Flask app:

```bash
python run.py
```

---

### 2️⃣ Frontend Setup

```bash
cd frontend
npm install
npm start
```

The frontend runs on `http://localhost:3000`  
The backend runs on `http://localhost:5000`

---

## 📦 API Reference

### `POST /api/speak`

Generate speech audio.

**Request JSON**:
```json
{
  "text": "Hello from VoxShift",
  "style": "neutral",
  "language": "en"
}
```

**Returns**: `.mp3` audio file

---

## 📥 Download & Play Audio

- 🎧 Output is streamed to the browser
- 📥 Download as `.mp3` with one click

---

## 🧪 Planned Enhancements

- 🎙 Support more voice engines (like ElevenLabs)
- 🔊 Real-time voice previews
- 🗂 Save history & favorites
- 🎚 Fine-tune voice pitch, speed, stability

---

## 🤝 Contributing

Want to contribute? PRs are welcome!  
To get started:
1. Fork the repo
2. Create a feature branch
3. Submit a pull request

---

## 🛡 License

MIT © 2025 Nuraj250

---

## 🌐 Project Name

> **VoxShift** — Where words find their voice.