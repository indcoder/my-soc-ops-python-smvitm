🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎉 Soc Ops

> A fast, fun social bingo app for in-person mixers.

Get people talking in minutes: each player gets a bingo board of conversation prompts, then finds people in the room who match each square. First to 5 in a row wins.

## ✨ Why this project

- **Breaks the ice quickly** in classes, workshops, and team events
- **Simple game loop**: start game → mingle → mark matches → celebrate bingo
- **Built for learning** with a practical FastAPI + Jinja reference app

## 🕹️ How it works

1. Start a new game session
2. Walk around and meet people
3. Mark squares as you find matching participants
4. Hit bingo with 5 in a row
5. Reset and play again

## 🚀 Quick start

```bash
python -m pip install fastapi itsdangerous jinja2 "uvicorn[standard]"
python -m uvicorn app.main:app --reload
```

Then open: http://127.0.0.1:8000

## 🧱 Tech stack

- Python + FastAPI
- Server-rendered Jinja templates
- Session-based game state
- Lightweight frontend (HTML + CSS + HTMX patterns)

---

## 📚 Lab guide

| Part | Title |
|------|-------|
| [**00**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=00-overview) | Overview & Checklist |
| [**01**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=01-setup) | Setup & Context Engineering |
| [**02**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=02-design) | Design-First Frontend |
| [**03**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [**04**](https://copilot-dev-days.github.io/agent-lab-python/docs/step.html?step=04-multi-agent) | Multi-Agent Development |

> 📝 Lab guides are also available in [`workshop/`](workshop/) for offline reading.
