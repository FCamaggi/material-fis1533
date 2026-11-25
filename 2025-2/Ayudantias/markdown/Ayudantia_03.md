---
title: "Ayudantia 03"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_03_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_03_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 03

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Ayudantía 3
19 de Agosto 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Ley de Gauss

1.1

Ley de Gauss - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Identificar las condiciones necesarias para utilizar la Ley de Gauss.
□
✓ Reconocer los distintos intervalos en los que se debe aplicar la Ley de Gauss.
□
□ Determinar el campo eléctrico generado por un cuerpo cargado que presente simetría
plana mediante la Ley de Gauss.

✓ Determinar el campo eléctrico generado por un cuerpo cargado que presente simetría
□
cilíndrica mediante la Ley de Gauss.
✓ Determinar el campo eléctrico generado por un cuerpo cargado que presente simetría
□
esférica mediante la Ley de Gauss.
✓ Calcular la carga de un cuerpo mediante su definición, ya sea una densidad de carga
□
uniforme o variable.
✓ Evaluar el campo eléctrico en un punto del espacio, considerando su sentido y dirección.
□
✓ Graficar la magnitud del campo eléctrico en función del radio para alambres, cilindros y
□
esferas.
✓ Comprender matemáticamente el concepto de flujo.
□
□ Aplicar la primera ecuación de Maxwell en el vacío en diversos contextos.

---

### Página 2

1.2

Ley de Gauss - Generalidades

El flujo de un campo eléctrico = E” a través de una superficie = S” está dado por:
Z
E · ds
Φe =

(1)

S

Se debe considerar que solo la componente ortogonal a la superficie contribuye al flujo.

Luego, la Ley de Gauss se puede enunciar como:
I
Qenc
E · ds =
ε0
S

(2)

Donde = Qenc ” es la carga encerrada y = ds” la diferencial de superficie.

Finalmente, y aplicando el teorema de la divergencia al flujo del campo eléctrico, es posible
obtener la primera ecuación de Maxwell en el vacío:
ρ
∇·E=
(3)
ε0

1.3

Ley de Gauss - Cómo Utilizarlo Correctamente

Es importante aclarar que esta ley solo se podrá utilizar cuando el problema presente simetría
plana, cilíndrica o esférica. De aquí en adelante, y siempre cuando lo amerite, se deberá tratar
de usar la Ley de Gauss por sobre la definición de campo eléctrico para resolver de una manera
más sencilla los ejercicios. Así, la aplicación consta de dos partes:
H
a) = S E · ds ”: en esta se calculará el flujo que aporta el campo eléctrico al pasar por la
superficie gaussiana. De esta manera:
1. Se deberá elegir la superficie gaussiana según la simetría del cuerpo.
2. Calcular el flujo eléctrico, considerando que solo la componente perpendicular a la
superficie gaussiana contribuye a su valor.
3. Generalmente, este cálculo resultará en el producto entre el área de la superficie
gaussiana = importante” y la componente ortogonal del campo. Todos los aspectos
revelantes se resumen en la tabla del Anexo 2.3.
b) = Qεenc
”: en esta parte se deberá calcular la carga del cuerpo que está encerrada por la
superficie gaussiana.
1. Luego, se deberá despejar el campo eléctrico de la igualdad.
2. En caso de requerir la forma vectorial del campo, se añade el componente vectorial
que aporta al flujo, el cual será siempre hacia fuera del cuerpo (vector normal = n̂”).
3. Todo este procedimiento se debe realizar para cada intervalo existente, los cuales se
pueden reconocer fácilmente mediante los = cortes” visuales del cuerpo.
4. Además, una superficie cargada provocará una discontinuidad en el campo eléctrico.
Gráficamente esto podría verse como una = punta”, lo cual matemáticamente equivaldría a una inexistencia del límite en el punto respectivo (en otras palabras, los
límites por la derecha e izquierda del punto no coinciden en su valor).

---

### Página 3

Anexos

2.1

Series de Taylor

Decimos que una función = f (x)” puede expandirse como una serie de potencias en torno a = a”:
f (x) =

∞
X

cn (x − a)n

para todo |x − a| < R con R > 0

n=0

Ahora, y si la función = f (x)” puede derivarse infinitamente alrededor de = a”, podemos expresarla como una serie de Taylor:
T (x) =

∞
X
f (n) (a)

n!

n=0

(x − a)n = f (a) +

f ′ (a)
f ′′ (a)
f (3) (a)
(x − a) +
(x − a)2 +
(x − a)3 + . . .
1!
2!
3!

