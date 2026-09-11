# llm-meter

Estimate LLM cost of a file before you send it

## Install

```bash
# stdlib only
```

## Features

- Zero dependencies
- Per-model pricing table in JSON
- Heuristic token estimate (~4 chars/token)
- Reports input/output tokens and USD estimate

## How to use

```bash
python cost.py prompt.txt --model gpt-4o-mini --expect-out 500
```

## Project structure

```text
├── .github/
│   ├── workflows/
│   │   └── ci.yml
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   ├── development.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── SECURITY.md
├── cost.py
└── pricing.json
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## 说明

个人练习项目, 谨慎用于生产环境。
