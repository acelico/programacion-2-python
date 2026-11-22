# Programación II: Python para el análisis de datos

Materiales de la asignatura **Programación II** del **Grado en Economía y Data Analytics** (UNAV).

La asignatura es una introducción práctica a la programación en **Python** orientada al análisis de datos. Empieza por los fundamentos del lenguaje (tipos de datos, estructuras, control de flujo y funciones) y llega a las librerías principales del ecosistema científico: **NumPy**, **pandas**, **Matplotlib** y **Seaborn**.

Este repositorio recoge el temario y guarda todos los materiales de clase: notebooks de teoría, ejercicios con soluciones y datasets.

---

## Estructura del repositorio

```
programacion-2-python/
├── teoria/                      # Notebooks de teoría (uno por tema)
│   ├── datos/                   # Datasets usados en los notebooks
│   └── imagenes/                # Figuras y esquemas que se ven en los notebooks
├── ejercicios/
│   ├── enunciados/              # Ejercicios para practicar (sin resolver)
│   ├── soluciones/              # Soluciones de los ejercicios
│   └── pandas_exercises_guipsamora/   # Ejercicios extra de pandas (material de terceros)
└── requirements.txt             # Librerías necesarias
```

En la carpeta `teoria/` hay dos versiones de algunos temas:

- `NN_Tema.ipynb`: **versión para el alumno**. Los ejercicios de clase están sin resolver.
- `NN_Tema_SOLUTIONS.ipynb`: **versión resuelta**, con el código de los ejercicios de clase.

Los temas que solo tienen un archivo ya incluyen las soluciones.

> Los notebooks están en inglés, que es el idioma de impartición de la asignatura.

---

## Temario

| # | Tema | Contenidos | Teoría | Ejercicios |
|---|------|-----------|--------|------------|
| 1 | **Hello Python: tipos de datos y variables** | Introducción a Python y Google Colab · programación orientada a objetos · variables · números, strings y booleanos · casting · operadores aritméticos, relacionales y lógicos · prioridad de operadores | [01_Hello_Python](teoria/01_Hello_Python.ipynb) | [enunciado](ejercicios/enunciados/01_Hello_Python_exercises.ipynb) · [solución](ejercicios/soluciones/01_Hello_Python_solutions.ipynb) |
| 2 | **Estructuras de datos: listas, condicionales y bucles `for`** | Listas, tuplas, sets y diccionarios (introducción) · operaciones con listas · bucle `for-in` · ordenación · slicing · copia de listas · list comprehension · condicionales `if / elif / else` | [alumno](teoria/02_Data_structures_Lists.ipynb) · [resuelto](teoria/02_Data_structures_Lists_SOLUTIONS.ipynb) | [enunciado](ejercicios/enunciados/02_Lists_exercises.ipynb) · [solución](ejercicios/soluciones/02_Lists_solutions.ipynb) |
| 3 | **Input, bucles `while` y ficheros CSV** | Entrada de usuario · control de errores con `try-except` · bucle `while` y `break` · menús interactivos · procesar listas con `while` · leer ficheros CSV con el módulo `csv` | [alumno](teoria/03_While_loops_input_csv.ipynb) · [resuelto](teoria/03_While_loops_input_csv_SOLUTIONS.ipynb) | [enunciado](ejercicios/enunciados/03_While_loops_exercises.ipynb) · [solución](ejercicios/soluciones/03_While_loops_solutions.ipynb) |
| 4 | **Diccionarios** | Crear, añadir, modificar y eliminar elementos · métodos `.items()`, `.keys()`, `.values()`, `.get()`, `.setdefault()`, `.pop()`, `.update()` · bucles sobre diccionarios · diccionarios anidados | [alumno](teoria/04_Dictionaries.ipynb) · [resuelto](teoria/04_Dictionaries_SOLUTIONS.ipynb) | [enunciado](ejercicios/enunciados/04_Dictionaries_exercises.ipynb) · [solución](ejercicios/soluciones/04_Dictionaries_solutions.ipynb) |
| 5 | **Funciones** | Definir funciones · `return` · argumentos posicionales y por nombre (keyword) · valores por defecto · número arbitrario de argumentos (`*args`, `**kwargs`) | [alumno](teoria/05_Functions.ipynb) · [resuelto](teoria/05_Functions_SOLUTIONS.ipynb) | [enunciado](ejercicios/enunciados/05_Functions_exercises.ipynb) · [solución](ejercicios/soluciones/05_Functions_solutions.ipynb) |
| 6 | **NumPy** | Creación de arrays · matrices y tensores · inicialización de arrays · slicing · búsqueda de elementos · funciones matemáticas y estadísticas · lectura de CSV con NumPy | [alumno](teoria/06_NumPy.ipynb) · [resuelto](teoria/06_NumPy_SOLUTIONS.ipynb) | [enunciado](ejercicios/enunciados/06_NumPy_exercises.ipynb) · [solución](ejercicios/soluciones/06_NumPy_solutions.ipynb) |
| 7.1 | **pandas (I): Series y DataFrames** | Series y DataFrames · leer CSV (rutas absolutas y relativas) · seleccionar con `.loc` / `.iloc` · añadir y eliminar filas y columnas · `.astype()` · ordenar y rankear · filtrar (`.isin()`, `.between()`, …) · duplicados · valores ausentes · joins | [alumno](teoria/07a_Pandas_I.ipynb) · [resuelto](teoria/07a_Pandas_I_SOLUTIONS.ipynb) | [enunciado](ejercicios/enunciados/07_Pandas_exercises.ipynb) · [solución](ejercicios/soluciones/07_Pandas_solutions.ipynb) |
| 7.2 | **pandas (II): índices, `apply` y `groupby`** | `.set_index()` / `.reset_index()` · renombrar índices y columnas · `.apply()` · `.copy()` · agrupación split-apply-combine con `.groupby()` y `.agg()` | [07b_Pandas_II](teoria/07b_Pandas_II.ipynb) | |
| 7.3 | **pandas (III): reestructurar datos** | `.melt()` · MultiIndex · `.transpose()` · `.swaplevel()` · `.pivot()` · `.stack()` / `.unstack()` · `.pivot_table()` | [07c_Pandas_III](teoria/07c_Pandas_III.ipynb) | |
| 8.1 | **Visualización con Matplotlib** | Figuras y ejes · subplots · tipos de gráficos · cómo elegir el gráfico adecuado (pregunta, audiencia, gráficos exploratorios y explicativos, estética frente a precisión) | [alumno](teoria/08a_Visualization_Matplotlib.ipynb) · [resuelto](teoria/08a_Visualization_Matplotlib_SOLUTIONS.ipynb) | |
| 8.2 | **Visualización con Seaborn** | Sintaxis de Seaborn · gráficos de dispersión, líneas, barras, histogramas, boxplots, densidad y violín · pair plots y facet plots · heatmaps | [08b_Visualization_Seaborn](teoria/08b_Visualization_Seaborn.ipynb) | |

