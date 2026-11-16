# Urban Mobility & Economic Productivity Analysis – Sprint 5

Este repositorio contiene el análisis realizado durante el Sprint 5 de TripleTen sobre movilidad urbana y productividad económica en las principales ciudades de América Latina.

El proyecto integra y procesa datos reales de tráfico vehicular (`tomtom_traffic.csv`, con más de 1,004,000 registros horarios) junto con indicadores socioeconómicos (`oecd_city_economy.csv`), abarcando finalmente **15 ciudades principales de 7 países latinoamericanos** durante el año 2024.

## 📂 Contenido del repositorio

- `notebooks/ladb_mobility_economy_analysis.ipynb` S5 ladb_mobility_economy_project.ipynb`
  → Notebook principal con exploración, limpieza de datos, estandarización de esquemas, agregación por ciudad-año, unión (`INNER JOIN`), visualizaciones y resumen ejecutivo.
- `data/ladb_mobility_economy_2024_clean.csv`
  → Dataset final limpio y consolidado listo para análisis posteriores.

## 📘 Cómo reproducir el análisis

1. Abre el notebook principal (`S5 ladb_mobility_economy_project.ipynb`)
2. Ejecuta las celdas en orden
3. El notebook procesa los datasets `tomtom_traffic.csv` y `oecd_city_economy.csv` desde `/datasets/` (o la ruta local correspondiente) y exporta el archivo `ladb_mobility_economy_2024_clean.csv`

## 🧠 Objetivo del análisis

- Estandarizar columnas (`snake_case`) y limpiar formatos numéricos y de fecha en ambos datasets
- Filtrar la información correspondiente al período 2024 y consolidar métricas de tráfico promedio por ciudad
- Integrar indicadores de movilidad y economía mediante un `INNER JOIN`
- Analizar distribuciones, valores atípicos (`outliers`) y patrones entre congestión vehicular (`jams_delay`) y PIB per cápita (`city_gdp_capita`)
- Generar recomendaciones estratégicas respaldadas en datos para priorizar inversiones en infraestructura de transporte en la región (destacando casos como Bogotá y Lima)
