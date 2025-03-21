# Datasets Overview

## 1. Train Dataset (Train.csv)

This dataset contains historical data on disease outbreaks in hospitals, including the number of outbreaks and associated metadata.

### Columns:

- **ID**: Unique identifier for each record.
- **Total**: Number of disease outbreaks per hospital per month (target variable).
- **Location**: Unique identifier for the hospital location.
- **Category_Health_Facility_UUID**: Unique identifier for the health facility.
- **Disease**: Type of disease (e.g., Dysentery, Typhoid, Diarrhea).
- **Month**: Month of the outbreak (1–12).
- **Year**: Year of the outbreak (2019–2022).
- **Transformed_Latitude**: Latitude of the hospital location (geospatial data).
- **Transformed_Longitude**: Longitude of the hospital location (geospatial data).

### Purpose:

Used to train the model to predict the number of outbreaks (**Total**) based on temporal and spatial features.

---

## 2. Waste Management Dataset (waste_management.csv)

This dataset contains climate data and geospatial coordinates for waste management sites.

### Columns:

- **Year**: Year of the climate data (2019–2023).
- **Month**: Month of the climate data (1–12).

### Climate Variables:

- **10u, 10v**: Wind components (east-west and north-south directions).
- **2d, 2t**: Dew point temperature and air temperature at 2 meters above the surface.
- **tp**: Total precipitation.
- **swvl1, swvl2, swvl3, swvl4**: Volumetric soil water content in different soil layers.
- Many other climate-related variables (e.g., evaporation, runoff, surface temperature).

- **Transformed_Latitude**: Latitude of the waste management site.
- **Transformed_Longitude**: Longitude of the waste management site.
- **Month_Year**: Combined month and year (e.g., "1_2019").
- **lat_lon**: Combined latitude and longitude (e.g., "-8.58518_68.25058").
- **Month_Year_lat_lon**: Combined month, year, latitude, and longitude.

### Purpose:

Provides climate data and geospatial information for waste management sites, which can influence disease outbreaks.

---

## 3. Toilets Dataset (toilets.csv)

This dataset contains climate data and geospatial coordinates for toilet locations.

### Columns:

- **Year**: Year of the climate data (2019–2023).
- **Month**: Month of the climate data (1–12).

### Climate Variables:

- Same as in the **Waste Management** dataset.

- **Transformed_Latitude**: Latitude of the toilet location.
- **Transformed_Longitude**: Longitude of the toilet location.
- **Month_Year**: Combined month and year (e.g., "1_2019").
- **lat_lon**: Combined latitude and longitude (e.g., "-8.61768_68.24536").
- **Month_Year_lat_lon**: Combined month, year, latitude, and longitude.

### Purpose:

Provides climate data and geospatial information for toilet locations, which can influence disease outbreaks.

---

## 4. Water Sources Dataset (water_sources.csv)

This dataset contains climate data and geospatial coordinates for water sources.

### Columns:

- **Year**: Year of the climate data (2019–2023).
- **Month**: Month of the climate data (1–12).

### Climate Variables:

- Same as in the **Waste Management** dataset.

- **Transformed_Latitude**: Latitude of the water source location.
- **Transformed_Longitude**: Longitude of the water source location.
- **Month_Year**: Combined month and year (e.g., "1_2019").
- **lat_lon**: Combined latitude and longitude (e.g., "-8.57424_68.23761").
- **Month_Year_lat_lon**: Combined month, year, latitude, and longitude.

### Purpose:

Provides climate data and geospatial information for water sources, which can influence disease outbreaks.

---

## 5. Test Dataset (Test.csv)

This dataset contains data for 2023, the prediction period.

### Columns:

- **Location**: Unique identifier for the hospital location.
- **Disease**: Type of disease (e.g., Dysentery, Typhoid, Diarrhea).
- **Month**: Month of the outbreak (1–12).
- **Category_Health_Facility_UUID**: Unique identifier for the health facility.
- **Year**: Year of the outbreak (2023).
- **Transformed_Latitude**: Latitude of the hospital location.
- **Transformed_Longitude**: Longitude of the hospital location.
- **ID**: Unique identifier for each record.

### Purpose:

Used to predict the number of outbreaks (**Total**) for 2023. Since you’re not aiming for the competition, you can use this dataset for validation or ignore it.

---

## 6. Sample Submission Dataset (SampleSubmission.csv)

This dataset is a template for competition submissions.

### Columns:

- **ID**: Unique identifier for each record (matches the ID column in the Test dataset).
- **Total**: Placeholder for predicted number of outbreaks (all zeros).

### Purpose:

Not relevant for your project since you’re not participating in the competition.
