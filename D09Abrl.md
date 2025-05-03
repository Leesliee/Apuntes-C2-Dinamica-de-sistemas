# Modelamiento de sistemas eléctricos RLC
### Nestor Alexander Avila Rojas, Leslie Stephania Rodriguez Marín
## 1. Introducción
En el estudio de sistemas dinámicos, modelar circuitos eléctricos es fundamental para comprender cómo responden ante diferentes estímulos en el tiempo. Esta clase se centró en el análisis de circuitos utilizando las leyes de Kirchhoff, que permiten establecer las ecuaciones diferenciales que describen el comportamiento dinámico de corrientes y tensiones en el sistema.

A través de la identificación de elementos como resistencias, inductancias y capacitancias, y del reconocimiento de las variables de entrada y salida del circuito, se puede representar matemáticamente su evolución. Este tipo de modelado es esencial para predecir el comportamiento del sistema ante diversas condiciones iniciales y entradas, facilitando el diseño y control de sistemas eléctricos en aplicaciones reales.

Comprender estos principios no solo permite resolver circuitos, sino también visualizar su dinámica como parte integral de un sistema físico, donde la energía se almacena, disipa y transfiere.
## 2. Ciruitor RLC
>🔑 Un circuito RLC es un circuito eléctrico que está formado por resistencias inductancias y capacitancias estas a su vez están conectadas en serie o en paralelo también pueden ser circuitos mixtos son fundamentales para los sistemas de control filtrado de señales y otros circuitos electrónicos.

![image](https://github.com/user-attachments/assets/bfbdd38f-73fe-4780-82c3-9c42bf77f4ca) 

Estos circuitos se rigen bajo la ley de ohm y otras leyes más como podemos ver en las siguientes ecuaciones tenemos que para cada uno de los elementos tenemos una ecuación característica estas son las siguientes.

$$R=\frac{V(t)}{I(t)}$$
$$I= C\frac{dV(t)}{dt}$$
$$V= L\frac{di(t)}{dt}$$


### 💡Ejemplo:

![image](https://github.com/user-attachments/assets/c25c2e1c-5cd9-41b0-a014-92bb979aec6c)

Figura2: Ejemplo 1

Iniciaremos haciendo la suma de voltajes e igualando a cero:

$$V_i + V_R + V_L V_C = 0$$

Luego reemplazaremos las ecuaciones mostradas anteriormente en la ecuación.

$$V_i (t) + i(t)R + L\frac{di(t)}{dt} + V_C = 0$$

Una vez teniendo esto nos podemos dar cuenta que para que nos quede todo el factor es de voltaje del condensador reemplazaremos en la derivada de $i(t)$ por lo que vale $I$, teniendo la siguiente ecuación.

$$-U(t)+RC\frac{\mathrm{d}V_{C}(t)}{\mathrm{d} t}+LC\frac{\mathrm{d^2}V_{C}(t)}{\mathrm{d}t^2}+V_{C}=0$$

## 3. Conclusiones
## 4. Referencias
