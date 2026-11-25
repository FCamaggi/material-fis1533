---
title: "Examen 2018-2"
source_pdf: "Electro/pruebas-anteriores/Examen/Examen 2018-2.pdf"
pages: 12
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Examen 2018-2

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Instituto de Física
FIS1533 — Electricidad & Magnetismo
Segundo Semestre 2018

Nombre:
RUT:

N lista:

Examen
Duración total: 150 minutos
Reglas generales:
1. Escriba su nombre, RUT, y sección, de manera clara y legible en cada hoja.
2. Está prohibido el uso de aparatos electrónicos: calculadora, celulares, etc.
3. Se debe firmar el acta de asistencia y mostrar su TUC o cédula de identidad al momento de firmar.
4. No se aceptan preguntas de ningún tipo. Si cree que hay algún error, déjelo claramente explicado
al final de la prueba.
5. Está permitido el uso de lápiz mina en las preguntas de desarrollo, pero pierde el derecho a recorrección.
6. Cualquier acto vaya en contra del código de honor se sancionará con nota final 1.0 en el curso.

---

### Página 2

#### Problema 1 [6 puntos]
La siguiente figura muestra dos cargas puntuales ubicadas sobre el eje x. La carga +4Q está
ubicada en x = 0 y la carga −Q está localizada en x = L.

y

−Q

+4Q

x
L
Determine:
a) El punto P del plano donde el campo eléctrico es nulo [2 puntos].
b) El potencial eléctrico debido a las dos cargas puntuales en el punto P [2 puntos].
c) El trabajo sobre una carga puntual q = −5Q, necesario para traerla desde infinito hasta el
punto P [2 puntos].

a) El punto P donde el campo eléctrico es nulo debe estar sobre el eje x, ya que son los únicos
puntos donde el campo generado por ambas cargas son paralelos. Sobre el eje x el campo
solamente tiene componente x (0.5 puntos). Como se puede apreciar de la figura, el punto P
debe estar más cercano a la carga −Q, ya que la intensidad del campo generado por esta es
menor al de la carga +4Q. Además, el punto P debe estar a la derecha de la carga −Q, ya
que no puede estar entre ambas cargas, ya que en ese tramo el campo eléctrico generado por
ambas cargas puntales van en el mismo sentido.
Aplicando la Ley de Coulomb para obtener el campo eléctrico de cada carga y sumando ambos
campos para obtener el campo total, se tiene para la componente Ex del campo total (para
x > L):
Ex =

1 4Q
Q
−
=0
4π0 x
4π0 (x − L)2

=⇒

=
x
(x − L)2

(1 punto)

de modo que
=
|x|
|x − L|

=⇒

x = 2L (0.5 puntos).

El único punto del plano donde el campo eléctrico se anula está en (2L, 0), es decir, a una
distancia L a la derecha de la carga −Q.
b) El potencial eléctrico debido a las dos cargas en el punto P se obtiene sumando el potencial
debido a cada carga
V (~r) =

4Q
Q
p
p
−
.
4π0 x + y
4π0 (x − L)2 + y 2

---

### Página 3

Reemplazando la posición del punto P en la expresión anterior (~r = (2L, 0)) tenemos
VP =

1 4Q
1 Q
1 Q
−
=
. (2 puntos)
4π0 2L
4π0 L
4π0 L

c) El trabajo sobre una carga q = −5Q, necesario para traerla desde infinito hasta el punto P .
El trabajo necesario corresponde a la energía potencial eléctrica de la carga q = −5Q en el
punto P (1 punto), es decir:
Wnecesario = UE = qVP = −5Q

1 5Q2
1 Q
=−
4π0 L
4π0 L

(1 punto)

---

### Página 4

#### Problema 2 [6 puntos]
Considere un cable coaxial recto, muy largo, formado por un conductor cilíndrico interno de
radio a y otro conductor de radio interno b y externo c. La región entre a y b está rellena con un
material dieléctrico isotrópico y lineal de permitividad eléctrica . El sistema tiene un largo total
L
c. Suponga que el cilindro interno tiene carga total +Q, mientras que el externo tiene carga
−Q.

