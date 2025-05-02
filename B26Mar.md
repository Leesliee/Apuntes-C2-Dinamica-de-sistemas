# Modelamiento de sistemas
### Nestor Alexander Avila Rojas, Leslie Stephania Rodriguez Marín
## 1. Introducción
## 2. Sistemas mecánicos
​Un sistema mecánico es un conjunto de componentes físicos interconectados cuya función principal es transformar o transmitir movimiento y fuerza desde una fuente de energía hasta un punto de salida, permitiendo así la realización de un trabajo específico.
### 1.1 Sistema masa-resorte-amortiguador

Un sistema masa-resorte-amortiguador es un modelo mecánico fundamental que describe cómo una masa se mueve bajo la influencia de fuerzas elásticas y de amortiguamiento. Este sistema es un modelo clasico en la mecanica que describe el comportamiento de un objeto (masa) que esta sujeto a la accion de un resorte y un amortiguador. Este sistema es fundamental para entender para entender como las fuerzas afectan el movimiento de objetos y como se disipa la energia en sistemas reales

### 1.2 Componentes principales

- **Masa(m):** Representa el objeto que se mueve bajo la influencia de las fuerzas del resorte y el amortiguador.
- **Resorte(k):** Aplica una fuerza proporcional a la deformacion del resorte, segun ley de hooke. Esta fuerza tiende a devolver la masa a su poscición de equilibrio. La constante del resorte mide la rigidez del mismo.
- **Amortiguador(B):** Representa la ressitencia que disipa energia, como la fricion o un amortiguador real, su función es reducir la velocidad del sistema con el tiempo. La fuerza de amortiguamiento es proporcional a la velocidad de la masa.
- **Fuerza externa F(t):** Es cualquier fuerza que se apliquye desde el exterior, como una fuerza constante o periodica. 

### 1.3 Ecuacion del movimiento

La dinámica del sistema se describe mediante una ecuación diferencial de segundo orden $m\ddot{x}(t) + b\dot{x}(t) + kx = F(t)\$ 

## 2 Sistemas Acoplados 

Los sistemas acoplados son aquellos en los que dos o mas sistemas interactúan entre sí, influyendo mutuamente en su comportamiento. Estos sitemas están conectados de tal forma que el movimiento o la dinámica de un sistema afecta directamente al otro, lo que genera una relación interdependiente

### 2.1 Caracteristicas de los sistemas acoplados
- **Interaccion:** los sistemas no son independientes, las variables que describen uno de los sitemas influyen en las variables del otro.
- **Ecuaciones interrelacionadas:** Las ecuaciones que describen cada sistema están vinculadas. es decir, las ecuaciones diferenciales o algebraicas de un sistema contienen términos que dependen de las variables del otro sistema.
- **Transferencia de energia:** Existe una transferencia de energia, fuerza o información entre los sistemas. esto puede ser a través de fuerzas fisicas (como una conexión elástica o un amortiguador) o señales de otro tipo.

### 2.2 Ecuaciones en sistemas acoplados 

las ecuaciones diferenciales que describren estos sistemas suelen ser de la forma:

$m_1\ddot{x_1} + d_1\dot{x_1} + k_1x_1 - k_2(x_2-x_1) = F_1(t)\$ 

$m_2\ddot{x_2} + d_2\dot{x_2} + k_2(x_2-x_1) = F_2(t)\$ 

aqui $x_1$ y $x_2$ representan el desplazamiento de cada masa, $k_2$ es la cosnstante del resorte que conecta las dos masas, y $f_1(t)$ y $f_2(t)$ son las fuerzas externas aplicadas a cada masa. Las ecuaciones estan interconectadas por que el movimiento de una masa afecta directamente a la otra.

# 📚 Ejercicio masa-resorte-amortiguador

Obtener las ecuaciones diferenciales del siguiente sistema 
![image](https://github.com/user-attachments/assets/ba02c2d3-3465-40e8-b9e0-e8a318840834)


**Se procede a realizar el diagrama de fuerzas para cada masa (Diagrama de cuerpo libre)

**Para masa 2:**

![image](https://github.com/user-attachments/assets/fc3dab1e-3f57-476a-a1d6-b6f01a37c325)


$$fb+fk-ff=0$$
$$b(\dot{y_2(t)} - \dot{y_1(t)}) + k(y_2(t) - y_1(t))= 0$$
$$b(\dot{y_2(t)} - \dot{y_1(t)}) + k(y_2(t) - y_1(t))= m*a$$
**Donde a = $\frac{d^2y(t)}{dt^2}$ que tambien se puede respresentar como $\ddot{y}$**

**sabiendo esto tenemos:**

$$b(\dot{y_2(t)} - \dot{y_1(t)}) + k(y_2(t) - y_1(t))= = m_2*\ddot{y}$$

**Para masa 1:**

![image](https://github.com/user-attachments/assets/15612b6a-3e37-492a-adcc-3fd46a156a49)

$$f(t)-fk-fb=0$$
$$f(t)- b(\dot{y_1(t)} - \dot{y_2(t)}) - k(y_1(t) - y_2(t)) = m_1*\ddot{y}$$
