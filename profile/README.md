<div align="center">
  <img width="1920" height="806" alt="shorekeeper" src="https://github.com/user-attachments/assets/e32b7bbc-8ae7-455c-9dfc-96675b9e3177" alt="Organization Banner" width="100%"/>

  <br />

  # 🌌 Project ShoreKeeper
  
  **A modular, open-source ecosystem enabling users to build, run, and interact with their own autonomous 2D AI VTuber/Companion.**
  *(Local & Cloud supported).*

  Inspired by *Neuro-sama* (Vedal) & *Project AIRI* & *Wuthering Waves*.

  <!-- [![Website](https://img.shields.io/badge/Website-shorekeeper.ai-000000?style=for-the-badge&logo=vercel)](https://shorekeeper.ai)
  [![Discord](https://img.shields.io/badge/Discord-Join_Community-7289da?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/yourlink)
  [![Twitter](https://img.shields.io/badge/Twitter-Follow_Us-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/yourhandle) -->
</div>

<br />

## 🏛️ System Architecture (The 4 Pillars)

The ecosystem is heavily modularized into 4 microservices/components to ensure plug-and-play capability:

### 1. 👁️ Sensory Inputs (The Senses)
- **Hearing:** Real-time Speech-to-Text (STT) running on-device (**Web Audio API** + **ONNX/Silero VAD** + **Whisper**).
- **Vision:** Computer vision module for screen-reading and game state analysis.
- **Reading:** Real-time Twitch/YouTube chat integration.

### 2. 🧠 Cognitive Core (The Brain)
- **LLM Router:** Prompt engineering and routing queries to local/cloud LLMs (**Llama 3, Qwen**) with character persona (System Prompts).
- **Memory Engine:** Short-term (context) and Long-term memory (**Vector Database**) for viewer recognition.

### 3. 🗣️ Expression Output (The Body & Voice)
- **Vocal Cords:** Text-to-Speech (TTS) with emotional embedding.
- **Body (Live2D):** Audio-based lip-sync and LLM-triggered facial expressions/animations.

### 4. ✋ Agentic Actions (The Hands)
- Autonomous macro/input simulation for playing games or executing computer tasks.

<br />

## 🛠️ Tech Stack Per Module

We strictly adhere to a decoupled architecture. Code is expected to be modular, well-typed (**TypeScript/Pydantic**), and highly optimized for real-time AI latency.

### 🌐 Frontend / Client UI
*Responsible for UI, local VAD, and WebGPU tasks.*
- **Core:** `React`, `Vite`, `TypeScript`
- **Styling & Components:** `TailwindCSS`, `Radix UI`
- **AI Models:** Hugging Face `transformers.js` (for web-based inference)

### ⚙️ Backend / Core Server
*Responsible for heavy AI inference, LLM routing, and Database management.*
- **Core:** `Python`, `FastAPI`

<div align="center">
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/ONNX-005CDB?style=for-the-badge&logo=onnx&logoColor=white" />
</div>

<br />

## 🤝 Contributing

This project is open-source, and we welcome all contributions from the community!
1. Please read our [Contributing Guidelines](.github/blob/main/CONTRIBUTING.md).
2. Look for issues labeled `good first issue` in our repositories to get started.
3. Join our Discord server to chat directly with the core development team.