Más aún, y si a = 0, esta serie pasa a llamarse la serie de McLaurin de la función = f (x)”:

M (x) =

∞
X
f (n) (0)

n!

n=0

xn = f (0) +

f ′ (0)
f ′′ (0) 2 f (3) (0) 3
x+
x +
x + ...
1!
2!
3!

Ejemplo: Series más Utilizadas
Algunas de las series más comunes se muestran a continuación:
∞

X
=
xn = 1 + x + x2 + x3 + . . . ,
1−x

R=1

n=0

sin x =

∞
X

(−1)n

n=0
∞
X

cos x =

x3 x5 x7
x2n+1
=x−
+
−
+ ...,
(2n + 1)!
3!
5!
7!

(−1)n

n=0
k

(1 + x) =

∞  
X
k
n=0

n

x2n
x2 x4 x6
=1−
+
−
+ ...,
(2n)!
2!
4!
6!

xn = 1 + kx +

R=∞

R=∞

k(k − 1) 2 k(k − 1)(k − 2) 3
x +
x + ...,
2!
3!

R=1

Ejemplo: Aproximación por Grados
Sería muy poco conveniente usar toda la expresión asociada a la serie de potencia, por
lo que se acostumbra utilizarlas hasta cierto = grado”, el cual será igual al exponente más
alto que acompañe a cualquiera de las = x”. Por ejemplo, podríamos querer aproximar
la expansión de = ex ” a primer orden (aún así, se incluyen todos los términos de orden
inferior a este), tal como se muestra a continuación:
ex =

∞
X
xn
n=0

n!

=1+

x
x2 x3
x
+
+
+ ··· ≈ 1 +
1!
2!
3!
1!

Si es que aún te cuesta, puedes seguir consultando estos conceptos en Series de Taylor y de McLaurin.

---

### Página 4

r = xx̂ + yŷ + zẑ

Forma
Vectorial

dV = dx dy dz

Diferencial
Volumen

Se debe notar que pueden haber distintas notaciones para el vector unitario (î = x̂, ĵ = ŷ, k̂ = ẑ)
y que la diferencial de volumen también se puede obtener mediante el cálculo de la matriz jacobiana.
Finalmente, en las coordenadas esféricas se considera al ángulo = θ” como el que barre verticalmente
desde arriba (0 < θ < π), mientras que al ángulo = ϕ” como el que barre el = suelo” (0 < ϕ < 2π).

dV = r2 sin θ dr dθ dϕ

dSr=cte = r2 sin θ dθ dϕ r̂
dSθ=cte = r sin θ dr dϕ θ̂
dSϕ=cte = r dr dθ ϕ̂
dSρ=cte = ρ dθ dz ρ̂
dSθ=cte = dρ dz θ̂
dSz=cte = ρ dρ dθ ẑ

dSx=cte = dy dz x̂
dSy=cte = dx dz ŷ
dSz=cte = dx dy ẑ

Diferencial
Superficie

dV = ρ dρ dθ dz

dr = drr̂ + r dθθ̂ + r sin θ dϕϕ̂

dr = dρρ̂ + ρ dθθ̂ + dzẑ

r̂ = sin θ cos ϕ x̂+sin θ sin ϕ ŷ+cos θ ẑ

ρ̂ = cos θ x̂ + sin θ ŷ
θ̂ = − sin θ x̂ + cos θ ŷ

dr = dxx̂ + dyŷ + dzẑ

r = rr̂

C. Esféricas

r = ρρ̂ + zẑ

C. Cilíndricas

Coordenadas y Diferenciales

Diferencial
Línea

Componente

C. Cartesianas

Conceptos

2.2

---

### Página 5

Cilindro Ortogonal

Perpendicular (ẑ)

Superficie
Gaussiana

Componente
Ortogonal

Resultado
Integral
S.G.I

Integral
S.G.I

S = πR2

S = 2πrL

0 r dz dθ

R 2π R L

Manto Cilindro

Radial (ρ̂)

Cilindro Coaxial

Alambres - Cilindros Infinitos

Simetría Cilíndrica

Aplicación Ley de Gauss

2 sin θ dθ dϕ

S = 4πr2

0 r

R 2π R π

Superficie Esfera

Radial (r̂)

Esfera Concéntrica

Esferas

Simetría Esférica

En algunos casos será necesario integrar, por lo que no se recomienda solo saber los resultados.
Para armar las integrales puede ser de utilidad conocer las relaciones de los diferenciales del Anexo 2.2.
R 2π R π R R
Podría ser conveniente tener en mente que Vesfera, R = 0 0 0 r2 sin θ dr dθ dϕ = 34 πR3

