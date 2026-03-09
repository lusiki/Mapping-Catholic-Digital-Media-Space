# Attention Markets in Religious Digital Media: Mapping the Croatian Catholic Digital Space

A computational analysis of **600,000+ posts** from Croatian Catholic digital media across 8 platforms (2021--2026), examining attention concentration, engagement quality, sentiment dynamics, liturgical temporality, and platform effects.

---

## Working Paper

**Kovačić, S., Palić, P. & Sikić, L. (2026). Tržišta pažnje u religijskim digitalnim medijima: Mapiranje hrvatskog katoličkog digitalnog prostora.**

| Format | Link |
|:------:|:----:|
| PDF (v5) | [**Read online**](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/drafts/attention_markets_paper_hr_v5.pdf) |
| HTML (v7) | [**Read online**](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/drafts/attention_markets_paper_hr_v7.html) |
| Source | [`attention_markets_paper_hr_v7.qmd`](paper/hr/drafts/attention_markets_paper_hr_v7.qmd) |

---

## Abstract

The paper applies the attention economics framework to a non-commercial religious digital ecosystem. Using the DigiKat database (600,000+ posts, 2021--2026, 8 platforms), five interconnected hypotheses are tested:

1. **H1 -- Concentration**: Attention follows power-law distributions (Gini > 0.80, R² > 0.90)
2. **H2 -- Engagement quality**: Institutional actors attract qualitatively different engagement (more deliberative, less affective)
3. **H3 -- Sentiment mechanism**: Negative content drives disproportionate engagement, but less so for institutionally constrained actors
4. **H4 -- Liturgical temporality**: The liturgical calendar explains significant variance in posting activity beyond secular temporal patterns
5. **H5 -- Platform architecture**: Algorithmically curated platforms show higher attention concentration than editorially curated ones

### Key findings

- Extreme attention inequality across all platforms (Gini = 0.96)
- Institutional actors receive proportionally more comments and shares relative to likes
- Negative sentiment amplifies engagement 2--3x, with institutional actors showing a smaller negativity boost
- The liturgical calendar significantly structures digital activity (F-test p < 0.001)
- Algorithmically curated platforms exhibit stronger winner-takes-all dynamics

---

## Repository Structure

```
paper/hr/drafts/
  attention_markets_paper_hr_v7.qmd   # Current working paper (source)
  attention_markets_paper_hr_v7.html   # Rendered HTML

paper/hr/drafts/                       # Previous versions (v2, v3, v4, v5, v6)
paper/hr/final/                        # Earlier complete draft (v1)
paper/en/                              # English language versions

maps/                                  # Supplementary interactive analyses
archive/                               # Archived materials
output/                                # Additional outputs
```

---

## Rendering

The paper is a Quarto document with embedded R code. To render all formats:

```bash
quarto render paper/hr/drafts/attention_markets_paper_hr_v7.qmd --to html
```

**Requirements:** R (v4.x+), Quarto, XeLaTeX (for PDF), and the following R packages:

```r
install.packages(c("tidyverse", "data.table", "scales", "ggplot2",
                    "knitr", "kableExtra", "ineq", "lubridate"))
```

---

## Supplementary Materials

### Interactive Analyses (Maps)

Detailed exploratory analyses that informed the working paper:

| Map | Title | View |
|:---:|-------|:----:|
| 1 | Platform and Actor Structure | [Open](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/maps/map_1_platform_actors.html) |
| 2 | Thematic Structure (STM, 35 topics) | [Open](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/maps/map_2_thematic.html) |
| 3 | Emotional Structure | [Open](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/maps/map_3_emotional.html) |
| 4 | Temporal Dynamics | [Open](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/maps/map_4_temporal.html) |

### Previous Paper Versions

| Version | Language | Link |
|:-------:|:--------:|:----:|
| v6 | HR | [HTML](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/drafts/attention_markets_paper_hr_v6.html) |
| v5 | HR | [PDF](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/drafts/attention_markets_paper_hr_v5.pdf) |
| v4 | HR | [HTML](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/drafts/attention_markets_paper_hr_v4.html) |
| v3 | HR | [HTML](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/drafts/attention_markets_paper_hr_v3.html) |
| v2 | HR | [HTML](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/drafts/attention_markets_paper_hr_v2.html) |
| v1 | HR | [HTML](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/final/attention_markets_paper_hr.html) |
| Complete | EN | [HTML](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/en/final/attention_markets_paper_complete.html) |
| Short | EN | [HTML](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/en/drafts/attention_markets_paper_en_short.html) |

### Data

The analysis uses the **DigiKat database** -- a media monitoring corpus of Croatian Catholic digital content collected via the Mediatoolkit platform. The raw data file (`merged_comprehensive.rds`) is not included in this repository due to size and platform terms of service. Available upon request subject to ethical and legal constraints.

---

## Citation

```
Kovacic, S., Palic, P. & Sikic, L. (2026). Trzista paznje u religijskim
  digitalnim medijima: Mapiranje hrvatskog katolickog digitalnog prostora.
  Working paper. https://github.com/lusiki/Mapping-Catholic-Digital-Media-Space
```

---

## Authors

**Siniša Kovačić** | HINA
**Petra Palić** | UNICATH
**Luka Sikić** | UNICATH
