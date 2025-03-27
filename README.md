# Corrección de parcial, corte 1

## 1. Introducción
En la sesión del 19 de marzo, se desarrolló la retroalimentación del primer parcial de la asignatura. Habían dos temas según la terminación del documento de identidad de cada estudiante, si el último número de la identificación del estudiante era impar se debía desarrollar el tema 1; si por el contrario el último número de la identificación era par, se debía desarrollar el tema 2. En este caso, se desarrollára la corrección del tema 1; pues el parcial se realizó con el número de documento: 1025523271.
## 2. Retroalimentación: Tema 1
### 📚 Ejercicio 1

### 📚 Ejercicio 2
Determinar la función en el dominio del tiempo de F(s):

$$F(s) = \frac{5*(s+2)}{s^2(s^2-4s+8)}$$

$$F(s) = \frac{5s+10}{s^2(s^2-4s+8)} = \frac{A}{(s)}+\frac{B}{s^2}+\frac{Cs+D}{s^2-4s+8}$$

$$\frac{(s^2)(s^2+4)(s^2 + 2s + 8)}{(s^2)(s^2+4)} = \frac{(s^2)(s^2+4)A}{(s)}+\frac{(s^2)(s^2+4)B}{(s^2)}+\frac{Cs+D}{(s^2+4)}$$

$$s^2 + 2s + 8= (s)(s^2+4)A + (s^2+4)B +(s^2)(Cs+D)$$

Al evaluar s = 0:

$$(0)^2 + 2(0) + 8= (0)((0)^2+4)A + ((0)^2+4)B +((0)^2)(Cs+D)$$
$$ 8 = (0)A + (4)B +(0)C $$
$$ B =  \frac{8}{4} $$
$$ B = 2 $$

Al evaluar s = 2i:

$$(2i)^2 + 2(2i) + 8= (2i)((2i)^2+4)A + ((2i)^2+4)B +((2i)^3)C+((2i)^2)D$$
$$ 4+4i = (0)A + (0)B - 4D - 8iC $$

Parte real con parte real y parte imaginaria con parte imaginaria:

$$\[
\begin{cases}
  -8C = 4 \\
  -4D = 4
\end{cases}
\]$$

$$ C = \frac{-1}{2}$$
$$ D = -1 $$

Sabiendo los valores de B, C y D; al evaluar s=1:

$$(1)^2 + 2(1) + 8= (1)((1)^2+4)A + ((1)^2+4)(2) +((1)^2)(-1/2-1)$$
$$ 11 = (5)A + 10 -\frac{3}{2} $$
$$ A =  \frac{11-10+\frac{3}{2}}{5} $$
$$ A = \frac{1}{2} $$

Se reemplaza:

$$F(s) =\frac{1/2}{(s)}+\frac{2}{(s^2)}+\frac{-1/2s-1}{(s^2+4)^2}$$

$$\mathcal{L}^{-1} \{ F(s) \} = \mathcal{L}^{-1} \left( \frac{1/2}{(s)} \right) + \mathcal{L}^{-1} \left( frac{2}{(s^2)} \right) + \mathcal{L}^{-1} \left( \frac{-1/2s-1}{(s^2+4)} \right)$$

$$\mathcal{L}^{-1} \{ F(s) \} = \frac{1}{2}\mathcal{L}^{-1} \left( \frac{1}{(s)} \right) + 2*\mathcal{L}^{-1} \left( \frac{1}{(s^2)} \right) - \frac{1}{2}\mathcal{L}^{-1} \left( \frac{s}{(s^2+4)^2} \right)-\mathcal{L}^{-1} \left( \frac{1}{(s^2+4)} \right)$$

$$\mathcal{L}^{-1} \{ F(s) \} = 1 + 2t -\frac{1}{2}*cos(2t)-\frac{1}{2}*sen(2t)$$

Y por último se encuentra la solución en el dominio del tiempo: 

$$f(t) =  1 + 2t -\frac{1}{2}*cos(2t)-\frac{1}{2}*sen(2t)$$
## 4. Conclusiones
En esta sesión, se evidenció que resolver un ejercicio extenso que involucre uno o varios casos 
## 5. Referencias
Jorge Eduardo Cote Ballesteros (2024). Soluciones de ecuaciones diferenciales; dinámica de sistemas. ETITC
