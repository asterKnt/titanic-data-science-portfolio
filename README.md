# Titanic Data Science Portfolio

Repositorio académico y didáctico dedicado al análisis integral, modelado predictivo y aprendizaje no supervisado sobre el conjunto de datos del RMS Titanic.

## Estructura del Proyecto

```text
titanic-data-science-portfolio/
├── data/                               # Conjuntos de datos en formatos brutos y procesados
│   ├── titanic5.csv
│   ├── titanic5.xlsx
│   ├── titanic5.xlsx - Titanic5_all.csv
│   ├── titanic.sav
│   └── titanic.sdd
├── proyecto-1/                         # Fase 1: Exploración, limpieza y modelos base
│   ├── P1-Aguilar.ipynb                # Cuaderno de análisis del Proyecto 1
│   ├── peer_critique.md                # Evaluación y retroalimentación entre pares
│   ├── Proyecto 1 - Enunciado.pdf      # Guía y lineamientos de la entrega 1
│   └── 12. Lab Proyecto 1 (1 de septiembre).ipynb
├── proyecto-2/                         # Fase 2: Ensamble supervisado y clustering
│   ├── P2-Aguilar.ipynb                # Cuaderno de modelado y análisis no supervisado
│   ├── Proyecto 2 - Enunciado.pdf      # Requerimientos y rúbrica oficial
│   └── 22. Lab Proyecto 2 (8 de octubre).ipynb
├── pyproject.toml                      # Definición del proyecto y dependencias (PEP 621)
├── uv.lock                             # Bloqueo determinista de dependencias
├── .gitignore                          # Exclusiones de Git
└── README.md                           # Documentación general
```

## Contenido de las Entregas

### Proyecto 1: Análisis Exploratorio y Modelado Base
- Análisis descriptivo e inferencial sobre características sociodemográficas y de viaje.
- Tratamiento de datos faltantes e ingeniería de características inicial.
- Modelos de referencia (Dummy y KNN) y evaluación inicial.
- *Etiqueta de lanzamiento:* `v1.0-proyecto1`

### Proyecto 2: Predecir y Agrupar
- **Parte Predictiva:** Pipeline sin fugas (`ColumnTransformer`), modelo tonto, modelo simple y ensamble (Random Forest / Gradient Boosting) con búsqueda razonada de hiperparámetros.
- **Parte Sin Respuestas:** Aprendizaje no supervisado (clustering o reducción de dimensionalidad) con interpretación conceptual de cada grupo.
- **Conexión Analítica:** Caracterización de los segmentos o grupos donde el modelo predictivo comete más errores.

## Reproducibilidad del Entorno

Este proyecto utiliza [`uv`](https://github.com/astral-sh/uv) como gestor de paquetes y entornos de Python.

### Requisitos previos
- Python >= 3.13
- `uv` instalado en el sistema

### Instalación y sincronización del entorno

Para sincronizar el entorno virtual determinista con todas las dependencias:

```bash
uv sync
```

### Ejecución de Jupyter Lab

Para iniciar el entorno interactivo dentro del entorno virtual gestionado:

```bash
uv run jupyter lab
```
