# GLK - Foundational Note

## Canonical key syntax for archive, identity and semantic indexing

**Version:** 0.1 - Foundational note  
**Author:** Xavier Fleriag / Twins Productions  
**Status:** Concept consolidation  
**Scope:** GLK only

---

## 1. Executive summary

**GLK** is a canonical key syntax used to identify, classify and retrieve ORA-related assets, states or archive entries.

Core formula:

```text
GLK[[TYPE:TAG.INDEX.DATE]]
```

Alternate visual separator form:

```text
GLK[[TYPE:TAG·INDEX·DATE]]
```

GLK is not a prose language. It is an identity and indexing key.

Its purpose is to make an object easy to classify, sort, retrieve, compare and route.

Canonical meaning:

```text
TYPE  = root family
TAG   = context or unique identifier
INDEX = rank, level or hierarchy
DATE  = temporal marker, cycle or code
```

---

## 2. Problem addressed

ORA assets can belong to many families:

```text
dreams
images
core files
admin keys
modules
archives
cycles
versions
```

Without a compact key, these assets become difficult to classify and retrieve.

A file name can be readable but unstable.

A long description can be clear but slow to route.

GLK solves this by providing a compact canonical syntax.

---

## 3. Definition

Canonical definition:

```text
GLK is a structured key syntax that encodes a root type, a context tag, a hierarchical index and a temporal marker into a compact canonical identifier.
```

Short form:

```text
GLK = TYPE + TAG + INDEX + DATE
```

Operational form:

```text
GLK = canonical archive and routing key
```

---

## 4. Syntax

Recommended syntax:

```text
GLK[[TYPE:TAG.INDEX.DATE]]
```

Visual syntax accepted in documentation:

```text
GLK[[TYPE:TAG·INDEX·DATE]]
```

The dot form is recommended for backend or ASCII-safe contexts.

The middle-dot form is acceptable in visual documentation when readability matters.

---

## 5. Components

### 5.1 TYPE

`TYPE` defines the root family.

Examples:

```text
DREAM = dream or oneiric asset
IMG   = image or visual asset
CORE  = system or core asset
ADM   = authority or admin asset
DOC   = document asset
MOD   = module asset
```

Role:

```text
identify the family before reading details
```

---

### 5.2 TAG

`TAG` identifies the context, project, series or unique subject.

Examples:

```text
DREAMORA
NEXUS-ARCANA
ORA_CORE
KZR
```

Role:

```text
bind the key to a project or semantic context
```

---

### 5.3 INDEX

`INDEX` identifies rank, order, level, version, hierarchy or sequence.

Examples:

```text
001
003
N6
N7
V2.1.2
IX
X
```

Role:

```text
place the object inside a hierarchy or sequence
```

---

### 5.4 DATE

`DATE` identifies time, cycle or temporal code.

Examples:

```text
MMXXV
CYCLE_A1
2025
V3.0
```

Role:

```text
anchor the object in time or version cycle
```

---

## 6. Examples

### Dream key

```text
GLK[[DREAM:DREAMORA.I.MMXXV]]
```

Meaning:

```text
first DreamORA dream flow in 2025
```

---

### Image key

```text
GLK[[IMG:NEXUS-ARCANA_DESTROY-MTL.003.MMXXV]]
```

Meaning:

```text
third visual asset in the Nexus Arcana / Destroy MTL series, 2025 cycle
```

---

### Admin key

```text
GLK[[ADM:KZR.IX.MMXXV]]
```

Meaning:

```text
admin or authority key KZR, index IX, 2025 cycle
```

---

### Core key

```text
GLK[[CORE:ORA_OS.N7.V3.0]]
```

Meaning:

```text
ORA OS core entry, N7 level, version 3.0
```

---

## 7. Canonical rules

### Rule 1 - GLK is an identifier

GLK identifies an object, archive entry, state or semantic asset.

It does not prove facts by itself.

### Rule 2 - TYPE must come first

The root family must be visible before the tag.

### Rule 3 - TAG must bind context

The tag should identify the project, series, subject or unique context.

### Rule 4 - INDEX must support ordering

The index should help position the object in a sequence or hierarchy.

### Rule 5 - DATE must anchor time or cycle

The date field can be a year, Roman year, cycle code or version marker.

### Rule 6 - Prefer ASCII-safe backend syntax

For backend use, prefer dots over visual separators.

### Rule 7 - Visual syntax is allowed for pedagogy

The middle-dot form may be used in diagrams and visual maps.

---

## 8. What GLK is not

GLK is not:

```text
a paragraph language
a truth engine
a proof system
a full metadata schema
a replacement for source citations
a decorative code
```

GLK is a key.

It helps classify and retrieve.

It does not replace verification.

---

## 9. Validation criteria

A key can be considered GLK if it satisfies:

```text
1. It starts with GLK[[.
2. It closes with ]].
3. It contains TYPE before the colon.
4. It contains TAG after the colon.
5. It contains an INDEX segment.
6. It contains a DATE or cycle segment.
7. It remains compact and stable.
```

Invalid or weak examples:

```text
GLK[[DREAMORA]]
GLK[[IMG:]]
GLK[[NEXUS-ARCANA.003]]
GLK[[this is a long description]]
```

---

## 10. Public short definition

English:

```text
GLK is a compact canonical key syntax for classifying and retrieving ORA assets.

It encodes TYPE, TAG, INDEX and DATE into a stable identifier.
```

French:

```text
GLK est une syntaxe de cle canonique compacte pour classer et retrouver les actifs ORA.

Elle encode TYPE, TAG, INDEX et DATE dans un identifiant stable.
```

---

## 11. Conclusion

GLK gives ORA assets a compact identity.

It is useful for archive, retrieval, indexing, routing and version awareness.

Final formula:

```text
GLK = TYPE + TAG + INDEX + DATE
GLK = canonical archive key
GLK = compact identity for retrieval and routing
```
