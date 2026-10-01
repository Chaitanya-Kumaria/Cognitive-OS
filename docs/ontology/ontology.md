# Initial Ontology

This is a conceptual, provisional vocabulary for distinguishing what the system may eventually store. It is intentionally not a complete taxonomy or a final database design. Revise it as real material reveals useful distinctions.

| Type | What it represents | Why it exists | Possible relationships |
| --- | --- | --- | --- |
| **Source** | An original or user-provided artifact, such as a book, slide deck, article, or interview. | Preserves the evidence and its identity. | contains claims; supports or contradicts objects; has authors, locations, and versions. |
| **Fact** | A claim represented as established within a stated scope and evidence context. | Separates supported claims from ideas, interpretations, and guesses. | supported by sources or observations; may be challenged or contradicted. |
| **Concept** | An idea, construct, or term used to understand a subject. | Gives a reusable unit of meaning across sources and domains. | defined by sources; used by frameworks and methods; related to other concepts. |
| **Framework** | An organized set of concepts or dimensions used to analyze or structure a situation. | Captures an applicable structure rather than a loose list of notes. | uses concepts; supports methods; applies to examples or problems. |
| **Theory** | An explanatory account of how or why a phenomenon occurs. | Distinguishes explanatory propositions from descriptive labels or practical recipes. | explains phenomena; uses concepts; supported, challenged, or compared by evidence. |
| **Principle** | A general rule, value, or proposition intended to guide judgment or action. | Records durable guidance separately from a specific tactic. | informs decisions and methods; may derive from experience or sources. |
| **Method** | A procedure or repeatable way to perform a task or investigate a question. | Makes actionable practices identifiable and reusable. | implements principles; uses frameworks; can be applied in experiences. |
| **Heuristic** | A practical rule of thumb that can aid judgment but is not guaranteed to be correct. | Preserves useful shortcuts without overstating their reliability. | informs decisions; may have conditions, exceptions, and supporting experiences. |
| **Example** | A concrete illustration of an idea, framework, method, or claim. | Grounds abstractions and helps compare applications. | illustrates or instantiates other objects; may come from a source or experience. |
| **Experience** | A personally observed event or situation, with context and interpretation kept distinguishable. | Gives personal memory a first-class place alongside published knowledge. | has actions and outcomes; informs reflections, beliefs, or decisions. |
| **Decision** | A choice made in a particular context, including alternatives and rationale when known. | Preserves the reasoning and constraints behind consequential choices. | responds to a question or situation; uses principles or evidence; has outcomes. |
| **Outcome** | An observed or reported result following an action, method, or decision. | Allows later reflection to compare intent with what happened. | follows decisions or methods; may support or challenge beliefs and hypotheses. |
| **Belief** | A proposition the person currently accepts, with degree, context, and history left explicit. | Captures personal understanding without presenting it as universal fact. | supported or challenged by sources and experiences; can change over time. |
| **Preference** | A stated tendency, value, or favored option in a context. | Helps tailor future recommendations while avoiding assumptions from sparse evidence. | informs decisions; may be context-dependent and revised by reflection. |
| **Hypothesis** | A provisional, testable explanation or prediction. | Keeps ideas to investigate distinct from established claims. | motivated by observations or theory; tested by methods; updated by outcomes. |
| **Question** | An explicit unknown, inquiry, or open problem. | Preserves learning needs and directs investigation. | prompted by sources, experiences, or decisions; answered by evidence or reasoning. |
| **Reflection** | A retrospective interpretation of an experience, decision, or outcome. | Captures lessons and corrections without rewriting what originally happened. | refers to experiences and outcomes; may revise beliefs or suggest hypotheses. |

## Cross-cutting attributes

Types above describe what an object is; epistemic status describes where a statement came from. At minimum, distinguish: explicitly stated by a source, inferred from a source, inferred by AI, provided by the user, experimentally validated, and uncertain. These categories must not be silently converted into one another.

Knowledge objects and relationships should have stable identifiers and carry provenance references when derived from a source. Provenance should point as specifically as available from source file to page, slide, section, timestamp, or supporting span. User-provided personal memory can cite the user as its origin even when it has no external source file.

Contradictory sources or beliefs are allowed to coexist. A conflict is something to represent and investigate, not a reason to discard one side. The ontology does not yet prescribe a formal contradiction model, confidence score, identity system, or storage engine.
