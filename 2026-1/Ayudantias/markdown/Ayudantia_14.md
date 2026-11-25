---
title: "Ayudantia 14"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_14.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_14_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 14

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 12
Corriente Eléctrica

#### Problema 1
Dos esferas metálicas de radio a y b están separadas por un medio de conductividad σ constante.

(a) Si estas esferas fueran mantenidas a una diferencia de potencial V constante, encuentre la
corriente que va de una a la otra. (Asuma un camino radial para la corriente)
(b) Encuentre la resistencia entre las esferas.
#### Problema 2
Considere un condensador de placas conductoras perfectas, planas, paralelas y de área A. El espacio interno entre las placas se llena con dos bloques de materiales distintos cuyas permitividades
y conductividades valen respectivamente pε1 , g1 q y pε2 , g2 q, tal como se muestra en la figura. El
espesor del primer material es d1 y el del segundo es d2 (ver figura). El valor de la diferencia de
potencial entre los extremos del sistema es V0 .

---

### Página 2

⃗ en el sistema.
(a) Determine los vectores de densidad de corriente J⃗ y de campo eléctrico E
(b) Determine los valores de las cargas ligadas donde corresponda.
(c) Determine la capacitancia equivalente, Ceq , del sistema y la carga libre, donde corresponda.
(d) Determine la resistencia equivalente, R, y la corriente que fluye por el sistema.
#### Problema 3
Suponga que se construye una cuña (figura abajo izquierda) usando material de resistividad ρ.
Determine la resistencia del cuerpo entre las caras A y B mostradas en la figura. Repita para el
cono truncado mostrado abajo a la derecha. El material es el mismo que en el primer resistor.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 12
Corriente Eléctrica

#### Problema 1
Dos esferas metálicas de radio a y b están separadas por un medio de conductividad σ constante.

(a) Si estas esferas fueran mantenidas a una diferencia de potencial V constante, encuentre la
corriente que va de una a la otra. (Asuma un camino radial para la corriente)
(b) Encuentre la resistencia entre las esferas.

#### Solución
Pensemos primero en que queremos obtener, necesitamos obtener una corriente I, una forma de
hacerlo sin conocer la resistenca, como en este caso, es utilizando una densidad de corriente J⃗ que
sabemos que cumple con,
⃗
J⃗ = σ E
⃗ el campo eléctrico en la región,
Donde σ representa la conductividad y E

---

### Página 2

Entonces queremos obtener el campo eléctrico, pero no conocemos la carga, pero tenemos información que nos sirve para determinarla, la diferencia de potencial. Al existir una diferencia de
potencial V entre las esferas, se inducen cargas Q y ´Q en cada una.
Para obtener el campo eléctrico en la región entre las esferas utilizamos ley de gauss,
ż

⃗ ¨ dS
⃗“ Q
E
ε0

⃗ “
E

Ñ

Q
r̂
4πr2 ε0

No conocemos la carga Q como tal, pero podemos obtenerla a partir de calcular la diferencia de
potencial, integrando el campo eléctrico por medio de un camino radial entre r = a y r = b ya que
sabemos que debe dar como resultado V , es decir,
ża

⃗ ¨ d⃗r = Q
V = ´
E
4πε0
b

ˆ

1 1
´
a b

˙

Esto de acá nos permite obtener la carga en función de parámetros conocidos como,
Q“

4πε0 abV
b´a

Con esto ya tenemos el ejercicio practicamente hecho, como conocemos la carga, conocemos el
campo eléctrico,
⃗ “
E

V ab
r̂
pb ´ aqr2

Con esto tenemos que la densidad de corriente es,
⃗ = σE
⃗ “
J(r)

σV ab
r̂
pb ´ aqr2

La corriente la obtenemos de integrar esta densidad de corriente en una superficie esférica con
a < r < b como,
ĳ
I“

⃗ = 4πσV ab
J⃗n̂dA = 4πr2 J(r)
pb ´ aq

S

Para la resistencia, el procedimiento es bastante directo, conocemos la corriente y el la diferencia
de potencial entre los terminales, utlizando ley de ohm macroscópica,
V
“
R“
I
4πε0

ˆ

1 1
´
a b

˙

---

### Página 3

#### Problema 2
Considere un condensador de placas conductoras perfectas, planas, paralelas y de área A. El espacio interno entre las placas se llena con dos bloques de materiales distintos cuyas permitividades
y conductividades valen respectivamente pε1 , g1 q y pε2 , g2 q, tal como se muestra en la figura. El
espesor del primer material es d1 y el del segundo es d2 (ver figura). El valor de la diferencia de
potencial entre los extremos del sistema es V0 .

⃗ en el sistema.
(a) Determine los vectores de densidad de corriente J⃗ y de campo eléctrico E
(b) Determine los valores de las cargas ligadas donde corresponda.
(c) Determine la capacitancia equivalente, Ceq , del sistema y la carga libre, donde corresponda.
(d) Determine la resistencia equivalente, R, y la corriente que fluye por el sistema.