0 r dr dθ

R 2π R R

Bases Cilindro

Planos - Bloques Infinitos

Ejemplos
Cuerpos

Superficie
Gaussiana
Importante

Simetría Plana

Conceptos

2.3

---

### Página 6

2.3.1

“Problemas de Electromagnetismo”, 1.46, Sebastián Urrutia

Un cascarón cilíndrico de largo infinito, con densidad volumétrica de carga homogénea
ρ, radio interior 2a y radio exterior 4a es ubicado en el origen del plano XY con su eje a
lo largo del eje Z. Además, por el punto (0, a, 0) pasa un alambre infinito perpendicular
al plano XY (paralelo al eje Z) con densidad de carga lineal λ como es mostrado en la
figura. ¿Cuál debiese ser la relación entre λ y ρ para que el campo eléctrico en el punto
P = (0, 3a, 0) sea cero?

Figura 1. Esquema sobre el cascarón y el alambre.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la relación entre λ y ρ de manera que el campo eléctrico cumpla la condición
dada en el punto P . Como se está hablando de un alambre y cilindro de extensión infinita, es
posible aplicar Ley de Gauss utilizando un cilindro coaxial de altura = h” y radio = r” arbitrario:
I
Qenc
E · ds =
ε0
S
No se entrega explícitamente la carga contenida en ambos cuerpos,
por lo que se tendrá que utilizar la definición de carga:

Z
Q=
λ dl
L
ZZZ
Q=
ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio en la densidad
de carga del cilindro, se debe trabajar por intervalos: r < 2a, 2a < r < 4a y r > 4a.
Finalmente, se deberán evaluar y superponer ambos campos eléctricos.

---

### Página 7

2.3.2

“Problemas Resueltos de Electromagnetismo”, 3.10, Rodrigo Chi

Un cilindro infinito de radio R tiene su eje coincidente con el eje z. El cilindro posee
una densidad volumétrica ρ(r) = ar donde a es una constante positiva y r es la distancia
desde el eje del cilindro.
a) Calcule la carga contenida en un cilindro centrado en el eje z, de radio r y altura
h para los casos r < R y r > R.
b) Determine el campo eléctrico en todo el espacio.
c) Grafique la magnitud del campo eléctrico en función de r.

Figura 2. Esquema sobre cilindro.

---

### Página 8

Solución a) y b)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico y la carga contenida en todo el espacio. Como se está
hablando de un cilindro de extensión infinita, es posible aplicar Ley de Gauss utilizando un
cilindro concéntrico de altura = h” y radio = r” arbitrario:
I
Qenc
E · ds =
ε0
S
No se entrega explícitamente la carga contenida en el cilindro y su densidad
de carga no es uniforme, por lo que se tendrá que utilizar la definición de carga:

ZZZ
ρ dV

Q=
V

Además, y como se presentan = cortes visuales” relacionados con un cambio en la
densidad de carga del cilindro, se debe trabajar por intervalos: r < R y r > R.

Solución c)
Paso Único: Campo Eléctrico - Gráfico
Para realizar el gráfico solo se debe observar la parte variable (en este caso r) del módulo del
campo en cada uno de los intervalos y asociarlos a una gráfica conocida, además de evaluar (si
es que necesario) sus valores límite.

---

### Página 9

2.3.3

“Ejercicios Teoría Electromagnética ”, 4.1.5, Fabián Cádiz

Considere dos esferas no concéntricas de radio R. La primera de ellas lleva una densidad
volumétrica de carga ρ y la segunda −ρ. Los centros de las esferas están a distancia
menor que 2R. Si d⃗ es el vector que va del centro de la esfera positiva al centro de la
negativa, demuestre que el campo eléctrico en la intersección de las esferas es constante
y encuentre su valor.

Figura 3. Esquema sobre las esferas.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en la intersección de las esferas. Como se está hablando
de una esfera, es posible aplicar Ley de Gauss utilizando una esfera concéntrica de radio = r”
arbitrario:
I
Qenc
E · ds =
ϵ0
S
No se entrega explícitamente la carga contenida en ambos cuerpos,
por lo que se tendrá que utilizar la definición de carga:

ZZZ
Q=

ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: r < R y r > R.
Finalmente, se deberá superponer ambos campos eléctricos.

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 3
19 de Agosto 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Ley de Gauss

1.1

