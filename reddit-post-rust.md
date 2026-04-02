# Awesome Python Rust - Showcasing Rust's impact on the Python ecosystem

I've compiled a curated list of Python tools and libraries that use Rust for their performance-critical components: https://github.com/ritwik/awesome-python-rs

## Why this matters for Rust developers

This list demonstrates the growing adoption of Rust in one of the world's most popular programming languages. It's a great showcase of:

- **Real-world Rust applications** at massive scale (tools like uv, ruff, and polars have millions of downloads)
- **PyO3 ecosystem** - Most projects use PyO3 for Python bindings
- **Performance wins** - Many projects achieve 10-100x speedups over pure Python implementations
- **Production success stories** - These aren't toy projects; they're being used by major companies and projects

## Categories covered (70+ projects)

- Package management (uv, maturin, pixi)
- Development tools (ruff, ty, pyrefly)
- Data processing (polars, datafusion-python, delta-rs)
- Web frameworks (granian, Robyn)
- Serialization (orjson, jiter)
- ML/AI (tokenizers, tiktoken, safetensors, chroma)
- Cryptography (cryptography, blake3-py)
- And 15+ more categories

## Notable achievements

- **uv** - Replaced pip, pip-tools, poetry, pyenv, and virtualenv; 10-100x faster
- **ruff** - Replaced flake8, black, isort, and more; 10-100x faster
- **polars** - DataFrame library competing with pandas; 5-10x faster with less memory
- **cryptography** - Python's standard crypto library now uses Rust

## For Rust devs interested in Python

The list includes:
- PyO3 resources and documentation
- Tutorials on writing Python extensions in Rust
- Community links (PyO3 Discord, etc.)
- Real-world examples to learn from

If you're working on a Rust+Python project or know of one that should be included, contributions are very welcome!
