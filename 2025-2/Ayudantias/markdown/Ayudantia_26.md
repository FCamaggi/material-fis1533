---
title: "Ayudantia 26"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_26_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_26_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 26

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 26
#### Problema 1
Un generador de corriente G produce una corriente I(t) en un circuito formado por un riel
conductor sin roce, en forma de U y una barra conductora de masa m que atraviesa los
⃗ que apunta
rieles en dirección perpendicular. Un campo magnético constante y uniforme B
perpendicular al plano del circuito existe en todo el espacio. La corriente I(t) que circula en
el circuito varía en el tiempo de acuerdo con

t<0

0 ,
I(t) = bt , 0 < t < T

0 ,
T <t
Para t ≤ T , determine la fuerza electromotriz inducida en el circuito y la velocidad de la
barra en función del tiempo.

---

### Página 2

#### Problema 2
Considere dos espiras coplanares y concéntricas, de radios R1 y R2 con R1 ≫ R2 . Encuentre
la inductancia mutua entre ambas espiras.

#### Problema 3
Note la similitud entre la Ley de Ampere
I

⃗ · d⃗r = µI
B

y la ley de Faraday-Lenz
I

⃗ · d⃗r = − dΦB
E
dt
Nada nos impide aplicar los métodos de = anillos amperianos” al cálculo de campos eléectricos
generados por campos magnéticos variables, de forma análoga al cálculo de campos magnéticos producidos por corrientes estacionarias. Suponga un solenoide largo y recto, de radio a y
con n vueltas por unidad de largo, por el que circula una corriente I(t). Si la corriente varía
en el tiempo, encuentre el campo eléctrico que se induce dentro y fuera del solenoide.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 26
#### Problema 1
Un generador de corriente G produce una corriente I(t) en un circuito formado por un riel
conductor sin roce, en forma de U y una barra conductora de masa m que atraviesa los
⃗ que apunta
rieles en dirección perpendicular. Un campo magnético constante y uniforme B
perpendicular al plano del circuito existe en todo el espacio. La corriente I(t) que circula en
el circuito varía en el tiempo de acuerdo con

t<0

0 ,
I(t) = bt , 0 < t < T

0 ,
T <t
Para t ≤ T , determine la fuerza electromotriz inducida en el circuito y la velocidad de la
barra en función del tiempo.

---

### Página 2

La fuerza electromotriz inducida es
Z L Z x(t)

d
dΦ
=−
ε=−

B(−ẑ) · dxdyẑ

de este modo se obtiene que
ε = BLẋ = BLv
Por otro lado, considerando que la fuente de corriente es capaz de mantener la corriente
constante (en el sentido de la figura) y sin alteraciones durante cada período de tiempo (ie.
se ignora la corriente adicional inducida en el circuito), se tiene que la velocidad de la barra
está dada por
⃗
dF⃗ = Id⃗ℓ × B
dF⃗ = I(t)dy(−ŷ) × B(−ẑ)
dF⃗ = BI(t)dy x̂
⇒ F⃗ = BI(t)L x̂
Entonces
dv
m = BLI(t) =⇒

Z v(t)

BL
dv =
m

Z t

Si t < 0
v(t) = 0
Si 0 < t ≤ T
BL
v(t) =
m

Z t
btdt =

BLbt2
2m

Por lo tanto se tiene que la fem inducida en el circuito es

t<0
ε(t) =
B 2 L2 bt2
0<t≤T
2m

I(t)dt

---

### Página 3

#### Problema 2
Considere dos espiras coplanares y concéntricas, de radios R1 y R2 con R1 ≫ R2 . Encuentre
la inductancia mutua entre ambas espiras.

La inductancia mutua se puede obtener suponiendo que por el anillo más grande circula una
corriente I1 como se muestra a continuación:

El campo magnético en el centro del anillo puede obtenerse fácilmente utilizando la ley de
Biot-Savart (desarrollo en ayudantía), obteniendo
⃗ 1 = µ0 I1 ẑ
B
2R1
Entonces, el flujo de la espira exterior a través de la espira interior es
Z
⃗ 1 · dS⃗2
Φ12 =
B
S2

Si definimos la normal a la superficie encerrada por el anillo interior según el eje ẑ
Φ12 = B1 S2 =

µ0 I1
· πR22
2R1

Finalmente, la inductancia mutua está dada por
M=

Φ21
µ0 πR22
=
I1
2R1

---

### Página 4

#### Problema 3
Note la similitud entre la Ley de Ampere
I

⃗ · d⃗r = µI
B

y la ley de Faraday-Lenz
I

⃗ · d⃗r = − dΦB
E
Nada nos impide aplicar los métodos de = anillos amperianos” al cálculo de campos eléectricos
generados por campos magnéticos variables, de forma análoga al cálculo de campos magnéticos producidos por corrientes estacionarias. Suponga un solenoide largo y recto, de radio a y
con n vueltas por unidad de largo, por el que circula una corriente I(t). Si la corriente varía
en el tiempo, encuentre el campo eléctrico que se induce dentro y fuera del solenoide.
Como vieron en clases, el campo magnético producido por el solenoide recto es:
⃗ = µ0 nI(t)ẑ
B
siendo el eje z coincidente con el eje del solenoide. Supongamos un loop circular de radio
r < a. El flujo magnético encerrado por ese loop es
ΦB = B(t)πr2 = µ0 πr2 nI(t)
y la variación de flujo queda como
dΦB
˙
= Ḃ(t)πr2 = µ0 πr2 nI(t)
Por la ley de Faraday-Lenz,
I

⃗ · d⃗r = −Ḃ(t)πr2 = −µ0 πr2 nI(t)
˙
E

Dado que el campo magnético es paralelo al eje z, el campo eléctrico inducido será perpen⃗ = E θ̂. Así, la fem inducida será
dicular a éste, en la dirección tangencial, por lo que E
I
I
⃗ · d⃗r = E θ̂ · drθ̂ = 2πrE(r)
ε= E
y por ende
˙
2πE(r) = −µ0 πr2 nI(t)
Con ello,

˙ θ̂
⃗ in = − µ0 nr I(t)
E

---

### Página 5

Este es el campo dentro del solenoide. El campo fuera se obtiene de forma análoga, pero el
loop ahora encierra todo el solenoide. El flujo es
ΦB = B(t)πa2 = µ0 nπa2 I(t)

−→

dΦB
˙
= µ0 nπa2 I(t)

Por la ley de Faraday-Lenz,
˙
2πrE(r) = −µ0 nπa2 I(t)
Y finalmente:

⃗ out = − µ0 na I˙θ̂
E
2r
