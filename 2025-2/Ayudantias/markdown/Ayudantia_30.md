---
title: "Ayudantia 30"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_30_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_30_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 30

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 30
#### Problema 1
Considere el siguiente circuito:

a) Encuentre la impedancia equivalente a la derecha de los puntos a y b.
b) Determine el valor de X de modo que la fuente esté en fase con la corriente.
c) ¿Cómo tiene que ser la reactancia X: inductiva o capacitiva? Determine el valor de L
o C según corresponda.

---

### Página 2

#### Problema 2
El circuito de la figura se denomina filtro RC pasa-altos porque transmite con mayor amplitud
las señales de alta frecuencia que las de baja. Si la tensión de entrada es Vin = V0 cos ωt,
demostrar que la de salida es Vout = VR cos(ωt − ϕ), donde
V0
VR = q
2
1 + ωRC
y estudie los casos en que ω ≪ RC
, ω = RC
y ω ≫ RC
.

#### Problema 3
Un circuito tiene 2 resistencias R1 y R2 , un condensador C y una inductancia L dispuestas
de la forma que se indica en la figura. El circuito es alimentado por una fuente de voltaje
altero de ecuación V (t) = V0 sin ωt. Determine la impedancia equivalente del circuito y el
módulo de la corriente en función del tiempo por cada rama del circuito.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 30
#### Problema 1
Considere el siguiente circuito:

a) Encuentre la impedancia equivalente a la derecha de los puntos a y b.
b) Determine el valor de X de modo que la fuente esté en fase con la corriente.
c) ¿Cómo tiene que ser la reactancia X: inductiva o capacitiva? Determine el valor de L
o C según corresponda.
#### SOLUCION:
a) La impedancia, Z1 , de la rama R − C está dada por
Z1 = R +

jωC

---

### Página 2

Aquí R = 100Ω, C = 25µ F y ω = 400rads/seg. Entonces,
Z1 = 100 − 100j
La impedancia, Z2 , de la rama de la inductancia está dada por
Z2 = jωL
En este caso ω = 400 rads/seg y L = 0, 1H, de modo que, Z2 = 40j. La impedancia
equivalente vista desde a − b, Z, está dada por
=
+
Z
Z1 Z2
i.e.,
Z=

Z1 Z2
100(1 − j)40j
=
=
(1 + 4j)
Z1 + Z2
100 − 60j

b) Para que v(t) esté en fase con la corriente es necesario que la impedancia total, vista
desde la fuente, sea real. Ahora, la impedancia vista desde la fuente es:
Z′ = 3 + X + Z = 3 + X +

200 800j
+
.

Para que Z ′ sea real es suficiente que X = −800j/17
c) El término
X=−

800j
=
=
17j
jωC ′

corresponde a una reactancia capacitiva. El valor de la capacidad C ′ es tal que
ωC ′ =

y, como ω = 400 rads /seg
C′ =

= 53, 1µ F
800 × 400

---

### Página 3

#### Problema 2
El circuito de la figura se denomina filtro RC pasa-altos porque transmite con mayor amplitud
las señales de alta frecuencia que las de baja. Si la tensión de entrada es Vin = V0 cos ωt,
demostrar que la de salida es Vout = VR cos(ωt − ϕ), donde
V0
VR = q
2
1 + ωRC
, ω = RC
y ω ≫ RC
.
y estudie los casos en que ω ≪ RC

La impedancia equivalente está dada por:
r
j
Z =R+
=R−
= R2 + 2 2 ejϕ ,
jωC
ωC
ω C

ϕ = − arctan

Luego, la corriente fasorial circulante por el circuito es:
Vo
V̂
=q
Iˆ =
Z
R2 +

e−jϕ
ω2 C 2

Finalmente, Vout es el voltaje entre los extremos de la resistencia,
Vo
ˆ = q RVo
V̂out = IR
e−jϕ = q
e−jϕ
R2 + ω 2 C 2
1 + ω 2 R2 C 2
Con esto,
o
n
Vo
Vout (t) = Re V̂out ejωt = q
2 cos(ωt − ϕ)
1 + ωRC
Ahora estudiemos los casos pedidos:

ωRC



---

### Página 4

ω ≪ RC

ω≪
−→ 1 ≪
−→
RC
ωRC

s

1+

ωRC

2
≈

=K
ωRC

Luego,
Vo
cos(ωt − ϕ)
K
y, como K ≫ 1, el voltaje de salida se atenúa en gran cantidad. Por tanto, para bajas
frecuencias, las señales se atenúan.
Vout (t) ≈

ω = RC

Vo
Vout (t) = √ cos(ωt − ϕ)
lo que en Circuitos Eléctricos se conoce como frecuencia de corte del circuito.
ω ≫ RC

ω≫
−→ 1 ≫
−→
RC
ωRC

s

1+

ωRC

2
≈1

Luego,
Vout (t) ≈ V0 cos(ωt − ϕ)
y el voltaje de salida preserva su amplitud. Por tanto, para altas frecuencias, las señales
se transmiten.

---

### Página 5

#### Problema 3
Un circuito tiene 2 resistencias R1 y R2 , un condensador C y una inductancia L dispuestas
de la forma que se indica en la figura. El circuito es alimentado por una fuente de voltaje
altero de ecuación V (t) = V0 sin ωt. Determine la impedancia equivalente del circuito y el
módulo de la corriente en función del tiempo por cada rama del circuito.

La impedancia equivalente está dada por
−1
Zeq =
+
R1 + ZL R2 + ZC
. Luego
donde ZL = jXL y ZC = −jXC , con XL = ωL y XC = ωC

−1
Zeq =
+
R1 + jXL R2 − jXC
(R1 + jXL ) (R2 − jXC )
=
(R1 + R2 ) + j (XL − XC )
(R1 R2 + XL XC ) + j (XL R2 − XC R1 )
=
(R1 + R2 ) + j (XL − XC )
[(R1 R2 + XL XC ) + j (XL R2 − XC R1 )] [(R1 + R2 ) + j (XL − XC )]
=
(R1 + R2 )2 + (XL − XC )2
(R1 R2 + XL XC ) (R1 + R2 ) − (XL R2 − XC R1 ) (XL − XC )
=
(R1 + R2 )2 + (XL − XC )2
(R1 R2 + XL XC ) (XL − XC ) + (XL R2 − XC R1 ) (R1 + R2 )
+j
(R1 + R2 )2 + (XL − XC )2

Los módulos de cada una de las corrientes vale
|I1 (t)| =

V0 ejωt
V0
=p 2
R1 + jωL
R1 + ω 2 L2

|I2 (t)| =

V0 ejωt
V0
=q
R1 − j ωC
R2 +


1 2
ωC
