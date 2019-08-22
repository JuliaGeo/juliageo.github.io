### Get involved
Communcation is mostly done on the Julia [Discourse](https://discourse.julialang.org/c/domain/geo). More short-lived interaction is found on Julia [Slack #geo](https://slackinvite.julialang.org/). Feel free to create issues, PRs on packages.

We're currently discussing changes to our common GeoInterface.

### Packages
Here's a partial listing of some of the existing libraries in julia that you can use for working with geospatial data. Not all of them are listed under the JuliaGeo organization, but some of them might get moved over.

#### Wrappers for external libraries
Using the excellent [BinaryBuilder.jl](https://github.com/JuliaPackaging/BinaryBuilder.jl) we try to provide prebuilt binaries for most external libraries.
- [LibGEOS.jl](https://github.com/JuliaGeo/LibGEOS.jl) is a wrapper to GEOS for performing geospatial operations on vector geometries
- [Proj4.jl](https://github.com/JuliaGeo/Proj4.jl) is a wrapper to PROJ.4 for performing cartographic projections
- [GDAL.jl](https://github.com/JuliaGeo/GDAL.jl) is a wrapper to GDAL (Geospatial Data Abstraction Library) for reading and writing raster and vector datasets; [ArchGDAL.jl](https://github.com/yeesian/ArchGDAL.jl) builds on top of GDAL.jl for a more Julian user experience. [GeoArrays.jl](https://github.com/evetion/GeoArrays.jl) builds on top of both to provide the easiest, but simplest experience.
- [NetCDF.jl](https://github.com/JuliaGeo/NetCDF.jl) and [NCDatasets.jl](https://github.com/Alexander-Barth/NCDatasets.jl) provides a high-level and a medium-level interface for writing and reading netcdf files.
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

#### Other Projects
- [OpenStreetMapX.jl](https://github.com/pszufe/OpenStreetMapX.jl) provides basic functionality for parsing, viewing, and working with OpenStreetMap map data.
- [LasIO.jl](https://github.com/visr/LasIO.jl) is native Julia package for working with .las pointcloud data. [LazIO.jl](https://github.com/evetion/LazIO.jl) does the same for compressed .laz pointcloud data.


