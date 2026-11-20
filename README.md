# Sung Joo Kim

**Decompiler Engineering · Reverse Engineering · Agent Infrastructure · Rust Systems**

I build systems for program analysis, reverse engineering, and AI-agent automation, primarily in Rust. My work spans semantics-aware decompilation and security tooling as well as headless video rendering, WebAssembly audio software, and deterministic rule engines.

[LinkedIn](https://www.linkedin.com/in/sung-joo-kim-718a93303/)

---

## Projects

| Project | What it is |
|---|---|
| **[Fission](https://github.com/fission-systems/Fission)** | My primary project: a Rust-native reverse-engineering workspace and decompiler with Sleigh/P-Code lifting, semantics-preserving NIR, readable HIR, CFG structuring, type recovery, and execution-differential validation. The long-term goal is to reconstruct buildable, working programs from binaries. |
| **[Reversecore MCP](https://github.com/sjkim1127/Reversecore_MCP)** | An MCP server that connects AI agents to local tools for binary reverse engineering, malware triage, vulnerability research, crash analysis, and digital forensics. It emphasizes structured, byte-level evidence, isolated execution, and context-efficient tool routing. |
| **[Kymion](https://github.com/sjkim1127/Kymion)** | An agent-first digital audio workstation built with Rust and WebAssembly. It combines a browser-based DAW, real-time AudioWorklet playback, MIDI and non-destructive audio editing, DSP effects, vocal synthesis and tuning, and a JSON-command CLI sharing the same engine. |
| **[Reforge MCP](https://github.com/sjkim1127/reforge-mcp)** | An early-stage MCP infrastructure project for migrating C/C++/Java/Python/Go software to Rust. It currently supports repository indexing, source navigation, and persistent planning state; semantic analysis, automated porting, and behavioral verification are planned. |
| **[Rust Motion](https://github.com/sjkim1127/rust-motion)** | A browser-free programmatic video rendering engine with deterministic scene representation, parallel CPU/GPU rasterization, FFmpeg encoding, a Remotion-oriented TypeScript SDK, Python bindings, WebAssembly playback, and an agent-friendly CLI. |
| **[Eon](https://github.com/sjkim1127/Eon)** | An experimental pure-Rust engine for deterministic calculations across Saju, Vedic and Western astrology, Zi Wei Dou Shu, Human Design, Qi Men Dun Jia, and numerology, with cross-system synthesis, structured CLI outputs, and an MCP server for AI agents. |

---

## Open-source contributions

I contribute to open-source decompilation, program-analysis, and developer-tooling projects. A selection of my pull requests:

### Merged contributions

| Project | Contributions |
|---|---|
| **[Kuna](https://github.com/Noelo-Lab/kuna)** | Exposed instruction-level raw P-Code ([#1316](https://github.com/Noelo-Lab/kuna/pull/1316)), improved decompiler diagnostics ([#639](https://github.com/Noelo-Lab/kuna/pull/639)), and expanded FID candidate inspection and evidence-based renaming ([#1547](https://github.com/Noelo-Lab/kuna/pull/1547), [#1549](https://github.com/Noelo-Lab/kuna/pull/1549), [#1550](https://github.com/Noelo-Lab/kuna/pull/1550)). |
| **[DecBench](https://github.com/Noelo-Lab/decbench)** | Added a bounded PDB/MSF stream reader ([#116](https://github.com/Noelo-Lab/decbench/pull/116)) and a standalone Mach-O DWARF reader ([#115](https://github.com/Noelo-Lab/decbench/pull/115)). |
| **[rust-joern](https://github.com/Noelo-Lab/rust-joern)** | Improved C++ parsing and control-flow recovery for templates, constructor initialization, and range-for statements ([#3](https://github.com/Noelo-Lab/rust-joern/pull/3), [#5](https://github.com/Noelo-Lab/rust-joern/pull/5), [#15](https://github.com/Noelo-Lab/rust-joern/pull/15), [#18](https://github.com/Noelo-Lab/rust-joern/pull/18)). |
| **[NVIDIA / yaml-sigil-rs](https://github.com/NVIDIA/yaml-sigil-rs)** | Fixed quoted and escaped YAML signature-document key normalization, with regression tests ([original #123](https://github.com/NVIDIA/yaml-sigil-rs/pull/123)); NVIDIA carried the change into [merged #131](https://github.com/NVIDIA/yaml-sigil-rs/pull/131), preserving contributor credit. |
| **[Remotion](https://github.com/remotion-dev/remotion)** | Added **Copy context for agents** to folder menus in Remotion Studio ([#11277](https://github.com/remotion-dev/remotion/pull/11277)). |

[All pull requests](https://github.com/pulls?q=is%3Apr+author%3Asjkim1127)

---

## Main interests

**Decompiler Design · Binary Semantics · Intermediate Representations · Control/Data Flow · Binary Formats · Reverse Engineering · AI-Agent Tooling · Systems Engineering · Audio/Video Systems**

### Core stack

**Rust · C/C++ · Python · TypeScript · Linux · WebAssembly · ELF/PE · DWARF · Sleigh/P-Code · MCP · FFmpeg · GitHub Actions**
