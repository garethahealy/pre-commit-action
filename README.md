garethahealy/pre-commit-action
=================

A fork of [pre-commit/action](https://github.com/pre-commit/action)

### Using this action

To use this action, make a file `.github/workflows/pre-commit.yml`.
Here's a template to get started:

```yaml
name: pre-commit

on:
  pull_request:
  push:
    branches: [main]

jobs:
  pre-commit:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@de0fac2e4500dabe0009e67214ff5f5447ce83dd # v6.0.2

      - uses: actions/setup-python@a309ff8b426b58ec0e2a45f0f869d46889d02405 # v6.2.0
        with:
          python-version: 3.x
          
      - uses: garethahealy/pre-commit-action@c93005939a88ad60af0f8334b1e42ab91c30ad75 # v4.6.0
```
