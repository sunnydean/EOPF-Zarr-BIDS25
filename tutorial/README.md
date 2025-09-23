---
title: EOPF Tutorial at BiDS'25
---


# EOPF Sample Service Getting Started with Zarr

**Date:** September 29, 2025 | **Time:** 1:30 pm - 5:00 pm | **Location:** Room 103, BiDS25, Riga, Latvia

## 🎯 Tutorial Objectives

- **Introduce Cloud-Native Workflows**: Explain the paradigm shift from traditional, file-based workflows to scalable, cloud-native analysis using formats like `zarr` to overcome the challenges of processing large-scale Earth observation data.
- **Data Discovery with STAC**: Provide practical skills in using the EOPF STAC catalog's web interface and programmatic tools (like `pystac-client`) to find and filter Earth observation data efficiently.
- **Discover the newly developed plugins:** Get an overview of the xarray EOPF backend, the xcube EOPF data store, the GDAL EOPF reader, and a Julia EOPF re
- **Build Practical Data Analysis Skills**: Guide participants through a hands-on, end-to-end workflow based in Python libraries such as `xarray` and `zarr` to perform a real-world analysis (e.g., wildfire monitoring), showcasing the integration of STAC and `zarr`.



### Familiarize Yourself:

**New to EOPF?** No problem!

- **Start with EOPF 101**: [https://eopf-toolkit.github.io/eopf-101/](https://eopf-toolkit.github.io/eopf-101/) - Essential introduction to the EOPF ecosystem
- Browse available datasets in the STAC catalog (11 different Sentinel collections!)
- Review example notebooks: [EOPF Sample Notebooks](https://eopf-sample-service.github.io/eopf-sample-notebooks/)
- Check out the GitHub repository: [https://github.com/EOPF-Sample-Service/eopf-sample-notebooks](https://github.com/EOPF-Sample-Service/eopf-sample-notebooks)

---

## 🚀 Pre-Tutorial Setup (Complete Before start)

### Essential Registration Steps:
1. **Register for Copernicus Data Space Ecosystem**: [https://dataspace.copernicus.eu](https://dataspace.copernicus.eu)
2. **Access JupyterHub Environment**: [https://jupyterhub.user.eopf.eodc.eu/hub](https://jupyterhub.user.eopf.eodc.eu/hub)
3. **Explore the STAC Browser**: [https://stac.browser.user.eopf.eodc.eu](https://stac.browser.user.eopf.eodc.eu/?language=en)

![](https://zarr.eopf.copernicus.eu/wp-content/uploads/2025/06/image-3.png)

---

## 📅 Detailed Agenda

#### 13:30-14:00: Introduction

- **About Cloud Optimised Formats**
Overview of cloud-optimised formats, focusing on their role in enabling FAIR data principles.
- **Zarr introduction to Sentinel**
We will delve into the `Zarr` format as applied to Sentinel data.
- **Chunking for Optimisation**
This topic covers the fundamental concept of chunking and its importance in optimising data access.

#### 14:00 - 15:00: Data Discovery

- **STAC EOPF Catalog Exploring**
Guided demo on how to explore the web interface of the [EOPF STAC catalog](https://stac.browser.user.eopf.eodc.eu/?.language=en).
- **Python STAC Access**
Guided walk for generating the connection to the EOPF STAC Catalog Endpoint through Python.

#### 15:00 - 15:30: EOPF Zarr Plugins for easy acess
Overview on the availabe plugins deveolped by [EOPF Sample Service](https://zarr.eopf.copernicus.eu/data-and-tools/#open_source_plugins). 
Short handons demos for each plugin: 
  - [xarray EOPF backend](https://eopf-sample-service.github.io/xarray-eopf/)
  - [xcube EOPF data store](https://eopf-sample-service.github.io/xcube-eopf/)
  - [GDAL EOPF Reader](https://github.com/EOPF-Sample-Service/GDAL-ZARR-EOPF)
  - [Julia Reader](https://github.com/JuliaGeo/SentinelDataSource.jl)


#### 15:30 - 16:30: Wildfire in Sardinia
Guided example of how to integrate Sentinel products into a specific use case.

Support on replicating the workflow with provided case studies.

#### 16:30 - 17:00: Wrap-up & Summary

Key takeaways on how **Zarr** and **STAC** together form a powerful, cloud-native ecosystem that directly supports data-driven decision-making and contributes to the goals of open science and interoperability in the BIDS community.

*Breaks are considered along the event* 😉

## 🛠️ Technical Resources

### Getting Help:
- **EOPF team members** available throughout the day
- **New to EOPF?** Start with [EOPF 101](https://eopf-toolkit.github.io/eopf-101/) for core concepts
- **Slack channel**: #eopf-hackathon (link provided on-site)
- **Documentation**: [EOPF Sample Notebooks](https://eopf-sample-service.github.io/eopf-sample-notebooks/)

### Data Available:
- **Real Copernicus Sentinel data** in Zarr format
- **Global coverage** with recent acquisitions
- **All processing levels** from L1 to L2
- **Optimized chunking** for cloud processing



---

## 🔄 After the Tutorial

### Stay Connected:

Join ongoing discussions and join the [EOPF Community Support Platform on Discourse](https://discourse.eopf.copernicus.eu)


