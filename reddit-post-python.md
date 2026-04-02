# Awesome Python Rust - A curated list of Python tools with Rust under the hood

I've been compiling a comprehensive list of Python libraries and tools that leverage Rust for performance-critical components, and wanted to share it with the community: https://github.com/ritwik/awesome-python-rs

## What's included

The list covers a wide range of categories:

- **Package Management & Tooling** - uv, maturin, pixi, rye
- **Linting & Formatting** - ruff, ty, pyrefly
- **Data Processing** - polars, datafusion-python, delta-rs, connector-x
- **Web Frameworks** - granian, Robyn
- **Serialization** - orjson, jiter, ormsgpack
- **Validation** - pydantic-core, jsonschema-rs
- **ML & Tokenization** - tokenizers, tiktoken, safetensors
- **Cryptography** - cryptography, blake3-py
- **And much more** - 70+ projects across 20+ categories

## Why Rust for Python?

Python's flexibility is great for rapid development, but computationally intensive operations can become bottlenecks. Rust provides:
- Memory safety without garbage collection overhead
- Zero-cost abstractions
- Safe concurrency
- 10-100x performance improvements in many cases

## Notable projects

Some standout examples:
- **uv** - 10-100x faster than pip
- **polars** - 5-10x faster than pandas with lower memory usage
- **ruff** - 10-100x faster than traditional Python linters
- **orjson** - Fastest Python JSON library

The list also includes learning resources, articles, and community links to help you get started with Rust-Python development.

Contributions and suggestions are welcome! If you know of any Python projects using Rust that aren't listed, please open a PR or issue.
