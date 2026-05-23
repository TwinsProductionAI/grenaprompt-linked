# GPL training - Level 1: Read

## Goal

Learn to read a GPL contract and explain it in plain language.

Level 1 is focused on comprehension, not production.

## Required knowledge

Before this module, read:

- `docs/GPL_IN_5_MINUTES.md`
- `docs/GPL_GLOSSARY.md`

## The four GPL blocks

A minimal GPL contract contains:

```text
INTENTION
EMOTION
GLYPHE
FLUX
```

## 1. Read INTENTION

`INTENTION` answers:

```text
What is the user trying to achieve?
```

Example:

```text
INTENTION: "Prepare a professional response to a dissatisfied customer"
```

Plain-language reading:

```text
The user wants a professional customer-support response.
```

Review questions:

- Is the goal clear?
- Is there one main objective?
- Is the objective actionable?

## 2. Read EMOTION

`EMOTION` answers:

```text
How should the system modulate the task?
```

Example:

```text
EMOTION: valence("calme") intensity(0.65) tint("empathique")
```

Plain-language reading:

```text
The answer should be calm, moderately careful and empathetic.
```

Review questions:

- Is the valence understandable?
- Is the intensity between 0.0 and 1.0?
- Does the tint add useful context?

## 3. Read GLYPHE

`GLYPHE` answers:

```text
Which symbolic markers guide interpretation or routing?
```

Example:

```text
GLYPHE: glyphes(CLIENT, SUPPORT, CONFIANCE, RISQUE)
```

Plain-language reading:

```text
The contract relates to customer support, trust and risk-aware response handling.
```

Review questions:

- Are the glyphes meaningful?
- Are they reusable?
- Do they support the task?

## 4. Read FLUX

`FLUX` answers:

```text
What execution route should the system follow?
```

Example:

```text
FLUX: route(issue -> empathy -> solution -> uncertainty_check -> response)
```

Plain-language reading:

```text
The system should understand the issue, respond with empathy, propose a solution, check uncertainty and produce the final response.
```

Review questions:

- Does the route have a logical order?
- Does it start from an input state?
- Does it end in a useful output?

## Full reading example

GPL contract:

```text
INTENTION: "Create a structured internal process summary"
EMOTION: valence("neutre") intensity(0.40) tint("operationnel")
GLYPHE: glyphes(PROCESS, STEPS, REUSE, AUDIT)
FLUX: route(input -> extraction -> ordering -> validation -> final_steps)
```

Plain-language interpretation:

```text
The user wants a reusable internal-process summary. The tone is neutral and operational. The important markers are process, steps, reuse and audit. The expected route is to extract the process, order it, validate it and produce final reusable steps.
```

## Level 1 completion checklist

The learner can:

- identify the four GPL blocks;
- explain each block in plain language;
- detect a vague intention;
- detect invalid or decorative emotion;
- detect weak glyphes;
- detect an unreadable route.

## Mini-test

Read this contract:

```text
INTENTION: "Create a concise meeting agenda for a product review"
EMOTION: valence("neutre") intensity(0.35) tint("coordination")
GLYPHE: glyphes(MEETING, PRODUCT, PRIORITY, DECISION)
FLUX: route(context -> objectives -> topics -> decisions -> agenda)
```

Answer:

1. What is the main goal?
2. What is the tone?
3. What do the glyphes indicate?
4. What route is expected?
5. Is the contract readable?
