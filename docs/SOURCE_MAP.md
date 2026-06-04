# Source Map

This document tracks the model and dataset sources to use inside the FMCG research chat.

## 1. Epicure Explorer

Use for ingredient-level intelligence.

Role in workflow:
- Pairing discovery
- Substitution research
- Chemistry-aware ingredient neighbours
- Cuisine direction shifts
- Ingredient maps and flavour-space exploration

Best for:
- `what goes with this?`
- `how do I Indianize/globalize this ingredient?`
- `what can replace this ingredient?`
- `what variants should a sauce/snack/beverage line have?`

Current status:
- Live in the Codex chat workspace.
- Models cached locally: `epicure-cooc`, `epicure-core`, `epicure-chem`.

## 2. RecipeBERT

Use for recipe-space plausibility and similarity.

Role in workflow:
- Score concepts for recipe familiarity
- Compare variants to cuisine/category archetypes
- Detect concepts that feel too generic or too strange
- Cluster product ideas around culinary meaning

Current status:
- Live in the Codex chat workspace through Transformers/Torch.
- Useful for scoring, ranking, and comparison; not a recipe generator by itself.

## 3. flax-community/t5-recipe-generation

Source: https://huggingface.co/flax-community/t5-recipe-generation

Use for rough prototype recipe generation from ingredient lists.

Current status:
- Live in the Codex chat workspace.
- Minimal local inference files cached under `work/model-cache/t5-recipe-generation`.

Notes:
- Hugging Face describes it as a T5/text2text-generation recipe model.
- The model card references RecipeNLG as the dataset base, with over 2 million recipes.
- Useful after Epicure suggests ingredient stacks and RecipeBERT ranks them.
- Outputs should be treated as test-kitchen inspiration, not final FMCG formulation.

Potential workflow:
1. Generate concept ingredients with Epicure.
2. Rank concept plausibility with RecipeBERT.
3. Use T5 recipe generation for rough prototype directions.
4. Rewrite into FMCG-friendly formulation language.

## 4. FoodSky / FoodEarth

Sources:
- GitHub: https://github.com/LanceZPF/FoodSky
- Zenodo: https://zenodo.org/records/14892842
- Paper: https://arxiv.org/abs/2406.10261

Use for food-domain reasoning and corpus inspiration.

Notes:
- FoodSky is described by its authors as a food-oriented LLM.
- FoodEarth is the related food corpus.
- The GitHub README says the full dataset is encrypted due to commercial conflicts and points users to a mini version with 20K instances.

Potential workflow:
- Mine the mini dataset for food-domain prompts and categories.
- Use FoodSky ideas as a reference layer for expert-style food Q&A.
- Treat availability/licensing carefully before commercial use.

## 5. Global Gastronomic Culinary Dataset

Source: https://github.com/IS2AI/Global-Gastronomic-Culinary-Dataset

Use for global food/cuisine visual and category awareness.

Potential workflow:
- Support global cuisine mapping.
- Help build content around recognizable food categories.
- Reference for visual/product content research, not primary formulation logic.

## 6. Open Food Facts Recipe Estimator Metrics

Source: https://github.com/openfoodfacts/recipe-estimator-metrics

Use for ingredient percentage estimation evaluation.

Notes:
- The README describes a metrics framework for estimating ingredient and sub-ingredient percentages.
- The main metric is ingredient weight difference against known ingredient percentages.

Potential workflow:
- Estimate approximate ingredient percentage ranges for FMCG concepts.
- Build evaluation-style checks for prototype formulations.
- Compare sauce/snack variants against target nutrition or label constraints.

## Working Rule

Use these sources as research and modelling aids, not as final commercial claims. Any production claim about health, nutrition, regulation, or consumer safety needs separate validation.
