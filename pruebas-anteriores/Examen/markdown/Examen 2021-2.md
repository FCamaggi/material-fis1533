---
title: "Examen 2021-2"
source_pdf: "Electro/pruebas-anteriores/Examen/Examen 2021-2.pdf"
pages: 5
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Examen 2021-2

### Página 1

Examen
FIS1533 Electricidad y Magnetismo
Profesores: E. Arévalo, F. Castillo, M.A. Díaz,
A. Meza, A. Russomando y A. Varas
15 de diciembre, 2021, 18:30 hrs.
Importante:
El examen tiene una duración de 2 horas.
El examen es individual. Se permite el uso de apuntes personales y material impreso.
No se puede usar ningún tipo de aparato electrónico. El uso de celulares, tabletas y dispositivos similares será sancionado.
La copia será sancionada de acuerdo a las reglas de la universidad.
Escriba de forma clara su nombre, RUN y sección en cada una de las hojas que entregue.
Consultas solo de enunciado, durante la primera media hora de la evaluación.

Ej. 1 — (6 puntos)
Considere un circuito constituido por una FEM E y tres resistencias conectadas tal como se muestra en la figura. El valor de las resistencias y de la FEM se dan por conocidos. Las expresiones que se preguntan abajo deben ser dadas en términos de las resistencias R1 , R2 , R3 y de E.

a)Determine las expresiones de las corrientes I1 , I2 e I3 mostradas en la figura.

(3 puntos)

b)¿Cuál es la expresión de la diferencia de potencial entre los extremos de la resistencia R3 ? (1
punto)
c)¿Cuál es el valor de la potencia disipada por la resistencia R3 ?

(1 punto)

d)Si el valor de la resistencia R2 fuera infinito, R2 = ∞, ¿cuál sería el valor de la corriente que
circula por la resistencia R3 ?
(1 punto)
Solución (Ej. 1) —
a)
Por las reglas de Kirchhoff se puede obtener que
I1 = I2 + I3 ,

(1)

E = R1 I1 + R2 I2 ,

(2)

---

### Página 2

E = R1 I1 + R3 I3 .

(3)

Nótese que restando de la ecuación (3) la ecuación (2) se obtiene que
R2 I2 = R3 I3 .

(4)

Despejando la corriente I2 de la ecuación (2) y la corriente I3 de la ecuación (3) y sustituyendo en
la ecuación (1) se obtiene
E − R1 I1 E − R1 I1
I1 =
+
.
R2
R3
De esta última expresión se obtiene que
I1 =

E(R2 + R3 )
E(1/R2 + 1/R3 )
=
.
1 + R1 /R2 + R1 /R3
R2 R3 + R1 R3 + R1 R2

1pt

Sustituyendo la expresión de I1 en la ecuación (2) se obtiene
E(R1 + RR1 R2 3 )
E
ER3
I2 =
−
=
.
R2 R2 R3 + R1 R3 + R1 R2
R2 R3 + R1 R3 + R1 R2

1pt

Por último, sustituyendo la expresión de I2 en la ecuación (4) se obtiene
I3 =

E
E(R2 R1 /R3 + R1 )
ER2
−
=
.
R3 R2 R3 + R1 R3 + R1 R2
R2 R3 + R1 R3 + R1 R2

1pt

b)
V3 = R3 I3 =

ER2 R3
.
R2 R3 + R1 R3 + R1 R2

1pt

c)
P3 = R3 I32 = R3



ER2
R2 R3 + R1 R3 + R1 R2

2
=

E 2 R22 R3
.
(R2 R3 + R1 R3 + R1 R2 )2

1pt

d)
La corriente I3 se puede escribir de la forma
I3 =

E
R3 + R1 + R3 /R2

por tanto cuando R2 → ∞, I3 toma la forma
I3 =

E
.
R3 + R1

1pt

Ej. 2 — (6 puntos)
Dos cilindros infinitos y paralelos, de radio R = 30 cm, están separados una distancia D = 90 cm
(ver figura). Si el primer cilindro presenta una carga volumétrica uniforme ρ1 = 8 µC/m3 , y no hay
campo eléctrico en un punto P a distancia d = 9 cm desde el eje del segundo cilindro, ¿cuál es la
densidad de carga ρ2 (supuesta uniforme) del segundo cilindro?

---

### Página 3

Solución (Ej. 2) —
Aprovechamos de la simetría del problema con Gauss, se puede calcular el campo eléctrico de un
cilindros indefinido. Consideramos el campo por un radio menor del radio del cilindro y por un
radio mayor
del radio del cilindro.
R
2pt
ΦC = C E0 n̂dS = 2πrLE0 (r) = Qϵint
Asi que Qint = ρπr2 L si r<R, y Qint = ρπR2 L si r>R
De aca se puede recabar el campo electrico:
ρR2
Eint = 2ϵρr0 si r<R, Eext = 2rϵ
si r>R 2pt
Y estas ecuaciones se pueden usar para ambos cilindros. Con el principio de superposición ahora
podemos solucionar el problema
E1 (D − d) = E2 (d)
ρ1 R 2
= ρ2ϵ20d
2ϵ0 (D−d)

