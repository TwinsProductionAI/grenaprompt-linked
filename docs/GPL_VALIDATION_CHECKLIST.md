# GPL validation checklist

## Purpose

This checklist provides a first-pass review method for GPL contracts.

It is not a runtime validator. It is a documentation-level quality gate that can later be converted into a linter or schema validator.

## 1. Required blocks

A valid minimal GPL contract should contain:

- `INTENTION`
- `EMOTION`
- `GLYPHE`
- `FLUX`

## 2. INTENTION checks

Check that `INTENTION`:

- states one main goal;
- is understandable without hidden context;
- does not include several unrelated tasks;
- avoids unsupported claims;
- can be converted into an execution route.

Good example:

```text
INTENTION: "Prepare a structured response to a customer request"
```

Weak example:

```text
INTENTION: "Make everything perfect and solve the whole business problem"
```

## 3. EMOTION checks

Check that `EMOTION` uses:

- a valid `valence`;
- an `intensity` between `0.0` and `1.0`;
- an optional but meaningful `tint`.

Recommended form:

```text
EMOTION: valence("calme") intensity(0.48) tint("professionnel")
```

Avoid using emotion as decoration. In GPL, emotion is a contextual modulation signal.

## 4. GLYPHE checks

Check that `GLYPHE`:

- contains meaningful symbolic markers;
- avoids excessive quantity;
- uses reusable labels;
- supports routing or interpretation;
- does not encode unverifiable claims as facts.

Good example:

```text
GLYPHE: glyphes(PME, CLIENT, SUPPORT, AUDIT)
```

Weak example:

```text
GLYPHE: glyphes(PERFECT, MAGIC, ABSOLUTE)
```

## 5. FLUX checks

Check that `FLUX`:

- declares a readable route;
- follows a plausible execution order;
- starts from input or request state;
- ends in an output or final state;
- does not pretend to execute code by itself.

Good example:

```text
FLUX: route(input -> classification -> draft -> validation -> output)
```

Weak example:

```text
FLUX: route(do_everything -> success)
```

## 6. Governance checks

A GPL contract should preserve:

- uncertainty;
- constraints;
- source requirements when applicable;
- risk markers when applicable;
- the difference between facts and assumptions.

## 7. Anti-patterns

Avoid:

- hidden constraints;
- vague intention;
- decorative glyphes;
- fake certainty;
- overloaded routes;
- multiple unrelated goals;
- final outputs that add unsupported facts.

## 8. Minimal review verdict

Use this simple verdict format:

```text
GPL_CHECK:
  required_blocks: pass|fail
  intention_clarity: pass|fail
  emotion_validity: pass|fail
  glyph_relevance: pass|fail
  flux_readability: pass|fail
  uncertainty_preserved: pass|fail
  final_verdict: pass|revise|reject
```

## 9. Recommended next step

This checklist can later become:

- `spec/gpl_schema_v1.json`
- `tools/gpl_lint.md`
- a runtime validation helper
- a test suite for GPL examples
