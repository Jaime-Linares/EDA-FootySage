# EXPLORATORY DATA ANALYSIS (EDA) - FootySage

Este proyecto realiza un análisis exploratorio de los datos de StatsBomb *Open Data*, enfocado en proporcionar insights sobre el fútbol profesional.

A continuación se detalla el flujo de trabajo y los principales hallazgos:

## 1. Preparación y Carga de Datos
- **Importación de Librerías**: Utilizamos `pandas` para manipulación de datos, `statsbombpy` para acceso a datos de fútbol, y `mplsoccer` para visualizaciones. Finalmente se ha preferido descargar los datos del reporitorio []()
- **Carga de Archivos JSON**: Se cargaron datos de competiciones, partidos, eventos y alineaciones desde una estructura jerárquica de directorios.
- **Optimización de Datos**: Conversión a formatos eficientes como Parquet para mejorar la lectura y escritura de datos.

## 2. Información General de las Competiciones
- Se analizan todas las competiciones disponibles, representando la **distribución de partidos por competición** mediante un gráfico.
- Identificación de competiciones con datos completos, como LaLiga (2015/2016) y la Copa del Mundo (2018).

## 3. Resultados en Partidos y Equipos
- **Impacto de Jugar como Local**:
  - Gráficos de sectores muestran que los equipos locales ganan en un ~50% de los casos.
  - Ejemplos comparativos: FC Barcelona vs. Sevilla FC en LaLiga 2015/2016.
- Los datos confirman que jugar en casa es una ventaja significativa, pero algunos equipos destacan por su rendimiento uniforme en casa y fuera.

## 4. Distribución de Goles por Minuto
- Análisis del momento en el que se marcan más goles durante un partido.
  - Mayoría de goles en los últimos 15 minutos de cada tiempo.
  - Tendencia decreciente en tiempo extra.

## 5. Mapas de Calor de Tiros y Goles
- **Tiros**:
  - La mayoría se concentran dentro del área cercana a la portería.
- **Goles**:
  - Predominan los disparos realizados desde distancias cortas.
- Representación visual con mapas de calor utilizando `mplsoccer`.

## 6. Tipos de Pases y Posiciones
- **Clasificación por Altura**:
  - Pases rasos (~70%) dominan debido a su facilidad técnica.
  - Pases altos y a media altura representan el resto.
- **Análisis de Posiciones**:
  - Defensas realizan más pases, lo que refleja estrategias de mantener la posesión.

## 7. Top 10 Jugadores por Apariciones
- **Por Competición**:
  - Identificación de los jugadores con más partidos jugados en torneos como la Eurocopa 2024.
- **Por Equipo**:
  - Ejemplo: Top 10 jugadores del Sevilla FC en LaLiga 2015/2016.

## Visualizaciones y Herramientas
- Uso de gráficos avanzados para representar distribuciones, probabilidades y mapas espaciales.
- Enfoque en comunicar patrones clave de manera clara y visual.

Este análisis proporciona una base sólida para profundizar en técnicas analíticas avanzadas, identificando tendencias y patrones relevantes en el juego profesional de fútbol.
