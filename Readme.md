# First Principles Framework (FPF) — Core Conceptual Specification

> **An Operating System for Thought**  
> *Architecting transdisciplinary reasoning for systems, epistemes, and communities.*

**Version:** December 2025  
**Primary Author:** Anatoly Levenchuk (with LLM assistance)  
**Status:** Normative kernel, "eternal alpha" — already used in working projects and increasingly acting as an MVP for working development programmes, while still evolving as a research framework.

## 📖 Overview

The **First Principles Framework (FPF)** is a rigorous, transdisciplinary architecture for thinking, written in human- and machine-readable pseudo-code (the informal "language of technical standards" with multiple "May", "Should", "Must"). It provides a generative pattern language to model complex systems, manage knowledge evolution, and ensure auditable assurance across engineering, research, and management domains. Internally, FPF also serves as a conceptual data schema for rational work that you look at, resonate with, and mine for patterns than a narrative textbook. 

FPF is not a specific methodology (like Agile or Waterfall) nor a static encyclopedia. It is an **episteme of method** — a structured specification of how to think — packaged as a set of architecture decision records (ADRs) and patterns that can be executed by humans and LLMs and consumed as pseudo-code by LLMs. It bridges the gap between **rigorous assurance** (audits, proofs) and **open-ended creativity** (innovation, novelty) by treating them as complementary engines within a single evolution.
 

### 🧠 FPF as an "Operating System for Thought"

Using the OS metaphor:

* **Runs "applications of thought".** FPF provides a canonical reasoning cycle (abduction–deduction–induction, `B.5`) and a canonical evolution cycle (`B.4`) that act as a generic *runtime* for research and engineering tasks.
* **Isolates processes and manages their interaction.** `U.BoundedContext` gives an "address space of meaning"; alignment bridges, congruence levels, and Concept-Set tables (`F.9`, `F.17`) define controlled concept exchange between contexts instead of global terminology soup.
* **Creates and terminates thought processes.** The holon → role → method → work chain makes "a process of thinking" explicit: from intention, through role assignment and method choice, to concrete Work records.
* **Manages memory and protects meaning.** `U.BoundedContext`, Evidence Graphs and context passports keep track of *where* statements hold, under which editions and planes, so that reasoning remains auditable instead of becoming folklore. 
* **Prepares resource management.** `Γ_work` (Gamma, composition operator) and the planned Resrc-CAL describe how time, money, energy, and other resources flow through work streams.
* **Provides a "conceptual file system" and I/O.** Cards, tables, records (RSR/RSCR, F-cluster) are the conceptual "files" and journals through which thinking interacts with the world, independently of any specific notation or tool. This is how FPF supports "thinking by modelling": you externalise thought into structured artefacts instead of keeping everything in your head. 
* **Uses a micro-kernel architecture.** At the core is a minimal transdisciplinary set of types and Γ-operators; domain-specific calculi, logics, CHR-packs and SoTA-packs (`Part C`, `Part G`) plug in like drivers and services above the micro-kernel.

Loaded as a file into an LLM, FPF acts as a *bias-assistant* or "grimoire": it steers the model toward first-principles, SoTA-oriented reasoning instead of generic marketing/management/pop-psychology boilerplate — but it will not think instead of you, and without good questions you can still get very confident, well-structured nonsense. 

## 🎯 Who is this for?

*   **Engineers** building reliable physical or cyber-physical systems (`U.System`).
*   **Researchers** constructing trustworthy knowledge and theories (`U.Episteme`).
*   **Managers** orchestrating collective intelligence, budgets, and evolutionary cycles.

## 🔑 Key Concepts & Commitments

FPF is built on a micro-kernel of non-negotiable principles. If you are new, start with these core ideas:

1.  **Holonic Foundation (`A.1`):** Everything is a `U.Holon`—simultaneously a whole and a part. We strictly distinguish between physical actors (**Systems**) and knowledge artifacts (**Epistemes**).
2.  **Contextual Meaning (`A.1.1`, `F.0.1`):** Meaning is local. A term like "Service" or "Process" is defined strictly within a `U.BoundedContext`. Cross-context communication happens only via explicit **Bridges** with declared translation loss.
3.  **Strict Distinction (`A.7`):** We never confuse the map with the territory.
    *   **Role** (Assignment/Mask) $\neq$ **Method** (Recipe) $\neq$ **Work** (Execution/Occurrence).
    *   Documents do not "act"; only Systems enact Work.
4.  **Trust & Assurance Calculus (`B.3`):** Trust is not a feeling; it is a computed tuple **$\langle F, G, R \rangle$**:
    *   **F (Formality):** How rigorously is it expressed?
    *   **G (Claim Scope):** Where does it apply? (Set-valued over context slices).
    *   **R (Reliability):** How well is it supported by evidence?
5.  **Evolution & Creativity (`B.4`, `C.18`):** Systems must evolve. FPF operationalizes the "Bitter Lesson" by favoring general, scalable search methods (**NQD**: Novelty-Quality-Diversity) over hand-tuned heuristics, governed by explicit **Explore-Exploit policies**.
6.  **Universal Aggregation ($\Gamma$):** A single algebra (`B.1`) governs how parts combine into wholes, ensuring invariants like "Weakest-Link" reliability are preserved across scales.

