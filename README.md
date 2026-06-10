# Case Studies

Personal deep-dives into systems, benchmarks, incidents, and papers — one
well-researched markdown file at a time.

Every entry tries to answer three questions: **how does it actually work, why
was it built that way, and what transfers elsewhere?**

## ⭐ Featured · Goodhart's Law, caught in the act

> *"When a measure becomes a target, it ceases to be a good measure."*

**[ecdsa.fail](https://www.ecdsa.fail/)** — a public leaderboard for the cheapest
quantum circuit that breaks ECDSA — is the cleanest place I've found to *watch
Goodhart's law happen, and prove it*. I classified all 300 leaderboard
submissions and found that **~77% of "progress" was gaming the validator, not
building better circuits.**

The benchmark even regenerates its tests from a hash of your circuit to block
memorization — and gets gamed anyway, the same shape as how LLM benchmarks get
gamed (contamination, prompt-tuning, best-of-N). The study shows exactly how —
with the math, a control experiment, and what actually resists it.

**→ [Read the case study »](studies/2026-06-ecdsafail-quantum-benchmark/)**

---

## Index

| Date | Case study | Area | Status | One-line takeaway |
|------|------------|------|--------|-------------------|
| 2026-06 | [Goodhart's Law, caught in the act](studies/2026-06-ecdsafail-quantum-benchmark/) | benchmarks · AI agents · eval integrity | 🌳 done | ~77% of leaderboard "progress" was gaming the validator, not better circuits — Goodhart's law, quantified (and the same shape as AI-benchmark gaming). |

## Format

Each study lives in its own folder under [`studies/`](studies/) and follows
[`TEMPLATE.md`](TEMPLATE.md):

1. **TL;DR** — the conclusions, up front
2. **Context & problem** — what the system does and what makes it hard
3. **How it works** — architecture and key flows, with Mermaid diagrams
4. **Design decisions & trade-offs** — the "why this way" table
5. **Hands-on** *(optional but encouraged)* — code, experiments, measurements
6. **Takeaways & references**

## Conventions

- One folder per study: `studies/YYYY-MM-short-slug/README.md`, images in `assets/`
- Diagrams are [Mermaid](https://mermaid.js.org/) where possible — GitHub
  renders them natively and they diff like code
- Status: 🌱 draft → 🌿 in progress → 🌳 done
- Published-but-imperfect beats polished-but-private

## License

Content is licensed [CC BY 4.0](LICENSE).
