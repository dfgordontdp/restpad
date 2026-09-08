# restpad

Small bookmark service with search and tags

Started as a weekend hack, grew on me.

## Getting started

```bash
npm install
npm run dev
```

## Usage

```bash
curl -X POST localhost:3000/api/bookmarks \
  -H 'content-type: application/json' \
  -d '{"url": "https://example.com", "tags": ["reading"]}'
```

## Highlights

- In-memory store with optional JSON persistence
- Request validation helpers, no framework magic
- env-driven port, runs anywhere Node does
- REST endpoints: list / create / delete / search
- Morgan logging and centralized error handler

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   ├── faq.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── src/
│   ├── config.js
│   ├── index.js
│   └── store.js
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
└── package.json
```
