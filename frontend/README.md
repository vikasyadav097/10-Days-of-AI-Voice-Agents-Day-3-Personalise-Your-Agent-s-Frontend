# 📚 Day 3 – Personalise Your Agent's Frontend

> Building a personalised voice learning assistant designed to make learning more interactive, accessible, and engaging.

Part of **10 Days of Voice Agents – Voice for Bharat Edition** 🚀

Day 1 focused on making the voice agent talk. 🎙️
Day 2 gave the agent a personality, learning-focused objectives, and safety guardrails. 🛡️
Day 3 focuses on the **frontend experience** — making LearnMate feel like a friendly, modern learning companion. 🎨

---

## 🧠 Meet LearnMate

**LearnMate** is a voice-powered AI learning assistant designed to help learners understand concepts through natural conversation.

Instead of simply giving answers, LearnMate encourages learners to:

- ❓ Ask questions
- 💡 Understand difficult concepts
- 🪜 Learn step-by-step
- 🗣️ Practice through conversation
- 🌱 Build confidence while learning

The interface is designed to feel simple, friendly, and distraction-free.

---

## 🎯 Day 3 Objectives

The goal of Day 3 was to personalise the frontend around the **Learning & Literacy** track.

The frontend includes:

- ✅ Learning-focused visual design
- ✅ Student-friendly interface
- ✅ Clear voice interaction states
- ✅ Listening and speaking indicators
- ✅ Animated AI learning visualisation
- ✅ Microphone permission handling
- ✅ Restart conversation flow
- ✅ Responsive layout
- ✅ LiveKit voice interaction

---

## 🎨 Frontend Design

The LearnMate interface uses a **modern dark educational theme** with:

- 🌌 Deep blue and purple gradients
- ✨ Soft glowing backgrounds
- 🔲 Subtle technology grid
- 📖 Learning-focused icons
- 🎙️ Animated voice indicators
- 🤖 AI-themed visual elements
- 🔤 Clean typography
- 🧘 Minimal distractions

The goal is to combine **education + AI + voice technology** into a single, calm interface.

---



---

## 🔄 Agent States

The frontend clearly represents every major state of the voice agent.

| State | Screen text | What the learner sees |
|---|---|---|
| 🟢 **Ready** | "Ready to Learn?" | A clear button to begin the session |
| 🔵 **Connecting** | "Connecting to LearnMate..." | Indicator that the agent is joining the call |
| 🎧 **Listening** | "Listening to you..." | Animated voice indicators showing the mic is active |
| 🔊 **Speaking** | "LearnMate is speaking..." | Voice visualisation shifts to show a response is playing |
| ⚪ **Call Ended** | "Session ended" | A restart option to begin another learning session |

```text
READY → CONNECTING → LISTENING → SPEAKING → CALL ENDED → START AGAIN
```

---

## 🎙️ Voice Interaction Flow

LearnMate uses real-time voice communication end to end:

```text
Learner
  │
  ▼
🎤 Microphone
  │
  ▼
🧾 Speech Recognition
  │
  ▼
🧠 LearnMate AI Agent
  │
  ▼
🔊 Murf Falcon TTS
  │
  ▼
Natural Voice Response
```

This lets learners interact naturally instead of typing every question. ⌨️❌ 🗣️✅

---

## 📚 Learning Experience

LearnMate is built around the **Learning & Literacy** track and handles Hindi, English, and Hinglish conversations naturally.

**Example interaction:**

> **Learner:** "Mujhe photosynthesis simple language mein samjha do."
>
> **LearnMate:** "Bilkul! 🌱 Plants sunlight ki help se apna food banate hain. Is process ko photosynthesis kehte hain. Agar tum chaho toh main ise ek simple example ke saath step-by-step bhi samjha sakta hoon."

---

## 🛡️ Learning Safety

LearnMate follows learning-focused guardrails.

**The agent should:**

- ✅ Encourage learners
- ✅ Explain concepts without unnecessary complexity
- ✅ Ask guiding questions
- ✅ Admit when it doesn't know something
- ✅ Encourage further learning

**The agent should never:**

- ❌ Shame a learner for a wrong answer
- ❌ Mock mistakes
- ❌ Claim a learner has a learning disability
- ❌ Pretend to be a teacher or professional when it isn't
- ❌ Give unsafe or inappropriate instructions
- ❌ Invent educational facts when uncertain

A wrong answer is treated as an opportunity to learn, never a moment to correct harshly. 🌱

---

## 🎤 Microphone Permission Handling

If microphone access is blocked, LearnMate shows a clear, friendly message instead of failing silently:

