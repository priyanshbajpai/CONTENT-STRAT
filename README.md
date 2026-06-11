# CONTENT STRAT

A working research workspace for FMCG brand strategy, food product R&D, ingredient exploration, content ideas, and market-facing concept development.

This repo is the durable strategy layer. The Codex chat workspace is the live model execution layer.

## What This Workspace Is For

- FMCG product concept generation
- Food brand positioning and content strategy
- Ingredient pairing and substitution research
- Indian market adaptation for global food ideas
- Sauce, snack, beverage, condiment, ready-to-cook, and packaged food ideation
- Prototype formulation briefs and tasting hypotheses
- Competitive/white-space research notes
- Retail, QSR, and content strategy development

## Active Local Model Stack In Chat

- Epicure Explorer: ingredient pairings, substitutions, chemistry neighbours, cuisine shifts
- RecipeBERT: recipe-space plausibility and similarity scoring
- T5 Recipe Generation: rough recipe/prototype generation from ingredient stacks

## Registered Research Sources

- FoodSky/FoodEarth: food-domain LLM and food corpus reference
- Global Gastronomic Culinary Dataset: global cuisine/category reference
- Open Food Facts recipe-estimator-metrics: ingredient percentage estimation evaluation framework

## Marcha Brand System

Marcha is the content and brand layer for this workspace: an AI-first food content page that can evolve into a healthy Indian sauces and FMCG product brand.

Before creating any Marcha concept, carousel, reel, single image, product idea, recipe, sauce, or FMCG research output, start with:

- [Marcha Source Bank](MARCHA_SOURCE_BANK.md)
- [FMCG-OS Thread Starter](FMCG_OS_THREAD_STARTER.md)
- [Marcha System Docs](docs/marcha-system/README.md)
- [Marcha System Output Mirror](outputs/00-marcha-system/README.md)
- [Source Library](sources/source-registry.json)

## Source Library

The `sources/` folder separates durable source references by type:

- `models.md` - local and candidate model stack
- `datasets.md` - dataset and corpus references
- `github-repos.md` - primary and external GitHub repositories
- `research-links.md` - research URLs and Marcha research gate
- `visual-references.md` - Marcha image style references
- `fonts-and-brand.md` - typography, colours, and brand rules
- `source-registry.json` - machine-readable source registry

## Core Docs

- [FMCG Research OS](docs/FMCG_RESEARCH_OS.md)
- [Model Stack](docs/MODEL_STACK.md)
- [Workspace Guide](docs/WORKSPACE_GUIDE.md)
- [Source Map](docs/SOURCE_MAP.md)
- [Research Prompts](docs/RESEARCH_PROMPTS.md)
- [Marcha System](docs/marcha-system/README.md)

## Current Workflow

1. Ask the chat for a brand/product/category research task.
2. The chat runs model-assisted exploration where useful.
3. Promising outputs become briefs, reports, or strategy notes.
4. Durable learnings and reusable workflows are synced back here.

## Example Requests

- Research tomato sauce variants for the Indian market.
- Generate 20 premium snack concepts using millet and Indian fusion.
- Compare global fusion condiment ideas for QSR use.
- Create a launch content strategy for a new FMCG sauce brand.
- Build a tasting panel brief for 5 product variants.
- Use T5 to turn an ingredient stack into rough prototype directions.
- Find substitutes for expensive ingredients while preserving flavour direction.
