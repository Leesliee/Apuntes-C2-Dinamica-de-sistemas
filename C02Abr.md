# Modelamiento de sistemas mecánicos 2
### Nestor Alexander Avila Rojas, Leslie Stephania Rodriguez Marín
## 1. Introducción
## 2. Sistemas Rotacionales
Los sistemas rotacionales son otro tipo de sistemas mecanicos solo que en este caso lo que varia es la fuerza aplicada ya que es un movimiento circular que nos genera un torque,estos sistemas se analizan usando las leyes del movimiento rotacional, que son parecidas a las del movimiento traslacional pero en términos angulares.

![image](https://github.com/user-attachments/assets/9e5ba5dd-1701-4749-8064-39ca76fd514d)

Para el anaisis de estos sistemas usaremos leyes comparables al movimiento lineal tales como la fuerza de rosamiento donde el angulo $\varphi$ es el angulo de torcion.
$$F_r = k*\varphi$$

Tambien tendremos la fuerza de friccion donde la $\frac{\mathrm{d}\varphi }{\mathrm{d} t}$ es la velocidad angular del sistema
$$F_{f}=b*\frac{\mathrm{d}\varphi }{\mathrm{d} t}$$
y por ultimo el torque donde la constante j es el momento de inercia del sistema 

$$T=j*\frac{\partial \varphi ^2 }{\partial t^2}$$

Deigual forma como se venia trabajando para los demas sistemas este tambien lo anamizaremos por medio de un diagrama de cuerpo libre el cual nos quedara de la siguiente forma ya con las fuerzas dibujadas para asi poder generar la funcion correspondiente.

💡**Ejemplo:**
![image](https://github.com/user-attachments/assets/5180bf33-115c-42fb-9293-3210f8cc7aa8)

Una vez con esto podremos hacer la funcion teniendo que $\sum T=J*\alpha$ para ello tendremos que:

$$T-F_{R}-F_{F}=j*\alpha$$
Remplazando tendriamos que la funcion no quedaria de la siguiente forma.

$$T(t)-K\theta (t)-B\frac{\partial \theta(t)}{\partial t}=J\frac{\partial^2\theta (t) }{\partial t^2}$$

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
