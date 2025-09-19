---
title: EOPF Hackathon at BiDS'25
---


# Get ready to hack together!

**Date:** September 30, 2025 | **Time:** 09:00 - 17:00 | **Location:** BiDS25, Riga, Latvia

## 🎯 Hackathon Objectives

Transform how we access and process Copernicus Sentinel data using cloud-native technologies! This hackathon event focuses on:
- Exploring the **EOPF Sentinel Zarr Samples Service** and its diverse datasets;
- Developing new Jupyter notebooks that leverage the existing EOPF Sample datasets;
- Experimenting with **Discrete Global Grid Systems (DGGS)**, particularly HEALPix, starting from EOPF Sample datasets;


### Familiarize Yourself:

**New to EOPF?** No problem! Make sure to attend the EOPF Sample Service - Getting Started with Zarr (Sep 29, 01:30 PM - 05:00 PM, Room 103).

- **Start with EOPF 101**: [https://eopf-toolkit.github.io/eopf-101/](https://eopf-toolkit.github.io/eopf-101/) - Essential introduction to the EOPF ecosystem
- Browse available datasets in the STAC catalog (11 different Sentinel collections!)
- Review example notebooks: [EOPF Sample Notebooks](https://eopf-sample-service.github.io/eopf-sample-notebooks/)
- Check out the GitHub repository: [https://github.com/EOPF-Sample-Service/eopf-sample-notebooks](https://github.com/EOPF-Sample-Service/eopf-sample-notebooks)

---

## 🚀 Pre-Hackathon Setup (Complete Before 09:00)

### Essential Registration Steps:
1. **Register for Copernicus Data Space Ecosystem**: [https://dataspace.copernicus.eu](https://dataspace.copernicus.eu)
2. **Access JupyterHub Environment**: [https://jupyterhub.user.eopf.eodc.eu/hub](https://jupyterhub.user.eopf.eodc.eu/hub)
3. **Explore the STAC Browser**: [https://stac.browser.user.eopf.eodc.eu](https://stac.browser.user.eopf.eodc.eu/?language=en)

![](https://zarr.eopf.copernicus.eu/wp-content/uploads/2025/06/image-3.png)

---

## 📅 Detailed Agenda

### 🌅 Morning Session (09:00 - 12:30)

#### 09:00 - 09:30: Welcome & Team Formation
- **Welcome & Introductions** (15 min)
- **Quick Overview**: EOPF ecosystem and Zarr Samples Service capabilities
- **New to EOPF?** Quick reference to [EOPF 101](https://eopf-toolkit.github.io/eopf-101/) for foundational concepts
- **Team Formation**: Based on interests and proposed projects (see [Project Ideas](#project-ideas) below)

#### 09:30 - 10:30: Data Exploration Sprint
- **Hands-on exploration** of the STAC browser
- **Discover available datasets**:
  - Sentinel-1 (GRD, SLC, OCN)
  - Sentinel-2 (Level-1C, Level-2A) 
  - Sentinel-3 OLCI & SLSTR products
- **Identify data** for your project ideas and agree on the use case you would like to work on.

#### 10:30 - 10:45: ☕ Coffee Break

#### 10:45 - 12:30: Project Kickoff
- **Finalize team projects** and register them as GitHub issues
- **Download** the official notebook template: [template.ipynb](https://github.com/EOPF-Sample-Service/eopf-sample-notebooks/blob/main/notebooks/template/template.ipynb)
- Review contribution guidelines (see [Contribution Guidelines below](#contribution-guidelines))
- **Begin coding**: Start with existing examples and adapt to your use case
- **Technical support** available from EOPF team

### 🍽️ 12:30 - 13:30: Lunch Break

### 🌞 Afternoon Session (13:30 - 17:00)

#### 13:30 - 15:30: Deep Development
- **Intensive coding session**
- **Experiment with**:
  - Multi-source data fusion
  - DGGS/HEALPix implementations
  - Advanced chunking strategies
  - Zarr optimization techniques
- **Collaborative problem-solving**

#### 15:30 - 15:45: ☕ Coffee Break

#### 15:45 - 16:30: Project Presentations
- **5-minute team presentations** of developed notebooks
- **Demo your solutions** and key findings
- **Community feedback** and discussion

#### 16:30 - 17:00: Wrap-up & Next Steps
- **Reflection on achievements**
- **Discussion of future development**
- **Community notebook competition** introduction
- **Closing remarks**

---

## 💡 Project Ideas & Team Formation

### How to Participate:

1. **Browse Existing Challenges**: Check our [GitHub Issues](https://github.com/EOPF-Sample-Service/eopf-sample-notebooks/issues) for predefined problems
2. **Propose New Ideas**: Create a new issue describing your project concept
3. **Join a Team**: Comment on issues you're interested in contributing to

### 🎯 Suggested Project Themes:

#### **Multi-Mission Data Fusion**
- Combine Sentinel-1 SAR with Sentinel-2 optical data for enhanced land cover mapping
- Integrate Sentinel-3 ocean products with meteorological data

#### **DGGS Applications**
- Implement HEALPix gridding for global climate monitoring
- Develop DGGS-based data aggregation workflows

#### **Performance Optimization**
- Optimize chunking strategies for different use cases
- Benchmark Zarr vs. traditional formats

#### **Novel Applications**
- Time-series analysis across multiple Sentinel missions
- Machine learning pipelines using cloud-native data
- Interactive visualization dashboards

#### **Metadata & Standards**
- Explore Parquet for metadata storage
- Contribute to GeoZarr and CF-conventions discussions

### 🤝 Team Formation Process:

**Before the hackathon:**
1. Create or comment on [GitHub issues](https://github.com/EOPF-Sample-Service/eopf-sample-notebooks/issues) with your interests
2. Use issue labels: `hackathon-2025`, `team-wanted`, `dggs`, `multi-mission`, etc.

**During the hackathon:**
1. Teams of 2-4 people work best
2. Mix of skills encouraged (data scientists, developers, domain experts)
3. One designated team lead for coordination

---

## 🛠️ Technical Resources

### Available Tools & Libraries:
- **Data Access**: STAC, xarray, Dask
- **Processing**: EOPF toolkit, Zarr v3
- **Visualization**: Matplotlib, Plotly, Folium
- **Languages**: Python, Julia
- **Grid Systems**: HEALPix, DGGS implementations
- **Templates**: [Official Jupyter notebook template](https://github.com/EOPF-Sample-Service/eopf-sample-notebooks/blob/main/notebooks/template/template.ipynb) (required for all submissions)

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

## 📋 Project Registration

### Create Your Project Issue:

Use this template when creating a new GitHub issue:

```markdown
**Project Title**: [Your innovative project name]

**Team Members**: [@github-username1, @github-username2, ...]

**Objective**: [Brief description of what you want to achieve]

**Data Sources**: [Which Sentinel missions/products you'll use]

**Technical Approach**: [Tools, methods, or algorithms you plan to explore]

**Expected Outcome**: [Jupyter notebook, visualization, analysis results, etc.]

**Skills Needed**: [What expertise would be helpful for your team]

**Labels**: hackathon-2025, [add relevant tags: dggs, multi-mission, performance, etc.]
```

### Join Existing Projects:

Comment on existing issues with:
- Your background and skills
- How you'd like to contribute
- Your GitHub username for team coordination

---

## 🏆 What Success Looks Like

By the end of the day, each team should have:
- **A working Jupyter notebook** following the provided template
- **Template compliance** with all required metadata and documentation sections
- **Clear documentation** of your approach and findings
- **Identified next steps** for further development
- **Contributions** to the EOPF community knowledge base

### Bonus Achievements:
- **Novel use of DGGS/HEALPix** for EO applications
- **Performance improvements** or optimization insights
- **Cross-mission data fusion** techniques
- **Reproducible workflows** others can build upon

---

## 🔄 After the Hackathon

### Stay Connected:

Join ongoing discussions and join the [EOPF Community Support Platform on Discourse](https://discourse.eopf.copernicus.eu)

---

**Ready to hack? Let's build the future of cloud-native Earth Observation together! 🌍🛰️**

*Questions? Contact the organizing team or join our Slack workspace for real-time support.*
