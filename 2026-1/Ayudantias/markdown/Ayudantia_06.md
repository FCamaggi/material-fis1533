---
title: "Ayudantia 06"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_06.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_06_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 06

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 6
Ley de Gauss II: Conductores
#### Problema 1
Considere un cable coaxial infinito y recto, el cual está compuesto por un cilindro central y casquetes cilíndricos de radios R1,2,3,4 . Cada material tiene, respectivamente, densidades volumétricas
ρ1,2,3,4 . El cilindro y el segundo casquete (radio R3 ) tienen carga 0. Encuentre el campo eléctrico
en el espacio.

#### Problema 2
Una esfera de metal de radio R y carga q está rodeada por un cascarón esférico metálico de radio
interior a y radio exterior b. El cascarón no tiene carga neta. Encuentre la densidad superficial de
carga en cada superficie.

---

### Página 2

#### Problema 3
Considere un sistema esféricamente simétrico formado por las siguientes regiones concéntricas:
Región I: 0 < r < a, material aislante con densidad de carga volumétrica
ρ1 (r) = αr2
Región II: a < r < b, conductor macizo en equilibrio electrostático.
Región III: b < r < c, material aislante con densidad de carga volumétrica
ρ2 (r) = 

β
r

Región IV: c < r < d, conductor macizo en equilibrio electrostático.
Región V: r > d, vacío.
En las interfases entre regiones existen cargas superficiales uniformes:
en r = a una densidad superficial σa
en r = b una densidad superficial σb
en r = c una densidad superficial σc
en r = d una densidad superficial σd
El conductor de la región II posee carga total Q1 , mientras que el conductor de la región IV posee
carga total Q2 .
(a) Usando la ley de Gauss y las propiedades de los conductores en equilibrio electrostático,
determine el campo eléctrico E(r) en todas las regiones:
0<r<a

a<r<b

b<r<c

(b) Determine las densidades superficiales constantes
σa

σb

σc

σd

c<r<d

r>d

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Solución Ayudantía 6
Ley de Gauss II: Conductores

#### Problema 1
Considere un cable coaxial infinito y recto, el cual está compuesto por un cilindro central y casquetes cilíndricos de radios R1,2,3,4 . Cada material tiene, respectivamente, densidades volumétricas
ρ1,2,3,4 . El cilindro y el segundo casquete (radio R3 ) tienen carga 0. Encuentre el campo eléctrico
en el espacio.

#### Solución
Para todos los casos utilizaremos ley de gauss aprovechando la simetría cilíndrica del problema,
r < R1 :
En esta región no hay cargas libres, ya que por enunciado sabemos que ρ1 = 0, no hay nada que
calcular acá, el campo es nulo ya que no hay carga encerrada para ninguna superficie gaussiana,
E = 0

,

r < R1

---

### Página 2

R1 < r < R2 :
Aquí ya hay carga que debe ser considerada, cualquier superficie gaussiana con radio entre R1 y
R2 va a encerrar toda la región R1 que no tiene carga, más una contribución de la región R2 que
depende de r, entonces nuestra carga encerrada será,
qenc (r) = 

ż 2π

żL

¡

dz

ρdV “

żr
dϕ

ρ2 rdr = 2πLρ2 p

R1

r2 R12
´
q

Entonces utilizando ley de gauss,
ż

qenc
EdS “
ϵ0
ż
qenc
E dS “
ϵ0
r 2 R2
E2πrL = 2πLρ2 p - 1 q
ϵ0
ρ2 2
E“
pr ´ R12 q
2rϵ0
Entonces el campo para la segunda región queda como,
⃗ = ρ2 pr2 - R2 qr̂
E
2rϵ0

,

R1 < r < R 2

R2 < r < R3 :
En la tercera región no hay carga, al igual que la primera, por lo que, cualquier superficie gaussiana
que cumpla con R2 < r < R3 va a encerrar la totalidad de la región de entre R1 y R2 , por lo que
solo debemos utilizar la carga encerrada de la región anterior para calcular,
¡
qenc “

