<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <img alt="Vonzlov / ai-engineer — Nikita Kozlov, AI engineer building LLM agents and RAG for real business processes" src="assets/header-light.svg" width="100%">
</picture>

<p align="right"><b>English</b> · <a href="README_RU.md">Русский</a></p>

I build LLM-powered tools that live inside real business processes: assistants embedded in the software people already use, workflows that take routine work off a team, and pipelines that turn plain text into finished documents.

## Model details

- **Developed by:** Nikita Kozlov
- **Model type:** AI engineer: LLM agents, RAG, process automation
- **Languages:** English, Russian

## Evaluation

### [pptx-telegram-bot](https://github.com/Vonzlov/pptx-telegram-bot) &nbsp; ![stable](https://img.shields.io/badge/status-stable-2ea44f?style=flat-square)

A team at another company asked for a free way to stop building PowerPoint decks by hand. You send the bot plain text in Telegram and get back a ready `.pptx` in the company's own template. The template mapping lives in a YAML file, with a helper script that builds that mapping for any corporate template, so swapping in a real template takes no code changes. Built as an MVP to prove the job can be done entirely on free, open-source software.

**Stack:** Python, aiogram, python-pptx, pydantic, optional local LLM via Ollama, Docker, pytest

### [llm-bench](https://github.com/Vonzlov/llm-bench) &nbsp; ![in development](https://img.shields.io/badge/status-in%20development-d29922?style=flat-square)

A benchmark service for choosing an LLM for a specific task. It runs the same task set against local models (Ollama, vLLM) and cloud APIs such as GigaChat, and compares the results side by side. Runs on k3s on a single machine, with compatibility with vanilla Kubernetes checked in CI on kind.

**Stack:** Python, Ollama, vLLM, cloud LLM APIs, k3s, kind, Docker

### [pqc-scout](https://github.com/Vonzlov/pqc-scout) &nbsp; ![early stage](https://img.shields.io/badge/status-early%20stage-8b949e?style=flat-square)

An assistant for migrating code to post-quantum cryptography: it looks for quantum-vulnerable algorithms in a codebase and helps plan their replacement.

**Stack:** Python, LLM

### Deployed in production (closed source)

**HR assistant in Outlook.** Three buttons on the Outlook ribbon: draft a reply to the selected email, rework a draft according to the user's comments, summarise a whole thread including meetings and attachments. Built in VBA on top of a corporate LLM, with fault tolerance as the first requirement: it should never crash on an unexpected item in the mailbox.

**n8n workflows** that send project members digests of their tasks, plus Excel and VBA tooling for monthly bonus calculations and KPI maps.

### Smaller experiments

A Telegram bot on n8n that collects vacancies from hh.ru and picks the ones that fit me. A Telegram bot that voices text through a third-party TTS API.

## Technical specifications

**Software.**

- **Languages:** Python, SQL, VBA
- **LLM:** Ollama, vLLM, OpenAI-compatible APIs, GigaChat, prompt engineering
- **Automation:** n8n, Telegram bots (aiogram), RPA (PIX), Bubble.io
- **Infrastructure:** Docker, k3s, Kubernetes (kind), Git, Linux

**Currently training on.** Fine-tuning and LoRA, MLOps.

**Hardware.** A desktop with an RTX 3060 and a MacBook. Local models stay small on purpose.

## Intended use

**Direct use.** Designing and shipping LLM assistants and agents that plug into existing tools: email, messengers, internal systems. Automating business processes end to end with Python, n8n, APIs and Docker. Choosing a model for a specific task and checking that choice with measurements rather than vibes.

**Out-of-scope use.** Training foundation models from scratch. I integrate, evaluate and ship models.

## Bias, risks and limitations

Strong bias toward simple, boring solutions: a straightforward script that the next person can read beats an elegant one they can't, even at the cost of some duplication. Asks what problem we are solving before writing any code.

## How to get started with the model

```python
from transformers import AutoEngineer

engineer = AutoEngineer.from_pretrained("Vonzlov/ai-engineer")
engineer.generate("Automate our monthly bonus calculation")
# → a working pipeline, a README in plain language and a short list of trade-offs
```

<!-- TODO: подставить свои ссылки, лишнее удалить -->
**Contact:** [LinkedIn](https://www.linkedin.com/in/YOUR-HANDLE) · [Telegram](https://t.me/YOUR-HANDLE) · [Email](mailto:YOUR-EMAIL)

## Citation

```bibtex
@misc{kozlov2026engineer,
  author = {Kozlov, Nikita},
  title  = {ai-engineer},
  year   = {2026},
  url    = {https://github.com/Vonzlov}
}
```
