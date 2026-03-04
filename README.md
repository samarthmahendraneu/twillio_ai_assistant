# Twilio GPT Realtime Voice Chatbot

A real-time AI voice chatbot that can **call and converse with users over phone calls using Twilio**, powered by the **OpenAI GPT Realtime API**. The system streams audio between Twilio and the AI model, enabling natural, low-latency conversations.

This project demonstrates how to build a **production-style AI voice agent** capable of interacting with humans via phone calls.

---

## Features

- 🎙️ Real-time voice conversations over phone calls
- 📞 Twilio Voice integration for inbound and outbound calls
- 🤖 OpenAI **GPT Realtime API** for low-latency conversational AI
- 🌐 WebSocket audio streaming between Twilio and the AI model
- 🧠 Conversational context handling
- 🔧 Extensible architecture for tool calling (e.g., scheduling meetings or CRM queries)

---

## Architecture

```
Caller
  │
  ▼
Twilio Voice
  │
  ▼
WebSocket Media Stream
  │
  ▼
Backend Server (FastAPI / Python)
  │
  ▼
OpenAI GPT Realtime API
  │
  ▼
AI-generated speech response
```

The backend server acts as a **proxy**, forwarding audio streams between Twilio and the GPT Realtime API while maintaining conversation state.

---

## Tech Stack

| Technology | Role |
|---|---|
| **Python** | Core backend language |
| **FastAPI** | Async web framework for WebSocket server |
| **Twilio Voice + Media Streams** | Phone call integration & audio streaming |
| **OpenAI GPT Realtime API** | Low-latency conversational AI engine |
| **WebSockets** | Bi-directional audio stream proxy |

---

## Example Use Cases

- 🧑‍💼 AI recruiter calling candidates
- 🎧 AI customer support agents
- 📅 Automated appointment scheduling
- 🗣️ Interactive voice assistants

---



## Future Improvements

- [ ] Voice cloning support
- [ ] Real-time analytics dashboard

---

## Author

**Samarth Mahendra**  
Backend & Distributed Systems Engineer
