# chads.name

Hugo site for ChadCon. Uses the [Altru](https://github.com/ctindel/altru) theme,
pulled from upstream — the `themes/` directory is gitignored and never
committed.

## Prerequisites

- Hugo extended ≥ 0.60 (`brew install hugo`)
- Git

## Install the theme

The theme lives in `themes/altru` and must be cloned from upstream before
running Hugo. It is intentionally not vendored in this repo.

```bash
git clone https://github.com/ctindel/altru.git themes/altru
```

To update the theme later:

```bash
git -C themes/altru pull
```

## Run the dev server

```bash
hugo server -D --buildFuture
```

- `-D` builds draft content
- `--buildFuture` builds posts dated in the future

Site serves at http://localhost:1313/.

## Build for production

```bash
hugo --minify
```

Output goes to `public/` (also gitignored).
