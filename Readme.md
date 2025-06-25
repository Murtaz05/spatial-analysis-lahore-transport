Population-Based Bus Stop Analysis

This project explores the spatial distribution of bus stops in Lahore with respect to population density, aiming to identify patterns, service coverage, and underserved areas.
📌 Objective

To evaluate whether public transport infrastructure (bus stops) is equitably distributed across population-dense regions and identify areas lacking adequate service.
🗂️ Data Sources

    🚏 Bus Stop Data: Extracted from OpenStreetMap (OSM) via OSMnx.

    🌍 Population Density: 2020 gridded raster data from WorldPop. (https://data.worldpop.org/GIS/Population/Global_2000_2020/2020/PAK/pak_ppp_2020.tif)

    📍 Administrative Boundaries: Lahore boundary shapefile.

🧹 Preprocessing

    Clipped population raster to Lahore boundary.

    Reprojected data to UTM Zone 43N (EPSG:32643) for accurate spatial analysis.

    Masked no-data values and handled missing attributes.

    Linked raster data (population) to bus stops via spatial sampling.

📊 Analyses Performed

    Visual overlay of bus stops on population maps.

    Population served per bus stop estimation.

    Nearest Neighbor Distance analysis.

    Spatial autocorrelation using Moran's I.

    Gini coefficient and Lorenz curve to assess population-service inequality.

📌 Key Findings

    Bus stops are clustered in densely populated urban centers.

    Significant positive spatial autocorrelation indicates clustered service regions.

    A low Gini coefficient (~0.0964) suggests relatively equitable population coverage.

    Identified underserved zones visually through spatial raster analysis.

🔮 Future Work

    Integrate schools and office locations for commuter-focused analysis.

    Extend to multimodal transport access and time-based accessibility studies.

📸 Visuals Included

    Population heatmaps with bus stop overlays.

    Choropleth maps showing population served per stop.

    Plots for nearest neighbor distances, Lorenz curve, and underserved regions.

📜 Acknowledgements

    Bus stop data: OpenStreetMap contributors

    Population data: WorldPop, University of Southampton
    
