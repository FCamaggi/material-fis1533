---
title: "I2 2012-2 (Bañados)"
source_pdf: "Electro/pruebas-anteriores/I2/I2 2012-2 (Bañados).pdf"
pages: 6
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# I2 2012-2 (Bañados)

### Página 1

Electricidad y Magnetismo - Primavera 2012
Prof. Máximo Bañados

Interrogación 2
Tiempo: 2:00 horas - Sin apuntes.
PROBLEMAS:
1. Dos cables eléctricos de distinta conductividad σ1 y σ2 e igual sección transversal A están unidos
~
longitudinalmente (ver figura). Asuma que σ1 > σ2 . En todo el espacio hay un campo eléctrico E
paralelo a los cables.

Una corriente I circula longitudinalmente por este cable compuesto. La corriente es la misma en
ambos lados. Se observa que una densidad de carga superficial σ0 se acumula en la interfase de área
A que une los dos cables. (No confunda la densidad superficial σ0 con las conductividades σ1 , σ2 .)
Considere la interfase como un plano infinito. De este manera, el campo eléctrico generado por la
~ = σ0 n̂. Recuerde que I = JA y J = σE.
carga acumulada es E
20
~ y a la distribución de carga en
(a) Determine el campo eléctrico total (debido al campo externo E,
la interfase) en las regiones 1 y 2.
(b) Derive una expresión para la carga superficial σ0 en función de σ1 , σ2 y el campo externo
aplicado. Ayuda: note que la corriente I es la misma en ambos cables.
#### Solución:
(a) Sobre la interfase se acumula una densidad superficial σ0 . El campo eléctrico debido a esta
~ = σ0 n̂ donde n̂ es normal a la superficie. Por esta razón, en la zona del cable
carga es E
20
2, ambos campos (el campo externo y el campo debido a σ0 ) apuntan en la misma dirección,
mientras que en la zona 1, se oponen. Concluimos,
E1 = E −

σ0
,
20

E2 = E +

σ0
20

(1)

(b) La densidad de corriente en cada zona entonces es
J1 = σ1

σ0
,
E−
20





J 2 = σ2

σ0
E+
20





(2)

---

### Página 2

Ahora, las corrientes son iguales, y puesto que las areas también son iguales concluimos que
debe cumplirse la relación,




σ0
σ0
σ1 E −
= σ2 E +
20
20
de donde se deduce
σ0 = 2Eσ0

σ1 − σ2
σ1 + σ2

---

### Página 3

2. Tres placas conductoras perfectas, idénticas, planas y de área A se disponen en forma paralela como
se muestra en la figura. La distancia entre las placas 1 y 2 es d, mientras que la distancia entre 2
y 3 es 2d. Una fem (diferencia de potencial) de magnitud V0 se conecta entre las placas superior e
inferior.
Supongamos primero que el espacio entre las placas se encuentra vacío:
(a) Determine la capacidad equivalente Ceq entre los terminales 1 y 3. (1,5 ptos.)
(b) Encuentre la densidad de carga σ inducida en la parte inferior de 2 y la caída de potencial entre
2 y 3 (V23 ). (1,5 ptos.)
Supongamos ahora que la mitad del espacio entre las placas se llena con un dieléctrico de permitividad
1 para 1-2 y 2 para 2-3 (ver figura):
(c) Determine la capacidad equivalente Ceq
entre los terminales 1 y 3. (1,5 ptos.)

(d) Encuentre la densidad de carga de polarización σP en la cara inferior del dieléctrico ubicado
entre 2 y 3. (1,5 ptos.)

d

ε1

2d

ε2

V0

#### Solución:
(a) Primero, recordemos que la capacidad de un condensador de placas paralelas de área A y que se
encuentran a una distancia d es
0 A
.
C=
d
Cuando tenemos tres placas paralelas el sistema corresponde a dos condensadores conectados en
serie. Es decir,
d
2d
0 A
+
+
→ Ceq =
.
Ceq
C1 C 2
0 A 0 A
3d
(b) Sabemos que la carga inducida en la cara inferior
de la placa 1 al conectar la fem será,

