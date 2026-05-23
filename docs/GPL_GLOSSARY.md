# GPL glossary

This glossary defines the core vocabulary used by GPL, or GrenapromptLinked, as an execution-contract layer.

## Core terms

### GPL

GrenapromptLinked. A semantic execution contract that turns a governed human request into a structured, routable and reusable instruction.

### Prompt

A free-form human instruction. A prompt can be useful, but it is often ambiguous and difficult to audit without additional structure.

### Contract

A structured representation of a request. In GPL, the contract separates intention, contextual modulation, symbolic routing markers and execution flow.

### INTENTION

The actual goal of the user request.

Example:

```text
INTENTION: "Create a structured customer-response assistant for a small business"
```

### EMOTION

The contextual modulation applied to the request. It does not mean uncontrolled emotion. It describes tone, intensity and contextual tint.

Canonical form:

```text
EMOTION: valence("calme") intensity(0.48) tint("professionnel")
```

### valence

The qualitative tone of the request. Examples: `calme`, `neutre`, `tendu`, `joyeux`, `grave`, `colere`, `triste`.

### intensity

A numeric modulation value between `0.0` and `1.0`.

### tint

An optional contextual color or orientation, such as `professionnel`, `audit`, `support`, `strategique` or `technique`.

### GLYPHE

A symbolic marker or set of markers used to support routing, interpretation or semantic indexing.

Example:

```text
GLYPHE: glyphes(PME, CLIENT, SUPPORT, VERITE, AUDIT)
```

### glyphes

The list of symbolic markers associated with the request. Glyphes should stay compact, meaningful and reusable.

### FLUX

The expected execution flow. It defines how the request should move from input to output.

Example:

```text
FLUX: route(input -> classification -> draft -> validation -> output)
```

### route

A declared execution path. A route should be clear enough to guide downstream interpretation without pretending to execute code by itself.

### PROMPT.gpl

A GPL-formatted prompt contract.

### EXEC_STATE.glg

A compressed backend state emitted by a GL_G-compatible layer after reading a GPL contract.

### Grenaprompt

The hybrid human-machine prompt layer. It uses a structured container and natural-language intention to represent the request before governance and compilation.

### FGP

Framework GrenaPrompt. The governance, stabilization and audit frame around Grenaprompt.

### GL

A constrained semantic layer used for truth, limits, facts, sources, uncertainty and risk.

### GL_G

A compact backend layer used for indexes, tags, routes, packed state and uncertainty carry.

### GPV2

A compact governed execution packet derived from a structured and governed request.

### NATIVE_FINAL

The final human-facing render. It should remain faithful to the governed backend state and should not add unsupported facts.

## Practical rule

```text
Grenaprompt understands.
FGP governs.
GPL contractualizes.
GL / GL_G route and preserve controlled backend state.
```
