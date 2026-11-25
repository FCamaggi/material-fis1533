---
title: "Examen 2024-1 (1)"
source_pdf: "Electro/pruebas-anteriores/Examen/Examen 2024-1.pdf"
pages: 8
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Examen 2024-1 (1)

### Página 1

FIS 1533: Primer semestre 2024

Exámen

Exámen
Fecha: 1 de Julio 2024

Respuestas Forma 1

---

### Página 2

1. Un cable coaxial muy largo consiste en un cilindro sólido con un radio interior de radio a, rodeado
por un cascarón cilíndrico conductor concéntrico de radio interno b y exterior c. El conductor interior tiene una densidad de corriente no uniforme ⃗J1 = αr ẑ donde α es una constante. El cilindro
exterior tiene una densidad de corriente ⃗J2 = − βẑ donde β es una constante positiva. Ambas regiones conductoras, llevan cada una, una corriente total I0 > 0 de igual magnitud pero en opuestas
direcciones. Entre ambos conductores existe vacío.

(a) Encuentre los valores α y β en términos de a, b, c y I0 . [2 puntos]
(b) Determine el campo magnético en todo el espacio. Exprese sus resultados en términos de a,
b, c e I0 . [2 puntos]
(c) Realice un gráfico de |⃗B| con respecto a la distancia desde el eje de simetría r. [2 puntos]
(a) Usando la definición de corriente eléctrica a partir de la densidad de corriente, se obtiene que
ZZ

I0 =
y

− I0 =
De estas ecuaciones obtenemos

ZZ

Z 2π Z a

⃗J1 · d⃗s =

⃗J2 · d⃗s =

Z 2π Z c
b

(αr ẑ) · (rdrdθ ẑ) =

2παa3

0.5

(− βẑ) · (rdrdθ ẑ) = − βπ (c2 − b2 ) .

3I0

β =

0.5 α = 2πa3 ,

I0
π ( c2 − b2 )

0.5

0.5

(b) Por simetría el campo magnético es de la forma ⃗B(r, θ, z) = B(r )θ̂. Podemos calcular B(r ) por medio de ley
de Ampère
I
⃗B · d⃗l = µ0 Ienc (Γ)

BONUS: 0.5

Γ

donde Ienc (Γ) es la corriente encerrada por el camino cerrado Γ.
- r<a
Z
Z
B(r )2πr = µ0

de donde se deriva
B (r ) =

- a⩽r⩽b
B(r )2πr = µ0

r

2π

(αr ẑ) · (rdrdθ ẑ) =

µ0 αr2
µ I r2
= 0 03 .
2πa

Z 2π Z a

B (r ) =

µ0 I0
2πr

(αr ẑ) · (rdrdθ ẑ) = µ0 I0

de donde se deriva

2παr3

---

### Página 3

- b<r⩽c


B(r )2πr = µ0

Z 2π Z r

I0 +

b



(− βẑ) · (rdrdθ ẑ)

de donde se deriva
B (r ) =

- r>c

µ0 I0
2πr

= µ0 I0 − µ0 βπ (r2 − b2 )

 2

c − r2
c −b

B(r )2πr = µ0 ( I0 − I0 ) = 0

de donde se deriva
B (r ) = 0 .

(c) Observando que |⃗B(r, θ, z)| = B(r ) se ve que el gráfico de |⃗B| es

1 POR EL GRAFICO
0.5 B(a)
0.5 B(b)

---

### Página 4

2. Un lazo rectangular de dimensiones l y w se mueve con una velocidad constante ⃗v alejándose de
un alambre recto infinitamente largo que lleva una corriente I en el plano del lazo, como se muestra
en la figura. La resistencia total del lazo es R.

(a) Usando la ley de Ampère, encuentra el campo magnético a una distancia s del alambre recto
que lleva corriente. [2 puntos]
(b) Calcule el flujo magnético a través del lazo rectangular en el instante en que el lado inferior
de longitud l está a una distancia r del alambre recto, como se muestra en la figura. [2 puntos]
(c) En el instante en que el lado inferior está a una distancia r del alambre, encuentre la f.e.m.
inducida y la correspondiente corriente inducida en el lazo rectangular. Indique en qué dirección fluye la corriente inducida. [2 puntos]
(a) Para hallar el campo magnético, se escoge un circuito amperiano como el que muestra la figura:

Así, dada la simetría del problema, el campo magnético se dirige en la dirección êϕ . De esta forma, la Ley
de Ámpere es:
I

⃗B · d⃗l = µ0 Ienc ,

(1)

en donde Ienc es la corriente que cruza el circuito amperiano, es decir, Ienc = I.
Por otro lado, el elemento diferencial de línea es paralelo al campo punto a punto, por lo que ⃗B · d⃗l = B dl,
y por lo tanto:
Z

B

dl = µ0 I → B(2πs) = µ0 I → B =

µ0 I
2πs

0.75

(2)

Por lo tanto:

⃗B = µ0 I êϕ .
2πs

0.25 por la dirección

