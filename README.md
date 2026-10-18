# Repolex Knowledge Graph of adamchainz/django-browser-reload

RDF knowledge graph data for [adamchainz/django-browser-reload](https://github.com/adamchainz/django-browser-reload), parsed by [repolex](https://repolex.ai).

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
rlex download adamchainz/django-browser-reload
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 9e07824fe16e413fccf4078bd8d5e68b75a553c7
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 9e07824fe16e413fccf4078bd8d5e68b75a553c7
│           └── chunk-001.nq.gz
├── blob
│   ├── 00b77d4b6ad0fe8d25160d56f9a6e3df665e874c.nq.gz
│   ├── 03bc6a98f04e033d55c912fd935ff31f481861a4.nq.gz
│   ├── 0699ce339a81fed412cbafb6c7544ed62d1468bc.nq.gz
│   ├── 0d944831505484f3ec48221ad50d804afa07ac65.nq.gz
│   ├── 17f2360b0f716394649e6e02b5ba22c51fc40fd8.nq.gz
│   ├── 205ab9ad9df4ab629d1b7b8d8a72b41f44d8824c.nq.gz
│   ├── 20819b4d1eed8cdd0b95e0a95a2e86650b827361.nq.gz
│   ├── 22778a85d4459d741572065b2475bc14284dfc61.nq.gz
│   ├── 22ddbb118475b52ce8ecba56d9ec45009923da58.nq.gz
│   ├── 2347410ca4ebab6df18650e89d5b7d27051c0f8f.nq.gz
│   ├── 25a6eb4e5ab8bd0914309b62e6a7cc3d594e1cfa.nq.gz
│   ├── 25c337ae32ab36ebe2c1e6304e2f1bab1c6bc3f1.nq.gz
│   ├── 2a7f84f54867d02714727f82eef95d3be939d666.nq.gz
│   ├── 303b877dd39adb64a44ee8ef045395d8349c2294.nq.gz
│   ├── 3ba13e0cec6cbbfd462e9ebf529dd2093148cd69.nq.gz
│   ├── 40f4ac757715bb1a8c355eda9124141fdda3aeff.nq.gz
│   ├── 49a97e7d84c244231a7781b721dcea338aa65d90.nq.gz
│   ├── 4b59632c82219f385b39b9b0a82e1c786cdbbec7.nq.gz
│   ├── 528885ca34e76e518e5e98be37251aedceff7e34.nq.gz
│   ├── 586337e8c666f0552e8845b626e0e9d01e0ec12d.nq.gz
│   ├── 599ca4da39c9927e4c03712f35bd067626bdd7cd.nq.gz
│   ├── 6468c53459df00eee147711fb5ae4351d74c9bc5.nq.gz
│   ├── 7f1d007c01048570d774e58f46203d3e92056c39.nq.gz
│   ├── 8516bae48d799208c5c1d1f7491fcc8aa9134344.nq.gz
│   ├── 8e62c9fa5583994ce153cb9644385a98c5f5c27e.nq.gz
│   ├── 929599134d369fcb24dab0f291061788d362107a.nq.gz
│   ├── 9f5118c27bba265cb7f6113e0822269943aa5ca8.nq.gz
│   ├── b21d4e8c5234bcb3a59eea843209bf9e19f99ce4.nq.gz
│   ├── b541c276855fdb05d8bb2b987a963b3437c86a76.nq.gz
│   ├── b638205d7dd93c32b6168965762c172b04e48f37.nq.gz
│   ├── bbb05c38fdfe87ac9174563834f8be12495ec62f.nq.gz
│   ├── bf83742411e2d552e008a79d521c10a63cb7241b.nq.gz
│   ├── c02f5b9da2d4799de8a9aebf10312034e599825b.nq.gz
│   ├── c45c6e23c85e58e8f6b171765b6c4120411e0427.nq.gz
│   ├── cda834ad15fa8f7fbd1778c2e326b24ee29cbca5.nq.gz
│   ├── de6bd5b0999d1983609ee3d04589c460e750f65d.nq.gz
│   ├── e191c4e8545fceb522276a61af1a7e7a743a104e.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── fe3a19c05f3ba3278ffec155c10052c84ac040b7.nq.gz
│   └── ff68a8b9a05992035ea0ec28e2b04e995ec7758d.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 9e07824fe16e413fccf4078bd8d5e68b75a553c7.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
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

[adamchainz/django-browser-reload](https://github.com/adamchainz/django-browser-reload)

---
*Parsed on 2026-10-18 by [repolex](https://repolex.ai)*
