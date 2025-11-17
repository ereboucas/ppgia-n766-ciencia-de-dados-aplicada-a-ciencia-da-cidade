# TODO - Ciência de Dados Aplicada à Ciência da Cidade

## Current Work

### 07 - Percolation Theory
- [x] Create percolation study folder
- [x] Implement site percolation simulation
- [x] Add cluster identification algorithms
- [x] Add percolation threshold analysis
- [x] Create urban application examples (service coverage)
- [ ] Explore bond percolation
- [ ] Implement hierarchical percolation model
- [ ] Apply to real urban data (building density, green spaces)
- [ ] Create visualizations with real city data

## New Assignments

### Assignment 1: GSHL Population Density Visualization
- [ ] Download dataset from GSHL (Global Human Settlement Layer)
- [ ] Create new folder/notebook for GSHL analysis
- [ ] Load and process population density data
- [ ] Create visualizations of population density
- [ ] Add geographic context and analysis
- [ ] Document findings and patterns

### Assignment 2: Final Project Proposal
- [ ] Review all completed topics (random walk, Schelling, Zipf, isochrone, beta, Voronoi, Gibrat, percolation)
- [ ] Identify real dataset sources for chosen topic
- [ ] Draft project idea covering:
  - [ ] Topic selection from existing coursework
  - [ ] Real dataset identification (no simulated data)
  - [ ] Application of concepts learned
  - [ ] Expected outcomes and visualizations
- [ ] Prepare proposal presentation

## Completed Topics

### 00 - Random Walk
- [x] Basic implementation

### 01 - Schelling Model
- [x] Segregation dynamics

### 02 - Zipf's Law
- [x] City size distributions

### 03 - Isochrone Mapping
- [x] Urban accessibility analysis

### 04 - Beta Model
- [x] Implementation

### 05 - Voronoi Diagrams
- [x] Spatial analysis

### 06 - Gibrat's Law
- [x] Urban growth patterns

## Upcoming Topics

### Future Studies
- [ ] Network analysis (street networks, transit)
- [ ] Spatial statistics and autocorrelation
- [ ] Urban scaling laws (comprehensive study)
- [ ] Agent-based modeling applications
- [ ] Machine learning for urban predictions
- [ ] Fractal analysis of urban form

## Percolation - Detailed Tasks

### Theory
- [x] Understand site percolation basics
- [x] Learn about percolation threshold
- [x] Study cluster size distributions
- [ ] Research hierarchical percolation
- [ ] Investigate directed percolation
- [ ] Explore continuum percolation

### Implementation
- [x] Basic site percolation on square lattice
- [ ] Bond percolation implementation
- [ ] Hexagonal/triangular lattice geometries
- [ ] Hierarchical percolation multi-scale model
- [ ] Spatial heterogeneity (varying probabilities)
- [ ] 3D percolation models

### Urban Applications
- [x] Service coverage analysis (WiFi, transit)
- [ ] Green space connectivity mapping
- [ ] Building density and urban fabric continuity
- [ ] Infrastructure network resilience
- [ ] Population distribution patterns
- [ ] Gentrification and segregation dynamics
- [ ] Disease spread modeling

### Data Analysis
- [ ] Download real urban datasets
- [ ] Process building footprint data
- [ ] Analyze green space connectivity
- [ ] Study transit network coverage
- [ ] Map service accessibility gaps
- [ ] Compare different cities

## Project Ideas

### Research Questions
- [ ] What is the percolation threshold for green space connectivity in major Brazilian cities?
- [ ] How does transit coverage compare to the theoretical percolation threshold?
- [ ] Can we predict urban sprawl patterns using percolation models?
- [ ] How resilient are urban infrastructure networks to disruptions?
- [ ] Does segregation follow percolation-like phase transitions?

### Visualizations
- [ ] Interactive percolation explorer
- [ ] Real-time threshold finder
- [ ] Urban coverage heat maps
- [ ] Time-series percolation (city growth over time)
- [ ] Comparative analysis dashboard

## Notes

### Key Insights
- Site percolation threshold for 2D square lattice: p_c ≈ 0.593
- Below threshold: fragmented clusters
- Above threshold: spanning cluster emerges (phase transition)
- Critical behavior shows power-law distributions (scale-free)

### Resources to Explore
- [ ] Stauffer & Aharony - "Introduction to Percolation Theory"
- [ ] Urban scaling literature (Bettencourt, West)
- [ ] Complex networks and cities (Barthelemy)
- [ ] Real urban datasets: OSM, census data, satellite imagery

### Technical Debt
- [ ] Add unit tests for percolation functions
- [ ] Optimize cluster identification for large lattices
- [ ] Create reusable visualization library
- [ ] Document all functions with docstrings (done for site_percolation.ipynb)

## Questions for Professor/Discussion

- [ ] How to obtain high-resolution urban data for Fortaleza?
- [ ] Best practices for validating percolation models against real cities?
- [ ] Connection between percolation and other urban theories?
- [ ] Suggestions for final project topic?

---

Last updated: 2025-11-17 (Added new assignments)
