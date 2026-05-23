# GPL versus classic prompt

## Purpose

This note explains the difference between a classic prompt and a GPL execution contract.

## Short distinction

```text
Classic prompt: asks.
GPL contract: structures, routes and preserves auditability.
```

## Classic prompt

A classic prompt is a free-form instruction written in natural language.

It is useful when the task is simple, conversational or one-off.

Typical strengths:

- fast to write;
- natural for humans;
- flexible;
- good for exploration.

Typical limits:

- ambiguity is easy to introduce;
- constraints can be hidden inside prose;
- reuse is difficult;
- auditability is weak;
- routing is implicit;
- uncertainty can be lost.

## GPL execution contract

A GPL contract is a structured representation of a request.

It separates:

- intention;
- contextual modulation;
- symbolic markers;
- execution flow.

Typical strengths:

- clearer intent;
- reusable structure;
- explicit route;
- better auditability;
- easier integration with GPV2, GL and GL_G;
- easier validation by downstream governance layers.

Typical limits:

- more structured than a plain prompt;
- unnecessary for simple conversational tasks;
- requires shared vocabulary;
- should not be used as a substitute for truth validation.

## Comparison table

| Dimension | Classic prompt | GPL contract |
| --- | --- | --- |
| Format | Free text | Structured contract |
| Intent | Often implicit | Explicit |
| Constraints | Mixed in prose | Separated and inspectable |
| Routing | Implicit | Declared with `FLUX` |
| Reuse | Variable | Easier |
| Audit | Weak by default | Stronger by structure |
| Backend compatibility | Depends on interpretation | Designed for routing |
| Best use | Simple one-off requests | Governed, reusable or routed requests |

## Example

Classic prompt:

```text
Write a professional answer to a dissatisfied customer. Stay calm and do not invent details.
```

GPL contract:

```text
INTENTION: "Prepare a professional response to a dissatisfied customer"

EMOTION: valence("calme") intensity(0.65) tint("empathique")

GLYPHE: glyphes(CLIENT, SUPPORT, CONFIANCE, RISQUE)

FLUX: route(issue -> empathy -> solution -> uncertainty_check -> response)
```

## Rule of thumb

Use a classic prompt when speed matters more than structure.

Use GPL when structure, traceability, reuse or routing matter.

## Positioning sentence

```text
GPL does not eliminate prompting. It turns a prompt into an execution contract when the task requires structure, routing and governance.
```
