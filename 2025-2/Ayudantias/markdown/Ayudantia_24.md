---
title: "Ayudantia 24"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_24_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_24_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 24

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 24
#### Problema 1 (I2 2023-1)
La espira de la figura está formada por 2 segmentos rectos de largo L, uno de largo 2L y otro
semicircular de radio L. Si la espira conduce una corriente total I en la dirección mostrada
⃗ en el punto A (centro del semicírculo).
en la figura, calcule el campo magnético B

---

### Página 2

#### Problema 2 (I2 2022-2)
Un capacitor está formado por dos cilindros conductores concéntricos de largo L y radios a
y c, respectivamente. El espacio entre los cilindros se llena con dos materiales dieléctricos de
permitividad ϵ1 y ϵ2 como se muestra en la figura.

Suponiendo que el capacitor posee carga +Q en el cilindro interior y −Q en el cilindro exterior
y despreciando los efectos de borde, determine:
a) El campo eléctrico y el vector de polarización en la región entre los cilindros conductores.
b) La densidad de carga de polarización σ en cada una de las superficies de los materiales
dieléctricos.
c) La capacitancia del sistema.

#### Problema 3 (I2 2014-2)
Una partícula cargada, de carga q y masa m, parte del reposo en el origen de coordenadas
⃗ paralelo al eje x, y un campo magnetico B
⃗
en una región donde existe un campo eléctrico E
paralelo al eje z. Muestre que las coordenadas de la partícula un instante t más tarde serán:
E
(1 − cos ωt)
ωB
E
y=−
(ωt − sin ωt)
ωB
z=0
x=

donde ω = |q|B
.
m

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 24
#### Problema 1 (I2 2023-1)
La espira de la figura está formada por 2 segmentos rectos de largo L, uno de largo 2L y otro
semicircular de radio L. Si la espira conduce una corriente total I en la dirección mostrada
⃗ en el punto A (centro del semicírculo).
en la figura, calcule el campo magnético B

#### SOLUCION:
De forma cualitativa, a partir de la regla de la mano derecha, podemos notar que el campo
magnético en el punto A posee dirección −ẑ (entrando en la página).
Igual como lo hemos hecho en otras oportunidades, separaremos el problema en 4 zonas
distintas. Es decir, calcularemos el campo producido por la espira semi-circular y los 3 segmentos rectos por separado, para luego obtener el total por principio de superposición. La
ley de Biot-Savart para una densidad lineal de carga, como es una espira, se enuncia como
Z ⃗
⃗
µ
I
dR × (⃗r − R)
⃗
B(r)
=
⃗ 3
4π
|⃗r − R|

---

### Página 2

Por simplicidad, escogemos el origen del sistema de coordenadas en el punto A, de modo que
el campo magnético en ese punto nos queda
µ0 I
B(0)
=
4π

Z

⃗ × (−R)
dR
⃗ 3
|R|

Semi-circunferencia:
⃗ es claramente
En este caso el vector R
⃗ = L(− cos θ x̂ + sin θ ŷ)
R
⇒ |R|3 = L3
⃗ = L(sin θ x̂ + cos θ ŷ)dθ
⇒ dR
Con θ variando entre 0 y π. Reemplazando
Z
µ0 I π −L2 sin2 θ ẑ + L2 cos2 θ (−ẑ)
dθ
B1 (0) =
4π 0
L3
Z
µ0 I π
=−
dθ ẑ
4πL 0
µ0 I
=−
ẑ
4L
Segmentos rectos:
En este punto, debemos calcular los aportes de cada uno de los segmentos por separado,
lo cual nos llevaría a calcular 3 integrales distintas. De forma alternativa, y mucho
más rápida, notemos lo siguiente: Si observamos el semi-cuadrado conformado por los
segmentos rectos, podemos notar que ambos segmentos verticales aportan el mismo
campo sobre A. De igual modo, si dividimos el segmento horizontal en dos mitades
iguales de largo L/2, cada una de ellas contribuye lo mismo que uno de los segmentos
verticales. Entonces, en vez de calcular 3 integrales, podemos calcular el aporte de uno
de los segmentos verticales y multiplicarlo por 4 para así obtener el aporte de todo el
semi-cuadrado.
⃗ resulta
Utilizamos el segmento cuya corriente apunta hacia abajo, de este modo R
⃗ = Lx̂ − y ŷ
R
⇒ |R|3 = (L2 + y 2 )3/2
⃗ = −dy ŷ
⇒ dR
Con y variando entre 0 y L. Reemplazando
Z
µ0 I L −L dy
ẑ
B2 (0) =
4π 0 (L2 + y 2 )3/2

