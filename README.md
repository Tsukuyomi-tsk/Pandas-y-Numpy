# Introducción a NumPy y Pandas

Ayudantía 1 de Introducción a la Ciencia de Datos (IDS). Un recorrido práctico por un flujo de trabajo típico de análisis de datos: entender por qué NumPy es la base del ecosistema, y luego cargar, explorar, limpiar, consultar y resumir un dataset de ventas con Pandas.

## Qué vas a aprender

- Qué es un *array* de NumPy y por qué la **vectorización** es más rápida que un ciclo `for`.
- Cargar y explorar un `DataFrame` (`head`, `info`, `describe`, `isna`, `value_counts`).
- Detectar y tratar **valores nulos** e **inválidos**, justificando la estrategia elegida.
- Filtrar datos con condiciones simples, combinadas y por fecha.
- Combinar NumPy y Pandas con `np.where` y `np.select`.
- Resumir información con `groupby` y construir rankings (Top-N).

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `script ayudantia 1 (1).ipynb` | Notebook principal con el tutorial completo, resultados incluidos. |
| `dataset ayudantia 1.ipynb` | Notebook que genera el dataset de ejemplo. |
| `ventas_gigantes1.csv` | Dataset de 100.000 ventas (datos sintéticos). |
| `guia rapida Pandas  NumPy (1).txt` | Guía de referencia rápida con los comandos más usados. |

## Estructura del tutorial

1. **NumPy: la base de todo.** Listas vs. arrays, estadísticas básicas, vectorización, comparación de tiempos y por qué NumPy es rápido.
2. **Carga y exploración de datos.** `read_csv`, `info`, `describe`, conteo de nulos, percentiles y `value_counts`.
3. **Limpieza de datos.** Corrección de tipos, valores inválidos y tratamiento de nulos (eliminar o rellenar).
4. **Filtros y consultas.** Máscaras booleanas y condiciones múltiples.
5. **NumPy y Pandas trabajando juntos.** `np.where` y `np.select`.
6. **Agregación y resumen.** `groupby`, rankings y `.agg()`.
7. **Eliminación de columnas.**
8. **Resumen y ejercicios propuestos.**

## El dataset

`ventas_gigantes1.csv` contiene datos **sintéticos**, generados con NumPy: no corresponden a ventas reales.

| Columna | Descripción |
|---|---|
| `fecha` | Fecha de la venta (2015 a 2026). |
| `venta` | Monto de la venta (entre 10 y 500). Incluye ~500 valores nulos a propósito. |
| `id_tienda` | Identificador de la tienda (1 a 49). |
| `ciudad` | Madrid, Paris, Barcelona, Roma o Sevilla. |
| `categoria_producto` | Electrónica, Ropa, Alimentos, Hogar o Juguetes. |

## Cómo ejecutarlo

### Requisitos

- Python 3.10 o superior
- `numpy`, `pandas` y Jupyter

### Instalación

```bash
git clone https://github.com/Tsukuyomi-tsk/Pandas-y-Numpy.git
cd Pandas-y-Numpy
pip install numpy pandas jupyterlab
jupyter lab
```

### Uso

1. Abre `script ayudantia 1 (1).ipynb` y ejecuta las celdas en orden. El CSV ya viene incluido en el repositorio.
2. Opcional: ejecuta `dataset ayudantia 1.ipynb` para regenerar el dataset. Los datos se crean al azar sin semilla, así que los resultados del tutorial (por ejemplo los Top 5) cambiarán respecto a los que se muestran.

## Ejercicios

Al final del notebook principal hay 5 ejercicios propuestos para practicar lo aprendido.


«© 2026 Tsukuyomi-tsk. Todos los derechos reservados. Este material se publica solo para consulta.»