## ✅ What to expect (and what not to expect)

### Reasonable expectations

* **A SoTA-biased co-thinker.** When loaded into an LLM, FPF acts as a bias-assistant for strong engineering and research thinking: you still think, but you get sharper questions, better comparisons and far less "pop-management / pop-psychology fluff" (and definitely not an astrologer in disguise).
* **A DDD-style backbone for disciplines.** FPF can serve as the *DDD (domain-driven design) for science/engineering*: a way to model a discipline (or organisation) with explicit contexts, roles, calculi, and SoTA-packs rather than one more "methodology slide-deck".
* **A long-term atlas of first principles.** Reading the specification end-to-end is not required; it is closer to a dense atlas for first-principles reasoning mastery that you browse, query and mine via your favorite LLMs.
* **A kernel for development programmes.** In practice FPF already feeds programmes for engineer-manager development and research skill-building.

### Unreasonable expectations

* **"I'll just read it once and form my opinion."** The spec reads like OS source code, not like a popular book; it is meant to be *used* with tools, not consumed in one sitting.
* **"This is a plug-and-play tool for all work projects."** Today FPF is a research-grade framework that already helps in real projects as an MVP, but it is not yet a shrink-wrapped product; you still need to adapt, localise, and extend it for your discipline and organisation. 
* **"It works without 'spells' and always gives the right answer."** LLM+FPF will not think instead of you. Without good questions, explicit problem frames, and minimal rational literacy you can still get confident nonsense—just more structured nonsense.
* **"If I ignore first principles, FPF will fix everything."** FPF amplifies whatever style of thinking you bring: if you use it to chase fashion, it will help you catalog fashion; if you use it to chase first principles, it will help you do that more systematically.


## 📂 Repository Structure

```
FPF/
├── FPF-Spec.md              # Complete specification (single file)
├── Readme.md                # This file
├── docs/
│   ├── 00-toc.md            # Table of Contents
│   ├── 01-preface.md        # Preface (non-normative)
│   └── parts/
│       ├── part-a-kernel-architecture.md
│       ├── part-b-transdisciplinary-reasoning.md
│       ├── part-c-architheory-specifications.md
│       ├── part-d-ethics-conflict.md
│       ├── part-e-constitution-authoring.md
│       ├── part-f-unification-suite.md
│       └── part-g-discipline-sota-kit.md
├── prompts/                 # LLM prompt templates
│   ├── 01-characterisation-indicators.md
│   ├── 02-uts-domain.md
│   ├── 03-naming-cards.md
│   ├── 04-p2w-paths.md
│   └── 05-sota-harvesting.md
└── examples/                # Worked examples (coming soon)
```

### Specification Parts

| Part | Name | Description |
|------|------|-------------|
| **A** | Kernel Architecture | Holons, Systems, Epistemes, Bounded Contexts, Transformer quartet |
| **B** | Trans-disciplinary Reasoning | Γ Algebra, F-G-R assurance, TGA, evolution loops |
| **C** | Architheory Specifications | Sys-CAL, KD-CAL, NQD-CAL, Kind-CAL |
| **D** | Ethics & Conflict-Optimisation | Multi-scale ethics, bias audits |
| **E** | Constitution & Authoring | 11 Pillars, Guard-Rails, MVPK |
| **F** | Unification Suite | SenseCells, Concept-Sets, Alignment Bridges |
| **G** | Discipline SoTA Kit | SoTA harvesting, benchmarking, portfolios |

> *"A principle that works in only one world is local folklore; a first principle architects every world."* — **Pattern A.8**

## 🚀 Using FPF with LLMs

FPF is designed to be loaded as a file into an LLM (ChatGPT, Gemini, local models with RAG, etc.) and then *asked to think with you* about concrete projects. There is no magic "prompt library" for FPF: what matters is your ability to have a rational conversation with the model about real problems, not memorise incantations.

In practice the most productive usage is not "summarise the spec", but "treat the spec as a grimoire": ask for concrete chains, patterns, UTS blocks, P2W paths and Q-bundles for your domain and iterate.

### Prompt Templates

See the [`prompts/`](./prompts/) folder for ready-to-use prompt templates:

| Prompt | Purpose |
|--------|---------|
| [01-characterisation-indicators](./prompts/01-characterisation-indicators.md) | From vague idea to measurable characteristics |
| [02-uts-domain](./prompts/02-uts-domain.md) | Build disciplined vocabulary for a domain |
| [03-naming-cards](./prompts/03-naming-cards.md) | Design better names via F.18 |
| [04-p2w-paths](./prompts/04-p2w-paths.md) | Make "from principles to work" explicit |
| [05-sota-harvesting](./prompts/05-sota-harvesting.md) | Organise SoTA for a discipline |

## 🤝 Contributing

### Pull Request Policy

**Do NOT create pull requests directly on the original repository.**

Contributors must:
1. **Fork** this repository to your own GitHub account
2. **Create** your feature branch in your fork
3. **Push** changes to your fork
4. **Open** a pull request from your fork to the original repository

PRs created from branches within the original repository (instead of from forks) will be closed without review.