---

### Página 3

Usando el reemplazo y = L tan α → dy = L sec2 α dα, podemos escribir la ecuación
anterior de la forma
Z
L2 sec2 α
µ0 I
dα
B2 (0) = −
4π
(L2 + L2 tan2 α)3/2
Z
L2 sec2 α
µ0 I
=−
dα
4π
(L2 sec2 α)3/2
Z
µ0 I
cos α dα
=−
4πL
µ0 I
[sin α]
=−
4πL
Deshaciendo el cambio con α = arctan(y/L), nos queda
h
 iL
⃗ 2 (0) = − µ0 I sin(arctan y
B
ẑ
4πL
L 0
µ0 I
ẑ
=− √
4 2πL
⃗ □ (0) = 4B
⃗ 2 (0) = − √µ0 I ẑ.
Y en tanto, el campo producto del semi-cuadrado es B
2πL
Finalmente, el campo total en el punto A viene dado por
√ !
µ
I
⃗ 1 (0) + B
⃗ □ (0) = −
B(0)
=B
+
ẑ
2L 2
π

---

### Página 4

#### Problema 2 (I2 2022-2)
Un capacitor está formado por dos cilindros conductores concéntricos de largo L y radios a
y c, respectivamente. El espacio entre los cilindros se llena con dos materiales dieléctricos de
permitividad ϵ1 y ϵ2 como se muestra en la figura.

Suponiendo que el capacitor posee carga +Q en el cilindro interior y −Q en el cilindro exterior
y despreciando los efectos de borde, determine:
a) El campo eléctrico y el vector de polarización en la región entre los cilindros conductores.
b) La densidad de carga de polarización σ en cada una de las superficies de los materiales
dieléctricos.
c) La capacitancia del sistema.
#### SOLUCION:
a) Calcularemos lo que nos piden en distintas regiones del capacitor utilizando la ley de
Gauss en dieléctricos
Z
⃗ · dS
⃗ = qfree
D
S

0 < r < a:
Para esta región, notemos que qfree = 0. Por lo tanto
⃗ =E
⃗ = P⃗ = 0
D
a < r < b:
Ya que nuestra superficie gaussiana encierra el cilindro interior, qfree = +Q y la

---

### Página 5

ley de Gauss nos entrega
Z

⃗ · dS
⃗=Q
D

S

D · 2πrL = Q
⃗ = Q r̂
D
2πrL
⃗ = D/ϵ,
Ya que E
tenemos
⃗ =
E

Q
r̂
2πϵ1 rL

⃗ − ϵ0 E.
⃗ Nos queda
Por definición P⃗ = D
Q(ϵ1 − ϵ0 )
r̂
P⃗ =
2πϵ1 rL
b < r < c: La carga libre encerrada sigue siendo +Q. El procedimiento es análogo
al paso anterior, pero considerando que el dieléctrico tiene constante ϵ2 :
Q
r̂
2πrL
⃗ = Q r̂
E
2πϵ2 rL
Q(ϵ2 − ϵ0 )
P⃗ =
r̂
2πϵ2 rL
⃗ =
D

r > c: La carga libre encerrada es qfree = Q − Q = 0, tal que
⃗ =E
⃗ = P⃗ = 0
D
b) Podemos obtener σ utilizando
σ(r) = P⃗ (r) · n̂
Para el dieléctrico de constante ϵ1 tenemos la superficie interna en r = a y la superficie
externa en r = b. La densidad de polarización σ nos queda
Q(ϵ1 − ϵ0 )
σint = P⃗ (a) · (−r̂) = −
2πϵ1 aL
Q(ϵ
1 − ϵ0 )
σext = P⃗ (b) · (r̂) =
2πϵ1 bL
Para el dieléctrico de constante ϵ2 tenemos la superficie interna en r = b y la superficie
externa en r = c. Nos queda
Q(ϵ2 − ϵ0 )
2πϵ2 bL
Q(ϵ
2 − ϵ0 )
σext = P⃗ (c) · (r̂) =
2πϵ2 cL

