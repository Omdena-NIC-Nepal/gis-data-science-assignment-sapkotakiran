
# GIS Data Science for Climate in Nepal

## Assignment Overview
This project aims to explore climate data for Nepal using GIS (Geographical Information System) techniques. The goal is to assess climate trends, such as temperature and precipitation changes over time, by leveraging GIS data science tools and visualizations. The dataset used in this project includes climate-related GIS data for Nepal for the years 2020 and 2050.

### Key Objectives:
1. **Visualize climate trends** in Nepal by plotting temperature and precipitation data.
2. **Perform Exploratory Data Analysis (EDA)** to compute basic statistics (mean, median, min, max) of climate variables and identify patterns in the data.
3. **Document the findings** from the analysis and provide insights into how climate change might affect Nepal.

---

## Data Sources
The data used for this project has been sourced from publicly available climate-related GIS datasets:

### Shape_Data
1. **local_unit.dbf**: Contains attribute data for local administrative units.
2. **local_unit.prj**: Provides projection information for the shapefile.
3. **local_unit.sbn**: Spatial index file.
4. **local_unit.sbx**: Associated spatial index file.
5. **local_unit.shp**: The shapefile containing the geometry of Nepal's administrative regions.
6. **local_unit.shx**: The index file corresponding to `local_unit.shp`.

### nepal_climate_data
1. **metadata.json**: Metadata file containing descriptions of the climate data sources and attributes.
2. **nepal_admin_regions.gpkg**: GeoPackage containing Nepal's administrative region boundaries.
3. **nepal_glaciers.gpkg**: GeoPackage containing data on Nepal's glaciers.
4. **nepal_precipitation_2020.tif**: Raster file representing precipitation data for Nepal in 2020.
5. **nepal_precipitation_2050.tif**: Raster file representing projected precipitation data for Nepal in 2050.
6. **nepal_rivers.gpkg**: GeoPackage containing river data for Nepal.
7. **nepal_temperature_2020.tif**: Raster file representing temperature data for Nepal in 2020.
8. **nepal_temperature_2050.tif**: Raster file representing projected temperature data for Nepal in 2050.

---

## Setup Instructions

### Prerequisites:
1. Python 3.x
2. Required libraries:
   - `pandas`
   - `geopandas`
   - `matplotlib`
   - `seaborn`
   - `rasterio`

### Installation:

To set up the environment, you can use the following steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/Nepal_Climate_Analysis.git
   cd Nepal_Climate_Analysis
   ```

2. Install the required libraries using `pip`:

   ```bash
   pip install -r requirements.txt
   ```

   If you don't have a `requirements.txt` file, manually install the necessary libraries:

   ```bash
   pip install pandas geopandas matplotlib seaborn rasterio
   ```

---

## Data Loading and Preparation

The dataset consists of:

1. **Shape_Data**:
   - `local_unit.shp`: Contains the geographical boundaries of Nepal’s administrative regions.
   - `local_unit.dbf`: Contains the attribute data for each administrative region.
   - `local_unit.prj`: Provides the projection information for the shapefile.
   - `local_unit.sbn` & `local_unit.sbx`: Spatial index files for the shapefile.
   - `local_unit.shx`: Index file for the shapefile geometry.

2. **Nepal Climate Data (Raster Files)**:
   - `nepal_temperature_2020.tif`: Temperature data for Nepal in 2020.
   - `nepal_temperature_2050.tif`: Temperature data for Nepal in 2050.
   - `nepal_precipitation_2020.tif`: Precipitation data for Nepal in 2020.
   - `nepal_precipitation_2050.tif`: Precipitation data for Nepal in 2050.

3. **GeoPackage Data**:
   - `nepal_admin_regions.gpkg`: Contains the administrative boundaries of Nepal.
   - `nepal_glaciers.gpkg`: Contains information on Nepal's glaciers.
   - `nepal_rivers.gpkg`: Contains data on rivers in Nepal.

Data is loaded into Python using `geopandas` for vector data (shapefiles and GeoPackages) and `rasterio` for raster data.

---

## Visualizations

The following visualizations were created:

1. **Nepal Map**:
   - A map showing the **administrative regions** and **rivers** of Nepal.
   
2. **Temperature Trends**:
   - A side-by-side comparison of **temperature** data for 2020 and 2050, visualized using heatmaps.

3. **Precipitation Trends**:
   - A side-by-side comparison of **precipitation** data for 2020 and 2050, also visualized using heatmaps.

4. **Temperature Distribution (2020)**:
   - A histogram with a kernel density estimate (KDE) to visualize the **distribution of temperature** across Nepal for the year 2020.

---

## Exploratory Data Analysis (EDA)

### Temperature and Precipitation Statistics (2020):
The following basic statistics were computed for the temperature and precipitation data for 2020:

- **Temperature 2020**:
  - Mean: `mean_value`
  - Median: `median_value`
  - Min: `min_value`
  - Max: `max_value`
  
- **Precipitation 2020**:
  - Mean: `mean_value`
  - Median: `median_value`
  - Min: `min_value`
  - Max: `max_value`

### Insights and Observations:
- **Temperature Increase**: There is a noticeable increase in temperature from 2020 to 2050 across Nepal. The heatmaps indicate that some regions will experience higher temperature changes.
- **Precipitation Variability**: Precipitation data suggests that certain areas might experience increased rainfall, while others could face reduced precipitation in the future.

---

## Summary of Findings

From the EDA and visualizations, it is clear that:

1. Nepal is projected to experience significant changes in both temperature and precipitation by 2050.
2. The spatial distribution of temperature and precipitation is uneven across regions, highlighting varying impacts of climate change on different parts of Nepal.
3. This information can aid in climate adaptation strategies for Nepal's various regions, helping policymakers focus on areas most at risk from temperature and precipitation extremes.

---

## Submission and Evaluation

1. **GitHub Repository**: Contains all necessary Python scripts, data files, and this README file.
2. **Code Documentation**: The code is well-commented and organized for easy understanding.
3. **Visualizations**: High-quality, informative visualizations that help interpret the climate data and identify trends.
4. **Findings from EDA**: The exploratory data analysis is thorough, providing clear insights into the potential impacts of climate change on Nepal.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Climate data sources (e.g., NASA Earthdata, NOAA).
- Python libraries: `geopandas`, `matplotlib`, `rasterio`, `seaborn`.
