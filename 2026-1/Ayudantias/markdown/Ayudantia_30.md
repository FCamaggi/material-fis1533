---
title: "Ayudantia 30"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_30.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_30_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 30

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 28
Repaso examen

#### Problema 1
Una barra conductora de masa m y resistencia R es empujada en la dirección horizontal a través
de dos rieles sin fricción apartados una distancia l, mediante un hilo de masa despreciable que pasa
a través de una polea ideal y que está conectada a un bloque de masa M . Un campo magnético
uniforme es aplicado verticalmente hacia arriba. La barra parte del reposo.

a) Sea la velocidad de la barra en algún instante igual a v. Encuentre una expresión para la
corriente inducida. ¿En qué dirección fluye, de a hacia b o de b hacia a?
b) Resuelva la ecuación diferencial para la velocidad de la barra en función del tiempo.
#### Problema 2
Una espira conductora, plana y circular, de radio R se encuentra en reposo en un campo magnético
⃗ cuya dirección forma un ángulo θ con el plano de la espira, tal como se muestra en la
uniforme B,
figura. El campo magnético varía con el tiempo de acuerdo con
B = B0 e´αt .

---

### Página 2

(a) Calcule la magnitud de la fem inducida en función del tiempo.
(b) Determine el instante en que la fem inducida es igual a 1{10 de su valor inicial.
(c) Determine si la dirección de la corriente inducida en la espira va a favor o en contra del
movimiento de las manecillas del reloj al observar la espira desde arriba (punto O).
#### Problema 3
Considere los siguientes alambres, todos ubicados en el plano xy. El primero es un alambre recto
e infinito en x = 0 y z = 0. Este alambre lleva una corriente I > 0 en la dirección `ŷ. El segundo
alambre también es recto e infinito, está en x = L y z = 0, y lleva una corriente I en la dirección
opuesta ´ŷ. A una distancia d del segundo alambre hay una espira cuadrada de lado a, cuyos
vértices están en:
(1) x = L ` d, y = 0, z = 0,

(2) x = L ` d ` a, y = 0, z = 0,

(3) x = L ` d ` a, y = a, z = 0,

(4) x = L ` d, y = a, z = 0.

La corriente I varía en el tiempo, es decir, I9 ‰ 0, de una forma no especificada.
Calcule la f.e.m. inducida en la espira y su inductancia. Indique el sentido de la corriente inducida en la espira para los casos en que la corriente I disminuye con el tiempo y aumenta con el tiempo.

#### Problema 4
Un circuito tiene dos resistencias R1 y R2 , un condensador C y una inductancia L dispuestas de la
forma que se indica en la figura. El circuito es alimentado mediante una fuente de voltaje alterno
de ecuación V (t) = V0 sin ωt. Determine:
a) La impedancia equivalente del circuito y el módulo de la corriente en función del tiempo por
cada rama del circuito.
b) La frecuencia de resonancia del circuito, ¿Cuál es el valor de la corriente máxima que sale
de la fuente? (exprese su resultado en función de la frecuencia de resonancia).

---

### Página 3

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 28
Repaso examen

#### Problema 1
Una barra conductora de masa m y resistencia R es empujada en la dirección horizontal a través
de dos rieles sin fricción apartados una distancia l, mediante un hilo de masa despreciable que pasa
a través de una polea ideal y que está conectada a un bloque de masa M . Un campo magnético
uniforme es aplicado verticalmente hacia arriba. La barra parte del reposo.

a) Sea la velocidad de la barra en algún instante igual a v. Encuentre una expresión para la
corriente inducida. ¿En qué dirección fluye, de a hacia b o de b hacia a?
b) Resuelva la ecuación diferencial para la velocidad de la barra en función del tiempo.

#### Solución
EL flujo es bastante directo de calcular, el camino que recorre la corriente inducida es un rectángulo
de lado l constante y x que varía según v. De esta forma el flujo se calcula como,
ż
ΦB “

⃗ ¨ dA
⃗ = BA = Bxl
B

Utilizando la ley de Faraday obtenemos la f.e.m inducida como,

---

### Página 2

dΦB
“ -Blv
dt
y con la ley de ohm obtenemos la corriente inducida,
ε = ´

I“

|ε|
Blv
“
R
R

Para definir el sentido de la corriente pensamos en el movimiento natural del conductor, este va a
incrementar el valor de x, incrementando directamenre el flujo magnético; por lo que la corriente
inducida quiere oponerse a este aumento generando un campo magnético que se oponga al existente, esto se logra solo si la corriente inducida va de b hacia a.
Para obtener la velocidad partimos de las ecuaciones de movimiente de la segunda ley de newton,
recordando que la fuerza que siente un conductor en un campo magnétivo viene dado por F⃗ “
⃗
I⃗l ˆ B,
ÿ

⃗ = T î - I ĵ ˆ B k̂ = pT - IlBqî = m d x î
F⃗ = T î - I⃗ ˆ B
dt2

Para la masa M la ecuación es mas sencilla,
d2 y
dt2
Existe una ligadura en este problema que viene dada por la cuerda, la condición que esta impone
es que ambas aceleraciones son iguales, por lo que esta última ecuación la podemos escribir como,
Mg - T = M

T = Mg - M

d2 x
dt2

Reemplazando esta definición de T en la ecuación para la masa M ,

d2 x
M g ´ M 2 ´ IlB
dt

˙
“m

d2 x
dt2

Reemplazando ahora la definición de I obtenida en el inciso anterior y juntando terminos obtenemos,
Mg ´

l2 B 2
d2 x
v = pm ` M q 2
R
dt

Esta ecuación es de primer orden en v ya que recordemos que v = dx{dt. Reemplazando por dicha
definición y ordenando obtenemos,
dv
l2 B 2
Mg
`
v´
“0
dt RpM ` mq
M `m

---

### Página 3

Esta ecuación es lineal de primer orden y puede escribirse en la forma estándar:
dv
` P v = Q,
dt
donde:
l2 B 2
Mg
P “
, Q“
.
RpM ` mq
M `m
Primero resolvemos la ecuación homogénea asociada, obtenida al hacer Q = 0:
dv
` P v = 0.
dt
Reescribiendo:
dv
“ -P dt.
v
Integrando ambos lados:
ln |v| = -P t ` C,
donde C es la constante de integración. Elevando a la exponencial:
vh (t) = Ce´P t .
Sustituyendo el valor de P :
l2 B 2

vh (t) = Ce´ RpM `mq t .
Para obtener una solución particular, suponemos vp = A, donde A es una constante. Sustituyendo
en la ecuación original:
P A = Q.
Resolviendo para A:
Mg

M gR
Q
“ Ml2`m
“ 2 2.
A“
B
P
l B
RpM `mq
La solución general de la ecuación es la suma de la solución homogénea y la solución particular:
l2 B 2
M gR
v(t) = vh (t) ` vp = Ce´ RpM `mq t ` 2 2 .
l B
Usando la condición inicial v(0) = 0, tenemos:
M gR
v(0) = C ` 2 2 .
l B
Resolviendo para C:
M gR
C = - 2 2.
l B
Sustituyendo C en la solución general:
l2 B 2
M gR
M gR
v(t) = - 2 2 e´ RpM `mq t ` 2 2 .
l B
l B
Simplificando:
˙
l2 B 2
M gR
´ RpM
t
`mq
v(t) = 2 2 1 - e
l B

---

### Página 4

#### Problema 2
Una espira conductora, plana y circular, de radio R se encuentra en reposo en un campo magnético
⃗ cuya dirección forma un ángulo θ con el plano de la espira, tal como se muestra en la
uniforme B,
figura. El campo magnético varía con el tiempo de acuerdo con
B = B0 e´αt .

(a) Calcule la magnitud de la fem inducida en función del tiempo.
(b) Determine el instante en que la fem inducida es igual a 1{10 de su valor inicial.
(c) Determine si la dirección de la corriente inducida en la espira va a favor o en contra del
movimiento de las manecillas del reloj al observar la espira desde arriba (punto O).

#### Solución
Para calcular la FEM inducida, primero necesitamos calcular el flujo magnético a través de la
espira. Tomamos como normal positiva a la superficie la dirección que apunta hacia el observador
O.
El campo magnético forma un ángulo θ con el plano de la espira, por lo que la componente perpendicular al área de la espira es
BK = B sin θ.

(1)

A = πR2 ,

(2)

Como el área de la espira circular es

el flujo magnético es
ż
Φ“

⃗ ¨ dA
⃗ = BK A = BA sin θ.
B

Usando que el campo magnético varía en el tiempo según

(3)

---

### Página 5

B(t) = B0 e´αt ,

(4)

Φ(t) = B0 e´αt πR2 sin θ.

(5)

se obtiene

Lo que varía en el tiempo en este caso es la magnitud del campo magnético debido a la exponencial.
Por la ley de Faraday, la FEM inducida es
dΦ
.
dt

(6)

˘
d `
B0 e´αt πR2 sin θ .
dt

(7)

E = ´
Entonces,
E = ´
Derivando,

E = αB0 e´αt πR2 sin θ.

(8)

E(t) = αB0 e´αt πR2 sin θ .

(9)

Por lo tanto,

Ahora buscamos el tiempo t1 para el cual la FEM inducida vale un décimo de su valor inicial, es
decir,
Ept1 q “

Ep0q.

(10)

Como
E(0) = αB0 πR2 sin θ,

(11)

y

E(t1 ) = αB0 e´αt πR2 sin θ,

(12)

tenemos

αB0 e´αt πR2 sin θ “
Cancelando los factores comunes,

αB0 πR2 sin θ.

(13)

---

### Página 6

e´αt “

.

(14)

Aplicando logaritmo natural,

˙
.

(15)

“ - ln 10,

(16)

ln 10
.
α

(17)

´αt = ln
Como
ln

˙

se obtiene finalmente
t1 “

Para determinar el sentido de la corriente inducida, usamos la ley de Lenz. En la figura, la componente perpendicular del campo magnético apunta hacia el observador O. Además, como
B(t) = B0 e´αt ,

(18)

la magnitud del campo magnético disminuye con el tiempo. Por lo tanto, el flujo magnético hacia
el observador O también disminuye.
La corriente inducida aparece de manera que se opone a esta disminución del flujo. Entonces, la
espira debe generar un campo magnético inducido también hacia el observador O.
Por la regla de la mano derecha, para que el campo magnético producido por una corriente circular
apunte hacia el observador O, la corriente debe circular en sentido antihorario al mirar la espira
desde arriba.
Por lo tanto,
la corriente inducida circula en sentido antihorario vista desde O.

(19)

#### Problema 3
Considere los siguientes alambres, todos ubicados en el plano xy. El primero es un alambre recto
e infinito en x = 0 y z = 0. Este alambre lleva una corriente I > 0 en la dirección `ŷ. El segundo
alambre también es recto e infinito, está en x = L y z = 0, y lleva una corriente I en la dirección
opuesta ´ŷ. A una distancia d del segundo alambre hay una espira cuadrada de lado a, cuyos
vértices están en:
(1) x = L ` d, y = 0, z = 0,

(2) x = L ` d ` a, y = 0, z = 0,

---

### Página 7

(3) x = L ` d ` a, y = a, z = 0,

(4) x = L ` d, y = a, z = 0.

La corriente I varía en el tiempo, es decir, I9 ‰ 0, de una forma no especificada.
Calcule la f.e.m. inducida en la espira y su inductancia. Indique el sentido de la corriente inducida en la espira para los casos en que la corriente I disminuye con el tiempo y aumenta con el tiempo.

#### Solución
Elegimos como normal positiva de la espira la dirección `ẑ. Con esta elección, el sentido positivo
de circulación en la espira es antihorario visto desde `ẑ, es decir, siguiendo los vértices
p1q Ñ p2q Ñ p3q Ñ p4q Ñ p1q.
Los dos alambres son infinitos y paralelos al eje y. El campo magnético producido por un alambre
recto infinito a una distancia perpendicular r es
B“

µ0 I
.
2πr

Primero analicemos la dirección del campo magnético en la región donde se encuentra la espira, es
decir, para x > L ` d.
El alambre ubicado en x = 0 lleva corriente en la dirección `ŷ. Usando la regla de la mano derecha,
en la zona x > 0 su campo magnético apunta en la dirección ´ẑ. Por lo tanto,
⃗ 1 (x) = - µ0 I ẑ.
B
2πx
El segundo alambre está en x = L y lleva corriente en la dirección opuesta, es decir, en ´ŷ. En la
región a la derecha de este alambre, x > L, su campo magnético apunta en la dirección `ẑ. Por
tanto,
µ0 I
⃗ 2 (x) = 
B
ẑ.
2πpx ´ Lq
Entonces, el campo magnético total sobre la espira es
⃗
⃗ 1 (x) ` B
⃗ 2 (x),
B(x)
“B
es decir,

„
ȷ
µ0 I
⃗
ẑ.
B(x) = 
´
2π x ´ L x

Como la espira está a la derecha del segundo alambre, se cumple x > L. Además,
> ,
x´L
x
por lo que el campo magnético neto atraviesa la espira en la dirección `ẑ.

---

### Página 8

El flujo magnético a través de la espira es
ż
⃗ ¨ dA.
⃗
B

ΦB “
Como la espira está en el plano xy, tenemos

⃗ = dx dy ẑ.
dA
Los límites de integración son
L ` d ď x ď L ` d ` a,
y
0 ď y ď a.
Por lo tanto,
ż a ż L`d`a
ΦB “

L`d

„
ȷ
µ0 I
dx dy.
´
2π x ´ L x

Como el campo no depende de y, la integral en y entrega simplemente un factor a:
„
ȷ
ż
µ0 Ia L`d`a
ΦB “
dx.
´
2π L`d
x´L x
Ahora integramos:
ż „

ȷ
´
dx = lnpx - Lq - ln x.
x´L x

Entonces,
ΦB “

µ0 Ia
rlnpx ´ Lq ´ ln xsL`d`a
.
L`d
2π

Evaluando en los límites:
ΦB “

µ0 Ia
rlnpd ` aq ´ lnpL ` d ` aq ´ ln d ` lnpL ` dqs .
2π

Agrupando los logaritmos,
µ0 Ia
ΦB “
ln
2π

pd ` aqpL ` dq
dpL ` d ` aq

˙
.

Como el flujo es proporcional a la corriente I, podemos escribir
ΦB = M I,
donde M es la inductancia mutua entre el sistema de alambres y la espira. Por tanto,
˙
µ0 a
pd ` aqpL ` dq
M“
ln
.
2π
dpL ` d ` aq

---

### Página 9

Luego, la f.e.m. inducida se obtiene usando la ley de Faraday:
E = ´

dΦB
.
dt

Como M es constante geométrica, tenemos
E = -M

dI
.
dt

Por lo tanto,
µ0 a
ln
E = ´
2π

pd ` aqpL ` dq
dpL ` d ` aq

˙

dI
dt

Esta expresión está escrita tomando como positivo el sentido antihorario visto desde `ẑ.
Sentido de la corriente inducida
El flujo magnético externo atraviesa la espira en la dirección `ẑ. Por la ley de Lenz, la corriente
inducida siempre aparece de forma que se opone al cambio de flujo magnético.
Caso 1: I disminuye con el tiempo
Si I disminuye, entonces
dI
< 0.
dt
Como el flujo externo es proporcional a I, el flujo en dirección `ẑ está disminuyendo. La espira
intenta oponerse a esa disminución, generando un campo magnético inducido también en dirección
`ẑ.
Para que una corriente en la espira produzca un campo en dirección `ẑ, debe circular en sentido
antihorario vista desde `ẑ. Por lo tanto,
si I disminuye, la corriente inducida es antihoraria.
Equivalentemente, como
E = -M

dI
,
dt

< 0, entonces
y M > 0, si dI
dt
E > 0,
lo que corresponde al sentido positivo elegido, es decir, antihorario.

---

### Página 10

Caso 2: I aumenta con el tiempo
Si I aumenta, entonces
dI
> 0.
dt
En este caso, el flujo externo en dirección `ẑ está aumentando. La espira se opone a ese aumento
generando un campo magnético inducido en dirección ´ẑ.
Para que la espira genere un campo en dirección ´ẑ, la corriente inducida debe circular en sentido
horario vista desde `ẑ. Por lo tanto,
si I aumenta, la corriente inducida es horaria.
> 0, entonces
Equivalentemente, si dI
dt
E < 0,
lo que significa que la corriente inducida va en el sentido opuesto al positivo elegido, es decir, en
sentido horario.
#### Problema 4
Un circuito tiene dos resistencias R1 y R2 , un condensador C y una inductancia L dispuestas de la
forma que se indica en la figura. El circuito es alimentado mediante una fuente de voltaje alterno
de ecuación V (t) = V0 sin ωt. Determine:
a) La impedancia equivalente del circuito y el módulo de la corriente en función del tiempo por
cada rama del circuito.
b) La frecuencia de resonancia del circuito, ¿Cuál es el valor de la corriente máxima que sale
de la fuente? (exprese su resultado en función de la frecuencia de resonancia).

#### Solución
a) Sabemos que se tiene un circuito con dos ramas en paralelo:
Rama 1: una resistencia R1 en serie con una inductancia L.