Ley de Gauss - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Identificar las condiciones necesarias para utilizar la Ley de Gauss.
□
✓ Reconocer los distintos intervalos en los que se debe aplicar la Ley de Gauss.
□
□ Determinar el campo eléctrico generado por un cuerpo cargado que presente simetría
plana mediante la Ley de Gauss.

✓ Determinar el campo eléctrico generado por un cuerpo cargado que presente simetría
□
cilíndrica mediante la Ley de Gauss.
✓ Determinar el campo eléctrico generado por un cuerpo cargado que presente simetría
□
esférica mediante la Ley de Gauss.
✓ Calcular la carga de un cuerpo mediante su definición, ya sea una densidad de carga
□
uniforme o variable.
✓ Evaluar el campo eléctrico en un punto del espacio, considerando su sentido y dirección.
□
✓ Graficar la magnitud del campo eléctrico en función del radio para alambres, cilindros y
□
esferas.
✓ Comprender matemáticamente el concepto de flujo.
□
□ Aplicar la primera ecuación de Maxwell en el vacío en diversos contextos.

---

### Página 2

1.2

Ley de Gauss - Generalidades

El flujo de un campo eléctrico = E” a través de una superficie = S” está dado por:
Z
E · ds
Φe =

(1)

S

Se debe considerar que solo la componente ortogonal a la superficie contribuye al flujo.

Luego, la Ley de Gauss se puede enunciar como:
I
Qenc
E · ds =
ε0
S

(2)

Donde = Qenc ” es la carga encerrada y = ds” la diferencial de superficie.

Finalmente, y aplicando el teorema de la divergencia al flujo del campo eléctrico, es posible
obtener la primera ecuación de Maxwell en el vacío:
ρ
∇·E=
(3)
ε0

1.3

Ley de Gauss - Cómo Utilizarlo Correctamente

Es importante aclarar que esta ley solo se podrá utilizar cuando el problema presente simetría
plana, cilíndrica o esférica. De aquí en adelante, y siempre cuando lo amerite, se deberá tratar
de usar la Ley de Gauss por sobre la definición de campo eléctrico para resolver de una manera
más sencilla los ejercicios. Así, la aplicación consta de dos partes:
H
a) = S E · ds ”: en esta se calculará el flujo que aporta el campo eléctrico al pasar por la
superficie gaussiana. De esta manera:
1. Se deberá elegir la superficie gaussiana según la simetría del cuerpo.
2. Calcular el flujo eléctrico, considerando que solo la componente perpendicular a la
superficie gaussiana contribuye a su valor.
3. Generalmente, este cálculo resultará en el producto entre el área de la superficie
gaussiana = importante” y la componente ortogonal del campo. Todos los aspectos
revelantes se resumen en la tabla del Anexo 2.3.
b) = Qεenc
”: en esta parte se deberá calcular la carga del cuerpo que está encerrada por la
superficie gaussiana.
1. Luego, se deberá despejar el campo eléctrico de la igualdad.
2. En caso de requerir la forma vectorial del campo, se añade el componente vectorial
que aporta al flujo, el cual será siempre hacia fuera del cuerpo (vector normal = n̂”).
3. Todo este procedimiento se debe realizar para cada intervalo existente, los cuales se
pueden reconocer fácilmente mediante los = cortes” visuales del cuerpo.
4. Además, una superficie cargada provocará una discontinuidad en el campo eléctrico.
Gráficamente esto podría verse como una = punta”, lo cual matemáticamente equivaldría a una inexistencia del límite en el punto respectivo (en otras palabras, los
límites por la derecha e izquierda del punto no coinciden en su valor).

---

### Página 3

Anexos

2.1

Series de Taylor

Decimos que una función = f (x)” puede expandirse como una serie de potencias en torno a = a”:
f (x) =

∞
X

cn (x − a)n

para todo |x − a| < R con R > 0

n=0

Ahora, y si la función = f (x)” puede derivarse infinitamente alrededor de = a”, podemos expresarla como una serie de Taylor:
T (x) =

∞
X
f (n) (a)

n!

n=0

(x − a)n = f (a) +

f ′ (a)
f ′′ (a)
f (3) (a)
(x − a) +
(x − a)2 +
(x − a)3 + . . .
1!
2!
3!

Más aún, y si a = 0, esta serie pasa a llamarse la serie de McLaurin de la función = f (x)”:

M (x) =

∞
X
f (n) (0)

n!

n=0

xn = f (0) +

f ′ (0)
f ′′ (0) 2 f (3) (0) 3
x+
x +
x + ...
1!
2!
3!

