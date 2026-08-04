# Great Lakes Potential Longshore Sediment Transport Atlas

Interactive visualizations of shoreline-scale potential longshore sediment
transport for the five Laurentian Great Lakes (Superior, Michigan, Huron, Erie,
Ontario), computed with the van Rijn (2014) formulation from 1979–2023 wave
hindcast data.

> **Status:** This repository accompanies a manuscript currently in preparation.
> The interactive material is provided for review purposes. Please do not
> redistribute the links until the associated paper is published.

## Two ways to explore

**1. Detailed transport map** (`index.html`)
Full-resolution Folium/Leaflet map on an Esri satellite basemap: ~1,940
shoreline segments with potential transport magnitude and direction, signed
transport-direction coloring, per-segment time series, and layer control for
individual lakes and map backgrounds.

- Live: https://mnsahvelet.github.io/great-lakes-transport-atlas/

**2. Paper-companion dashboard** (`dashboard/index.html`)
A layered dashboard that mirrors the manuscript results. Switch between:

- Net transport (Qnet) — signed magnitude colorbar with white direction arrows
- Gross activity (Qgross)
- Multidecadal trend (Qgross %/decade; FDR-significant segments emphasized)
- Seasonal trend (DJF/MAM/JJA/SON)
- Leading EOF mode of Qnet variability (EOF1)
- Alongshore gradient (ΔQ) — erosion / accretion tendency
- Breaking-wave height (Hbreak) and offshore wave height (Hm0) climate
- ENSO teleconnection (OND Niño 3.4 correlation with Qgross)

Click any segment for its 1979–2023 annual time series and statistics. A
per-lake "unwrapped" alongshore profile panel and major-city / town labels
reproduce the manuscript figure style.

- Live: https://mnsahvelet.github.io/great-lakes-transport-atlas/dashboard/

## Repository contents

| Path | Purpose |
|------|---------|
| `index.html` | Detailed interactive transport map |
| `dashboard/index.html` | Paper-companion layered dashboard (self-contained, data embedded) |
| `.nojekyll` | Tells GitHub Pages to serve files as-is (required for these outputs) |
| `robots.txt` | Requests that search engines do not index the pages |
| `README.md` | This file |
| `LICENSE` | License terms |
| `CITATION.cff` | How to cite this work |

## How to view

Open either `index.html` (root) or `dashboard/index.html` in any modern browser
(Chrome recommended), or visit the GitHub Pages links above. An internet
connection is required because basemaps and map libraries load from online
services.

## Method (summary)

Hourly offshore waves from the USACE Wave Information Studies (WIS) hindcast were
routed to ~5 km shoreline points, transformed to depth-limited breaking
conditions (shoaling, refraction), and converted to hourly potential longshore
sediment transport using the van Rijn (2014) sand trendline. Hourly transport
was aggregated to net (Qnet) and gross (Qgross) quantities, directional balance
and persistence, Sen-slope trends, an EOF decomposition, alongshore gradients
(ΔQ), and climate-index associations. Full methodology is described in the
accompanying manuscript.

## Data sources

- Wave data: USACE WIS (Wave Information Studies) hindcast, 1979–2023
- Shoreline geometry: derived ~5 km shoreline points and segments (see manuscript)
- Climate indices: OND Niño 3.4 (ENSO)

## Citation

If you use this atlas, please cite it using the metadata in `CITATION.cff`
(and the associated paper once published).

## License

See `LICENSE`.

## Contact

Muhammed N. Sahvelet — muhammedsahvelet@gmail.com
