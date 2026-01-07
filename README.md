# LADE_Evolutionary_Project
Optimización evolutiva multiobjetivo de la asignación de pedidos en servicios de entrega de última milla usando NSGA-II y el dataset LaDe.
## 📌 Descripción del problema
La entrega de última milla constituye una de las etapas más complejas y costosas de la logística moderna.
En este proyecto se aborda el problema de asignar pedidos a repartidores de forma eficiente, considerando
objetivos conflictivos como el tiempo total de entrega, la distancia recorrida y el balance de carga entre
repartidores.

## ⚙️ Metodología
Se implementa un enfoque de **Computación Evolutiva multiobjetivo** basado en el algoritmo **NSGA-II**,
formulando el problema con tres funciones objetivo:

- **f1 (Makespan):** tiempo máximo de finalización entre repartidores.
- **f2 (Distancia total):** distancia total recorrida por el sistema.
- **f3 (Desbalance):** diferencia entre el máximo y mínimo número de pedidos asignados.

El algoritmo genera un frente de Pareto y se selecciona una **solución compromiso** para su análisis práctico.

## 📂 Contenido del repositorio
- `proyComputacionEvol.ipynb`: Implementación del modelo evolutivo, análisis de convergencia,
  estudio de sensibilidad y comparación con una heurística básica.
- `README.md`: Descripción general del proyecto.
- `.gitignore`: Exclusión de datos y archivos temporales.

## 🛠️ Requisitos

El proyecto fue desarrollado y probado con las siguientes versiones de librerías:

- Python 3.8+
- datasets==2.21.0
- huggingface_hub==0.24.6
- pyarrow
- pandas==2.2.2
- fsspec==2024.6.1
- pymoo
- numpy
- matplotlib

## ▶️ Ejecución

El proyecto se ejecuta a través de un notebook Jupyter.

```bash
jupyter notebook proyComputacionEvol.ipynb
