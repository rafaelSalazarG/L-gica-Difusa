# Lógica-Difusa
Este código implementa un simulador de un sistema de control difuso aplicado a un péndulo invertido montado sobre un carrito. El objetivo es estabilizar el péndulo utilizando lógica difusa para calcular la fuerza necesaria en el carrito. 
1. Parámetros del sistema
Define constantes físicas como la masa del carrito, la masa del péndulo, la longitud del péndulo y la fuerza máxima aplicable.
Utiliza conjuntos difusos (NG, NP, Z, PP, PG) para representar las categorías de los valores de ángulo y velocidad angular del péndulo.
2. Simulación (simulate)
Simula el comportamiento del sistema durante un tiempo t_max con un paso de tiempo delta_t.
Calcula la posición angular (theta) y la velocidad angular (w) del péndulo en cada paso, utilizando la aceleración derivada de la dinámica del sistema.
Grafica la evolución del ángulo del péndulo en función del tiempo.
3. Dinámica del sistema (calcular_aceleracion)
Calcula la aceleración angular del péndulo considerando las fuerzas aplicadas, la gravedad y las propiedades físicas del sistema.
4. Lógica difusa
Funciones de pertenencia (mu, muw): Determinan el grado de pertenencia de un valor (ángulo o velocidad) a un conjunto difuso (e.g., NG, Z, PG).
Reglas difusas (fuerza): Implementan reglas basadas en la lógica difusa para calcular la fuerza aplicada al carrito. Estas reglas combinan las pertenencias de los valores actuales de ángulo y velocidad angular.
5. Visualización
La simulación genera un gráfico que muestra cómo el ángulo del péndulo evoluciona con el tiempo, permitiendo evaluar la efectividad del control.
