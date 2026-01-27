# DigiKat: Mapping the Croatian Catholic Digital Media Space

A comprehensive research project analyzing 600,000+ posts from Croatian Catholic digital media across multiple platforms (2021-2024).

## Overview

This project produces four analytical "maps" that examine different dimensions of Catholic digital media presence:

| Map | Focus | Key Question |
|-----|-------|--------------|
| **Map 1** | Platform & Actor Structure | Who communicates where? Who dominates visibility? |
| **Map 2** | Thematic Structure | What topics dominate Catholic digital discourse? |
| **Map 3** | Emotional Structure | What is the emotional tone and sentiment? |
| **Map 4** | Temporal Dynamics | How does activity vary over time? |

## Repository Structure

```
├── maps/                        # Quarto analysis files (.qmd)
│   ├── map_1_platform_actors.qmd
│   ├── map_2_thematic.qmd
│   ├── map_3_emotional.qmd
│   └── map_4_temporal.qmd
├── archive/                     # Previous versions
├── output/                      # Rendered HTML reports
├── CLAUDE.md                    # AI assistant instructions
└── README.md                    # This file
```

## Technology

- **Analysis**: R with Quarto
- **Topic Modeling**: Structural Topic Modeling (STM)
- **Visualization**: ggplot2, pheatmap
- **Text Analysis**: quanteda, tidytext

## Actor Classification

The project classifies sources into meaningful actor types:

- Institutional Official (HKM, IKA, HBK)
- Diocesan (Biskupije, Nadbiskupije)
- Independent Media (Laudato, Bitno.net, Glas Koncila)
- Religious Orders (Franciscans, Jesuits, Dominicans, etc.)
- Individual Priests
- Charismatic Communities
- Youth Organizations
- Academic
- Lay Influencers

## Requirements

```r
install.packages(c(
  "tidyverse", "data.table", "scales", "ggplot2",
  "knitr", "kableExtra", "ineq", "quanteda",
  "quanteda.textstats", "stm", "tidytext",
  "pheatmap", "viridis", "RColorBrewer"
))
```

## Usage

Render individual maps:
```bash
quarto render maps/map_1_platform_actors.qmd
```

Render all maps:
```bash
quarto render maps/
```

## Data

The analysis uses a merged dataset (`merged_comprehensive.rds`) containing posts from:
- Web portals
- Facebook pages
- Instagram accounts
- YouTube channels
- Twitter/X accounts
- Forums
- Reddit

**Note**: Raw data is not included in this repository.

## Author

DigiKat Project

## License

[Add your preferred license]
