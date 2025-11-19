# 🌃 Airbnb NYC Data Analysis & Business Intelligence Dashboard 🌃

## ◽️Project Overview

This project involved developing a comprehensive Business Intelligence solution using Power BI to analyze public Airbnb listing data for New York City. The primary goal was to conduct an in-depth Exploratory Data Analysis (EDA) focused on the relationships between listing price, geographical location, property availability, and guest popularity (review volume). This work demonstrates ability in data modeling, advanced DAX scripting, and translating complex metrics into actionable visualizations.

## ◽️Business Question & Hypothesis

- Hypothesis: Listings located in highly touristic zones (e.g., Manhattan) and classified as "Entire Home/Apt" types are more expensive and show higher annual availability compared to listings in less touristic areas or those classified as "Shared Rooms."

## ◽️Key Technologies & Skills

- Platform: Power BI
- Modeling Language: DAX (Data Analysis Expressions)
- Data Preparation: Power Query (M Language)
- Concepts: Data Modeling (Schema creation, relationship management), Advanced Metrics Calculation, Data Visualization, Exploratory Data Analysis (EDA).

## ◽️Data Modeling and DAX Implementation

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

## ◽️Dashboard Structure (5 Pages)

The final dashboard is organized into 5 pages to guide the user through the analysis:

- Home: Informative landing page with navigation buttons and project details.
- Glosario (Glossary): Definitions of key metrics and concepts.
- Ubicación (Location): Visual analysis of pricing and listing density by geographical zone (e.g., Map visualization color-coded by average price: Red=Highest, Green=Lowest).
- Disponibilidad y Popularidad (Availability & Popularity): Examines the relationship between listing availability, review volume, and average price (e.g., Bar charts comparing price vs. availability ranges).
- Tipo Airbnb (Listing Type): Focuses on the price distribution and availability stratified by the type of listing (Private Room, Entire Home/Apt, etc.).

## 📊Key Findings & Insights

The analysis yielded actionable results that both confirmed and challenged the initial hypothesis:

- 📌Price and Location Confirmation: The analysis confirmed that listings in highly touristic zones (e.g., Manhattan) and those classified as "Entire Home/Apt" command the highest average prices. This finding reinforces the premium pricing strategy for exclusive properties in high-demand areas.
- 📌Availability Insight: Listings located in touristic zones demonstrated higher overall annual availability, suggesting a more professionalized and investment-oriented approach to hosting in those specific markets.
- 📌Unexpected Popularity vs. Price: Contrary to the initial assumption, the data revealed that listings with the highest total number of reviews typically exhibited a lower average price. This key insight suggests a potential market segment of high-value, competitively-priced properties that are favored by travelers, indicating a strong opportunity for budget-conscious options.

## ◽️Future Work
Future analysis should be expanded to include:

- In-depth exploration of Host Classification distribution.
- Advanced temporal analysis to identify seasonal price fluctuations.
  
# 🏙️ Análisis de Datos de Airbnb NYC y Dashboard de Business Intelligence 🏙️

## ◽️Resumen del Proyecto

Este proyecto consistió en el desarrollo de una solución integral de Business Intelligence (BI) utilizando Power BI para analizar datos públicos de listados de Airbnb en la ciudad de Nueva York. El objetivo principal fue llevar a cabo un Análisis Exploratorio de Datos (EDA) en profundidad, centrado en las relaciones entre el precio del listado, la ubicación geográfica, la disponibilidad de la propiedad y la popularidad entre los huéspedes (volumen de reseñas). Este trabajo demuestra competencia en modelado de datos, scripting avanzado en DAX y traducción de métricas complejas en visualizaciones accionables.

## ◽️Pregunta de Negocio e Hipótesis

Hipótesis: Los listados ubicados en zonas altamente turísticas (por ejemplo, Manhattan) y clasificados como "Entire Home/Apt" (Casa/Apto Completo) son más caros y muestran una mayor disponibilidad anual en comparación con los listados en áreas menos turísticas o aquellos clasificados como "Shared Rooms" (Habitaciones Compartidas).

## ◽️Tecnologías y Habilidades Clave