a) Calcule el campo eléctrico en todo el espacio (magnitud y dirección) [2 puntos]
b) Obtenga la polarización P~ del material entre a y b [1,5 puntos]
c) Encuentre las densidades superficiales de carga de polarización inducidas en las caras internas
y externas del material dieléctrico (σa y σb ) [1,5 puntos]
d) ¿Cuál es la capacitancia por unidad de largo del cable coaxial? [1 punto].
a) Como el campo eléctrico dentro de un conductor es siempre cero. Por lo tanto:
~
(i) r < a: E(r)
= 0 (interior del conductor) (0.4 puntos)
(ii) Para a < r < c podemos usar la ley de Gauss modificada y el hecho que el material
~ = E)
~ tenemos:
dieléctrico es lineal (D
I

~ · dA
~ =Qenc-libre = +Q
D
~
E2πrL = Q =⇒ E(r)
=

Q
r̂
2πLr

(0.8 puntos)

~
(iii) b < r < c: E(r)
= 0 (interior del conductor) (0.4 puntos)
(iv) Además, para r > c, usando la ley de Gauss tenemos:
I

~ · dA
~ = Qenc = +Q − Q = 0 =⇒ E(r)
~
E
=0
0
0

(0.4 puntos)

---

### Página 5

~ = E)
~ (0.4 puntos),
b) Para la polarización usamos el hecho que el material dieléctrico es lineal (D
por lo tanto:
~ = 0 E
~ + P~
D
~ = 0 E
~ + P~
E

(0.4 puntos)

~ =
=⇒ P~ = ( − 0 )E

Q( − 0 )
r̂
2πLr

(0.7 puntos)

c) Usando que la densidad de carga inducida está dada por σind = P~ · n̂ (0.3 puntos), tenemos
que:
σa = P~ (r = a) · (−r̂)
σa = −

( − 0 ) Q

2πLa

(0.6 puntos)

y
σb = P~ (r = b) · r̂
σb =

( − 0 ) Q

2πLb

(0.6 puntos)

d) Para obtener la capacitancia es necesario obtener la diferencia de potencial entre ambos conductores. Usando la definición de la diferencia de potencial eléctrico en término del campo
eléctrico tenemos:
Z b
V =Vb − Va = −

~ · d~l (0.25 puntos)
E

a

Z b

Q
Q
dr =
ln
V =Vb − Va = −
2πLr
2πL
a

 
b
a

(0.25 puntos)

La capacitancia por unidad de largo es simplemente
C
1Q
2π
=
=
L
LV
ln (b/a)

(0.5 puntos)

---

### Página 6

#### Problema 3 [6 puntos]
~ = B ŷ
Al selector de velocidades mostrado en la figura, se aplica un campo magnético constante B
conocido (B > 0). Las placas de arriba y abajo están separadas una distancia d y se pueden cargar
con una densidad de carga ±σ (no conocida). Una partícula de masa m, carga q > 0, y velocidad
conocida ~v = v0 x̂ (v0 > 0) entra en el selector desde la izquierda, como se muestra la figura.

Selector de velocidades

z

× × × × × × ×
q, m
v0

× × × × × × × d
× × × × × × ×

⊗

x

y

× × × × × × ×
Determine:
~ (magnitud y dirección) que se necesita en el interior del selector para
a) El campo eléctrico E
que la partícula siga en linea recta [1.5 puntos]
b) La densidad de cargas ±σ con que hay que cargar las placas para producir el campo campo
eléctrico del inciso anterior. Indique en qué placa va la densidad de carga positiva y en cuál
va la densidad de carga negativa [1 punto].
~ (E
~ = 0) y se mantiene el campo B
~ = B ŷ (B > 0), a cuál placa se
c) Si se apaga el campo E
dirigen las partículas y con con que rápidez (magnitud de la velocidad) impactan esta placa
[1.5 puntos]
~ (B
~ = 0) y se mantiene un campo E
~ = Ez ẑ (Ez < 0), a cuál
d) Si se apaga ahora el campo B
placa se dirigen las partículas y con que rápidez (magnitud de la velocidad) impactan esta
placa [2 puntos]

a) Para que la partícula siga en línea recta tenemos que la fuerza sobre esta debe ser cero
(0.5 puntos). Despreciando la fuerza peso de la partícula que es mucho menor que las fuerzas
electromagnética y usando la ley de Lorentz tenemos que:


