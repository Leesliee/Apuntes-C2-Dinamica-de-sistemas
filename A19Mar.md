# Corrección de parcial, corte 1
### Alexander Ávila Rojas, Leslie Stephania Rodriguez Marín
## 1. Introducción
En la sesión del 19 de marzo, se desarrolló la retroalimentación del primer parcial de la asignatura. Habían dos temas según la terminación del documento de identidad de cada estudiante, si el último número de la identificación del estudiante era impar se debía desarrollar el tema 1; si por el contrario el último número de la identificación era par, se debía desarrollar el tema 2. En este caso, se desarrollará la retroalimentación de los dos temas.
## 2. Retroalimentación: Tema 1
### 📚 Ejercicio 1
Hallar la solución a la ecuación diferencial:

$$\ddot{x} + 4x = 5$$    
$$x(0) = 5  $$
$$\dot{x}(0) = 0$$

$$s^2X(S)-5s+4X(S) = \frac{5}{s}$$
$$X(S)[s^2+4] =\frac{5}{s} +5s $$
$$X(S) =\frac{\frac{5}{s}+5s}{s^2+4} $$
$$X(S) =\frac{5+5s}{s(s^2+4)} $$
$$X(S) =\frac{5+5s}{s(s^2+4)}= \frac{A}{s}+\frac{Bs+D}{s^2+4}$$
$$X(S) =5+5s^2= (s^2+4)A + s(Bs+D)$$

Al evaluar s = 0:

$$5+5(0)^2=((0)^+4)A+ 0(Bs+D)$$
$$5=4A+0$$
$$A=\frac{5}{4}$$

Al evaluar s = 2i:

$$5+5(2i)^2=((2i)^2+4)A+ (2i)^2B+2iD$$
$$-15=0A-4B+2iD$$

Se genera un sistema de ecuaciones con parte real y parte imaginaria:

$$
\begin{cases}
-4B = -15 \\
2D = 0 \\
\end{cases}
$$

$$D=0$$

$$B=\frac{-15}{-4}$$
$$B=\frac{15}{4}$$

Reemplazando:

$$X(S) = \frac{\frac{5}{4}}{s}+\frac{\frac{15}{4}s}{s^2+4}$$

$$
x(t) = \frac{5}{4}*\mathcal{L}^{-1}\{ \frac{1}{s}\}+\frac{15}{4} *\mathcal{L}^{-1}\{ \cdot \frac{s}{s^2 + 4} \} 
$$
$$ x(t)=\frac{5}{4} + \frac{15}{4} \cos(2t)$$



### 📚 Ejercicio 2
Determinar la función en el dominio del tiempo de F(s):
t
$$F(s) = \frac{5*(s+2)}{s^2(s^2-4s+8)}$$

$$F(s) = \frac{5s+10}{s^2(s^2-4s+8)} = \frac{A}{s}+\frac{B}{s^2}+\frac{Cs+D}{s^2-4s+8}$$

$$\frac{(s^2)(s^2 -4s + 8)*(5s+10)}{s^2(s^2-4s+8)} =(s^2)(s^2 -4s + 8) (\frac{A}{s}+\frac{B}{(s^2)}+\frac{(Cs+D)}{(s^2-4s+8)})$$

$$5s+10 = (s)(s^2 -4s + 8)A + (s^2 -4s + 8)B +s^2(Cs)+s^2D$$

aquiAl evaluar s = 0:

$$5(0)+10= (0)((0)^2-4(0)+8)A + ((0)^2-4(0)+8)B+(0)^2(Cs)+(0)^2D$$
$$ 10 = (0)A + (8)B +(0)(Cs+D) $$
$$ B =  \frac{10}{8} $$
$$ B = \frac{5}{4} $$

Al evaluar s = 2+2i:

$$5(2+2i)+10= (2+2i)((2+2i)^2-4(2+2i)+8)A + ((2+2i)^2-4(2+2i)+8)B +((2+2i)^2)^3C+((2+2i)^2)^2D$$
$$ 20+10i= (0)A + (0)B +(-16+16i)C+8iD $$
$$ 20+10i = -16C+16iC+8iD $$

