# GitHub Repositories

Primary GitHub sync target:

- Repo: https://github.com/priyanshbajpai/FOOD-INTELLIGENCE-OS
- Local branch: `main`
- Role: durable strategy layer for FMCG-OS and Marcha source documents

External reference repositories:

- FoodSky: https://github.com/LanceZPF/FoodSky
- Global Gastronomic Culinary Dataset: https://github.com/IS2AI/Global-Gastronomic-Culinary-Dataset
- Open Food Facts Recipe Estimator Metrics: https://github.com/openfoodfacts/recipe-estimator-metrics

## Sync Policy

- Commit durable markdown, source registry files, and lightweight brand-token files.
- Keep local model caches, virtual environments, generated images, and raw creative outputs out of Git unless explicitly selected.
- Mirror the stable Marcha system in `outputs/00-marcha-system/`.
