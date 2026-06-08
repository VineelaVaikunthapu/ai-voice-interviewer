# AI Avatar Interviewer

A voice AI interviewer built with Python, LangGraph, and LiveKit featuring real-time voice interaction and a RAG pipeline for company knowledge.

## Features
- 🎙️ Real-time voice conversation using LiveKit
- 🧠 Structured interview flow powered by LangGraph
- 📄 Company knowledge base using RAG (PDF + ChromaDB)
- 🗣️ Speech-to-text via Deepgram
- 💬 LLM responses via OpenAI GPT-4o
- 🔊 Text-to-speech via Cartesia

## Tech Stack
- Python
- LangGraph
- LiveKit Agents
- Deepgram (STT)
- OpenAI (LLM)
- Cartesia (TTS)
- ChromaDB (Vector Store)

## Setup

1. Install uv
2. Install dependencies:
   uv add "livekit-agents[deepgram,openai,cartesia,silero,turn-detector]~=1.2"
3. Add your API keys to .env.local
4. Place TechCompanyInfo.pdf in the project folder
5. Run the agent:
   uv run agent.py console