# Recipe Workflow

Recipes move through a simple maturity path:

```text
EXPERIMENTAL -> TEST -> CONFIRMED
```

`REFERENCE` is used for background or traditional material that has not yet become a working house recipe.

## Add recipes one at a time

Each recipe should be added, tested, and refined independently.

This keeps version history clear and makes it easier to understand what changed.

## EXPERIMENTAL

Use `EXPERIMENTAL` for early ideas, unfinished drafts, failed tests, or rough adaptations.

Before moving to `TEST`, the recipe should have:

- A clear ingredient list
- Measurements, preferably in grams
- A workable method
- Basic temperature, timing, and pan/equipment notes where applicable
- Clear gluten-free assumptions or substitutions

## TEST

Use `TEST` when the recipe is cookable and moving in the right direction, but not yet final.

A `TEST` recipe must include:

- Oven temperature where applicable
- Pan size where applicable
- Timing
- Resting or cooling instructions where applicable
- Texture targets
- A `What changed / feedback` section

The `What changed / feedback` section should capture:

- Version changes
- Test result
- Flavor notes
- Texture notes
- Timing notes
- What to adjust next

## CONFIRMED

Move a recipe to `CONFIRMED` only when it is tried, approved, and repeatable.

A `CONFIRMED` recipe should have:

- Stable measurements
- Repeatable method
- Clear doneness and texture targets
- Known pan size / equipment notes
- Known timing and cooling/resting instructions
- Gluten-free/celiac safety notes where relevant

Do not overwrite a `CONFIRMED` recipe without incrementing `version`.

## REFERENCE

Use `REFERENCE` for traditional, background, or source recipes that are not yet working house recipes.

A `REFERENCE` recipe may become:

- `EXPERIMENTAL` when adaptation begins
- `TEST` when it has a cookable working version
- `CONFIRMED` only after successful repeatable testing

## Versioning

Use simple version numbers:

```text
1.0
1.1
1.2
2.0
```

Suggested meaning:

- Patch/minor version changes such as `1.0` to `1.1` = small measurement, timing, or note changes
- Major version changes such as `1.0` to `2.0` = meaningful formulation or process change

Any change to a `CONFIRMED` recipe should increment `version`.
