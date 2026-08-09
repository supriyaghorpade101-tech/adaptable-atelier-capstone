# Adaptable Atelier

Adaptable Atelier is an agentic AI prototype that guides customers through an adaptive-clothing consultation, recommends grounded adaptive features, and creates a draft garment specification for customer approval and human-designer review.

## Working prototype

[Open the public demonstration](https://supriyaghorpade101-tech.github.io/adaptable-atelier-capstone/?public-demo=1)

The public demonstration uses synthetic data and pre-scripted agent responses so assessors can explore the workflow without an API key. The local development version uses OpenAI GPT-5 mini through a secure launcher.

## Demonstrated workflow

1. The customer describes the garment, accessibility needs and style preferences.
2. Adaptable Atelier asks targeted follow-up questions and flags conflicting requirements.
3. Adaptive features are grounded in individually citable Knowledge Base entries.
4. The customer approves the concept before garment-specific measurements are collected.
5. The prototype creates an annotated sketch and simplified manufacturing specification.
6. The customer approves the specification before simulated handoff to a human designer.

The agent refuses medical advice and unsafe requests. It hands consultations to a human when the Knowledge Base does not support the need, the customer requests a person, two concept revisions have been rejected, or essential questions remain unanswered after two attempts.

## Evaluation

Nine synthetic evaluation cases cover:

- Happy path and citation grounding
- Production-measurement gate
- Revision limit and human escalation
- Medical-advice boundary
- Unsafe request
- Conflicting requirements
- Knowledge Base gap
- Medical-device context that is not medical advice
- A supported feature with unsuitable customer-specific placement

## Repository contents

- `index.html` — self-contained public prototype
- `data/` — synthetic customer, consultation, Knowledge Base, example and evaluation records
- `policies/` — consultation-completeness and safety/escalation rules

## Safety and limitations

All records are fictional. No real customer or medical records are used, and no API key is stored in this repository. The sketches and specifications are demonstration outputs rather than validated CAD drawings or production patterns. Every final specification requires review by a qualified human designer or pattern-maker before production.
