# System Overview

## Purpose

Personal Cognitive OS is intended to grow into a personal knowledge and reasoning system. It should preserve what was learned and experienced, connect ideas across domains, and help its owner apply relevant knowledge to new problems without losing provenance or uncertainty.

The flow below describes a long-term architecture. It is not a claim that these components exist today. Only the foundation is being established initially; the first implementation should cover a small, inspectable portion of the early stages.

## Conceptual flow

```text
RAW SOURCES
    ↓
INGESTION
    ↓
EXTRACTION
    ↓
KNOWLEDGE OBJECTS
    ↓
RELATIONSHIPS / KNOWLEDGE GRAPH
    ↓
RETRIEVAL
    ↓
REASONING
    ↓
USER RESPONSE / ACTION
    ↓
REFLECTION / LEARNING
    ↓
MEMORY UPDATE
```

## Stage responsibilities

1. **Raw sources** are the original books, slides, documents, articles, and other material. They are preserved as the source of truth and are never rewritten by processing.
2. **Ingestion** records a source and makes its content available for processing. It should retain source identity and useful location information such as page, slide, section, or timestamp.
3. **Extraction** proposes structured knowledge from a source. It must distinguish explicitly stated claims from source-based inference and AI inference, and retain supporting locations.
4. **Knowledge objects** represent distinct kinds of knowledge, such as concepts, frameworks, methods, principles, examples, experiences, and decisions. The initial ontology is deliberately small and provisional.
5. **Relationships / knowledge graph** connect objects with named, inspectable relationships. Each relationship may itself need evidence and an uncertainty status.
6. **Retrieval** finds potentially relevant sources and knowledge objects. The long-term direction may combine lexical, semantic, and graph-based retrieval; no retrieval technology is selected yet.
7. **Reasoning** uses retrieved evidence to develop an answer or recommendation. It should cite the knowledge it used, expose assumptions, and preserve disagreement rather than conceal it.
8. **User response / action** presents a useful, appropriately qualified result for the person to assess or act on.
9. **Reflection / learning** captures corrections, outcomes, and changes in understanding. It does not silently rewrite past evidence or decisions.
10. **Memory update** records accepted new knowledge, personal experience, decisions, beliefs, preferences, and reflections with their origin and time context.

## Cross-cutting requirements

- Preserve the chain `source → extracted knowledge → relationships → conclusions`.
- Represent source statements, several kinds of inference, user input, experimental validation, and uncertainty distinctly.
- Preserve contradictions and historical changes for later investigation.
- Keep canonical knowledge portable and independent of a particular model provider.
- Treat personal data as private by default; keep it out of Git unless deliberately reviewed.
- Add infrastructure only when a demonstrated need justifies it.

## Initial implementation boundary

The current repository establishes documentation, draft schemas, and folder boundaries only. It does not ingest documents, create embeddings, construct a graph, retrieve or reason over personal knowledge, call an LLM, or store personal data. The first working slice should be selected after reviewing the privacy boundary and testing the assumptions against a small, non-sensitive source.
