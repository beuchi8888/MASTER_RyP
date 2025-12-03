# MASTER_RyP

## Sistemas de Control Difuso con scikit-fuzzy

Este repositorio contiene implementaciones de sistemas de control difuso (Fuzzy Logic Control Systems) utilizando la librería scikit-fuzzy en Python. 
El notebook demuestra dos ejemplos principales: un sistema de propinas (PARTE1) y un sistema de protección de batería (PARTE2).

# Contenido
Como se ha comentado, el notebook está dividido en dos partes principales:

Sistema de Propinas (Fuzzy Tipping System): Un ejemplo clásico que calcula la propina ideal basándose en la calidad de la comida y el servicio.
Sistema de Protección de Batería (Fuzzy Battery Protection System): Un sistema más complejo que decide la acción de protección de una batería (standby, recirculación, calentamiento) en función de la temperatura, el estado de carga (SoC) y el estado de la red eléctrica (Sgrid).

# Características
Definición de antecedentes y consecuentes con funciones de pertenencia automáticas y personalizadas.
Creación de reglas difusas para modelar el conocimiento experto.
Simulación de sistemas de control difuso para obtener salidas basadas en entradas.
Visualización de funciones de membresía y el grafo del sistema de control.

# Librerias utilizadas
Python
scikit-fuzzy
numpy
matplotlib
networkx (para la visualización de grafos)

# Instalación
Para ejecutar este notebook, necesitarás instalar las siguientes librerías de Python:

pip install scikit-fuzzy==0.5.0 numpy matplotlib networkx
# Uso
Clona este repositorio:
git clone https://github.com/tu_usuario/tu_repositorio.git
cd tu_repositorio
Abre el notebook (nombre_del_notebook.ipynb) en Google Colab o Jupyter Notebook.
Ejecuta las celdas en orden. Asegúrate de instalar las dependencias como se describe en la sección de instalación.
Explora los ejemplos para entender cómo funcionan los sistemas de control difuso.

# Ejemplo de Tipping System (Propinas)
El sistema de propinas toma como entrada la calidad del servicio y la calidad de la comida, y produce una propina recomendada.

# Ejemplo de Battery Protection System (Protección de Batería)
Este sistema evalúa la temperatura ambiente para poder así proteger la batería. Y estudia si esta se puede poner en funcionamiento según la temperatura ambiente, su estado de carga (SoC) y si la red eléctrica tiene demanda o excedente, para determinar la acción de protección adecuada (ej. standby, recirculation, heating). 
Se prueban diferentes escenarios para demostrar el comportamiento del sistema.

# Estructura del Código

Definición de Variables: Creación de Antecedentes (entradas) y Consecuentes (salidas).
Funciones de pertenencia: Asignación de funciones de pertenencia (ej. trimf, trapmf) a las variables.
Reglas Difusas: Creación de ctrl.Rule combinando las entradas y salidas.
Sistema de Control: Creación de ctrl.ControlSystem con las reglas.
Simulación: Uso de ctrl.ControlSystemSimulation para calcular la salida.
Visualización: Gráficos de funciones de pertenencia y el grafo del sistema.
