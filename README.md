# NOVA — AI Personal Assistant

A cinematic, single-page AI chat assistant built with plain **HTML, CSS and JavaScript**. It talks to Large Language Models (LLMs) through their APIs using your own API key.

## Features
- Animated intro, starfield background and glowing colour orbs
- Switch between multiple models:
  - **Groq:** Llama 3.1 8B Instant, Llama 3.3 70B, GPT-OSS 120B
  - **Anthropic:** Claude Opus, Sonnet, Haiku
  - **OpenAI:** GPT-4o mini
  - **Google:** Gemini 2.5 Flash
  - Add any other model id yourself
- API Keys panel (Groq, OpenAI, Gemini, Anthropic, OpenRouter)
- Chat history sidebar, saved in your browser
- Typing animation, response time and Copy button
- Works on desktop and mobile

## How to run
1. Download or clone this repository.
2. Open `index.html` in Chrome (no install or server needed).
3. Click **🔑 API Keys**, paste your key (for example, a free Groq key from https://console.groq.com/keys) and press **Save**.
4. Click **🧠 Models**, pick a model and start chatting.

## How it works
1. You type a message.
2. JavaScript `fetch()` sends the message, the chat history and a **system prompt** to the chosen provider's API, with your API key.
3. The LLM returns a reply, which is shown with a typing effect.
4. The conversation is saved in the browser's `localStorage`, so the AI remembers context and your history stays after a refresh.

## Security note
API keys are **not** stored in this code. Each user enters their own key, which stays only in their browser. Never commit an API key to GitHub.

## Tech stack
HTML5 · CSS3 (glassmorphism, animations) · Vanilla JavaScript · LLM REST APIs

## Author
Aditya Singh Chauhan — CSE, IILM
