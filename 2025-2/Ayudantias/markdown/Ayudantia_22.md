---
title: "Ayudantia 22"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_22_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_22_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 22

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 22
#### Problema 1
Un cable coaxial muy largo consiste en un cilindro sólido con un radio interior de radio a,
rodeado por un cascarón cilíndrico conductor concéntrico de radio interno b y exterior c. El
conductor interior tiene una densidad de corriente no uniforme J⃗1 = αrẑ donde α es una
constante. El cilindro exterior tiene una densidad de corriente J⃗2 = −β ẑ donde β es una
constante positiva. Los conductores llevan una igual y opuesta corriente de magnitud I0 .
Entre ambos conductores existe vacío.
a) Encuentre los valores de α y β en términos de a, b, c y I0 .
b) Determine el campo magnético en todo el espacio.

---

### Página 2

#### Problema 2
Sobre el plano xy se encuentra una moneda magnetizada muy pequeña de radio R y espesor
d. Experimentalmente sólo se conoce la componente axial del campo magnético dentro de la
moneda, dado por
Bz = B0 (1 + κz 2 )
donde κ es una constante. Suponiendo que el campo magnético posee simetría axial y no posee
componente en θ̂, determine la intensidad de corriente que circula dentro de la moneda.

#### Problema 3
Suponga que tiene dos cables infinitamente largos con densidad lineal de carga λ, separados
por una distancia d, moviéndose a velocidad v constante. Encuentre el valor de v para que
la atracción magnética se compense con la repulsión eléctrica. ¿Es razonable este resultado?

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 22
#### Problema 1
Un cable coaxial muy largo consiste en un cilindro sólido con un radio interior de radio a,
rodeado por un cascarón cilíndrico conductor concéntrico de radio interno b y exterior c. El
conductor interior tiene una densidad de corriente no uniforme J⃗1 = αrẑ donde α es una
constante. El cilindro exterior tiene una densidad de corriente J⃗2 = −β ẑ donde β es una
constante positiva. Los conductores llevan una igual y opuesta corriente de magnitud I0 .
Entre ambos conductores existe vacío.
a) Encuentre los valores de α y β en términos de a, b, c y I0 .
b) Determine el campo magnético en todo el espacio.

---

### Página 2

#### SOLUCION:
a) Usando la definición de corriente eléctrica a partir de la densidad de corriente, se obtiene
que
Z
I0 =

⃗=
J⃗1 · dS

Z 2π Z a
αrẑ · rdrdθẑ =

S

2παa3

3I0
⇒α=
Z
Z 2π Z c 2πa

⃗=
−I0 =
J⃗2 · dS
−β ẑ · rdrdθẑ = −βπ c2 − b2
S

b

⇒β=

I0
π (c − b2 )

b) Por otro lado, el campo magnético es por ley de Ampere, la cual nos dice que
I
⃗ · d⃗r = µ0 Ienc
C

⃗ = B θ̂ y por tanto:
En nuestro caso, por la simetría axial del problema, B
r<a:
Z 2π Z r
B(r) · 2πr = µ0

αrẑ · rdrdθẑ = µ0

⃗ =
⇒B

2π 3
αr

µ0 I0 r2
θ̂
2πa3

a<r<b:
Z 2π Z a
B(r) · 2πr = µ0

αrẑ · rdrdθẑ = µ0 I0

⃗ =
⇒B

µ0 I0
θ̂
2πr

b<r<c:
Z 2π Z r
B(r) · 2πr = µ0 I0 − µ0
⃗ =
⇒B

β ẑ · rdrdθẑ

b

µ0 I0 c − r
θ̂
2πr c2 − b2

r>c:
B(r) · 2πr = I0 − I0 = 0
⃗ =0
⇒B

---

### Página 3

#### Problema 2
Sobre el plano xy se encuentra una moneda magnetizada muy pequeña de radio R y espesor
d. Experimentalmente sólo se conoce la componente axial del campo magnético dentro de la
moneda, dado por
Bz = B0 (1 + κz 2 )
donde κ es una constante. Suponiendo que el campo magnético posee simetría axial y no posee
componente en θ̂, determine la intensidad de corriente que circula dentro de la moneda.