#### Solución
La diferencia de potencial suministrada por la bateria debe ser igual al potencial entre los terminales del condensador, como el campo eléctrico de placas paralelas es constante entre las placas, el
potencial se calcula facilmente,
V0 = V1 ` V2 = E1 d1 ` E2 d2

(1)

⃗
Además por ley de ohm (J⃗ = g E).
V0 “

J
J
d1 ` d2
g1
g2

(2)

En este caso las densidades de corriente son iguales, ya que las secciones transversales y la corriente
total es la misma, con esto obtenemos que,

---

### Página 4

J“

g1 g2 V0
g1 d2 ` g2 d1

y utilizando nuevamente ley de Ohm obtenemos los campos eléctrico,
g2 V0
⃗ 1 = E1 p´ẑq = J p´ẑq = 
p´ẑq
E
g1
g1 d2 ` g2 d1
g1 V0
⃗ 2 = E2 p´ẑq = J p´ẑq = 
E
p´ẑq
g2
g1 d2 ` g2 d1
Para la b partimos de la definición de vector desplazamiento
⃗ 1 = ε1 E
⃗ 1 = ε0 E
⃗ 1 ` P⃗1
D
con
⃗1
P⃗1 = ε0 χ1 E
Sustituyendo P⃗1 en la expresión del desplazamiento eléctrico:
⃗ 1 = ε0 E
⃗ 1 ` ε 0 χ1 E
⃗1
ε1 E
Factorizando:
ε1 = ε0 p1 ` χ1 q
De donde:
χ1 “

ε1 ´ ε 0
ε0

Entonces la polarización queda:
⃗ 1 = pε1 - ε0 qE1 p´ẑq
P⃗1 = pε1 - ε0 qE
De forma análoga para el segundo medio:
⃗ 2 = pε2 - ε0 qE2 p´ẑq
P⃗2 = pε2 - ε0 qE
Finalmente, la densidad de carga ligada superficial se define como:
σb = P⃗ ¨ n̂
En z = 0:

(3)

---

### Página 5

σb (0) = P⃗1 ¨ n̂1 = pε1 - ε0 qE1 p´ẑq ¨ p´ẑq = pε1 - ε0 qE1
En z = d1 ` d2 :
σb pd1 ` d2 q = P⃗2 ¨ n̂2 = pε2 - ε0 qE2 p´ẑq ¨ ẑ = -pε2 - ε0 qE2
Usando la ley de Gauss para dieléctricos se tiene que en la placa positiva se cumple que
QL = ε2 E2 A
donde QL > 0 es la carga libre en el conductor. De la misma forma para la placa negativa, se
cumple que
QL = ε1 E1 A.
Sustituyendo en la ecuación de potenciales se tiene
V0 = E1 d1 ` E2 d2 = 

QL
QL
d1 `
d2
ε1 A
ε2 A

Factorizando y teniendo en cuenta que Ceq = QL {V0 , se tiene que
Ceq “

QL
ε1 ε2 A
“
V0
ε1 d 2 ` ε 2 d 1

y
QL “

ε1 ε2 AV0
ε1 d 2 ` ε 2 d 1

La corriente eléctrica, en términos de la densidad de corriente, se define como
I = JA = 

g1 g2 A
V0
g1 d2 ` g2 d1

por tanto
R“

V0
d1
d2
“
`
I
g1 A g2 A

---

### Página 6

#### Problema 3
Suponga que se construye una cuña (figura abajo izquierda) usando material de resistividad ρ.
Determine la resistencia del cuerpo entre las caras A y B mostradas en la figura. Repita para el
cono truncado mostrado abajo a la derecha. El material es el mismo que en el primer resistor.

#### Solución
La resistividad de estas geometrías se calculan a partir del área transversal siguiendo la forma,
dR “

ρpxqdx
A(x)

(4)

Entonces necesitamos encontrar el área de un pedacito dx visto de frente, es decir de la siguiente
forma,

donde la profunidad es d por lo que el área de una sección transversal de ancho dx es,
ˆ
A(x) = hpxqd = 

˙
b
a` x d
L

(5)

---

### Página 7

reemplazando en la ecuación para R,
żL

ˆ
˙
ρ
ρL
b
dx “
ln 1 `
R“
b
bd
a
0 a ` Lx

(6)

Para el caso del cono truncado es exactamente lo mismo, tomamos una sección transversal donde
el área corresponde al área de un círculo (Recordar sólido de revolución de C1),

en este caso, para un pedacito de dx, el área de la sección transversal es,
ˆ

b
A(x) = πr (x) = π a ` x
h

˙2

(7)

Con esto la resistencia, de esta configuración es,
żh

ρdx

ρh
R“
dx “
`
˘
b
bπ
0 π a` x
h

(9)

ˆ

´
a a`b

˙
(8)
