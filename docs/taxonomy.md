# Recipe Taxonomy

This repository uses a simple status-driven taxonomy.

Every recipe must have exactly one status in YAML front matter:

```yaml
---
title:
status:
version:
category:
last_tested:
notes:
---
```

## Status values

### CONFIRMED

A `CONFIRMED` recipe has been tried, approved, and is repeatable.

Use this status when:

- The recipe has been made successfully.
- Measurements, timing, temperature, texture, and process are stable.
- The recipe is good enough to repeat without major changes.

Rules:

- Do not overwrite a `CONFIRMED` recipe without incrementing `version`.
- Preserve the confirmed baseline before making major changes.
- If experimenting with a confirmed recipe, create a new `TEST` version or clearly increment the version.

### TEST

A `TEST` recipe is a working recipe with a good direction, but it still needs refinement.

Use this status when:

- The recipe works but needs better texture, flavor, timing, structure, or yield.
- Measurements are mostly defined.
- The recipe has been tested at least once or is ready for a controlled test.

Required section:

```md
## What changed / feedback
```

Use that section to track:

- What changed from the prior version
- What worked
- What failed
- What to adjust next time

### EXPERIMENTAL

An `EXPERIMENTAL` recipe is an early idea, unfinished draft, failed test, or rough formulation.

Use this status when:

- The recipe has not been fully tested.
- Key measurements are missing.
- The process is incomplete.
- It is a concept worth preserving but not yet reliable.

Rules:

- Clearly mark uncertainty.
- Do not present the recipe as repeatable.
- Move to `TEST` only when the recipe has enough structure to cook from.

### REFERENCE

A `REFERENCE` recipe is traditional, background, source, or inspiration material that has not yet been converted into a working house recipe.

Use this status when:

- Capturing a traditional recipe for context.
- Saving an external recipe as inspiration.
- Recording a non-gluten-free recipe that still needs conversion.
- Preserving background ratios, methods, or historical notes.

Rules:

- Clearly state that it is not yet a confirmed house recipe.
- Add conversion notes if gluten-free adaptation is needed.
- Move to `EXPERIMENTAL` or `TEST` when actively adapting it.

## Category values

Initial categories should stay broad:

- `desserts`
- `savory`
- `breakfast`

Do not create narrow folders or status folders unless the repository structure is intentionally revised later.
