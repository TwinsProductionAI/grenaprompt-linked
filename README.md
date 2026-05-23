# grenaprompt-linked

Language specification, white paper, and examples for GrenapromptLinked, GL, GPL, and GL_G semantic transport.

This repository is the language/protocol layer of the public ORA Core map. It is intentionally separate from the runtime and from the main ORA Core OS architecture repository.

## Repository Role

Read this when you want to understand the symbolic transport layer behind ORA Core outputs and module wiring.

| Public order | Repository role |
| ---: | --- |
| 5 | GL/GPL/GL_G language and protocol repository. |

## Foundational Grenaprompt Layer

Start here for the base definition of Grenaprompt before reading the later protocol layers:

- [Grenaprompt Foundational Whitepaper](docs/GRENAPROMPT_FOUNDATIONAL_WHITEPAPER.md)

Core foundation:

```text
Grenaprompt = JSON + EN + FR
JSON = structural container
EN = technical precision
FR = emotion, intention, and human context
```

## FGP Governance Layer

The FGP, or Framework GrenaPrompt, is the governance framework around Grenaprompt.

- [FGP Framework GrenaPrompt](docs/FGP_FRAMEWORK_GRENAPROMPT.md)

Core distinction:

```text
Grenaprompt = hybrid language
FGP = governance, stabilization, and audit framework around that language
```

## GPL Execution Contract Layer

GPL, or GrenapromptLinked, is the routable execution-contract layer derived from a governed request.

Start here for the public GPL documentation path:

1. [GPL in 5 minutes](docs/GPL_IN_5_MINUTES.md)
2. [GPL glossary](docs/GPL_GLOSSARY.md)
3. [Grenaprompt + FGP + GPL example](docs/GRENAPROMPT_FGP_GPL_EXAMPLE.md)
4. [GPL versus classic prompt](docs/GPL_VS_CLASSIC_PROMPT.md)
5. [GPL validation checklist](docs/GPL_VALIDATION_CHECKLIST.md)
6. [Professional GPL examples v1](examples/gpl_professional_examples_v1.md)

Core distinction:

```text
Grenaprompt understands.
FGP governs.
GPL contractualizes.
```

GPL is not the GNU General Public License. In this repository, GPL means GrenapromptLinked execution contract.

## GPL Training Path

Use this path to teach GPL progressively:

1. [GPL training curriculum](docs/GPL_TRAINING_CURRICULUM.md)
2. [Level 1 - Read GPL](docs/GPL_TRAINING_LEVEL_1_READ.md)
3. [Level 2 - Write GPL](docs/GPL_TRAINING_LEVEL_2_WRITE.md)
4. [Level 3 - Compile GPL](docs/GPL_TRAINING_LEVEL_3_COMPILE.md)
5. [GPL training exercises v1](examples/gpl_training_exercises_v1.md)

Training progression:

```text
Read -> Write -> Compile -> Review
```

## Gibberlink Layer

Gibberlink is the compact symbolic state language used for `.glg` state, vectors, flux and priority representations.

- [Gibberlink Foundational Whitepaper](docs/GIBBERLINK_FOUNDATIONAL_WHITEPAPER.md)
- [Gibberlink Glossary](docs/GIBBERLINK_GLOSSARY.md)

Core foundation:

```text
Gibberlink = symbolic compact state
Gibberlink = vectors + energy_flux + priority
```

## Gibberlink_Glyph Layer

Gibberlink_Glyph is the optional glyph and phonetic bridge above Gibberlink.

- [Gibberlink_Glyph Foundational Note](docs/GIBBERLINK_GLYPH_FOUNDATIONAL_NOTE.md)
- [Gibberlink_Glyph Glossary](docs/GIBBERLINK_GLYPH_GLOSSARY.md)

Core distinction:

```text
Gibberlink = symbolic compact state
Gibberlink_Glyph = optional glyph / phonetic bridge
```

## GLK Layer

GLK is the canonical key syntax for archive, identity, retrieval and semantic indexing.

- [GLK Foundational Note](docs/GLK_FOUNDATIONAL_NOTE.md)

Core foundation:

```text
GLK[[TYPE:TAG.INDEX.DATE]]
GLK = TYPE + TAG + INDEX + DATE
```

