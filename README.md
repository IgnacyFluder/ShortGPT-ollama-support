
# ShortGPT - Ollama & Groq Support Fork

This is a fork of [ShortGPT](https://github.com/ShortGPT/ShortGPT)](https://github.com/RayVentura/ShortGPT). enhanced with support for:

- [ ] **Ollama** – Run local LLMs on your machine using the Ollama runtime.
- [ ] **Groq** – Use the ultra-fast Groq Cloud API to run open-source LLMs like Mixtral or LLaMA.
- [x] **OpenAI** – (existing support)
- [x] **Gemini** – Google’s powerful LLM (if API key is present)

Repo: [IgnacyFluder/ShortGPT-ollama-support](https://github.com/IgnacyFluder/ShortGPT-ollama-support)

This fork prioritizes flexibility and modularity by detecting available API keys and choosing the most capable LLM backend automatically.

---

## LLM Backend Priority

The system selects which LLM backend to use in this order:

1. **Gemini** (Google) – if `GEMINI_API_KEY` is set
2. **OpenAI** – if `OPENAI_API_KEY` is set
3. **Groq** – if `GROQ_API_KEY` is set
4. **Ollama** – fallback if no cloud keys are present

> No configuration required — the backend is selected based on available environment variables.

---

## Features

- AI-powered video creation from text prompts
- Modular LLM support
  - [x] Gemini
  - [x] OpenAI
  - [ ] Groq
  - [ ] Ollama
- Script generation, voiceovers, image generation, video compilation
- Local and cloud-based execution options

---

## Setup Instructions

### Prerequisites

- Python 3.9+
- `ffmpeg` installed
- One of the following: API keys for Gemini, OpenAI, Groq or [Ollama](https://ollama.com/) installed

---

## Installation

```bash
git clone https://github.com/IgnacyFluder/ShortGPT-ollama-support
cd ShortGPT-ollama-support
pip install -r requirements.txt