σint = P⃗ (b) · (−r̂) = −

---

### Página 6

c) La capacitancia viene dada por
C=

Q
|∆V |

La diferencia de potencial entre los cilindros es
Z c
⃗ · d⃗ℓ
E
∆V = −
a
Z c
Z b
Q
Q
dr −
dr
=−
b 2πϵ2 rL
a 2πϵ1 rL
 
c
Q
b
Q
=−
ln
−
ln
2πϵ1 L
a
2πϵ2 L
b

 



Q
b
c
=−
ln
+ ln
2πL ϵ1
a
ϵ2
b
Por lo tanto, obtenemos que la capacitancia es

 
−1
b
1 c
C = 2πL
ln
+ ln
ϵ1
a
ϵ2
b

---

### Página 7

#### Problema 3 (I2 2014-2)
Una partícula cargada, de carga q y masa m, parte del reposo en el origen de coordenadas
⃗ paralelo al eje x, y un campo magnetico B
en una región donde existe un campo eléctrico E
paralelo al eje z. Muestre que las coordenadas de la partícula un instante t más tarde serán:
E
(1 − cos ωt)
ωB
E
y=−
(ωt − sin ωt)
ωB
z=0
x=

.
donde ω = |q|B
m
#### SOLUCION:
La fuerza que actúa sobre las partículas de carga q en presencia del campo electromagnético
está dada en general por
⃗ + ⃗v × B)
F⃗ = q(E
(1)
en que ⃗v es la velocidad de las partículas. La ecuación de movimiento para una partícula
cargada en presencia de la fuerza de Lorentz, es
m

d⃗v
⃗ + ⃗v × B)
= F⃗ = q(E
dt

(2)

⃗ = E x̂, B
⃗ = B ẑ. Si descomponemos la velocidad de la partícula
En este caso particular E
en coordenadas cartesianas, i.e., ⃗v = vx x̂ + vy ŷ + vz ẑ, podemos calcular las componentes de
⃗ = vy B x̂ − vx B ŷ. Reemplazamos las expresiones para obtener las siguientes ecuaciones
⃗v × B
para las componentes de la velocidad:
dvz
=0
dt
dvx
q
=
(E + vy B)
dt
m
dvy
q
= − vx B
dt
m

(3)
(4)
(5)

Integrando (3) obtenemos vz (t) = c = vz (0) = 0. Ahora derivando la ecuación (5) con respecto
al tiempo y luego utilizando (4) para reemplazar dvx /dt en términos de vy , obtenemos una
ecuación diferencial para vy :
d2 v y
q dvx
=− B
dt
m dt
d vy
q
q2 2
=
−
BE
−
B vy
dt2
m2
m2

---

### Página 8

d2 vy
E
(6)
+ ω 2 vy = −ω 2
dt
B
en que ω = |q|B/m (conocida como la frecuencia de Larmor). La solución general de la
ecuación (6) es:
E
vy (t) = A cos ωt + D sen ωt −
(7)
B
en que A y D son constantes de integración. Derivando (7) con respecto al tiempo y utilizando
(5) encontramos:
vx (t) = A sen ωt − D cos ωt
(8)
Usando las condiciones iniciales para la velocidad determinamos las constantes A y D. Como
vx (0) = vy (0) = 0, obtenemos a partir de (7) y (8) que A = E/B y D = 0. Entonces,
E
dx
= vx (t) = sen ωt
dt
B
dy
E
= vy (t) = (cos ωt − 1)
dt
B
dz
= vz (t) = 0
dt

(9)
(10)
(11)

Integrando (9), (10) y (11), usando las condiciones iniciales x(0) = y(0) = z(0) = 0, finalmente obtenemos,
E
(1 − cos ωt)
ωB
E
(ωt − sen ωt)
y=−
ωB
z=0
x=

que era lo que se pedía demostrar.
Otros ejercicios que han salido en pruebas: 10.2, 10.3, 11.2, 13.1, 13.3, 14.3, 15.1, 20.1