Ejemplo: Series más Utilizadas
Algunas de las series más comunes se muestran a continuación:
∞

X
=
xn = 1 + x + x2 + x3 + . . . ,
1−x

R=1

n=0

sin x =

∞
X

(−1)n

n=0
∞
X

cos x =

x3 x5 x7
x2n+1
=x−
+
−
+ ...,
(2n + 1)!
3!
5!
7!

(−1)n

n=0
k

(1 + x) =

∞  
X
k
n=0

n

x2n
x2 x4 x6
=1−
+
−
+ ...,
(2n)!
2!
4!
6!

xn = 1 + kx +

R=∞

R=∞

k(k − 1) 2 k(k − 1)(k − 2) 3
x +
x + ...,
2!
3!

R=1

Ejemplo: Aproximación por Grados
Sería muy poco conveniente usar toda la expresión asociada a la serie de potencia, por
lo que se acostumbra utilizarlas hasta cierto = grado”, el cual será igual al exponente más
alto que acompañe a cualquiera de las = x”. Por ejemplo, podríamos querer aproximar
la expansión de = ex ” a primer orden (aún así, se incluyen todos los términos de orden
inferior a este), tal como se muestra a continuación:
ex =

∞
X
xn
n=0

n!

=1+

x
x2 x3
x
+
+
+ ··· ≈ 1 +
1!
2!
3!
1!

Si es que aún te cuesta, puedes seguir consultando estos conceptos en Series de Taylor y de McLaurin.

---

### Página 4

r = xx̂ + yŷ + zẑ

Forma
Vectorial

dV = dx dy dz

Diferencial
Volumen

Se debe notar que pueden haber distintas notaciones para el vector unitario (î = x̂, ĵ = ŷ, k̂ = ẑ)
y que la diferencial de volumen también se puede obtener mediante el cálculo de la matriz jacobiana.
Finalmente, en las coordenadas esféricas se considera al ángulo = θ” como el que barre verticalmente
desde arriba (0 < θ < π), mientras que al ángulo = ϕ” como el que barre el = suelo” (0 < ϕ < 2π).

dV = r2 sin θ dr dθ dϕ

dSr=cte = r2 sin θ dθ dϕ r̂
dSθ=cte = r sin θ dr dϕ θ̂
dSϕ=cte = r dr dθ ϕ̂
dSρ=cte = ρ dθ dz ρ̂
dSθ=cte = dρ dz θ̂
dSz=cte = ρ dρ dθ ẑ

dSx=cte = dy dz x̂
dSy=cte = dx dz ŷ
dSz=cte = dx dy ẑ

Diferencial
Superficie

dV = ρ dρ dθ dz

dr = drr̂ + r dθθ̂ + r sin θ dϕϕ̂

dr = dρρ̂ + ρ dθθ̂ + dzẑ

r̂ = sin θ cos ϕ x̂+sin θ sin ϕ ŷ+cos θ ẑ

ρ̂ = cos θ x̂ + sin θ ŷ
θ̂ = − sin θ x̂ + cos θ ŷ

dr = dxx̂ + dyŷ + dzẑ

r = rr̂

C. Esféricas

r = ρρ̂ + zẑ

C. Cilíndricas

Coordenadas y Diferenciales

Diferencial
Línea

Componente

C. Cartesianas

Conceptos

2.2

---

### Página 5

Cilindro Ortogonal

Perpendicular (ẑ)

Superficie
Gaussiana

Componente
Ortogonal

Resultado
Integral
S.G.I

Integral
S.G.I

S = πR2

S = 2πrL

0 r dz dθ

R 2π R L

Manto Cilindro

Radial (ρ̂)

Cilindro Coaxial

Alambres - Cilindros Infinitos

Simetría Cilíndrica

Aplicación Ley de Gauss

2 sin θ dθ dϕ

S = 4πr2

0 r

R 2π R π

Superficie Esfera

Radial (r̂)

Esfera Concéntrica

Esferas

Simetría Esférica

En algunos casos será necesario integrar, por lo que no se recomienda solo saber los resultados.
Para armar las integrales puede ser de utilidad conocer las relaciones de los diferenciales del Anexo 2.2.
R 2π R π R R
Podría ser conveniente tener en mente que Vesfera, R = 0 0 0 r2 sin θ dr dθ dϕ = 34 πR3

0 r dr dθ

R 2π R R

Bases Cilindro

Planos - Bloques Infinitos

Ejemplos
Cuerpos

Superficie
Gaussiana
Importante

Simetría Plana

Conceptos

