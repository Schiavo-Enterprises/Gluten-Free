# Gluten-Free Recipe Repository

This repository stores gluten-free recipes only.

The goal is to keep the collection simple, status-driven, and easy to evolve one recipe at a time. Recipes are organized into broad categories, while each recipe's maturity is tracked inside the recipe file using YAML front matter.

## Folder structure

```text
GF/
  README.md

  recipes/
    desserts/
    savory/
    breakfast/

  templates/
    recipe_template.md

  docs/
    taxonomy.md
    workflow.md
```

## Recipe categories

Use only the initial broad folders for now:

- `recipes/desserts/`
- `recipes/savory/`
- `recipes/breakfast/`

Do not reorganize into many food categories yet.

## Recipe status

Every recipe must have exactly one status in YAML front matter:

- `CONFIRMED` = tried, approved, repeatable
- `TEST` = working recipe, good direction, still needs refinement
- `EXPERIMENTAL` = early idea or failed/unfinished test
- `REFERENCE` = traditional/background recipe, not yet converted into a working house recipe

Status belongs inside the recipe file. Do not create separate locked, confirmed, test, or archive folders.

## Recipe index

### Desserts

- `CONFIRMED` — [Basque Cheesecake — La Viña Style (Reduced Sugar)](recipes/desserts/basque-cheesecake-la-vina-style-reduced-sugar.md)
- `CONFIRMED` — [Gluten-Free Almond Cookies (杏仁饼)](recipes/desserts/gluten-free-almond-cookies-xing-ren-bing.md)
- `TEST` — [Gluten-Free Easter Koulourakia](recipes/desserts/gluten-free-easter-koulourakia.md)

### Breakfast

- `CONFIRMED` — [Gluten-Free German Pancake / Dutch Baby](recipes/breakfast/gluten-free-german-pancake-dutch-baby.md)

### Savory

- `TEST` — [Hummus](recipes/savory/hummus.md)
- `EXPERIMENTAL` — [Gluten-Free Pita with Sourdough Discard](recipes/savory/gluten-free-pita-with-sourdough-discard.md)
- `REFERENCE` — [Greek Lentil Soup (Fakes)](recipes/savory/greek-lentil-soup-fakes.md)

## Recipe file requirements

- Use lowercase kebab-case filenames.
- Add recipes one at a time.
- Use grams wherever possible.
- Include oven temperature, pan size, timing, resting/cooling, and texture targets when applicable.
- Include `What changed / feedback` when the recipe status is `TEST`.
- Do not overwrite `CONFIRMED` recipes without incrementing the recipe `version`.

## Template

Use `templates/recipe_template.md` for every new recipe.

## Workflow

See:

- `docs/taxonomy.md`
- `docs/workflow.md`
