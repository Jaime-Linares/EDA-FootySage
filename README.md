# EXPLORATORY DATA ANALYSIS (EDA) - FootySage


<div style="display: flex; align-items: center;">
  <div style="flex: 1; margin-right: 10px;">
    Este proyecto realiza un análisis exploratorio de los datos de StatsBomb <em>Open Data</em>, enfocado en proporcionar insights sobre el fútbol profesional.
    <p>A continuación se detalla el flujo de trabajo y los principales hallazgos:</p>
  </div>
  <div style="flex-shrink: 0;">
    <img src="https://i0.wp.com/lamediainglesa.com/wp-content/uploads/2020/01/statsbomb_la_media_inglesa.jpg?fit=1000%2C523&ssl=1" alt="StatsBomb Logo" width="200">
  </div>
</div>


## Preparación y Carga de Datos
- **Importación de Librerías**: Utilizamos `pandas` para manipulación de datos, `statsbombpy` para acceso a datos de fútbol, y `mplsoccer` para visualizaciones. Finalmente, se ha preferido descargar los datos del reporitorio [https://github.com/statsbomb/open-data](https://github.com/statsbomb/open-data) antes que usar la API en varios análisis. Únicamente se ha usado la API para representar la importancia de los datos 360.
    - **Carga de Archivos JSON**: Los datos ya mencionado arriba del repositorio de *Open Data*. Se cargaron datos de competiciones, partidos, eventos y alineaciones desde una estructura jerárquica de directorios.
- **Optimización de Datos**: Conversión a formatos eficientes como Parquet para mejorar el tiempo en la lectura de datos.


## Información General de las Competiciones
- Se analizan todas las competiciones disponibles, representando la **distribución de partidos por competición** mediante un gráfico.
- Identificación de competiciones con datos completos, como LaLiga (2015/2016) y la Copa del Mundo (2018).


## Resultados en Partidos y Equipos
- **Impacto de Jugar como Local**:
  - Gráficos de sectores muestran que los equipos locales ganan en un ~50% de los casos.
  - Ejemplos comparativos: FC Barcelona vs. Sevilla FC en LaLiga 2015/2016.
- Los datos confirman que jugar en casa es una ventaja significativa, pero algunos equipos destacan por su rendimiento uniforme en casa y fuera.


## Distribución de Goles por Minuto
- Análisis del momento en el que se marcan más goles durante un partido.
  - La mayoría de goles se centra en la mitad del partido aunque es una distribución bastante uniforme.
  - Tendencia decreciente en tiempo extra.


## Mapas de Calor de Tiros y Goles
- **Tiros**:
  - La mayoría se concentran dentro del área cercana a la portería.
- **Goles**:
  - Predominan los disparos realizados desde distancias cortas.
- Representación visual con mapas de calor utilizando `mplsoccer` y creando un campo de fútbol a mano.


## Tipos de Pases y Posiciones
- **Clasificación por Altura**:
  - Pases rasos (~70%) dominan debido a su facilidad técnica.
  - Pases altos y a media altura representan el resto.
- **Análisis de Posiciones**:
  - Defensas realizan más pases, lo que refleja estrategias de mantener la posesión.


## Top 10 Jugadores por Apariciones
- **Por Competición**:
  - Identificación de los jugadores con más partidos jugados en torneos como la Eurocopa 2024.
- **Por Equipo**:
  - Ejemplo: Top 10 jugadores del Sevilla FC en LaLiga 2015/2016.


## Visualización datos 360
- Para visualizar la importancia de los datos 360 hemos representado un ejemplo en un partido (Argentina-Países Bajos, cuartos de final de la Copa del Mundo masculina 2022). El ejemplo es la asistencia de Messi en el primer gol de Argentina en el partido. Gracias a estos datos podemos obtener información mucho más valiosa.


## Visualizaciones y Herramientas
- Uso de gráficos avanzados para representar distribuciones, probabilidades y mapas espaciales.
- Enfoque en comunicar patrones clave de manera clara y visual.


Este análisis proporciona una base sólida para profundizar en técnicas analíticas avanzadas, identificando tendencias y patrones relevantes en el juego profesional de fútbol.
