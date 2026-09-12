# ft-data-prep

Clean and split JSONL datasets for fine-tuning

Small but I use it weekly.

## Features

- Dedup by normalized instruction text
- Prints a stats summary you can eyeball
- Deterministic split with a seed
- Length filters keep the sweet spot

## How to use

```bash
python prep.py raw.jsonl --out-dir data/ --valid-ratio 0.1
```

## Getting started

```bash
# stdlib only
```

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── LICENSE
└── prep.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Why

Needed this for myself; figured others might too.

## License

MIT - see [LICENSE](LICENSE).
