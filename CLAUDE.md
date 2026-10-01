# Project Development Rules

These rules apply to all implementation and design work in Personal Cognitive OS. When a proposal conflicts with them, explain the conflict and resolve it before changing the system.

## Source of truth and provenance

- Raw source material is immutable input. Never overwrite, delete, or silently normalize an original source as part of ingestion or processing.
- Derived files must be distinguishable from originals. Preserve a link from every extracted item and generated conclusion back through its evidence to the source.
- Provenance should be precise enough to recover the source file and, when available, its page, slide, section, timestamp, or quoted span.
- Record transformations and their producing tool or model when processing is introduced. A model-generated statement is not a source.
- Treat checksums, stable IDs, and source revisions as future design questions; do not add infrastructure for them before a demonstrated need.

## Knowledge distinctions

Do not collapse unlike things into a generic note or claim. Preserve the distinction between source, fact, concept, framework, theory, method, principle, heuristic, example, experience, decision, outcome, belief, preference, hypothesis, question, and reflection. The ontology is intentionally provisional and should change in response to real material.

## Epistemic status and uncertainty

Keep these origins distinct wherever a statement is stored or presented:

- explicitly stated by a source
- inferred from a source
- inferred by an AI model
- provided by the user
- experimentally validated
- uncertain

Never silently upgrade an inference, hypothesis, or uncertain statement into a fact. Retain the evidence and the reasoning that support an inference, and show uncertainty when presenting it.

## Contradictions and change

- Never silently overwrite conflicting sources, claims, or personal beliefs.
- Represent conflicts explicitly, preserve both positions and their provenance, and investigate before resolving them.
- Preserve history when a belief, preference, or decision changes. A later position does not erase the earlier one or its context.

## Model independence

- Keep knowledge objects, schemas, and core application behavior independent of any one LLM vendor or model API.
- Keep provider-specific adapters at explicit boundaries if and when models are introduced.
- Store durable knowledge in portable, human-readable formats where practical; model prompts and outputs are not the canonical knowledge store.

## Human-readable, privacy-aware storage

- Prefer Markdown, YAML, JSON, and standard, portable databases when a need for persistence is demonstrated.
- Avoid proprietary formats and opaque serialized blobs for canonical knowledge.
- Assume personal source material, experiences, decisions, and beliefs are sensitive. `data/` is ignored by Git by default; do not change that default casually.
- Do not add credentials, API keys, private source files, or personal records to commits. Keep secrets in local environment configuration, never in source control.
- Before tracking any data, explain what it contains, where it will be stored, and who can access it. Prefer keeping private data outside the source repository.

## Incremental architecture

- Build only the smallest useful next capability. The architecture and roadmap describe a long-term direction, not permission to implement every stage now.
- Do not introduce a database, vector or graph database, agent framework, cloud service, embedding pipeline, or LLM integration without a concrete, demonstrated requirement and an explicit trade-off.
- Prefer reversible choices and clear module boundaries. Avoid premature abstractions, speculative configuration, and infrastructure that has no current user.
- Keep the core pipeline inspectable: source, transformation, derived object, relationship, retrieval, reasoning, response, and learning should be separable stages.

## Engineering practice

- Read nearby code and tests before making changes; follow existing conventions and keep edits scoped.
- Add tests for implemented behavior and meaningful edge cases. Do not create scaffolding that has no executable behavior yet.
- Validate inputs at boundaries and fail visibly rather than dropping evidence or silently producing partial knowledge.
- Keep generated output separate from authored source. Make scripts repeatable and non-destructive by default.
- Update documentation when behavior, schemas, privacy handling, or architecture changes.
- Do not process personal source material, call external services, or install heavyweight dependencies without explicit task-level need.
