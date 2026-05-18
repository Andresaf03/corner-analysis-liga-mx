# Corner Analysis

Análisis de tiros de esquina en Liga MX usando StatsBomb 360 data (4 temporadas · 2021/22 – 2024/25).

## Objetivo

Convertir \~13 000 tiros de esquina en recomendaciones tácticas accionables para cuerpos técnicos: qué tipo de envío (inswinging / outswinging / corto) maximiza OBV y xG, y cómo varía por equipo y temporada.

## Estructura

```
corner-analysis-liga-mx/
├── data/                  # Datos StatsBomb (no versionados)
│   ├── events.parquet
│   ├── matches.parquet
│   ├── comps.parquet
│   └── lineups.json
├── figures/               # Gráficas generadas por el notebook
├── analysis.ipynb         # Notebook principal
├── requirements.txt       # Dependencias Python
└── README.md
```

## Setup

```bash
pip install -r requirements.txt
jupyter lab analysis.ipynb
```

## Datos

Los archivos en `data/` no están versionados por tamaño.\
Fuente: [StatsBomb Open Data](https://github.com/statsbomb/open-data) / HUDL API proporcionada por ISAC.
