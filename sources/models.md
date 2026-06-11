# Models

This file tracks model sources and local model roles for FMCG-OS.

## Active Local Models

### Epicure Explorer

- Status: live locally
- Local cache: `work/model-cache/epicure-cooc`, `work/model-cache/epicure-core`, `work/model-cache/epicure-chem`
- Uses: ingredient pairings, substitutions, chemistry neighbours, cuisine shifts, ingredient-space exploration
- Best for: sauce variants, snack seasoning directions, beverage flavour pairings, Indian/global adaptation, ingredient cost-down routes

### RecipeBERT

- Status: live locally
- Local environment: `work/flavorforge-venv`
- Uses: recipe-space plausibility, concept similarity, variant ranking, familiarity vs novelty checks
- Best for: ranking product concepts, comparing Indian/global fusion variants, filtering ideas that feel too generic or too strange

### T5 Recipe Generation

- Source: https://huggingface.co/flax-community/t5-recipe-generation
- Status: live locally
- Local cache: `work/model-cache/t5-recipe-generation`
- Uses: rough recipe or prototype direction from ingredient stacks
- Caution: treat outputs as test-kitchen inspiration, not final FMCG formulation.

## Local CLI

Status:

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
