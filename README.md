# Análisis Estadístico del MVP de la NBA (Temporada 2022–2023)

## Descripción del Proyecto

Este proyecto realiza un análisis exploratorio y comparativo de datos de jugadores de la NBA durante la temporada 2022–2023 con el objetivo de evaluar, desde una perspectiva estadística, quién tenía el caso más sólido para ganar el premio **MVP (Most Valuable Player)**.

Para ello se analizan y comparan las estadísticas de tres de los principales candidatos al MVP de esa temporada:

- Nikola Jokić (Denver Nuggets)
- Joel Embiid (Philadelphia 76ers)
- Giannis Antetokounmpo (Milwaukee Bucks)

El análisis combina estadísticas de temporada completa con datos partido a partido, utilizando herramientas de **Python para ciencia de datos**, con el fin de explorar:

- producción ofensiva
- eficiencia de tiro
- creación de juego
- impacto general en el equipo
- consistencia a lo largo de la temporada

El objetivo es mostrar cómo el **análisis de datos puede utilizarse para estudiar el rendimiento deportivo y apoyar debates tradicionales del deporte con evidencia cuantitativa**.

---

# Autores

- Felipe Tamaki  
- Matías Goldschmidt  
- Lucas Binello  

---

# Datos Utilizados

El proyecto utiliza cuatro archivos de datos.

## Dataset general de jugadores

`2023_nba_player_stats.csv`

Contiene estadísticas agregadas de todos los jugadores de la NBA durante la temporada 2022–2023, incluyendo:

- puntos por partido
- porcentajes de tiro (FG%, 3P%, FT%)
- rebotes
- asistencias
- robos
- bloqueos
- minutos jugados
- pérdidas
- +/-  

Este dataset se utiliza para:

- filtrar jugadores con rendimiento de nivel MVP
- normalizar estadísticas
- comparar métricas clave entre jugadores

---

## Datos partido a partido de candidatos MVP

Archivos utilizados:

- `Giannis Antetokounmpo.xlsx`
- `Joel Embiid.xlsx`
- `Nikola Jokic.xlsx`

Estos datasets contienen estadísticas de cada partido jugado durante la temporada por cada uno de los candidatos.

Permiten analizar:

- consistencia de rendimiento
- distribución de puntos por partido
- variabilidad en desempeño
- impacto partido a partido

---

# Metodología

El análisis fue desarrollado en **Python utilizando Jupyter Notebook**.

Principales librerías utilizadas:

- pandas
- numpy
- matplotlib
- seaborn
- adjustText
- openpyxl

---

## 1. Limpieza y preparación de datos

Se realizó un proceso de limpieza que incluyó:

- conversión de variables a formato numérico
- manejo de valores faltantes
- selección de estadísticas relevantes
- estandarización de columnas

Esto permitió construir un dataset consistente para el análisis.

---

## 2. Filtrado de jugadores relevantes

Para identificar jugadores comparables a nivel MVP se aplicaron filtros como:

- mínimo de partidos jugados
- minutos promedio elevados
- producción ofensiva significativa

Esto permite evitar comparaciones con jugadores con bajo tiempo de juego.

---

## 3. Normalización de estadísticas (Per 36 minutos)

Para comparar jugadores con diferentes cargas de minutos, las estadísticas fueron ajustadas a **producción por 36 minutos**.

Esto permite una comparación más justa entre jugadores con distinto volumen de minutos en cancha.

---

## 4. Análisis por posición

Los jugadores fueron categorizados según su posición:

- PG
- SG
- SF
- PF
- C

Esto ayuda a contextualizar el rendimiento estadístico según el rol dentro del juego.

---

## 5. Visualización de datos

Se generaron gráficos utilizando **Matplotlib y Seaborn** para analizar visualmente:

- producción ofensiva
- eficiencia de tiro
- rebotes
- asistencias
- consistencia de rendimiento

Las visualizaciones permiten identificar **patrones y diferencias entre los candidatos al MVP**.

---

# Principales Insights

## Producción ofensiva

**Joel Embiid** destaca como el jugador con mayor capacidad anotadora entre los tres candidatos.

Su volumen de puntos por partido refleja su rol como principal arma ofensiva de Philadelphia.

---

## Creación de juego

**Nikola Jokić** sobresale claramente en playmaking.

Sus números de asistencias muestran un perfil único para un pivot, funcionando como generador principal de juego para Denver.

Este estilo de juego lo convierte en uno de los centros más versátiles de la NBA moderna.

---

## Impacto integral

**Giannis Antetokounmpo** presenta el perfil más equilibrado y completo.

Destaca simultáneamente en:

- anotación
- rebotes
- impacto defensivo

Esto refleja su estilo de juego dominante en ambos lados de la cancha.

---

## Consistencia a lo largo de la temporada

El análisis partido a partido muestra que:

- **Jokić mantiene una producción extremadamente consistente**
- **Embiid presenta picos ofensivos más altos**
- **Giannis combina anotación con fuerte presencia en rebotes**

---

## Eficiencia

Las métricas de eficiencia indican que:

- **Jokić logra una eficiencia ofensiva excepcional**
- **Embiid combina volumen y eficiencia en anotación**
- **Giannis mantiene alto volumen ofensivo aunque con menor eficiencia relativa debido a su estilo de ataque**

---

# Conclusión

El análisis muestra que los tres jugadores presentan **perfiles estadísticos distintos para el premio MVP**.

| Jugador | Fortaleza Principal |
|--------|---------------------|
| Joel Embiid | Dominio anotador |
| Nikola Jokić | Playmaking y eficiencia |
| Giannis Antetokounmpo | Impacto completo en ambos lados de la cancha |

Esto demuestra que el debate del MVP no depende únicamente de una métrica, sino de cómo se valoran distintos tipos de impacto dentro del juego.

El proyecto ilustra cómo la **ciencia de datos puede aportar herramientas cuantitativas para analizar debates tradicionales del deporte**.

---

# 🚀 Cómo usar este repositorio

## 1️⃣ Clonar el repositorio
Descarga el proyecto desde GitHub:

git clone https://github.com/FelipeTamaki/Analisis-Estadistico-del-MVP-de-la-NBA-Temporada-2022-2023.git

Luego entra en la carpeta del proyecto:

cd Analisis-Estadistico-del-MVP-de-la-NBA-Temporada-2022-2023

---

## 2️⃣ Instalar dependencias
Instala las librerías necesarias para ejecutar el análisis:

pip install pandas numpy matplotlib seaborn openpyxl adjustText jupyter

---

## 3️⃣ Ejecutar el análisis

Abre el notebook de Jupyter:

jupyter notebook Analisis.ipynb

Luego ejecuta todas las celdas para reproducir el análisis y generar los gráficos.

---

# Posibles Extensiones

Este proyecto podría ampliarse incorporando:

- métricas avanzadas (PER, BPM, Win Shares)
- impacto en victorias del equipo
- análisis defensivo más profundo
- modelos de machine learning para predicción de MVP

---

# Aplicación

Este proyecto muestra cómo aplicar herramientas de **data science y análisis estadístico en el contexto del deporte**, integrando:

- análisis exploratorio de datos
- visualización estadística
- comparación cuantitativa de rendimiento