Parte real con parte real y parte imaginaria con parte imaginaria:

$$\[
\begin{cases}
  -16C = 20 \\
  16C+8D = 10
\end{cases}
\]$$

$$ C = \frac{20}{-16}$$
$$ C = -\frac{5}{4}$$

$$ 16*-\frac{5}{4}+8D = 10 $$
$$ 8D = 10+20 $$
$$ D = \frac{30}{8} $$
$$ D = \frac{15}{4} $$

aquiSabiendo los valores de B, C y D; al evaluar s=1:

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
## 2. Retroalimentación: Tema 2
## 📚 Ejercicio 1:
$$2\ddot{x} + 2\dot{x} + x = 1\$$  

**Con las condiciones iniciales:**  $x(0) = 0,\quad \dot{x}(0) = 2$

**Aplicando Transformada de Laplace:**

$$2[s^2 X(s) - s x(0) - \dot{x}(0)] + 2[s X(s) - x(0)] + X(s) = \frac{1}{s}$$

**Sustituyendo condiciones iniciales:**

$$2[s^2 X(s) - 2] + 2[s X(s)] + X(s) = \frac{1}{s}$$

$$2s^2 X(s) - 4 + 2s X(s) + X(s) = \frac{1}{s}$$

$$X(s)(2s^2 + 2s + 1) = \frac{1}{s} + 4$$

$$X(s) = \frac{1 + 4s}{s(2s^2 + 2s + 1)}$$

**Aplicando fracciones parciales:** 

$$\frac{1 + 4s}{s(2s^2 + 2s + 1)} = \frac{A}{s} + \frac{Bs + D}{2s^2 + 2s + 1}$$

**Determinación de A:**

$$1 + 4s = A(2s^2 + 2s + 1) + (Bs + D)s$$

**Al evaluar s= 0**

$$A = \frac{1 + 4(0)}{2(0)^2 + 2(0) + 1} = \frac{1}{1} = 1$$

**Al evaluar s = -1 + 2i**

$$\frac{1 + 4(-1 + 2i)}{-1 + 2i}  = (-1 + 2i)(B(-1 + 2i) + D)$$

$$\frac{1 + 4(-1 + 2i)}{-1 + 2i}  = -B+ 2Bi + D$$

$$\frac{1 + 4 + 8i}{-1 + 2i} * \frac{-1 + 2i}{-1 + 2i} = -B+ 2Bi + D$$

$$\frac{3 + 6i + 8i + 16}{5} = -B + 2Bi + 5$$

$$\frac{19}{5} = -B - D$$

$$\frac{2i}{5} = 2Bi$$

$$B=\frac{1}{5}$$
$$D=\frac{20}{5} = 4$$
$$A = 1$$

## 📚 Ejercicio 2:

Determinar la función en el dominio del tiempo de F(s):

$$\frac{6S}{(S-\frac{5}{2})(S^2 -4S + 8)}$$

**Aplicando fracciones parciales:**

$$\frac{6S}{(S-\frac{5}{2})(S^2 -4S + 8)} = \frac{A}{S-\frac{5}{2}} + \frac{Bs + C}{S^2-4S+8}$$

**Se multiplica ambos lados por el denominador comun para eliminar los denominadores**

**Se expande y se agrupa en términos semejantes**

$$6s= As^2 - 4As + 8A + Bs^2 - \frac{5}{2} Bs + Cs - \frac{5}{2}C$$

$$6s= (A+B)s^2 + (-4A - \frac{5}{2}B + C)s + (8A - \frac{5}{2}C) - \frac{5}{2}C$$

**Se igualan los coeficientes de ambos lados:**

**Coeficiente de s^2:**

$$A+B=0$$
$$B = -A$$

**Coeficiente de s:**

$$-4A - \frac{5}{2}B + C = 6$$

**Término independiente**

