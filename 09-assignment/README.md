# Final Assignment - Optimal Placement of Government Services in Ceará

## Objective

Apply urban data science concepts to determine optimal placement of government services or private businesses in Ceará municipalities, using socioeconomic metrics from IPEADATA.

## Course Concepts Applied

1. **Zipf's Law** - City size distributions for understanding population hierarchy
2. **Voronoi Diagrams** - Service area allocation and coverage analysis
3. **Scaling Laws (β exponent)** - Resource allocation based on population scaling
4. **Gravity Models** - Distance decay effects on accessibility

## Data Sources

### Population Data
- **IPEADATA** (http://www.ipeadata.gov.br/)
  - Population by municipality (2022 Census)
  - Employment/unemployment data (optional extension)
  - IDHM, PIB per capita (optional extension)

### Geographic Data
- **Municípios Brasileiros Dataset** (https://github.com/kelvins/Municipios-Brasileiros)
  - Latitude/longitude for all 5,570 Brazilian municipalities
  - IBGE codes for data joining

### Existing Project Data
- `../02-zipf/ceara_cities.csv` - Population data for 184 Ceará municipalities

## Methodology

### 1. Data Preparation
- Load population data from existing Zipf analysis
- Fetch geographic coordinates from GitHub dataset
- Merge datasets on IBGE municipal code

### 2. Exploratory Analysis
- Visualize municipality distribution
- Apply Zipf's Law to understand city hierarchy
- Identify population concentration patterns

### 3. Optimal Placement Algorithms

#### 3.1 Population-Weighted Centroid
Single facility location that minimizes total weighted distance to population.

#### 3.2 Weighted K-Means
Multiple facility location using population-weighted k-means clustering:
- Initialize centers from high-population cities
- Assign cities to nearest center
- Recalculate centers as population-weighted centroids
- Iterate until convergence

#### 3.3 Voronoi Service Areas
Visualize service regions using Voronoi tessellation from optimal centers.

#### 3.4 Gravity Model Accessibility
Calculate accessibility scores using distance decay:

$$A_{ij} = \frac{1}{d_{ij}^\beta}$$

Where β is the distance decay exponent (typically 1.5-2.0).

### 4. Scaling Law Application
Use β exponent from scaling laws for resource allocation:
- β = 1.0: Linear (proportional to population)
- β > 1.0: Superlinear (larger cities get more per capita)
- β < 1.0: Sublinear (smaller cities get more per capita)

## Files

- `final_assignment.ipynb` - Main Jupyter notebook with full analysis
- `README.md` - This documentation file

## Required Libraries

```python
# Core
pandas
numpy
matplotlib

# Geospatial
scipy (Voronoi, cdist, optimize)

# Optional
folium  # Interactive maps
geopandas  # Spatial analysis
ipeadatapy  # IPEADATA API wrapper
```

## Installation

```bash
pip install pandas numpy matplotlib scipy
pip install ipeadatapy  # Optional: for additional IPEADATA metrics
```

## Usage

```bash
# Activate virtual environment
source .venv/bin/activate

# Launch Jupyter
jupyter notebook 09-assignment/final_assignment.ipynb
```

## References

- IPEADATA: http://www.ipeadata.gov.br/
- IBGE: https://www.ibge.gov.br/
- Municípios Brasileiros: https://github.com/kelvins/Municipios-Brasileiros
- ipeadatapy: https://www.luanborelli.net/ipeadatapy/docs/
