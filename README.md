Este proyecto implementa un algoritmo genético (GA) para resolver el Capacitated Vehicle Routing Problem (CVRP). El objetivo es determinar las rutas óptimas para una flota de vehículos con capacidad limitada, que deben atender a un conjunto de clientes con demandas conocidas, minimizando la distancia total recorrida.

El algoritmo genético utilizado en este proyecto simula el proceso de evolución natural mediante operadores como selección, cruza (crossover) y mutación para encontrar soluciones eficientes al CVRP. Se utilizó la biblioteca `pyeasyga` como base, con modificaciones para implementar `selección por torneo` y otras mejoras experimentales.

Este enfoque es útil para instancias grandes o realistas donde los métodos exactos como programación lineal entera no escalan adecuadamente.

## Técnicas Utilizadas

- Algoritmos Genéticos  
- `Selección por torneo`  
- `Representación basada en cromosomas con rutas`  
- `Evaluación de aptitud (fitness) basada en distancia total`  
- `Operadores personalizados de mutación y cruce`  
- `Múltiples ejecuciones con semillas aleatorias para análisis comparativo`

---

Este proyecto asimismo tiene la intención de comparar el modelamiento matemático con las heurísticas, por lo que se encontrarán tanto modelos de GA como de Pyomo en los archivos.

Para entender la estructura del proyecto se considera que hay 3 casos, guardados en 3 carpetas denominadas `Caso1`, `Caso2`, `Caso3`.

Cada una de estas luego cuenta con una división de directorios interna: `Datos` y `Modelo`.

> Se recomienda **no modificar** la carpeta de `Datos`, ya que contiene los archivos `.csv` necesarios para que corran los modelos.

En la carpeta `Modelo` se encuentra un notebook llamado `modelo.ipynb`, este contiene toda la lógica tanto de los algoritmos genéticos como de los modelos en Pyomo.

## Instrucciones de Ejecución

1. Instalar las dependencias necesarias:
   ```bash
   pip install -r requirements.txt
