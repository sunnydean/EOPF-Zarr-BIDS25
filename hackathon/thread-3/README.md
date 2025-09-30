# Bids25 EOPF-Zarr hackathon: RGB Composites/Vegetation indexes/burned area
	
**Goal: reproduce the comfort we had with STAC/COG**

* Simple application using xarray reading one or more Sentinel-2 acquisitions
* Focus on STAC/Zarr metadata to reduce mission knowledge (no need to know `b04` is the red band):

And thus avoid: 

```python
red = dt["measurements/reflectance/r10m"]["b04"].chunk({"x": 512, "y": 512})
green = dt["measurements/reflectance/r10m"]["b03"].chunk({"x": 512, "y": 512})
blue = dt["measurements/reflectance/r10m"]["b02"].chunk({"x": 512, "y": 512})
nir = dt["measurements/reflectance/r10m"]["b08"].chunk({"x": 512, "y": 512})
```

Note: this is a proof of concept, not by any means the solution for the problem

Contributors:

- @fabricebrito
- @simonevaccari
- @pl-marasco
