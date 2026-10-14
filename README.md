# Awesome-Podcast-To-Video-Repurposing

## Top Precision Agricultural Fertilizer Orchestration Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Variable Rate Application, Nutrient Zoning & Satellite-Based Prescription Mapping*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Precision Agricultural Fertilizer Orchestration**. These tools combine satellite imagery, soil sampling, yield history, and agronomic models to generate variable rate application (VRA) prescription maps that tell equipment exactly how much fertilizer to apply in each zone of a field.

**Examples** include Climate FieldView, Farmers Edge, Taranis, CropX, Agworld, Semios, Yara Atfarm, John Deere Operations Center, FarmQA, and Sentera (the category leaders).

**Open-source emphasis**: This section is expanded with every major active project for self-hosting, custom prescription generation, and transparent nutrient modeling — ideal for agronomists prioritizing data sovereignty, developers building precision ag pipelines, and cooperatives avoiding per-acre platform fees.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Yara Atfarm](https://www.yara.co.nz/crop-nutrition/farmers-toolbox/atfarm2/)**  
  Free precision nitrogen management platform using satellite imagery analyzed with Yara N-Sensor technology. Supports variable-rate nitrogen application even without a VRA spreader — the mobile app provides GPS-based recommendations that farmers can apply manually by adjusting flow rate or speed. Includes N-Tester integration for ground-truthing crop nitrogen status and smartphone photo analysis for oilseed rape and cereal nitrogen uptake estimation [citation:7].

- **[OneSoil Nitrogen](https://blog.onesoil.ai/en/onesoil-nitrogen-app)**  
  Free web application that calculates nitrogen variable rates and creates task files for onboard computers. Uses machine learning and multispectral satellite imagery to allocate three vegetation zones (yellow = most need, pale green = average, green = best). Compatible with Trimble, Ag Leader, Amazone, Raven, John Deere, and Topcon controllers. Zones are defined by NDVI and rates can be adjusted based on farmer knowledge [citation:19].

- **[Climate FieldView](https://climate.com/)**  
  Bayer's digital farming platform with variable rate seeding and fertilizer prescription tools, imagery, and field data management.

- **[Farmers Edge](https://www.farmersedge.ca/)**  
  Precision agriculture platform with soil sampling, satellite imagery, and variable rate prescription generation.

- **[Taranis](https://www.taranis.com/)**  
  AI-powered crop monitoring with high-resolution aerial imagery and agronomic insights for nutrient management.

- **[CropX](https://www.cropx.com/)**  
  Soil intelligence platform with sensor-based moisture and nutrient monitoring for irrigation and fertilization decisions.

- **[Agworld](https://www.agworld.com/)**  
  Collaborative farm management platform with precision ag tools and prescription management.

- **[Semios](https://semios.com/)**  
  Precision agriculture platform with IoT sensors, pest monitoring, and variable rate application support.

- **[John Deere Operations Center](https://www.deere.com/)**  
  Equipment telematics and farm management platform with prescription file support and variable rate application.

- **[Sentera](https://sentera.com/)**  
  Drone and satellite imagery analytics for crop health, nutrient status, and prescription mapping.

## Open-Source GitHub Projects

- **[YieldStack](https://gitlab.com/Roxanne_Ardary/yieldstack)**  
  **Open-source (AGPL-3.0+) agricultural intelligence platform** for optimizing water, nitrogen, crop performance, and soil sustainability. Features AI-based nitrogen application recommendations with split application timing, fertilizer efficiency modeling, nitrogen leaching and runoff risk prediction, and **variable-rate fertilizer prescription maps**. Supports soil test integration, crop-stage nutrient demand modeling, cost optimization, and ROI tracking. Modular architecture with pluggable ML models (XGBoost, Random Forest, LightGBM, neural networks), GIS and remote sensing layer (NDVI, thermal, multispectral), and sensor/IoT ingestion. Self-hosted, cloud, or hybrid deployment [citation:6].

- **[GeoFIS](https://github.com/GeoFIS/GeoFIS)**  
  **Open-source decision-support tool for precision agriculture data** developed by INRAE (French National Research Institute for Agriculture). Covers the full process from spatial data to spatial information and decision support. Key capabilities include mapping of spatial variability, evaluation and cross-comparison of site-specific management opportunities across multiple fields, and **delineation of within-field zones for variable-rate applications**. Validated across banana, wheat, and vineyard case studies. Published in Agriculture journal (2018), open access [citation:10].

- **[Operationalizing GIS and ML across Cropping Systems](https://github.com/halilunaziru73-creator/Operationalizing-GIS-and-Machine-Learning-across-Contrasting-Cropping-Systems)**  
  **GIS, remote sensing, and machine learning for precision agriculture** across maize, vineyard, and grape systems. Includes spatial fertility mapping and **variable-rate prescription for a maize field in Coimbra (16.85 ha)**. Methodology: yield correlated strongly with deep soil-water content (r = 0.972) and potassium oxide (r = 0.751); quadratic yield-fertiliser regression (R² = 0.995) supported a variable-rate NPK/liming programme that **cut total lime demand by 2.69 t versus uniform application**. Repository includes Python notebooks, data, and variable-rate prescription map outputs [citation:5].

- **[Agri-Vision System](https://github.com/maknoonisar/agricultural-AI)**  
  **AI-powered agricultural intelligence platform** with interactive MapBox visualizations, crop health diagnostics using computer vision, yield forecasting, and **resource optimization recommendations for irrigation and fertilization**. Integrates drone and satellite imagery with live weather data. Features NDVI mapping, disease detection, and downloadable reports. Python/Streamlit stack with PostgreSQL option [citation:9].

- **[EasySpectra](https://github.com/matheusfreitasbit/EasySpectra)**  
  **Open-source multispectral imagery processing library** for precision agriculture. Provides tools for processing drone and satellite multispectral data including NDVI and other vegetation indices used in nutrient zoning and prescription generation. Archived on Zenodo for long-term accessibility and reproducibility [citation:17].

- **[AgroSat](https://www.agrosat.it/)**  
  **Free web-based decision support system** for precision agriculture developed by Italian National Research Council (IBE-CNR). Uses open satellite imagery (Sentinel-2, MODIS) and climatic data to generate **variable-rate nitrogen fertilization maps** and productive potential maps. Implements two fertilization management modes — compensation and differentiation — based on intra-field variability and crop growth dynamics. Case study on winter wheat demonstrated stabilized within-field yield and crop vigor through zonal N prescription maps [citation:4][citation:15].

- **[SATIVUM](https://eu-cap-network.ec.europa.eu/projects/practice-abstracts/tech-1-sativum-technology-provider-instituto-tecnologico-agrario-de_en)**  
  **Free web application** from Instituto Tecnológico Agrario de Castilla y León (ITACyL) providing data-driven insights for plot management. Features crop monitoring via Sentinel-2 satellite images, **fertilization module**, pest alert calendars, and **tools for zoning plots to enable Variable Rate Application (VRA)**. Includes Farm Digital Notebook and soil information. Open APIs for third-party integration [citation:3].

- **[Agropixel Synapse](https://zenodo.org/records/22801967)**  
  **Open-source geospatial decision-support platform** for precision agriculture, integrating UAV, remote sensing, GIS, and analytical workflows for agricultural monitoring and prescription generation [citation:13].

### Additional Strong Open-Source Options

- **QGIS** — Free, open-source, cross-platform Geographic Information System widely used for precision agriculture data processing, zone delineation, and prescription map generation [citation:2].
- **FarmBot Genesis** — Fully open-source farming platform automating seeding, watering, and weeding with customizable gantry system. Suitable for educational and research applications [citation:2].
- **IoT Agrointelligence LoRaWAN Node** — Open-source LoRaWAN node for agricultural monitoring with multiple ADC channels and solar energy management, for building custom soil and crop sensor networks [citation:2].
- **V62 VRA Prescription Engine** — Open-source governed VRA prescription engine supporting fertilizer, lime, seed, and irrigation product types. Features productivity zones, soil sampling plans, lab results integration, and a **readiness gate that blocks prescription generation without sufficient data** (no zones → blocked; no lab results without explicit allow_estimated → blocked). Prescriptions require agronomist review before export [citation:1].
- **LiteFarm** — Free, open-source farm management platform being extended for variable rate irrigation prescription systems in collaboration with Farming Smarter and University of British Columbia [citation:14].

**Frameworks for building custom systems**: Combine **YieldStack** for nitrogen optimization and prescription mapping, **GeoFIS** for within-field zone delineation, **Operationalizing GIS and ML** for fertility zoning workflows, **Agri-Vision** for crop health monitoring, and **EasySpectra** for multispectral imagery processing to build a complete self-hosted precision fertilizer orchestration stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Precision fertilizer orchestration tools must comply with agricultural regulations, environmental protection laws (nutrient runoff), and equipment safety standards. **VRA prescription maps must be validated against multiple data layers before application** — single-year yield maps or single-source imagery are insufficient and can systematically over-apply or under-apply inputs [citation:8].
- Self-hosted open-source solutions require proper satellite data access, soil sampling integration, and agronomic validation before field deployment.

---

**Made for agronomists, precision agriculture specialists, farm managers, and developers building nutrient management platforms.**  
Let's make precision fertilizer orchestration more open, data-driven, and environmentally responsible.
