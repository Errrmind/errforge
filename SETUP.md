# errforge — Quick Setup Guide

## 1. Clone & Start the Stack

```bash
git clone https://github.com/Errrmind/errforge.git
cd errforge
cp .env.example .env
# (Optional) Edit .env if you want custom ports or keys

docker compose up -d
```

## 2. Access Your Sovereign AI Brain

| Service          | URL                        | Purpose                          |
|------------------|----------------------------|----------------------------------|
| Open WebUI      | http://localhost:8080     | Chat with local LLMs            |
| AnythingLLM     | http://localhost:3001     | RAG collections + agents        |
| Qdrant          | http://localhost:6333     | Vector database dashboard       |
| N8N             | http://localhost:5678     | Workflow automation             |

## 3. Load Your First Skill

```bash
cd skills/errmind-dream-reprogrammer
python run.py --goal "Install the identity of a sovereign, execution-obsessed builder who ships daily"
```

Then import the generated `reprogramming_protocol_*.md` into AnythingLLM as a permanent collection.

## 4. Next Level (Recommended)

- Add Traefik + Authentik for secure remote access
- Connect AnythingLLM to your personal documents/Notion export
- Schedule recurring Errmind sessions via N8N
- Fork this repo and make it yours

**You now have a complete, local, sovereign AI + workflow system.**
No recurring costs. No data leaving your machine. Fully forkable.
