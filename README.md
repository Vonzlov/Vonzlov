<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Nikita Kozlov — AI engineer building LLM agents and RAG for real business processes" src="assets/header-light.svg" width="100%">
</picture>

<p align="right"><b>English</b> · <a href="README_RU.md">Русский</a></p>

I build LLM-powered tools for real business processes: assistants inside the software people already use, automation of routine work and pipelines that turn plain text into finished documents.

## Projects

### [pptx-telegram-bot](https://github.com/Vonzlov/pptx-telegram-bot) &nbsp; ![stable](https://img.shields.io/badge/status-stable-2ea44f?style=flat-square)

Telegram bot that turns plain text into a ready `.pptx` deck in a corporate template. Any template is plugged in through a YAML config, without code changes.

**Stack:** Python, aiogram, python-pptx, pydantic, Ollama (optional), Docker, pytest

### [llm-bench](https://github.com/Vonzlov/llm-bench) &nbsp; ![in development](https://img.shields.io/badge/status-in%20development-d29922?style=flat-square)

Benchmark service for choosing an LLM for a specific task: runs the same task set through local models and cloud APIs and compares the results.

**Stack:** Python, Ollama, vLLM, cloud LLM APIs, Docker, k3s, kind

### [pqc-scout](https://github.com/Vonzlov/pqc-scout) &nbsp; ![early stage](https://img.shields.io/badge/status-early%20stage-8b949e?style=flat-square)

Assistant for migrating code to post-quantum cryptography: finds quantum-vulnerable algorithms in a codebase and helps plan their replacement.

**Stack:** Python, LLM

### Work projects (closed source)

**HR assistant in Outlook.** Three ribbon buttons: draft a reply to the selected email, revise a draft from the user's comments, summarise a whole thread. VBA on top of a corporate LLM API.

**Process automation.** n8n workflows that send project members digests of their tasks, and VBA macros for monthly bonus calculations and KPI maps.

### Smaller projects

**Vacancy matcher.** Telegram bot on n8n that collects vacancies from hh.ru and picks the ones that match my profile.

**Text-to-speech bot.** Telegram bot that voices text through a third-party TTS API.

## Stack

- **Languages:** Python, JavaScript, SQL, VBA
- **LLM:** OpenAI-compatible APIs, Ollama, vLLM, LLM agents, RAG, prompt engineering, LLM evaluation
- **Automation:** n8n, Telegram bots (aiogram), RPA (PIX), Bubble.io
- **Infrastructure:** Docker, k3s, Kubernetes (kind), Git, Linux

## How I work

- **Simplicity over elegance.** Straightforward code that the next person can read and maintain, even at the cost of some duplication.
- **Reliability first.** A tool embedded in someone's workflow doesn't crash on unexpected input: anything it can't handle gets skipped or flagged.
- **Measure, then choose.** I pick a model by testing it on the actual task, not by its reputation.

## Contact

<!-- TODO: подставить свои ссылки, лишнее удалить -->
[LinkedIn](https://www.linkedin.com/in/YOUR-HANDLE) · [Telegram](https://t.me/YOUR-HANDLE) · [Email](mailto:YOUR-EMAIL)