ρdV = 2πLp

R22 ´ R12
q

Utilizando ley de Gauss,
ż

qenc
EdS “
ϵ0
ż
qenc
E dS “
ϵ0
R2 R2
E2πrL = 2πLρ2 p 2 - 1 q
ϵ0
ρ2 R2 R1
E“
p
´
q
rϵ0 2

---

### Página 3

Entonces nuestra tercera región de campo eléctrico cumple con,
ρ2 1 2
⃗
pR ´ R12 qr̂
E(r)
“
2ϵ0 r 2

,

R2 < r < R 3

R3 < r < R4 :
Análogo a nuestra segunda región, debemos considerar toda la carga que encierra una superficie
gaussiana entre R2 y R3 , es decir,

dz

ρ2 rdr `

dϕ

dz

qenc “

ż 2π

żL

ż R2

ż 2π

żL

R1

żr
dϕ

ρ4 rdr
R3

Lo que sigue es exactamente lo mismo de las secciones anterior, utilizar ley de gauss para calcular
el campo eléctrico y darle una dirección radial, en este caso el campo eléctrico dará,
1 1
⃗
E(r)
“
pρ2 pR22 ´ R12 q ` ρ4 pr2 ´ R32 qqr̂
2ϵ0 r

,

R3 < r < R 4

R4 < r:
Análogo a la tercera región, debemos considerar ahora TODA la carga en el problema, las contribuciones de ρ2 y ρ4 , quedando la carga como,
¡
qenc “

¡
ρ2 dV `

ρ4 dV

Realizando esta integral y haciendo el mismo procedimiento de todas las secciones anteriores llegamos a que el campo eléctrico fuera de la configuración es,
1 1
⃗
pρ2 pR22 ´ R12 q ` ρ4 pR42 ´ R32 qqr̂
E(r)
“
2ϵ0 r

,

R4 < r

#### Problema 2
Una esfera de metal de radio R y carga q está rodeada por un cascarón esférico metálico de radio
interior a y radio exterior b. El cascarón no tiene carga neta. Encuentre la densidad superficial de
carga en cada superficie.

---

### Página 4

#### Solución
Como la esfera metálica es conductora, no puede tener carga libre volumétrica, por lo que toda la
carga q está en su superficie, asumiendo que esta se distribuye uniformemente, la densidad de carga
en r = R es,
σR “

q
4πR2

(1)

En el cascarón conductor toda la carga encerrada debe ser 0, ya que el campo eléctrico dentro de
esta región debe ser nulo, por tanto toda la carga en r = a debe anular a la que se encuentra en
r = R, es decir,
Qenc = 0 = q `

q
σa
Ñ σa = ´
4πa
4πa2

(2)

Como el cascarón debe ser neutro (Por enunciado), entonces,
a2
σa 4πa2 ` σb 4πb2 = 0 Ñ σb = -σa 2
b

(3)

#### Problema 3
Considere un sistema esféricamente simétrico formado por las siguientes regiones concéntricas:
Región I: 0 < r < a, material aislante con densidad de carga volumétrica
ρ1 (r) = αr2
Región II: a < r < b, conductor macizo en equilibrio electrostático.
Región III: b < r < c, material aislante con densidad de carga volumétrica
ρ2 (r) = 

β
r

---

### Página 5

Región IV: c < r < d, conductor macizo en equilibrio electrostático.
Región V: r > d, vacío.
En las interfases entre regiones existen cargas superficiales uniformes:
en r = a una densidad superficial σa
en r = b una densidad superficial σb
en r = c una densidad superficial σc
en r = d una densidad superficial σd
El conductor de la región II posee carga total Q1 , mientras que el conductor de la región IV posee
carga total Q2 .
(a) Usando la ley de Gauss y las propiedades de los conductores en equilibrio electrostático,
determine el campo eléctrico E(r) en todas las regiones:
0<r<a

a<r<b

b<r<c

c<r<d

r>d

(b) Determine las densidades superficiales constantes
σa

σb

σc

σd

