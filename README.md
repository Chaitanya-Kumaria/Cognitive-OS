# Personal Cognitive OS

Personal Cognitive OS is a long-term project to build a personal knowledge and reasoning system: one that can preserve what its owner learns, connect ideas across domains, remember personal experience and decisions, and bring relevant knowledge to future problems.

## The problem

Useful knowledge is scattered across learning materials, notes, experience, and decisions. Ordinary note-taking and basic retrieval can find text, but do not by themselves preserve evidence, distinguish kinds of knowledge, surface contradictions, or help determine what is relevant to a new situation. This project explores those capabilities incrementally, with traceability and user control as foundations.

## What this is not

This is not intended to be just a notes app, an Obsidian vault, or a simple RAG chatbot. It is not an autonomous agent or a system that treats generated answers as authoritative. Those descriptions may fit individual tools or experiments later, but do not define the project.

## Current status

**Phase 0: Foundation.** This repository contains initial architecture and ontology documents, draft v0.1 schemas, privacy-conscious Git defaults, and a development backlog. There is no ingestion engine, application, database, model integration, or processed personal material yet.

## Architecture at a glance

The long-term flow is:

`Raw sources → ingestion → extraction → knowledge objects → relationships/graph → retrieval → reasoning → response/action → reflection/learning → memory update`

Every derived claim should remain traceable to its evidence, and its epistemic status should remain explicit. This is a direction, not a build specification for the first release. See [the system overview](docs/architecture/system-overview.md) and [the roadmap](docs/architecture/roadmap.md).

## Repository structure

- `docs/`: architecture, ontology, decisions, and research notes.
- `data/`: future personal sources and derived knowledge; content is ignored by Git by default.
- `system/`: evolving ontology, schemas, prompts, and configuration.
- `src/`: planned capability boundaries; implementation has not started.
- `tests/`: planned behavior-focused tests.
- `scripts/`: small, repeatable project utilities.
- `CLAUDE.md`: project-wide development and data-handling rules.
- `TODO.md`: staged, evolving engineering backlog.

Each directory has a short README describing its intended purpose. Do not put private source material into Git. Prefer a separate local data location for sensitive material and review ignore rules before storing anything.

## How development will proceed

Work in small phases. First review and refine the foundation with real constraints; then implement one inspectable capability at a time, validating preservation, provenance, uncertainty, privacy, and usefulness before adding infrastructure. Later roadmap phases are not authorized implementation work yet.

## Current next step

Review the architecture, ontology, and draft schemas; decide the data/privacy boundary and repository license; then choose a small, non-sensitive sample source for a future ingestion prototype. Do not process MBA files or connect external services as part of this foundation.
