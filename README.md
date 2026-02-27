# Predicción de Aprobacion de un Estudiante
1. Importación de librerías Se importan bibliotecas para cálculo numérico (NumPy),
manejo de datos (Pandas), visualización (Matplotlib) y modelado probabilístico (pome-
granate).
2. Definición de distribuciones iniciales Se modelan las probabilidades a priori
de Estudio, Asistencia y Dificultad. Por ejemplo:
P (Estudio = Alto) = 0,6 (1)
Estas representan probabilidades marginales.
3. Tabla de probabilidad condicional Aquí se define:
P (Aprueba | Estudio, Asistencia, Dif icultad) (2)
Cada combinación de variables independientes tiene asociada una probabilidad de
aprobar o no aprobar.
5. Construcción de la red Se crean nodos (State) y se conectan mediante aristas
dirigidas hacia la variable Aprueba. Luego se ejecuta bake() para compilar el modelo.
6. Inferencia Se calcula la probabilidad de aprobar bajo condiciones específicas:
Estudio = Alto, Asistencia = Alta, Dificultad = Dif´ıcil.
El resultado esperado es aproximadamente:
P (Aprueba = S´ı | Alto, Alta, Dif´ıcil) = 0,7(3)
7. Simulación Monte Carlo Se generan 1000 muestras aleatorias del modelo para
estimar probabilidades empíricas usando frecuencias relativas.
