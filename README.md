### Get involved
Communcation is mostly done on the Julia [Discourse](https://discourse.julialang.org/c/domain/geo). More short-lived interaction is found on Julia [Slack #geo](https://julialang.org/slack/). Feel free to create issues, PRs on packages.

We're currently discussing changes to our common GeoInterface.

### Talks
- FOSS4G 2019 Bucharest by @visr, @evetion. JuliaGeo: A Fresh Approach to Geospatial Computing. [Video](https://media.ccc.de/v/bucharest-428-juliageo-a-fresh-approach-to-geospatial-computing), [Slides](https://nextjournal.com/juliageo/foss4g-2019).

### GitHub organizations
The [JuliaGeo](https://github.com/JuliaGeo) GitHub organization is intended primarily for the collaborative development of packages that are generally applicable across the geospatial and geosciences domains. For dealing with geospatial data, packages from the [JuliaGeometry](https://github.com/JuliaGeometry) and [JuliaImages](https://github.com/JuliaImages) organizations may also be of interest, and we will aim for good integration with those. Since the JuliaGeo organization aims to provide mostly general tools, more domain specific packages may be better suited for development in domain specific organizations. [JuliaClimate](https://github.com/JuliaClimate) is a nice example of such an organization that will be especially interesting to climate, atmosphere and ocean scientists.
[EcoJulia](https://github.com/EcoJulia) also provides some tools for generating and downloading spatial data sets, with a focus on ecological applications.

### Packages
Here's a partial listing of some of the existing libraries in [Julia](https://julialang.org/) that you can use for working with geospatial data. Not all of them are listed under the JuliaGeo organization, but some of them might get moved over.

#### Wrappers for external libraries
Using the excellent [BinaryBuilder.jl](https://github.com/JuliaPackaging/BinaryBuilder.jl) we try to provide prebuilt binaries for most external libraries.
- [LibGEOS.jl](https://github.com/JuliaGeo/LibGEOS.jl) is a wrapper to GEOS for performing geospatial operations on vector geometries
- [Proj4.jl](https://github.com/JuliaGeo/Proj4.jl) is a wrapper to PROJ.4 for performing cartographic projections
- [GDAL.jl](https://github.com/JuliaGeo/GDAL.jl) is a wrapper to GDAL (Geospatial Data Abstraction Library) for reading and writing raster and vector datasets; [ArchGDAL.jl](https://github.com/yeesian/ArchGDAL.jl) builds on top of GDAL.jl for a more Julian user experience. [GeoArrays.jl](https://github.com/evetion/GeoArrays.jl) builds on top of both to provide the easiest, but simplest experience.
- [Rasters.jl](https://github.com/rafaqz/Rasters.jl) defines common types and methods for reading, writing and manipulating rasterized spatial data.
- [NetCDF.jl](https://github.com/JuliaGeo/NetCDF.jl) and [NCDatasets.jl](https://github.com/Alexander-Barth/NCDatasets.jl) provides a high-level and a medium-level interface for writing and reading netcdf files.
- [GeoDataFrames.jl](https://github.com/evetion/GeoDataFrames.jl) provides simple geographical vector interaction built on top of ArchGDAL with a Tables.jl interface.
- [GMT.jl](https://github.com/joa-quim/GMT.jl) provides a wrapper for working with the [G]eneric [M]apping [T]ools (GMT) library in julia.
- [LibSpatialIndex.jl](https://github.com/JuliaGeo/LibSpatialIndex.jl) provides functionality for spatially indexing kD bounding box data (based on [libspatialindex](https://github.com/libspatialindex/libspatialindex))

#### Native Julia libraries
- [GeoInterface.jl](https://github.com/JuliaGeo/GeoInterface.jl) is a Julia package defining the common interface between packages, currently mostly based on the GeoJSON format
- [Geodesy.jl](https://github.com/JuliaGeo/Geodesy.jl) is a Julia package for working with points defined in different coordinate systems, with support for LLA/ENU/ECEF currently.
- [CoordinateTransformations.jl](https://github.com/FugroRoames/CoordinateTransformations.jl) is a Julia package to manage simple or complex networks of coordinate system transformations.
- [Shapefile.jl](https://github.com/JuliaGeo/Shapefile.jl) is a Julia package that parses in ESRI Shapefiles.
- [GeoJSON.jl](https://github.com/JuliaGeo/GeoJSON.jl) is a Julia package that provides utilities for encoding and decoding GeoJSON formatted data.
- [NearestNeighbors.jl](https://github.com/KristofferC/NearestNeighbors.jl) is Julia package to perform high performance nearest neighbor searches in arbitrarily high dimensions. It uses Kd-trees.
- [SpatialIndexing.jl](https://github.com/alyst/SpatialIndexing.jl) provides a native RTree implementation.
- [RegionTrees.jl](https://github.com/rdeits/RegionTrees.jl) provides Quadtrees, Octrees and their N-Dimensional cousins. 
- [GeoStats.jl](https://github.com/juliohm/GeoStats.jl) is an extensible Julia framework for high-performance geostatistics
- [Turf.jl](https://github.com/philoez98/Turf.jl) A spatial analysis library written in Julia, ported from the great Turf.js
- [RasterDataSources.jl](https://github.com/EcoJulia/RasterDataSources.jl) Simplifies downloads of environmental raster data like WorldClim, EarthEnv and CHELSA. 

#### Other Projects
- [OpenStreetMapX.jl](https://github.com/pszufe/OpenStreetMapX.jl) provides basic functionality for parsing, viewing, and working with OpenStreetMap map data.
- [LasIO.jl](https://github.com/visr/LasIO.jl) is native Julia package for working with .las pointcloud data. [LazIO.jl](https://github.com/evetion/LazIO.jl) does the same for compressed .laz pointcloud data.
- [GeoMakie.jl](https://github.com/JuliaPlots/GeoMakie.jl) adds cartography to the [Makie.jl](https://makie.juliaplots.org/stable/) plotting package.
- [OSMMakie.jl](https://github.com/fbanning/OSMMakie.jl) is a [Makie.jl](https://makie.juliaplots.org/stable/) recipe for plotting OpenStreetMap data. It works on top of [LightOSM.jl](https://github.com/DeloitteDigitalAPAC/LightOSM.jl) and currently provides basic functionality to plot all kinds of ways and buildings.


