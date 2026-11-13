![Auto Assign](https://github.com/money-trade/demo-repository/actions/workflows/auto-assign.yml/badge.svg)
![Proof HTML](https://github.com/money-trade/demo-repository/actions/workflows/proof-html.yml/badge.svg)

# Welcome to your organization's demo repository
This code repository (or "repo") is designed to demonstrate the best GitHub has to offer with the least amount of noise.

The repo includes an `index.html` file (so it can render a web page), two GitHub Actions workflows, and a CSS stylesheet dependency.

## Files

| File | What it does |
|---|---|
| `index.html` | A small HTML5 page styled with [Primer CSS](https://primer.style/css) |
| `package.json` | Declares the `@primer/css` 17.0.1 dependency (the page loads the same version from jsDelivr) |
| `.github/workflows/proof-html.yml` | **Proof HTML**: validates the HTML and checks links on every push and pull request |
| `.github/workflows/auto-assign.yml` | **Auto Assign**: assigns every new issue and pull request to `Chiraphinyo001` |

## View the page

- **On your computer:** open `index.html` in a browser (needs internet for the stylesheet)
- **On the web:** turn on GitHub Pages in *Settings → Pages → Deploy from a branch → `main` / root*,
  then open `https://money-trade.github.io/demo-repository/`

## Workflows

| Workflow | Runs when | Action (version) |
|---|---|---|
| Proof HTML | push, pull request, or manually (*Actions → Proof HTML → Run workflow*) | `anishathalye/proof-html@v2.2.5` |
| Auto Assign | an issue or pull request is opened | `pozil/auto-assign-issue@v4.1.0` |

The badges at the top show the latest result of each workflow.
To assign someone else, change `assignees:` in `auto-assign.yml`.

## Check the HTML locally (optional)

Proof HTML uses the W3C validator. To run the same check before pushing (needs Java):

```bash
pip install html5validator
html5validator --root .
```
