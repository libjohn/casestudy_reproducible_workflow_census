README
================
John Little
2/2/23

<!-- README.md is generated from README.Rmd. Please edit that file -->

The following is an example of a reproducible Quarto project using the R
language to download.

This project generates a choropleth map of North Carolina counties from
USA Census ACS population data for the year 2020.

### case_study_quarto_default_tier_protocol_applied

<!-- badges: start -->
<!-- badges: end -->

Using a basic TIER Protocol and working with Posit (née RStudio) IDE &
Quarto, set up a Quarto website project ( \_qyarto.yml -
`project: type: website` )

## Code, analysis, and publishing notes

- The main analysis script `index.qmd` is in the main project directory.
  Other scripts are in the `scripts` subdirectory and serve only as
  example scripts/documents demonstrating the flexibility of Quarto.org
  when used to render a project report

- The data processed in this project are found in `data/raw`; then
  cleaned in `index.qmd` and re-saved in `data/cleaned`

  - Source data for the project is original to the US Census Bureau. The
    data download procedure was performed via the
    `data/raw/data_provenance.qmd` script. (That script was run once and
    set to `eval = FALSE`.) This document also contains a **codebook**.

- The report expression of the project is a website. The website is
  published to, and hosted by, the quarto.pub website at
  <https://libjohn.quarto.pub/reproducible-workflow-casestudy>.

  - the `_quarto.yaml` manages the report expression. Since the project
    is written with reproducible code. The expression can be rendered
    into alternative formats by changing the project type to an
    alternate format, such as a book. (See Quarto.org)

- To rebuild the quarto website. Open the code in the RStudio IDE \>
  Build \> Render Project

  - Reproducible code was composed in the R programming language and is
    distributed via GitHub at
    <https://github.com/libjohn/casestudy_reproducible_workflow_census>

  - README is rendered from `README.qmd` separately

- Code dependencies (i.e. R versions and library packages) are managed
  with the [{renv} package](https://rstudio.github.io/renv)