(3)

Es decir, el campo entra a la página.

---

### Página 5

(b) el flujo magnético viene dado por:
Φ=

ZZ

⃗
⃗B · d A,

(4)

⃗ el vector de área.
con d A
⃗ = lds êϕ ,
Para cierto tiempo t, las líneas de campo magnético a una distancia s cruzan un área diferencial d A
y entonces:

Z r +w 
µ0 I
µ Il 
w
Φ=
(lds) = 0 ln 1 +
(5)
2πs
2π
r
r

0.5

0.5

(c) Por definición:
f.e.m.

=
=
=

dΦ
dt

µ0 Il d
w
−
ln 1 +
2π dt
r
µ0 Il
w
dr
2π r (r + w) dt

−

0.5

(6)

pero dado que la velocidad de movimiento es constante, entonces r = vt, tal que:
f.e.m. = −

µ Il
wv
dΦ
= 0
dt
2π r (r + w)

0.5

(7)

Esta f.e.m. actúa como una fuente de voltaje en el circuito y por lo tanto, la corriente es:
I=

f.e.m.
µ Il
wv
= 0
R
2πR r (r + w)

(8)

El flujo decrece y por la ley de Lenz, se debe inducir una corriente que se oponga dicho cambio, es decir,
que genere un campo magnético que contrarrestare el campo que = se pierde”. Por lo tanto, dicha corriente
debe generar un campo en la misma dirección del original, lo cual se logra con unca corriente en la dirección
de las manecillas del reloj.

---

### Página 6

3. Un anillo de radio R0 tiene una carga Q positiva, la cual está distribuida de manera uniforme sobre
el anillo, como se ilustra en la gura. Considere una carga puntual de carga negativa q (q < 0) y
masa m, la cual es depositada en reposo sobre el eje central del anillo cerca del centro representado
por el punto A, además la carga esta soldada a un resorte ideal de constante elástica k o y largo
natural cero con extremo jo en el punto A.

(a) Calcule el campo eléctrico provocado por el anillo cargado en el eje de simetría del mismo. [3
puntos]
(b) Calcule la fuerza total que siente la carga q. [2 puntos]
(c) Si la carga q se mueve exclusivamente en el eje de simetría, escriba (usando Newton) la ecuación de movimiento que rige su movimiento. Estime la frecuencia de pequeñas oscilaciones
(z ≪ R0 ) con que se moverá. [1 punto]

---

### Página 7

(a) Considere el anillo cargado como en la siguiente figura:

En este problema, la carga está a lo largo de un cuerpo unidimensional y por lo tanto, es posible definir
una densidad lineal de carga λ.
La simetría del problema muestra que la única contribución al campo se da a lo largo del eje z, tal que

⃗E =

4πϵ0

Z

dq
cos α êz .
r2

0.5

(1)

De la geometría del problema:
r2

=

cos α

=

R2 + z2
z
√
R2 + z2

(2)

Además, se puede definir el diferencial de carga
dq = λ ds,

(3)

con ds un diferencial de arco en el anillo. Reemplazando:
z
⃗E = 2λ
4πϵ0 ( R2 + z2 )3/2

Z

0.5

ds êz .

(4)

Integrando en media circunferencia (ya que se hizo la suma vectorial de dos dq diametralmente opuestos):

(πR)z
⃗E = 2λ
êz .
4πϵ0 ( R2 + z2 )3/2

(5)

Finalmente, ya que la densidad de carga es uniforme:
λ=

dq
Q
q
yλ=
→λ=
,
ds
s
2πR

(6)

lo cual implica que:

⃗E =

Qz
êz .
4πϵ0 (z2 + R20 )3/2

(7)

(b) Si la carga q se encuentra a una distancia z del centro del anillo, el campo eléctrico hará una fuerza dada
por:

|q| Qz
⃗Felec = −|q|⃗E = − 1
êz ,
4πϵ0 (z2 + R20 )3/2

0.5

(8)

mientras que el resorte hará una fuerza:

⃗Felstica = −k0 z êz ,
con lo que la fuerza total es:

"
⃗Ftotal = − k0 +

0.5

|q| Q
4πϵ0 (z2 + R20 )3/2

(9)

#
z êz

(10)

---

### Página 8

(c) De la segunda ley de Newton, se tiene que en la dirección z:
#
"
|q| Q
⃗Ftotal = m d z êz → d z + k0 +
z = 0,
m
4πϵ0 m (z2 + R20 )3/2
dt2
dt2

(11)

que es la ecuación de movimiento de q.
Ahora, para oscilaciones pequeñas, es decir, z ≪ R0 :
z
z
≈ 3,
R
(z2 + R20 )3/2
entonces la ecuación de movmiento es
d2 z
+
dt2



k0
|q| Q
+
m
4πϵ0 mR3

(12)


z = 0,

(13)

que es la ecuación de un Movimiento Armónico Simple con frecuencia
ω2 =

|q| Q
k0
+
m
4πϵ0 mR3

(14)