2.3

---

### Página 6

2.3.1

“Problemas de Electromagnetismo”, 1.46, Sebastián Urrutia

Un cascarón cilíndrico de largo infinito, con densidad volumétrica de carga homogénea
ρ, radio interior 2a y radio exterior 4a es ubicado en el origen del plano XY con su eje a
lo largo del eje Z. Además, por el punto (0, a, 0) pasa un alambre infinito perpendicular
al plano XY (paralelo al eje Z) con densidad de carga lineal λ como es mostrado en la
figura. ¿Cuál debiese ser la relación entre λ y ρ para que el campo eléctrico en el punto
P = (0, 3a, 0) sea cero?

Figura 1. Esquema sobre el cascarón y el alambre.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la relación entre λ y ρ de manera que el campo eléctrico cumpla la condición
dada en el punto P . Como se está hablando de un alambre y cilindro de extensión infinita, es
posible aplicar Ley de Gauss utilizando un cilindro coaxial de altura = h” y radio = r” arbitrario:
I
Qenc
E · ds =
ε0
S
No se entrega explícitamente la carga contenida en ambos cuerpos,
por lo que se tendrá que utilizar la definición de carga:

Z
Q=
λ dl
L
ZZZ
Q=
ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio en la densidad
de carga del cilindro, se debe trabajar por intervalos: r < 2a, 2a < r < 4a y r > 4a.
Finalmente, se deberán evaluar y superponer ambos campos eléctricos.

---

### Página 7

Paso 1: Ley de Gauss - Alambre
Se calculará el campo eléctrico aplicando la Ley de Gauss:
I
Qenc
E · ds =
ε0
Como es un alambre infinito, el campo solo poseerá componente radial.
Además, la carga encerrada estará determinada por una integral simple en cartesianas:

R

I
E·

dS =

L λ dl

ε0

Como la densidad de carga lineal del alambre es uniforme,
se puede tratar como una constante y sale de la integral.
Ahora, la integral cerrada es en verdad la superficie del manto del
cilindro gaussiano, pues el flujo es ortogonal a este en todo momento:

R
λ · L dl
E · 2πrh =
ε0
La integral de línea se refiere al perímetro encerrado
por el cilindro gaussiano de altura = h” y radio = r”.
En este caso, sería parte del perímetro del alambre:

Rh
λ · 0 dl
E · 2πrh =
ε0
λ·h
E · 2πrh =
ε0
λ
E=
2πε0 r
Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

E=

λ
r̂
2πε0 r

(4)

Considerando que el campo eléctrico generado por el alambre apunta verticalmente
hacia arriba en el punto P y que se ubica en (0, a, 0), se debe evalúar su campo en
r = 2a para determinar el campo elétrico generado por este en el punto (0, 3a, 0):

Ealambre,P =

λ
ŷ
4πε0 a

Nota: Se recuerda que el campo de cada uno de los cuerpos se origina desde su propio
eje, por lo que al momento de evaluarlo es necesario calcular la distancia y sentido desde
aquel sistema de referencia.

(5)

---

### Página 8

Paso 2: Ley de Gauss - Cilindro
Como el punto a evaluar se encuentra en la región 2a < r < 4a, solo se calculará el campo
eléctrico para el cilindro en tal región aplicando la Ley de Gauss:
I
Qenc
E2a<r<4a · ds =
ε0
Como es un cilindro infinito, el campo solo poseerá componente radial.
Además, la carga encerrada estará determinada por una integral triple en cilíndricas:

RRR

I
E2a<r<4a ·

V ρ dV

dS =

ε0

Como la densidad de carga volumétrica del cascarón es uniforme,
se puede tratar como una constante y sale de la integral.
Ahora, la integral cerrada es en verdad la superficie del manto
del cilindro gaussiano, pues el flujo es ortogonal a este en todo momento:

E2a<r<4a · 2πrh =

ρ·

RRR

V dV

ε0

La integral de volumen se refiere al volumen encerrado
por el cilindro gaussiano de altura = h” y radio = r”.
En este caso, sería parte del volumen del cilindro con carga:

R h R 2π R r
ρ · 0 0 2a r dr dθ dz
E2a<r<4a · 2πrh =
ε0

ρ · h · 2π · ( r2 − (2a)
2 )
E2a<r<4a · 2πrh =
ε0
ρ
E2a<r<4a =
(r − 4a2 )
2ε0 r
Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

E2a<r<4a =

ρ
(r2 − 4a2 ) r̂
2ε0 r

(6)

