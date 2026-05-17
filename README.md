# Gluten-Free Recipe Collection

A personal recipe repository for gluten-free and celiac-conscious cooking, with low-carb notes where useful.

## Structure

```text
recipes/
  breakfast/
  dinner/
  snacks/
  desserts/
templates/
  recipe-template.md
```

## Recipe standards

Each recipe should include:

- Ingredients
- Step-by-step instructions
- Tags
- Celiac / gluten-free safety notes
- Low-carb notes when relevant
- Source notes if the recipe came from ChatGPT, family notes, a cookbook, or another source

## Adding recipes with ChatGPT and Codex

1. Create or refine the recipe in ChatGPT.
2. Ask ChatGPT to output it as Markdown using the template in `templates/recipe-template.md`.
3. Paste the Markdown into Codex and ask it to create the file in the correct folder.
4. Review the diff before committing or pushing.

Recommended Codex prompt:

```text
Add the recipe below to this repository.

Rules:
- Use one Markdown file per recipe.
- Put it in the correct folder under recipes/.
- Use a kebab-case filename.
- Follow templates/recipe-template.md.
- Do not invent missing ingredients, measurements, or steps.
- Preserve uncertainty with notes where needed.
- Include celiac-safety and low-carb notes.

Recipe:
[paste recipe here]
```
