# ATM (Atom)

ATM is a minimalist, C-in-spirit compiled language with a modern, batteries-in-the-tooling workflow.

The language stays small on purpose. The ecosystem (CLI + package/dependency workflow + reproducible project env) is where the “modern” lives.

> Goal: the speed + control of low-level development, with a workflow that feels as smooth as an interpreted language.

---

## Status

ATM is currently under active development.
- Lexer/tokenization: **in progress**
- Parser/AST: planned
- Semantic analysis + codegen: planned
- Package/dependency workflow: planned

ATM is **not stable** yet. Expect breaking changes.

---

## Why ATM?

Most languages pick one:
- **Fast + native** but tooling is chaotic, dependency resolution is manual, and “it worked on my machine” becomes a lifestyle.
- **Smooth workflow** but you pay with runtime baggage, heavy virtual machines, or bloat.

ATM tries to sit in the middle:
- Compiled output (native executable target)
- Minimal core language surface area
- A CLI-first workflow that manages projects and dependencies for you
- Per-project environment isolation by default (no global installs)

---

## Key Ideas

### Minimal language, strong ecosystem
ATM keeps the syntax and core semantics small.
Everything else is provided through libraries and packages.

### Reproducible builds by default
ATM projects are self-contained:
- dependency metadata is stored in a **tool-managed local datastore**
- project builds are repeatable across machines

### CLI-driven workflow
No GUI required. No “edit 4 files and pray.”
The CLI is the single source of truth for:
- project init/build/run
- dependencies
- dev vs production build behavior

---

## Installation (Development)

ATM is currently built from source.

High-level plan:
1. Clone the repo
2. Build the `atm` CLI
3. Ensure `atm` is on your PATH


---

## Quick Start

### Create a new project
```sh
atm init hello_atm
cd hello_atm
