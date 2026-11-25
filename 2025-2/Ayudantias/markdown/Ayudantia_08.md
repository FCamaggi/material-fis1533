---
title: "Ayudantia 08"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_08_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_08_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 08

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 8
#### Problema 1
Se tiene un circuito como el que se muestra en la figura:

a) Encontrar la carga de cada condensador cuando se cierra el interruptor S1 .
b) Encontrar la carga de cada condensador cuando, además, se cierra S2 .

---

### Página 2

#### Problema 2
Se tienen tres cascarones esféricos conductores concéntricos de radios a, b y c. El espacio
entre los dos primeras está lleno con un dieléctrico de constante κ. Inicialmente, la esfera de
radio a está descargada y las esferas de radios b y c tienen carga q1 y q2 , respectivamente.
Posteriormente, la esfera interior de radio a se conecta con la esfera de radio c con un cable
aislado delgado. Calcule la carga libre en cada esfera.

#### Problema 3
Dos placas conductoras con área A están separadas por una distancia d. Entre las placas se
encuentra un material cuya constante dieléctrica varia linealmente desde la unidad al lado
de una placa hasta κ al lado de la otra.
a) ¿Cuál es la capacitancia del dispositivo?
b) Demuestre que el resultado anterior coincide con el resultado esperado cuando κ → 1.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 8
#### Problema 1
Se tiene un circuito como el que se muestra en la figura:

a) Encontrar la carga de cada condensador cuando se cierra el interruptor S1 .
b) Encontrar la carga de cada condensador cuando, además, se cierra S2 .
#### SOLUCION:
a) Cuando S1 está cerrado, los dos capacitores superiores están en serie, así como también
los dos inferiores. Las capacidades equivalentes son:

−1
Carriba = 1 +
µF = µF

−1
1 1
Cabajo =
+
µF = µF
2 4

---

### Página 2

Por último, Carriba y Cabajo están en paralelo, por lo que la capacidad total será:
Ct = Carriba + Cabajo =

µF

Con esto, podemos determinar la carga total suministrada por la fuente: Q = V C =
25µC. Ahora, sean Qi y Vi la carga y diferencia de potencial -respectivamente- del iésimo condensador, numerados en orden creciente respecto a su capacitancia. Por estar
en serie, Q1 = Q3 , Q2 = Q4 . Así:
Q1 = 1µV1 ,

Q2 = 2µV2 ,

Q3 = 3µV3 = Q1 ,

Q4 = 4µV4 = Q2

Además, los voltajes satisfacen
12 = V1 + V3 = V2 + V4
Resolviendo el sistema,
Q1 = V1 = 36 − 3V1 ,

Q2 = 2V2 = 48 − 4V2

−→

V1 = 9, V2 = 8, V3 = 3, V4 = 4

Por último,
Q1 = 9 µC
Q2 = 16 µC
Q3 = 9 µC
Q4 = 16 µC
Se comprueba que Q1 + Q2 = Q3 + Q4 = 25 µC = Q.
b) En este caso, los condensadores C1 y C2 están en paralelo, al igual que C3 y C4 :
Cizquierda = C1 + C2 = 3 µF
Cderecha = C3 + C4 = 7 µF
⇒ Ceq =
µF
La carga suministrada por la fuente será:
Q = Ceq V = 25,2 µC
Además, se tiene V1 = V2 , V3 = V4 , ya que se encuentran en paralelo. Así,
= V2 =
Q1
Q2
V3 =
= V4 =
Q3
Q4
V1 =

---

### Página 3

Con esto, 2Q1 = Q2 y 4Q3 = 3Q4 . También debe darse que Q1 + Q2 = Q3 + Q4 =
25,2 µC, y por tanto:
2Q1 = Q2 = 25,2 − Q1
y
Q3 = 25,2 − Q4 = 25,2 − Q3
Finalmente, de estas ecuaciones obtenemos:
Q1 = 8,4 µC
Q2 = 16,8 µC
Q3 = 10,8 µC
Q4 = 14,4 µC

---

### Página 4

#### Problema 2
Se tienen tres cascarones esféricos conductores concéntricos de radios a, b y c. El espacio
entre los dos primeras está lleno con un dieléctrico de constante κ. Inicialmente, la esfera de
radio a está descargada y las esferas de radios b y c tienen carga q1 y q2 , respectivamente.
Posteriormente, la esfera interior de radio a se conecta con la esfera de radio c con un cable
aislado delgado. Calcule la carga libre en cada esfera.