~ + ~v × B
~
F~ = q E


~ + v~0 × B
~
0=q E
(0.5 puntos)
~ = −v~0 × B
~ = −v0 B(x̂ × ŷ) = −v0 B ẑ
=⇒ E

(0.5 puntos)

---

### Página 7

b) La magnitud del campo eléctrico entre dos placas con densidades de cargas opuestas es sim~ = |σ|/0 . Por lo tanto tenemos que:
plemente |E|
|σ|
= v0 B =⇒ |σ| = 0 v0 B
0

(0.5 puntos)

Como el campo eléctrico va en la dirección −ẑ, +σ = 0 v0 B va en la placa superior y −σ =
−0 v0 B va en la placa inferior (0.5 puntos).
~ = 0 tenemos que la fuerza es ahora:
c) Si E


~ + ~v × B
~
F~ = q E


~
F~ = q 0 + v~0 × B
~ = qv0 B(x̂ × ŷ) = qv0 B ẑ
=⇒ F~ = q v~0 × B

(0.5 puntos)

Como la fuerza es hacia arriba, la partícula choca con la placa superior (0.2 puntos). Además,
~ NO hace trabajo (0.5 puntos), no hay variación de la
como la fuerza magnética (q v~0 × B)
energía cinética y por lo tanto la partícula choca la placa de arriba con la misma rapidez que
entra en el selector, v0 (0.3 puntos).
~ = 0 tenemos que la fuerza es:
d) Si ahora B


~ + ~v × B
~
F~ = q E


~ +0
F~ = q E
=⇒ F~ = qEz ẑ
Como Ez < 0, la fuerza es hacia abajo y la partícula choca con la placa inferior (0.5 puntos).
La fuerza eléctrica SI hace trabajo, por lo tanto, usando el teorema de trabajo y energía
cinética tenemos que:
W = ∆K
Z
Z d/2

F~ · d~l = Kf − Ki

(0.5 puntos)

~ z |dy = 1 mv 2 − 1 mv 2 (0.5 puntos)
q|E
2 0
d
q|Ez | = mv 2 − mv02
2r
q
=⇒ v = v02 + d|Ez | (0.5 puntos)
m

---

### Página 8

#### Problema 4 [6 puntos]
Un alambre formado por dos semicírculos de radios a y b conduce una corriente constante I como
se muestra en la figura. Calcule el campo magnético total (magnitud y dirección) producido por el
alambre en el punto P mostrado en la figura

Para resolver este problema usamos la ley de Biot-Savart:
~ =
dB

µ0 I d~s × r̂
4π r2

(1 punto)

Los dos segmentos rectos NO producen campo magnético en P , ya que los vectores d~s y r̂ son
paralelos en esos segmentos (1 punto).
Para los segmentos semicirculares, los vectores d~s y r̂ son perpendiculares, por lo tanto, |d~s × r̂| =
ds en estos segmentos. La magnitud del campo magnético para un alambre semicircular de radio R
es entonces:
Z
Z
µ0 I
|d~s × r̂|
µ0 I
ds
µ0 I πR
µ0 I
B=
=
=
=
(2 puntos)
4π
R2
4π
R2
4π R2
4R
La dirección del campo magnético está dada por la mano derecha. El campo generado por el
semicírculo de radio a sale de la hoja, mientras que el campo generado por el semicírculo de radio b
entra en la hoja. Tomando el vector unitario ẑ saliendo de la hoja tenemos:


~ = µ0 I ẑ − µ0 I ẑ = µ0 I 1 − a ẑ
B
4a
4b
4a
b

(2 puntos)

---

### Página 9

#### Problema 5 [6 puntos]
Considere el siguiente circuito:

S

V

L

C

R
a) Si el interruptor ha estado cerrado por un largo rato, ¿cuál es la corriente a través del inductor,
(0)
IL , y la carga en el capacitor Q0 )? [2 puntos]
Si el interruptor en el circuito ha estado cerrado por un largo rato y ahora en t = 0 se abre,
responda las siguientes preguntas:
(1)

b) ¿Cuál es la corriente a través del inductor, IL , inmediatamente después de que se abre el
interruptor (indicar magnitud y sentido)? [2 puntos]
c) ¿Cuál es la frecuencia angular con la que oscila la corriente después de abierto el interruptor?
[2 puntos]

