# CODEQL PRIOR DOCS

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-software_development-lightgrey)

> Anticloud-hardened packaging of the upstream project `CODEQL_PRIOR_DOCS` in category **SOFTWARE DEVELOPMENT**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SOFTWARE DEVELOPMENT · **Upstream:** https://github.com/github/codeql · **Upstream pin:** `4f40d241e9891bf397f48cbfc1084490773c3cc5` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# CodeQL

This open source project contains the standard CodeQL libraries and queries that power [GitHub Advanced Security](https://github.com/features/security/code) and the other application security products that [GitHub](https://github.com/features/security/) makes available to its customers worldwide.

## How do I learn CodeQL and run queries?

There is extensive documentation about the [CodeQL language](https://codeql.github.com/docs/), writing CodeQL using the [CodeQL extension for Visual Studio Code](https://docs.github.com/en/code-security/codeql-for-vs-code/) and using the [CodeQL CLI](https://docs.github.com/en/code-security/codeql-cli).

## Contributing

We welcome contributions to our standard library and standard checks. Do you have an idea for a new check, or how to improve an existing query? Then please go ahead and open a pull request! Before you do, though, please take the time to read our [contributing guidelines](CONTRIBUTING.md). You can also consult our [style guides](https://github.com/github/codeql/tree/main/docs) to learn how to format your code for consistency and clarity, how to write query metadata, and how to write query help documentation for your query.

For information on contributing to CodeQL documentation, see the "[contributing guide](docs/codeql/CONTRIBUTING.md)" for docs.

## License

The code in this project is licensed under the [MIT License](LICENSE) by [GitHub](https://github.com).

The CodeQL CLI (including the CodeQL engine) is hosted in a [different project](https://github.com/github/codeql-cli-binaries) and is [licensed separately](https://github.com/github/codeql-cli-binaries/blob/main/LICENSE.md). If you'd like to use the CodeQL CLI to analyze closed-source code, you will need a separate commercial license; please [contact us](https://github.com/enterprise/contact) for further help.

## Visual Studio Code integration

If you use Visual Studio Code to work in this project, there are a few integration features to make development easier.

### CodeQL for Visual Studio Code

You can install the [CodeQL for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-codeql) extension to get syntax highlighting, IntelliSense, and code navigation for the QL language, as well as unit test support for testing CodeQL libraries and queries.

### Tasks

The `.vscode/tasks.json` file defines custom tasks specific to working in this project. To invoke one of these tasks, select the `Terminal | Run Task...` menu option, and then select the desired task from the dropdown. You can also invoke the `Tasks: Run Task` command from the command palette.

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Rust / Cargo** (manifests: Cargo.toml, Cargo.lock; scanned in UPSTREAM_CLONE)
- Top-level source layout: `actions/`, `change-notes/`, `config/`, `cpp/`, `csharp/`, `go/`, `java/`, `javascript/`, `misc/`, `python/`, `ql/`, `ruby/`
- Snapshot size: **58213 files**, **1201502 lines of code** (measured; see Benchmarks)
- Primary languages: `.java` (8198), `.ql` (7705), `.expected` (6851), `.qll` (5675), `.md` (4611), `.js` (2731)
- Upstream commit pinned for this packaging: `4f40d241e9891bf397f48cbfc1084490773c3cc5`

---

## Installation

No installation section was found in the upstream readme, so the commands below are generated from the manifests detected in this project directory.

```sh
cargo build --release
```

Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

```sh
cargo run --release
```

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `CODEQL_PRIOR_DOCS` source tree vendored in `UPSTREAM_CLONE/` (Rust / Cargo ecosystem). Public entry points:

- Source modules: `actions/`, `change-notes/`, `config/`, `cpp/`, `csharp/`, `go/`, `java/`, `javascript/`
- The snapshot declares 1066 dependency references across 4 ecosystem(s); see Dependencies below.
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Rust / Cargo |
| Manifests detected | Cargo.toml, Cargo.lock |
| Files in snapshot | 58213 |
| Lines of code | 1201502 |
| Dependency references | 1066 |
| Dependencies by ecosystem | cargo: 223, go: 699, npm: 143, pypi: 1 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| cargo | resolver | 2 | Cargo.toml |
| cargo | name | swift-syntax-rs | unified/swift-syntax-rs/Cargo.toml |
| cargo | description | Rust wrapper around the swift-syntax package for parsing Swift source | unified/swift-syntax-rs/Cargo.toml |
| cargo | version | 0.1.0 | unified/swift-syntax-rs/Cargo.toml |
| cargo | edition | 2024 | unified/swift-syntax-rs/Cargo.toml |
| cargo | links | SwiftSyntaxFFI | unified/swift-syntax-rs/Cargo.toml |
| cargo | name | swift_syntax_rs | unified/swift-syntax-rs/Cargo.toml |
| cargo | path | src/lib.rs | unified/swift-syntax-rs/Cargo.toml |
| cargo | name | swift-syntax-parse | unified/swift-syntax-rs/Cargo.toml |
| cargo | path | src/main.rs | unified/swift-syntax-rs/Cargo.toml |
| cargo | name | codeql-extractor-unified-unsupported-os | unified/extractor-unsupported-os/Cargo.toml |
| cargo | description | Fallback executable for unsupported CodeQL Unified extractor platforms | unified/extractor-unsupported-os/Cargo.toml |
| cargo | version | 0.1.0 | unified/extractor-unsupported-os/Cargo.toml |
| cargo | edition | 2024 | unified/extractor-unsupported-os/Cargo.toml |
| cargo | name | codeql-extractor-unified | unified/extractor/Cargo.toml |
| ... | (485 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `Cargo.toml`
- `config`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing to CodeQL

We welcome contributions to our CodeQL libraries and queries. Got an idea for a new check, or how to improve an existing query? Then please go ahead and open a pull request! Contributions to this project are [released](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-project-license) to the public under the [project's open source license](LICENSE).

There is lots of useful documentation to help you write queries, ranging from information about query file structure to tutorials for specific target languages. For more information on the documentation available, see [CodeQL queries](https://codeql.github.com/docs/writing-codeql-queries/codeql-queries) on [codeql.github.com](https://codeql.github.com).

Note that the CodeQL for Visual Studio Code documentation has been migrated to https://docs.github.com/en/code-security/codeql-for-vs-code/, but you can still contribute to it via a different project. For more information, see [Contributing to GitHub Docs documentation](https://docs.github.com/en/contributing)."

## Change notes

Any nontrivial user-visible change to a query pack or library pack should have a change note. For details on how to add a change note for your change, see [this guide](docs/change-notes.md).

## Submitting a new experimental query

If you have an idea for a query that you would like to share with other CodeQL users, please open a pull request to add it to this project. New queries start out in a `<language>/ql/src/experimental` directory, to which they can be merged when they meet the following requirements.

1. **Directory structure**

    There are ten language-specific query directories in this project:

      * Actions: `actions/ql/src`
      * C/C++: `cpp/ql/src`
      * C#: `csharp/ql/src`
      * Go: `go/ql/src`
      * Java/Kotlin: `java/ql/src`
      * JavaScript: `javascript/ql/src`
      * Python: `python/ql/src`
      * Ruby: `ruby/ql/src`
      * Rust: `rust/ql/src`
      * Swift: `swift/ql/src`

    Each language-specific directory contains further subdirectories that group queries based on their `@tags` or purpose.
    - Experimental queries and libraries are stored in the `experimental` subdirectory within each language-specific directory in the [CodeQL project](https://github.com/github/codeql). For example, experimental Java queries and libraries are stored in `java/ql/src/experimental` and any corresponding tests in `java/ql/test/experimental`.
 

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
MIT License

Copyright (c) 2006-2025 GitHub, Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `CODEQL_PRIOR_DOCS` (category: SOFTWARE DEVELOPMENT)
- **Upstream URL:** https://github.com/github/codeql
- **Pinned commit (SHA):** `4f40d241e9891bf397f48cbfc1084490773c3cc5`
- **Branch:** main
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`115a2da9e24a1781c0e6013e7c900ff4621e43b4b4f009350eb4c2de740f755c`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

