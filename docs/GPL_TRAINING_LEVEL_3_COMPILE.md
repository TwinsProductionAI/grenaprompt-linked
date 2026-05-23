# GPL training - Level 3: Compile

## Goal

Understand how a GPL contract can continue toward GPV2, GL, GL_G and a final human-facing render.

Level 3 is conceptual. It does not define a runtime implementation.

## Required knowledge

Before this module, read:

- `docs/GPL_TRAINING_LEVEL_1_READ.md`
- `docs/GPL_TRAINING_LEVEL_2_WRITE.md`
- `docs/GRENAPROMPT_FGP_GPL_EXAMPLE.md`

## Compilation path

A professional GPL flow can be represented as:

```text
Human Request
  -> Grenaprompt
  -> FGP Governance Frame
  -> GPL Execution Contract
  -> GPV2 Packet
  -> GL Truth Layer
  -> GL_G Route Layer
  -> NATIVE_FINAL
```

## Step 1 - GPL contract

Input GPL:

```text
INTENTION: "Prepare a reusable customer-email response structure for cases with missing information"

EMOTION: valence("calme") intensity(0.52) tint("professionnel")

GLYPHE: glyphes(CLIENT, EMAIL, SUPPORT, INCERTITUDE, REUSE)

FLUX: route(
  customer_email
  -> identify_known_information
  -> identify_missing_information
  -> draft_response
  -> final_check
)
```

## Step 2 - GPV2-style compact packet

A GPV2-style packet keeps the same intent but makes it compact and governed.

```text
GPV2{
  MODE:RESPONSE_STRUCTURE;
  INTENT:customer_email_response_structure;
  LIMIT:preserve_missing_information;
  LIMIT:no_unsupported_claims;
  OUT:structured_response_model;
  ROUTE:customer_email>known_info>missing_info>draft>final_check
}
```

## Step 3 - GL truth layer

GL should preserve limits, facts, uncertainty and risk markers.

```text
LIMIT(output,structured_response_model)
LIMIT(truth,no_unsupported_claims)
LIMIT(uncertainty,preserve_missing_information)
STATE(intent,response_structure)
RISK(low)
UNSURE(customer_specific_details,requires_input,0.60)
```

Important rule:

```text
A compilation step must not increase certainty artificially.
```

## Step 4 - GL_G route layer

GL_G compresses indexes, tags, routes and uncertainty carry.

```text
IDX(task.customer_response_structure)
TAG(domain,customer_support)
TAG(output,structured_response_model)
TAG(uncertainty,preserve_missing_information)
ROUTE(module,ora_compiler_core)
PACK(route,customer_email_known_info_missing_info_draft_final_check)
STAT(risk=low,uq=0.40)
```

## Step 5 - NATIVE_FINAL render

The final render should be useful and faithful to the governed backend state.

```text
Here is a reusable customer-email response structure. It separates known information, missing information, a professional draft and a final review step before sending.
```

## Preservation rules

During compilation, preserve:

- original intention;
- visible uncertainty;
- output constraints;
- route meaning;
- risk markers when applicable;
- distinction between facts and assumptions.

## Do not do this

Do not compile:

```text
UNSURE(customer_specific_details,requires_input,0.60)
```

into:

```text
FACT(customer_specific_details,complete,0.99)
```

That would artificially increase certainty.

## Level 3 review checklist

```text
COMPILE_CHECK:
  intent_preserved: pass|fail
  limits_preserved: pass|fail
  uncertainty_preserved: pass|fail
  route_preserved: pass|fail
  no_new_facts_added: pass|fail
  final_render_faithful: pass|fail
  verdict: pass|revise|reject
```

## Mini-test

Take this GPL contract:

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
