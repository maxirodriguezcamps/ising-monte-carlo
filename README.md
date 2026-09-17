Simulación Monte Carlo del modelo de Ising
Trabajo grupal de la materia Mecánica Estadística (FCEyN, UBA, 2025). Proyecto colaborativo realizado en equipo de 5 integrantes.

Objetivo
Simular el modelo de Ising bidimensional mediante el algoritmo de Metropolis y estimar la temperatura crítica del sistema en el límite termodinámico, comparando red cuadrada y red hexagonal.

Metodología
Implementación del algoritmo de Metropolis, optimizada con numba (@njit) para permitir simulaciones de cientos de miles de pasos de Monte Carlo en tiempos razonables.
Estudio de la termalización del sistema y del fenómeno de critical slowing down cerca de la temperatura crítica.
Simulaciones para múltiples tamaños de red (L = 10 hasta L = 100), midiendo magnetización y energía por sitio en función de la temperatura.
Escaleo de tamaño finito (finite-size scaling): ajuste con curve_fit y propagación de errores para extrapolar la temperatura crítica en el límite L → ∞.
Resultados
Se obtuvo una estimación de la temperatura crítica con incertidumbre del orden de 10⁻⁴, tanto para la red cuadrada como para la hexagonal, consistente con los valores conocidos de la literatura.

Nota sobre autoría
Este fue un trabajo genuinamente colaborativo entre los 5 integrantes del equipo (diseño del algoritmo, implementación, y análisis se trabajaron en conjunto), por lo que no se atribuyen secciones específicas del código a cada integrante.

Herramientas
Python · NumPy · Numba (@njit) · SciPy (curve_fit) · Matplotlib
