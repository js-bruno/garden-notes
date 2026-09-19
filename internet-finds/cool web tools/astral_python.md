---
title: Astral tooling
aliases:
  - Astral Tooling(python)
  - astral_python
  - astral
tags:
  - find/tool
  - python
  - rust
description: Linter e package manager ultra-rápidos pra Python, escritos em Rust.
---

Basicamente o lint e o package manager ultra rapido feito com rust

- [[ruff]]: lint
- [[uv]]: package manager

https://astral.sh/blog/uv-unified-python-packaging

## Por que importa

Ambos trocam a toolchain inteira do Python (pip, venv, pip-tools, flake8,
isort, black, pyupgrade) por dois binários Rust. É o mesmo movimento que o
[[nix-os]] faz no nível do sistema: substituir uma pilha de scripts por uma
camada declarativa e rápida.

See also: [[ruff]], [[uv]], [[nix-os]], [[internet-finds]]