#### SOLUCION:
Para resolver el problema, definimos 3 regiones
Región I: r < a
Región II: a < r < b
Región III: b < r < c
Al conectar las esferas de radios a y c, estas distribuirán la carga en ambas de modo que
queden al mismo potencial, tal que
q 2 = qa + q c
⃗ < a) = 0, pues corresponde al interior de un
Ahora, para la Región I tenemos que E(r
conductor.
Para la Región II, utilizamos la ley de Gauss para dieléctricos
Z
⃗ · dS
⃗ = Qfree
D
S

como no nos dicen nada del dieléctrico, asumimos que este es lineal, homogéneo e isotrópico,
⃗ = ϵE,
⃗ con ϵ = κϵ0 . Las cargas libres van a estar en los
de modo que podemos escribir D
conductores que encerramos con nuestra superficie gaussiana, en este caso el cascaron de
radio a. De este modo, tenemos
Z
qa
⃗ · dS
⃗ = 4πr2 κE(r) = qa → E(r)
⃗
κE
=
r̂
ϵ0
4πκϵ0 r2
S

---

### Página 5

Para la Región III:
Z

qa + q1
⃗
⃗ · dS
⃗ = 4πr2 E(r) = qa + q1 → E(r)
=
r̂
E
ϵ0
4πϵ0 r2
S

Se sabe que la diferencia de potencial entre las esferas de radios a y c es nula, puesto que
ambas están unidas por un cable. Así
Z c
Z b
Z c
⃗ · d⃗r = 0
⃗
⃗
E
E · d⃗r +
E · d⃗r →
0 = V (c) − V (a) = −
a

a

donde

Z b

⃗ · d⃗r +
E

Z c

a

b

⃗ · d⃗r =
E

qa
4πκϵ0

b

Z b

dr qa + q1
+
4πϵ0
a r

Z c
b

Luego,




1 1
qa + q1 1 1
qa
−
+
−
=0
4πκϵ0 a b
4πϵ0
b c




b−a
c−b
qa
+ κ(qa + q1 )
=0
ab
bc
Despejando la carga qa





b−a
c−b
c−b
+κ
qa
= −κq1
a
c
c




c(b − a) + aκ(c − b)
c−b
qa
= −κq1
ac
c


aκ(c − b)
qa = −
q1
c(b − a) + aκ(c − b)
Y finalmente se obtiene



aκ(c − b)
qc = q2 − q a = q2 +
q1
c(b − a) + aκ(c − b)

dr
r2

---

### Página 6

#### Problema 3
Dos placas conductoras con área A están separadas por una distancia d. Entre las placas se
encuentra un material cuya constante dieléctrica varia linealmente desde la unidad al lado
de una placa hasta κ al lado de la otra.
a) ¿Cuál es la capacitancia del dispositivo?
b) Demuestre que el resultado anterior coincide con el resultado esperado cuando κ → 1.
#### SOLUCION:
La constante dieléctrica no es uniforme dentro del condensador. Como esta varia linealmente,
llamemos x la distancia de cualquier punto de la primera placa que tiene κ′ = 1 hasta κ′ = κ.
De este modo, la constante dieléctrica varía de la siguiente forma:

Como es una linea recta, es fácil ver que la ecuación que satisface el comportamiento de κ′ es


κ−1
′
κ =
x+1
d
Para resolver el problema, consideremos que dividimos el dieléctrico en pequeñas losas de
grosor dx, tal como se muestra a continuación

---

### Página 7

A partir de la ecuación de capacitancia de un condensador de placas paralelas, C = κϵd0 A ,
podemos obtener la capacitancia de una sola de las losas
dC =

κϵ0 A
dx

Estas losas están en serie entre ellas, tal que 1/Ceq = 1/C1 +1/C2 +..., pero cada capacitancia
se añade infinitesimalmente, de modo que debemos integrar para obtener la suma
Z
=
C
C
Z d
dx
=
′
0 κ ϵ0 A
Z d
dx
=
ϵ0 A 0 1 + (κ − 1)x/d

d
d
(κ − 1)x
ln 1 +
=
ϵ0 A(κ − 1)
d
Evaluando y reordenando, se obtiene
C=

ϵ0 A(κ − 1)
d ln κ

Al evaluar κ → 1, el resultado es indeterminado, por lo que podemos utilizar la regla de
L’Hopital para resolver




ϵ0 A
ϵ0 A(κ − 1)
ϵ0 A 1
C = lím
= lím
=
K→1
K→1
d ln κ
d 1/κ
d
Podemos reconocer que este resultado corresponde a un condensador de placas paralelas lleno
de un material dielectrico de constante κ uniforme.
