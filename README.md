
##  JuliaGeo
The [JuliaGeo](https://github.com/JuliaGeo) GitHub organization serves as a focal point for developing and maintaining the next generation of tooling for geospatial analysis. It aims to leverage the intuitive syntax and high-performance of the [Julia language](https://julialang.org/) to provide robust, efficient, and easy-to-use tools for working with geographic data.

## Get involved
JuliaGeo fosters a collaborative environment for creating a comprehensive geospatial toolkit within the Julia ecosystem. Communication is mostly done on:
1. [Julia Geo Discourse](https://discourse.julialang.org/c/domain/geo) for general questions on the JuliaGeo ecosystem 
2. [Slack #geo](https://julialang.org/slack/) for more short-lived interaction. 

Feel free to create issues and/or PRs on packages.

## High-level packages
Most geospatial analysis can be accomplished with these three packages (in combination with extensions as needed):

1. [Rasters.jl](https://rafaqz.github.io/Rasters.jl/dev/) provides a powerful Julia framework for reading, writing, and manipulating rasterized spatial data, such as satellite imagery or climate model outputs. It offers a standardized interface to work with various data formats and in-memory arrays through Raster, RasterStack, and RasterSeries types, simplifying complex geospatial workflows. Rasters.jl provides [significant performance gains](https://github.com/user-attachments/assets/1c6c56ac-4c5a-4096-984d-15bf2783682c) over similar packages in other languages.

2. [GeoDataFrames.jl](https://www.evetion.nl/GeoDataFrames.jl/dev/) enables the handling of geospatial vector data in Julia by integrating geometric operations directly within DataFrame structures, inspired by Python's [GeoPandas](https://geopandas.org/en/stable/). It achieves this by treating a vector of geometries as a column, allowing for intuitive spatial data manipulation and analysis alongside tabular attributes.

3. [GeometryOps.jl](https://juliageo.org/GeometryOps.jl/dev/) provides a suite of highly efficent geometric operations for vector data (i.e. points, lines, polygons), designed to work seamlessly with any [GeoInterface.jl](https://juliageo.org/GeoInterface.jl/dev/) compatible geometry. It aims to unify geometric calculations within the Julia ecosystem by offering pure Julia implementations of common spatial functions crucial for GIS and Earth data workflows. GeometryOps.jl provides [significant performance gains](https://github.com/JuliaGeo/GeometryOps.jl/assets/32143268/0be8672c-c90f-4e1d-81c5-8522317c5e29) over similar packages in other languages.

## Inter-package operability
[GeoInterface.jl](https://juliageo.org/GeoInterface.jl/dev/) serves as a Julia protocol and interface for handling geospatial data. It provides a set of traits based on the Simple Features standard, enabling the parsing, serialization, and usage of various geometries within the Julia ecosystem.

[GeoFormatTypes.jl](https://github.com/JuliaGeo/GeoFormatTypes.jl): Defines wrapper types to make it easy to pass and dispatch on geographic formats (like Well Known Text) between packages.

[CommonDataModel.jl](https://github.com/JuliaGeo/CommonDataModel.jl): Defines a common data model for NetCDF, GRIB, Zarr, and GeoTIFF datasets.

## Visualization
See [Makie](https://docs.makie.org/stable/) and [Plots.jl](https://docs.juliaplots.org/stable/) for general purpose plotting.

[Tyler.jl](https://github.com/MakieOrg/Tyler.jl) for displaying tiled maps interactively with [Makie](https://docs.makie.org/stable/).

[GeoMakie.jl](https://github.com/MakieOrg/GeoMakie.jl) for geographic plotting utilities using [Makie](https://docs.makie.org/stable/).


## Lower-level file I/O - native Julia
[NCDatasets.jl](https://github.com/JuliaGeo/NCDatasets.jl): For working with NetCDF files, a common format for scientific data, including climate and oceanographic data. (Also NetCDF.jl exists).

[GeoJSON.jl](https://github.com/JuliaGeo/GeoJSON.jl): Offers utilities for reading, writing, and manipulating GeoJSON data, a widely used open standard format for encoding geographic data structures.

[Shapefile.jl](https://github.com/JuliaGeo/Shapefile.jl): Enables the reading and writing of ESRI Shapefiles, a common vector data format in GIS.

[GeoParquet.jl](https://github.com/JuliaGeo/GeoParquet.jl): Facilitates working with geospatial data stored in Parquet files.

[LazIO](https://github.com/evetion/LazIO.jl): Enables the reading and writing of Laz files.

[STAC.jl](https://github.com/JuliaClimate/STAC.jl): SpatioTemporal Asset Catalogs (STAC) client in Julia

[FlatGeobuf.jl](https://github.com/evetion/FlatGeobuf.jl): A native flatgeobuf implementation in Julia

## Lower-level packages - C bindings
[ArchGDAL.jl](https://yeesian.com/ArchGDAL.jl) A complete solution for working with GDAL in Julia.

[GDAL.jl](https://github.com/JuliaGeo/GDAL.jl): A Julia wrapper for the powerful Geospatial Data Abstraction Library (GDAL), enabling the reading and writing of a vast array of raster and vector geospatial data formats.

[LibGEOS.jl](https://github.com/JuliaGeo/LibGEOS.jl): A wrapper for the GEOS (Geometry Engine - Open Source) library, offering a wide range of geometry operations.

[Proj.jl](https://github.com/JuliaGeo/Proj.jl): A Julia wrapper for the PROJ library, which is a standard for coordinate transformations and cartographic projections. (Note: Proj4.jl was an older version, with Proj.jl being the more current wrapper).


## Access to geospatial datasets
[MapTiles.jl](https://github.com/JuliaGeo/MapTiles.jl): For working with tiled web maps.

[GADM.j](https://github.com/JuliaGeo/GADM.jl): Provides access to the GADM dataset of global administrative areas.

[NaturalEarth.jl](https://github.com/JuliaGeo/NaturalEarth.jl) Interface to the Natural Earth dataset.

[GeoDatasets.jl](https://github.com/JuliaGeo/GeoDatasets.jl) Access to common geographic datasets.

[SpaceLiDAR.jl](https://github.com/evetion/SpaceLiDAR.jl) Utilities for accessing and working with satellite altimetry data (i.e. ICESat, ICESat-2, GEDI)


## Geospatial analysis packages
[Geomorphometry.jl](https://deltares.github.io/Geomorphometry.jl/v0.7.0/) Geospatial operations, cost and filtering algorithms as used for elevation rasters.

[Geodesy.jl](https://github.com/JuliaGeo/Geodesy.jl): Provides tools for working with points defined in various coordinate systems (e.g., LLA, ECEF, ENU) and performing geodetic calculations.

[SortTileRecursiveTree.jl](https://github.com/asinghvi17/SortTileRecursiveTree.jl) An Sort-Tile-Recursive (SRT) tree implementation for GeoInterface compatible geometries.