---

### Página 11

Rama 2: una resistencia R2 en serie con un condensador C.
Luego, sabemos que, las impedancias individuales están dadas por definición como:
Inductor: ZL = jωL
“ -j ωC
Condensador: ZC = jωC

Entonces, las impedancias de cada rama son, respectivamente:
Z1 = R1 ` jωL

Z2 = R2 - j

ωC

Así, la impedancia equivalente está dada por (considerando que están en paralelo):
Zeq “

`
Z1 Z2

˙´1

“

`
R1 ` ZL R2 ` ZC

˙´1

. Luego
donde ZL = jXL y ZC = -jXC , con XL = ωL y XC = ωC

“

“

Zeq “

`
R1 ` jXL R2 ´ jXC

“

pR1 ` jXL qpR2 ´ jXC q
pR1 ` R2 q ` jpXL ´ XC q

˙´1

pR1 R2 ` XL XC q ` jpXL R2 ´ XC R1 q
pR1 ` R2 q ` jpXL ´ XC q

rpR1 R2 ` XL XC q ` jpXL R2 ´ XC R1 qsrpR1 ` R2 q ` jpXL ´ XC qs
pR1 ` R2 q2 ` pXL ´ XC q2
“

pR1 R2 ` XL XC qpR1 ` R2 q ´ pXL R2 ´ XC R1 qpXL ´ XC q
pR1 ` R2 q2 ` pXL ´ XC q2

