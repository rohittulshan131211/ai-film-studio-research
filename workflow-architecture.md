# Workflow Architecture

## Core entities

| Entity | Purpose |
|---|---|
| Project | Holds overall production settings and source material |
| Script | Source narrative or creative brief |
| Asset | Character, environment, prop, or style reference |
| Scene | A time-bounded visual and narrative unit |
| Prompt | Structured instruction for image or video generation |
| Generation job | A tracked generation request and its result |
| Review record | A human approval, rejection, or revision decision |
| Export package | Approved files and metadata prepared for local editing |

## Proposed workflow

1. Ingest a script and create a production plan.
2. Define and approve reusable character, environment, and prop references.
3. Bind the relevant references to every scene.
4. Generate one controlled output for each job.
5. Record the result and conduct human review.
6. Regenerate only failed or rejected items.
7. Export approved assets and metadata for editing and publishing.

## Design principles

- **Traceability:** every output links back to its scene, prompt, references, and review decision.
- **Consistency:** reusable references are explicit rather than recreated for each scene.
- **Control:** generation is queued, measurable, and recoverable.
- **Human oversight:** the creator remains responsible for creative and publishing decisions.

## What will be evaluated

The research will examine whether this structure improves practical production work: asset consistency, prompt reuse, error recovery, review clarity, and the time creators spend coordinating a multi-scene project.
