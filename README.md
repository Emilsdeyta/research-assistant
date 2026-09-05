\# research-assistant



Async, multi-source research assistant — queries Wikipedia, arXiv, and web search \*\*in parallel\*\*, then synthesizes a single citation-backed answer.



> This project is built as part of a Software Engineering Final Project (Topic 4 — Async Research Assistant). The AI module under `ai/` is provided as-is and will not be modified; this repo covers the surrounding software engineering layer (concurrency, caching, CLI, retries, logging, validation, tests, Docker).



\## Status



🚧 Project is under active development.



\## Setup



```bash

git clone https://github.com/Emilsdeyta/research-assistant.git

cd research-assistant



python -m venv .venv

source .venv/bin/activate      # Windows: .venv\\Scripts\\activate



pip install -r requirements.txt

cp .env.example .env

```



\## Project structure



research-assistant/

├── ai/ # provided, unchanged

├── src/

│ ├── services/

│ ├── core/

│ ├── concurrency/

│ └── storage/

├── tests/

├── data/

├── docs/

│ └── adr/

└── scripts/



\## Team



| Member | Role |

|---|---|

| Nural Shukurlu | Concurrency \& AI Integration — `src/concurrency/`, `src/services/ai\_service.py` |

| Mahammadali Babayev | Storage \& Data Modeling — `src/storage/`, `src/services/cache.py`, `src/models.py` |

| Emil Mammadov | CLI, Config \& Validation — `src/cli.py`, `src/config.py` |

| Baylar Bayramov | Testing \& DevOps — `tests/`, `Dockerfile`, `docs/architecture.md`, CI |





