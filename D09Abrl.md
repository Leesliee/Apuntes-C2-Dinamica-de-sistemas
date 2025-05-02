# Modelamiento de sistemas eléctricos RLC
### Nestor Alexander Avila Rojas, Leslie Stephania Rodriguez Marín
## 1. Introducción
## 2. Ciruitor RLC
Un circuito RLC es un circuito eléctrico que está formado por resistencias inductancias y capacitancias estas a su vez están conectadas en serie o en paralelo también pueden ser circuitos mixtos son fundamentales para los sistemas de control filtrado de señales y otros circuitos electrónicos.

![image](https://github.com/user-attachments/assets/bfbdd38f-73fe-4780-82c3-9c42bf77f4ca) 

💡**Ejemplo 2:**
![image](https://github.com/user-attachments/assets/c25c2e1c-5cd9-41b0-a014-92bb979aec6c)

Estos circuitos se rigen bajo la ley de ohm y otras leyes más como podemos ver en las siguientes ecuaciones tenemos que para cada uno de los elementos tenemos una ecuación característica estas son las siguientes.

$$R=\frac{V(t)}{I(t)}$$
$$I= C\frac{dV(t)}{dt}$$
$$V= L\frac{di(t)}{dt}$$

Teniendo en cuenta estas ecuaciones y la imagen anterior podemos resolver el ejemplo 2 el cual sería la solución del circuito en serie, para ello utilizaremos la ley de voltajes de kirchhoff para así poder solucionar y encontrar la ecuación que nos describe el sistema.

Iniciaremos haciendo la suma de voltajes e igualando a cero.

$$V_i + V_R + V_L V_C = 0$$

Luego reemplazaremos las ecuaciones mostradas anteriormente en la ecuación.

$$V_i (t) + i(t)R + L\frac{di(t)}{dt} + V_C = 0$$

Una vez teniendo esto nos podemos dar cuenta que para que nos quede todo el factor es de voltaje del condensador reemplazaremos en la derivada de $i(t)$ por lo que vale $I$, teniendo la siguiente ecuación.

$$-U(t)+RC\frac{\mathrm{d}V_{C}(t)}{\mathrm{d} t}+LC\frac{\mathrm{d^2}V_{C}(t)}{\mathrm{d}t^2}+V_{C}=0$$

