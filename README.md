# Awesome Python x Rust [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of Python tools, libraries, and frameworks with Rust under the hood.

Python's ecosystem is increasingly leveraging Rust for performance-critical components. This list tracks that movement.

---

## Contents

- [Package Management & Tooling](#package-management--tooling)
- [Rust-Python Interop](#rust-python-interop)
- [Linting, Formatting & Type Checking](#linting-formatting--type-checking)
- [Web Frameworks & Servers](#web-frameworks--servers)
- [Data Processing & DataFrames](#data-processing--dataframes)
- [Serialization & Parsing](#serialization--parsing)
- [Validation & Data Modeling](#validation--data-modeling)
- [Tokenization & ML](#tokenization--ml)
- [Cryptography & Hashing](#cryptography--hashing)
- [Search & Indexing](#search--indexing)
- [Arrow & Columnar Data](#arrow--columnar-data)
- [Cloud Storage](#cloud-storage)
- [Data Structures](#data-structures)
- [File Watching & System Utilities](#file-watching--system-utilities)
- [Date & Time](#date--time)
- [Web Scraping & HTML](#web-scraping--html)
- [HTTP Clients](#http-clients)
- [Graph Libraries](#graph-libraries)
- [Visualization](#visualization)
- [Scientific Computing](#scientific-computing)
- [Miscellaneous](#miscellaneous)

---

## Package Management & Tooling

- [uv](https://github.com/astral-sh/uv) - An extremely fast Python package and project manager.
- [maturin](https://github.com/PyO3/maturin) - Build and publish Rust-based Python packages with pyo3, cffi, and uniffi bindings.
- [pixi](https://github.com/prefix-dev/pixi) - A fast conda/pip package manager.
- [rye](https://github.com/astral-sh/rye) - A Python project management tool (largely succeeded by uv).

## Rust-Python Interop

- [PyO3](https://github.com/PyO3/pyo3) - Rust bindings for the Python interpreter. The foundation for most projects on this list.
- [setuptools-rust](https://github.com/PyO3/setuptools-rust) - Setuptools plugin for Rust extensions.
- [RustPython](https://github.com/RustPython/RustPython) - A Python 3 interpreter written entirely in Rust.

## Linting, Formatting & Type Checking

- [ruff](https://github.com/astral-sh/ruff) - An extremely fast Python linter and code formatter.
- [ty](https://github.com/astral-sh/ty) - An extremely fast Python type checker and language server by Astral.
- [pyrefly](https://github.com/facebook/pyrefly) - A fast Python type checker and language server from Meta.

## Web Frameworks & Servers

- [granian](https://github.com/emmett-framework/granian) - A Rust HTTP server for Python WSGI/ASGI/RSGI apps, built on Hyper and Tokio.
- [robyn](https://github.com/sansyrox/robyn) - A super fast async Python web framework with a Rust runtime.

## Data Processing & DataFrames

- [polars](https://github.com/pola-rs/polars) - A fast multi-threaded DataFrame library.
- [datafusion-python](https://github.com/apache/datafusion-python) - Python bindings for Apache DataFusion, an in-memory query engine.
- [delta-rs](https://github.com/delta-io/delta-rs) - Native Rust library for Delta Lake with Python bindings (`deltalake` on PyPI).
- [connector-x](https://github.com/sfu-db/connector-x) - Fastest library to load data from databases into DataFrames.
- [pathway](https://github.com/pathwaycom/pathway) - Performant Python ETL framework with a Rust runtime.

## Serialization & Parsing

- [orjson](https://github.com/ijl/orjson) - Fast, correct JSON library supporting dataclasses, datetimes, and numpy.
- [jiter](https://github.com/pydantic/jiter) - Fast iterable JSON parser, used by pydantic and the OpenAI Python SDK.
- [ormsgpack](https://github.com/aviramha/ormsgpack) - Fast MessagePack serialization/deserialization, derived from orjson.

## Validation & Data Modeling

- [pydantic-core](https://github.com/pydantic/pydantic-core) - Core validation logic for pydantic, written in Rust.

## Tokenization & ML

- [tokenizers](https://github.com/huggingface/tokenizers) - HuggingFace's fast tokenizer library with Python bindings.
- [tiktoken](https://github.com/openai/tiktoken) - A fast BPE tokenizer for use with OpenAI's models.
- [safetensors](https://github.com/huggingface/safetensors) - A safe and fast format for storing and loading tensors.

## Cryptography & Hashing

- [cryptography](https://github.com/pyca/cryptography) - The standard Python cryptographic library, with performance-critical parts in Rust.
- [blake3-py](https://github.com/oconnor663/blake3-py) - Python bindings for the BLAKE3 cryptographic hash function.

## Search & Indexing

- [tantivy-py](https://github.com/quickwit-oss/tantivy-py) - Python bindings for Tantivy, a full-text search engine library (Lucene alternative).

## Arrow & Columnar Data

- [arro3](https://github.com/kylebarron/arro3) - A minimal Python library for Apache Arrow, binding to the Rust Arrow crate.

## Cloud Storage

- [obstore](https://github.com/developmentseed/obstore) - High-throughput Python interface to S3, GCS, and Azure Storage.
- [opendal](https://github.com/apache/opendal) - Apache OpenDAL: unified data access layer for all storage services.

## Data Structures

- [rpds-py](https://github.com/crate-py/rpds) - Python bindings to the Rust rpds crate for persistent data structures.

## File Watching & System Utilities

- [watchfiles](https://github.com/samuelcolvin/watchfiles) - Simple, modern, fast file watching and code reload, powered by Rust's `notify` crate.
- [cramjam](https://github.com/milesgranger/cramjam) - Thin Python bindings to de/compression algorithms (snappy, brotli, lz4, zstd, etc.).

## Date & Time

- [pendulum](https://github.com/python-pendulum/pendulum) - Python datetimes made easy; performance-critical parts rewritten from C to Rust in v3.

## Web Scraping & HTML

- [css-inline](https://github.com/Stranger6667/css-inline) - CSS inlining implemented in Rust, for fast HTML email preparation.
- [selectolax](https://github.com/rushter/selectolax) - Fast HTML5 parser with CSS selectors, using Rust's html5ever engine.

## HTTP Clients

- [primp](https://github.com/deedy5/primp) - Fast HTTP client that can impersonate browsers by mimicking TLS/JA3/HTTP2 fingerprints.

## Graph Libraries

- [rustworkx](https://github.com/Qiskit/rustworkx) - A high-performance Python graph library (originally created for Qiskit).

## Visualization

- [rerun](https://github.com/rerun-io/rerun) - Visualize streams of multimodal data. Built in Rust with a Python SDK.

## Scientific Computing

- [river](https://github.com/online-ml/river) - Online machine learning in Python; computationally heavy algorithms in Rust.
- [forust](https://github.com/jinlow/forust) - A lightweight gradient boosted decision tree library.

## Miscellaneous

- [pycrdt](https://github.com/jupyter-server/pycrdt) - Python bindings for the Yrs Rust CRDT implementation (collaborative editing).
- [pyxel](https://github.com/kitao/pyxel) - A retro game engine for Python, with core written in Rust.

---

## Contributing

Contributions welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.

## Acknowledgements

Inspired by [awesome-python](https://github.com/vinta/awesome-python).