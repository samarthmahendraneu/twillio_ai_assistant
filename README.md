# 🤖 AI Voice Recruiter Assistant

An AI-powered voice assistant that **answers calls from recruiters and responds to resume queries in real time**, built on **Twilio Voice** and the **OpenAI GPT Realtime API**. Samarth's personal details, skills, and experience are embedded into the assistant — so it can speak on his behalf, 24/7.

> 📞 **Try it live:** Call **+1 (833) 970-3274** and ask about Samarth's experience, skills, or availability.

---

## What It Does

A recruiter calls the number. The AI picks up, introduces itself as Samarth's assistant, and can answer questions like:

- *"What's his experience with distributed systems?"*
- *"Has he worked with Kafka or gRPC before?"*
- *"Is he open to remote roles?"*
- *"Can you schedule a call with him?"*

The assistant responds naturally using real-time speech, with Samarth's resume context baked in.

---

## Features

- 🎙️ **Real-time voice conversations** — no hold music, no forms, just a live AI call
- 📄 **Resume-aware responses** — answers questions about skills, projects, and experience
- 🛠️ **Tool calling** — can take actions like logging interest or scheduling follow-ups
- 📞 **Twilio Voice integration** — works on any phone, no app needed
- 🤖 **OpenAI GPT Realtime API** — low-latency, natural conversational AI
- 🌐 **WebSocket audio streaming** — continuous two-way audio between caller and AI

---

## Architecture

```
Recruiter calls +1 (833) 970-3274
  │
  ▼
Twilio Voice (inbound call handler)
  │
  ▼
WebSocket Media Stream (real-time audio)
  │
  ▼
FastAPI Backend (resume context + tool routing)
  │
  ▼
OpenAI GPT Realtime API (speech ↔ AI ↔ speech)
  │
  ▼
AI responds as Samarth's voice assistant
```

The backend injects Samarth's resume and personal context into the system prompt, so the AI always answers in his context. Tool calls (e.g., scheduling, logging) are handled server-side.

---

## Tech Stack

| Technology | Role |
|---|---|
| **Python** | Core backend language |
| **FastAPI** | Async WebSocket server |
| **Twilio Voice + Media Streams** | Phone call handling & audio transport |
| **OpenAI GPT Realtime API** | Conversational AI engine |
| **WebSockets** | Bi-directional audio streaming |
| **Tool Calling** | Actions like scheduling & CRM logging |



## Future Improvements

- [ ] Voice cloning to sound more like Samarth
- [ ] Calendar integration for live scheduling
- [ ] CRM logging (save recruiter info + questions)
- [ ] Real-time transcript dashboard

---

## Author

**Samarth Mahendra**  
Backend & Distributed Systems Engineer
