# GPL in 5 minutes

GPL, or GrenapromptLinked, is an execution-contract layer for AI instructions.

It transforms a human request into a structured, routable, auditable and reusable instruction contract.

```text
Human request -> GPL execution contract -> backend route -> controlled output
```

## One sentence definition

```text
GPL is a semantic execution contract that turns a human request into a structured, routable, auditable and reusable AI instruction.
```

## What GPL is

GPL captures four core elements:

- `INTENTION`: what the user wants to achieve.
- `EMOTION`: the contextual modulation of the task.
- `GLYPHE`: symbolic markers used for routing or interpretation.
- `FLUX`: the expected execution flow.

A GPL message is not a plain prompt. It is a structured contract between the human request and the execution pipeline.

## What GPL is not

GPL is not:

- the GNU General Public License;
- a complete programming language;
- a decorative prompt style;
- a proof of truth by itself;
- an automatic execution guarantee.

GPL structures intent. Governance and validation remain the responsibility of the surrounding ORA Core layers.

## Relationship with Grenaprompt and FGP

```text
Grenaprompt = hybrid human-machine prompt language
FGP         = governance, stabilization and audit framework around Grenaprompt
GPL         = routable execution contract derived from the governed request
```

Short form:

```text
Grenaprompt understands.
FGP governs.
GPL contractualizes.
```

## Minimal professional example

Human request:

```text
Create an AI assistant to help a small business answer customer requests professionally, while making uncertainty visible.
```

GPL contract:

```text
INTENTION: "Create an AI assistant for structured customer-response drafting in a small business"

EMOTION: valence("calme") intensity(0.48) tint("professionnel")

GLYPHE: glyphes(PME, CLIENT, SUPPORT, VERITE, INCERTITUDE, AUDIT)

FLUX: route(
  human_request
  -> governed_structure
  -> response_model
  -> uncertainty_marking
  -> final_output
)
```

## Why GPL matters

Classic prompts are flexible but often ambiguous. GPL keeps the flexibility of human intent while adding explicit structure.

```text
Classic prompt: asks.
GPL contract: structures, routes and preserves auditability.
```

## Canonical flow

```text
Human Request
  -> Grenaprompt
  -> FGP Governance Frame
  -> GPL Execution Contract
  -> GPV2 / GL / GL_G
  -> NATIVE_FINAL
```
