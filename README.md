# Repolex Knowledge Graph of jazzband/geojson

RDF knowledge graph data for [jazzband/geojson](https://github.com/jazzband/geojson), parsed by [repolex](https://repolex.ai).

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
rlex download jazzband/geojson
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 82055e8679bbcdef5bd7fc0a3c7168e86cbd3d12
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 82055e8679bbcdef5bd7fc0a3c7168e86cbd3d12
│           └── chunk-001.nq.gz
├── blob
│   ├── 05cadfd996ce39080bb467a37da71494e501bbe1.nq.gz
│   ├── 05ce9cdf179c521c62d89a93bc797aa8fb6339e9.nq.gz
│   ├── 0ecda8abe5324512295f1ae8b65e6c3b4f94874e.nq.gz
│   ├── 10f3c4993ff56b15f100e3b269aa3b6fb09ef7a5.nq.gz
│   ├── 1869c8925bbb8c4f5cecc15ffb32259d506384b3.nq.gz
│   ├── 19fc4a7224905171e6702b2279f491a27b22d341.nq.gz
│   ├── 1aeb8f5d58ccac49eeeebea5fddfab04fa8684d3.nq.gz
│   ├── 1c52ca5a9cf11e56bb2934d6f24c756fb016c792.nq.gz
│   ├── 1ceffbc127a62c7cd768138dc059b4488b869085.nq.gz
│   ├── 1e352a31423c77f8f39d8ca6d7008eeccfb9c3b1.nq.gz
│   ├── 218747d9cff22f7332cc82700d382cff2890bb3d.nq.gz
│   ├── 24072911362a9e14efd6db18d2ec685c251676bb.nq.gz
│   ├── 380f4a2e222c5a4d292f804af21fcf79933196c3.nq.gz
│   ├── 41e3f5015f66f41ae0dc8ccd1b69678366ffba6f.nq.gz
│   ├── 468661a62ab42816db99e5405f53a1a9177ed233.nq.gz
│   ├── 4a028476b3148588e823ca6a9fdffb4afe4272e0.nq.gz
│   ├── 50d6b0f7dbd70da902ddf967f76576112c140e87.nq.gz
│   ├── 5339cb830912103abe131ff40574e8fd82b64547.nq.gz
│   ├── 54c6d8e7179d2d4902b94bafde2f6f90f6848c73.nq.gz
│   ├── 5d90cac0e903755ff2ccbe3f49261d1aff0f95be.nq.gz
│   ├── 5f0616cfbca1a0a2fd9333f9d90f0c08047dd085.nq.gz
│   ├── 61c55d6c1d2d11d394b4dd189221a3582d8f1046.nq.gz
│   ├── 77477e3e71d95eaf94f36733ddd0acdfb56b0009.nq.gz
│   ├── 7da1f9608ee1595463f3aefec0e087e57ca6c49f.nq.gz
│   ├── 84a1ff66a666d1b81e37b8c3d78743761c335de5.nq.gz
│   ├── a8dd939b849e9042f89233a2a57924fb04779840.nq.gz
│   ├── aa8618f9bf2b9289c88197c810a81093c6f70b22.nq.gz
│   ├── c4578fd84c0c9fde42ec5d6426360415843de49f.nq.gz
│   ├── ca8255a70e5970ea254269748fb8cd87cd211d79.nq.gz
│   ├── d0cc47b94eeb62a456c8bbc7ca9367b5ad20aad4.nq.gz
│   ├── d6cef8ee8a259f25f66c97511fed298ccb27be65.nq.gz
│   ├── da2e23ac57df54bcbac793b379d4c451ae0f2f87.nq.gz
│   ├── e0d5efab56fb94577e7804603eb6f21f36977cb2.nq.gz
│   ├── e262438389c44f9f7982ac5faf3fba2225c1f8d9.nq.gz
│   ├── e30fd22de423f6584424ce49b6dcbdb7d0ca89f4.nq.gz
│   ├── e6f96a11f592176b0eb2b7641fa2820ab809fa71.nq.gz
│   ├── ee8dffcfa9568d457cecc429970ee00cfb151b10.nq.gz
│   ├── f17be533f25f2da8b6563a07a04ca80042d510ca.nq.gz
│   ├── f363d8723c6b05b400023741ba728c4438c4d390.nq.gz
│   ├── fc3af324a4ec2b5fc548aa6d22de7eb54bfda44a.nq.gz
│   └── fed528d4a7a148fd0bf0b0198a6461f8c91b87e9.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 82055e8679bbcdef5bd7fc0a3c7168e86cbd3d12.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
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

[jazzband/geojson](https://github.com/jazzband/geojson)

---
*Parsed on 2026-10-10 by [repolex](https://repolex.ai)*
