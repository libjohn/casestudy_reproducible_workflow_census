# README

John Little 6/20/23

<!-- README.md is generated from README.Rmd. Please edit that file -->


[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8044810.svg)](https://doi.org/10.5281/zenodo.8044810)

[![ORCID](https://img.shields.io/badge/ORCID-0000--0002--3600--0972-A6CE39?logo=ORCID&logoColor=A6CE39.png "ORCID")](https://orcid.org/0000-0002-3600-0972)<br/>

[![Creative Commons CC BY-NC](https://img.shields.io/badge/Creative%20Commons-BY--NC-EF9421?logo=creative%20commons&logoColor=EF9421.png "CC BY-NC")](https://creativecommons.org/licenses/by-nc-nd/4.0/)<br/>

The following is an example of a reproducible Quarto project using the R language.

This project generates a choropleth map of North Carolina counties from USA Census ACS population data for the year 2020. [^readme-1]

[^readme-1]: United States Census. (2020). American Community Survey: Tigerline data. Retrieved programmatically via <https://walker-data.com/tidycensus/index.html> package. Full dataset available at: <https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.2020.html>

### case_study_quarto_default_tier_protocol_applied

<!-- badges: start -->

<!-- badges: end -->

Using a basic TIER Protocol and working with Posit (née RStudio) IDE & Quarto, set up a Quarto website project ( \_qyarto.yml - `project: type: website` )

## Code, analysis, and publishing notes

-   The main analysis script `index.qmd` is in the main project directory. The other scripts, in the `scripts` subdirectory, serve only as demonstrations of the flexibility of Quarto.org when used to render a project reports

-   The data processed in this analysis are found in `data/raw`, then cleaned in `index.qmd`, and re-saved in `data/cleaned`

    -   Source data for the project is original to the US Census Bureau. The data download procedure was performed via the `data/raw/data_provenance.qmd` script. (That script was run once and set to `eval = FALSE`.) This document also contains a **codebook**.

-   The report expression of the project is a website. The website is published to, and hosted by, the quarto.pub website at <https://libjohn.quarto.pub/reproducible-workflow-casestudy>.

    -   the `_quarto.yaml` manages the report expression. Since the project is written with reproducible code. The expression can be rendered into alternative formats by changing the project type

-   To rebuild the quarto website. Open the code in the RStudio IDE \> Build \> Render Project

    -   Reproducible code was composed in the R programming language and is distributed via GitHub at <https://github.com/libjohn/casestudy_reproducible_workflow_census>

    -   README is rendered from `README.qmd` separately

-   Code dependencies (i.e. R versions and library packages) are managed with the [{renv} package](https://rstudio.github.io/renv)