> ⚠️ **Microphone access is blocked.**
> Please allow microphone permission in your browser settings and try again.

This makes it easy for learners to recover from permission issues without getting stuck. 🔓

---

## 🏗️ Frontend Architecture

```text
Next.js Frontend
      │
      ▼
  LearnMate UI
      │
      ├── 🟢 Ready State
      ├── 🔵 Connecting State
      ├── 🎧 Listening State
      ├── 🔊 Speaking State
      └── ⚪ Call Ended State
      │
      ▼
LiveKit Components
      │
      ▼
  Voice Agent
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Next.js, React, TypeScript, Tailwind CSS |
| Voice AI | LiveKit Agents, Murf Falcon TTS, Speech-to-Text |
| Development | Git, GitHub, VS Code, Python |

---

## 📂 Project Structure

```text
murf-livekit-starter-main/
├── backend/
│   ├── src/
│   │   └── agent.py
│   ├── .env.example
│   └── pyproject.toml
│
├── frontend/
│   ├── app/
│   ├── components/
│   ├── hooks/
│   ├── lib/
│   ├── styles/
│   └── package.json
│
├── README.md
├── AGENTS.md
└── LICENSE
```

---

## ▶️ Running the Project

**Backend**

```bash
cd backend
uv sync
uv run python src/agent.py dev
```

**Frontend**

```bash
cd frontend
pnpm install
pnpm dev
```

Then open 👉 `http://localhost:3000`

---

## 🧪 Day 3 Testing Checklist

**Frontend**
- [x] 🎨 Personalised Learning & Literacy theme
- [x] 🏷️ LearnMate branding
- [x] 🌌 Custom background
- [x] 🤖 AI visualisation
- [x] 👀 Animated Glow Eyes
- [x] 📱 Responsive interface

**Voice States**
- [x] 🟢 Ready
- [x] 🔵 Connecting
- [x] 🎧 Listening
- [x] 🔊 Speaking
- [x] ⚪ Call ended

**Voice Interaction**
- [x] 🎤 Microphone access
- [x] ⚡ LiveKit connection
- [x] 🗣️ Learner voice input
- [x] 🔊 AI voice response
- [x] 🔁 Conversation restart

**Accessibility**
- [x] 💬 Clear status messages
- [x] 🔘 Clear interaction button
- [x] 🔓 Microphone permission guidance
- [x] 🧭 Easy-to-understand interface

---

## 🎥 Day 3 Demo

The Day 3 video demonstrates the complete LearnMate experience:

1. 🏠 LearnMate landing screen
2. 🎨 Personalised Learning & Literacy interface
3. 👀 Animated AI Glow Eyes
4. 🟢 Ready state
5. 🔵 Connecting state
6. 🎧 Listening state
7. 🙋 Learner asking a question
8. 🔊 LearnMate responding through voice
9. 🗣️ Speaking state
10. ☎️ Ending the conversation
11. ⚪ Call ended state
12. 🔁 Restarting the learning session

---

## 🚀 What I Built

For Day 3, I personalised the frontend of my voice agent around the **Learning & Literacy** track.

The main focus wasn't just making the interface visually attractive — it was making every interaction state obvious to the learner, so they always know exactly what LearnMate is doing:

```text
🟢 READY  →  🔵 CONNECTING  →  🎧 LISTENING  →  🔊 SPEAKING  →  ⚪ CALL ENDED  →  🔁 START AGAIN
```

The custom animated AI eyes give LearnMate an additional visual identity, while keeping the interface calm and focused on learning rather than flashy for its own sake. ✨

---

## 🔮 Future Improvements

- 📖 Subject-specific learning modes
- 🧮 Interactive mathematics tutoring
- 🔬 Science explanations
- 🗣️ Pronunciation practice
- 🌐 More Indian languages
- 📝 Voice-based quizzes
- 🎯 Personalised learning paths
- 📊 Learning progress tracking
- 🧠 Adaptive difficulty
- 👨‍🏫 Teacher dashboard

---

## 👨‍💻 Author

**Vikas Yadav**
GitHub: [github.com/vikasyadav097](https://github.com/vikasyadav097)

## 📜 License

MIT License

---

## 🚀 10 Days of Voice Agents

Built as part of **10 Days of Voice Agents – Voice for Bharat Edition** 🇮🇳

Powered by **Murf Falcon • LiveKit • AI • Next.js**

`#VoiceForBharat` `#10DaysOfVoiceAgents` `#MurfAI` `#VoiceAI` `#GenerativeAI` `#LearningAndLiteracy` `#AI` `#NextJS` `#LiveKit`
