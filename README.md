# Sung Joo Kim

**Decompiler Systems · Reverse Engineering · Program Analysis · Rust Systems**

I build systems that recover structure and semantics from binaries, evaluate decompiler correctness, and expose low-level program analysis to reproducible tooling and AI agents.

My main work is around **decompilation, binary semantics, IR design, benchmark correctness, and systems tooling** — mostly in Rust.

[LinkedIn](https://www.linkedin.com/in/sung-joo-kim-718a93303/)

---

## What I work on

```text
binary
  → loader / decoder
  → instruction semantics
  → IR
  → control & data-flow analysis
  → structuring / type recovery
  → readable or rebuildable output
  → validation / benchmark / agent interface
```

| Area | Current focus |
|---|---|
| **Decompiler systems** | IR design, structuring, semantic recovery, rendering, and restoration-oriented decompilation |
| **Program analysis** | CFG/data-flow analysis, function identity, DWARF-backed ground truth, and binary semantics |
| **Decompiler evaluation** | Reproducible benchmarks, cross-decompiler comparison, correctness bugs, and corpus qualification |
| **Reverse-engineering tooling** | Binary inspection, analysis automation, MCP interfaces, and agent-first workflows |
| **Systems engineering** | Rust workspaces, native pipelines, CI, differential testing, and performance-sensitive tooling |

---

## Selected systems

### [Fission](https://github.com/fission-systems/Fission)

My primary project: a **Rust-native reverse-engineering and decompiler workspace** built around Sleigh decoding, raw p-code, and its own NIR/HIR analysis pipeline.

The long-term goal is not only readable pseudocode, but progressively restoring a compiled binary into a project that can **build and run again**. Current work includes structuring, type recovery, semantic parity, binary-format support, emulator-backed validation, and decompiler robustness.

### [DecBench C++ Target Qualification](https://github.com/sjkim1127/Decbench_SampleSet)

Artifact-backed research workspace for extending decompiler evaluation toward real C++ programs.

Current work includes **DWARF-based function identity, overload/collision handling, corpus-scale target qualification, cross-decompiler validation, and benchmark-pipeline correctness**.

### [Reversecore MCP](https://github.com/sjkim1127/Reversecore_MCP)

MCP-based reverse-engineering and security tooling for AI-assisted analysis workflows, with an emphasis on explicit tool contracts, isolation, reproducibility, and composable analysis primitives.

### [Reforge MCP](https://github.com/sjkim1127/reforge-mcp)

Experimental MCP system for **porting C, C++, Java, Python, and Go projects to Rust**, with source analysis, dependency-aware planning, compiler feedback, and differential validation as the intended loop.

### [Rust Motion](https://github.com/sjkim1127/rust-motion)

Browser-free, code-driven video rendering in Rust. The project combines a native scene graph, CPU/GPU rasterization, FFmpeg pipelines, and optional Dioxus authoring/preview.

---

## Recent open-source work

- **[Noelo-Lab/decbench#91](https://github.com/Noelo-Lab/decbench/pull/91)** — collision-safe C++ function identity across DWARF, storage, metrics, source lookup, and re-evaluation paths.
- **[Noelo-Lab/decbench#92](https://github.com/Noelo-Lab/decbench/pull/92)** — differential pull-request CI designed around an upstream test suite with known baseline failures.
- **[revng/revng#630](https://github.com/revng/revng/pull/630)** — PE/COFF importer hardening for malformed/stale Load Config Table RVAs that can make LLVM object creation fail.
- **[radareorg/r2sleigh#64](https://github.com/radareorg/r2sleigh/pull/64)** — unsigned bitwise constant folding for r2dec, including AArch64 `mov`/`movk` constant-construction cases.

---

## Current directions

- Improving **Fission NIR/HIR correctness, structuring, type recovery, and rebuildability**
- Extending **DecBench-style evaluation toward C++** without losing function identity or benchmark integrity
- Building **agent-first reverse-engineering interfaces** with inspectable evidence and reproducible analysis steps
- Exploring **Rust-native systems** for source transformation, media pipelines, and automation

### Core stack

**Rust · C/C++ · Python · Linux · GitHub Actions · DWARF · ELF/PE · Sleigh/P-Code**
