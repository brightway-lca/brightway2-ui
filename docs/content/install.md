# Installation

This project ships as two closely related packages:

- `bw25ui` for Brightway25 users.
- `bw2ui` for the classic Brightway2 stack.

Both expose the same `bw2-browser` command-line interface, but the dependency pins differ, so pick the flavour that matches your Brightway universe.

## Conda / Mamba

Use conda (or its speedier cousin, mamba) when you want the whole environment managed for you.

### Brightway25

```bash
mamba install -c tomas_navarrete bw25ui
```

### Brightway2

```bash
mamba install -c tomas_navarrete bw2ui
```

## pip

Prefer wheels or already have the dependencies sorted? Install from PyPI instead.

### Brightway25

```bash
pip install bw25ui
```

### Brightway2

```bash
pip install bw2ui
```

## Version notes

- Brightway25 builds expect `bw2calc >= 2.0.dev10` and `bw2analyzer >= 0.11`.
- Brightway2 builds stick with `bw2calc < 2` and `bw2analyzer >= 0.10`.

As long as those requirements are respected, both packages run the same code and produce identical command-line behaviour. Pick the installer you’re comfortable with, point it at the right package name, and you’re ready to go 🧭.

