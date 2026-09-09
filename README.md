# Model Adapters

Open‑source adapters that standardize LLM access across multiple providers.

## Purpose

Building on top of different large language model providers often means writing provider‑specific code. Model Adapters solves this by providing a unified interface for common LLM operations, making it easy to switch between OpenAI, Anthropic, Gemini, and open‑source models without changing your application logic.

## Features

- Provider‑agnostic interface for completion and chat
- Built‑in support for OpenAI, Anthropic, Google, and Hugging Face
- Prompt templating and caching
- Error normalization and retries
- TypeScript and Python clients

## Supported Providers

- OpenAI (`openai`)
- Anthropic (`anthropic`)
- Google Gemini (`gemini`)
- Hugging Face Inference (`huggingface`)

## Install

### Node.js

```bash
npm install @genesiscraft/model-adapters


Python

pip install genesis-craft-model-adapters


Quick Start

JavaScript / TypeScript

import { ModelAdapter } from '@genesiscraft/model-adapters';

const adapter = new ModelAdapter({
  provider: 'openai',
  model: 'gpt-4',
  apiKey: process.env.OPENAI_API_KEY,
});

const result = await adapter.complete({
  prompt: 'Generate a REST endpoint for user authentication',
});

console.log(result.text);


Python

from model_adapters import ModelAdapter

adapter = ModelAdapter(
    provider="anthropic",
    model="claude-3-sonnet-20240229",
    api_key="YOUR_API_KEY",
)

result = adapter.complete(
    prompt="Generate a REST endpoint for user authentication"
)

print(result.text)


Documentation

Detailed API reference and configuration options are available in the docs directory.


Contributing

Contributions are welcome. See CONTRIBUTING.md.


License

Apache-2.0
