Este proyecto implementa un algoritmo genético (GA) para resolver el Capacitated Vehicle Routing Problem (CVRP). El objetivo es determinar las rutas óptimas para una flota de vehículos con capacidad limitada, que deben atender a un conjunto de clientes con demandas conocidas, minimizando la distancia total recorrida.
El algoritmo genético utilizado en este proyecto simula el proceso de evolución natural mediante operadores como selección, cruza (crossover) y mutación para encontrar soluciones eficientes al CVRP. Se utilizó la biblioteca pyeasyga como base, con modificaciones para implementar selección por torneo y otras mejoras experimentales.

Este enfoque es útil para instancias grandes o realistas donde los métodos exactos como programación lineal entera no escalan adecuadamente.

Técnicas Utilizadas

    Algoritmos Genéticos 

    Selección por torneo

    Representación basada en cromosomas con rutas

    Evaluación de aptitud (fitness) basada en distancia total

    Operadores personalizados de mutación y cruce

    Múltiples ejecuciones con semillas aleatorias para análisis comparativo.

    
  Este proyecto asimismo tiene la intención de comparar el modelamiento matemático con las heurísticas por lo que se encontrarán tanto modelos de GA como de pyomo en los archivos. Para entender la estructura del proyecto se entiende que hay 3 casos, guardados en 3 carpetas dominadas 'Caso1', 'Caso2', 'Caso3'
  Cada una de estas luego cuenta con una división de directorios interna de 'Datos' y 'Modelo'. Se recomienda no modificar la carpeta de 'Casos' ya que es la que contienen los cvs para que corra el modelo. En la carpeta de 'Modelo' se encuentra un notebook llamado 'modelo.ipynb', este contiene toda la información,
  tanto los algoritmos genéticos por caso, como los modelos en pyomo. Para ver los resultados primero debe instalar las dependencias a través de 'pip install -r requirements.txt'. Después de esto corra los Jupyter Notebooks de cada caso de manera secuencial. El informe se encuentra fuera de las carpetas anteriormente mencionadas. 
