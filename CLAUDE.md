# Project: Inertia and Primary Frequency Regulation Requirement Analysis

## Overview
This project develops methods for analyzing inertia and primary frequency regulation requirements in power systems. The research uses the RTS-GMLC (Reliability Test System - Grid Modernization Lab Consortium) dataset for validation and case studies.

## Project Structure
```
.
├── 文章初稿/              # Article draft (LaTeX)
│   └── main.tex          # Main LaTeX file (Elsevier format, Applied Energy)
│   └── sections/         # Paper sections (introduction, methods, results, etc.)
│   └── references.bib    # Bibliography
├── RTS-GMLC/             # Test system data (cloned from GridMod/RTS-GMLC)
│   ├── RTS_Data/
│   │   ├── SourceData/        # Original source data
│   │   ├── FormattedData/     # Processed data formats
│   │   └── timeseries_data_files/  # Time series (load, renewables, etc.)
│   └── RTS-GMLC.pdf      # System documentation
└── CLAUDE.md             # This file
```

## Research Focus
- **Inertia analysis**: System inertia requirements with increasing renewable penetration
- **Primary frequency regulation**: Governor response and frequency control
- **Test system**: IEEE RTS-GMLC (73-bus, 3-area system)

## Key Data Files in RTS-GMLC
- Generator parameters (capacity, ramp rates, costs)
- Load profiles (hourly/5-minute resolution)
- Renewable generation time series (solar, wind)
- Network topology and branch data

## LaTeX Compilation
```bash
cd 文章初稿
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## Conventions
- Language: Paper may be written in English or Chinese
- Units: SI units (MW, Hz, seconds)
- Figures: Save in `文章初稿/figures/`

## References
- RTS-GMLC GitHub: https://github.com/GridMod/RTS-GMLC
- Original RTS-96: IEEE Reliability Test System
