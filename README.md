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
│   │   ├── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae
│   │   │   └── chunk-001.nq.gz
│   │   └── c938db3f6ea262f5f087c75d8631c3aab9cbf0ad
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   ├── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae.nq.gz
│   │   └── c938db3f6ea262f5f087c75d8631c3aab9cbf0ad.nq.gz
│   └── repolex
│       ├── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae
│       │   └── chunk-001.nq.gz
│       └── c938db3f6ea262f5f087c75d8631c3aab9cbf0ad
│           └── chunk-001.nq.gz
├── blob
│   ├── 01f2a3b08d8c70b17701fdd1195fe2b244d41aa8.nq.gz
│   ├── 0aec4e63f467e4982024d1b66b4959ce6cec6514.nq.gz
│   ├── 0c3a0d6b4028154206b3bef49d0b2f007329b16a.nq.gz
│   ├── 0f55757d916807c17617833470d5565b2fd0c9fb.nq.gz
│   ├── 120be61b0740d16145164a31a63d2ae02850ad1e.nq.gz
│   ├── 16165276b611ec6b9adfeed65d7dba42ffd3138a.nq.gz
│   ├── 16e31575ba312399a16b2f1ffbb62228f33f165f.nq.gz
│   ├── 190904a6be871cb5b2a1eb45dda52c1ad634f274.nq.gz
│   ├── 1a3cd0416c9f1860986ca3f4f6a8107404be8ae9.nq.gz
│   ├── 1d2dafbbe58cd12b645e314d3ae4290f295a598b.nq.gz
│   ├── 1fe23ac07fb10d7ba8018616cecb23a6c0d80889.nq.gz
│   ├── 21b405d8c2dac873e9063b1dff87e46c3876aa58.nq.gz
│   ├── 24fd683602f4ec2383b3ad1e4c1e33a81e0c32ed.nq.gz
│   ├── 26fddfc4d462806cf5c098f0f7b77c7a88c6b7f7.nq.gz
│   ├── 29c38a9a6c58da8fa957babe0cceafa860024eca.nq.gz
│   ├── 2dc216c632a023a438c515f1d17942df08d03d69.nq.gz
│   ├── 2f4ae1eb049a490dc2ca68725e395932813a925e.nq.gz
│   ├── 318ee197eb3048a6e9778aa113dab9faf291f281.nq.gz
│   ├── 351b92c5a28f61c2990a8b8f361cd64df635c76f.nq.gz
│   ├── 354ff76790f4414a72861e92e29a217adecfed66.nq.gz
│   ├── 36b097ebda25728fa717025720ada7eb5bd4b56b.nq.gz
│   ├── 396fb047410ab0d5bc64841b06b475b745aae00d.nq.gz
│   ├── 3afcf8a6cdc1cac904f12c03e7bcb31a9f9501e0.nq.gz
│   ├── 3d129717ad00e9a800fe27cfc68b5e01aad29a6c.nq.gz
│   ├── 3e6d273c942b1ad5ac12e5c32315b4cd49ba131f.nq.gz
│   ├── 412136a41e1269a05bf60ea7df5a961a78c846e7.nq.gz
│   ├── 4d537b9b9338954724d7c34a64d630abdc61587b.nq.gz
│   ├── 4e9de49e44b172aae573cba0e8a64c3b2bfc4614.nq.gz
│   ├── 53386af00aad27cc6fdeabc4ad3e6227efad20ab.nq.gz
│   ├── 5a0eb0d2a1ef3b5b549e485e075ebcf31001a56b.nq.gz
│   ├── 638d6dd3d5a47b5a2eb4ca55a5c9150d3496adb4.nq.gz
│   ├── 673860fef9d73704e5eac9d77c6bde1f4036864e.nq.gz
│   ├── 68eb3d958ed71d0afe815b630a2a2a1f90ef4b99.nq.gz
│   ├── 6bc63498bb2b4ec3b8be65fa2c851aebad048e5c.nq.gz
│   ├── 784ed1a7daf9ff564fe8c297afc73d159a1160bd.nq.gz
│   ├── 7912b2e7b29e81c0e21026e0d95f99f44adc2674.nq.gz
│   ├── 8b3a76cc8b8f347af81a6fc7f3ae86e6164950ba.nq.gz
│   ├── 8e1efa701ade4472a6391338959b509635992020.nq.gz
│   ├── 8fb479f505037fde7976a4d933603a99c5aa7bdf.nq.gz
│   ├── 942b76f1fea77599f51a392f8fe61a9a45ea12cd.nq.gz
│   ├── 9683fb4d80758b75faa9e45cfa0a1e45ed39e9ac.nq.gz
│   ├── 9adfbfb12421b234f65e38e553c3758bbb002dbb.nq.gz
│   ├── a0891f563f38b0900eb12126983a36bafd2dcd03.nq.gz
│   ├── a264841a0bc7a1fd8f29812d45e35894203ebb66.nq.gz
│   ├── a6db7f019b78b6eb534fb32718467da502e99a22.nq.gz
│   ├── a6dfd673080a16a94c3499dc3e8e4ea52abb0cf6.nq.gz
│   ├── af3da677d89bdb9adaeef88557d4667b133eb8df.nq.gz
│   ├── b5dae7e2dbfb11bddd60c914b33a257f9301e243.nq.gz
│   ├── c2336342e2cd67e9c3022ecaa4788bb909039e77.nq.gz
│   ├── c76399e547beb2bd2a9899025f30d40fb1d4b4e1.nq.gz
│   ├── ca13063a2f15468b868b60646b3aaab53071b059.nq.gz
│   ├── ca21e22c2b7cca261ee376bfb6eb151a2877def0.nq.gz
│   ├── d222e8e858543b0b35e99bdcca6caf1ab8995473.nq.gz
│   ├── d4839a6b14c11e64143d1d200c2d4733595ffc6c.nq.gz
│   ├── dae8285b1ac06218a3af78b4d145bb3ee183f71d.nq.gz
│   ├── dd9623afc72fb6ed7bae4676a9a8d3bf68b7716e.nq.gz
│   ├── e227180450d50be2bd7a7ff3ba370e7d964687dc.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ea93bc4f2a679f4f7ff87060f4b9724c8b4b2f3c.nq.gz
│   ├── f0d3dfa5c184ed69aba01028bb2fa87245f489b0.nq.gz
│   ├── fb650ec1be29b005530f1dcf8391b357187f61a6.nq.gz
│   └── fcc4eddcfd3b5f47d3753f7e36a1e66ac08484a1.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   ├── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae.nq.gz
│   └── c938db3f6ea262f5f087c75d8631c3aab9cbf0ad.nq.gz
├── filetree
│   ├── 1f0a6343e9ba9aa487c3d4cc952ecf5d81483bae.nq.gz
│   └── c938db3f6ea262f5f087c75d8631c3aab9cbf0ad.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

17 directories, 77 files
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
