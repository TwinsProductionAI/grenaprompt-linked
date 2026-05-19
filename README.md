# grenaprompt-linked

Language specification, white paper, and examples for GrenapromptLinked, GL, GPL, and GL_G semantic transport.

This repository is the language/protocol layer of the public ORA Core map. It is intentionally separate from the runtime and from the main ORA Core OS architecture repository.

## Repository Role

Read this when you want to understand the symbolic transport layer behind ORA Core outputs and module wiring.

| Public order | Repository role |
| ---: | --- |
| 5 | GL/GPL/GL_G language and protocol repository. |

Recommended public slug: `grenaprompt-linked`.

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

## Glossary

Use the glossary as the canonical terminology map for Grenaprompt and FGP terms:

- [Grenaprompt Glossary](docs/GRENAPROMPT_GLOSSARY.md)

## Scope

- Grenaprompt foundational material
- FGP governance material
- Grenaprompt glossary and terminology
- GrenapromptLinked (`.gpl`) reference material
- Gibberlink / GL_G (`.glg`) reference material
- white paper material
- protocol examples
- symbolic backend vocabulary for ORA-style semantic routing

## Main Files

- Foundational whitepaper: `docs/GRENAPROMPT_FOUNDATIONAL_WHITEPAPER.md`
- FGP framework: `docs/FGP_FRAMEWORK_GRENAPROMPT.md`
- Glossary: `docs/GRENAPROMPT_GLOSSARY.md`
- White paper PDF: `whitepaper/WHITE_PAPER_GRENAPROMPTLINKED_v1_Sciences_DeepDive.pdf`
- GL specification: `spec/grenapromptlinked.gpl`
- Backend cognitive protocol: `api/protocol.glg`
- Examples: `examples/*.gpl` and `examples/*.glg`

## Pipeline

```text
[INTENTION] -> [EMOTION] -> [GLYPH] -> EXECUTION
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