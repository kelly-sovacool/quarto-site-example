# quarto-site-example

And example quarto website for a curriculum.

See the quarto docs for details on authoring sites with quarto: 
<https://quarto.org/docs/guide/>

## Instructions

One-time download & install:

```
git clone https://github.com/kelly-sovacool/quarto-site-example
cd quarto-site-example
mamba env create -f environment.yml -n swc
```

To render the site locally

```
conda activate swc
quarto render
```

View output in `_site/`. This directory is intentionally ignored in git.

To update the real site on github pages, commit and push your changes:

```
git add .
git commit -m "descriptive message"
git push
```

The [github actions workflow](.github/workflows/quarto-publish.yml) will activate
the conda environment, render the quarto documents, and push the rendered html
documents to the `gh-pages` branch to deploy the site.

View the example site at <https://sovacool.dev/quarto-site-example/>