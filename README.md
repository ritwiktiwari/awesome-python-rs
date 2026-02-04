# Awesome Python Rust [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of Python tools, libraries, and frameworks with Rust under the hood.

## Contents

- [Why Rust for Python](#why-rust-for-python)
- [Arrow & Columnar Data](#arrow--columnar-data)
- [Bioinformatics & Astronomy](#bioinformatics--astronomy)
- [Cloud Storage](#cloud-storage)
- [Cryptography & Hashing](#cryptography--hashing)
- [Data Processing & DataFrames](#data-processing--dataframes)
- [Date & Time](#date--time)
- [Data Structures](#data-structures)
- [File Watching & System Utilities](#file-watching--system-utilities)
- [Finance](#finance)
- [Geospatial](#geospatial)
- [Graph Libraries](#graph-libraries)
- [HTTP Clients](#http-clients)
- [Linting, Formatting & Type Checking](#linting-formatting--type-checking)
- [Miscellaneous](#miscellaneous)
- [Package Management & Tooling](#package-management--tooling)
- [Rust-Python Interop](#rust-python-interop)
- [Scientific Computing](#scientific-computing)
- [Search & Indexing](#search--indexing)
- [Serialization & Parsing](#serialization--parsing)
- [Tokenization & ML](#tokenization--ml)
- [Validation & Data Modeling](#validation--data-modeling)
- [Visualization](#visualization)
- [Web Frameworks & Servers](#web-frameworks--servers)
- [Web Scraping & HTML](#web-scraping--html)

## Why Rust for Python

Python's flexibility makes it ideal for rapid development, but computationally intensive operations can become bottlenecks. Rust provides memory safety without garbage collection overhead, zero-cost abstractions, and safe concurrency—making it increasingly popular for implementing performance-critical Python components.

This list tracks the growing movement of Python projects leveraging Rust for their performance-critical components.

---

## Arrow & Columnar Data

- [arro3](https://github.com/kylebarron/arro3) - A minimal Python library for Apache Arrow, binding to the Rust Arrow crate.

## Bioinformatics & Astronomy

- [bed-reader](https://github.com/fastlmm/bed-reader) - Read and write the PLINK BED format, simply and efficiently.
- [haem](https://github.com/BooleanCat/haem) - A Python library for working on bioinformatics problems.
- [mocpy](https://github.com/cds-astro/mocpy) - Astronomical Python library for describing coverage regions on the unit sphere.

## Cloud Storage

- [obstore](https://github.com/developmentseed/obstore) - High-throughput Python interface to S3, GCS, and Azure Storage.
- [opendal](https://github.com/apache/opendal) - Apache OpenDAL: unified data access layer for all storage services.

## Cryptography & Hashing

- [cryptography](https://github.com/pyca/cryptography) - The standard Python cryptographic library, with performance-critical parts in Rust.
- [blake3-py](https://github.com/oconnor663/blake3-py) - Python bindings for the BLAKE3 cryptographic hash function.
- [johnnycanencrypt](https://github.com/kushaldas/johnnycanencrypt) - OpenPGP library with Yubikey support.

## Data Processing & DataFrames

- [polars](https://github.com/pola-rs/polars) - Blazingly fast DataFrame library with lazy evaluation and parallel execution. Often 5-10x faster than Pandas with significantly lower memory usage.
- [datafusion-python](https://github.com/apache/datafusion-python) - Python bindings for Apache DataFusion, an in-memory query engine.
- [delta-rs](https://github.com/delta-io/delta-rs) - Native Rust library for Delta Lake with Python bindings (`deltalake` on PyPI).
- [connector-x](https://github.com/sfu-db/connector-x) - Fastest library to load data from databases into DataFrames.
- [pathway](https://github.com/pathwaycom/pathway) - Performant Python ETL framework with a Rust runtime.
- [hudi-rs](https://github.com/apache/hudi-rs) - Native Rust implementation for Apache Hudi with Python bindings.
- [sail](https://github.com/lakehq/sail) - Unifying stream, batch, and AI workloads with Apache Spark compatibility.

## Date & Time

- [pendulum](https://github.com/python-pendulum/pendulum) - Python datetimes made easy; performance-critical parts rewritten from C to Rust in v3.

## Data Structures

- [rpds-py](https://github.com/crate-py/rpds) - Python bindings to the Rust rpds crate for persistent data structures.
- [fastbloom](https://github.com/yankun1992/fastbloom) - A fast bloom filter and counting bloom filter.
- [fastuuid](https://github.com/thedrow/fastuuid) - Python bindings to Rust's UUID library.

## File Watching & System Utilities

- [watchfiles](https://github.com/samuelcolvin/watchfiles) - Simple, modern, fast file watching and code reload, powered by Rust's `notify` crate.
- [cramjam](https://github.com/milesgranger/cramjam) - Thin Python bindings to de/compression algorithms (snappy, brotli, lz4, zstd, etc.).

## Finance

- [finalytics](https://github.com/Nnamdi-sys/finalytics) - Investment analysis library.
- [rateslib](https://github.com/attack68/rateslib) - A fixed income library for Python using Rust extensions.

## Geospatial

- [geo-index](https://github.com/kylebarron/geo-index) - Packed, immutable, zero-copy spatial indexes.
- [tzfpy](https://github.com/ringsaturn/tzfpy) - Fast longitude/latitude to timezone name conversion.
- [utiles](https://github.com/jessekrubin/utiles) - Fast web-map tile utilities.

## Graph Libraries

- [rustworkx](https://github.com/Qiskit/rustworkx) - A high-performance Python graph library (originally created for Qiskit).

## HTTP Clients

- [primp](https://github.com/deedy5/primp) - Fast HTTP client that can impersonate browsers by mimicking TLS/JA3/HTTP2 fingerprints.
- [rnet](https://github.com/0x676e67/rnet) - Asynchronous Python HTTP client powered by Rust.

## Linting, Formatting & Type Checking

- [ruff](https://github.com/astral-sh/ruff) - An extremely fast Python linter and code formatter.
- [ty](https://github.com/astral-sh/ty) - An extremely fast Python type checker and language server by Astral.
- [pyrefly](https://github.com/facebook/pyrefly) - A fast Python type checker and language server from Meta.

## Miscellaneous

- [pycrdt](https://github.com/jupyter-server/pycrdt) - Python bindings for the Yrs Rust CRDT implementation (collaborative editing).
- [pyxel](https://github.com/kitao/pyxel) - A retro game engine for Python, with core written in Rust.

## Package Management & Tooling

- [uv](https://github.com/astral-sh/uv) - An extremely fast Python package and project manager. 10-100x faster than pip, replaces pip-tools, poetry, pyenv, pipx, and virtualenv in a single tool.
- [maturin](https://github.com/PyO3/maturin) - Build and publish Rust-based Python packages with pyo3, cffi, and uniffi bindings.
- [pixi](https://github.com/prefix-dev/pixi) - A fast conda/pip package manager.
- [rye](https://github.com/astral-sh/rye) - A Python project management tool (largely succeeded by uv).

## Rust-Python Interop

- [PyO3](https://github.com/PyO3/pyo3) - Rust bindings for the Python interpreter. The foundation for most projects on this list.
- [setuptools-rust](https://github.com/PyO3/setuptools-rust) - Setuptools plugin for Rust extensions.
- [RustPython](https://github.com/RustPython/RustPython) - A Python 3 interpreter written entirely in Rust.

## Scientific Computing

- [river](https://github.com/online-ml/river) - Online machine learning in Python; computationally heavy algorithms in Rust.
- [forust](https://github.com/jinlow/forust) - A lightweight gradient boosted decision tree library.
- [radiate](https://github.com/pkalivas/radiate) - A high-performance evolution engine for genetic programming and evolutionary algorithms.
- [cellular_raza](https://github.com/jonaspleyer/cellular_raza) - A cellular agent-based simulation framework.
- [feos](https://github.com/feos-org/feos) - Lightning fast thermodynamic modeling with a fully developed Python interface.

## Search & Indexing

- [tantivy-py](https://github.com/quickwit-oss/tantivy-py) - Python bindings for Tantivy, a full-text search engine library (Lucene alternative).

## Serialization & Parsing

- [orjson](https://github.com/ijl/orjson) - Fast, correct JSON library supporting dataclasses, datetimes, and numpy.
- [jiter](https://github.com/pydantic/jiter) - Fast iterable JSON parser, used by pydantic and the OpenAI Python SDK.
- [ormsgpack](https://github.com/aviramha/ormsgpack) - Fast MessagePack serialization/deserialization, derived from orjson.

## Tokenization & ML

- [tokenizers](https://github.com/huggingface/tokenizers) - Hugging Face's fast tokenizer library with Python bindings.
- [tiktoken](https://github.com/openai/tiktoken) - A fast BPE tokenizer for use with OpenAI's models.
- [safetensors](https://github.com/huggingface/safetensors) - A safe and fast format for storing and loading tensors.

## Validation & Data Modeling

- [pydantic-core](https://github.com/pydantic/pydantic-core) - Core validation logic for pydantic, written in Rust.
- [jsonschema-rs](https://github.com/Stranger6667/jsonschema) - A high-performance JSON Schema validator.

## Visualization

- [rerun](https://github.com/rerun-io/rerun) - Visualize streams of multimodal data. Built in Rust with a Python SDK.


## Web Frameworks & Servers

- [granian](https://github.com/emmett-framework/granian) - A Rust HTTP server for Python WSGI/ASGI/RSGI apps, built on Hyper and Tokio.
- [robyn](https://github.com/sansyrox/robyn) - A super fast async Python web framework with a Rust runtime.

## Web Scraping & HTML

- [css-inline](https://github.com/Stranger6667/css-inline) - CSS inlining implemented in Rust, for fast HTML email preparation.
- [selectolax](https://github.com/rushter/selectolax) - Fast HTML5 parser with CSS selectors, using Rust's html5ever engine.
- [html2text-rs](https://github.com/deedy5/html2text_rs) - Python library for converting HTML to markup or plain text.
- [html-py-ever](https://github.com/SimonSapin/html5ever-python) - Fast HTML parsing and CSS selecting via html5ever.

---

## Footnotes

### Learning Resources
- [PyO3 User Guide](https://pyo3.rs/) - Official guide for writing Python extensions in Rust.
- [maturin User Guide](https://www.maturin.rs/) - Build and publish Rust Python packages.
- [Writing Python Extensions in Rust](https://www.infoworld.com/article/3687744/how-to-write-python-extensions-in-rust-with-pyo3.html) - InfoWorld tutorial.

### Articles
- [Making Python 100x faster with less than 100 lines of Rust](https://ohadravid.github.io/posts/2023-03-rusty-python/) - Performance optimization guide.
- [Why Rust is the Future of Python Tooling](https://pythonspeed.com/articles/rust-python-tooling/) - Analysis of the Rust-Python ecosystem.

### Communities
- [PyO3 Discord](https://discord.gg/33kcChzH7f) - Official PyO3 community.
- [r/rust](https://reddit.com/r/rust) - Rust community.
- [r/Python](https://reddit.com/r/Python) - Python community.

## Contributing

Contributions welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.
