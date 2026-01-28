# Mapping the Croatian Catholic Digital Media Space

A comprehensive computational analysis of **600,000+ posts** from Croatian Catholic digital media across multiple platforms (2021-2026). This project maps the structure, themes, emotions, and temporal dynamics of religious communication in the Croatian digital public sphere.

## Working Paper

📄 **[Attention Markets in Religious Digital Media: Mapping the Croatian Catholic Digital Space](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/en/final/attention_markets_paper_complete.html)**

📄 **[Attention Markets in Religious Digital Media: Mapping the Croatian Catholic Digital Space (short version)](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/en/drafts/attention_markets_paper_en_short.html)**

🇭🇷 **[Tržišta pažnje u religijskim digitalnim medijima: Mapiranje hrvatskog katoličkog digitalnog prostora](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/final/attention_markets_paper_hr.html)**

🇭🇷 **[Tržišta pažnje u religijskim digitalnim medijima (kratka verzija)](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/paper/hr/drafts/attention_markets_paper_hr_v2.html)**

---

## Interactive Maps

Explore the full interactive analyses:

| Map | Title | View |
|:---:|-------|:----:|
| 1 | **Platform and Actor Structure** | [**Open Map 1**](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/maps/map_1_platform_actors.html) |
| 2 | **Thematic Structure** | [**Open Map 2**](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/maps/map_2_thematic.html) |
| 3 | **Emotional Structure** | [**Open Map 3**](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/maps/map_3_emotional.html) |
| 4 | **Temporal Dynamics** | [**Open Map 4**](https://raw.githack.com/lusiki/Mapping-Catholic-Digital-Media-Space/main/maps/map_4_temporal.html) |

---

## Project Overview

The analysis applies computational social science methods to understand how the Catholic Church and Catholic voices communicate in Croatia's digital landscape. Each "map" addresses a distinct research question:

### Map 1: Platform and Actor Structure
> **Who communicates where, and who dominates visibility?**

Analyzes the distribution of content across platforms and the stratification of visibility among different actor types. Examines engagement metrics, Lorenz curves, and power-law distributions to understand concentration of attention in Catholic digital spaces.

**Key analyses:**
- Platform distribution (Web, Facebook, Instagram, YouTube, Twitter, Forums)
- Actor type classification and engagement patterns
- Cross-platform presence strategies
- Gini coefficients and visibility inequality

### Map 2: Thematic Structure
> **What is Croatian Catholic digital media about, and who specializes in what?**

Uses **Structural Topic Modeling (STM)** to discover the 35 latent themes in the corpus. Maps how different actors and platforms specialize in particular topics.

**Key analyses:**
- Topic modeling with 35 discovered themes
- Actor-topic specialization profiles
- Platform-topic distributions
- Thematic categories: Liturgical/Sacramental, Devotional, Institutional, Social/Ethical, Political, Youth/Community, Educational

### Map 3: Emotional Structure
> **What emotional register characterizes Croatian Catholic digital communication, and where does controversy emerge?**

Combines automated sentiment analysis with Facebook reaction data (LOVE, WOW, HAHA, SAD, ANGRY) to map the emotional landscape of religious digital discourse.

**Key analyses:**
- Sentiment distribution (positive/neutral/negative)
- Emotional fingerprints by actor type
- Controversy detection and analysis
- Temporal patterns of emotional expression

### Map 4: Temporal Dynamics
> **How does Croatian Catholic digital communication evolve over time, and how does it respond to events?**

Examines communication patterns across multiple time scales—from hourly posting rhythms to annual liturgical cycles.

**Key analyses:**
- Macro trends (yearly, monthly growth patterns)
- Weekly and daily posting rhythms
- Liturgical calendar effects (Advent, Lent, Easter, feast days)
- Event response patterns
- Platform growth trajectories

---

## Actor Classification

The project classifies sources into meaningful actor types within the Croatian Catholic media landscape:

| Actor Type | Description |
|------------|-------------|
| **Institutional Official** | HKM (Croatian Catholic Network), IKA (Catholic News Agency), HBK (Bishops' Conference) |
| **Diocesan** | Dioceses and archdioceses (Zagreb, Split-Makarska, Rijeka, etc.) |
| **Independent Media** | Laudato TV, Bitno.net, Glas Koncila, Nova Eva |
| **Religious Orders** | Franciscans, Jesuits, Dominicans, Salesians, Carmelites, etc. |
| **Individual Priests** | Personal accounts of clergy members |
| **Charismatic Communities** | Charismatic renewal movements |
| **Youth Organizations** | Catholic youth groups and initiatives |
| **Academic** | Catholic educational institutions |
| **Lay Influencers** | Individual Catholic content creators |

---

## Platforms Analyzed

| Platform | Color Code |
|----------|------------|
| Web portals | ![#4285F4](https://via.placeholder.com/15/4285F4/4285F4.png) `#4285F4` |
| Facebook | ![#1877F2](https://via.placeholder.com/15/1877F2/1877F2.png) `#1877F2` |
| Instagram | ![#E4405F](https://via.placeholder.com/15/E4405F/E4405F.png) `#E4405F` |
| YouTube | ![#FF0000](https://via.placeholder.com/15/FF0000/FF0000.png) `#FF0000` |
| Twitter/X | ![#1DA1F2](https://via.placeholder.com/15/1DA1F2/1DA1F2.png) `#1DA1F2` |
| Forums | ![#FF6600](https://via.placeholder.com/15/FF6600/FF6600.png) `#FF6600` |
| Reddit | ![#FF4500](https://via.placeholder.com/15/FF4500/FF4500.png) `#FF4500` |

---

## Methodology

### Data Collection
- **Corpus size:** 600,000+ posts
- **Time period:** 2021 – 2026
- **Sources:** Web scraping, API collection, platform exports

### Analytical Methods
- **Topic Modeling:** Structural Topic Models (STM) for thematic discovery
- **Sentiment Analysis:** Automated classification + Facebook reactions
- **Network Metrics:** Gini coefficients, Lorenz curves, power-law fitting
- **Time Series Analysis:** Rolling averages, YoY comparisons, CAGR calculations

### Technology Stack
- **Language:** R
- **Document System:** Quarto
- **Key Packages:** tidyverse, ggplot2, quanteda, stm, tidytext, data.table

---

## Repository Structure

```
├── paper/                          # Working paper
│   ├── attention_markets_paper.qmd # Paper source
│   └── attention_markets_paper.html# Paper rendered
├── maps/                           # Interactive map analyses
│   ├── map_1_platform_actors.qmd   # Map 1 source
│   ├── map_1_platform_actors.html  # Map 1 rendered
│   ├── map_2_thematic.qmd          # Map 2 source
│   ├── map_2_thematic.html         # Map 2 rendered
│   ├── map_3_emotional.qmd         # Map 3 source
│   ├── map_3_emotional.html        # Map 3 rendered
│   ├── map_4_temporal.qmd          # Map 4 source
│   └── map_4_temporal.html         # Map 4 rendered
├── archive/                        # Previous versions
├── output/                         # Additional outputs
├── CLAUDE.md                       # AI assistant instructions
├── README.md                       # This file
└── .gitignore                      # Git ignore rules
```

---

## Theoretical Framework

This project draws on:
- **Platform studies** and affordance theory (van Dijck, 2013)
- **Attention economics** and visibility inequality (Webster, 2014)
- **Long tail distributions** in online content (Anderson, 2006)
- **Digital religion studies** and mediatization of religion
- **Computational social science** methods for text analysis

---

## Citation

If you use this research, please cite:

```
Sikic (2026). Attention Markets in Religious Digital Media: Mapping the Croatian Catholic Digital Space.
https://github.com/lusiki/Mapping-Catholic-Digital-Media-Space
```

---

## Author

**DigiKat Project**
