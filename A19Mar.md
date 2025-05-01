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

$$\mathcal{L}^{-1} \left\{ \frac{5}{4s} + \frac{15}{4} \cdot \frac{s}{s^2 + 4} \right\} = \frac{5}{4} + \frac{15}{4} \cos(2t)$$

### 📚 Ejercicio 2
Determinar la función en el dominio del tiempo de F(s):
t
$$F(s) = \frac{5*(s+2)}{s^2(s^2-4s+8)}$$

$$F(s) = \frac{5s+10}{s^2(s^2-4s+8)} = \frac{A}{s}+\frac{B}{s^2}+\frac{Cs+D}{s^2-4s+8}$$

$$\frac{(s^2)(s^2 -4s + 8)*(5s+10)}{s^2(s^2-4s+8)} = \frac{(s^2)(s^2 + 2s + 8)A}{s}+\frac{(s^2)(s^2 + 2s + 8)B}{(s^2)}+\frac{(s^2)(s^2 + 2s + 8)(Cs+D)}{(s^2-4s+8)}$$

$$5s+10 = (s)(s^2 -4s + 8)A + (s^2 + 2s + 8)B +(s^2)(Cs+D)$$

Al evaluar s = 0:

$$5(0)+10= (0)((0)^2-4(0)+8)A + ((0)^2-4(0)+8)B +((0)^2)(Cs+D)$$
$$ 10 = (0)A + (8)B +(0)(Cs+D) $$
$$ B =  \frac{10}{8} $$
$$ B = \frac{5}{4} $$

Al evaluar s = 2+2i:

$$5s+10 = (s)(s^2 -4s + 8)A + (s^2 + 2s + 8)B +Cs^3+Ds^2$$
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
## 2. Retroalimentación: Tema 2
## 4. Conclusiones
En esta sesión 
## 5. Referencias

