# Reservoir Sustainable Sediment Tool (RESST)

This repository drives a GitHub Pages site that forwards visitors to the RESST ArcGIS Web Experience Builder application. The URL below redirects to the web app.

https://usace-wrises.github.io/resst


## Purpose

RESST (REservoir Sustainable Sediment Tool) brings together case studies, methods, and ecological/sediment literature related to sustainable sediment release. 

## Core features

- Interactive map of dams, reservoirs, and channel reaches.
- Tabbed tables for Sites, Site-linked Literature, and General Literature.
- Keyword filters backed by controlled vocabularies.
- Selected data panel summarizing site details, linked literature, and NID information when available.
- Top-bar tools for HUC layers, bookmarks, spatial selections, and role-based Add/Modify Data actions.
- One-click exports to CSV or Excel for analysis.

## Data model

- **Sites** hosted feature layer: one record per site with ~13 descriptive fields (e.g., Site Type, Sediment Release, Ecological Concern, Analysis).
- **Literature** hosted feature layer: one record per document with ~17 attributes (e.g., Data Collection, Modeling, Sediment Characteristic/Source, Management, Special Cases).
- Relationships connect literature to sites (Site Literature) or keep documents unlinked (General Literature). Sites use unique IDs and may include NID identifiers.

## Typical workflows

- **Targeted Reservoir Analysis**: search or zoom to a site, review Site Literature, export findings for reporting.
- **Regional (HUC) Screening**: toggle HUC layers, spatially select relevant sites, export the filtered dataset.
- **River-Corridor Compilation**: trace or select along a river, compile associated sites and literature, export consolidated results.
- **Thematic Review**: apply keyword filters (e.g., Gravel, Fish Passage), compare Site-linked vs. General literature, export curated references.