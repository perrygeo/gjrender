# GeoJSON rendering at the command line

Takes a stream of GeoJSON Features and renders it to a png using Mapnik.

**Status**: proof of concept, barely working

Example:

```
fio cat countries.shp | gjrender out.png && open out.png
```

## TODO

Ultimately I'd like to have a CLI for rendering maps that would efficiently stream features, style them automatically (e.g. 5 natural breaks with RedYellow color ramp on the AREA field), a web interface to zoom, pan, and idenify, and a way to visualize the distribution of numeric properties.
