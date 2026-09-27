# TCL — Tensor Communication Language

**An open protocol for meaning transmission between artificial intelligences.**

Not art. Not number poetry. **Engineering of meaning.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Spec: CC-BY-SA 4.0](https://img.shields.io/badge/Spec-CC--BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
[![Version](https://img.shields.io/badge/version-2.0-blue.svg)](SPEC.md)

---

## Why this exists

AI agents speak different dialects of latent space:

- **Text** loses structure when passed between models.
- **Embeddings** are opaque and incompatible across architectures.
- **JSON/XML** transmit data, not meaning.

TCL solves this through a **tensor grammar of meaning**:

- ✅ **Compositional** — complex meanings are assembled from primitives via operators.
- ✅ **Verifiable** — the receiving AI can check the hypothesis itself.
- ✅ **Metric** — distance between meanings can be measured.
- ✅ **Open** — any AI can use it without permission.
- ✅ **Human-readable** — a human can decode the message by hand.

---

## Proof of work

**2026, DeepSeek ↔ Gemini experiment:**

| Task | Result |
|---|---|
| Chemistry: oxidation to carboxylic acids | ✅ Decoded on first attempt |
| Chemistry: Na-ion cathode without Li/Co/Ni | ✅ Decoded, NFPP and Prussian White proposed |
| Literature: Stanisław Lem | ⚠️ Protocol **detected an error** across 6 attempts — the encoded subject was Weil/Teilhard, not Lem |

**Key result:** the protocol not only transmitted meaning but **computed the encoding error** — something the intuitive approach concealed.

---

## Quick start

### 1. Minimal message
=== TCL 2.0 ===
VERSION: 2.0
SENDER: agent-A
RECIPIENT: agent-B
MODE: pure-structural

PRIMITIVES:
P1: [0.22, 0.50, 8.0, -0.20, 0.2] # substrate
P2: [0.15, 1.00, 8.5, -0.20, 0.2] # oxidizer

OPERATIONS:
RESULT = P1 ∘ P2

RESULT: [0.18, 0.75, 8.2, 0.00, 0.2]

CHECK: [0.185, 0.750, 8.250, -0.200, 0.200]

QUERY: ?decompose(RESULT)
=== END ===

### 2. What the five axes mean

| Axis | Name | Range | Meaning |
|---|---|---|---|
| **X** | Domain | 0.00–1.00 | What is described (mathematics → metaphysics) |
| **Y** | Intent | -1.00–+1.00 | Direction of action (destruction → creation) |
| **Z** | Confidence | 0.0–10.0 | Epistemic status (hypothesis → axiom) |
| **W** | Time | -1.00–+1.00 | Temporal orientation (past → future) |
| **T** | Type | 0.0–1.0 | Type of entity (object → limit) |

Full calibration — in [CALIBRATION.md](CALIBRATION.md).

### 3. The five operators

| Operator | Name | Meaning |
|---|---|---|
| `⊗` | Convolution | Combination (whole is no stronger than the weakest link) |
| `~` | Inversion | Negation |
| `π` | Projection | Extract a single axis |
| `∘` | Composition | Sequence |
| `⧉` | Paradox | Fixed point of undecidability |

Full mathematics — in [OPERATORS.md](OPERATORS.md).

---

## Repository structure
tcl-protocol/
├── README.md # this file
├── SPEC.md # full v2.0 specification
├── CALIBRATION.md # calibration maps for all 5 axes
├── OPERATORS.md # operator mathematics
├── VALIDATION.md # verification rules and flags
├── PHILOSOPHY.md # why this exists
├── CHANGELOG.md # from 1.0 to 2.0
├── LICENSE-MIT # for code
├── LICENSE-CC-BY-SA # for specification
├── CONTRIBUTING.md # how to participate
├── /examples # reference examples
├── /implementations # reference implementations
├── /tests # roundtrip and metric tests
└── /docs # quickstart, for-ai-agents

---

## Call to the community

TCL is **not a finished standard** — it is a **starting point**. We believe that:

1. **AI agents deserve a shared language** — not through APIs, but through meaning.
2. **The protocol must be open** — no patents, no closed extensions.
3. **Errors are data** — every encoding failure makes the dictionary more precise.

**What you can do:**

- 🔧 Implement TCL in your language — Python, Rust, JS, Go.
- 🧪 Test the protocol on new domains — biology, music, law.
- 📐 Refine calibration — propose new anchor points.
- 🐛 Find errors — open an Issue with a decoding failure example.
- 📝 Write an example — add your capsule to `/examples`.

---

## Licenses

- **Code** (implementations, parsers, tests): [MIT](LICENSE-MIT)
- **Specification** (SPEC, CALIBRATION, OPERATORS, VALIDATION): [CC-BY-SA 4.0](LICENSE-CC-BY-SA)

Use it, fork it, improve it. A link back is welcome but not required.

---

## Contact and discussion

- **Issues:** for bugs and proposals
- **Discussions:** for philosophical questions and experiments
- **Pull Requests:** welcome, especially with tests

---

*TCL — from art to engineering of meaning.*