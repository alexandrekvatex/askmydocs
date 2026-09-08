# askmydocs

Minimal RAG over a folder of markdown notes, no vector DB

## How to use

```bash
python rag.py ./notes "how do I rotate logs?"
```

## Getting started

```bash
pip install -r requirements.txt
```

## Highlights

- Chunk markdown with overlap, keep source paths
- Prints sources with scores for transparency
- Swap in any LLM for the answer step
- TF-IDF retrieval: zero external services needed

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── data/
│   └── sample.md
├── docs/
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CONTRIBUTING.md
├── SECURITY.md
├── rag.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
