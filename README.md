# SpatialDataToolbox
A toolbox for manipulating spatial data.

## Installation

To install the current version, use `devtools`.

```R
devtools::install_github("MBalthasar/SpatialDataToolbox")
```

## Available Functions

The following functions are currently available and tested on Windows 10.

* `SHPDissolve()` This function automatically dissolves a shapefile based on its feature attributes.
* `UTMConversion()` This function automatically converts a raster or shapefile from a longlat projection into the corresponding UTM projection.
* `FishnetFunction()` This function creates a fishnet polygon from an input shapefile. The output fishnet will be reprojected to UTM.
* `TilesMaker()` This function divides the input file in tiles based on user preferences. The output data will be reprojected to UTM.
* `BookletMaker()` This function uses a fishnet polygon to create a map booklet pdf based on a ggplot. The booklet contains an overview map with the original ggplot and the fishnet polygon added on top, as well as sub-maps for each tile of the fishnet polygon.
