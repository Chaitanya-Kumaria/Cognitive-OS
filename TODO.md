# Development Backlog

This backlog is intentionally provisional. Reorder it as constraints and real use become clearer. **NOW is the only work ready to execute.** NEXT, LATER, and RESEARCH items are not commitments to start early phases prematurely.

## Foundation

- [x] [NOW] Inspect the environment and establish the initial repository structure.
- [x] [NOW] Write initial development rules, architecture, ontology, roadmap, draft schemas, and privacy defaults.
- [ ] [NOW] Review the ontology and v0.1 schemas; record changes that real use requires.
- [ ] [NOW] Decide how personal/raw data will be kept separate from public or shareable source code.
- [ ] [NOW] Select a project license before any public distribution or external contribution.
- [ ] [NEXT] Record consequential architecture choices as short decision records.
- [ ] [LATER] Revisit repository layout when implementation creates real module or packaging needs.

## Knowledge ingestion

- [ ] [NEXT] Define a small, non-sensitive sample and a source-preservation acceptance test.
- [ ] [NEXT] Prototype one document format end to end without modifying the original.
- [ ] [LATER] Add formats based on actual learning-material needs, including PDF, slides, and office documents.
- [ ] [RESEARCH] Compare extraction approaches for page, slide, section, and timestamp fidelity.

## Knowledge extraction

- [ ] [LATER] Define claim-level extraction and evidence-location requirements from real examples.
- [ ] [LATER] Add human review before extracted objects are treated as accepted knowledge.
- [ ] [RESEARCH] Evaluate model-assisted extraction quality, calibration, and failure modes.

## Knowledge representation

- [ ] [NEXT] Review draft schemas against representative, non-sensitive examples.
- [ ] [LATER] Version accepted objects and preserve correction history.
- [ ] [RESEARCH] Decide whether human-readable Markdown/YAML/JSON remains adequate as the collection grows.

## Knowledge graph

- [ ] [LATER] Define a minimal relationship vocabulary from actual cross-domain links.
- [ ] [LATER] Preserve evidence and uncertainty on relationships, not only on nodes.
- [ ] [RESEARCH] Compare a simple file-based graph with database options only after a measured need appears.

## Retrieval

- [ ] [LATER] Gather representative questions and define what counts as a useful result.
- [ ] [LATER] Establish a lexical baseline before adding semantic retrieval.
- [ ] [RESEARCH] Compare hybrid lexical, semantic, and graph-based retrieval on a small reviewed corpus.

## Reasoning

- [ ] [LATER] Require answers to cite the retrieved objects and distinguish evidence from inference.
- [ ] [LATER] Represent unresolved disagreement, assumptions, and uncertainty in responses.
- [ ] [RESEARCH] Compare model providers and approaches without coupling canonical knowledge to one provider.

## Personal memory

- [ ] [LATER] Define consent, context, retention, and deletion expectations before recording sensitive experiences.
- [ ] [LATER] Capture experiences, beliefs, preferences, and reflections as distinct, time-aware objects.

## Decision modeling

- [ ] [LATER] Record decisions with context, alternatives, rationale, assumptions, and later outcomes.
- [ ] [RESEARCH] Explore how to learn decision patterns without overgeneralizing from sparse or biased examples.

## Reflection

- [ ] [LATER] Link corrections and outcomes to earlier beliefs or decisions without erasing history.
- [ ] [RESEARCH] Evaluate when a suggested memory update should require explicit user approval.

## Evaluation

- [ ] [NEXT] Define initial acceptance criteria for provenance, non-destruction, and privacy before ingestion work.
- [ ] [LATER] Build a small, human-reviewed benchmark for retrieval and answer usefulness.
- [ ] [RESEARCH] Develop tests for calibration, contradiction handling, and personalization over time.

## Interface

- [ ] [LATER] Identify the lowest-friction review and correction workflow from actual prototype use.
- [ ] [RESEARCH] Compare command-line, local web, and editor-based workflows after core behavior is understood.

## Security/privacy

- [ ] [NOW] Verify ignored data paths before adding any personal material.
- [ ] [NEXT] Threat-model local storage, backups, logs, and any future model-provider boundary.
- [ ] [LATER] Add explicit data export and deletion behavior before storing substantial personal memory.
- [ ] [RESEARCH] Assess privacy implications of external inference and telemetry before enabling either.

## Backup/export

- [ ] [NEXT] Decide where private originals and derived data will be backed up before ingestion.
- [ ] [LATER] Define a portable export and restoration test for accepted knowledge and provenance.
- [ ] [RESEARCH] Compare encrypted local backup options appropriate to the eventual data volume.

## Future research

- [ ] [RESEARCH] Study provenance models, temporal knowledge, contradiction representation, and epistemic status.
- [ ] [RESEARCH] Investigate evaluation methods for personal knowledge systems and long-term memory quality.
- [ ] [RESEARCH] Reassess graph, vector, database, agent, and cloud infrastructure only against demonstrated requirements.
