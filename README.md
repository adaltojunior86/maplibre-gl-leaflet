## MapLibre GL Leaflet

This is a binding from [MapLibre GL JS](https://maplibre.org) to the familiar
[Leaflet](http://leafletjs.com/) API. It was originally developed for Mapbox (https://github.com/mapbox/mapbox-gl-leaflet) and was migrated to MapLibre after Mapbox changed its license.

## Code example

## Installation

## Motivation
This project is a fork from [@maplibre/maplibre-gl-leaflet](https://github.com/maplibre/maplibre-gl-leaflet). I needed to improve the code to export the function that creates the layer instead of adding it to variable `L` of the leaflet. In my project, any other library overrides the variable `L` and removes the function to create the map libre of the layer. I took the opportunity to make any changes suggested by lint and improve the code to use the es2021 specification.

This project makes it possible to easily add a maplibre-gl-js layer in your Leaflet map. When using maplibre-gl-leaflet, you won't be able to use some of the maplibre-gl-js features.
Here are the main differences between a "pure" maplibre-gl-js map and a Leaflet map using maplibre-gl-leaflet:
- No rotation / bearing / pitch support
- Slower performances: When using maplibre-gl-leaflet, maplibre-gl-js is set as not interactive. Leaflet receives the touch/mouse events and updates the maplibre-gl-js map behind the scenes. Because maplibre-gl-js doesn't redraw as fast as Leaflet, the map can seem slower.

On the bright side, the maplibre-gl-leaflet binding will allow you to use all the leaflet features and plugins.

If you only need the maplibre-gl-js features ([adding a map with a mapbox-style, adding a GeoJSON, etc.](https://maplibre.org/maplibre-gl-js-docs/example/)), you are probably better off using it directly.

## Licence
ISC © [MapLibre](https://github.com/maplibre) © [Mapbox](https://github.com/mapbox)
