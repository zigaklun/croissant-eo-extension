# Earth Observation Croissant Extension

**Extending MLCommons Croissant for Earth Observation datasets**

**Version**: v1.0.0

---

##  Purpose

This extension enhances the **MLCommons Croissant** metadata standard with Earth Observation (EO)-specific fields. Its goal is to improve the description, sharing, and discovery of satellite imagery datasets used in machine learning workflows.

---

##  Quick Start

Just add the EO namespace to your Croissant metadata:

```json
{
  "@context": {
    "cr": "https://mlcommons.org/croissant/",
    "eo": "https://zigaklun.github.io/croissant-eo-extension/schema/v1.0.0/"
  },
  "@type": "sc:Dataset",
  "name": "my-eo-dataset",
  "eo:scope": "global",
  "eo:has-task": ["classification", "segmentation"],
  "eo:spatialResolutionInMeters": 10.0,
  "eo:dataSource": ["Sentinel-2"]
}
