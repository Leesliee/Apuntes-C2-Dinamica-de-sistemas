# Modelamiento de sistemas eléctricos e hidráulicos
### Nestor Alexander Avila Rojas, Leslie Stephania Rodriguez Marín
## 1. Introducción
En esta clase de sistemas dinámicos se exploraron dos áreas fundamentales del modelado físico: los amplificadores operacionales no inversores y los sistemas hidráulicos. En el caso de los amplificadores, se analizó cómo modelar su comportamiento dinámico mediante ecuaciones que relacionan la entrada con la salida, destacando la importancia de estos dispositivos en el procesamiento y control de señales dentro de sistemas electrónicos. Se identificaron las condiciones de ideales, así como los elementos que afectan su estabilidad.

Por otro lado, se introdujo el análisis de sistemas hidráulicos, donde se estudia el comportamiento del flujo y nivel de fluidos dentro de tanques.  Ambos enfoques permiten desarrollar una comprensión más amplia de cómo diferentes dominios físicos pueden representarse bajo marcos matemáticos similares, reforzando así la capacidad de análisis y diseño de sistemas dinámicos complejos.
## 2. Amplificador operacional NO inversor
Para determinar el modelamiento de un amplificador operacional no iversor es crucial tener en cuenta sus características:
+La tensión en ambas entradas del amplificador son iguales

+Las corrientes en las entradas del amplificador son nulas

+La impedancia de entrada es muy grande

+La impedancia de salida es muy pequeña (se asume que es 0)

La impedancia de entrada es rande para que el amplificador reciba una señal y toda la magnitud de la señal se quede en el amplificador, y la impedancia de salida es pequeña donde la mínima cantidad de tensión se quede en el amplificador.

El análisis de este modelo es mejor hacerlo por nodos.

![Figura 3](Imagenes/OP1png)

Figura 1: Amplificador operacional

### 💡 Ejemplo 1:

![Figura 3](Imagenes/OP1png)

Figura 2: Ejemplo 1

$$i_1-i_2=0$$

$$\frac{e_o-v_x}{R_2}-\frac{v_x-0}{R_1}=0$$

$$v_x = e_i$$

Reemplazando:

$$e_o = e_i(\frac{1}{R_2}+\frac{1}{R_1})R_2

### 💡 Ejemplo 2:
![Figura 3](Imagenes/OP1png)

Figura 4: Ejemplo 2

$$i_1-i_2-i_3=0$$

$$\frac{e-e'}{R_1}-\frac{e'-e_o}{R_2}-C(\dot{e'}-\dot{e_o})=0$$

$$e'=0$$

Reemplazando:

$$\frac{e}{R_1}+\frac{e_o}{R_2}-C(-\dot{e_o})=0$$

$$\frac{e}{R_1}+\frac{e_o}{R_2}+C(\dot{e_o})=0$$

## 3. Sistemas hidráulicos
>🔑 Un sistema hidráulico es un conjunto de componentes que utiliza un fluido, generalmente aceite o agua, para transmitir energía y generar movimiento o fuerza. Funciona mediante la presión del fluido dentro de tuberías, cilindros o bombas, y es común en maquinaria industrial, frenos y sistemas de control.

En este caso, se analizarán en tanques:




## 4. Conclusiones
Para modelar correctamente un sistema con amplificadores operacionales no inversores, es fundamental comprender sus propiedades eléctricas como la impedancia de entrada y salida, y el comportamiento ideal del amplificador. Estas características determinan la forma en que la señal se amplifica y cómo responde el sistema ante diferentes entradas.

En cuanto a los sistemas hidráulicos, es esencial tener en cuenta factores físicos como la rugosidad de las tuberías, ya que esta genera una resistencia al flujo que afecta directamente al caudal del sistema. Además, para facilitar el análisis y asegurar un comportamiento predecible, se debe asumir que el flujo es laminar, condición bajo la cual las ecuaciones de modelado hidráulico son más estables y aplicables.

## 5. Referencias
Jorge Eduardo Cote Ballesteros. (2024). Sistemas eléctricos, dinámica de sistemas. ETITC

Jorge Eduardo Cote Ballesteros. (2024). Sistemas hidráulicos y térmicos, dinámica de sistemas. ETITC

Ogata, Katsuhiko (1987) : Dinámica de Sistemas, Traducido de la primera edición en inglés de la obra System Dynamics, Prentice Hall Hispanoamericana, S.A., México.


