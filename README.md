# Análisis RNMC — Registro Nacional de Medidas Correctivas

> **Nota de confidencialidad** — Este repositorio se publica el 27 de abril de 2026
> exclusivamente como muestra del trabajo desarrollado dentro de una entidad pública.
> El código y los resultados corresponden a análisis reales sobre datos institucionales
> que hasta esta fecha no habían salido del entorno interno. Se comparte con fines
> de portafolio para proceso de selección y será removido o puesto en privado una
> vez concluya dicho proceso.

Exploración y análisis del Registro Nacional de Medidas Correctivas (RNMC)
para Colombia, período 2020-2025. Desarrollado en el contexto de análisis
de seguridad ciudadana y gestión de convivencia. Los notebooks cubren desde
la carga y limpieza del dataset hasta visualizaciones y análisis comparativo
por año, municipio y tipo de infracción.

## Qué hay aquí

| Notebook | Descripción |
|---|---|
| `limpiando2023.ipynb` | Carga, limpieza y normalización del dataset 2023 |
| `revision2024.ipynb` | Análisis comparativo y visualizaciones 2024 |
| `revision2025.ipynb` | Análisis y tendencias del período 2025 |

## Stack

- Python 3
- Pandas
- Matplotlib / Seaborn
- Jupyter Notebook

## Datos

El dataset original (~700 MB en CSV) no está incluido en el repo.
Procede del portal de datos abiertos del gobierno colombiano y de
registros internos de la entidad. Los notebooks asumen que el CSV
está en la misma carpeta o en `/data`.

## Uso

```bash
pip install pandas matplotlib seaborn jupyter
jupyter notebook
```

Correr los notebooks en orden: limpieza 2023 primero, luego revisión
2024 y 2025. Cada uno es independiente pero el flujo de normalización
de columnas es consistente entre los tres.

## Contexto

El RNMC registra las medidas correctivas impuestas por policía nacional
y otras autoridades. Con ~700 MB de datos por año, el trabajo central
fue normalizar columnas inconsistentes entre versiones anuales del CSV,
identificar municipios con mayor volumen de registros y cruzar variables
como tipo de infracción, hora, y localidad para detectar patrones.
