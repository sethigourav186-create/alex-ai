# alex-ai
Secure local AI assistant with password + face 2FA, 4 activation modes, TinyLlama 1.1B, real-time search. 100% local, no cloud, no GPU required.
# A.L.E.X — Artificial Local EXecutive

**Defence Intelligence Assistant | Secure | Voice-Activated | 100% Local**

A locally-run AI assistant powered by TinyLlama-1.1B with multi-factor authentication, 4 activation modes, and real-time web intelligence.

## ✨ Key Features

- 🔐 **Security**: Password (PBKDF2-SHA256) + Face Lock 2FA with injection detection
- 🎙️ **4 Activation Modes**: Voice (en-IN), Clap detection, Face scan, Keyboard
- 🧠 **Local AI**: TinyLlama 1.1B on CPU (no GPU needed, no cloud)
- 🌐 **Live Intelligence**: DuckDuckGo + Wikipedia real-time search
- 🛡️ **Threat Protection**: Prompt injection blocking + security logging
- 🔇 **Offline Voice**: pyttsx3 TTS + Google Speech API (en-IN)
- ⚡ **Compact**: 444 lines Python, production-ready

## 🎯 Problems Solved

| Problem | Solution |
|---------|----------|
| No security in AI tools | Password + Face Lock 2FA |
| Cloud privacy risk | 100% local (no data leaves PC) |
| Always need keyboard | 4 hands-free activation modes |
| AI knowledge outdated | Live DuckDuckGo + Wikipedia |
| Expensive AI tools | Free & open-source (TinyLlama) |
| Needs expensive GPU | Runs on CPU only |

## 🚀 Quick Start

```bash
pip install torch transformers SpeechRecognition pyttsx3 pyaudio numpy opencv-contrib-python duckduckgo-search

python alex_compact.py
```

**First run:** Set password → Enable Face Lock (optional) → Choose activation mode → Start querying

## 📋 Tech Stack

- **AI**: PyTorch + HuggingFace Transformers (TinyLlama-1.1B)
- **Vision**: OpenCV + LBPH Face Recognizer
- **Voice**: SpeechRecognition + pyttsx3 TTS
- **Security**: PBKDF2-SHA256 + XOR encryption
- **Search**: DuckDuckGo API + Wikipedia REST

## 🎮 Commands

- `/changepass` — Change login password
- `/facelock` — Enable/disable/re-enroll Face Lock
- `/clear` — Clear conversation history
- `quit` — End session

## 📊 Performance

- **Login**: 2-3 sec (+ 8 sec with face)
- **Response**: 3-8 sec (search + AI + TTS)
- **Memory**: ~1.5-2GB RAM
- **Hardware**: Any laptop (CPU-only)

## 🔒 Security Notes

- Passwords stored as PBKDF2-SHA256 encrypted XOR (never plain text)
- Face data local in `.face_model.yml` (not in cloud)
- All injection attempts logged to `.thr` file
- Lockout: 3 fails = 5-minute access denial

## 📚 Author

**Gourav** — B.Tech IT, Rajasthan Technical University (RTU), Kota  
Built for academic project & real-world security research.

---

## License

MIT License — Feel free to fork, modify, and use!
