# owenlin926.github.io

This repository contains a website about myself, along with 2 pages featuring basic analysis performed with R and Python.

## Install First

- Quarto 1.10.18
- uv 0.12.5
- R 4.6.1

## Building the Site

1) Clone the repository (shell)

```bash
git clone https://github.com/owenlin926/owenlin926.github.io.git
```

2) Move into repository (shell)

```bash
cd owenlin926.github.io
```

3) Set up the Python environment (shell):

```bash
uv sync
```

4) Start setting up the R environment (shell):

```bash
uv run R
```

5) Finish setting up the R environment (R from the shell)

```r
renv::restore()
```
If prompted to proceed, type "Y"

```r
q("no")
```


6) Render site (shell):

```bash
uv run quarto render
```

## Site Landing

The rendered website can be found in the docs/ folder.

To render the site locally, navigate to the top level of the repository in shell and enter:

```bash
uv run quarto preview
```

## Data Sources
mtcars comes with R's built-in datasets package

palmerpenguins comes with the "palmerpenguins" package, loaded by: 

`from palmerpenguins import load_penguins`

No network access is needed to render the website but it is necessary to download python, the python packages, and the R packages.