# iris-demo

A small teaching demo: one-way ANOVA on the `iris` dataset, Tukey HSD post-hoc
test, and a compact letter display (CLD) on a boxplot. Provided in **two
formats** so you can compare:

| File                  | Format       | Render with                |
|-----------------------|--------------|----------------------------|
| `iris_anova.Rmd`   | R Markdown   | Knit button in Positron, or `rmarkdown::render("iris_anova.Rmd")` |
| `iris_anova.qmd`   | Quarto       | Render button in Positron, or `quarto render iris_anova.qmd`      |

Both produce the same analysis and the same plot — only the YAML and chunk
options differ.

## Required R packages

```r
install.packages(c("multcompView", "ggplot2", "rmarkdown"))
# Quarto CLI is bundled with Positron; no R package needed.
```

## Workflow this repo is built for

1. Open the folder in **Positron**.
2. Open `iris_anova.qmd` (or `.Rmd`) and click **Render** (or **Knit**).
3. Confirm the HTML preview looks right.
4. Commit any changes and `git push` to GitHub.
5. On [connect.posit.cloud](https://connect.posit.cloud), connect this repo
   and publish either notebook. The platform re-renders on every push.

## Repo layout

```
iris-demo/
├── README.md
├── .gitignore
├── iris_anova.Rmd   # R Markdown version
└── iris_anova.qmd   # Quarto version
```

Rendered HTML is gitignored — Posit Connect Cloud renders from source.
