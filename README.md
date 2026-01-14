
---

# Transport Poverty Heatmap (UK)

## Overview

This project explores the **scale and geography of transport poverty in the UK**, with a focus on identifying areas where limited transport access significantly affects vulnerable populations.

To do this, I built an **interactive heatmap** that highlights **transport poverty hotspots**, helping policymakers, planners, and researchers understand where transport provision can play a role in poverty mitigation.

---

## Core Objectives

* Identify areas most affected by transport poverty
* Combine social vulnerability and transport accessibility into a single index
* Visualise transport inequality at a highly granular level
* Highlight priority locations for intervention

---

## Key Metrics

### Transport Poverty Index (TPI)

The **Transport Poverty Index** combines multiple datasets to capture both **vulnerability** and **access constraints**:

* **Income deprivation**

  * Index of Multiple Deprivation (IMD) deciles
* **Population vulnerability**

  * Share of elderly residents
  * Share of residents with long-term disabilities
  * Percentage of households without access to a car
* **Access to essential services**

  * Average travel time to hospitals
  * Average travel time to GP services

Each component contributes to a composite score that reflects the severity of transport poverty in an area.

---

### Bus Frequency Score

To capture the **supply-side** of public transport, I developed a **Bus Frequency Score** using:

* Bus Open Data Service (BODS) datasets
* GTFS route data
* Bus stop locations
* Service frequencies

This score highlights areas where **low bus frequency** is a key driver of transport poverty.

---

## Geographic Unit of Analysis

* Each polygon on the map represents an **LSOA (Lower Layer Super Output Area)**
* LSOAs are among the **smallest statistical areas** in the UK, allowing for highly granular insights
* The colour of each polygon reflects its **Transport Poverty Index score**

---

## How to Read the Map

### Colour Scale

At the bottom of the map, a colour bar shows the **Transport Poverty Index scale**:

* **Light yellow** → lower transport deprivation
* **Orange to deep red** → increasing levels of transport poverty

This allows for quick comparison of transport challenges across neighbourhoods.

---

### Interactive Features

* **Hover over an LSOA** to see:

  * LSOA code
  * Neighbourhood name
  * Local authority
  * Exact Transport Poverty Index score

* **Black dots** mark the **Top 10 transport poverty hotspots in Lancashire**

  * Hovering reveals the hotspot rank, local authority, and LSOA name
  * Clicking opens a popup with the precise Transport Poverty Index value

---

## Map Styling & Navigation

* **Thick black boundary lines** show local authority borders
* **Large, clear labels** identify each local authority
* The map remains readable as you zoom in and out, making exploration intuitive

---

## Data Sources

The analysis combines official UK government and census datasets to ensure accuracy and consistency:

1. **Journey Time Statistics (JTS)** – GOV.UK

   * Provides average travel times to key services such as hospitals and GP surgeries
   * Source: [https://www.gov.uk/government/statistical-data-sets/journey-time-statistics-data-tables-jts](https://www.gov.uk/government/statistical-data-sets/journey-time-statistics-data-tables-jts)

2. **Age by Single Year (Census 2021)** – Office for National Statistics

   * Used to identify areas with a higher concentration of elderly residents
   * Source: [https://www.ons.gov.uk/datasets/TS007/editions/2021/versions/3](https://www.ons.gov.uk/datasets/TS007/editions/2021/versions/3)

3. **Household Deprivation** – ONS Census Maps

   * Measures multi-dimensional household deprivation
   * Source: [https://www.ons.gov.uk/census/maps/choropleth/population/household-deprivation/hh-deprivation/household-is-deprived-in-three-dimensions](https://www.ons.gov.uk/census/maps/choropleth/population/household-deprivation/hh-deprivation/household-is-deprived-in-three-dimensions)

4. **Disability (Age-Standardised Proportions)** – Office for National Statistics

   * Captures the proportion of residents with long-term disabilities
   * Source: [https://www.ons.gov.uk/datasets/TS038ASP/editions/2021/versions/2](https://www.ons.gov.uk/datasets/TS038ASP/editions/2021/versions/2)

5. **Car and Van Availability** – ONS Census Maps

   * Identifies households without access to a car or van
   * Source: [https://www.ons.gov.uk/census/maps/choropleth/housing/number-of-cars-or-vans/number-of-cars-3a/no-cars-or-vans-in-household](https://www.ons.gov.uk/census/maps/choropleth/housing/number-of-cars-or-vans/number-of-cars-3a/no-cars-or-vans-in-household)

6. **English Indices of Deprivation (IMD) 2019** – Open Data Communities

   * Used to capture income and multiple deprivation at a local level
   * Source: [https://imd-by-geo.opendatacommunities.org/imd/2019/decile](https://imd-by-geo.opendatacommunities.org/imd/2019/decile)

---

## Why This Matters

Transport poverty limits access to **healthcare, employment, education, and social participation**. By combining social vulnerability with transport availability, this project provides a **data-driven tool** to:

* Support evidence-based transport planning
* Identify priority areas for investment
* Inform policy discussions around transport equity

---

