# AI Apps & Learnings

![AI Banner](https://images.unsplash.com/photo-1677442136019-21780ecad995?auto=format&fit=crop&q=80&w=1600)  
*(A collection of my AI experiments, projects, and key learnings — built with curiosity and fast inference)*

Welcome to my personal AI playground!  
This repository is a living collection of **AI-powered projects**, prototypes, and notes as I explore modern AI tools, APIs, LLMs, and deployment patterns.

**Goal**: Document everything I build and learn — from simple fun apps to more advanced agents, RAG, fine-tuning experiments, and serverless AI deployments.

## First Project: Instant AI Welcome

**Live Demo** : [https://ai-apps-instant.vercel.app](https://instant-pcupe9qkv-kays-projects-0b9c80ce.vercel.app/)

This is a lightweight, **fully serverless** web app that greets every visitor with a **unique, enthusiastic, AI-generated welcome message**.

### Features
- Connects securely to the **Groq API** (super-fast LLM inference)
- Uses your Groq API key (stored as environment variable — never hard-coded!)
- Generates creative, personalized welcome messages via chat completion
- Returns clean, styled **HTML** responses
- Built to run entirely on **Vercel** (serverless functions + static hosting)
- Minimal dependencies, blazing fast cold starts thanks to Groq

### Tech Stack
- **Backend**: Python + Groq SDK (or OpenAI-compatible client)
- **Frontend**: Simple HTML + minimal CSS (served from Vercel)
- **API**: Groq (`llama-3.1-8b-instant` or similar fast model)
- **Deployment**: Vercel (serverless functions at `/api/welcome`)
- **No database** — purely stateless & edge-friendly