- Plataforma: Power BI
- Lenguaje de Modelado: DAX (Data Analysis Expressions)
- Preparación de Datos: Power Query (Lenguaje M)
- Conceptos: Modelado de Datos (Creación de esquemas, gestión de relaciones), Cálculo de Métricas Avanzadas, Visualización de Datos, Análisis Exploratorio de Datos (EDA).

## ◽️Modelado de Datos e Implementación DAX

La solución requirió una sólida preparación y modelado de datos para respaldar el análisis:

### 1. Fuentes de Datos: Conjunto de datos de listados de Airbnb NYC, complementado con tablas de dimensión personalizadas.
### 2. Tablas Personalizadas (DAX):

- Calendar Table: Creada usando CALENDAR(FIRSTDATE(...), LASTDATE(...)) para establecer una línea temporal para el análisis basado en el tiempo (por ejemplo, reseñas por mes).
- Zone_Barrio Table: Creada usando SUMMARIZE para agregar datos geográficos, incluyendo el precio promedio y el total de listados por vecindario y zona.

### 3. Medidas Calculadas (DAX): Se desarrollaron más de 7 medidas personalizadas para calcular métricas centrales, que incluyen:

- Precio Promedio (Average Price): Calculó el precio promedio excluyendo valores cero y vacíos.
- Disponibilidad Promedio (Average Availability): Calculó la media de disponibilidad anual.
- Promedio Reseñas por Mes (Average Reviews Per Month).

### 4. Columnas Calculadas (DAX): Se crearon columnas personalizadas para segmentar los datos para la visualización:

- Rango_Disponibilidad (Availability Range): Categorizó los listados en 5 rangos (por ejemplo, "0-30 días", "271-365 días").
- Cantidad Reseñas (Review Count Range): Agrupó los listados en 11 rangos basados en el volumen total de reseñas.
- Clasificación Host (Host Classification): Categorizó a los anfitriones según el número de listados que gestionan (por ejemplo, "1-10 listados", "más de 100 listados").

## ◽️Estructura del Dashboard (5 Páginas)

El dashboard final está organizado en páginas lógicas para guiar al usuario a través del análisis:

- Home: Página de inicio informativa con botones de navegación y detalles del proyecto.
- Glosario: Definiciones de métricas y conceptos clave.
- Ubicación: Análisis visual de precios y densidad de listados por zona geográfica (por ejemplo, visualización de mapa codificada por color según el precio promedio: Rojo=Más Alto, Verde=Más Bajo).
- Disponibilidad y Popularidad: Examina la relación entre la disponibilidad de listados, el volumen de reseñas y el precio promedio (por ejemplo, gráficos de barras que comparan el precio con los rangos de disponibilidad).
- Tipo Airbnb: Se centra en la distribución de precios y la disponibilidad estratificada por el tipo de listado (Habitación Privada, Casa/Apto Completo, etc.).

## 📊Hallazgos e Insights Clave

El análisis arrojó resultados accionables que tanto confirmaron como desafiaron la hipótesis inicial:

- 📌Confirmación de Precio y Ubicación: El análisis confirmó que los listados en zonas altamente turísticas (por ejemplo, Manhattan) y aquellos clasificados como "Entire Home/Apt" tienen los precios promedio más altos. Este hallazgo refuerza la estrategia de precios premium para propiedades exclusivas en áreas de alta demanda.
- 📌Insight de Disponibilidad: Los listados ubicados en zonas turísticas demostraron una mayor disponibilidad anual general, lo que sugiere un enfoque de alojamiento más profesionalizado y orientado a la inversión en esos mercados específicos.
- 📌Popularidad Inesperada vs. Precio: Contrariamente a la suposición inicial, los datos revelaron que los listados con el mayor número total de reseñas típicamente exhibieron un precio promedio más bajo. Este insight clave sugiere un posible segmento de mercado de propiedades de alto valor y precio competitivo que son favorecidas por los viajeros, lo que indica una fuerte oportunidad para opciones conscientes del presupuesto.

## ◽️Trabajo Futuro

El análisis futuro debería ampliarse para incluir:

- Exploración en profundidad de la distribución de la Clasificación de Host.
- Análisis temporal avanzado para identificar las fluctuaciones estacionales de precios.
