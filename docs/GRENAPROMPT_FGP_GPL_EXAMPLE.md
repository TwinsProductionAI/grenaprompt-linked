# Grenaprompt + FGP + GPL example

## Purpose

This document shows a neutral professional flow:

```text
Human Request
  -> Grenaprompt
  -> FGP Governance Frame
  -> GPL Execution Contract
```

## 0. Human request

```text
Create an AI assistant to help a small business answer customer requests professionally while making uncertainty visible.
```

## 1. Grenaprompt

Grenaprompt keeps the request readable while adding structure.

```json
{
  "task": "EN: create a client-response assistant for a small business",
  "intent": "FR: aider une PME a repondre aux demandes clients avec professionnalisme",
  "context": {
    "organization_type": "PME",
    "use_case": "support client",
    "audience": "clients externes"
  },
  "constraints": {
    "truth": "EN: do not invent facts",
    "uncertainty": "FR: signaler clairement les informations manquantes ou incertaines",
    "tone": "FR: professionnel, calme, utile",
    "output": "EN: structured response draft"
  }
}
```

## 2. FGP governance frame

FGP adds governance, stabilization and audit rules around the Grenaprompt.

```text
FGP_FRAME:
  PURPOSE:
    Stabilize a request for a small-business customer-response assistant.

  TRUTH_RULES:
    - Do not invent customer information.
    - Do not turn an assumption into a fact.
    - Keep uncertainty visible.
    - Ask for missing information when it is required.

  OUTPUT_RULES:
    - Produce a clear answer.
    - Separate known facts, assumptions and next actions.
    - Keep the format reusable by a small business.

  AUDIT_RULES:
    - Preserve the initial intention.
    - Preserve the constraints.
    - Preserve visible uncertainty markers.
```

## 3. GPL execution contract

GPL compiles the governed request into a routable execution contract.

```text
INTENTION: "Create an AI assistant for structured customer-response drafting in a small business"

EMOTION: valence("calme") intensity(0.48) tint("professionnel")

GLYPHE: glyphes(PME, CLIENT, SUPPORT, VERITE, INCERTITUDE, AUDIT)

FLUX: route(
  human_request
  -> grenaprompt_structure
  -> fgp_governance_check
  -> response_model
  -> uncertainty_marking
  -> final_output
)
```

## 4. Operational reading

```text
Grenaprompt captures the hybrid request.
FGP applies governance and audit constraints.
GPL turns the governed request into a routable execution contract.
```

## 5. Canonical sentence

```text
Grenaprompt understands. FGP governs. GPL contractualizes.
```

## 6. Downstream continuation

```text
Human Request
  -> Grenaprompt
  -> FGP Governance Frame
  -> GPL Execution Contract
  -> GPV2 / GL / GL_G
  -> NATIVE_FINAL
```
