---
title: Anthropic
slug: ../anthropic
---

## Chat model

We recommend configuring **Claude 3.5 Sonnet** as your chat model.

```json title="config.json"
{
  "models": [
    {
      "title": "Claude 3.5 Sonnet",
      "provider": "anthropic",
      "model": "claude-3-5-sonnet-20240620",
      "apiKey": "[API_KEY]"
    }
  ]
}
```

## Autocomplete model

Anthropic currently does not offer any autocomplete models.

[Click here](../../model-types/autocomplete.md) to see a list of autocomplete model providers.

## Embeddings model

Anthropic currently does not offer any embeddings models.

[Click here](../../model-types/embeddings.md) to see a list of embeddings model providers.

## Reranking model

Anthropic currently does not offer any reranking models.

[Click here](../../model-types/reranking.md) to see a list of reranking model providers.

## Prompt caching

Anthropic supports [prompt caching with Claude](https://docs.anthropic.com/en/docs/build-with-claude/prompt-caching).

Currently, we only allow caching of the system message. To enable this feature, update your your model configuration with `"cacheSystemMessage": true`:

```json
{
  "models": [
    {
      // Enable prompt caching
      "cacheSystemMessage": true,
      "title": "Anthropic",
      "provider": "anthropic",
      "model": "claude-3-5-sonnet-20240620",
      "apiKey": "[API_KEY]"
    }
  ]
}
```