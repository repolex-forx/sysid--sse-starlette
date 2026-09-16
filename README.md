# Repolex Knowledge Graph of sysid/sse-starlette

RDF knowledge graph data for [sysid/sse-starlette](https://github.com/sysid/sse-starlette), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download sysid/sse-starlette
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae.nq.gz
│   └── repolex
│       └── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae
│           └── chunk-001.nq.gz
├── blob
│   ├── 01f2a3b08d8c70b17701fdd1195fe2b244d41aa8.nq.gz
│   ├── 0f55757d916807c17617833470d5565b2fd0c9fb.nq.gz
│   ├── 120be61b0740d16145164a31a63d2ae02850ad1e.nq.gz
│   ├── 16e31575ba312399a16b2f1ffbb62228f33f165f.nq.gz
│   ├── 1a3cd0416c9f1860986ca3f4f6a8107404be8ae9.nq.gz
│   ├── 21b405d8c2dac873e9063b1dff87e46c3876aa58.nq.gz
│   ├── 24fd683602f4ec2383b3ad1e4c1e33a81e0c32ed.nq.gz
│   ├── 29c38a9a6c58da8fa957babe0cceafa860024eca.nq.gz
│   ├── 3d129717ad00e9a800fe27cfc68b5e01aad29a6c.nq.gz
│   ├── 6bc63498bb2b4ec3b8be65fa2c851aebad048e5c.nq.gz
│   ├── 784ed1a7daf9ff564fe8c297afc73d159a1160bd.nq.gz
│   ├── a6db7f019b78b6eb534fb32718467da502e99a22.nq.gz
│   ├── af3da677d89bdb9adaeef88557d4667b133eb8df.nq.gz
│   ├── c2336342e2cd67e9c3022ecaa4788bb909039e77.nq.gz
│   ├── ca13063a2f15468b868b60646b3aaab53071b059.nq.gz
│   ├── d222e8e858543b0b35e99bdcca6caf1ab8995473.nq.gz
│   ├── ea93bc4f2a679f4f7ff87060f4b9724c8b4b2f3c.nq.gz
│   ├── fb650ec1be29b005530f1dcf8391b357187f61a6.nq.gz
│   └── fcc4eddcfd3b5f47d3753f7e36a1e66ac08484a1.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae.nq.gz
├── filetree
│   └── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 29 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |

## Source repository

[sysid/sse-starlette](https://github.com/sysid/sse-starlette)

---
*Parsed on 2026-09-16 by [repolex](https://repolex.ai)*
