---
title: "Introduction to the EOPF Zarr Plugins"
format:
    html:
        code-fold: true
---

## 🗺️ Overview of EOPF Zarr Plugins

![plugins_overview](img/plugins_overview.png){fig-align="center"}

We build the following plugins:

* xarray EOPF backend
* xcube EOPF data store
* GDAL EOPF driver
* Julia EOPF reader
* SNAP EOPF reader (Prototype for Sentinel-2 L2A)

These plugins can be used in the following visualization framework:

![visualization_overview](img/visualization_overview.png){fig-align="center"}

### What we will learn

- 🔍 What can be done with each plugin.
- 🌳 Current developement state future developement plans of each plugin.
- 🔦 How to access data with each plugin.


### xarray-eopf backend

`xarray-eopf` is a Python package that enhances [xarray](https://docs.xarray.dev/en/stable/user-guide/io.html) by a new backend
named `"eopf-zarr"`. This backend allows for reading the [ESA EOPF data](https://eopf.copernicus.eu/eopf-products-and-adfs/) products
in Zarr format and representing them using analysis ready data models.

After installing `xarray-eopf`, you can open EOPF products with standard xarray functions:

```python
import xarray as xr

dataset = xr.open_dataset(url_or_path, engine="eopf-zarr")
datatree = xr.open_datatree(url_or_path, engine="eopf-zarr")
```

**Modes of operation**

1. Analysis mode (`op_mode="analysis"`): Returns user-friendly, analysis-ready data
   with preprocessing (e.g. band selection, resampling, rectification). This mode
   supports only Sentinel-2 and Sentinel-3 products.
2. Native mode (`op_mode="native"`): Returns a near 1:1 view of the Zarr structure
   with minimal preprocessing.

**🔗 Useful links**

- 🐙 **GitHub:** [EOPF-Sample-Service/xarray-eopf](https://github.com/EOPF-Sample-Service/xarray-eopf)
- 📦 **PyPI:** [xarray-eopf](https://pypi.org/project/xarray-eopf)
- 🐍 **Anaconda:** [xarray-eopf on conda-forge](https://anaconda.org/conda-forge/xarray-eopf)
- 📖 **Documentation:** [xarray-eopf docs](https://eopf-sample-service.github.io/xarray-eopf)
- 📓 **Example notebook:** [Introduction to xarray-eopf plugin](https://eopf-sample-service.github.io/eopf-sample-notebooks/introduction-xarray-eopf-plugin)


### xcube EOPF data store

`xcube-eopf` extends [xcube](https://xcube.readthedocs.io/en/latest) with an
`"eopf-zarr"` data store, enabling the creation of analysis-ready data cubes (ARDC)
from Sentinel products via the [EOPF Sentinel Zarr Samples Service STAC API](https://stac.browser.user.eopf.eodc.eu/?.language=en).

Once installed, you can access EOPF data products through the standard xcube interface
and generate analysis ready data cubes form multiple Sentinel Zarr samples. The
workflow for building 3D analysis-ready cubes from Sentinel-2 products involves
the following steps:

1. **Query** products using the [EOPF STAC API](https://stac.browser.user.eopf.eodc.eu/)
   for a given time range and spatial extent.
2. **Retrieve** observations as cloud-optimized Zarr chunks via the
   [xarray-eopf backend](https://eopf-sample-service.github.io/xarray-eopf/).
3. **Mosaic** spatial tiles into single images per timestamp.
4. **Stack** the mosaicked scenes along the temporal axis to form a 3D cube.

> **Note**
> `xcube-eopf` supports Sentinel-2 and Sentinel-3 products (Sentinel-1 coming soon).

**🔗 Useful links**

- 🐙 **GitHub:** [EOPF-Sample-Service/xcube-eopf](https://github.com/EOPF-Sample-Service/xcube-eopf)
- 📦 **PyPI:** [xcube-eopf](https://pypi.org/project/xcube-eopf)
- 🐍 **Anaconda:** [xcube-eopf on conda-forge](https://anaconda.org/conda-forge/xcube-eopf)
- 📖 **Documentation:** [xcube-eopf docs](https://eopf-sample-service.github.io/xcube-eopf)
- 📓 **Example notebook:** [Introduction to xcube-eopf plugin](https://eopf-sample-service.github.io/eopf-sample-notebooks/introduction-xcube-eopf-plugin)


### GDAL EOPF driver

A GDAL driver plugin for reading EOPF (Earth Observation Processing Framework) Zarr datasets.

**Features**

- **QGIS integration** - Works with "Add Raster Layer"
- **Geospatial intelligence** - Automatic CRS and geotransform detection
- **Performance optimized** - Caching, lazy loading, block prefetching
- **Cloud native** - HTTP/HTTPS and virtual file system support
- **Cross-platform** - Windows, macOS, Linux

**🔗 Useful links**

- 🐙 **GitHub:** [EOPF-Sample-Service/GDAL-ZARR-EOPF](https://github.com/EOPF-Sample-Service/GDAL-ZARR-EOPF)
- 📖 **Documentation:** [GDAL EOPF driver docs](https://github.com/EOPF-Sample-Service/GDAL-ZARR-EOPF/blob/main/README.md)
- 📓 **Example notebook:** [Explore EOPF Zarr Sentinel-2 files using GDAL](https://eopf-sample-service.github.io/eopf-sample-notebooks/gdal-explore-zarr)


### Julia EOPF reader

A Julia plugin for reading EOPF (Earth Observation Processing Framework) Zarr datasets.
You can open the EOPF data into a DimTree with Raster leaves for the underlying data. 
This currently gives you a 1:1 representation of the data in the zarr folder.

**🔗 Useful links**

- 🐙 **GitHub:** [JuliaGeo/SentinelDataSource](https://github.com/JuliaGeo/SentinelDataSource.jl)
- 📖 **Documentation:** [JuliaGeo/SentinelDataSource docs](https://github.com/JuliaGeo/SentinelDataSource.jl/blob/main/README.md)
- 📓 **Example notebook:**