R
ρ2 = ρ1 d(D−d)
= 9,87µC 2pt

Ej. 3 — (6 puntos)
Una espira conductora, plana y circular, de radio R se encuentra en reposo en un campo magnético
⃗ cuya dirección forma un ángulo θ con el plano de la espira, tal como se muestra en la
uniforme B,
figura. El campo magnético varía con el tiempo de acuerdo con B = B0 e−αt .

a) Calcule la magnitud de la fem inducida en función del tiempo.

(2.0 puntos)

b) Determine el instante en que la fem inducida es igual a 1/10 de su valor inicial. (2.0 puntos)

---

### Página 4

c) Determine si la dirección de la corriente inducida en la espira a favor o en contra del movimiento
de las manecillas del reloj al observar la espira desde arriba (punto O).
(2.0 puntos)
Solución (Ej. 3) —
a) La magnitud de la fem inducida está dada por:
|E| =

dΦB
dt

0.5pt

⃗ un vector perpendicular a la espira (hacia arriba en la figura) cua magnitud corresponde
Sea A
al área de la espira, entonces:
|E| = A sin θ


dB
= (πR2 ) sin θ (αB0 ) e−αt
dt

1.5pt

b) La magnitud de la fem inducida está dada por:
E=


1 
(πR2 ) sin θ (αB0 )
E0 =

0.5pt

Así:


1 
(πR2 ) sin θ (αB0 ) e−αt =
(πR2 ) sin θ (αB0 )

→

ln

= −αt

→

t=

ln 10
α

1.5pt

⃗ está en la dirección de A,
⃗ por lo tanto ΦB > 0. Además el campo B
⃗ es cada vez
c) El campo B
más débil a medida que t aumenta, por lo tanto la magnitud de ΦB también disminuye y por
lo tanto dΦB dt < 0 y de acuerdo a la ley de Faraday E > 0.
1.5pt
Así, la dirección de la corriente inducida en la espira es positiva, es decir, en contra del movi0.5pt
miento de las manecillas del reloj (vista la espira desde el punto O).
Ej. 4 — (6 puntos)
Considere los siguientes alambres, todos ubicados en el plano xy. El primero es un alambre recto e
infinito en x = 0 y z = 0. Este alambre lleva una corriente I > 0 en la dirección +ŷ. El segundo
alambre también es recto e infinito, está en x = L y z = 0, y lleva una corriente I en la dirección
opuesta −ŷ. A una distancia d del segundo alambre hay una espira cuadrada de lado a, cuyos
vértices están en: (1) x = L + d, y = 0, z = 0, (2) x = L + d + a, y = 0, z = 0, (3) x = L + d + a,
y = a, z = 0, (4) x = L + d, y = a, z = 0. La corriente I varía en el tiempo, es decir, I˙ ̸= 0, de una
forma no especificada.
Calcule la f.e.m. ε inducida en la espira y su inductancia. Indique el sentido de la corriente inducida
en la espira para los casos en que la corriente I disminuye con el tiempo y aumenta con el tiempo.
Solución (Ej. 4) —
La magnitud del campo magnético producido por un alambre recto e infinito con corriente I depende
de la distancia r al alambre:
µ0 I
B=
(5)
2πr

---

### Página 5

Entonces, el flujo ϕ1 producido por el primer alambre en la espira cuadrada es,
Z L+d+a
Z
L+d+a
µ0 I
µ0 I L+d+a dr
µ0 I
µ0 I L + d + a
ϕ1 =
a
dr = a
=a
ln r
=a
ln
2πr
2π r=L+d r
2π
2π
L+d
r=L+d
r=L+d
Este flujo tiene dirección −ẑ. 1.0pt .
El flujo ϕ2 que produce el segundo alambre en la espira es,
Z d+a
Z
d+a
µ0 I
µ0 I d+a dr
µ0 I
µ0 I d + a
a
ϕ2 =
dr = a
=a
ln r
=a
ln
2πr
2π r=d r
2π
2π
d
r=d
r=d

(6)

(7)

Este flujo tiene dirección +ẑ. 1.0pt . El flujo total ϕ en la dirección +ẑ es la diferencia,
ϕ = ϕ2 − ϕ1 = a

µ0 I  d + a
L + d + a
µ0 I (d + a)(L + d)
ln
− ln
=a
ln
2π
d
L+d
2π
d(L + d + a)

(8)

1.0pt .
La f.e.m. inducida es,
ε=−

µ0 I˙ (d + a)(L + d)
dϕ
= −a
ln
dt
2π
d(L + d + a)

(9)

µ0 (d + a)(L + d)
ln
2π
d(L + d + a)

(10)

1.0pt .
La inductancia es,
L=a

1.0pt .
La corriente inducida tiene el sentido de las manecillas del reloj cuando la corriente crece (I˙ > 0),
y el sentido contra las manecillas del reloj cuando la corriente decrece (I˙ < 0). 1.0pt .
