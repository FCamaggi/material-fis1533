---
title: "Pauta C1 FIS1533"
source_pdf: "Electro/pruebas-anteriores/Controles/Control 1 2023-2 (pauta).pdf"
pages: 2
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Pauta C1 FIS1533

### Página 1

FIS 1533-5: Segundo semestre 2023

Control 3

Control 1
Fecha: 6 de Septiembre 2023

1. Considere un cilindro aislante de radio R y largo infinito cargado con una densidad de carga ρ que
aumenta linealmente con la distancia al eje del cilindro (r) de la siguiente forma:
ρ (r ) = ρ0 e −r
a) Calcule el campo eléctrico para r<R

(15 pts.)

b) Calcule el campo eléctrico para r>R

(12 pts.)

c) Calcule la diferencia de potencial entre los puntos r A = 2R y r B = 3R

(3 pts.)

d) Tarea: Calcule la diferencia de potencial entre los puntos r A = R/2 y r B = 2R.

(0 pts.)

a) Para calcular el campo en r < R se usará una superficie gaussiana de cilíndrica de largo L y radio r concéntrica
con el cilindro:

Como el cilindro cargado es infinito, la simetría permite notar que el campo eléctrico a cualquier disstancia r
del centro, aputa sólo en r̂. Es decir: ⃗E(r ) = E(r )r̂. En cualquier punto, las componentes de campo paralelas
al eje, se anulan. La ley de Gauss entonces indica que sólo hay campo cruzando el manto, mientras que en
⃗ Con esto la parte izquierda de ley de Gauss resulta:
las tapas ⃗E es paralelo a d A.
I
A

⃗ =
⃗E · d A

Z
Manto

⃗ =
⃗E · d A

Z 2π Z L/2

− L/2

Erdθdz = E2πrL

Esta expresión debe ser igual a la carga encerrada por la superficie Gaussiana. Para encontrar la carga
encerrada, debemos integrar:
Qin =

Z
V

ρdV =

Z r Z 2π Z L/2

− L/2

ρ(r )rdrdθdz = 2πLρ0

Z r

e−r rdr

La integral se puede calcular usando integración por partes, haciendo u = r y dv = e−r dr con lo que du = dr
y v = −e−r con lo que la carga encerrada resulta:


Z R
r

Qin = 2πLρ0 −re−r +
e−r dr = 2πLρ0 −re−r − e−r + 1

Igualando las expresiones de la derecha e izquierda en la ley de Gauss:
I
A

⃗
⃗E · d A

=

E2πrL

=

E

=

Qin
ε0
2πLρ0 (1 − e−r − re−r )
ε0
ρ0 1 − e−r − re−r
ε0
r

La función para E dentro del cilindro ya no es tan sencilla.

■

Respuestas Forma 1

---

### Página 2

FIS 1533-5: Segundo semestre 2023

Control 3

b) Para el campo fuera del cilindro (r > R), se hace un cilindro imaginario de radio r > R y largo L. La parte
izquierda de la ecuación de Gauss queda igual, pero en la parte derecha, en el cálculo de la carga encerrada,
sólo se debe integrar hasta R, pues de ahí en adeante ρ = 0:
I
A

⃗
⃗E · d A

=

Qin
ε0

E2πrL

=

2πLρ0 1 − e− R − Re− R
ε0

E

=

ρ0 1 − e− R − Re− R
ε0
r



Se puede notar que fuera del cilindro, el campo eléctrico disminuye como 1/r (r > R)
c) La diferencia de potencial entre A y B será entonces:
VAB = VA − VB =

Z B
A

⃗E · d⃗ℓ

Al ir de A a B, d⃗ℓ = drr̂. Además el campo eléctrico apunta en el mismo sentido: ⃗E = E(r )r̂. Así:
VAB =

Z r

B

rA

Edr =

Z r 
B

rA

ρ0 1 − e− R − Re− R
ε0
r


dr =

ρ0
(1 − e− R − Re− R ) [Ln|3R| − Ln|2R|]
ε0

Con lo que:
VAB = VA − VB =

ρ0
(1 − e− R − Re− R )Ln
ε0

 

Que es positivo siempre que ρ0 > 0, ε 0 > 0 y R > 0. Lo anterior está de acuerdo con la noción de que
desplazarse en el sentido del campo eléctrico, implica desplazarse en dirección del potencial decreciente y
VB < VA .

■

Respuestas Forma 1
