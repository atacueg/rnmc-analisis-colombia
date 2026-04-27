# rnmc-analisis-colombia

Exploracion y analisis del Registro Nacional de Medidas Correctivas (RNMC) para Colombia, periodo 2020-2025. Los notebooks cubren desde la carga y limpieza de datos hasta visualizaciones y analisis estadistico basico.

## Que hay aqui

- Carga y normalizacion del dataset RNMC (CSV ~700MB)
- Analisis por municipio, departamento y tipo de infraccion
- Visualizaciones con matplotlib y seaborn
- Comparativos por año y tendencias generales

## Stack

- Python 3
- Pandas
- Matplotlib / Seaborn
- Jupyter Notebook

## Datos

El dataset original no esta incluido en el repo por el tamaño. Se puede descargar desde el portal de datos abiertos del gobierno colombiano.

## Uso

Clonar el repo, instalar dependencias y correr los notebooks en orden. Los archivos asumen que el CSV esta en la misma carpeta o en `/data`.

```bash
pip install pandas matplotlib seaborn jupyter
jupyter notebook
```
