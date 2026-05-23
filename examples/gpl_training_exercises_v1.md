# GPL training exercises v1

## Purpose

This exercise pack supports the GPL training curriculum.

It contains drills for:

- Level 1: reading GPL;
- Level 2: writing GPL;
- Level 3: compiling GPL conceptually.

## Level 1 - Reading exercises

### Exercise 1

Read the contract:

```text
INTENTION: "Create a concise meeting agenda for a product review"
EMOTION: valence("neutre") intensity(0.35) tint("coordination")
GLYPHE: glyphes(MEETING, PRODUCT, PRIORITY, DECISION)
FLUX: route(context -> objectives -> topics -> decisions -> agenda)
```

Answer:

1. What is the main goal?
2. What is the contextual modulation?
3. What do the glyphes indicate?
4. What is the execution route?
5. Is the contract readable?

### Exercise 2

Read the contract:

```text
INTENTION: "Review an AI answer and identify unsupported claims"
EMOTION: valence("grave") intensity(0.55) tint("audit")
GLYPHE: glyphes(AUDIT, CLAIM, SOURCE, RISQUE)
FLUX: route(answer -> claim_extraction -> source_check -> risk_marking -> verdict)
```

Answer:

1. What is the task?
2. Why is the tint `audit` useful?
3. Which part of the route preserves governance?
4. What uncertainty may need to remain visible?

## Level 2 - Writing exercises

### Exercise 3

Convert this request into GPL:

```text
Create a simple internal guide that explains how to review AI-generated answers before sending them to clients.
```

Expected structure:

```text
INTENTION: ...
EMOTION: ...
GLYPHE: ...
FLUX: ...
```

### Exercise 4

Convert this request into GPL:

```text
Summarize a project idea into a reusable markdown brief for internal discussion.
```

Expected structure:

```text
INTENTION: ...
EMOTION: ...
GLYPHE: ...
FLUX: ...
```

### Exercise 5

Improve this weak GPL contract:

```text
INTENTION: "Make support better"
EMOTION: valence("great") intensity(1.5) tint("wow")
GLYPHE: glyphes(BEST, MAGIC, FAST)
FLUX: route(request -> success)
```

Tasks:

1. Rewrite the intention.
2. Replace the emotion with a valid modulation.
3. Replace decorative glyphes with useful ones.
4. Rewrite the route.
5. Apply the validation checklist.

## Level 3 - Compilation exercises

### Exercise 6

Compile this GPL contract conceptually:

```text
INTENTION: "Create a short internal guide for reviewing AI-generated answers before client delivery"
EMOTION: valence("grave") intensity(0.55) tint("audit")
GLYPHE: glyphes(AI, REVIEW, CLIENT, AUDIT, VERITE)
FLUX: route(answer -> claim_check -> uncertainty_check -> revision -> approval)
```

Produce:

1. a GPV2-style packet;
2. a GL truth layer;
3. a GL_G route layer;
4. a faithful NATIVE_FINAL render.

### Exercise 7

Compile this GPL contract conceptually:

```text
INTENTION: "Prepare a reusable response structure for customer emails when information is missing"
EMOTION: valence("calme") intensity(0.52) tint("professionnel")
GLYPHE: glyphes(CLIENT, EMAIL, SUPPORT, INCERTITUDE, REUSE)
FLUX: route(customer_email -> known_information -> missing_information -> draft -> final_check)
```

Produce:

1. a GPV2-style packet;
2. a GL truth layer;
3. a GL_G route layer;
4. a faithful NATIVE_FINAL render;
5. a compile check verdict.

## Answer key - sample responses

### Exercise 3 sample

```text
INTENTION: "Create an internal guide for reviewing AI-generated answers before client delivery"
EMOTION: valence("grave") intensity(0.50) tint("audit")
GLYPHE: glyphes(AI, REVIEW, CLIENT, VERITE, AUDIT)
FLUX: route(answer -> claim_check -> uncertainty_check -> revision -> approval)
```

### Exercise 4 sample

```text
INTENTION: "Summarize a project idea into a reusable markdown brief"
EMOTION: valence("neutre") intensity(0.42) tint("production")
GLYPHE: glyphes(PROJECT, MARKDOWN, BRIEF, REUSE)
FLUX: route(idea -> scope -> structure -> markdown -> review)
```

### Exercise 5 sample improvement

```text
INTENTION: "Create a clearer customer-support response process"
EMOTION: valence("calme") intensity(0.45) tint("professionnel")
GLYPHE: glyphes(CLIENT, SUPPORT, CLARTE, QUALITE)
FLUX: route(request -> classification -> draft -> review -> response)
```

## Review rubric

```text
PASS:
  Required blocks are present, readable and aligned.

REVISE:
  Structure exists but intention, glyphes or flux need clarification.

REJECT:
  Required blocks are missing, invalid or misleading.
```