`j

pR1 R2 ` XL XC qpXL ´ XC q ` pXL R2 ´ XC R1 qpR1 ` R2 q
pR1 ` R2 q2 ` pXL ´ XC q2

Luego, utilizando la ley de Ohm fasorial, los módulos de cada una de las corrientes valen:
V̂
Z

I“
ˇ
ˇ
ˇ V0 ejωt ˇ
ˇ = a V0
|I1 (t)| “ ˇˇ
R1 ` jωL ˇ
R2 ` ω 2 L2

ˇ
ˇ
ˇ V0 ejωt ˇ
ˇ b V0
|I2 (t)| “ ˇˇ
1 ˇ “
` 1 ˘2
R1 ´ j ωC
R22 ` ωC

---

### Página 12

Nótese que los módulos de las corrientes son constantes en el tiempo y sólo dependen de los parámetros fijos del circuito. El aporte temporal está dado netamente por la parte exponencial compleja
de la corriente.
b) La frecuencia de resonancia puede ser calculada al hacer nula la parte imaginaria de la impedancia, de modo que:
pR1 R2 ` XL XC qpXL - XC q ` pXL R2 - XC R1 qpR1 ` R2 q = 0
Reemplazando los valores de XL y XC

L
R1 R2 `
C

˙ˆ

´ ω0 L
ω0 C

˙

“

R1
ω0 LR2 ´
ω0 C

˙
pR1 ` R2 q

donde puede despejarse el valor de ω0 como
d
ω0 “ ?
¨
LC

R12 C ´ L
R22 C ´ L

El valor de la corriente para esa frecuencia vale

I“

V
|V0 |
ñ |I| “
“ V0 ¨ `
Zeq
|Zeq |

´

ω0 L ´ ω01C

¯2

pR1 ` R2 q `
¯2
˘2 ´
R1 R2 ` CL ` ω0 LR2 ´ ω01C R1
