# Ahsan Iqbal — Personal Technical Website

A Quarto-based personal website for CV/research/projects and notebook-style technical notes.

## Local setup

Install Quarto:
https://quarto.org/docs/get-started/

Optional but recommended for executable Python notes:

```bash
python -m venv .venv
source .venv/bin/activate
pip install jupyter torch
```

Preview locally:

```bash
quarto preview
```

Render once:

```bash
quarto render
```

## GitHub Pages hosting

1. Create a GitHub repository named exactly:

   `Ahsaniqbal.github.io`

2. Push this project to that repository.

3. In GitHub, go to:

   `Settings -> Pages`

4. Under **Build and deployment**, choose **GitHub Actions**.

5. Push to `main`. The included workflow will build and deploy the Quarto site.

Your site should then be available at:

`https://ahsaniqbal.github.io`

## Writing notes

Use either `.qmd` files or real `.ipynb` notebooks.

Quarto renders TeX math using MathJax by default in this project:

Inline:

```text
$E = mc^2$
```

Display:

```text
$$
q = \operatorname{round}(x/s)
$$
```
