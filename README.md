# PPGIA - N766 - Ciência de Dados aplicada a Ciência da Cidade

## About

This repository contains Jupyter notebooks exploring complex systems, urban modeling, and data analysis applied to urban contexts.

## Content

### Random Walk (`random_walk/`)
- **random_walk.ipynb** - Basic random walk implementation
- **animation.ipynb** - Random walk animations
- **histogram.ipynb** - Distribution analysis
- **stddev-1d.ipynb** - Standard deviation scaling in 1D
- **stddev-2d.ipynb** - Standard deviation scaling in 2D

Explores stochastic processes, movement patterns, and applications in urban mobility modeling.

### Schelling Model (`schelling/`)
- **schelling_model_analysis.ipynb** - Segregation model analysis
- **color_maps.ipynb** - Visualization with color maps

Simulates urban segregation patterns and emergent behaviors in self-organizing systems.

### Zipf's Law (`zipf/`)
- **zipf.ipynb** - Power law distribution analysis

Studies urban population distributions, power law fitting, and model validation through log-log analysis.

### Isochrone Mapping (`03-isochrone_mapping/`)
- **isochrone_analysis.ipynb** - Urban accessibility analysis using isochrone maps

Explores equal-time accessibility zones in urban networks. Analyzes transportation mode differences (walking, cycling, driving), temporal dynamics (rush hour vs off-peak), accessibility equity across neighborhoods, and optimal service location strategies. Demonstrates applications in transit planning, facility placement, and urban equity analysis.

### Scaling Analysis (`04-beta/`)
- **homicides.ipynb** - Full dataset analysis of homicides vs population scaling
- **homicides_10000.ipynb** - Analysis for cities ≥ 10,000 inhabitants
- **homicides_10000_1000000.ipynb** - Analysis for medium/large cities (10k-1M population)

Investigates the relationship between homicides and population across Brazilian municipalities (1980-2022) using scaling laws. Performs log-log regression analysis to extract scaling exponent β, revealing whether the relationship is superlinear (β>1), linear (β≈1), or sublinear (β<1). Tracks temporal evolution of β to understand how urban violence scaling patterns change over decades. Includes multiple population filters to analyze different city size ranges and exclude outliers.

