# RH Stadium Spectrum Analysis

This repository presents analysis and visualization of longitudinal RF spectrum measurements collected around the Notre Dame stadium environment.

The goal is to document observed spectral activity across multiple frequency bands, compare measurements from distributed receiver nodes, and relate observed emissions to possible event-time wireless systems when appropriate.

## Website

This repository is designed as a Quarto website published with GitHub Pages.

Once deployed, the site will be available at:

```text
https://hnbicer.github.io/RH-Stadium-Spectrum-Analysis/
```

## Contents

```text
RH-Stadium-Spectrum-Analysis/
├── _quarto.yml              # Quarto website configuration
├── index.qmd                # Main overview page
├── 1920_1930_mhz.qmd         # 1920–1930 MHz analysis
├── 5p8ghz_links.qmd          # 5.8 GHz link analysis
├── longitudinal_psd.qmd      # Temporal PSD evolution
├── figures/                 # Curated figures used by the website
├── scripts/                 # Analysis and plotting scripts
├── docs/                    # Rendered website output for GitHub Pages
└── README.md
```

## Analysis Topics

Current and planned analysis pages include:

- **1920–1930 MHz:** Activity related to possible DECT-like or Riedel Bolero intercom systems.
- **5.8 GHz links:** OFDM-like emissions observed near event time.
- **Temporal PSD evolution:** Time-varying PSD plots across distributed receiver nodes.
- **Node comparisons:** Comparison of spectral activity across spatially distributed sensors.

## Building the Website Locally

Install [Quarto](https://quarto.org/), then run:

```bash
quarto render
```

This renders the website into the `docs/` folder.

To preview locally:

```bash
quarto preview
```

## GitHub Pages Deployment

This site is intended to be deployed using GitHub Pages with the following settings:

```text
Source: Deploy from a branch
Branch: main
Folder: /docs
```

The `docs/.nojekyll` file should be included so that GitHub Pages serves the rendered Quarto HTML directly instead of processing it with Jekyll.

Only curated figures, scripts, and documentation needed for presenting the analysis should be committed.

## Repository Purpose

This repository is intended to serve as a lightweight, public-facing analysis report rather than a complete raw-data archive.