$$8A - \frac{5}{2}C=0$$

**Se sustituye B=A en la segunda ecuación:**

$$-4A - \frac{5}{2} (-A) + C = 6$$

$$-4A \frac{5}{2}A + C = 6$$

$$-\frac{8}{2}A + \frac{5}{2}A+C=6$$

**Ecuación 1:**

$$-\frac{3}{2}A + C = 6 $$

**Ecuación término independiente:**

$$8A - \frac{5}{2}C=0$$

$$8A = \frac{5}{2}C$$
**Ecueción 2:**

$$C=\frac{16}{5}A$$

**Se sustituye $C = \frac{16}{5}A$ en la Ecuación 1:**

$$-\frac{3}{2}A + \frac{16}{5}A = 6$$

$$-(\frac{15}{10}A+\frac{32}{10})A = 6$$

$$\frac{17}{10}A=6$$

$$A = \frac{60}{17}$$

**Entonces:**

$$B = -A = -\frac{60}{17}$$

$$C = \frac{16}{5} \cdot \frac{60}{17} = \frac{960}{85} = \frac{192}{17}$$

**Por tanto, la descomposición en fracciones parciales es:**

$$F(s) = \frac{60}{17} \cdot \frac{1}{s - \frac{5}{2}} + \frac{-\frac{60}{17}s + \frac{192}{17}}{s^2 - 4s + 8}$$

**Se simplifica:**

$$F(s) = \frac{60}{17} \cdot \frac{1}{s - \frac{5}{2}} - \frac{60}{17} \cdot \frac{s - \frac{192}{60}}{s^2 - 4s + 8}$$

$$F(s) = \frac{60}{17} \cdot \frac{1}{s - \frac{5}{2}} - \frac{60}{17} \cdot \frac{s - \frac{16}{5}}{s^2 - 4s + 8}$$

**Para el término $s^2 - 4s + 8$ se completa el cuadrado:**

$$s^2 - 4s + 8 = (s^2 - 4s + 4) + 4 = (s - 2)^2 + 4$$

**Por tanto:**

$$F(s) = \frac{60}{17} \cdot \frac{1}{s - \frac{5}{2}} - \frac{60}{17} \cdot \frac{s - \frac{16}{5}}{(s - 2)^2 + 4}$$

**Se separa el segundo término en dos partes para facilitar la transformada inversa:**

$$\frac{s - \frac{16}{5}}{(s - 2)^2 + 4} = \frac{s - 2}{(s - 2)^2 + 4} + \frac{-2 + \frac{16}{5}}{(s - 2)^2 + 4}$$

$$= \frac{s - 2}{(s - 2)^2 + 4} + \frac{\frac{6}{5}}{(s - 2)^2 + 4}$$

**Entonces:**

$$F(s) = \frac{60}{17} \cdot \frac{1}{s - \frac{5}{2}} - \frac{60}{17} \left( \frac{s - 2}{(s - 2)^2 + 4} + \frac{6}{5} \cdot \frac{1}{(s - 2)^2 + 4} \right)$$

**Distribuyendo:**

$$F(s) = \frac{60}{17} \cdot \frac{1}{s - \frac{5}{2}} - \frac{60}{17} \cdot \frac{s - 2}{(s - 2)^2 + 4} - \frac{60}{17} \cdot \frac{6}{5} \cdot \frac{1}{(s - 2)^2 + 4}$$

$$= \frac{60}{17} \cdot \frac{1}{s - \frac{5}{2}} - \frac{60}{17} \cdot \frac{s - 2}{(s - 2)^2 + 4} - \frac{72}{17} \cdot \frac{1}{(s - 2)^2 + 4}$$

**Aplicando transformada inversa de Laplace:**

$$f(t) = \frac{60}{17} e^{\frac{5}{2}t} - \frac{e^{2t}}{17} \left(60 \cos(2t) + 36 \sin(2t) \right)$$
## 4. Conclusiones
En esta sesión 
## 5. Referencias