#### SOLUCION:
Como el problema no depende de la componente según θ̂, se puede deducir que el campo
magnético es de la forma
⃗ z) = Br (r, z)r̂ + Bz (r, z)ẑ
B(r,
⃗ ·B
⃗ = 0, esto implica que
Esto es básicamente debido adicionalmente debe cumplirse que ∇
el flujo en cualquier superficie cerrada siempre es nulo. Usando lo anterior, por en enunciado
se sabe que Bz (r, z) = B0 (1 + κz 2 ), por lo que tomando un cilindro pequeño de radio r y
altura z dentro de la moneda se tiene que
ΦCilindro = Φ1 + Φ2 + Φ3
Donde Φ1 y Φ2 son los flujos sobre las tapas superior e inferior respectivamente, y Φ3 el flujo
sobre el manto. Ahora de acuerdo a la Ley de Gauss magnética se debe tener que
ZZ
⃗
⃗
⃗ · dS
⃗=0
∇ · B = 0 =⇒ ΦCilindro =
S

Determinando los flujos por separado se tiene

Z 2π Z r

Z 2π Z r

⃗ 0) · dS
⃗=
Φ1 =
B(r,
B0 ẑ · rdrdθ(−ẑ) = −B0 πr2
Z 2π Z r 0
Z 2π Z r 0


⃗ z) · dS
⃗=
Φ2 =
B(r,
B0 1 + κz 2 ẑ · rdrdθẑ = B0 1 + κz 2 πr2

---

### Página 4

Por lo que Φ1 + Φ2 + Φ3 = 0 =⇒ Φ3 = − (Φ1 + Φ2 ) = −B0 πr2 κz 2 , pero por otro lado
Z z
Z z Z 2π
⃗
Br (r, z)dz = −B0 πr2 κz 2
B(r, z) · rdθdzr̂ = 2πr
Φ3 =


1 d
⇒ Br (r, z) =
−B0 πr2 κz 2
2πr dz
⇒ Br (r, z) = −B0 rκz
entonces el campo magnético vale

⃗ = −B0 rκzr̂ + B0 1 + κz 2 ẑ
Finalmente para determinar la corriente
⃗ ×B
⃗ = µ0 J⃗
∇
1 ⃗
⃗ = − B0 κr θ̂
⇒ J⃗ = ∇
×B
µ0
µ0
Z dZ R
B0 κr
B0 κdR2
−
⇒I=
θ̂ · drdz θ̂ = −
µ0
2µ0

---

### Página 5

#### Problema 3
Suponga que tiene dos cables infinitamente largos con densidad lineal de carga λ, separados
por una distancia d, moviéndose a velocidad v constante. Encuentre el valor de v para que
la atracción magnética se compense con la repulsión eléctrica. ¿Es razonable este resultado?

#### SOLUCION:
El campo eléctrico generado por el cable izquierdo sobre el cable derecho está dado por
⃗ =
E

λ
ŷ
2πϵ0 d

De esta forma, la fuerza eléctrica por unidad de largo será
F⃗Le = λ

λ2
λ
ŷ =
ŷ
2πϵ0 d
2πϵ0 d

Por otro lado, los alambres en movimiento equivalen a una corriente
I=

λdx
dq
=
= λv
dt
dt

El campo magnético generado por el cable izquierdo sobre el derecho es
⃗ = − µ0 I ẑ = − µ0 λv ẑ
2πd
2πd
En este caso, la fuerza magnética por unidad de largo sobre el cable derecho será


µ0 λv
m
⃗
FL = −I x̂ × −
ẑ
2πd
µ0 λ2 v 2
F⃗Lm = −
ŷ
2πd

---

### Página 6

Para que éstas fuerzas se anulen
F⃗Le + F⃗Lm = 0
µ0 λ2 v 2
λ2
=
2πϵ0 d
2πd
= µ0 v 2
ϵ0
La velocidad debe ser

Evaluando

v=√
µ0 ϵ0
v=p
= 3 × 108
−12
−7
8, 85 × 10
× 4π10

Esta es la velocidad de la luz en el vacío, por lo que el resultado no es razonable y debemos
considerar física adicional.
