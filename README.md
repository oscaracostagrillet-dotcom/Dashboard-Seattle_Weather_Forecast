# Dashboard-Seattle_Weather_Forecast
Este proyecto contiene un análisis de datos climáticos de Seattle utilizando Power BI. Se emplea un dataset histórico con variables como temperatura máxima, temperatura mínima, precipitación, viento y condiciones climáticas (sun, rain, drizzle, fog).  El objetivo es visualizar tendencias y patrones del clima mediante KPIs y gráficos interactivos.

# Dashboard de Clima en Seattle

##  Descripción del Proyecto
Este repositorio contiene un **dashboard en Power BI** que analiza datos históricos del clima en Seattle.  
El conjunto de datos incluye registros diarios con las siguientes variables:
- Temperatura máxima y mínima (°C)
- Precipitación (mm)
- Velocidad del viento (mph)
- Condición climática (sol, lluvia, llovizna, niebla)
- Información de tiempo (día, mes, año)

El objetivo es **explorar tendencias y generar KPIs** que resuman el comportamiento climático de la ciudad.

##  Características del Dashboard

- **Distribución del clima**: gráfico circular con la proporción de días soleados, lluviosos, con niebla y llovizna.  
- **Tendencias de temperatura**: gráfico de barras con el promedio de temperatura máxima y mínima por año.  
- **Análisis de precipitación**: promedio de precipitación agrupado por año y condición climática.  
- **Análisis de viento**: promedio de la velocidad del viento por año y condición climática.  
- **KPIs principales en tarjetas**:
  - Temperatura mínima (°C)  
  - Temperatura máxima (°C)  
  - Total de registros  
  - Precipitación promedio (mm)  
  - Viento promedio (mph)  

## Herramientas y Tecnologías
- **Power BI** para modelado y visualización de datos.  
- **Medidas DAX** utilizadas para KPIs:
  - `Max Temperature = MAX('seattle-weather'[temp_max])`
  - `Min Temperature = MIN('seattle-weather'[temp_min])`
  - `Average Precipitation = AVERAGE('seattle-weather'[precipitation])`
  - `Average Wind = AVERAGE('seattle-weather'[wind])`
  - `Record Count = COUNTROWS('seattle-weather')`
