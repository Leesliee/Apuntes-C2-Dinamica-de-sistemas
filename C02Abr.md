# Modelamiento de sistemas mecánicos 2
### Nestor Alexander Avila Rojas, Leslie Stephania Rodriguez Marín
## 1. Introducción
En el estudio de los sistemas dinámicos, el modelamiento de sistemas rotacionales desempeña un papel fundamental, ya que permite representar y analizar el comportamiento de mecanismos presentes en una amplia variedad de aplicaciones industriales y tecnológicas. 

Durante esta clase se abordó la importancia de identificar elementos presentes en otro tipo de sistemas mecánicos. También se exploraron métodos alternativos de modelado a partir del análisis de trabajo, energía y potencia. Si bien este enfoque puede ser útil para sistemas simples, su aplicación en sistemas complejos resulta limitada debido a la dificultad para gestionar múltiples variables e interacciones.

Finalmente, se introdujeron conceptos clave relacionados con mecanismos de transmisión como engranajes, palancas y bandas, los cuales permiten transformar y transferir el movimiento en un sistema mecánico. Estos elementos, al igual que las fuerzas involucradas, deben ser cuidadosamente considerados en el proceso de modelado para lograr representaciones precisas y útiles del comportamiento dinámico del sistema.

## 2. Sistemas Rotacionales
>🔑Los sistemas rotacionales son otro tipo de sistemas mecánicos, sólo que en este caso lo que varia es la fuerza aplicada ya que es un movimiento circular que nos genera un torque, estos sistemas se analizan usando las leyes del movimiento rotacional, que tienen cierta analogía con respecto a las del movimiento traslacional.

![image](https://github.com/user-attachments/assets/9e5ba5dd-1701-4749-8064-39ca76fd514d)

Figura 1: Movimiento rotacional

Para el análisis de estos sistemas usaremos leyes comparables al movimiento lineal tales como la fuerza de rozamiento donde el ángulo $\varphi$ es el ángulo de torsión.

$$F_R = k*\varphi$$

Tambien tendremos la fuerza de fricción donde la $\frac{\mathrm{d}\varphi }{\mathrm{d} t}$ es la velocidad angular del sistema.

$$F_{f}=b*\frac{\mathrm{d}\varphi }{\mathrm{d} t}$$

Y por último el torque donde la constante $J$ es el momento de inercia del sistema: 

$$T=J*\frac{\partial \varphi ^2 }{\partial t^2}$$



De igual manera como se venía trabajando para los demás sistemas mecánicos este también lo anamizaremos por medio de un diagrama de cuerpo libre el cual nos quedara de la siguiente forma, ya con las fuerzas dibujadas para así generar la función correspondiente que modela el sistema.

### 💡Ejemplo 1:
Encuentre el modelo matemático de la figura teniendo en cuenta que la entrada es  T(t) y la salida es $\Theta (t)$:

![Figura 1](Imagenesf/sistema2.png)
Figura 1: Ejemplo 1

![Figura 1](Imagenesf/dcle3.png)
Figura 2: DCL carga

Una vez con esto podremos determinar la función teniendo en cuenta que $\sum T=J*\Theta$:

$$T-F_{R}-F_{F}=J*\Theta$$
Remplazando, se obtendría la función que modela el sistema:

$$T(t)-k\Theta (t)-b\dot{\Theta(t)}=J\ddot{\Theta (t) }$$

## 2.1 Conversion Movimiento Translacional-Rotacional
Para estos sistemas veremos el proceso mediante el cual se convierte un desplazamiento lineal en un desplazamiento angular o a la inversa todo esto mediante un sistema mecanico el cual puede ser desglosado en varias partes las mas comunes son:
### Poleas y correas
Transmiten movimiento rotacional a uno lineal o al contrario a través de una banda o varias bandas.
### Cremallera y piñón
Convierte el movimiento rotacional de un engranaje en movimiento lineal.
### Tornillos sin fin 
Convierte la rotación de un tornillo dada ya sea por un motor o un giro manual en movimiento lineal.

💡**Ejemplo:** Tenemos el siguiente sistema combinando el cual es un motor enganchado a una polea para a si poder mover la caja.

![image](https://github.com/user-attachments/assets/80f14a08-aa53-4ce4-a5bb-5852d78c2775)

Teniendo esto como base pasaremos al diagrama de cuerpo libre obteniendo a si las fuerzas positivas y negativas del sistema.

![image](https://github.com/user-attachments/assets/c8dc6e37-972a-4a1a-bf99-5ecab4da4df7)

Con esto pasaremos a resolver la $\sum T=J*\alpha$ teniendo asi:

$$T_{m}-T_{1}-T_{F}=J_{m}*\alpha$$

Donde remplazando las incognitas por sus funciones obtendremos el siguiente resultado, sabiendo que para $T_{1}$ el momento de inercia es $mr^{^2}$.

$$T_{m}-mr^{^2}\frac{\partial^2\theta  }{\partial t^2}-B\frac{\partial \theta }{\partial t}=J_{m}\frac{\partial^2\theta  }{\partial t^2}$$

Teniendo en cuenta que el $\theta = y/r$ remplazamos en la ecuacion

$$T_{m}-mr\frac{\partial^2 y}{\partial t^2}-\frac{B}{r}\frac{\partial y }{\partial t}=\frac{J_{m}}{r}\frac{\partial^2 y}{\partial t^2}$$
