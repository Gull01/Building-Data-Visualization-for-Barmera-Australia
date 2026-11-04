# Building Footprints of Barmera, South Australia

An interactive web map of building footprints in Barmera, a town in the Riverland region of South Australia, built with GeoPandas and Folium. Hover over any building to see its type.

## What the map shows

- Building footprint polygons loaded from a shapefile
- A tooltip with the building type for each footprint
- Google Satellite imagery plus several other basemaps, switchable from the layer control
- The map is centred automatically on the mean centroid of all buildings

## Run it

```bash
pip install geopandas folium jupyter
jupyter notebook "Building Data Visualization for Barmera-Australia.ipynb"
```

The building shapefile is not included in this repository. Point `shapefile_path` in the first cell to your own copy (the notebook expects a `building` attribute for the tooltip). Building footprints for Australia can be downloaded from OpenStreetMap, for example through [Geofabrik](https://download.geofabrik.de/australia-oceania/australia.html).

Running the notebook saves the map as `aus_building_data_map.html`.

Note: the Stamen basemaps in the notebook are no longer served at their old address. If they fail to load, remove those `TileLayer` lines.

## Built with

Python, GeoPandas, Folium (Leaflet)

## Author

Gul Nawaz. [gulnawaz.dev](https://gulnawaz.dev)
