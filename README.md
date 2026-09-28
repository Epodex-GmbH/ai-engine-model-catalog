# EPODEX model catalog

Public model recommendations for AI Engine.

Set `AUTO_LLM_CONFIG_URL` in the API and background service environments:

```text
https://raw.githubusercontent.com/Epodex-GmbH/ai-engine-model-catalog/main/recommended-models.json
```

The file sets visible chat models and the default model for each provider.
The default update interval is 30 minutes.
Only providers with auto mode enabled use these recommendations.

When model recommendations change, increase `version` and `updated_at`.
Use a UTC timestamp later than the previous `updated_at` value.
Review changes before merging them into `main`.

The catalog contains model names only. Keep credentials in AI Engine.
Catalog entries do not guarantee access through every provider account.