Q = Ceq V0 =

0 AV0
.
3d

Ahora, sabemos que la carga en la parte superior de la placa 2 debe ser entonces −Q. Por último,
como la placa 2 es neutra la carga de su cara inferior de be ser Q. Finalmente la densidad de carga
pedida es
Q
0 V0
σ=
.
A
3d

---

### Página 4

(c) Al insertar los trozos de dieléctrico las capacidades entre 1 y 2 y entre 2 y 3 se componen de dos
condensadores de dos condensadores de área A/2 conectados en paralelo. Tenemos,
C10 =

(0 + 1 )A
0 A/2 1 A/2
+
;
d
d
2d

C20 =

0 A/2 2 A/2
(0 + 2 )A
+
.
2d
2d
4d

Como a su vez estos dos condensadores están conectados en serie tenemos,
2d
4d
+
= 0 + 0 =
Ceq
C1 C2
(0 + 1 )A (0 + 2 )A

→ Ceq

(0 + 1 )(0 + 2 )A
.
2d(30 + 21 + 2 )

(d) Determinemos primero la diferencia de potencial entre las placas 2 y 3. Sea V12 y V23 las caidas de
potencial entre 1, 2 y 2, 3, respectivamente. Puesto que las cargas en las placas de los condensadores
son iguales se tienen las ecuaciones
C10 V12 = C20 V23

V12 + V23 = V0 ,

(3)

donde C10 y C20 son las capacidades equivalentes de cada condensador, calculadas en la parte (c).
Tenemos entonces dos ecuaciones para las incógnitas V12 y V23 . Nos interesa V23 cuya solución es:
V23 =

2(0 + 1 )
V0
30 + 21 + 2

El campo eléctrico E en el interior del dieléctrico (placas 2,3) satisface las igualdades
E = E0 − Ep =

0 E0
V23

2d

donde E0 es el campo debido a las cargas en los conductores y Ep el campo debido a las cargas
inducidas en el dieléctrico (polarización). Aquí hemos usado κ = 0 . Usando esta igualdad deducimos
Ep =

0
V23 
1−
.
2d 0





Finalmente, el campo Ep se relaciona con la densidad de carga σp correspondiente mediante Ep =
σp /0 , por lo tanto,
(0 + 1 )( − 0 )
σp =
d(30 + 22 + 2 )

---

### Página 5

L
.
3. Un objeto (cable) de largo L, sección transversal A, y conductividad σ tiene una resistencia R = σA
Para un objeto de sección transversal variable A(x) la fórmula adecuada es

R=

Z

dx
.
σA(x)

Considere un objeto volumétrico de conductividad uniforme σ. El objeto consta de dos secciones
cónicas y un cilindro que une los conos. Cada cono tiene un radio mínimo h y un radio máximo
L + h. El cilindro entre los conos tiene radio L + h y largo L (ver figura). Una corriente I circula
por este objeto horizontalmente a lo largo del eje de simetría.
(a) Considere el cono de la izquierda. Demuestre que el área de la sección transversal a la corriente
es A(x) = π(x + h)2 , donde x es una coordenada horizontal medida desde el inicio del cono.
(b) Determine la resistencia de este cono (cono de la izquierda).
(c) Determine la resistencia total del objecto.

#### Solución
(a) La resistencia sobre el cono de la izquierda se encuentra directamente de la fórmula entregada,
Z L

dx
0 σπ(x + h)2
L
σπh(L + h)

Rcono =

(4)

(b) dada la simetría del problema, el cono 2 (derecha) tendrá exactamente la misma resistencias.
Finalmente la resistencia del cilindro es:
Rcilindro =

L
σπ(L + h)2

---

### Página 6

Las tres components pueden ser interpretados como resistencias en serie y entonces la resistencia
total es:
L
L
L 3h + 2L
R=2×
+
σπh(L + h) σπ(L + h)2
σπh (h + L)2