Considerando que el campo eléctrico generado por el cilindro apunta verticalmente
hacia arriba en el punto P y que su eje se ubica en el (0,0,0), se debe evalúar su campo
en r = 3a para determinar el campo eléctrico generado por este en el punto (0,3a,0):

Ecilindro,P =

5ρa
ŷ
6ε0

Nota: Se recuerda que el campo de cada uno de los cuerpos se origina desde su propio
eje, por lo que al momento de evaluarlo es necesario calcular la distancia desde aquel
sistema de referencia.

(7)

---

### Página 9

Paso 3: Principio de Superposición - λρ
Luego, y mediante el principio de superposición, se impone la condición para que el campo en
el punto P = (0, 3a, 0) sea cero:
Ealambre,P + Ecilindro,P = 0
λ
5ρa2
ŷ = 0
ŷ +
4πε0 a
6ε0
Como la componente vectorial es única y equivalente
en la ecuación vectorial, se puede obviar en el análisis:

λ
5ρa
=−
4πε0 a
6ε0
λ
10 2
= − πa
ρ

(8)

---

### Página 10

2.3.2

“Problemas Resueltos de Electromagnetismo”, 3.10, Rodrigo Chi

Un cilindro infinito de radio R tiene su eje coincidente con el eje z. El cilindro posee
una densidad volumétrica ρ(r) = ar donde a es una constante positiva y r es la distancia
desde el eje del cilindro.
a) Calcule la carga contenida en un cilindro centrado en el eje z, de radio r y altura
h para los casos r < R y r > R.
b) Determine el campo eléctrico en todo el espacio.
c) Grafique la magnitud del campo eléctrico en función de r.

Figura 2. Esquema sobre cilindro.

---

### Página 11

Solución a) y b)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico y la carga contenida en todo el espacio. Como se está
hablando de un cilindro de extensión infinita, es posible aplicar Ley de Gauss utilizando un
cilindro concéntrico de altura = h” y radio = r” arbitrario:
I
Qenc
E · ds =
ε0
S
No se entrega explícitamente la carga contenida en el cilindro y su densidad
de carga no es uniforme, por lo que se tendrá que utilizar la definición de carga:

ZZZ
Q=

ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio en la
densidad de carga del cilindro, se debe trabajar por intervalos: r < R y r > R.

Paso 1: Ley de Gauss - Er<R
En primer lugar, se calculará el campo eléctrico mediante la Ley de Gauss en la región r < R:
I
Qenc
Er<R · ds =
ε0
Como es un cilindro infinito, el campo solo poseerá componente radial.
Además, la carga encerrada estará determinada por una integral triple en cilíndricas:

RRR

I
Er<R ·

V ρ dV

dS =

ε0

Como la densidad de carga lineal del cilindro no es uniforme,
no se puede tratar como una constante y es necesario integrar.
Ahora, la integral cerrada es en verdad la superficie del manto del
cilindro, pues el flujo es ortogonal a este en todo momento:

RRR
Er<R · 2πrh =

V ρ dV

ε0

La integral de volumen se refiere al volumen encerrado
por el cilindro gaussiano de altura = h” y radio = r”.
En este caso, sería parte del volumen del cilindro con carga:

R h R 2π R r r
Er<R · 2πrh =
Er<R · 2πrh =

0 a · r drdθdz

ε0
r3
h · 2π · 3a

ε0
r2
Er<R =
3aε0

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

Er<R =

r2
r̂
3aε0

(9)

---

### Página 12

Paso 2: Ley de Gauss - Er>R
Luego, se calculará el campo eléctrico mediante la Ley de Gauss en la región r > R:
I
Qenc
Er>R · ds =
ε0
Como es un cilindro infinito, el campo solo poseerá componente radial.
Además, la carga encerrada estará determinada por una integral triple en cilíndricas:

RRR

I
Er>R ·

V ρ dV

dS =

ε0

Como la densidad de carga lineal del cilindro no es uniforme,
no se puede tratar como una constante y es necesario integrar.
Ahora, la integral cerrada es en verdad la superficie del manto del
cilindro, pues el flujo es ortogonal a este en todo momento:

RRR
Er>R · 2πrh =

V ρ dV

ε0

La integral de volumen se refiere al volumen encerrado
por el cilindro gaussiano de altura = h” y radio = r”.
En este caso, sería todo el volumen del cilindro con carga:

R h R 2π R R r
Er>R · 2πrh =
Er>R · 2πrh =

0 a · r drdθdz

ε0
h · 2π · R
3a

ε0
R3
Er>R =
3aε0 r

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