#### Solución
Primero debemos aplicar ley de guass en cada una de las regiones para obtener el campo eléctrico.
r < a : En este caso la carga encerrada viene de integrar la densidad de carga entre o y
r variables (Ya que distintas superficies gaussianas dentro de esta región encierran distinta
cantidad de carga),
ż
Qenc “

ż
dΩ

αr14 dr = 4π

αr5

(4)

aplicando ley de Guass,
ż

⃗ ¨ dS
⃗ = Qenc
E
ϵ0
αr5
4πr2 = 4π

(5)
(6)

---

### Página 6

entonces,

⃗ = αr r̂
E
5ϵ0

;

r<a

(7)

a < r < b : Nada que calcular! esta región es conductora y como sabemos en regiones conductora el campo eléctrico debe ser 0.
⃗ = 0
E

;

a<r<b

(8)

b < r < c : En esta región debemos considerar TODA la carga de la primera región (QI ), la
carga Q1 de la región conductora y además una parte de la región en donde nos encontramos,
es decir,
żr

ż
Qenc = QI ` Q1 `

dΩ

β 12 1
αa5
r
dr
“
4π
` Q1 ` 2πβpr2 ´ b2 q
b r

(9)

Entonces por ley de Gauss repitiendo el mismo desarrollo que para la primera región obtenemos,
„
⃗
E(r)
“

ȷ
αa5
βpr2 ´ b2 q
Q1
`
`
r̂
4πr2 5ϵ0 r2
2ϵ0 r2

;

b<r<c

(10)

c < r < d : Nada que calcular nuevamente! esta región es conductora y como sabemos en
regiones conductora el campo eléctrico debe ser 0.
⃗ = 0
E

;

c<r<d

(11)

r > d : Acá encerramos toda la carga de la primera región (QI ), la carga de la primera región conductora (Q1 ), la carga de la tercera región (QIII ) y la carga de la segunda región
conductora (Q2 ), por lo tanto,
Qenc = QI ` Q1 ` QIII ` Q2 = 4π

αa5
` Q1 ` 2πβpc2 ´ b2 q ` Q2

(12)

y la ley de Gauss nos lleva a,
„
ȷ
Q1 ` Q 2
αa5
βpc2 ´ b2 q
⃗
E(r) = 
`
`
r̂
4πϵ0 r2
5ϵ0 r2
2ϵ0 r2

;

r>d

(13)

---

### Página 7

Para determinar las densidades superficiales utilizamos el hecho de que cualquier superficie gaussiana dentro de una región conductora debe encerrar carga 0, para que el campo eléctrico sea 0.
Entonces en la primera región conductora, encerramos toda la región I y la superficie interna del
conductor (r = a), lo que significa que,
Qa
αa5
αa3
Ñ σa “
Q1 ` Qa = 0 Ñ Qa = -4π
“´
4πa2

(14)

Como nos dicen que la primera región conductora tiene CARGA TOTAl Q1 , es decir, tanto radio interno como externo (No volumétrico porque un conductor no puede tener carga libre en su
interior),

Qa ` Qb = Q1 Ñ Qb = Q1 - Qa Ñ Qb = Q1 ` 4π

αa5
Q1
αa5
Ñ σb “
`
4πb2
5b2

(15)

Para la segunda región conductora, seguimos el mismo procedimiento, dibujamos una superficie
gaussiana que encierra toda la carga antes de (r = c) y la carga superficial en r = c, como toda esta
carga encerrada debe ser 0,

QI `Q1 `QIII `Qc = 0 Ñ Qc = -pQI `Q1 `QIII q Ñ σc = ´

αa5 βpc2 ´ b2 q
Q1
´
´
(16)
4πc2
5c2
2c2

Para la ultima densidad de carga que nos falta repetimos el desarrollo realizado para Qb ,
Q2 = Qc ` Qd Ñ Qd = Q2 - Qc Ñ σd = 

Q1 ` Q2 αa5 βpc2 ´ b2 q
` 2 `
4πd2
5d
2d2

(17)
