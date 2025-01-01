# RONIN GitHub Actions

A collection of reusable GitHub Actions for public repositories in the [RONIN GitHub org](https://github.com/ronin-co).

The contents of this repository are meant to be used exclusively by the RONIN team. The repository is only public because GitHub requires it to be. If it were private, other public repositories could not make use of it.

## Example

```yaml
name: Validate

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs:
  validate:
    uses: ronin-co/actions/.github/workflows/validate.yml@main
    with:
      package_dir: './'  # Adjust if your package is in a subdirectory
```
