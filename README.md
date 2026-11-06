# Repolex Knowledge Graph of zopefoundation/zope.i18nmessageid

RDF knowledge graph data for [zopefoundation/zope.i18nmessageid](https://github.com/zopefoundation/zope.i18nmessageid), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download zopefoundation/zope.i18nmessageid
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── f4639e2995f0e048bfa1e041ec6f94a45f2e6659
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── f4639e2995f0e048bfa1e041ec6f94a45f2e6659
│           └── chunk-001.nq.gz
├── blob
│   ├── 05574907ee3d89e6256c358fd672009ea0344e0f.nq.gz
│   ├── 080decae9e00b4c48c95560ec1dd0bda48c1ca6c.nq.gz
│   ├── 1c457f635d21ef5e876c4123614bb52af7fa19a1.nq.gz
│   ├── 26ef81d7e710f66cc3f698e8de3516897c221e00.nq.gz
│   ├── 2b3833e27f8c3128147812df565912c4dbb07ca9.nq.gz
│   ├── 3bcc42844d643a3256ed59277f41df111ceadf04.nq.gz
│   ├── 55956dabad1a5bbd3f6219d911e78337e383b96c.nq.gz
│   ├── 59c8f80d58cac76177d60cf6c4c681f07ada3e40.nq.gz
│   ├── 688f156f72a9c05e1a153a20e8b6047b6d28dc4a.nq.gz
│   ├── 6cebe84d02234e33c00f732364f9f006fab1c5af.nq.gz
│   ├── 6dd78a9572ea97aad3e2885c6c00d11335f68361.nq.gz
│   ├── 6f7114bd366650ca37d324b0420ac840f346b5ce.nq.gz
│   ├── 70de7bfc7ecf1cf0b42b6582e03ea3bdedfefe83.nq.gz
│   ├── 77f3c744e601e8cdd746df3914bf9c9c8ea5365f.nq.gz
│   ├── 78609a5f5a06dd7d09bef2926810c672a193b0a1.nq.gz
│   ├── 78fac7be11976f98db2bdb4af4963285df13d7dd.nq.gz
│   ├── 792b113634ff94ab7eb02dfc35852c4550d9fcbb.nq.gz
│   ├── 9052d2b5ff1a12e6259fdd9694ab679c302614a0.nq.gz
│   ├── a4a38a1803b01f191c832128836e48861d4a3612.nq.gz
│   ├── ad73ebaea9d908b6bd1cf5f4e7e8916dac5e4b92.nq.gz
│   ├── b8581dd898cbb33e63961b4d181ff0ffbe5d03ee.nq.gz
│   ├── bab7f94be5ef86cce49612e6cdab326a57143d7d.nq.gz
│   ├── d4e2a749627b33135575d934277b746c848b3536.nq.gz
│   ├── de8fca92b02c2882a67f443a888b2f10a9721798.nq.gz
│   ├── dfa330d7329ea156bc1e3f47e36e605223107e17.nq.gz
│   ├── e1f9ad7b3b48377bfbfaa1b380c384ddea24060f.nq.gz
│   ├── e3d1f2a901eb6b73bd0f17e88c45a254d71cc56e.nq.gz
│   ├── e62eec2685820226d926dae3ba92518b526a522e.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e86bb0827e323a682b909b67cb9f905a58d95799.nq.gz
│   ├── fba2627a4edbe8639fc0ac832b3cbfcf59f3b577.nq.gz
│   ├── febdc0380a69c6f10efdb7678b8485e40013d8bf.nq.gz
│   └── ffee6a163301e8ce55668b2a9bbe412f51a594fd.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── f4639e2995f0e048bfa1e041ec6f94a45f2e6659.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 41 files
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
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[zopefoundation/zope.i18nmessageid](https://github.com/zopefoundation/zope.i18nmessageid)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
