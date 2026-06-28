# 🎙️ AI Interviewer – End-to-End AI Powered Technical Interview Platform

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![React](https://img.shields.io/badge/Frontend-React-61DAFB)
![Express](https://img.shields.io/badge/Backend-Express-000000)
![Bun](https://img.shields.io/badge/Runtime-Bun-000000)
![OpenAI](https://img.shields.io/badge/AI-OpenAI_Realtime-10A37F)
![Gemini](https://img.shields.io/badge/LLM-Google_Gemini-4285F4)
![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791)
![Prisma](https://img.shields.io/badge/ORM-Prisma-2D3748)

---

# 📖 Overview

AI Interviewer is a full-stack AI-powered technical interviewing platform that conducts real-time voice interviews, evaluates candidate performance, and generates detailed interview feedback.

The platform simulates a real technical interview similar to products such as Mercor and modern AI recruiting assistants.

Candidates can provide their GitHub or LinkedIn profile, after which the AI gathers context about their background and conducts a personalized interview using voice conversations.

After the interview, an AI evaluator analyzes the complete conversation and produces a comprehensive performance report.

---

# 🚀 Features

## Candidate Profile Analysis

- GitHub Profile Analysis
- LinkedIn Profile Analysis
- Repository Information Extraction
- Programming Language Detection
- Project Analysis
- Candidate Skill Identification

---

## AI Voice Interview

- Real-time Voice Conversation
- AI Interviewer
- Natural Human-like Responses
- Low Latency Communication
- Dynamic Question Generation
- Context Aware Interview

---

## Speech Recognition

- Live Speech-to-Text
- Real-time Transcript Generation
- Conversation History Storage
- Accurate Voice Recognition

---

## AI Evaluation

After the interview, Gemini evaluates:

- Technical Knowledge
- Communication Skills
- Problem Solving Ability
- Confidence Level
- Explanation Quality
- Overall Performance
- Final Score
- Personalized Feedback

---

## Interview History

- Store Interview Sessions
- Complete Conversation History
- Candidate Reports
- Previous Interview Tracking

---

# 🏗️ System Architecture

```
Candidate
     │
     ▼
Frontend (React + Tailwind + ShadCN)
     │
     ▼
Express Backend (Bun Runtime)
     │
     ├──────────────► GitHub API
     │
     ├──────────────► LinkedIn Data
     │
     ├──────────────► OpenAI Realtime API
     │
     ├──────────────► Deepgram
     │
     ├──────────────► PostgreSQL
     │
     └──────────────► Gemini AI
```

---

# 🛠 Tech Stack

## Frontend

- React
- TypeScript
- Tailwind CSS
- ShadCN UI

---

## Backend

- Bun Runtime
- Express.js
- TypeScript

---

## AI Services

- OpenAI Realtime API
- Google Gemini
- Deepgram

---

## Database

- PostgreSQL
- Prisma ORM

---

## Other Technologies

- WebRTC
- REST APIs
- TurboRepo
- GitHub API

---

# ⚙️ Project Workflow

## Step 1 — Candidate Registration

The candidate enters:

- GitHub Profile
- LinkedIn Profile

The backend collects public profile information and builds a technical profile.

---

## Step 2 — AI Context Building

The system extracts:

- Skills
- Technologies
- Projects
- Programming Languages
- Repository Details
- Experience

This information becomes the context for the interview.

---

## Step 3 — Voice Interview

The browser establishes a WebRTC connection with the OpenAI Realtime API.

The AI interviewer begins asking technical questions based on the candidate profile.

Example:

> "I noticed you've worked on a RAG application using Azure. Can you explain how the retrieval pipeline works?"

---

## Step 4 — Live Conversation

During the interview:

- Candidate speaks
- Audio is streamed
- OpenAI generates responses
- Deepgram creates transcripts
- Messages are stored in PostgreSQL

Everything happens in real time.

---

## Step 5 — Conversation Storage

Every message is saved:

```
Candidate
↓

Question

↓

Candidate Answer

↓

AI Response

↓

Timestamp

↓

Database
```

This creates complete interview history.

---

## Step 6 — AI Evaluation

Once the interview finishes:

Conversation history is sent to Gemini.

Gemini analyzes:

- Technical Depth
- Communication
- Confidence
- Problem Solving
- Overall Performance

---

## Step 7 — Report Generation

The candidate receives:

- Final Score
- Strengths
- Weaknesses
- Improvement Suggestions
- Overall Recommendation

---

# 🗄 Database Design

The project uses PostgreSQL with Prisma.

Main entities include:

- User
- Interview
- Message
- Transcript
- Evaluation
- Score

Each interview stores:

- Interview Status
- Start Time
- End Time
- Transcript
- AI Feedback
- Final Score

---

# 🎤 Voice Pipeline

```
Microphone

↓

Browser

↓

WebRTC

↓

OpenAI Realtime API

↓

AI Response

↓

Deepgram

↓

Transcript

↓

Database
```

---

# 🧠 AI Evaluation Pipeline

```
Conversation History

↓

Gemini AI

↓

Technical Analysis

↓

Communication Analysis

↓

Confidence Analysis

↓

Final Score

↓

Feedback Report
```

---

# 📂 Project Structure

```
ai-interviewer/

├── apps/
│   ├── web
│   └── server
│
├── packages/
│   ├── database
│   ├── ui
│   └── shared
│
├── prisma
├── package.json
├── turbo.json
└── README.md
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/ai-interviewer.git
```

Install dependencies

```bash
bun install
```

Run the development server

```bash
bun dev
```

---

# 🔑 Environment Variables

Create a `.env` file.

```
DATABASE_URL=

OPENAI_API_KEY=

DEEPGRAM_API_KEY=

GEMINI_API_KEY=

GITHUB_TOKEN=
```

---

# 📊 Interview Flow

```
Candidate

↓

Profile Analysis

↓

Context Creation

↓

Voice Interview

↓

Speech Recognition

↓

Transcript Storage

↓

Gemini Evaluation

↓

Performance Report
```

---

# 🎯 Learning Outcomes

This project demonstrates experience with:

- Full Stack Development
- AI Engineering
- LLM Integration
- Voice AI
- WebRTC
- Backend APIs
- Database Design
- Prisma ORM
- Real-time Systems
- Prompt Engineering
- AI Evaluation Pipelines

---

# 🔮 Future Improvements

- Resume Upload
- Adaptive Interview Difficulty
- Coding Interview Support
- Recruiter Dashboard
- Candidate Dashboard
- AI Generated Interview Questions
- PDF Report Generation
- Email Notifications
- Multi-language Interviews
- Emotion Analysis
- Video Interview Support
- Interview Scheduling
- Authentication (Google & GitHub Login)

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

# 📄 License

This project is licensed under the MIT License.

---

# ⭐ Acknowledgements

This project leverages several powerful technologies and APIs:

- OpenAI Realtime API
- Google Gemini
- Deepgram
- React
- Bun
- Express
- Prisma
- PostgreSQL
- Tailwind CSS
- ShadCN UI

---

# 👨‍💻 Author

**Chetan D R**

If you found this project helpful, consider giving it a ⭐ on GitHub!
