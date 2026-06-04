# Workspace Guide

This repo is the durable strategy layer. The local Codex workspace is the model execution layer.

## What Belongs In GitHub

Keep these in this repo:

- Research playbooks
- Prompt libraries
- Source maps
- Brand strategy docs
- Product concept briefs
- Content calendars
- Retail/QSR pitch docs
- Validation templates
- Reusable frameworks

Do not commit:

- Model weights
- Python virtual environments
- Hugging Face caches
- One-off raw outputs unless they are polished deliverables
- API keys or secrets

## What Belongs Locally

Keep these in local `work/`:

- Model caches
- Virtual environments
- Temporary generated JSON
- Scratch research scripts
- Dataset downloads under review

Current local layout:

```text
work/
  flavorforge-venv/          Python ML environment
  hf-cache/                  Hugging Face cache for RecipeBERT
  model-cache/               Curated local model files
    epicure-cooc/
    epicure-core/
    epicure-chem/
    t5-recipe-generation/
  fmcg_engine/               Chat-side model engine and CLI
  fmcg_source_registry.json  Local source/model registry
```

## How To Use This Setup

For live research, ask the Codex chat directly.

Examples:

- `Use the local models to create sauce variants for tomato in the Indian market.`
- `Explore ingredient pairings for mango for a premium beverage brand.`
- `Create a 5-SKU architecture for a millet snack brand.`
- `Use T5 to create rough prototype directions for these ingredient stacks.`
- `Turn the top concept into a retailer pitch.`

## Sync Rule

When a finding becomes reusable, sync it to GitHub as one of:

- `docs/category/...`
- `docs/brands/...`
- `docs/concepts/...`
- `docs/content/...`
- `docs/templates/...`

Keep raw model exploration in chat/local files unless it becomes a polished brief.

## Optimization Rule

Local space should be used for tools that improve repeated research. GitHub should be used for memory, strategy, and collaboration.

Current local heavy assets are intentional:

- RecipeBERT cache: useful for scoring concepts
- T5 recipe-generation cache: useful for rough prototype generation
- Python venv: required for Torch/Transformers

Everything else should stay lightweight.