## Glossary

Use the glossary as the canonical terminology map for Grenaprompt and FGP terms:

- [Grenaprompt Glossary](docs/GRENAPROMPT_GLOSSARY.md)
- [GPL Glossary](docs/GPL_GLOSSARY.md)

## Scope

- Grenaprompt foundational material
- FGP governance material
- Grenaprompt glossary and terminology
- GPL execution-contract documentation
- GPL training curriculum and exercises
- GPL professional examples and validation checklist
- Gibberlink foundational material
- Gibberlink glossary and terminology
- Gibberlink_Glyph foundational material
- Gibberlink_Glyph glossary and terminology
- GLK canonical key syntax
- GrenapromptLinked (`.gpl`) reference material
- Gibberlink / GL_G (`.glg`) reference material
- white paper material
- protocol examples
- symbolic backend vocabulary for ORA-style semantic routing

## Main Files

- Foundational whitepaper: `docs/GRENAPROMPT_FOUNDATIONAL_WHITEPAPER.md`
- FGP framework: `docs/FGP_FRAMEWORK_GRENAPROMPT.md`
- Grenaprompt glossary: `docs/GRENAPROMPT_GLOSSARY.md`
- GPL in 5 minutes: `docs/GPL_IN_5_MINUTES.md`
- GPL glossary: `docs/GPL_GLOSSARY.md`
- Grenaprompt + FGP + GPL example: `docs/GRENAPROMPT_FGP_GPL_EXAMPLE.md`
- GPL versus classic prompt: `docs/GPL_VS_CLASSIC_PROMPT.md`
- GPL validation checklist: `docs/GPL_VALIDATION_CHECKLIST.md`
- GPL training curriculum: `docs/GPL_TRAINING_CURRICULUM.md`
- GPL training level 1 read: `docs/GPL_TRAINING_LEVEL_1_READ.md`
- GPL training level 2 write: `docs/GPL_TRAINING_LEVEL_2_WRITE.md`
- GPL training level 3 compile: `docs/GPL_TRAINING_LEVEL_3_COMPILE.md`
- GPL training exercises: `examples/gpl_training_exercises_v1.md`
- Professional GPL examples: `examples/gpl_professional_examples_v1.md`
- Gibberlink foundational whitepaper: `docs/GIBBERLINK_FOUNDATIONAL_WHITEPAPER.md`
- Gibberlink glossary: `docs/GIBBERLINK_GLOSSARY.md`
- Gibberlink_Glyph foundational note: `docs/GIBBERLINK_GLYPH_FOUNDATIONAL_NOTE.md`
- Gibberlink_Glyph glossary: `docs/GIBBERLINK_GLYPH_GLOSSARY.md`
- GLK foundational note: `docs/GLK_FOUNDATIONAL_NOTE.md`
- White paper PDF: `whitepaper/WHITE_PAPER_GRENAPROMPTLINKED_v1_Sciences_DeepDive.pdf`
- GL specification: `spec/grenapromptlinked.gpl`
- Backend cognitive protocol: `api/protocol.glg`
- Examples: `examples/*.gpl` and `examples/*.glg`

## Pipeline

```text
[INTENTION] -> [EMOTION] -> [GLYPH] -> EXECUTION
```

Expanded public documentation path:

```text
Human Request
  -> Grenaprompt
  -> FGP Governance Frame
  -> GPL Execution Contract
  -> GPV2 / GL / GL_G
  -> NATIVE_FINAL
```

## Design Boundary

This is a language/protocol repository. It should not become the runtime, the RAG layer, or the main ORA Core OS architecture repository.

Related repositories:

- [ora-core-os](https://github.com/TwinsProductionAI/ora-core-os): main architecture and install order.
- [ora-core-runtime](https://github.com/TwinsProductionAI/ora-core-runtime): runnable runtime and tests.
- [ora-core-specs](https://github.com/TwinsProductionAI/ora-core-specs): technical specifications and white papers.

## HALO Note

This repository may include HALO_ORA.v3 vocabulary and energy-ratio examples. Treat those values as protocol/specification material unless a linked audit explicitly provides current runtime measurements.

## License

Copyright Twins Productions 2025. See repository license files for reuse terms.