a) Como el interruptor ha estado cerrado por mucho tiempo, la corriente a través del inductor se
estabiliza y por lo tanto dIL /dt = 0. Además, la corriente por el capacitor es nula, ya que se
encuentra en equilibrio (0.5 puntos). Usando la ley de voltajes de Kirchhoff para la malla de
la izquierda tenemos:
V − VL − IR = 0
(0)

V − 0 − IR = 0 =⇒ I = IL =

V
R

(0.75 puntos)

Usando la ley de voltajes de Kirchhoff para la malla de la derecha tenemos:
VL + VC = 0
0 + Q0 /C = 0 =⇒ Q0 = 0

(0.75 puntos)

b) La corriente en el inductor inmediatamente después de que se abre el interruptor es la misma
que inmediatamente antes de que se abra, ya que esta no puede cambiar de forma abrupta en
un inductor (1 punto). Por lo tanto I(1)L = VR y va hacia abajo (1 punto).

---

### Página 10

c) Luego de abrir el interruptor, la malla de la izquierda está desconectada, por lo tanto se puede
ignorar. Ahora el circuito corresponde simplemente a la malla de la derecha y es un circuito
L − C (1 punto). Escribiendo la ley de voltajes de Kirchhoff para la malla derecha tenemos:
q
di
−
=0
dt C
d2 q
=⇒
+
q=0
dt
LC
−L

La solución a la ecuación anterior es oscilatoria con frecuenta angular:
ω=√

LC

(1 punto)

Tanto la carga como la corriente, oscilan con la misma frecuencia angular anterior.

---

### Página 11

#### Problema 6 [6 puntos]
En la figura se muestra una espira cuadrada de lado a cuya resistencia es R. A una distancia a,
a la izquierda de la espira, hay un alambre infinito por el cual circula una corriente que depende del
tiempo I(t).

R

a

I(t)
a
x

Utilizando el eje x mostrado en la figura, determine:
a) El campo magnético (magnitud y dirección) que produce la corriente I(t) en todo los puntos
del plano que contiene la espira [1 punto].
b) La magnitud del flujo magnético a través de la espira cuadrada [2 puntos].
dI(t)
> 0, calcule la magnitud
c) Asumiendo que la corriente es una función creciente, es decir,
dt
de la fem inducida (voltaje inducido) en la espira. Calcule, además. la magnitud y dirección
de la corriente inducida en la espira [3 puntos].
a) Por simetría, la magnitud del campo magnético solamente depende de la distancia al alambre
infinito. Usando la ley de Ampère con un anillo de radio r alrededor del alambre tenemos:
I

~ · d~l = µ0 Ienc
B

C

B2πr = µ0 I(t) =⇒ B =

µ0 I(t)
2πr

(0.5 puntos)

Usando el sistema de referencia propuesto y la regla de la mano derecha para identificar la
dirección del campo, tenemos que en el plano de la espira:
µ0 I(t)
~
B(x)
=−
ẑ
2πx

(0.5 punto)

donde ẑ es el vector unitario que perpendicular que sale de la página. Por lo tanto, a la derecha
del alambre el campo magnético entra en la página y en el lazo izquierdo sale.

---

### Página 12

b) El flujo magnético a través de la espira es:
Z
ΦB =
S

~ · dA
~=
B

Z 2a
Badx =
a

µ0 I(t)a
2π

Z 2a
a

dx
µ0 I(t)a
=
ln(2)
x
2π

c) Usando Ley de Faraday, la magnitud de la fem inducida es




d µ0 I(t)a
dΦB
µ0 ln(2)a dI(t)
=
ln(2) =
|E| =
dt
dt
2π
2π
dt

(2 puntos)

(1.5 puntos)

Para determinar la magnitud de la corriente, usamos simplemente la ley de Ohm:


E
µ0 a ln(2) dI(t)
Iespira =
=
(0.5 puntos)
R
2πR
dt
La dirección de la corriente en la espira está determinada por la ley de Lenz. En este caso, al ser la
dI(t)
corriente en el alambre creciente (
> 0), el flujo magnético aumenta hacia adentro de la página
dt
en la espira, por lo tanto la corriente inducida va en el sentido anti-horario para oponerse a dicho
aumento (1 punto)
