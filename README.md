# Terrain Analogs for Lunar and Martian Lava-Tube Sites

A case study in the Krong No volcanic field (Lam Dong Province, Vietnam)

NASA Space Apps Challenge 2026: *Identify Earth Locations that Analog the Permanent Moon Base Locations and Mars*

## Research Question

How closely does the terrain of the Krông Nô volcanic field resemble lava-tube pit and skylight sites at Marius Hills (Moon) and Arsia Mons (Mars), in terms of slope and surface roughness?

## Hypothesis

The terrain similarity between Krông Nô and the Moon/Mars sites is greater than the similarity between a non-volcanic control region (Mekong Delta) and those same sites.

## Why It Matters

Lava tubes are candidate locations for permanent bases because they may offer natural shelter. If Krông Nô is a terrain analog, it could support rover testing and lava-tube survey practice on Earth.

## Scope

- **In scope:** regional-scale terrain comparison using open DEMs, resampled to a common ~200 m resolution.
- **Out of scope:** climate, atmosphere, radiation, vegetation, and pit-scale morphology.

## Study Sites

Coordinates are listed in [`sites.csv`](sites.csv).

| Body | Site | Feature type |
|---|---|---|
| Earth | Krông Nô (Nâm Kar, Nâm B'Lang, lava caves) | Cinder cones, lava tubes |
| Moon | Marius Hills Pit | Mare pit / lava-tube skylight candidate |
| Mars | Arsia Mons region | Lava-tube skylight candidates |
| Earth (control) | Mekong Delta | Non-volcanic alluvial plain |

## Data Sources

- Earth: NASADEM / SRTM (NASA Earthdata)
- Moon: LRO LOLA gridded DEM (NASA PDS Geosciences Node)
- Mars: MGS MOLA / MEX HRSC blended DEM (USGS Astrogeology)

## Method (planned)

1. Crop a 50 × 50 km window around each site.
2. Resample all DEMs to a common resolution (~200 m).
3. Compute slope and local roughness.
4. Compare distributions using the normalized Wasserstein distance.
5. Compare each Moon/Mars site against Krông Nô and against the control.

## Limitations

- Earth, Moon and Mars differ in climate, erosion history and gravity; only terrain is compared.
- DEM resolution (~200 m) cannot resolve individual pits; the analysis is regional.
- Earth lava tubes are generally smaller than those inferred on the Moon and Mars, so the analog applies to feature type, not scale.

## Author

Nguyen Ngoc Thao Nguyen, NASA Space Apps Challenge 2026 (solo participant)
