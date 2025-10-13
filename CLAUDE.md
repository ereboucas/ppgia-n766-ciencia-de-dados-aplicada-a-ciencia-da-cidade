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
