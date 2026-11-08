# Repolex Knowledge Graph of canonical/prometheus-scrape-config-k8s-operator

RDF knowledge graph data for [canonical/prometheus-scrape-config-k8s-operator](https://github.com/canonical/prometheus-scrape-config-k8s-operator), parsed by [repolex](https://repolex.ai).

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
rlex download canonical/prometheus-scrape-config-k8s-operator
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── ab458e76d12fb6b231e9b0dc9aff7e827c77d354
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── ab458e76d12fb6b231e9b0dc9aff7e827c77d354
│           └── chunk-001.nq.gz
├── blob
│   ├── 015bec83b7fe26c99998ad7ec2d2bc8b86b3a976.nq.gz
│   ├── 0d8451addb3ab78f715423e10666212a54a454cd.nq.gz
│   ├── 14cd592e0466bfdd79dcf2003f3bf9310308a98a.nq.gz
│   ├── 1527248b125dabe30867ea3750b2a727c6797536.nq.gz
│   ├── 1bb45e9085b56696c3b53307f0da6268b4b3d16a.nq.gz
│   ├── 219793a0aa948e6766e7ef5ea130682b05755c83.nq.gz
│   ├── 222b54d6c97eb980ab500edb5df973ce38f986c8.nq.gz
│   ├── 261eeb9e9f8b2b4b0d119366dda99c6fd7d35c64.nq.gz
│   ├── 27b275189f81fa7ff104847505c9282999d0271e.nq.gz
│   ├── 35b58e91d0b00833c85d7d23ac07c0e131b70e05.nq.gz
│   ├── 3b67ae2244f23f5d1aff1726cab5fc473947a81f.nq.gz
│   ├── 48a8534d81da0b1dfd790e13a21ec42e053c33eb.nq.gz
│   ├── 534bd04a8fcaec68dbe40731dee7bea636e1c3fe.nq.gz
│   ├── 55969d643048afbcfabdfa8a3314e271294fff2f.nq.gz
│   ├── 5a7b3534ba9f58af4e93b052858a1fbc7003d782.nq.gz
│   ├── 652c7d218edf2dc1dcf39f46f745b352c2172801.nq.gz
│   ├── 6ccd559eabeae93e4d23215fa450130fa9b37ace.nq.gz
│   ├── 6f94cded4fec60283aa42d48789f2f779e32bb9a.nq.gz
│   ├── 701699edda5b6643d010a955d1e4e662a90a1ec3.nq.gz
│   ├── 7b8513e0333842532414b3c70e749c9c6acd2c00.nq.gz
│   ├── 7fa52ee9c9230fc16f9b4c97e5cb459c2449d04e.nq.gz
│   ├── 888c85583f72dc67ed997c9868566452e70cf898.nq.gz
│   ├── 8901c1d5711cc7644ca3be52ff6e2d238cf5a935.nq.gz
│   ├── 901f14351bdce339c3fcc6c3b3112c94e4fecb2f.nq.gz
│   ├── 94a7cecd707296e50764efed10cf57efcb76b77c.nq.gz
│   ├── 99e1e0c417d602f445bebbad9327af57837096a2.nq.gz
│   ├── 9f9dc042faa0c8decad8f35f0d8c739105261c75.nq.gz
│   ├── abcf006c16c149c0bf681cdb889aad44d7463bc5.nq.gz
│   ├── aff29f890a081dacb874528f6aa2e9edde9c581c.nq.gz
│   ├── b18eb1bcde711218ab39771c3d2f34a8502de6ce.nq.gz
│   ├── b2348b9fbfdc4eb154566c80f844510446be1d02.nq.gz
│   ├── bd7519d70b565e6b8f72b29783842a8a51ba3f3b.nq.gz
│   ├── c6e176df62768043b60ba33b7192f251db1f8151.nq.gz
│   ├── cc9c7a2281670ba58a85b296b9f7bd4307aa77db.nq.gz
│   ├── d45a3558ffaaedb3d9443b12370e8d7e9598ea2f.nq.gz
│   ├── db9aabbdd85880528169adeed3b25d4f09f75817.nq.gz
│   ├── de535d0f97c5fd103dfccb173b400b7e71461bd6.nq.gz
│   ├── deace15f5a3a2415250abaabd2e5e95951c29b26.nq.gz
│   └── f80ed2557e1fa0979c4cfb1bb2e84b77a8e9708f.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── ab458e76d12fb6b231e9b0dc9aff7e827c77d354.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 47 files
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

[canonical/prometheus-scrape-config-k8s-operator](https://github.com/canonical/prometheus-scrape-config-k8s-operator)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
