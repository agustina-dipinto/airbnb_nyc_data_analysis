# 🌃 Airbnb NYC Data Analysis & Business Intelligence Dashboard 🌃

## Project Overview

This project involved developing a comprehensive Business Intelligence solution using Power BI to analyze public Airbnb listing data for New York City. The primary goal was to conduct an in-depth Exploratory Data Analysis (EDA) focused on the relationships between listing price, geographical location, property availability, and guest popularity (review volume). This work demonstrates proficiency in data modeling, advanced DAX scripting, and translating complex metrics into actionable visualizations.

## Business Question & Hypothesis

- Hypothesis: Listings located in highly touristic zones (e.g., Manhattan) and classified as "Entire Home/Apt" types are more expensive and show higher annual availability compared to listings in less touristic areas or those classified as "Shared Rooms."

## Key Technologies & Skills

- Platform: Power BI

- Modeling Language: DAX (Data Analysis Expressions)

- Data Preparation: Power Query (M Language)

- Concepts: Data Modeling (Schema creation, relationship management), Advanced Metrics Calculation, Data Visualization, Exploratory Data Analysis (EDA).

## Data Modeling and DAX Implementation

The solution required robust data preparation and modeling to support the analysis:

### 1. Data Sources: Airbnb NYC Listings dataset, supplemented with custom dimension tables.

### 2. Custom Tables (DAX):

- Calendar Table: Created using CALENDAR(FIRSTDATE(...), LASTDATE(...)) to establish a temporal line for time-based analysis (e.g., reviews per month).

- Zone_Barrio Table: Created using SUMMARIZE to aggregate geographical data, including average price and total listings per neighborhood and zone.

### 3. Calculated Measures (DAX): Over 7 custom measures were developed to calculate core metrics, including:

- Precio Promedio (Average Price): Calculated average price excluding zero and blank values.

- Disponibilidad Promedio (Average Availability): Calculated the mean annual availability.

- Promedio Reseñas por Mes (Average Reviews Per Month).

### 4. Calculated Columns (DAX): Custom columns were created to segment the data for visualization:

- Rango_Disponibilidad (Availability Range): Categorized listings into 5 ranges (e.g., "0-30 days," "271-365 days").

- Cantidad Reseñas (Review Count Range): Grouped listings into 11 ranges based on total review volume.

- Clasificación Host (Host Classification): Categorized hosts based on the number of listings they manage (e.g., "1-10 listings," "more than 100 listings").

## Dashboard Structure (5 Pages)

The final dashboard is organized into logical pages to guide the user through the analysis:

- Home: Informative landing page with navigation buttons and project details.

- Glosario (Glossary): Definitions of key metrics and concepts.

- Ubicación (Location): Visual analysis of pricing and listing density by geographical zone (e.g., Map visualization color-coded by average price: Red=Highest, Green=Lowest).

- Disponibilidad y Popularidad (Availability & Popularity): Examines the relationship between listing availability, review volume, and average price (e.g., Bar charts comparing price vs. availability ranges).

- Tipo Airbnb (Listing Type): Focuses on the price distribution and availability stratified by the type of listing (Private Room, Entire Home/Apt, etc.).

## Key Findings & Insights

The analysis yielded actionable results that both confirmed and challenged the initial hypothesis:

- Price and Location Confirmation: The analysis confirmed that listings in highly touristic zones (e.g., Manhattan) and those classified as "Entire Home/Apt" command the highest average prices. This finding reinforces the premium pricing strategy for exclusive properties in high-demand areas.

- Availability Insight: Listings located in touristic zones demonstrated higher overall annual availability, suggesting a more professionalized and investment-oriented approach to hosting in those specific markets.

- Unexpected Popularity vs. Price: Contrary to the initial assumption, the data revealed that listings with the highest total number of reviews typically exhibited a lower average price. This key insight suggests a potential market segment of high-value, competitively-priced properties that are favored by travelers, indicating a strong opportunity for budget-conscious options.

## Future Work

- Future analysis should be expanded to include:

- In-depth exploration of Host Classification distribution.

- Advanced temporal analysis to identify seasonal price fluctuations.
