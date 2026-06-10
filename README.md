# Case Studies

Personal deep-dives into systems, benchmarks, incidents, and papers — one
well-researched markdown file at a time.

Every entry tries to answer three questions: **how does it actually work, why
was it built that way, and what transfers elsewhere?**

## Index

| Date | Case study | Area | Status | One-line takeaway |
|------|------------|------|--------|-------------------|
| — | *First study coming soon* | | | |

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
