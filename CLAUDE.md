# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains Jupyter notebooks for studying urban data science concepts

## Environment Setup

- Python environment managed via `.venv/` virtual environment
- API keys stored in `.env` file (never commit this file)

## Running Notebooks

All work is done in Jupyter notebooks. To run:

```bash
# Activate virtual environment
source .venv/bin/activate

# Launch Jupyter
jupyter notebook
```

## Creating New Notebooks

When creating new Jupyter notebooks, ALWAYS include the content from `HEADER.md` as the first markdown cell. This header contains:
- University name and program information
- Course title
- Professor and student details
## Key Dependencies

- numpy: Array operations and random number generation
- matplotlib: Plotting and animations
- pandas: Data manipulation for city population datasets
- scipy: Statistical analysis (power law fitting)

## Common Analysis Patterns

**Random Walk Analysis:**
- Walks are simulated using `np.random.choice([-1, 1])` for steps
- Position tracking via `np.cumsum()` on step arrays
- Multiple walks analyzed to measure standard deviation scaling

**Zipf Analysis:**
- Log-log plots of rank vs population
- Power law fitting using `np.polyfit()` on log-transformed data
- R² calculation to validate fit quality