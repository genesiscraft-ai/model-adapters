# Contributing

We welcome contributions from the community.

## Adding a New Provider Adapter

1. Fork the repository.
2. Create a new file under `src/adapters/` (or `model_adapters/adapters/` for Python) following the existing adapter pattern.
3. Implement the required methods: `complete`, `chat`, and `stream`.
4. Add tests for the new adapter.
5. Update the README provider list.
6. Submit a pull request.

## Development

### Node.js

```bash
git clone https://github.com/genesiscraft-ai/model-adapters.git
cd model-adapters
npm install
npm run dev


Python

git clone https://github.com/genesiscraft-ai/model-adapters.git
cd model-adapters
pip install -e .
pytest


Code of Conduct

This project follows the Contributor Covenant.
