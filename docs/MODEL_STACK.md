# Model Stack

This is the active model stack used by the Codex FMCG research workspace.

## Local Models

### Epicure Explorer

Status: live locally

Local cache:
- `work/model-cache/epicure-cooc`
- `work/model-cache/epicure-core`
- `work/model-cache/epicure-chem`

Use for:
- Ingredient pairings
- Chemistry neighbours
- Cuisine shifts
- Substitution research
- Ingredient-space exploration

Best FMCG use cases:
- Sauce variant development
- Snack seasoning exploration
- Beverage flavour pairing
- Indian/global fusion adaptation
- Ingredient cost-down substitution routes

### RecipeBERT

Status: live locally

Local environment:
- `work/flavorforge-venv`
- Hugging Face cache under `work/hf-cache`

Use for:
- Recipe-space plausibility
- Concept similarity
- Variant ranking
- Familiarity vs novelty checks

Best FMCG use cases:
- Rank product concepts
- Compare Indian vs global fusion variants
- Detect concepts that may be too strange or too generic

### T5 Recipe Generation

Status: live locally

Local cache:
- `work/model-cache/t5-recipe-generation`

Use for:
- Rough recipe/prototype direction from ingredient stacks
- First-pass preparation logic
- Translating ingredient stacks into test-kitchen language

Important note:
T5 outputs are rough culinary drafts. Treat them as inspiration for R&D, not final formulations.

## Candidate Sources Not Fully Local

### FoodSky / FoodEarth

Source:
- https://github.com/LanceZPF/FoodSky
- https://zenodo.org/records/14892842

Use when:
- We need food-domain benchmark ideas
- We need Chinese/Asian culinary corpus inspiration
- We want to inspect FoodEarth mini data

Caution:
Review access and licensing before commercial use.

### Global Gastronomic Culinary Dataset

Source:
- https://github.com/IS2AI/Global-Gastronomic-Culinary-Dataset

Use when:
- We need global cuisine/category references
- We need visual/category inspiration for food content

### Open Food Facts Recipe Estimator Metrics

Source:
- https://github.com/openfoodfacts/recipe-estimator-metrics

Use when:
- We need ingredient percentage estimation logic
- We want formulation evaluation metrics
- We need a method for comparing estimated ingredient proportions

## Local CLI

The chat can run:

```bash
PYTHONPATH=work HF_HOME=work/hf-cache work/flavorforge-venv/bin/python -m fmcg_engine.research_cli status --pretty
```

Concept generation:

```bash
PYTHONPATH=work HF_HOME=work/hf-cache work/flavorforge-venv/bin/python -m fmcg_engine.research_cli concepts --category Sauce --hero tomato --cuisine Indian-inspired
```

Ingredient exploration:

```bash
PYTHONPATH=work HF_HOME=work/hf-cache work/flavorforge-venv/bin/python -m fmcg_engine.research_cli ingredients --hero tomato --cuisine Indian-inspired
```

Prototype generation:

```bash
PYTHONPATH=work HF_HOME=work/hf-cache work/flavorforge-venv/bin/python -m fmcg_engine.research_cli prototype --ingredients "tomato, cumin, garlic, chili powder"
```
