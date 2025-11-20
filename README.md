# Architecture Playbook – Clarity Before Complexity

This repository is a concise architecture playbook that demonstrates how I approach
structure, decision-making and communication in complex IT landscapes.

It is based on a fictional travel platform but follows the same principles I apply
in real projects: clarity before complexity, explicit decisions, and transparent trade-offs.

## Goals

- Show how I:
  - frame business and IT goals,
  - describe current vs. target landscapes,
  - use C4 models to communicate architecture,
  - capture decisions via lightweight ADRs.
- Provide a reusable structure that can be adapted for real client engagements.

## Repository Structure

- `docs/` – narrative documentation (introduction, goals, summary)
- `models/`
  - `c4/` – C4 model descriptions (Context, Container, Component, Deployment)
  - `domain/` – domain and capability view
- `decisions/` – Architecture Decision Records (ADRs)
- `examples/` – sample scenarios and use cases for a travel platform

## How to Read

1. Start with `docs/00-introduction.md` and `docs/01-context-and-goals.md`
2. Look at `models/c4/01-context-diagram.md` for the high-level picture
3. Review ADRs in `decisions/` to see how trade-offs are made explicit
4. Use `examples/` as a lightweight case study

## Technologies and Notation

This playbook is tool-agnostic. Diagrams are described textually and can be rendered
with tools like Structurizr, PlantUML or diagram-as-code frameworks if needed.

## When This Is Useful

- Early-phase architecture framing
- Explaining my approach to clients, partners, or recruiters
- Using it as a template for real projects

## License

[MIT](./LICENSE)
