---
title: "Ayudantia 11"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_11_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_11_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 11

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 11
#### Problema 1
Dos esferas metálicas concéntricas, de radios a y b, están separadas por un material conductor
de conductividad σ constante.
a) Si estas esferas son mantenidas a una diferencia de potencial V constante, encuentre la
corriente que va de una a la otra.
b) Encuentre la resistencia entre las esferas.
c) Observe que, en el caso anterior, se cumple que R ∝ 1/C, donde C es la capacitancia.
Demuestre que dicha formula es valida para dos conductores caulesquiera, separados
por un material conductor de conductividad σ constante.

---

### Página 2

#### Problema 2
Entre dos cilindros conductores coaxiales muy largos, de radios a y c > a, se llena con
materiales de conductividades σ1 y σ2 , y permitividades ϵ1 y ϵ2 , como muestra la figura.
a) Encuentre la resistencia entre el núcleo y el conductor externo.
b) Si se conecta una diferencia de potencial V0 entre el núcleo y el conductor externo,
calcule la densidad de corriente J y la corriente I que circula.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 11
#### Problema 1
Dos esferas metálicas concéntricas, de radios a y b, están separadas por un material conductor
de conductividad σ constante.
a) Si estas esferas son mantenidas a una diferencia de potencial V constante, encuentre la
corriente que va de una a la otra.
b) Encuentre la resistencia entre las esferas.
c) Observe que, en el caso anterior, se cumple que R ∝ 1/C, donde C es la capacitancia.
Demuestre que dicha formula es valida para dos conductores caulesquiera, separados
por un material conductor de conductividad σ constante.

#### SOLUCION:
a) Al establecer una diferencia de potencial sobre los conductores
V = V (a) − V (b)

---

### Página 2

se inducirán cargas Q y −Q sobre las superficies r = a y r = b, respectivamente. El
campo eléctrico en la región interior se puede determinar a partir de la Ley de Gauss
debido a la simetría esférica del problema:
Q
⃗
⃗ · dS
⃗ = qenc −→ E(r)
=
ρ̂, a < r < b
E
ϵ0
4πϵ0 r2
Por otro lado,
Z a
V =−

⃗ · d⃗r = −
E

b

Z a
b

Q dr
Q
=
4πϵ0 r
4πϵ0



1 1
−
a b



donde se ha elegido una trayectoria radial. Con ello,
Q=

4πϵ0 abV
b−a

−→

⃗
E(r)
=

V ab
ρ̂
(b − a)r2

Debido a que la zona a < r < b está llena con un material conductor, el campo
eléctrico dará origen a un movimiento de cargas (corriente), en donde la densidad está
relacionada con el campo mediante la Ley de Ohm Microscópica
⃗ =
J⃗ = σ E

σV ab
ρ̂
(b − a)r2

La corriente que fluye entre los conductores se puede obtener integrando sobre una
superficie esférica S de radio r, a < r < b :
⃗ = 4πr2 J(r) = 4πσV ab
(b − a)
b) La resistencia vendrá dada por la Ley de Ohm Macroscópica, V = IR, y con ello:


V
b−a
1 1
=
=
−
4πσab
4πσ a b
c) Recordando que la capacidad de un condensador esférico es
C=

4πϵ0 ab
b−a

entonces, se tiene que:
b−a
=
4πϵ0 ab
C
multiplicando a ambos lados por ϵ0 /σ,
b−a
ϵ0
=
4πσab
σC
Notemos que el lado izquierdo no es otra cosa mas que la resistencia que encontramos
antes. De este modo,
ϵ0
σC
donde efectivamente se cumple que R ∝ 1/C.
Veamos que esto se cumple en el caso general: Sean 1 y 2 dos conductores cualesquiera,
separados por un material de conductividad σ :

---

### Página 3

Se tendrá un flujo de corriente dado por:
⃗

Por ley de Ohm,
⃗
J⃗ = σ E
Reemplazando,
I=σ

⃗ · dS
⃗ = σQ
E
ϵ0

Por ley de Gauss. Por otro lado, si C es la capacidad del sistema, se cumple que
Q = CV
Reemplazando,

σ
CV
ϵ0

→

ϵ0
V
=
.
σC

---

### Página 4

#### Problema 2
Entre dos cilindros conductores coaxiales muy largos, de radios a y c > a, se llena con
materiales de conductividades σ1 y σ2 , y permitividades ϵ1 y ϵ2 , como muestra la figura.
a) Encuentre la resistencia entre el núcleo y el conductor externo.
b) Si se conecta una diferencia de potencial V0 entre el núcleo y el conductor externo,
calcule la densidad de corriente J y la corriente I que circula.

#### SOLUCION:
a) Asumimos que la corriente circula radialmente desde la placa interna a la externa, de
tal forma que una corriente I se relaciona con la densidad como:
⃗=
J(r)dS

en donde S es el manto de un cilindro de radio r coaxial con los cascarones conductores.
Por simetría, la densidad de corriente sale de la integral. Si ℓ denota el largo de los
cables, entonces
I = J(r) dS = 2πrℓJ(r) −→ J(r) =
2πrℓ
Suponiendo válida la ley de Ohm en este material, el campo eléctrico podemos calcularlo
fácilmente. No obstante, debemos ser cuidadosos pues la conductividad varía en cada
región llena de material conductor. El campo en las regiones queda, respectivamente,
E1 =

,
2πσ1 rℓ

E2 =

2πσ2 rℓ

ambos en dirección radial. La diferencia de potencial entre ambas placas es
Z c
Z b
Z c
I ln(b/a) I ln(c/b)
|∆V | =
E(r)dr =
E1 (r)dr +
E2 (r)dr =
+
2πσ1 ℓ
2πσ2 ℓ
a
a
b

---

### Página 5

y, por tanto, la resistencia es:

ln(b/a) ln(c/b)
+
2πσ1 ℓ
2πσ2 ℓ

b) Por la ley de Ohm, si se aplica una diferencia de potencial V0 entre las placas, la
corriente que fluirá de una a la otra es

2πℓV0
V0
= ln(b/a) ln(c/b)
R
+
σ1

σ2

y la densidad de corriente es
J(r) =

V0
= ln(b/a) ln(c/b)
2πℓr
r
+
σ1

σ2
