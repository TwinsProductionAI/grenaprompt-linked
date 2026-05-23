# GPL training - Level 2: Write

## Goal

Learn to convert a human request into a clean GPL contract.

Level 2 is focused on production and review.

## Required knowledge

Before this module, read:

- `docs/GPL_TRAINING_LEVEL_1_READ.md`
- `docs/GPL_VALIDATION_CHECKLIST.md`

## Writing method

Use this five-step method:

```text
1. Extract the real intention.
2. Choose the contextual modulation.
3. Select useful glyphes.
4. Build the execution flux.
5. Review the contract with the checklist.
```

## 1. Extract the real intention

Start from the human request and reduce it to one clear objective.

Human request:

```text
Can you help us answer customer emails more professionally and avoid unclear responses?
```

GPL intention:

```text
INTENTION: "Create a professional customer-email response structure"
```

Good intention rules:

- one main goal;
- clear verb;
- clear object;
- no hidden promise;
- no overloaded scope.

Weak intention:

```text
INTENTION: "Make our customer service perfect"
```

Why it is weak:

```text
It is vague, not measurable and not directly routable.
```

## 2. Choose contextual modulation

`EMOTION` defines how the task should be modulated.

Recommended pattern:

```text
EMOTION: valence("neutre") intensity(0.40) tint("professionnel")
```

Guidelines:

- use `calme` for careful support contexts;
- use `neutre` for technical or procedural work;
- use `grave` for audit or risk review;
- keep intensity moderate unless the task requires stronger modulation;
- use a useful tint such as `professionnel`, `technique`, `audit`, `pedagogique`, `operationnel`.

## 3. Select useful glyphes

Glyphes should act as compact markers for meaning and routing.

Example:

```text
GLYPHE: glyphes(CLIENT, EMAIL, SUPPORT, CLARTE)
```

Good glyphes are:

- short;
- reusable;
- meaningful;
- connected to the task;
- not decorative.

Avoid:

```text
GLYPHE: glyphes(PERFECT, MAGIC, EVERYTHING)
```

## 4. Build the execution flux

`FLUX` should describe the route from input to output.

Example:

```text
FLUX: route(email -> intent_detection -> draft -> uncertainty_check -> final_response)
```

Good flux rules:

- start from the input;
- move through useful steps;
- include validation when needed;
- end with a clear output;
- avoid impossible shortcuts.

Weak flux:

```text
FLUX: route(request -> success)
```

Why it is weak:

```text
It does not describe a useful route.
```

## 5. Review the contract

Use this minimal review:

```text
GPL_CHECK:
  required_blocks: pass
  intention_clarity: pass
  emotion_validity: pass
  glyph_relevance: pass
  flux_readability: pass
  uncertainty_preserved: pass
  final_verdict: pass
```

## Full writing example

Human request:

```text
Prepare a reusable structure for answering customer emails when information is missing.
```

GPL contract:

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

Review:

```text
GPL_CHECK:
  required_blocks: pass
  intention_clarity: pass
  emotion_validity: pass
  glyph_relevance: pass
  flux_readability: pass
  uncertainty_preserved: pass
  final_verdict: pass
```

## Common mistakes

### Mistake 1 - Writing a slogan instead of an intention

Weak:

```text
INTENTION: "Improve everything"
```

Better:

```text
INTENTION: "Create a reusable structure for customer-response drafting"
```

### Mistake 2 - Using emotion as decoration

Weak:

```text
EMOTION: valence("amazing") intensity(2.0) tint("wow")
```

Better:

```text
EMOTION: valence("calme") intensity(0.45) tint("professionnel")
```

### Mistake 3 - Using glyphes with no routing value

Weak:

```text
GLYPHE: glyphes(SUPER, BEST, FAST)
```

Better:

```text
GLYPHE: glyphes(CLIENT, SUPPORT, QUALITE, AUDIT)
```

### Mistake 4 - Writing a route with no real steps

Weak:

```text
FLUX: route(input -> perfect_output)
```

Better:

```text
FLUX: route(input -> classification -> draft -> review -> output)
```

## Level 2 completion checklist

The learner can:

- turn a human request into one clear intention;
- choose valid contextual modulation;
- select useful glyphes;
- build a readable flux;
- review a GPL contract with the checklist;
- revise weak GPL contracts.

## Mini-test

Convert this request into GPL:

```text
Create a simple internal guide that explains how to review AI-generated answers before sending them to clients.
```

Expected output:

```text
INTENTION: ...
EMOTION: ...
GLYPHE: ...
FLUX: ...
```