### Ejercicios adicionales de pandas

La carpeta [`ejercicios/pandas_exercises_guipsamora`](ejercicios/pandas_exercises_guipsamora) contiene la colección **pandas_exercises** de Guilherme Samora ([repositorio original](https://github.com/guipsamora/pandas_exercises), licencia BSD-3-Clause). Sirve para practicar pandas con datos reales: exploración, filtrado, agrupación, `apply`, merges, estadística, visualización, series temporales e indexación. Cada ejercicio tiene una versión sin resolver y otra con las soluciones.

---

## Datasets

Los datasets de los notebooks de teoría están en [`teoria/datos/`](teoria/datos):

| Archivo | Se usa en |
|---------|-----------|
| `nba.csv`, `worldstats.csv` | pandas (I) |
| `billionaires.csv`, `movies.csv` | pandas (II) |
| `foods.csv`, `HDI.csv` | pandas (III) |
| `tips.csv` | Visualización con Seaborn |
| `CASchools.csv` | Ejercicios de pandas |
| `HousePrices.csv`, `iris.csv`, `NBA-playerlist.csv`, `PPR-2015.csv`, `UN98.csv` | Ejemplos y práctica adicional |

---

## Cómo trabajar con los materiales

### Opción 1: Google Colab (recomendada)

Los notebooks están preparados para **Google Colab**:

1. Sube la carpeta del repositorio (o los notebooks y la carpeta `datos/`) a tu Google Drive.
2. Abre el notebook con Google Colab.
3. Ejecuta la celda que monta Google Drive (`drive.mount(...)`) y ajusta la ruta a la carpeta donde hayas guardado los datos.

### Opción 2: en local (Jupyter / VS Code)

```bash
git clone <url-del-repositorio>
cd programacion-2-python
python -m venv .venv
# Windows:  .venv\Scripts\activate
# macOS/Linux:  source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

En local, **salta las celdas de Google Colab** (`from google.colab import drive`, `drive.mount(...)`) y carga los datos con rutas relativas, por ejemplo `pd.read_csv("datos/nba.csv")` desde la carpeta `teoria/`.

---

## Bibliografía y recursos

- McKinney, W. (2017). *Python for Data Analysis: Data Wrangling with Pandas, NumPy, and IPython* (2nd ed.). O'Reilly Media.
- Matthes, E. (2019). *Python Crash Course: A Hands-On, Project-Based Introduction to Programming* (2nd ed.). No Starch Press.
- Sweigart, A. (2019). *Automate the Boring Stuff with Python: Practical Programming for Total Beginners* (2nd ed.). No Starch Press.
- Lubanovic, B. (2019). *Introducing Python: Modern Computing in Simple Packages* (2nd ed.). O'Reilly Media.
- Documentación oficial: [Python](https://docs.python.org/3/) · [NumPy](https://numpy.org/doc/stable/) · [pandas](https://pandas.pydata.org/docs/) · [Matplotlib](https://matplotlib.org/stable/) · [Seaborn](https://seaborn.pydata.org/)
