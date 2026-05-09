# Backlash Politics in European Populist Party Manifestos (2018–2025)

A reproducible comparative political science project examining how European populist and right-wing parties emphasize different dimensions of backlash rhetoric in contemporary manifesto discourse using data from the Manifesto Project Database (MPD).

## Project Overview

This project explores how European populist and right-wing parties articulate backlash politics through manifesto rhetoric between 2018 and 2025. Rather than treating backlash politics as a single ideological phenomenon, the analysis compares how parties combine different rhetorical dimensions, including:

* traditional morality,
* nationalism,
* anti-multiculturalism,
* and law-and-order rhetoric.

The project uses manifesto data from the Manifesto Project Database (MPD) and reproducible workflows in R and Quarto.

## Research Question

> How do European populist parties articulate backlash politics in contemporary manifesto discourse?

## Cases Included

The analysis focuses on seven European populist and right-wing parties:

| Party                         | Country |
| ----------------------------- | ------- |
| Vox                           | Spain   |
| Alternative for Germany (AfD) | Germany |
| Rassemblement National (RN)   | France  |
| Fratelli d’Italia             | Italy   |
| Fidesz                        | Hungary |
| Law and Justice (PiS)         | Poland  |
| Austrian Freedom Party (FPÖ)  | Austria |

Timeframe:

* 2018–2025

## Data

* Source: [Manifesto Project Database (MPD)](https://manifesto-project.wzb.eu/?utm_source=chatgpt.com)
* Unit of analysis: Party manifestos
* Method: Comparative descriptive analysis

## Main Variables

The project examines four manifesto dimensions associated with backlash politics:

| Variable | Meaning                       |
| -------- | ----------------------------- |
| `per603` | Traditional morality rhetoric |
| `per601` | Nationalist rhetoric          |
| `per608` | Anti-multiculturalism         |
| `per605` | Law-and-order rhetoric        |

Variables represent the percentage of quasi-sentences within manifestos devoted to each category.

## Methods

The project uses:

* reproducible R workflows,
* manifesto analysis,
* descriptive comparative analysis,
* and data visualization.

Main R packages:

* `tidyverse`
* `ggplot2`
* `readr`
* `Quarto`

## Main Finding

The analysis suggests that backlash politics in Europe is multidimensional rather than ideologically uniform. While some parties combine strong nationalist, anti-multicultural, and moral-traditionalist rhetoric simultaneously, others rely more selectively on specific dimensions of backlash discourse.

## Repository Structure

```text id="jlwm0p"
├── data/
│   ├── raw/
│   └── processed/
│
├── outputs/
│   └── figures/
│
├── paper/
│   ├── backlash_manifestos.qmd
│   └── references.bib
│
├── scripts/
│   ├── 01_setup_and_import.R
│   ├── 02_build_corpus.R
│   └── 03_descriptive_analysis.R
│
└── README.md
```

## Reproducibility

To reproduce the project:

1. Download Manifesto Project data from the MPD website.
2. Place the raw files in:

   ```text
   data/raw/
   ```
3. Run the scripts sequentially:

   * `01_setup_and_import.R`
   * `02_build_corpus.R`
   * `03_descriptive_analysis.R`
4. Render the Quarto paper:

   ```bash
   quarto render paper/backlash_manifestos.qmd
   ```

## Author

Mauricio Sierra

## License

This repository is intended for academic and research purposes.
