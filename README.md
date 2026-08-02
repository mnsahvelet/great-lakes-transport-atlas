# Great Lakes Potential Longshore Sediment Transport Atlas

An interactive web map of shoreline-scale potential longshore sediment transport
for the five Laurentian Great Lakes (Superior, Michigan, Huron, Erie, Ontario),
computed with the van Rijn (2014) formulation.

**Live map:** https://mnsahvelet.github.io/great-lakes-transport-atlas/

> **Status:** This repository accompanies a manuscript currently in preparation.
> The interactive map is provided for review purposes. Please do not redistribute
> the link until the associated paper is published.

## What's in the map

- Interactive five-lake shoreline map (Leaflet / Folium, Esri satellite basemap)
- ~1,940 shoreline segments with potential transport magnitude and direction
- Signed transport-direction coloring
- Per-segment time series and statistics on click
- Layer control for individual lakes and map backgrounds

## Repository contents

| File | Purpose |
|------|---------|
| `index.html` | The interactive map (open this in a browser) |
| `.nojekyll` | Tells GitHub Pages to serve files as-is (required for Folium output) |
| `robots.txt` | Requests that search engines do not index the page |
| `README.md` | This file |
| `LICENSE` | License terms |
| `CITATION.cff` | How to cite this work |

## How to view

Open `index.html` in any modern browser (Chrome recommended), or visit the
GitHub Pages link above. An internet connection is required because the Esri
satellite basemap and map libraries load from online services.

## Method (summary)

Potential longshore sediment transport was estimated at shoreline segments
around the Great Lakes using wave conditions and the van Rijn (2014) transport
formulation. Segment-level gross (Qgross) and net (Qnet) transport quantities
are visualized. Full methodology is described in the accompanying manuscript.

## Data sources

- Wave data: USACE WIS (Wave Information Studies) hindcast
- Shoreline geometry: derived shoreline segments (see manuscript)

## Citation

If you use this atlas, please cite it using the metadata in `CITATION.cff`
(and the associated paper once published).

## License

See `LICENSE`.

## Contact

Muhammed Sahvelet — muhammedsahvelet@gmail.com
