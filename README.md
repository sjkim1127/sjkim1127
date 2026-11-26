# Sung Joo Kim

**Decompiler Engineering · Binary Analysis · Rust Systems · AI-Agent Infrastructure**

I build tools that recover, analyze, and validate the behavior of compiled software. My primary focus is decompiler correctness, intermediate representations, binary semantics, and automated program analysis.

I maintain [Fission Systems](https://github.com/fission-systems) and contribute to open-source decompilers, analysis frameworks, and their evaluation infrastructure. I also build deterministic multimedia engines and agent-oriented developer tools in Rust.

[LinkedIn](https://www.linkedin.com/in/sung-joo-kim-718a93303/) · [Open-source pull requests](https://github.com/pulls?q=is%3Apr+author%3Asjkim1127)

---

## Primary projects

| Project | Focus |
|---|---|
| **[Fission](https://github.com/fission-systems/Fission)** | Agent-first, Rust-native binary analysis and decompilation CLI. ELF/PE/Mach-O loading, SLEIGH/P-code lifting, NIR/HIR, CFG structuring, type recovery, structured machine contracts, and execution-based and solver-backed semantic validation. |
| **[FreshBench](https://github.com/fission-systems/freshbench)** | Rust-based static decompiler benchmark built on fresh, license-clean C corpora, with fingerprint-based DecBench exclusions, CFG graph edit distance, type recovery, recompilation metrics, and actionable improvement targets. The M1 corpus is published; tool evaluation is ongoing. |
| **[Fission Plugin API](https://github.com/fission-systems/fission-plugin-api)** | Experimental headless Rust SDK and capability-negotiated compatibility runtime for selected IDA Pro, Ghidra, Binary Ninja, and angr scripting APIs. |
| **[Reversecore MCP](https://github.com/sjkim1127/Reversecore_MCP)** | MCP infrastructure connecting AI agents to local binary analysis, malware triage, vulnerability research, crash analysis, and digital forensics tools, with structured evidence and context-efficient tool routing. |

## Research & engineering

My current work explores how to make decompilers more trustworthy, testable, and useful for both humans and autonomous agents.

| Direction | Approach |
|---|---|
| **Differential semantic checking** | Compare machine-code execution against decompiled IR, identify concrete counterexamples, expand input coverage with concolic execution, and track semantic regressions. |
| **Semantic bug localization** | Isolate potentially incorrect rewrite rules and investigate mismatches through counterfactual replay and mutation testing. |
| **State-machine recovery** | Explore active automata learning and solver-backed path-closure certificates for supported binary step functions. |
| **Decompiler evaluation** | Build reproducible corpora and independent scoring infrastructure; distinguish structural similarity from behavioral correctness. |
| **Agent-first reverse engineering** | Design deterministic CLIs, versioned JSON contracts, plugin interfaces, and evidence-oriented analysis workflows. |

## Open-source contributions

Selected contributions, grouped by upstream status.

### Merged contributions

| Project | Selected work |
|---|---|
| **[Kuna](https://github.com/Noelo-Lab/kuna)** | Differential semantic checking proposal ([#1714](https://github.com/Noelo-Lab/kuna/pull/1714)); SLEIGH processor-spec documentation ([#1766](https://github.com/Noelo-Lab/kuna/pull/1766)); SBORROW comparison polarity and escaped stack-store liveness ([#1833](https://github.com/Noelo-Lab/kuna/pull/1833), [#1834](https://github.com/Noelo-Lab/kuna/pull/1834)); ARM/Thumb and AArch64 instruction semantics ([#1901](https://github.com/Noelo-Lab/kuna/pull/1901), [#1907](https://github.com/Noelo-Lab/kuna/pull/1907), [#1909](https://github.com/Noelo-Lab/kuna/pull/1909), [#1951](https://github.com/Noelo-Lab/kuna/pull/1951)); calling-convention and argument/return recovery ([#1924](https://github.com/Noelo-Lab/kuna/pull/1924), [#1927](https://github.com/Noelo-Lab/kuna/pull/1927), [#1929](https://github.com/Noelo-Lab/kuna/pull/1929), [#1935](https://github.com/Noelo-Lab/kuna/pull/1935), [#1937](https://github.com/Noelo-Lab/kuna/pull/1937)); instruction-level raw P-code and diagnostics ([#1316](https://github.com/Noelo-Lab/kuna/pull/1316), [#639](https://github.com/Noelo-Lab/kuna/pull/639)); FID candidate inspection and evidence-based renaming ([#1547](https://github.com/Noelo-Lab/kuna/pull/1547), [#1549](https://github.com/Noelo-Lab/kuna/pull/1549), [#1550](https://github.com/Noelo-Lab/kuna/pull/1550)). |
| **[angr/binaries](https://github.com/angr/binaries)** | x86-64 regression fixtures for function-pointer tables and tail-call-dispatched function recovery ([#280](https://github.com/angr/binaries/pull/280)). |
| **[DecBench](https://github.com/Noelo-Lab/decbench)** | Standalone Mach-O DWARF reader and bounded PDB/MSF stream reader ([#115](https://github.com/Noelo-Lab/decbench/pull/115), [#116](https://github.com/Noelo-Lab/decbench/pull/116)). |
| **[rust-joern](https://github.com/Noelo-Lab/rust-joern)** | C++ parser and CFG recovery improvements for templates, constructors, type-name context, call operands, range-for loops, and C++20 init-statements ([#3](https://github.com/Noelo-Lab/rust-joern/pull/3), [#5](https://github.com/Noelo-Lab/rust-joern/pull/5), [#9](https://github.com/Noelo-Lab/rust-joern/pull/9), [#12](https://github.com/Noelo-Lab/rust-joern/pull/12), [#15](https://github.com/Noelo-Lab/rust-joern/pull/15), [#18](https://github.com/Noelo-Lab/rust-joern/pull/18)). |
| **[NVIDIA / yaml-sigil-rs](https://github.com/NVIDIA/yaml-sigil-rs)** | Quoted and escaped YAML signature-document key normalization with regression tests ([original #123](https://github.com/NVIDIA/yaml-sigil-rs/pull/123), incorporated in [merged #131](https://github.com/NVIDIA/yaml-sigil-rs/pull/131)). |
| **[Remotion](https://github.com/remotion-dev/remotion)** | Copy context for agents in Remotion Studio folder menus ([#11277](https://github.com/remotion-dev/remotion/pull/11277)). |

### Active upstream work

| Project | Work | Status |
|---|---|---|
| **Kuna — DiffVerify** | [#1830](https://github.com/Noelo-Lab/kuna/pull/1830): `kuna-verify`, a source-independent differential semantic checker with concrete and concolic inputs, rewrite-rule localization, instruction-level cross-checks, and a non-gating CI corpus baseline. Sampled agreement is not a proof of equivalence. | Open |
| **Kuna — WBCQ** | [#1947](https://github.com/Noelo-Lab/kuna/pull/1947): active automata learning and solver-backed path-closure certificates for supported binary state machines. | Draft |
| **Kuna — CSIC** | [#1948](https://github.com/Noelo-Lab/kuna/pull/1948): counterfactual interventions to produce localization witnesses for semantic mismatches, with mutation-based evaluation. | Draft |
| **angr** | [#7839](https://github.com/angr/angr/pull/7839): CFGFast recovery of functions tail-called through jump tables, using unwind and table-encoding evidence. | Open |
| **Ghidra** | Thumb STMIA writeback ([#10273](https://github.com/NationalSecurityAgency/ghidra/pull/10273)) and Thumb-2 shifter carry semantics ([#10274](https://github.com/NationalSecurityAgency/ghidra/pull/10274)). | Open |
| **DecBench** | C++ backend definition-name normalization ([#128](https://github.com/Noelo-Lab/decbench/pull/128)), deterministic Fission backend ([#129](https://github.com/Noelo-Lab/decbench/pull/129)), and toolchain-sensitivity analysis ([#127](https://github.com/Noelo-Lab/decbench/issues/127)). | Open PRs / research |
| **rev.ng** | [#630](https://github.com/revng/revng/pull/630): PE/COFF load-config table handling in BinaryImporter. | Draft |

[Browse all contributions](https://github.com/pulls?q=is%3Apr+author%3Asjkim1127)

---

## Other systems projects

| Project | Focus |
|---|---|
| **[Rust Motion](https://github.com/sjkim1127/rust-motion)** | Deterministic, browser-free programmatic video engine with a typed scene IR, parallel CPU rendering, optional GPU acceleration, FFmpeg encoding, Rust/Rhai/Python/TypeScript front ends, WASM playback, and an agent-friendly CLI. |
| **[Kymion](https://github.com/sjkim1127/Kymion)** | Experimental Rust/WASM digital audio workstation with MIDI, non-destructive audio editing, real-time AudioWorklet playback, DSP, vocal synthesis, and a shared JSON command engine. |
| **[Reforge MCP](https://github.com/sjkim1127/reforge-mcp)** | Early-stage MCP infrastructure for migrating software to Rust, with repository indexing, source navigation, and persistent planning state. |
| **[Eon](https://github.com/sjkim1127/Eon)** | Experimental Rust engine for deterministic calculations across traditional astrology and related systems, with structured CLI and MCP interfaces. |

## Technical interests & stack

**Program analysis:** Decompilation · Compiler IR · CFG/DFG · SSA · Binary semantics · Calling conventions · Type recovery · Symbolic execution · SMT · Differential testing · Automata learning

**Systems:** Rust · C/C++ · Python · TypeScript · Linux · WebAssembly · ELF/PE/Mach-O · DWARF/PDB · SLEIGH/P-code · Z3 · QEMU/Unicorn · MCP · FFmpeg · GitHub Actions

<sub>Selected upstream work and project status last reviewed: 2026-11-26.</sub>
