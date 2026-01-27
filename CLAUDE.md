# CLAUDE.md - AI Instructions for DigiKat Project

## Project Overview

This is the **DigiKat Project** - a research initiative mapping the Croatian Catholic Digital Media Space. The project analyzes 600,000+ posts from 2021-2024 across multiple digital platforms.

## Technology Stack

- **Document Format**: Quarto (`.qmd` files with embedded R code)
- **Language**: R
- **Key Libraries**: tidyverse, ggplot2, quanteda, stm (Structural Topic Modeling), tidytext
- **Output**: HTML reports with interactive visualizations

## Project Structure

```
maps/                    # Main analysis files (source of truth)
├── map_1_platform_actors.qmd   # Platform & actor structure analysis
├── map_2_thematic.qmd          # Topic modeling & thematic analysis
├── map_3_emotional.qmd         # Sentiment & emotion analysis
└── map_4_temporal.qmd          # Temporal dynamics & patterns

archive/                 # Previous versions of analysis files
output/                  # Rendered HTML outputs
```

## The Four Maps

### Map 1: Platform and Actor Structure
- **Question**: Who communicates where, and who dominates visibility?
- **Analysis**: Platform distribution, engagement metrics, Lorenz curves, power laws
- **Actor Types**: Institutional Official, Diocesan, Independent Media, Individual Priests, Charismatic Communities, Religious Orders, Youth Organizations, Academic, Lay Influencers

### Map 2: Thematic Structure
- **Question**: What topics dominate Catholic digital discourse?
- **Analysis**: Structural Topic Modeling (STM) with 35 topics
- **Outputs**: Topic prevalence, word clouds, actor-topic heatmaps, platform profiles

### Map 3: Emotional Structure
- **Question**: What is the emotional tone of Catholic digital media?
- **Analysis**: Sentiment polarity, emotion detection (joy, anger, love, etc.)
- **Metrics**: Controversy scores, love/angry ratios, temporal emotion patterns

### Map 4: Temporal Dynamics
- **Question**: How does activity vary over time?
- **Analysis**: Time-series, growth patterns, hourly/daily/weekly rhythms
- **Special**: Liturgical calendar analysis (feast days, Sundays, liturgical seasons)

## Data Source

The analysis uses `merged_comprehensive.rds` located at:
```
C:/Users/lsikic/Luka C/HKS/Projekti/Digitalni Kat/SHKM/DigiKat/data/
```

**Note**: The raw data file is NOT included in this repository due to size/privacy.

## Platform Color Codes

| Platform | Color |
|----------|-------|
| web | #4285F4 |
| facebook | #1877F2 |
| instagram | #E4405F |
| youtube | #FF0000 |
| twitter | #1DA1F2 |
| forum | #FF6600 |
| reddit | #FF4500 |
| comment | #808080 |

## Working with This Project

### To render a single map:
```r
quarto::quarto_render("maps/map_1_platform_actors.qmd")
```

### To render all maps:
```r
quarto::quarto_render("maps/")
```

### Required R packages:
```r
install.packages(c(
  "tidyverse", "data.table", "scales", "ggplot2",
  "knitr", "kableExtra", "ineq", "quanteda",
  "quanteda.textstats", "stm", "tidytext",
  "pheatmap", "viridis", "RColorBrewer"
))
```

## Key Variables in Data

- `SOURCE_TYPE`: Platform (web, facebook, instagram, youtube, twitter, forum, reddit, comment)
- `FROM`: Source/actor name
- `DATE`: Publication date
- `TITLE`, `FULL_TEXT`: Content fields
- `year`, `month`, `day`: Temporal fields
- `INTERACTIONS`: Engagement metric

## Notes for AI Assistants

1. The `.qmd` files in `maps/` are the authoritative source files
2. Files in `archive/` are older versions - prefer `maps/` versions
3. HTML outputs and `*_files/` directories are generated - don't edit manually
4. Data path is hardcoded to local machine - may need adjustment for reproduction
5. The project focuses on Croatian Catholic media - content is primarily in Croatian