Er>R =

R3
r̂
3aε0 r

(10)

---

### Página 13

Solución c)
Paso Único: Campo Eléctrico - Gráfico
Para realizar el gráfico solo se debe observar la parte variable (en este caso r) del módulo del
campo en cada uno de los intervalos y asociarlos a una gráfica conocida, además de evaluar (si
es que necesario) sus valores límite. De esta manera:
Intervalo Campo

Relación Valor Campo

Tipo Función

|Er<R |

r2
3aε0 ∝ r

Función Cuadrática

|Er>R |

R3
3aε0 r ∝ r

Función Racional Básica

Un bosquejo de la gráfica se muestra a continuación:

Figura 3. Gráfico sobre el módulo del campo eléctrico en función del radio.
Se debe notar que el campo eléctrico es continuo en r = R, pero no derivable debido a
la inexistencia del límite en tal punto. Gráficamente, esto podría verse como una = punta”.

---

### Página 14

2.3.3

“Ejercicios Teoría Electromagnética ”, 4.1.5, Fabián Cádiz

Considere dos esferas no concéntricas de radio R. La primera de ellas lleva una densidad
volumétrica de carga ρ y la segunda −ρ. Los centros de las esferas están a distancia
menor que 2R. Si d⃗ es el vector que va del centro de la esfera positiva al centro de la
negativa, demuestre que el campo eléctrico en la intersección de las esferas es constante
y encuentre su valor.

Figura 4. Esquema sobre las esferas.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en la intersección de las esferas. Como se está hablando
de una esfera, es posible aplicar Ley de Gauss utilizando una esfera concéntrica de radio = r”
arbitrario:
I
Qenc
E · ds =
ϵ0
S
No se entrega explícitamente la carga contenida en ambos cuerpos,
por lo que se tendrá que utilizar la definición de carga:

ZZZ
Q=

ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: r < R y r > R.
Finalmente, se deberá superponer ambos campos eléctricos.

---

### Página 15

Paso 1: Ley de Gauss - Er<R
Como la intersección entre las esferas se encuentra en la región r− , r+ < R de cada una de
ellas, solo se calculará el campo eléctrico en tal región para una esfera de densidad ρ:
I
Qenc
Er<R · ds =
ε0
Como es una esfera, el campo solo poseerá componente radial.
Además, la carga encerrada estará determinada por una integral triple en esféricas:

RRR

V ρ dV

I
Er<R ·

dS =

ε0

Como la densidad de carga de la esfera es uniforme,
se puede tratar como una constante y sale de la integral.
Ahora, la integral cerrada es en verdad la superficie de la esfera,
pues el flujo es ortogonal a esta en todo momento:

Er<R · 4πr =

ρ·

RRR

V dV

ε0

La integral de volumen se refiere al volumen
encerrado por la esfera gaussiana de radio = r”.
En este caso, sería parte del volumen de la esfera con carga:

R 2π R π R r
ρ · 0 0 0 r2 sin θ drdθdϕ
Er<R · 4πr =
ε0

Er<R · 4πr2 =

ρ · 2π · 2 · r3
ε0

ρ · 4πr
ε0
ρr
Er<R =
3ε0

Er<R · 4πr2 =

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

Eρ,r<R =

ρr
r̂
3ε0

(11)

Asimismo, el campo eléctrico en la región r < R para una esfera de densidad −ρ es:

E−ρ,r<R =

−ρr
r̂
3ε0

(12)

---

### Página 16

Paso 2: Principio de Superposición - Er+ ,r− <R
Se recuerda que el campo de cada una de las esferas se origina desde su propio centro, por
lo que sus sistemas de referencias serán distintos. Luego, y antes de realizar la superposición
de los campos, es necesario expresarlos en un mismo sistema de referencia. Utilizando como
nuevo origen el centro de la esfera de densidad −ρ, se puede reescribir ⃗r+ en términos de ⃗r− y
⃗
d:
Er+ ,r− <R = Eρ,r+ <R + E−ρ,r− <R
ρ
−ρ
=
⃗r+ +
⃗r−
3ε0
3ε0
ρ
⃗ + −ρ ⃗r−
=
(⃗r− + d)
3ε0
3ε0
ρ ⃗
=
d
3ε0

(13)

Figura 5. Esquema sobre el cambio de sistema de referencia.
Nota: El cambio de sistema de referencia también se puede realizar utilizando como
⃗
origen el centro de la esfera de densidad ρ y reescribiendo ⃗r− en términos de ⃗r+ y d.
