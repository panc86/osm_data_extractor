# OpenStreetMap (OSM) Data Extractor

## Map Features

https://wiki.openstreetmap.org/wiki/Map_features

- Buildings
- Hospitals
- Airports
- Runways
- Network Towers

## Normalization

### Buildings

Only 0.4% of buildings have `height`.

Missing `height` are filled out with value range 10-90 mt.
Wrong format e.g., 15m (str) instead of 15 (int), is normalized to numeric.

### Runways

Only runways longer than 1000 mt are selected.
Missing data is filled out using knowledge from local aviation authority.
