---
title: "Problemas de Electromagnetismo (Alternativas) - Sebastián Urrutia"
source_pdf: "Electro/material-apoyo/compilados/Problemas de Electromagnetismo (Alternativas) - Sebastián Urrutia.pdf"
pages: 155
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Problemas de Electromagnetismo (Alternativas) - Sebastián Urrutia

### Página 1

Electricidad y
Magnetismo
Problemas de selección múltiple

Sebastián Urrutia Quiroga
sgurruti@uc.cl
www.sgurruti.cl

Primera Edición – Julio de 2015

---

### Página 2

Disponible en línea: http://www.sgurruti.cl/
Sebastián Urrutia Quiroga
Contacto: sgurruti at uc.cl
Se autoriza la reproducción total o parcial, con fines académicos, por cualquier medio o procedimiento,
incluyendo la cita bibliográfica que acredita al trabajo y a su autor.
Prohibida su Comercialización

---

### Página 3

Índice general

1. Fuerzas y campos electrostáticos

2. Condensadores, dieléctricos y corriente eléctrica

3. Circuitos eléctricos

4. Magnetostática

5. Inductancias y flujo magnético

6. Circuitos de corriente alterna y campos variables en el tiempo

---

### Página 4

Fuerzas y campos electrostáticos

Ecuaciones de Maxwell en uno de los muros exteriores de la Universidad de Varsovia

---

### Página 5

#### Problema 1.1.
Se tienen dos alambres muy largos (que se pueden asumir infinitos) cada uno uniformemente cargado
con densidades lineales de carga λ y λ/2 respectivamente. Los alambres están situados paralelamente a
una distancia ℓ entre ellos. La magnitud de la fuerza por unidad de largo entre los alambres es:
a)

λ2
4πℓε0

λ2
b)
2πℓε0
c)

λ2
πℓε0

d)

2λ2
πℓε0

e) Ninguna de las anteriores.
Sin pérdida de generalidad, supongamos que ambos cables están ubicados en el plano XY . Supondremos que el cable con densidad de carga λ coincide con el eje Y y crea un campo
~ = E(x) ı̂ =
E

λ
ı̂
2πε0x

con x la distancia que separa al cable del punto donde se calcula el campo. Sobre un elemento dq
del cable con densidad de carga λ/2 este campo ejerce una fuerza de magnitud dF = dq E(ℓ). Para
este cable se tiene que dq = (λ/2) dy, y con ello
dF =

λ2
dy
4πε0 ℓ

Finalmente, la magnitud de la fuerza por unidad de largo es
f=

λ2
F
L
4πℓε0

#### Problema 1.2.

|x|
Considere un cable aislante de largo L en el eje X, donde su densidad lineal de carga es λ(x) = λ0
L
con respecto al sistema de referencia indicado en la figura. ¿Cuál de las siguientes expresiones expresa
~ y), con y > 0 arbitrario, producido por el cable?
correctamente la magnitud del campo eléctrico E(0,

---

### Página 6

a)

λ0
y2
4πε0 L (y 2 + L2 /4)

b)

λ0
y2
2πε0 L (y 2 + L2 /4)

c)

λ0
y
p
2πε0 L y + L2 /4

λ0
d)
4πε0 L
λ0
e)
2πε0 L

1− p

y

y 2 + L2

!

y
1− p
y + L2 /4

!

Usando la definición del campo eléctrico para una distribución continua de masa,
~ r) =
E(~

4πε0

ˆ

~
dq(R)

~
~r − R
~ 3
k~r − Rk

~ = x ı̂ y dq = λ(x) dx. Reemplazando en el campo eléctrico, tenemos
En este problema, ~r = y ̂, R
que:
ˆ L/2
y ̂ − x ı̂
~ r) =
E(~
λ0 |x| 2
dx
4πε0 −L/2
(x + y 2)3/2
La componente ı̂ se anula porque el integrando es impar y la integral se realiza entre ±L/2 (se
puede argumentar también por la geometría del problema). El integrando de la la componente ̂ es
par, por lo que:
!
ˆ L/2
λ
y
y
λ
x
~ r) = 2
̂
E(~
1− p
dx ̂ =
4πε0 0
(x2 + y 2)3/2
2πε0 L
y 2 + L2 /4

#### Problema 1.3.
Se intersecan dos esferas sólidas cargadas, E1 y E2 , con densidades de carga uniforme ρ1 y ρ2 respectivamente. Los radios de ambas esferas son 4R y 3R, y sus centros se ubican en los puntos (4R, 0, 0) y

---

### Página 7

(8R, 0, 0), respectivamente como indica la figura (notar que en la intersección la densidad es ρ1 + ρ2 ).
Suponiendo que las densidades de carga satisfacen la relación ρ1 = ρ2 ≡ ρ, ¿cuál de las siguientes
expresiones corresponde a la magnitud del campo eléctrico en el punto (12R, 0, 0)?
Y
E1 , ρ1
E2 , ρ2

X

Z

a)

18ρR
27ε0

b)

3ρR
8ε0

c)

ρR
4ε0

d)

43ρR
48ε0

e)

47ρR
36ε0

El punto 12R ı̂ se encuentra fuera de ambas esferas, por lo que el campo que cada esfera produce
corresponde al de dos cargas puntuales en sus respectivos orígenes. El punto 12R ı̂ está a distancia
8R del centro de E1 y a 4R del centro de E2 . El campo está dirigido a lo largo del eje X y es:
E=
Donde
Q1 =

Q1
Q2
+
4πε0 (8R)2 4πε0 (4R)2

4π(4R)3
ρ,

Reemplazando en E resulta
E=

Q2 =

4π(3R)3
ρ

43ρR
48ε0

#### Problema 1.4.
Considere nuevamente las esferas de la figura anterior. Suponiendo que ambas esferas tienen carga

---

### Página 8

positiva, ¿cuál debe ser la razón ρ1 /ρ2 entre las densidades para que el campo eléctrico en el punto
(6R, 0, 0) sea nulo?
b)
a)

c) 1
d)

e) Ninguna de las anteriores
El punto 6R está a la derecha del centro de E1 , y a una distancia 2R del mismo. Por otro lado, el
punto se encuentra también a distancia 2R del centro de la esfera E1 , pero a la izquierda. Por lo
tanto, solo si las densidades son iguales ambos campos serán de igual magnitud, pero de dirección
opuesta y se cancelan. Así, la respuesta correcta es:
ρ1
=1
ρ2

#### Problema 1.5.
La siguiente figura muestra las líneas de campo producidas por tres cargas con magnitud +1 C, +1 C y
−1 C, aunque no necesariamente en este orden. La superficie gaussiana que se muestra en la figura es
una esfera que contiene dos de las cargas. ¿Cuál de las siguientes afirmaciones es correcta para el flujo
eléctrico a través de esta superficie?

a) Es −
b) Es

2C
ε0

2C
ε0

---

### Página 9

c) Es cero
d) Dependerá de la distancia a la que se encuentren las cargas que están adentro
e) Dependerá de la distancia a la que se encuentre la carga que está afuera
En la región sombreada se ven líneas de campo que parten de una de las cargas y terminan en la
otra. Esto quiere decir que las cargas son de signo opuesto, por lo tanto la respuesta correcta es
Φe = 0

#### Problema 1.6.
Una esfera conductora masiva con radio r1 se encuentra dentro de un cascarón esférico conductor de
radio interior r2 y radio exterior r3 , el cual se encuentra dentro de otro cascarón esférico conductor
con radio interior r4 y radio exterior r5 . Los radios cumplen con r1 < r2 < r3 < r4 < r5 . Los tres
conductores están ubicados en forma concéntrica unos con otros. La esfera y el cascarón exterior están
eléctricamente cargados con carga positiva +2q y carga negativa −q, respectivamente. Por otro lado, el
cascarón del medio se encuentra eléctricamente neutro. La densidad superficial de carga eléctrica en la
superficie exterior del cascarón del medio es:
a) σ = −
b) σ =

q
2πr22

q
2πr32

q
4πr2 r3
q
d) σ =
4πr12
c) σ =

e) σ =

q
4πr52

La situación descrita se puede esquematizar de la siguiente forma:

---

### Página 10

Como, en el interior del cascarón intermedio, el campo tiene que ser cero, en la superficie interna
del cascarón se induce una carga −2q. Puesto que dicho cascarón es eléctricamente neutro, debe
inducirse una carga 2q en la cara externa del mismo. La densidad en esta superficie externa es:
σ=

q
2q
4πr3
2πr3 2

#### Problema 1.7.
Para la configuración del Problema 1.6, la magnitud del campo eléctrico como función del radio r en el
espacio r3 < r < r4 es:
a) E(r) =

q
4πε0 r 2

b) E(r) =

q
πε0 r 2

qr32
ε0 r 4
q
d) E(r) =
2πε0 r 2
q
e) E(r) = 3π 2
εr
4 0
c) E(r) =

Si se usa la ley de Gauss en esta región se descubrirá que la carga encerrada es 2q. Por tanto, el
campo es:
q
E(r) =
2πε0 r 2

---

### Página 11

#### Problema 1.8.
Para la configuración del Problema 1.6, la diferencia de potencial entre la esfera y el cascarón exterior
es:


r4 − r1 r3 − r2
−
r1 r4
r2 r3


q
−
b) ∆V =
2πε0 r1 r4
q
a) ∆V =
2πε0



c) ∆V = 0 V
q
d) ∆V =
4πε0



e) ∆V =

q
√

−
r2 r3



4πε0 r1 r4

Se nos pide calcular V (r1 )−V (r4 ). Antes que todo, calcularemos el campo eléctrico para r1 < r < r4 :

q

ρ̂ r1 < r ≤ r2


2πε0 r 2




~
~0
E(r) =
r2 < r ≤ r3





q


ρ̂ r3 < r ≤ r4
2πε0 r 2

Usando la definición de diferencia de potencial entre dos puntos,
ˆ r4
ˆ r1
~ · d~r
~
E
E · d~r =
V (r1 ) − V (r4 ) = −
r1
r4
ˆ r2
ˆ r4 
q
dr
dr
+
2πε0
r
r3 r
 r1

q
− + −
2πε0 r1 r2 r3 r4


q
r4 − r1 r3 − r2
−
2πε0
r1 r4
r2 r3

#### Problema 1.9.
Un cable coaxial consiste de un alambre metálico con radio r0 = 1 mm y un cascaron cilíndrico metálico
con radio interior ri = 6 mm y radio exterior re = 6.2 mm que se encuentra en forma concéntrica
alrededor del alambre. El alambre tiene una densidad superficial de carga σ = 3.6 µC m−2 y el cascarón
está conectado a tierra. El largo del cable es tal que se pueden despreciar los efectos en los extremos
del cable. Sabiendo que,

---

### Página 12

ε0 ≈ 9 × 10−12 C V−1 m−1
Un objeto conectado a tierra significa que, vía un cable conductor, el objeto se conecta a un
conductor infinitamente grande
el valor máximo de la magnitud del campo eléctrico en el espacio entre el alambre y el cascarón es:
a) Emax = 4 kV m−1
b) Emax = 20 kV m−1
c) Emax = 40 kV m−1
d) Emax = 80 kV m−1
e) Emax = 400 kV m−1
El campo eléctrico es más intenso cerca del cilindro interno y decae al alejarse, por lo tanto su mayor
valor ocurre en r = r0 . Como se trata de la superficie de un conductor sabemos que
E(r0 ) =

σ
ρ̂
ε0

Reemplazando los valores, fijándose en las unidades, se encuentra que:
Emax =

3.6 × 10−6
= 400 × 103 V m−1 = 400 kV m−1
9 × 10−12

#### Problema 1.10.
Para el cable coaxial del Problema 1.9, la densidad superficial de carga en la superficie interior del
cascarón es:
a) σi = −3.0 µC m−2
b) σi = −0.6 µC m−2
c) σi = −1.2 µC m−2
d) σi = −0.3 µC m−2
e) σi = −2.0 µC m−2

---

### Página 13

Aplicando la ley de Gauss a un cilindro concéntrico y de radio tal que quede en el interior del
cilindro externo, sabemos que el flujo es cero (puesto que el campo eléctrico es cero en el interior del
conductor). Esto implica que la carga encerrada tiene que ser cero. La carga encerrada es la suma
de la carga ubicada en el cilindro interno y la carga que está ubicada en la superficie interna del
cilindro externo. Entonces,
2πr0 h σ + 2πri h σi = 0
de donde se obtiene que:
σi = −

r0
σ = −0.6 µC m−2
ri

#### Problema 1.11.
Para el cable coaxial del Problema 1.9, la magnitud del campo eléctrico al exterior del cascaron (r > re )
es:
a) E(r) =

2πr0 Lσ
r2

b) E(r) =

2πr02 σ
r2

c) E(r) =

πr0 Lσ
r2

d) E(r) = 0 V m−1
e) E(r) =

L2 σ
r2

Como el cilindro externo está conectado a tierra, su potencial es cero. No se deposita carga en la
superficie externa de este cilindro por lo que el campo al exterior del cascarón es:
E(r) = 0 V m−1

#### Problema 1.12.
Una esfera conductora de radio a tiene dos cavidades también esféricas de radios R1 y R2 . Llamemos S
a la superficie exterior y Si a la superficie en torno a la cavidad i−ésima (i = 1, 2) como se muestra en
la figura. En el centro de la cavidad de radio R1 hay una carga puntual q1 y en el centro de la cavidad
de radio R2 hay una carga puntual q2 , mientras que la separación entre las ambas cargas es d. Por otra
parte, la esfera conductora tiene carga total Q.

---

### Página 14

El módulo de la fuerza sobre la carga q1 es:
a) F =

q1 q2
4πε0 d2

b) F =

Qq1
4πε0 d2

c) F = 0 N
d) F =

q1 q2
4πε0 R12

q12
e) F =
4πε0 R12
Como el campo en el conductor se anula y la carga q1 está al centro de la cavidad, la densidad
superficial en S1 se distribuye con simetría esférica y la carga inducida total es −q1 . Por tanto,
no se genera fuerza sobre la carga en la cavidad. Por otra parte, el campo eléctrico en la cavidad
corresponde solamente el campo creado por q1 , y por lo tanto nada hace fuerza sobre q1 . Así, la
solución correcta es:
F = 0N

#### Problema 1.13.
Considere nuevamente la configuración descrita en el Problema 1.12. Tomando como referencia el potencial en infinito igual a cero, la superficie S1 está a potencial eléctrico igual a:
a) V =

Q + q1 + q2
4πε0 a

b) V =

Q
q2
q1
+
+
4πε0 a 4πε0 R1 4πε0R2

c) V =

Q − q1 − q2
4πε0 a

---

### Página 15

d) V =

Q
4πε0 a

e) V =

Q + q1 + q2
4πε0 (a − R1 − R2 )

Sobre las superficies internas S1 y S2 se depositan −q1 y −q2 respectivamente. Sobre la superficie
externa S se deposita entonces una carga Q + q1 + q2 con simetría esférica. Desde fuera se ve como
una carga puntual en el origen, por lo tanto:
V =

Q + q1 + q2
4πε0a

#### Problema 1.14.
Dos cascarones esféricos concéntricos están a potenciales eléctricos V1 y V2 (tomamos como referencia
que el potencial en infinito es cero). El radio del cascarón interior es a y el radio del cascarón exterior
es 2a. Ambos cascarones poseen un grosor despreciable.

La carga en el cascarón interior es:
a) No se puede calcular con los datos dados
b) Q1 = 4πε0 aV1
c) Q1 = 2πε0 (aV1 + bV2 )
d) Q1 = 0 C
e) Q1 = 8πε0 a(V1 − V2 )

---

### Página 16

Llamemos Q1 la carga en el cascarón interior. En la región a < r < 2a el campo se debe solamente
a Q1 y es:
~ I = Q1 ρ̂
E
4πε0r 2
Entonces
V2 − V1 = −

ˆ r2 =2a
r1 =a

~ I · d~r = Q1
E
4πε0



−
r2 r1



=−

Q1
8πε0 a

Por tanto,
Q1 = 8πε0a(V1 − V2 )

#### Problema 1.15.
Considere la situación expuesta el Problema 1.14. La carga en el cascarón exterior es:
a) No se puede calcular con los datos dados
b) Q2 = 8πε0 a(2V2 − V1 )
c) Q2 = 8πε0 aV2
d) Q2 = Q1

V2
V1

e) Q2 = Q1

V1
V2

Si llamamos Q2 la carga en el cascarón exterior, el campo y el potencial en r > 2a son:
~ II = Q1 + Q2 ρ̂ ,
E
4πε0 r 2

VII =

Q1 + Q2
4πε0 r

Entonces V2 = VII (2a). Usando el valor de Q1 encontrado en el problema anterior, se despeja Q2 y
resulta:
Q2 = 8πε0 a(2V2 − V1 )

#### Problema 1.16.
Nuevamente considere la situación expuesta en el Problema 1.14. El trabajo necesario para llevar una
carga q desde infinito hasta el centro de las esferas es:
a) W = q(V1 + V2 )

---

### Página 17

b) W = q(V2 − V1 )
c) W = −q(V2 − V1 )
d) W = qV1
e) W = 0 J
El cascarón interior está a potencial V1 . Para r < a no hay otras cargas y por lo tanto el potencial
no cambia y V = V1 para r < a. Como el trabajo es W = q(Vfinal − Vinicial ), el resultado correcto:
W = qV1

#### Problema 1.17.
Nuevamente considere la situación expuesta en el Problema 1.14. El trabajo necesario para llevar una
carga q desde la esfera interna de radio a hasta una posición fuera de las esferas r = 3a es:
q
a) W = (2V2 − 3V1 )
q
b) W = (V2 + 2V1 )
q
c) W = (2V2 − V1 )
q
d) W = − (3V2 − 2V1 )
e) W = −q(3V2 + V1 )


El trabajo W = q V (3a) − V (a) . Sabemos V (a) = V1 . Y afuera el potencial es el de una carga
puntual, y vale V2 en r = 2a, de modo que afuera podemos escribir:
V = V2
La respuesta correcta es, entonces,

2a
,
r

r > 2a

q
W = (2V2 − 3V1 )

#### Problema 1.18.
Considere la siguiente distribución de carga: un plano infinito con densidad uniforme σ ubicado en
el plano XY y un alambre delgado de largo infinito con densidad uniforme de carga λ perpendicular
al plano (que atraviesa el plano por un orificio de tamaño despreciable). Elija el eje Z de modo que
coincida con el alambre. El trabajo necesario para llevar una carga q desde el punto (1, 0, 1) hasta el
punto (2, 0, 2) es:

---

### Página 18

q
(λ ln 2 + πσ)
2πε0
q
(λ ln 2 + πσ)
b) W = −
2πε0
q
c) W =
(λ ln 2 − πσ)
2πε0
q
(λ ln 2 − πσ)
d) W = −
2πε0
q
(λ ln 2 − 2πσ)
e) W =
πε0
a) W =

El campo eléctrico es la suma entre el campo que produce el alambre y el campo que produce el
plano:
~ = λ ρ̂ + σ k̂
E
2πε0 r
2ε0
El trabajo es
W = q(Vf − Vi ) = −q

ˆ (2,0,2)
(1,0,1)

~ · d~r
E

Tomamos el siguiente camino:
~r(t) = ~r1 (t) + ~r2 (t) ,

~r1 (t) : (x, y, z) = (t, 0, 1) ∀t ∈ [1, 2]
~r2 (t) : (x, y, z) = (2, 0, t) ∀t ∈ [1, 2]

Realizamos ambas integrales:
ˆ 2

λ dt
~
r1
1 2πε0 t
λ ln 2
2πε0
ˆ 2
ˆ
σ dt
~
E · d~r =
~
r2
1 2ε0
σ
2ε0
ˆ

~ · d~r =
E

Sumando ambos resultados,
W =−

q
(λ ln 2 + πσ)
2πε0

#### Problema 1.19.
Considere la configuración de cargas de la figura. Cada una de las cargas están separadas por una
distancia d de las otras. El trabajo necesario para lograr esta configuración, si inicialmente las cargas
estaban infinitamente separadas las unas de las otras, es:

---

### Página 19

a) W =

5q 2
4πε0 d

b) W =

5q 2
2πε0 d

c) W =

5q 2
8πε0 d

5q 2
d) W =
16πε0 d
e) Ninguna de las anteriores
La energía almacenada en esta configuración, que equivale al trabajo realizado para armar dicha
configuración, es:


q1 q2 q1 q3 q2 q3
W =
+
+
4πε0 r12
r13
r23
Como la distancia rij entre ellas es d, esto equivale a:
 2

5q 2
q
2q 2 2q 2
+
+
W =
4πε0 d
d
d
4πε0 d

#### Problema 1.20.
Dos anillos idénticos (muy delgados) de radio a, cargados uniformemente con cargas Q1 y Q2 , se colocan
coaxialmente a una distancia a de separación, como se muestra en la figura. Calcule el trabajo hecho
por un agente externo para mover una carga q desde el centro del anillo con Q1 al centro del anillo con
Q2 .

---

### Página 20

q(Q1 + Q2 )
a)
4πε0 a
b)

q(Q1 − Q2 )
4πε0 a

c)

q(Q1 − Q2 )
4πε0 a

d)

q(Q1 + Q2 )
4πε0 a

√ !
1− 2
√
√ !
1− 2
√
√ !
1+ 2
√
√ !
1+ 2
√

e) No se puede determinar con estos datos
Si pensamos que el centro del anillo con Q1 coincide con el origen de los ejes cartesianos, entonces
el potencial eléctrico realizado por este anillo en un punto P a una distancia x en el eje de simetría
es:
Q1
√
φQ1 (x) =
4πε0 x2 + a2
En el caso del segundo anillo, el potencial en el mismo punto P bajo las mismas condiciones es:
φQ2 (x) =

Q1
p
4πε0 (x − a)2 + a2

Con ello, el potencial total de la configuración es:
φ(x) = φQ1 (x) + φQ2 (x) =

4πε0

√

Q1
Q2
+p
x +a
(x − a)2 + a2

!

---

### Página 21

El trabajo realizado por un agente externo equivale a calcular W = q(φfinal − φinicial ). Por tanto,


W = q φ(a) − φ(0)

 

Q1
Q1
Q2
Q2
q
√ +
−
+√
4πε0
a
a
2a
2a
√ !
q(Q1 − Q2 ) 1 − 2
√
4πε0 a

#### Problema 1.21.
La figura muestra un cuadrado de largo L, formado por cinco cargas positivas iguales de magnitud Q en
un plano horizontal (cuatro en los vértices y una quinta en el centro del cuadrado). Una carga positiva,
de magnitud
q y masa m se introduce a una altura h por encima del centro del cuadrado. Suponga que
√
L = 6h. ¿Cuál de las siguientes relaciones es correcta cuando la carga q está en equilibrio? Considere
a la aceleración de la gravedad simplemente como g.

a) Q =

2πε0h2 mg
3q

b) Q =

4πε0h2 mg
3q

c) Q =

6πε0h2 mg
3q

d) Q =

8πε0h2 mg
3q

e) Ninguna de las anteriores
La simetría del problema nos indica que los campos eléctricos producidos por las cargas en los
vértices del cuadrado solo apuntan en la dirección k̂, pues las otras componentes se anulan unas con
otras, como indica la figura:

---

### Página 22

Sea α el ángulo indicado en la figura, que nos ayudará a encontrar la componente Ez del campo
eléctrico total. Si denotamos por D la distancia entre las cargas en los vértices y la carga q, entonces:
Ez = 4 ·

1 Q
cos α
4πε0 D 2

Usando las propiedades geométricas del problema,
D 2 = h2 +

6h2
L2
= h2 +
= 4h2 ,

y por tanto:
Ez =

cos α =

h
h
D
2h



Q 3
4πε0 2h2

Q 1
4πε0 2h2

Así, el campo eléctrico total viene dado por:
1 Q
Q
E = Ez +
4πε0 h
4πε0



+ 2
2h
h

Igualando fuerzas,
mg = qE =

3Qq
8πε0 h2

−→

Q=

8πε0 h2 mg
3q

#### Problema 1.22.
Una carga puntual positiva de magnitud q se encuentra en el vértice de una sección esférica, como se
muestra en la figura. Los planos verticales de la sección esférica forman un ángulo de 60◦ . ¿Cuál es el
flujo eléctrico que atraviesa la sección esférica?

---

### Página 23

q
4ε0
q
b)
8ε0
q
c)
16ε0
q
d)
32ε0
a)

e) Ninguna de las anteriores
Aplicando la ley de Gauss,
Φe =

¨

~ · n̂ dS =
E

ˆ π/3 ˆ π/2

q
q
r
sin
θ
dθ
dφ
4πε0 r 2
12ε0

#### Problema 1.23.
Tres cascarones esféricos concéntricos A, B y C, de espesores despreciables, poseen radios a, b y c y
densidades de carga +σ, −σ, y +σ, respectivamente, como muestra la figura. Si los cascarones A y C
están al mismo potencial, ¿cuál es la relación entre a, b y c?

a) a = b + c

---

### Página 24

b) a = b − c
c) a = −b + c
d) a = −b − c
e) Ninguna de las anteriores
Sabemos, por la ley de Gauss, que el campo eléctrico de un cascarón esférico de radio R y densidad
superficial de carga σ es
 2
R
4πR
σ
σ
~ =
E
ρ̂
∀r > R
ρ̂ =
4πε0 r
ε0 r
Con ello, el campo eléctrico de la configuración es:

~0









σ a2


ρ̂


ε0 r 2


~ total =
E
σ a2 − b2



ρ̂


ε0 r 2







σ a2 − b2 + c2


ρ̂

ε0
r2

0<r
a<r<b

b<r<c

c<r

Ahora, calculamos ambos potenciales tomando como referencia el infinito a potencial nulo:
ˆ c
ˆ ∞
~ · d~r =
~ · d~r
V (c) = −
E
E
∞
c
ˆ
σ(a2 − b2 + c2 ) ∞ dr
ε0
r2
c 
σ(a − b + c ) 1
ε0
c
ˆ a
ˆ ∞
~ · d~r =
~ · d~r
V (a) = −
E
E
∞
a




 
σa2 1 1
σ(a2 − b2 ) 1 1
σ(a2 − b2 + c2 ) 1
+
+
−
−
ε0 a b
ε0
b c
ε0
c

---

### Página 25

Igualando y simplificando,

a



1 1
−
a b




1 1
+ (a − b )
= 0
−
b c
a2 b2
+
= 0
a−b−
c
c
a2 − b2
a−b =
c
a+b
1 =
c



y, por tanto,
a+b=c

#### Problema 1.24.
Se tiene un medio anillo de radio R con densidad lineal de carga λ constante. Determine la magnitud
del campo eléctrico en el punto O de la figura:

y

λ
b

O
R

a) E =

λ
4πε0 R

b) E =

λ
8πε0 R

c) E =

λ
6πε0 R

d) E =

λ
2πε0 R

e) Ninguna de las anteriores

x

---

### Página 26

~ = R ρ̂, con π ≤ θ ≤ 3π . Así, y dado que dq = λR dθ,
En este caso, ~r = ~0 y R
ˆ 3π/2
ˆ 3π/2
~
dq (~r − R)
λ
~
E(~r) =
ρ̂ dθ
=−
~ 3
4πε0 π/2 k~r − Rk
4πε0 R π/2
Como el vector unitario radial depende del ángulo, debemos descomponerlo en coordenadas cartesianas:
"ˆ
#
ˆ 3π/2
ˆ 3π/2
3π/2
λ
λ
λ
~ r) = −
E(~
ρ̂ dθ = −
cos θ dθ ı̂ +
ı̂
sin θ dθ ̂ =
4πε0 R π/2
4πε0 R π/2
2πε0 R
π/2

#### Problema 1.25.
Una carga se encuentra en una esquina de un cubo de arista L, como indica la figura. ¿Cuál es el flujo
eléctrico que pasa por la cara gris de este cubo?

b

q

q
16ε0
q
b) Φe =
8ε0
q
c) Φe =
4ε0
q
d) Φe =
32ε0
q
e) Φe =
24ε0
a) Φe =

En vez de realizar alguna integral, abordaremos este problema desde una perspectiva cualitativa
utilizando argumentos de simetría. Consideremos que nuestra carga se encuentra en el centro de

---

### Página 27

un cubo imaginario de lado 2L. El flujo a través de la superficie de este cubo es q/ε0 por la ley
de Gauss, dado que se trata de una superficie cerrada que contiene carga. Ahora imaginemos que
dividimos cada cara del cubo mayor en cuatro cuadrados de largo L. Por simetría, el flujo a través
de cada cuadrado es el mismo, y hay en total 24 de dichos cuadrados (dado que hay 6 caras), por
q
.
lo que el flujo a través de cada cuadrado es
24ε0
Ahora, simplemente notemos que si cortásemos el cubo mayor en 8 cubos de largo L, entonces cada
uno de los cuadrados mencionados en el párrafo anterior corresponderían a una cara de uno de los
cubos en el cual la carga está en la esquina.
Por otra parte, observe que la porción de flujo que viene de la carga no atraviesa las caras del cubo
que tocan la carga. Solo un octavo del flujo total atraviesa las caras de cada uno de los cubos de
arista L. Entonces, por cada una de las tres caras opuestas a la carga hay un tercio del flujo en cada
cubo, puesto que las otras tres caras (adyacentes a la carga) son paralelas al campo eléctrico, y con
ello no hay flujo a través de ellas. Este argumento también nos lleva a la conclusión de que el flujo
q
a través de la cara marcada es
.
24ε0

#### Problema 1.26.
Considere la siguiente densidad de carga expresada en coordenadas cartesianas:
 2

x + y2 + z2
ρ(x, y, z) = ρ0
a2
¿Cuánto vale el módulo E del campo eléctrico en todo el espacio?
ρ0
a) E =
ε0



[x2 + y 2 + z 2 ]3/2
5a2



ρ0
b) E =
ε0



[x2 + y 2 + z 2 ]3/2
4a2



ρ0
c) E =
ε0



[x2 + y 2 + z 2 ]3/2
3a2



ρ0
d) E =
ε0



[x2 + y 2 + z 2 ]3/2
2a2



e) Ninguna de las anteriores
En coordenadas esféricas, la densidad de carga toma la siguiente forma:
 r 2
ρ(r) = ρ0
a

---

### Página 28

Aplicando la ley de Gauss en coordenadas esféricas, utilizando como superficie gaussiana una esfera
de radio r arbitrario,
‹
~ · n̂ dS = qenc
E
ε0
S
˚
4πr E =
ρ dV
ε0
ˆ
1 4πρ0 r ′ 4 ′
· 2
r dr
ε0
a
1 4πρ0 r 5
· 2 ·
ε0
a
Finalmente,
ρ0 r 3
ρ0
E=
ε0 5a
ε0



[x2 + y 2 + z 2 ]3/2
5a2



#### Problema 1.27.
Se tiene un conductor cilíndrico neutro de radio exterior ra y radio interior rb . La cavidad interior
(r < rb ) está llena con un material no conductor con densidad de carga ρ(r) = µ/r, donde r es la
distancia al eje de simetría del cilindro (ver figura). En la aproximación en que el cilindro es infinito,
determine el potencial eléctrico en las regiones r < rb y r > ra . Asuma que V (0) = 0.

ra

b

ρ(r)

rb

conductor

µrb  rb 
µr
y V (r > ra ) =
ln
ε0
ε0
r
µra  ra 
µrb  rb 
y V (r > ra ) =
ln
ln
b) V (r < rb ) =
ε0
r
ε0
r
h


i
µr
ra
µrb
ln
−1
y V (r > ra ) =
c) V (r < rb ) = −
ε0
ε0
r
i
i
µrb h  rb 
µra h  ra 
d) V (r < rb ) =
ln
− 1 y V (r > ra ) =
ln
−1
ε0
r
ε0
r
a) V (r < rb ) = −

---

### Página 29

e) Ninguna de las anteriores
Dada la simetría del problema, calcularemos primero el campo eléctrico vía ley de Gauss. Para
r < rb ,
‹
~ · n̂ dS = qenc
E
ε0
S
ˆ
2πL r
ρ(r ′ ) r ′ dr ′
2πrL E(r) =
ε0 0
2πrLµ
ε0
µ
∴ E(r) =
ε0
Para rb < r < ra ,
‹

~ · n̂ dS = qenc
E
ε0

S

ˆ
2πL rb
ρ(r ′ ) r ′ dr ′
2πrL E(r) =
ε0 0
2πrb Lµ
ε0
µrb
∴ E(r) =
ε0 r
donde hemos usado que el conductor es neutro. Fijando V (0) = 0, el potencial en la región interior
es:
ˆ r
~ · d~r
V (r < rb ) − V (0) = −
E

µr
= −
ε0
µr
∴ V (r < rb ) = −
ε0

En la región exterior,
ˆ r

~ · d~r
E
 
µrb
r
= −
ln
ε0
ra
i
µrb h  ra 
ln
−1
∴ V (r > ra ) =
ε0
r

V (r > ra ) − V (ra ) = −

ra

donde hemos usado que el potencial debe ser continuo y que V (ra ) = V (rb ) = −µrb /ε0 al tratarse
de un conductor.

---

### Página 30

#### Problema 1.28.
En el problema anterior, ¿cuál es la densidad de carga en la superficie interior del conductor?
a) σ = µ
b) σ = 2µ
c) σ = −µ
d) σ =

µ

e) Ninguna de las anteriores
Al tratarse de un conductor, el flujo eléctrico a través de un cilindro de radio rb < r < ra y largo L
es cero. Luego, la carga encerrada po dicha superficie debe ser cero. De acuerdo a lo calculado en el
problema anterior, la carga total del cilindro interior es Q = 2πrb Lµ. Por tanto, la carga superficial
debe ser Qb = −Q = −2πrb Lµ. Así,
σb =

Qb
2πrb Lµ
=−
= −µ
Ab
2πrb L

#### Problema 1.29.
Entre dos planos geométricos infinitos y paralelos ubicados en x = ±a se encuentra una distribución de
carga homogénea con densidad ρ. El campo eléctrico en la región |x| > a es:
ρa
ı̂
2ε0
~ = −signo(x) ρa ı̂
b) E
ε0
~ = signo(x)
a) E

~ = −signo(x)
c) E
~ = signo(x)
d) E

ρa
ı̂
2ε0

ρa
ı̂
ε0

e) Ninguna de las anteriores
Tomemos como superficie gaussiana un cilindro de radio R, orientado de forma perpendicular a
los planos y cuyas tapas se ubican en ±x (|x| > a). Por argumentos de simetría, planteamos que

---

### Página 31

~ = ±E(x) ı̂ con el signo según corresponda de acuerdo a la dirección del campo (hacia la derecha
E
para x > a y hacia la izquierda para x < −a). Así, por la ley de Gauss,
‹
~ · n̂ dS = qenc
E
ε0
S
h
i
πR2 E(x) − E(−x) = 2aρπR2
2πr 2E(x) =

∴ E(x) =

ρa
ε0

donde hemos usado la simetría E(−x) = −E(x) del campo. Así,
 ρa

(x > a)

 ε0
~ = signo(x) ρa ı̂
=⇒ E
E(x) =

ε0

 − ρa (x < −a)
ε0

#### Problema 1.30.
En la figura se muestra un plano infinito (MUY grande) localizado en y = 0 (i.e. el plano XZ) con
densidad superficial de carga σ = q/(25πd2), con d una constante positiva. Además, se tiene una carga
puntual q en el punto (x, y, z) = (0, −d, 0). Entonces, el campo eléctrico producido por el sistema en el
punto (0, 2d, 4d) es:
z

σ

q
b

y

x



q
̂
+
k̂
500πε0 d2


q
~ =
̂
+
k̂
b) E
500πε0 d2


q
~
c) E =
17 ̂ + 4 k̂
500πε0 d2
~ =
a) E

---

### Página 32



q
̂
+
k̂
500πε0 d2


q
~
e) E =
15 ̂ + 4 k̂
500πε0 d2

~ =
d) E

~q y E
~ σ a los campos eléctricos creados por la carga puntual y el plano infinito, respectiLlamemos E
vamente. Por el principio de superposición, tenemos que el campo en el punto pedido ~r = (0, 2d, 4d)
es:
~ r) = E
~ q (~r) + E
~ σ (~r)
E(~
El campo eléctrico de un campo infinito es:
q
~ σ (~r) = σ ̂ =
E
̂
2ε0
50πε0d2
~ =
Por otra parte, para calcular el campo de una carga puntual, utilizamos el hecho de que R
(0, −d, 0):
~
~r − R
q
~ q (~r) = q
(3 ̂ + 4 k̂)
E
~
4πε0 k~r − Rk
500πε0 d2
~ = (0, 3d, 4z) y k~r − Rk
~ = 5d. Finalmente,
donde hemos utilizado que ~r − R


q
~ r) =
E(~
̂
+
k̂
500πε0d2

#### Problema 1.31.
Considere la situación expuesta el Problema 1.30. El trabajo mínimo que debe realizar un agente externo
para transportar una carga de prueba Q desde el punto (0, d, d) hasta el punto (0, d, −d) es:
a) W = +

5qQ
8πε0 d

b) W = −

13qQ
25πε0 d

c) W = +

13qQ
50πε0 d

d) W = −

5qQ
8πε0 d

e) Ninguna de las anteriores

---

### Página 33

El trabajo requerido, realizado por un agente externo, es equivalente al producto de la carga Q y la
diferencia de potencial ∆V = V (~rf ) − V (~ri ) entre estos dos puntos. Por superposición, es claro que
∆V = ∆Vq + ∆Vσ
Notemos que las superficies equipotenciales de un plano infinito también son planos paralelos al
original. Dado que los puntos inicial y final están contenidos en el plano y = d, que es una superficie
equipotencial para el plano cargado, entonces ∆Vσ = 0. Por otra parte, las superficies equipotenciales
de una carga puntual son esferas centradas en la carga. Los puntos inicial y final están a la misma
distancia de la carga puntual, por lo que pertenecen a la misma equipotencial. Así, ∆Vq = 0. En
síntesis,
W = Q ∆V = 0 J

#### Problema 1.32.
Considere la situación expuesta el Problema 1.30. Asuma que Q y q son de igual signo. Suponga que
ponemos una carga de prueba Q en reposo en el punto (0, d, 0). Entonces, la energía cinética K de Q
en el punto (0, 2d, 0) es:
a) K =

47 qQ
300 πε0 d

b) K =

37 qQ
600 πε0 d

c) K =

41 qQ
400 πε0 d

d) K =

17 qQ
500 πε0 d

e) K =

21 qQ
200 πε0 d

De la conservación de energía,
U(~ri ) = K + U(~rf )

−→

h
i h
i
K = U(~ri ) − U(~rf ) = Uq (~ri ) − Uq (~rf ) + Uσ (~ri ) − Uσ (~rf )

donde ~ri = (0, d, 0) y ~rf = (0, 2d, 0). Es fácil ver que:
Uσ (~ri ) − Uσ (~rf ) = Q ·

σ
qQ
·d =
2ε0
50πε0 d

---

### Página 34

En el caso de la carga puntual,
Uq (~r) =

qQ
~
4πε0k~r − Rk

−→

qQ
Uq (~ri ) − Uq (~rf ) =
4πε0



−
2a 3a



qQ
24πε0d

Finalmente, sumando ambas contribuciones,
K=

37 qQ
600 πε0 d

#### Problema 1.33.
En t = 0, una carga Q > 0 se encuentra en el centro de una esfera conductora de radio R = 1 m. Si la
carga se mueve con una velocidad constante de 2 m/s en dirección radial, ¿cuánto vale el flujo eléctrico
a través de la esfera en t = 0.3 s?
a) Φe = 0
b) Φe = 0.3Q/ε0
c) Φe = Q/ε0
d) Φe = 2Q/ε0
e) Φe = 3Q/ε0
Notemos que la distancia recorrida por la carga Q es:
d = v ∆t = 0.6 m < 1 m = R
por lo que la carga sigue estando al interior de la esfera. Así, el flujo eléctrico -vía ley de Gauss- es:
Φe =

Q
ε0

#### Problema 1.34.
Considere una línea semicircular cargada en el plano Y Z con ecuaciones y 2 + z 2 = R2 , z ≥ 0. El
semicírculo posee una densidad de carga no uniforme λ(θ) = Qθ/(πR), donde Q tiene dimensiones de
carga y θ es el ángulo de cada punto del semicírculo medido desde el eje Y . Determine el potencial
eléctrico (con V = 0 en el infinito) en un punto x del eje X.
a) V (x) =

Q
√
8πε0 R2 + x2

---

### Página 35

b) V (x) =

Q
√
4πε0 R + x2

c) V (x) =

QR
√
8ε0 R2 + x2

d) V (x) =

QR
√
4ε0 R2 + x2

e) V (x) =

Q
√
8ε0 R2 + x2

Realizando las siguientes definiciones,
~ = R ρ̂
R

~r = x ı̂

dq = Rλ(θ) dθ

tenemos que:
ˆ π
dq
V (~r) =
~
4πε0 0 k~r − Rk
ˆ π
Q
√
θ dθ
4π 2 ε0 R2 + x2 0
Q
√
8ε0 R2 + x2

#### Problema 1.35.
Dos esferas metálicas idénticas de masa m y carga q están suspendidas por una cuerda de largo ℓ como
muestra la figura. Despreciando las masas de las cuerdas, encuentre |q| si el ángulo de equilibrio es θ.
Considere g como la aceleración de gravedad.

ℓ

θ

b

b

√
a) |q| = 4ℓ sin θ πmgε0 tan θ
√
b) |q| = 4ℓ sin θ πmgε0
√
c) |q| = 4ℓ πmgε0 tan θ

---

### Página 36

√
d) |q| = 4ℓ πmgε0
e) Ninguna de las anteriores
Aplicando la condición de equilibrio en el eje Y :
mg = T cos θ

−→

T =

mg
cos θ

En el eje X,
T sin θ =

q2
4πε0 d2

−→

p
p
|q| = 2d πmgε0 tan θ = 4ℓ sin θ πmgε0 tan θ

con d = 2ℓ sin θ la distancia que separa a ambas cargas.

#### Problema 1.36.
La molécula de agua tiene un momento dipolar de p = 6.3 × 10−30 C m. Una muestra contiene 1021
moléculas, todas con su momento dipolar alineado en la dirección de un campo eléctrico externo de
magnitud E = 2.5 × 105 N/C. El trabajo necesario para rotar todas las moléculas hasta una orientación
perpendicular al campo es:
a) 0 J
b) 2.5 × 10−26 J
c) 2.5 × 10−9 J
d) 1.6 × 10−24 J
e) 1.6 × 10−3 J
El trabajo realizado por un agente externo para orientar un molécula viene dado por:
W = N∆U = N(Uf − Ui )
~ = −pE cos θ la energía potencial de un dipolo, donde
con N el número de moléculas y U = −~p · E
θ es el ángulo entre el campo eléctrico y el momento dipolar. En este caso,
Ui = −pE cos θi = −1.575 × 10−24 J ≈ −1.6 × 10−24 J
pues θi = 0, mientras que
Uf = −pE cos θf = 0 J
porque θf = π/2. Con ello,
W = (1021 )(1.6 × 10−24 J) = 1.6 × 10−3 J

---

### Página 37

#### Problema 1.37.
Una carga puntual q > 0 se ubica a una distancia r de un dipolo eléctrico p~, como muestra la figura.
Asuma que el dipolo es muy pequeño, i.e. que la separación d entre las cargas del dipolo satisface d ≪ r.
La fuerza que experimenta la carga es:
b

q

p~

qp
hacia la derecha
4πε0 r 3
qp
hacia la izquierda
b) F =
2πε0 r 3
qp
c) F =
hacia la izquierda
4πε0 r 3
qp
hacia la derecha
d) F =
2πε0 r 3
a) F =

e) Ninguna de las anteriores
Sabemos que el campo eléctrico generado por un momento dipolar ~p en el origen está dado por:
i
1 h
~ dip (~r) =
3(~
p
·
r̂)r̂
−
p
~
E
4πε0 r 3
En nuestro caso, ~p = p ı̂ y ~r = −r ı̂ (r̂ = − ı̂), por lo que el campo toma la siguiente forma:
~ dip (~r) =
E

i
1 h
p
−
3(−p)
ı̂
−
p
ı̂
ı̂
4πε0 r
2πε0 r 3

De la ley de Coulomb,
~ dip (~r) =
F~ = q E

qp
ı̂
2πε0r 3

#### Problema 1.38.
¿Cuánta energía es necesaria para cargar una esfera conductora de radio R desde una carga Q hasta
una carga Q′ > Q (diferencia de energía acumulada con Q y Q′ )?
a)

(Q′ + Q)(Q′ − Q)
4πε0 R

(Q′ + Q)2
b)
4πε0 R
c)

(Q′ − Q)2
8πε0 R

---

### Página 38

d)

Q′ 2 − Q2
8πε0R

e) Ninguna de las anteriores
~ viene dada por:
Recordemos que la energía potencial asociada a un campo eléctrico E
˚
ε0
~ 2 dV
U=
kEk
R3

En este caso, el campo eléctrico de la esfera conductora de carga q es fácilmente calculable vía ley
de Gauss:

~0
(r < R)


~ r) =
E(~
q


ρ̂ (r > R)
4πε0 r 2
Con ello,

ε0
U(q) =

ˆ ∞

¨

q
4πε0

2

dΩ
R
2 ˆ ∞

dr
q
= 2πε0
4πε0
R r
q2
8πε0 R

Finalmente,
∆U = U(Q′ ) − U(Q) =

dr
r2

Q′ 2 − Q2
8πε0 R

#### Problema 1.39.
Sobre un disco plano de radio R se distribuye una carga superficial que varía radialmente de la forma:

 r 2

 σ0
(r < R)
R
σ(r) =


(r > R)

siendo r la distancia al centro del disco y σ0 > 0. Calcule el potencial eléctrico V en el eje Z perpendicular
al disco y que tiene su origen en el centro del mismo. Asuma que V (∞) = 0. La siguiente integral puede
resultar de utilidad:
ˆ
√
t
√
dt = (t − 2z 2 ) t + z 2
t + z2
i
√
√
σ0 h 2
2 + R2 ) + R2 z 2 + R2
z
a) V (0, 0, z) = −
2z
(|z|
−
6ε0 R2

---

### Página 39

i
√
√
σ0 h 2
2 + R2 ) + R2 z 2 + R2
2z
(|z|
+
z
6ε0R2
i
√
√
σ0 h 2
2z (|z| − z + R ) + R z + R
c) V (0, 0, z) = +
6ε0R2
i
√
√
σ0 h 2
2 + R2 ) − R2 z 2 + R2
d) V (0, 0, z) = +
z
2z
(|z|
−
6ε0R2
i
√
√
σ0 h 2
2 + R2 ) + R2 z 2 + R2
e) V (0, 0, z) = −
2z
(|z|
+
z
6ε0 R2
b) V (0, 0, z) = +

Sean:
~r = z k̂

~ = r ρ̂
R

dq = σ(r) dA = σ(r)r dr dθ

Con ello,
V (~r) =
4πε0

ˆ 2π ˆ R

ˆ R

dq

~
k~r − Rk
σ0
r 3 dr
√
(Sea t = r 2 )
2ε0R 0
r +z
ˆ R2
t dt
σ0
√
4ε0R 0
t + z2
h
iR2
√
σ0
t
+
z
(t
−
2z
)
6ε0R2
i
√
σ0 h 2
2 + z 2 + 2z 2 |z|
R
(R
−
2z
)
6ε0R2
i
√
√
σ0 h 2
2 + z 2 ) + R2 R2 + z 2
2z
(|z|
−
R
6ε0R2

#### Problema 1.40.
Considere una esfera conductora con carga Q y radio R1 , rodeada por un cascarón esférico conductor
concéntrico. Dicho cascarón es neutro y posee un radio interno R2 y un radio externo R3 (R1 < R2 < R3 ).
¿Cuál es la energía almacenada en el sistema?
 2
Q
a) −
+
+
R1 R2 R3 4πε0
 2

Q
−
+
b)
R1 R2 R3 8πε0
 2

Q
+
−
c)
R1 R2 R3 8πε0

 2
Q
d)
−
+
R1 R2 R3 4πε0


---

### Página 40

e) Ninguna de las anteriores
En este caso, el campo eléctrico puede ser calculado empleando la ley de Gauss de forma directa:

~0
(r < R1 )







Q



ρ̂ (R1 < r < R2 )

 4πε0 r 2
~ r) =
E(~


~0

(R2 < r < R3 )







Q


ρ̂
(R3 < r)
4πε0 r 2
Por tanto, la energía potencial almacenada en el sistema es:

2 ¨
ˆ R2
ˆ ∞ 
q
dr
dr
ε0
dΩ
+
U =
2 4πε0
R1 r
R3 r
2 


q
−
+
= 2πε0
4πε0
R1 R2 R3


Q2
−
+
8πε0 R1 R2 R3

#### Problema 1.41.
Dos cilindros concéntricos de radios a y b (a < b) y largo L ≫ b están cargados con cargas −Q en el
cilindro interior y +Q en el exterior. ¿Cuál es la capacitancia del sistema?
a)

4πε0 L
ln(b/a)

b) 4πε0 L ln(b/a)
c) 2πε0 L ln(b/a)
d)

2πε0 L
ln(b/a)

e) Ninguna de las anteriores
Para obtener la capacidad, debemos primero obtener el campo eléctrico en cualquier parte en la
región entre ambos conductores. Debido a la simetría cilíndrica del sistema, elegimos por superficie

---

### Página 41

gaussiana un cilindro coaxial con longitud ℓ < L y radio a < r < b. Usando la ley de Gauss, con un
campo radial, tenemos
Φe = E(r)2πℓr =

2πaℓσ
qenc
ε0
ε0

−→

E(r) =

aσ
ε0 r

La diferencia de potencial está dada por:
∆V

ˆ b

~ · d~r
= φ(b) − φ(a) = −
E
a
ˆ b
= −
E(r) dr
a
ˆ
aσ
aσ b dr
= − ln (b/a)
= −
ε0 a r
ε0

donde el camino de integración tiene la dirección radial del campo eléctrico. De esta forma, tenemos
que:
Q
2πε0 L
σ2πaL
C=
= aσ
|∆V |
ln (b/a)
ln (b/a)
ε0

#### Problema 1.42.
Un cilindro conductor hueco es colocado entre dos grandes placas paralelas de carga opuesta. ¿Qué
figura representa mejor las líneas equipotenciales ara esta situación?

a) Figura A
b) Figura B
c) Figura C
d) Figura D
e) Figura E

---

### Página 42

#### Problema 1.43.
La figura muestra las líneas de campo producidas por 4 cargas puntuales. Determine si:

a) 2 cargas son positivas y 2 son negativas
b) 3 cargas son positivas y 1 es negativa
c) 1 carga es positiva y 3 son negativas
d) Todas las cargas son del mismo signo
e) No hay suficiente información para saber
#### Problema 1.44.
Se tiene una barra de longitud a en la posición que se muestra en la figura abajo. La barra tiene una
carga positiva Q uniformemente distribuida sobre ella. Una carga puntual positiva q se encuentra a una
distancia a + r del origen sobre el eje X, como muestra la figura. La fuerza que siente la carga q es:
y

a

r
b

q

Q
a) F~ =

qQ
ı̂
4πε0 (r + a/2)2

b) F~ = −

qQ
ı̂
4πε0 (r + a/2)2

c) F~ = −

qQ
ı̂
4πε0 (r − a/2)2

d) F~ =

qQ
ı̂
4πε0 r(a + r)

x

---

### Página 43

e) F~ =

qQ
ı̂
4πε0 r(a − r)

Sean:
~ = x ı̂, x ∈ [0, a]
R

~r = (a + r) ı̂

dq =

Q
dx
a

El campo eléctrico generado por la barra en el punto en que se ubica la carga puntual es:
~ r) = 1
E(~
4πε0

ˆ a

Finalmente,



ˆ a
~
a
Q
Q
dq (~r − R)
dx
Q
ı̂
ı̂
ı̂
~
4πε0 a 0 (a + r − x)
4πε0a (a + r)r
4πε0 (a + r)r
k~r − Rk
~ = qQ
F~ = q E
ı̂
4πε0 (a + r)r

#### Problema 1.45.
Se tienen dos cargas negativas −Q fijas en dos vértices de un cuadrado de lado L, como se muestra en
la figura. También se tiene una carga positiva +Q que se puede mover sobre la diagonal del cuadrado,
a una distancia d del punto P . Determine el valor de d para que el campo eléctrico en el punto P sea
cero:

−Q

L

b

P
b

d

L
b

L

+Q
b

L
a) d = L(2)1/4
√
b) d = L 2
L
c) d = √
 1/4
d) d = L
e) d = L √

−Q

---

### Página 44

Sea P el origen del sistema de coordenadas. El campo eléctrico producido por la carga −Q ubicada
en (−L, 0) es:
~ 1 (P ) = Q ı̂
E
4πε0L2
Por otra parte, el campo eléctrico producido por la carga −Q ubicada en (0, −L) es:
~ 2 (P ) =
E

Q
̂
4πε0 L2

Finalmente, el campo eléctrico producido por la carga +Q es:
~ 3 (P ) = −
E


Q 
cos
θ
ı̂
+
sin
θ
̂
4πε0 d2

donde θ = π/4. Es fácil ver que, para un campo eléctrico total nulo en P , se debe cumplir la siguiente
relación:


 1/4
Q
Q
= √
−→
d=L
4πε0 L
2 4πε0d

#### Problema 1.46.
Un cascarón cilíndrico de largo infinito, con densidad volumétrica de carga homogénea ρ, radio interior
2a y radio exterior 4a es ubicado en el origen del plano XY con su eje a lo largo del eje Z. Además, por
el punto (0, a, 0) pasa un alambre infinito perpendicular al plano XY (paralelo al eje Z) con densidad
de carga lineal λ como es mostrado en la figura. ¿Cuál debiese ser la relación entre λ y ρ para que el
campo eléctrico en el punto P = (0, 3a, 0) sea cero?
y

P
b

b

λ
x

2a
4a

a)

λ
= − πa2
ρ

b)

λ
= − πa2
ρ

c)

λ
= πa2
ρ

---

### Página 45

d)

λ
= 10πa2
ρ

e)

λ
= − πa2
ρ

Aplicando la ley de Gauss sobre un cilindro de radio r = 3a (que corresponde al punto P ) y largo
L,
ˆ
5ρπa2 L
2πρL 3a
~ c (P ) = 5aρ ̂
−→
E
r dr =
2π(3a)L Ec (P ) =
ε0
ε0
6ε0
2a
El campo eléctrico, debido al alambre infinito, en el punto P es:
λ
̂
2πε0 (2a)

~ a (P ) =
E

puesto que la distancia entre el punto y el alambre es 3a − a = 2a. La magnitud total del campo
debe ser nulo en P , por lo que se debe cumplir la siguiente relación:
5aρ
λ
+
=0
6ε0
4πε0a

−→

λ
= − πa2
ρ

#### Problema 1.47.
Una carga Q positiva se encuentra dentro de una esfera como en la figura. ¿Qué se puede decir acerca
del flujo del campo eléctrico en los hemisferios norte y sur? No considere las tapas de los hemisferios.

Norte

b

Q

a) El flujo es mayor en el hemisferio norte que en el hemisferio sur
b) El flujo es mayor en el hemisferio sur que en el hemisferio norte
c) El flujo es el mismo en ambos hemisferios
d) El flujo en el hemisferio norte es
e) El flujo en el hemisferio sur es

Q
2ε0

Q
ε0

---

### Página 46

#### Problema 1.48.
Un conductor esférico relleno y neutral de radio R tiene una cavidad vacía esférica de radio R/2. El
centro de la cavidad está desplazado del centro del conductor por R/4 en dirección positiva del eje X.
Se coloca una carga Q en el centro del conductor, como muestra la figura. ¿Cuanto vale la magnitud
del campo eléctrico a una distancia 2R en dirección positiva del eje X (punto P )?

b

Q

2R

×

P

R/2
R

~ )k =
a) kE(P

Q
πε0 R2

~ )k =
b) kE(P

Q
2πε0 R2

~ )k =
c) kE(P

Q
4πε0 R2

~ )k =
d) kE(P

Q
16πε0 R2

e) Ninguna de las anteriores
Recordemos que cualquier carga al interior de una cavidad vacía en un conductor será vista desde
fuera como una carga puntual localizada en el origen. Así, el campo eléctrico fuera de la esfera
conductora será, simplemente,
~ = Q ρ̂
E
4πε0r 2
Así, el campo en el punto solicitado viene dado por:
~
E(2R)

Q
ı̂
16πε0R2

#### Problema 1.49.
Un cascarón esférico tiene un radio interior R1 = 1 m y un radio exterior R2 = 3 m. El cascaron es un
aislante con una densidad de carga neta positiva ρ = 108×10−10 C/m3 . Aproximando ε0 = 9×10−12 C/V,
calcule la magnitud del campo eléctrico en el punto Rb = 2 m.
~ b )k = 0 V/m
a) kE(R

---

### Página 47

~ b )k = 700 V/m
b) kE(R
~ b )k = 10 V/m
c) kE(R
~ b )k = 900 V/m
d) kE(R
~ b )k = 50 V/m
e) kE(R
Por la ley de Gauss, y dada la simetría del problema,
ΦE = 4πr 2 E(r) =

qenc
ε0

−→

E(Rb ) =

qenc
4πε0 Rb 2

En este caso,
qenc =

¨

ˆ Rb


4πρ  3
Rb − R1 = 4 · 36 · 7π × 10−10 C
dΩ
ρ r dr =
R1

Reemplazando,
E(Rb ) =

4 · 36 · 7π × 10−10
V/m = 700 V/m
(4π)(9 × 10−12 )(4)

#### Problema 1.50.
Un plano infinito y aislante está cargado con densidad de carga σ > 0. ¿Entre cuáles puntos el valor
absoluto del voltaje (diferencia de potencial) es máximo?

C1

b

A1
b

A2

b

B1
b

B2
b

b

C2
b

b

D1

D2

a) Entre A1 y A2
b) Entre B1 y B2

b

b

E1

E2

---

### Página 48

c) Entre C1 y C2
d) Entre D1 y D2
e) Entre E1 y E2
Supongamos que el plano yace en el eje Y , y que el eje X se extiende de derecha a izquierda. En
~ = E0 ı̂ para x > 0 y E
~ = −E0 ı̂ para x < 0, con E0 = σ/2ε0 . Entonces,
ese caso, E


−E0 (x > 0)

 −E0 x (x > 0)
dV
−→
V =
= −E0 |x|


dx
E0 (x < 0)
E0 x (x < 0)

y el potencial solo depende de la componente X. Por tanto, la diferencia de potencial entre cada
par de puntos es:
∆VA
∆VB
∆VC
∆VD
∆VE

3E0
5E0

#### Problema 1.51.
Una esfera maciza conductora de radio R está cargada con una carga q > 0 C. Calcule el potencial
eléctrico φ a una distancia de R/2 del centro de esta esfera asumiendo que el potencial eléctrico es V0
en el infinito.
q
2πε0 R
q
b) φ =
4πε0 R
q
+ V0
c) φ =
4πε0 R
q
d) φ =
+ V0
2πε0 R
a) φ =

e) φ = 0
El campo eléctrico fuera de la esfera conductora es:
~ > R) =
E(r

q
ρ̂
4πε0 r 2

---

### Página 49

Por otra parte,
φ(R) − φ(∞) = −

ˆ R
∞

~ · d~r =
E

q
4πε0R

−→

φ(R) =

q
+ V0
4πε0 R

Finalmente, dado que se trata de un conductor,
φ(R/2) = φinterior = φsuperficie = φ(R) =

q
+ V0
4πε0 R

#### Problema 1.52.
Una carga q0 = 100 µC se encuentra fija en el centro del sistema de coordenadas cartesianas, mientras
que una segunda carga q = −1 µC pasa volando. En el tiempo t1 la carga q tiene la posición ~r1 =
(−45, 0, 0) cm y rapidez v1 . Un tiempo t2 más tarde (t2 > t1 ) se ubica en ~r2 = (0, 20, 0) cm con rapidez
v2 . ¿Cuánta energía cinética gano la carga q? Usar (4πε0)−1 ≈ 9 × 109 V m/C.
a) ∆Ecin = 2.5 J
b) ∆Ecin = 2.0 J
c) ∆Ecin = 1.5 J
d) ∆Ecin = 1.0 J
e) ∆Ecin = 0.5 J
Por conservación de energía,
mv1

E1 = E2
qq0
mv2 2
qq0
+
+
4πε0 r1
4πε0 r2
mv2
mv1 2
∴ ∆Ecin =
−
2  2 
qq0
−
4πε0 r1 r2


qq0 r2 − r1
4πε0
r2 r1
= (−10

−6

C)(100 × 10

−6

(9 × 10−1 )(0.25)
J
0.09
= 2.5 J

C)(9 × 10 V m/C)



0.2 m − 0.45 m
(0.2 m)(0.45 m)



---

### Página 50

#### Problema 1.53.
Dos cargas q1 = q y q2 = 2q están ubicados en las posiciones ~r1 = (−d, 0, 0) y ~r2 = (d, 0, 0), respectivamente, en un sistema de coordenadas cartesianas. Una superficie equipotencial con potencial eléctrico
φ0 pasa por el punto (0, y, 0). ¿Cuáles son los valores correctos para la coordenada y, suponiendo que
φ(∞) = 0 V?

3q 2
a) y = ±
−d
4πε0 φ0
s
2
q
b) y = ±
− d2
2πε0 φ0
s
2
3q
+ d2
c) y = ±
4πε0 φ0
s
2
3q
− d2
d) y = ±
4πε0 φ0


e) y =

3q 2
±d
4πε0φ0

Por el principio de superposición,
φ(x, y, z) = φq1 + φq2 =
4πε0
De la condición de superficie equipotencial,

2q
q
p
+p
(x + d) + y
(x − d)2 + y 2

φ0 = φ(0, y, 0)
3q
p
4πε0 d2 + y 2
p
3q
d2 + y 2 =
4πε0 φ0

2
3q
y =
− d2
4πε0 φ0
s
2
3q
− d2
y = ±
4πε0 φ0

!

---

### Página 51

Condensadores, dieléctricos y corriente eléctrica

Ecuaciones de Maxwell en uno de los muros exteriores de la Universidad de Varsovia

---

### Página 52

#### Problema 2.1.
Considere el sistema de condensadores (C1 , C2 y C3 ) conectados por conductores perfectos, tal como
se muestra en la figura. Los extremos a y b están a una diferencia de potencial V0 = Va − Vb > 0. Si
asumimos que C1 = C, C2 = 2C y C3 = 3C, tenemos que la suma de la magnitud de la carga que
tienen los condensadores C1 y C2 (Q = Q1 + Q2 ) está dada por:
a

+
C2
V0

b

a) Q =

CV0

b) Q =

CV0

C1
C3

−

c) Q = CV0
d) Q = CV0
e) Ninguna de las anteriores
Sea Vi la diferencia de voltaje en el condensador i−ésimo. Es claro que:
V1 = V0

∧

V2 + V3 = V0

De la relación entre el voltaje y la carga de un condensador,
Q1 = C1 V1 = CV0
Al estar en serie, los condensadores C2 y C3 poseen la misma carga Q2 . Entonces,
V0 = V2 + V3 =

Q2 Q2
5Q2
+
C2
C3
6C

−→

Q = Q1 + Q2 =

CV0

Finalmente,

Q2 = CV0

#### Problema 2.2.
En la figura se muestra un condensador de dos cilindros conductores coaxiales de radios a y c cargados

---

### Página 53

con cargas Q > 0 y −Q, respectivamente. Los cilindros tienen un largo L >≫ c. En el espacio entre
los cilindros hay dos materiales dieléctricos. Uno de ellos es de permitividad ε1 = (3/2)ε0 y está en el
espacio r ∈ (a, b), siendo r la distancia al eje de simetría. El segundo se encuentra en el espacio r ∈ (b, c)
y tiene permitividad ε0 = (5/4)ε0 . ¿Cuál de las siguientes expresiones es correcta para la magnitud del
campo eléctrico E(r) en la región r ∈ (b, c)?
c

b
ε2

ε1

a
b

+Q

−Q

a) E(r) =

3Q
5πε0 rL

b) E(r) =

2Q
5πε0 rL

c) E(r) =

Q
3πε0 rL

d) E(r) =

2Q
3πε0 rL

e) E(r) =

Q
5πε0 rL

Usando la ley de Gauss para el desplazamiento eléctrico, tenemos que:
2πrL D(r) = qlibre
Así,

~
D(r)










−→
~0

D(r) =

si 0 < r < a

Q
ρ̂ si a < r < c

2πrL






~0
si c < r

qlibre
2πrL

---

### Página 54

~ y E,
~ se tiene que:
De acuerdo a la relación entre los vectores D

~0
si 0 < r < a







Q



ρ̂ si a < r < b


2πε1 rL
~
D(r)
~
E(r)

ε

Q


ρ̂ si b < r < c


2πε2 rL






~0
si c < r

Finalmente,

~ < r < c) =
E(b

2Q
ρ̂
5πε0 rL

#### Problema 2.3.
Considere el sistema del Problema 2.2. La carga inducida (o de polarización) en la superficie interior
del dieléctrico ε1 (i.e. r = a) es:
a) −Q/4
b) −Q/2
c) −Q/3
d) −2Q/3
e) −Q
El vector de polarización satisface la siguiente relación:
~ − ε0 E
~ = (ε − ε0 )E
~
P~ = D
Reemplazando en el espacio r ∈ (a, b),

  Q
Q
~ < r < b) = ε0
ρ̂ =
ρ̂
P~ (a < r < b) = (ε1 − ε0 )E(a
2 3πε0 rL
6πrL

La densidad superficial de carga inducida es:


Q
Q
σa = P~ · n̂
ρ̂ · (− ρ̂) = −
6πaL
6πaL
r=a

Por tanto, la carga inducida es:
Qa = σa Aa = −

Q

---

### Página 55

#### Problema 2.4.
Considere el sistema del Problema 2.2. ¿Cuál de las siguientes afirmaciones es incorrecta?
a) La diferencia de potencial entre los puntos r = a y r = c es menor con los dieléctricos que en ausencia
de ellos, i.e. cuando hay vacío en la región r ∈ (a, c)
b) El campo eléctrico en la región r ∈ (b, c) disminuye si ε2 aumenta
c) La magnitud del campo eléctrico E(r) es discontinuo en r = b
d) La magnitud de la carga inducida (o de polarización) en la superficie exterior del dieléctrico ε2 (i.e.
r = c) es igual a Q
e) El vector de polarización P~ (r) es discontinuo en r = b
Al adicionar un dieléctrico, el campo eléctrico disminuye respecto a su valor en vacío, por lo que la
diferencia de potencial también lo hace. Esta disminución depende de la magnitud de la permitividad del dieléctrico. Por tanto, las alternativas (a) y (b) son correctas. Del cálculo realizado en los
problemas anteriores, notamos que el campo eléctrico no es continuo, debido a que existe una carga
superficial inducida. De la misma forma, notamos que el vector polarización también es discontinuo.
Con ello, las alternativas (c) y (e) son correctas. Finalmente, ya sea por cálculo directo o debido a
que no hay más opciones, descubrimos que la carga inducida en r = c no es igual a Q, por lo que la
alternativa (d) es incorrecta.

#### Problema 2.5.
Se tiene una esfera de material dieléctrico de permitividad ε1 = 5ε0 . La esfera está rodeada de un
conductor ideal cargado con carga Q, que a su vez está rodeado por un segundo material dieléctrico
de permitividad ε2 = 10ε0 . Finalmente, en la última capa, hay segundo un conductor con carga −Q
(como indica la figura). Los radios de cada una de las capas esféricas son R1 = R, R2 = 2R, R3 = 3R
y R4 = 4R, respectivamente.

La magnitud de los campos eléctricos, E1 y E2 en los dieléctricos ε1 y ε2 son, respectivamente,
a) E1 =

Q
y E2 = 0
20πε0 r 2

---

### Página 56

b) E1 =

Q
Q
y E2 =
20πε0 r
40πε0 r 2

c) E1 = 0 y E2 =
d) E1 =

Q
40πε0 r 2

Q
Q
y
E
40πε0 r 2
20πε0 r 2

e) Ninguna de las anteriores
Usando la ley de Gauss para el desplazamiento eléctrico, tenemos que:

~0

si 0 < r < 2R






Q
~
D(r)
ρ̂ si 2R < r < 3R

4πr 2






~0
si 3R < r

Por tanto, la magnitud de los campos es:

E1 = 0 ,

E2 =

Q
40πε0r 2

#### Problema 2.6.
Considere el sistema del Problema 2.5. La capacitancia del sistema es:
a) 480ε0 πR
b) 120ε0 πR
c) 140ε0 πR
d) 240ε0 πR
e) Ninguna de las anteriores
La diferencia de potencial entre R3 = 3R y R2 = 2R es


Q
Q
|∆V | =
−
40πε0 R3 R2
240πε0R
por lo que la capacidad es, simplemente,
C=

Q
= 240ε0 πR
|∆V |

---

### Página 57

#### Problema 2.7.
Considere el sistema del Problema 2.5. ¿Cuál es la carga inducida en la superficie del dieléctrico interno
ε1 ?
a) −

Q

b) 0 C
c) − Q
d) − Q
e) −

Q

~ = ~0 en esa región, E
~ = ~0 y por lo tanto P~ = ~0. Así, la carga inducida es:
Como D
Qind,ε1 = 0 C

#### Problema 2.8.
Considere el sistema del Problema 2.5. ¿Cuál es la carga inducida en la superficie externa del dieléctrico
ε2 ?
a)

Q

b) 0 C
c)

Q

d)

Q

e)

Q

El campo eléctrico en el dieléctrico es:
~ =
E
y la polarización es:

Q
ρ̂
4πε2r 2

~
P~ = (ε2 − ε0 )E

---

### Página 58

La densidad de carga superficial en r = R3 es:
(ε2 − ε0 )Q
σ = P~ (R3 ) · ρ̂ =
4πε2R3 2
y la carga total de polarización es:
Qind,ε2 = 4πR3 2 σ =

Q

#### Problema 2.9.
Se tiene un alambre de un material desconocido de 2 m de largo y con una sección transversal de 1 mm2 .
Los extremos del alambre se someten a una diferencia de potencial de 3 V y se mide una corriente
circulante de 2 A. Entonces, la conductividad σ del material es:
a)

× 10−6 Ω−1 m−1

b)

× 10−6 Ω−1 m−1

c)

× 106 Ω−1 m−1

d)

× 106 Ω−1 m−1

e)

× 106 Ω−1 m−1

Si llamamos L al largo, A al área, y σ a la conductividad, la resistencia de este alambre es:
R=

L
σA

I=

∆V
R

Por otra parte, de la ley de Ohm,

Juntando ambas ecuaciones, podemos despejar:
σ=

IL
= × 106 Ω−1 m−1
A∆V

donde se tuvo cuidado de usar solamente unidades en el SI.

---

### Página 59

#### Problema 2.10.
Se tienen dos placas planas conductoras con áreas A y distancia entre ellas igual a d, como en la figura.
En caso (A), las placas están cargadas con cargas ±Q; en el caso (B), las placas están conectadas con
una pila de voltaje U.

(A)

2d

(B)

+Q

2d

d

d

U

−Q

Si un agente externo duplica la distancia entre las placas de d a 2d, las energías almacenadas en los
condensadores:
a) Se duplica en ambos casos
b) Disminuye a la mitad en ambos casos
c) Se duplica en caso (A) y disminuye a la mitad en caso (B)
d) Disminuye a la mitad en caso (A) y se duplica en caso (B)
e) No cambia en ningún caso
En el caso (A), la carga es constante y la dependencia de la energía con la separación entre placas
es:
Q2
Q2 d
UA =
2C
2ε0 A
Para el caso (B), la diferencia de potencial es constante y vale U = cte, por lo que la dependencia
de la energía con d es:
CV 2
ε0 AU 2
UB =
2d
Por lo tanto, al duplicar la distancia en el caso (A) la energía se duplica y en el caso (B), disminuye
a la mitad.

#### Problema 2.11.
Entre dos placas planas conductoras con áreas A y distancia d se inserta un dieléctrico con permitividad
ε = εr ε0 como se indica en la figura.

---

### Página 60

A/2

A/2

εr
d
d/2
Si la capacidad del sistema sin dieléctrico es C0 , ¿cuál es la capacidad del sistema con el dieléctrico?

εr + 4
C0
a) C =
ε 
r
b) C =
C0
 
C0
c) C =
εr


εr
d) C =
C0
+
εr + 1 2


εr + 1 1
+
C0
e) C =
εr


La forma más simple de abordar el problema es considerar la configuración del enunciado como tres
condensadores, dos en serie en paralelo con el tercero:
εr
C1
C3
C2

Recordando que la capacitancia total sin dieléctrico es C0 =

εr ε0 A
εr ε0 (A/2)
(d/2)
d
ε0 (A/2)
ε0 A
(d/2)
d
ε0 A
ε0 (A/2)
d
2d

C1 =
C2
C3

ε0 A
, tenemos que:
d

---

### Página 61

ya que todos tienen área A/2, C1 y C2 poseen separación d/2 y C3 tiene separación d. La capacidad
equivalente de esta combinación es:
−1



εr
ε0 A
+
Cserie =
C1 C2
d
εr + 1


εr
C0
εr + 1
∴ C = C3 + Cserie


εr
C0
+
εr + 1 2

#### Problema 2.12.
Para la configuración del problema 2.11, suponiendo cargas iniciales ±Q en las placas y una energía
potencial inicial E0 , ¿cuál es el trabajo que un agente externo hace para insertar el dieléctrico?
εr
E0
εr − 1
E0
b) W = −
3εr + 1
εr
E0
c) W = −
εr + 1
a) W = −

d) W = −

εr + 1
E0
εr

e) W = −E0
Para un sistema aislado y con carga conservada, sabemos que la variación de energía del sistema
más el trabajo que hace el sistema tiene que ser cero, es decir:
dUsis + dWsis = 0
y el trabajo que hace el sistema es dWsist = −dWext , de modo que:
dWext = dUsis

Entonces, el trabajo total que hace el agente externo es:
Q2
Q2
Wext = Ufinal − Uinicial =
−
= E0
2Cf
2Ci



Usando el resultado del problema anterior para Cf , tenemos que:
εr − 1
E0
W =−
3εr + 1

Ci − Cf
Cf



---

### Página 62

#### Problema 2.13.
Dos placas planas conductores con áreas A = ab y con cargas ±Q están ubicadas como indica la figura.
La placa de abajo puede moverse horizontalmente.
b/2

b/2

d
b/2

b/2

a

¿Cuál es la magnitud de la fuerza horizontal que ejerce la place de arriba sobre la placa de abajo?
a) F =

2Q2
ε0 b2

b) F =

Q2
4πε0 d2

c) F =

Q2 b
ε0 da2

d) F =

2Q2 d
ε0 ab2

e) F = 0 N
Consideremos el siguiente sistema coordenado:

x

O

b

x+b

Como es un sistema aislado (no conectado a una batería) sabemos que Fsis = −∇U. La capacidad
es:
ε0 a(b − x)
C(x) =
d
y la energía es:
U(x) =

Q2
Q2 d
2C(x)
2ε0 a(b − x)

La fuerza que hace el sistema (la placa fija sobre la que se desplaza) es, entonces,
F~ = −∇U

x=b/2

=−

Q2 d
2Q2 d
−
ı̂
ı̂
2ε0 a(b − x)2 x=b/2
ε0 ab2

---

### Página 63

Es decir, la atrae con una fuerza de módulo:
F =

2Q2 d
ε0 ab2

#### Problema 2.14.
Sobre la capacidad eléctrica, es correcto afirmar que:
a) Depende de la geometría de los conductores
b) Depende del voltaje aplicado
c) Depende de las cargas en las placas
d) Es diferente de cero solamente con dieléctrico
e) Depende de donde se conectan eléctricamente los dos conductores
#### Problema 2.15.
Un Farad equivale a:
a) 1 F = 1 V A
b) 1 F = 1 A V−1
c) 1 F = 1 J A−1
d) 1 F = 1 W C−1
e) 1 F = 1 C V−1
#### Problema 2.16.
Una pieza de cobre (con simetría cilíndrica) tiene la forma de que se muestra en la figura. Los extremos
están conectados a una batería de modo que en la pieza fluye corriente. ¿En qué región A, B o C es
mayor la densidad de corriente?

A

B

C

a) Región A
b) Región B

---

### Página 64

c) Región C
d) Es igual en todas las regiones
e) Depende de la diferencia de potencial que se aplique
Si circula una corriente constante, a menor superficie se obtiene una mayor densidad de corriente.

#### Problema 2.17.
En el Problema 2.16, ¿en qué región es mayor el campo eléctrico?
a) Región A
b) Región B
c) Región C
d) Es igual en todas las regiones
e) Depende de la diferencia de potencial que se aplique
A conductividad constante, mayor densidad de corriente implica mayor campo, de acuerdo a la ley
de Ohm microscópica.

#### Problema 2.18.
En el Problema 2.16, la razón entre los diámetros es A : B : C = 3 : 1 : 5. Entonces, la velocidad de
deriva de los electrones:
a) Tiene la misma magnitud en la región B que en la región C
b) Es cinco veces mayor en la región B que en la región C
c) Es veinticinco veces mayor en la región B que en la región C
d) Es cinco veces menor en la región B que en la región C
e) No tenemos suficientes datos para decidir
La densidad de corriente en este caso es J = I/A, en donde A es el área de cada segmento conductor.
Por otra parte, por tratarse del mismo material, la densidad de portadores de corriente ρ es constante.
Por tanto, la velocidad de deriva es vd = J/ρ ≈ 1/A. El área es proporcional al diámetro al cuadrado,
por lo que para las razones entre diámetros dadas se encuentra el resultado indicado.

---

### Página 65

#### Problema 2.19.
Considere un conductor cuya forma geométrica es semejante a la del Problema 2.16 pero hecho de
materiales de distinta conductividad. La conductividades σ de los tramos A, B y C están en la razón
σA : σB : σC = 2 : 1 : 5, y la razón entre los diámetros es A : B : C = 2 : 1 : 3. Entonces, una vez
establecido el régimen estacionario (∇ · J~ = 0), podemos afirmar que la densidad de corriente es menor
en:
a) Región A
b) Región B
c) Región C
d) Es igual en todas las regiones
e) Depende de la diferencia de potencial que se aplique
Es menor en la región C independientemente de las conductividades, puesto que una vez establecido
el régimen estacionario la corriente es constante.

#### Problema 2.20.
El espacio entre dos placas conductoras de áreas A, separadas una distancia d, está lleno en partes
iguales con materiales de distintas conductividades: σ1 = 2σ0 y σ2 = σ0 (ver figura). Las placas están
conectadas a una batería que provee una diferencia de potencial constante V0 . Entonces, la carga que
pasa por un área A/4 en la región con σ1 , en un intervalo de 8 segundos, es:

a) Q =

8σ0 V0 A
C
d

b) Q =

2σ0 V0 A
C
d

c) Q =

4σ0 V0 A
C
d

d) Q =

σ0 V0 A
C
d

e) Q =

σ0 V0 A
C
2d

---

### Página 66

Como la diferencia de potencial V0 es constante, el campo eléctrico es E = V0 /d. En l región de
conductividad σ1 , la densidad de corriente es:
J1 = σ1 E =

σ1 V0
d

Por el área A/4 pasa una corriente I = J1 · (A/4), y la carga total que atraviesa dicha área en un
intervalo ∆t es Q = I∆t. Reemplazando los valores dados de σ1 y ∆t = 8 s resulta:
Q=

4σ0 V0 A
C
d

#### Problema 2.21.
Un cilindro de radio a y largo L tiene una conductividad variable σ(z) = σ0 (z − 2L)2 , donde el eje Z
está dirigido a lo largo del eje de simetría del cilindro. Entonces, si suponemos que la corriente circula
en la dirección k̂, la resistencia del cilindro es:
a) R =

πa2 Lσ0

b) R =

L
2πa2 σ0

c) R =

2πa2 Lσ0

d) R =

2L
πa2 σ0

e) R =

πa2 Lσ0

Como el cilindro tiene área uniforme y la corriente circula perpendicular a las secciones transversales
(eje Z), entonces podemos tomar un elemento infinitesimal de volumen y calcular su resistencia:
dR =

dz
σ(z) A

Considerando que cada uno de ellos está en serie, la resistencia total corresponde a la suma de cada

---

### Página 67

una de las contribuciones individuales:
R =

ˆ L

dR
ˆ L

dz
σ0 A 0 (z − 2L)2
2Lσ0 A
2πa2 Lσ0

#### Problema 2.22.
Se carga un condensador de 4 µF con una fuente de 200 V. Después de cargarlo completamente, se
desconecta el condensador y se conecta en paralelo a otro condensador, de 2 µF inicialmente descargado.
¿Cuanta energía electrostática se libera al ambiente en el proceso?
a) 8.00 × 10−2 J
b) 5.33 × 10−2 J
c) 2.67 × 10−2 J
d) 1.00 × 10−4 J
e) 6.25 × 10−4 J
Como inicialmente el sistema se encuentra conectado a una batería, la energía potencial electrostática
inicial viene dada por:
Ui =

4 × 10−6 · 4 × 104
Ci V 2
J = 8 × 10−2 J

Al cargarse completamente, el primer condensador almacena una carga igual al:
Q = 4 µF · 200 V = 8 × 10−4 C
Posteriormente, el sistema se modifica hasta tener dos condensadores en paralelo, con una capacitancia equivalente Cf = 4 µF+ 2 µF = 6 µF. En este caso, la carga se ha repartido, pero la magnitud
total Q permanece intacta pues el sistema está aislado. Por tanto, la energía final del sistema es:
Uf =

Q2
64 × 10−8
J=
× 10−2 J
−6
2Cf
2 · 6 × 10

---

### Página 68

Así, la variación de energía es simplemente la resta:
∆U = Uf − Ui = − × 10−2 J = −2.67 × 10−2 J
donde el signo menos indica que dicha energía fue liberada al ambiente.

#### Problema 2.23.
La placa P1 de un condensador de placas planas y paralelas, lleno de aire y de área A, está conectada
a un resorte que tiene constante elástica k, mientras que la segunda placa P2 está fija. El aparato está
sobre una mesa sin fricción, como se muestra en la figura. Si una carga +q se coloca en la placa P1 y
una carga −q en la placa P2 , ¿cuánto es la máxima expansión del resorte?

k

P1

P2

x
a)

q2
2ε0 Ak

q2
b)
4ε0 Ak
c)

q2k
4ε0 A

d)

q2k
2ε0 A

e) Ninguna de las anteriores
Sea x la distancia que se mueve la placa P1 , respecto de su posición inicial. Esta cantidad coincide con
lo que se alarga el resorte, medido positivamente desde el la placa P1 hacia la placa P2 . Si el resorte
se alarga x unidades de largo, el condensador se acerca x unidades respecto de lo separación original,
d. Sobre la placa P1 actúan dos fuerzas: la fuerza elástica F~elast = −kx ı̂ y la fuerza electrostática
F~elect . Esta última, dado que el sistema se encuentra aislado, la calculamos como F~elect = −∇U:
ε0 A
C(x) =
d−x
q 2 (d − x)
q2
U(x) =
2C(x)
2ε0 A
q2
ı̂
F~elect = −∇U(x) =
2ε0 A

---

### Página 69

Aplicando la segunda ley de Newton, siendo m la masa de la placa, en el eje X:
mẍ =

q2
− kx ,
2ε0 A

x(0) = x′ (0) = 0

La ecuación diferencial anterior tiene por solución:
"
!#
r
q2
k
x(t) =
1 − cos
t
2ε0 Ak
m
Por tanto, el máximo desplazamiento corresponde a:
xmax =

q2
2ε0Ak

#### Problema 2.24.
Se tienen tres cilindros C1 , C2 y C3 óhmicos con resistividades ρj , largos Lj y áreas transversales Aj ,
con j = 1, 2, 3 respectivamente. Suponga que ρ1 = ρ3 = ρ y ρ2 = 2ρ, L1 = L3 = L y L2 = L/2 y las
áreas son A1 = A3 = A y A2 = A/2. Entonces, la resistencia del sistema entre las tapas a y b es:

a

a)

2ρL
A

b)

4ρL
A

c)

ρL
2A

d)

ρL
4A

C1

C2

C3

ρ1

ρ2

ρ3

b

e) Ninguna de las anteriores
Entre a y b, los tres cilindros están en serie, por lo que la resistencia total es:
R=

ρ1 L1 ρ2 L2 ρ3 L3
+
+
A1
A2
A3

---

### Página 70

Reemplazando,
R=

4ρL
ρL 2ρ(L/2) ρL
+
+
A
A/2
A
A

#### Problema 2.25.
Se tienen dos esferas conductoras, Sa y Sb , concéntricas de radios a y b con a < b. Entre las esferas hay
un material óhmico que tiene una resistividad ρ = ρ(r), dependiente de la distancia al centro de ambas
esferas, que se puede controlar a voluntad. Asuma que fluye una corriente estacionaria I, radial, desde
a hasta b. ¿Con cuál de las siguientes resistividades resulta un campo eléctrico E independiente de r?
r2
a) ρ(r) = ρ0 2
a
r
b) ρ(r) = ρ0
a
r
c) ρ(r) = ρ0
b


d) ρ(r) = ρ0 ln(a/r) − ln(b/r)
e) Ninguna de las anteriores
Tomemos un cascarón esférico de espesor dr, el cual posee una resistencia igual a:
dR =

ρ(r) dr
ρ(r) dr
A
4πr 2

De la ley de Ohm, se sabe que dV = I dR. Por otra parte, se sabe que dV = E dr. Igualando,
I dR = E dr

−→

dR =

E
dr
I

Así, se debe cumplir que:
ρ(r)
E
4πr
I
Por tanto, como la corriente I es estacionaria y se quiere que E sea independiente de r, la resistividad
debe ser proporcional a r 2 .

#### Problema 2.26.
Se tiene un cilindro MUY largo de material dieléctrico con permitividad relativa ǫr = 10. En el eje del
cilindro se encuentra un cable con una densidad de carga lineal de carga λ constante. Suponga que r
es la distancia al eje del cilindro. Entonces, el módulo del campo eléctrico, E(r), dentro del material
dieléctrico es:

---

### Página 71

a) E(r) =

λ
2πε0 r

b) E(r) =

λ
10πε0 r

c) E(r) =

λ
20πε0 r

d) E(r) =

λ
πε0 r

e) Ninguna de las anteriores
~ =
Por la simetría del problema, proponemos que el desplazamiento eléctrico posee la forma D
D(r) er. Por lo tanto, de la ley de Gauss para el desplazamiento eléctrico aplicada a un cilindro de
altura h y radio r,
¨
¨
λ
~
D · n̂ dS =
D(r) dS = 2πrh D(r) = qlibre = λ h −→ D(r) =
2πr
Así, en el dieléctrico,
E(r) =

λ
D(r)
εr ε0
20πε0 r

#### Problema 2.27.
Un alambre uniforme de largo ℓ y sección transversal A tiene una resistencia de 16 Ω. Se corta el alambre
en cuatro pedazos iguales de sección transversal A. Luego, cada uno de los cuatro alambres se estira,
manteniendo su densidad volumétrica, hasta alcanzar un largo ℓ cada uno. Si los cuatro alambres se
conectan en paralelo, ¿cuál es la resistencia equivalente de esta combinación?
a) 64 Ω
b) 4 Ω
c) 16 Ω
d) 1 Ω
e) Ninguna de las anteriores
Sea R la resistencia original y R′ la resistencia de cada uno de los cuatro segmentos. Si la resistividad
del material es ρ, entonces:
ρℓ
R′ = ′
A

---

### Página 72

Notar que utilizamos el mismo largo inicial, pero debemos determinar la nueva sección transversal
puesto que el material se estiró. Si m es la masa inicial del alambre, y la densidad se mantiene,
entonces:
m′
m/4
A
m
= ′ ′ = ′
−→ A′ =
Aℓ
Aℓ
Aℓ
Es decir, el área se reduce a la cuarta parte de la original. Por lo tanto, la resistencia de cada uno
de los segmentos es:
ρℓ
ρℓ
R′ =
=4
= 4R
A/4
A
Finalmente, la resistencia equivalente viene dada por:
−1

R′
+
+
+
= R = 16 Ω
Requiv =
R′ R′ R′ R′

#### Problema 2.28.
Un condensador de dos placas planas y paralelas se carga a una diferencia de potencial de 20 V. Una vez
cargado, se desconecta de la fuente de voltaje y se dobla la distancia entre las dos placas. Es correcto
afirmar que la diferencia de potencial o la carga cambian en la siguiente manera:
a) La carga y el voltaje se mantienen
b) El voltaje aumenta a 40 V
c) El voltaje disminuye a 5 V
d) La carga se duplica
e) La carga se reduce a la mitad
Una vez que el condensador está cargado, su carga inicial es:
Qi = Ci Vi
Al separarse las placas, la nueva capacidad del sistema es:
Cf =

Ci
ε0 A
2d

Como el sistema (luego de retirar la fuente de voltaje) está aislado, la carga se conserva y Qi = Qf .
Con ello, la nueva diferencia de potencial es:
Vf =

Qf
Qi
Ci Vi
= 2 Vi = 40 V
=2
Cf
Ci /2
Ci

---

### Página 73

#### Problema 2.29.
Considere dos cascarones esféricos metálicos concéntricos de radios a y b, ambos con un espesor despreciable. El espacio entre los dos cascarones (a < r < b) se llena con agua de mar de conductividad
σ = 4.8 Ω−1 m−1 y permitividad dieléctrica ε = 8.5 × 10−10 A s V−1 m−1 . Con una fuente de poder se
mantiene una carga constante Q = 109 C en el cascaron interno y −Q en el cascaron externo. Entonces,
la corriente eléctrica que circula entre los cascarones es:
a) I = 11.2 A
b) I = 4.8 A
c) I = 56 A
d) I = 0.48 A
e) I = 5.6 A
Al aplicar la ley de Gauss para el vector desplazamiento, tenemos que:
4πr 2 D(r) = Q

−→

D(r) =

Q
4πr 2

−→

E(r) =

Q
4πεr 2

Por la ley de Ohm microscópica, la densidad de corriente es:
J = σE =

σQ
4πεr 2

La corriente que circula cada sección esférica (cascarón esférico de radio r) es, entonces,
I = 4πr 2 J =

4.8
σQ
× 10 A = 5.6 A
ε
8.5

#### Problema 2.30.
√
Considere dos placas paralelas de área A y separadas por una distancia d ≪ A. El espacio entre las
placas está lleno con un material de conductividad σ. Calcule la resistencia del sistema, ignorando los
efectos de borde.
a) R =

2d
σA

b) R =

d
σA

c) R =

d
4σA

d) R =

d
2σA

---

### Página 74

e) R =

d
6σA

Supongamos que sometemos las dos placas a una diferencia de potencial V . Dado que la separación
entre las placas es mucho más pequeña que las dimensiones de las mismas, podemos aproximar la
situación a dos planos infinitos. Así, el campo eléctrico tendrá una magnitud E = V /d. De la ley de
Ohm microscópica, J = σE = σV /d. Como la densidad de corriente es constante, I = JA = σV A/d.
De la ley de Ohm macroscópica,
V
V
d
R=
I
σV A/d
σA

#### Problema 2.31.
Considere una esfera conductora perfecta de radio R = 0.2 m, inicialmente con carga Q0 = 10 C y
completamente rodeada por un medio uniforme de conductividad σ = 2 × 10−11 Ω−1 m−1 y constante
dieléctrica κ = ε/ε0 = 50 (el valor de la permitividad del vacío es ε0 ≃ 9 × 10−12 C2 N−1 m−2 ). Para que
la carga inicial se reduzca por un factor de e−1 ≃ 0.37, es necesario esperar un tiempo de:
a) 222.5 s
b) 0.1 s
c) 22.5 s
d) 112.4 s
e) 11.2 s
Sea Q = Q(t) la carga sobre la superficie de la esfera conductora. El campo eléctrico a una distancia
r mayor que el radio de la esfera es:
Q
~ =
E
ρ̂
4πκε0r 2
Por la ley de Ohm, la densidad de corriente está dada por:
~ =
J~ = σ E

σQ
ρ̂
4πκε0 r 2

Así, la corriente que circula desde la esfera a través de una superficie esférica de radio r es:
¨
Q
σQ
(∗)
I=
J~ · n̂ dS =
κε0
τ
S

con τ = κε0 /σ. Dado que se trata de un proceso de descarga, I = −dQ/dt, por lo que la ecuación
(∗) corresponde a una ecuación diferencial con solución:
Q(t) = Q0 exp(−t/τ )

---

### Página 75

Sea t∗ el tiempo pedido en el enunciado, i.e. Q(t∗ ) = Q0 e−1 . Con ello,
t∗ = τ =

50 · 9 × 10−12
κε0
s = 22.5 s
σ
2 × 10−11

#### Problema 2.32.
Una esfera de radio R = 0.2 m con carga libre Qlib = −20 C está sumergida en un medio dieléctrico lineal
homogéneo de constante dieléctrica κ = 3.5 y de extensión infinita. El valor absoluto de la densidad
superficial de carga de polarización en la esfera se aproxima mejor a:
a) 95 Cm−2
b) 142 Cm−2
c) 178 Cm−2
d) 0 Cm−2
e) 28 Cm−2
El campo eléctrico fuera de la esfera es el de una carga puntual en el origen en presencia de un
dieléctrico:
~ = Qlib ρ̂
E
4πκε0r 2
El vector polarización viene dado por:
~ = (κ − 1)Qlib ρ̂
P~ = (ε − ε0 )E
4πκr 2
Finalmente,
σpol = P~ · n̂

r=R

=−

2.5 · 20
(κ − 1)Qlib
≈
C m−2 ≈ 28 C m−2
4πκR
4 · 3.14 · 3.5 · 0.04

#### Problema 2.33.
Se tiene una esfera maciza sin carga libre de radio R hecha de un material dieléctrico no lineal. La esfera
~ = − kr ρ̂. La carga total de polarización en la
está polarizada, y el campo eléctrico en su interior es E
ε0
superficie de la esfera es:
a) Qp = −

kR2

---

### Página 76

b) Qp =

kR2

c) Qp = −4πR3 k
d) Qp = 4πR3 k
e) Qp = 0
~ = ~0. Por tanto, el vector polarización dentro de la esfera viene dado
Como la carga libre es cero, D
por:
~ − ε0 E
~ = kr ρ̂
P~ = D
Por tanto, la densidad superficial de carga de polarización es:
σp = P~ · n̂

= kR
r=R

pues la normal apunta hacia afuera. Finalmente,
Qp = 4πR2 σp = 4πR3 k

#### Problema 2.34.
Se tiene un cascarón esférico metálico de radio R con carga positiva Q, rodeado por un material dielétrico
con permitividad relativa κ hasta r = 3R/2. Todo lo anterior se rodea con otro cascarón esférico metálico
de radio r = 2R y carga −Q, quedando el espacio 3R/2 < r < 2R vacío. La capacitancia entre los dos
conductores de este sistema es:
a) C = 4πε0 R(κ + 1)
b) C = πε0 R(κ + 1)
c) C = 2πε0 R(κ + 1)


6κ
d) C = 4πε0 R
2+κ


6+κ
e) C = 4πε0 R
3κ
Recordemos que la capacitancia de un condensador formado por dos esferas metálicas de radios
0 < a < b es:
4πε0ab
Cesf =
b−a

---

### Página 77

Se puede considerar que el sistema se trata de un conjunto de condensadores Ci en serie, donde:
C1 corresponde al condensador que se extiende entre R < r < 3R/2 y un dieléctrico con
permitividad relativa κ:
4πκε0 (3R2 /2)
= 12πκε0 R
C1 =
R/2
C2 corresponde al condensador que se extiende entre 3R/2 < r < 2R sin dieléctrico en su
interior:
4πε0 (3R2 )
= 24πε0 R
C2 =
R/2
Por tanto,
C
24πε0R



+1
κ



24πε0R



2+κ
κ



−→

C = 24πε0 R



κ
2+κ



#### Problema 2.35.
Se tiene un capacitor de placas paralelas con separación entre las placas muy pequeña comparada a
sus dimensiones. Este capacitor se carga con una batería hasta que su carga y voltaje iniciales son Q0
y V0 , respectivamente. Luego, se desconecta el capacitor de la batería, mientras que la distancia entre
las placas se incrementa un factor de 4. Al mismo tiempo, se introduce un dieléctrico con permitividad
relativa κ = 3 en todo el espacio entre las placas. Los nuevos valores de la carga y el voltaje en el
capacitor son:
a) Q0 ,

V0

b) 3Q0 ,

V0

c)

Q0 , 3V0

d)

Q0 , V0

e) Q0 ,

V0

Notemos que, luego de retirar la batería, el proceso se realiza a carga constante, pues las placas
no pueden intercambiar carga entre ellas ni con el medio externo. Así, Qf = Q0 . Por otra parte,
siguiendo la misma nomenclatura para la capacitancia, se sabe que:
C0 =

ε0 A
d

−→

Cf =

κε0 A
= C0
4d

---

### Página 78

Así,
Vf =

Q0
Qf
= V0
Cf
3C0 /4

#### Problema 2.36.
Un capacitor de placas cuadradas planas y paralelas tiene lado L y separación entre las placas d. El
espacio entre las placas está inicialmente vacío. El capacitor esta conectado a una fuente de voltaje
ideal con voltaje V0 y un amperímetro que puede medir corriente, como indica la figura. Al introducir
un dieléctrico de permitividad relativa κ en el capacitor, se puede generar una corriente. ¿Con qué
velocidad v hay que introducir el dieléctrico para que la corriente generada tenga magnitud I?

A

κ

d

v
x

V0
a) v =

Id
V0 L(κ − 1)ε0

Id2
b) v =
V0 L2 (κ − 1)ε0
c) v =

Id
2V0 L(κ − 1)ε0

d) v =

2Id
V0 L(κ − 1)ε0

e) v =

2Id2
V0 L2 (κ − 1)ε0

Sea x la distancia, medida desde el borde de la placa, de dieléctrico que se ha introducido en el
condensador. Así, la capacitancia equivalente vendrá dada por:
C(x) =


κε0 Lx ε0 L(L − x)
ε0 L 
(κ − 1)x + L
+
d
d
d

---

### Página 79

Por tanto,

V0 ε 0 L 
(κ
−
1)x
+
L
Q(x) = C(x)V0 =
d
Finalmente,
v=

−→

I=

dQ
V0 ε0 L(κ − 1) dx
dt
d
dt

Id
dx
dt
V0 Lε0 (κ − 1)

#### Problema 2.37.
Tres cascarones conductores cilíndricos concéntricos de largo L, con cargas (−Q, +Q, 0) y radios (R, 2R, 3R)
forman tres espacios separados, identificados con las letras (a, b, c). En cada espacio se puede poner un
dieléctrico lineal y homogéneo con constantes dieléctricas relativas (permitividades relativas) (κa , κb , κc ).
¿Cuál de las siguientes configuraciones tiene la mayor cantidad de energía almacenada?
a) κa = 1, κb = 1, κc = 4
b) κa = 1, κb = 4, κc = 1
c) κa = 2, κb = 2, κc = 1
d) κa = 1, κb = 2, κc = 2
e) κa = 3, κb = 3, κc = 3
Recordemos que la energía almacenada en cierta configuración viene dada por:
˚
κε0
~ 2 dV
U=
kEk
R

Aplicando ley de Gauss, notaremos que el vector desplazamiento es no nulo únicamente en el espacio
b, con magnitud Db ∝ Q. De esta forma, dado que Db = κb ε0 Eb , entonces Eb ∝ Q/κb y U ∝ Q2 /κb .
Así, la energía será máxima en aquella configuración en que κb sea mínima, que corresponde al caso
κb = 1.

#### Problema 2.38.
El Cobre tiene una conductividad σ ≈ 6 × 107 Ω−1 m−1 a temperatura ambiente. En los metales, los
portadores de carga son los electrones (e ≈ 1.6×10−19 C, me ≈ 9×10−31 kg) que se mueven a temperatura
ambiente con una velocidad de deriva v ≈ 106 m/s. El Cobre tiene una densidad de electrones libres
n = 9 × 1028 m−3 . ¿Cuál es el tiempo promedio τ entre dos colisiones consecutivas de electrones en el
Cobre?
a) τ ≈ 24 ps

---

### Página 80

b) τ ≈ 18 ns
c) τ ≈ 24 fs
d) τ ≈ 1.8 ps
e) τ ≈ 0.24 ps
El modelo de Drude para la conductividad en los metales nos permite relacionar la conductividad
con el tiempo medio entre colisiones:
σ =
τ =
≈
≈
≈

nq 2 τ
me
σme
nq 2
(6 × 107 )(9 × 10−31 )
s
(9 × 1028 )(2.56 × 10−38 )
× 10−14 s
2.56
2.4 × 10−14 s = 24 fs

#### Problema 2.39.
Dos conductores con conductividades σ1 y σ2 = 2σ1 están conectados. A través de ellos circula una
corriente I producto de una diferencia de potencial V0 , como muestra la figura. ¿Qué voltaje V1 marca
el voltímetro V ?
L/2

L/2

σ1

I

σ2

V

V0

a) V1 = V0
b) V1 = V0
c) V1 = V0

---

### Página 81

d) V1 = V0
e) V1 = V0
Supongamos que los conductores poseen una sección transversal constante A. Entonces, la resistencia
de cada uno de ellos es:
A
A
R1
R1 =
∧
R2 =
σ1 L/2
σ2 L/2
Con ello, la resistencia equivalente es R = R1 + R2 = 3R1 /2. Dicha corriente se relaciona, a través
de la ley de Ohm, con la corriente de la siguiente forma:
R=

V0
I

−→

R1 =

2V0
3I

Así, la diferencia de potencial entre los extremos del conductor 1 es:
V1 = R1 I = V0

---

### Página 82

Circuitos eléctricos

Ecuaciones de Maxwell en uno de los muros exteriores de la Universidad de Varsovia

---

### Página 83

#### Problema 3.1.
Se tienen dos condensadores C1 y C2 con cargas iniciales Q1 (0) = 0 y Q2 (0) = Q0 respectivamente.
El condensador C2 está inicialmente conectado a una resistencia R. En el instante t = 0 se conecta el
condensador C1 al arreglo formado por la resistencia y el segundo condensador, como se aprecia en la
figura. La intensidad de la corriente eléctrica para la situación t > 0 es proporcional a:

C1

R
+

C2

-

 
 
1/C1 + 1/C2
t
a) exp −
2R
 
 
1/C1 + 1/C2
b) exp −
t
R
 
 
1/C1 − 1/C2
c) exp −
t
R


t
d) exp −
RC1


t
e) exp −
R(C1 + C2 )
Sabemos que la corriente durante el proceso de descarga es:
I(t) = I0 exp(−t/τ )
con τ la constante de tiempo del circuito, que corresponde a τ = Req Ceq . En este caso,
Req = R

∧

Ceq = (1/C1 + 1/C2 )−1

puesto que los condensadores están en serie. Así,
R
τ=
1/C1 + 1/C2

−→

 
 
1/C1 + 1/C2
t
I(t) = I0 exp −
R

---

### Página 84

#### Problema 3.2.
En el siguiente circuito, el interruptor ha estado cerrado por un largo tiempo. En t = 0, este se abre.
¿Cuál debiese ser el valor de la resistencia R, en términos de C y T para que en t = T la caída de
voltaje en la resistencia sea V /2?

R

+
−
V
C
a) R =

T
2C

b) R =

2T
C

c) R =

T
C ln(2)

d) R =

T ln(2)
2C

e) No se puede determinar
En t < 0 el condensador se encuentra inicialmente descargado, puesto que no hay diferencia de
voltaje entre sus extremos ya que están unidos por un conductor ideal. Una vez abierto el interruptor,
nos encontramos con un típico circuito RC en carga, donde la corriente está dada por:
I(t) =

V −t/RC
e
R

VR (t) = I(t)R = V e−t/RC

−→

R=

T
C ln(2)

Por la ley de Ohm,

Despejando,

#### Problema 3.3.
Considere el circuito de la figura. La corriente I1 está dada por:

V
= V e−T /RC

---

### Página 85

18 Ω
6Ω
9V

I2

+
−

3Ω
+
−

I1

I3

3V

a) I1 = 0.2 A
b) I1 = 0.3 A
c) I1 = 0.5 A
d) I1 = 0.6 A
e) I1 = 0.4 A
Sean i1 e i2 las corrientes que circulan por las mallas, según muestra la siguiente figura:
18 Ω
6Ω
9V

+
−

3Ω

i1
i2

+
−
3V

Aplicando el método de mallas,
−9 + 18i1 + 6(i1 − i2 ) + 3 = 0

∧

6(i2 − i1 ) + 3i2 − 3 = 0

Resolviendo,
i1 = 0.4 A

∧

i2 = 0.6 A

Notemos que I1 corresponde a la misma corriente i1 . Así,
I1 = 0.4 A

#### Problema 3.4.
Considere el sistema del Problema 3.3. La corriente I2 está dada por:
a) I2 = 0.2 A

---

### Página 86

b) I2 = 0.3 A
c) I2 = 0.5 A
d) I2 = 0.6 A
e) I2 = 0.4 A
Notemos que la corriente I2 se relaciona con nuestras corrientes i1 e i2 mediante la relación:
I2 = i2 − i1 = 0.2 A

#### Problema 3.5.
Determine el valor de la corriente I del circuito de la figura:
30 V
+
−

I
6Ω

30 Ω

60 Ω

22 Ω

30 Ω

45 Ω

a) I = 4 A
b) I = −3 A
c) I = 2 A
d) I = 1 A
e) I = 0.5 A
Notemos que las resistencias verticales están en paralelo, puesto que se encuentran a la misma
diferencia de potencial. Así, si llamamos R1 a la resistencia equivalente, tendremos que:

−1
R1 =
+
= 18 Ω
30 Ω 45 Ω
Por otra parte, R1 está en serie con la resistencia de 22 Ω. Si R2 es la resistencia equivalente, entonces:
R2 = R1 + 22 Ω = 40 Ω

---

### Página 87

A su vez, R2 está en paralelo con la resistencia de 60 Ω. Si R3 es la resistencia equivalente,
−1

+
= 24 Ω
R3 =
60 Ω R2
Ahora bien, R3 está en serie con la resistencia de 6 Ω. Llamando R4 a la resistencia equivalente,
R4 = 6 Ω + R3 = 30 Ω
Finalmente, R4 está en paralelo con la resistencia de 30 Ω. Llamando Req a la resistencia equivalente,
que corresponde a la resistencia equivalente de todo el circuito,

−1
Req =
+
= 15 Ω
30 Ω R4
Por tanto, por la ley de Ohm,
I=

V
= 2A
Req

#### Problema 3.6.
En el circuito de la figura, I1 = 4 A. Entonces:

28V
5Ω
I1
ε

x

6Ω
I2

3Ω
a) La corriente que circula por la resistencia de 5 Ω es de 2 A hacia la derecha
b) La corriente I2 es 5 A
c) ε vale 42 V
d) Si el circuito se interrumpe (abre) en el punto x, la corriente que circula por la resistencia de 5 Ω es
6 A hacia la derecha
e) Ninguna de las anteriores

---

### Página 88

Sean i1 e i2 las corrientes que circulan por las malla superior e inferior, en el sentido anti-horario,
respectivamente. La relación con I1 e I2 viene dada por:
I1 = i2 − i1

∧

I2 = i2

Aplicando las reglas de Kirchhoff, se cumple que:
3i2 + 6(i2 − i1 ) − ε = 0
5i1 − 28 + ε + 6(i1 − i2 ) = 0
i2 − i1 = 4
Resolviendo,
i1 = 2 A

∧

i2 = 6 A

∧

ε = 42 V

#### Problema 3.7.
Tres ampolletas iguales de 36 W y 12 V, se encuentran conectadas a dos baterías de 12 V según muestra
la figura. La potencia total disipada por las TRES ampolletas es:
A1

A2

12V
A3
12V

a) 36 W
b) 54 W
c) 108 W
d) 12 W
e) 24 W
Como las ampolletas son de 36 W y 12 V, significa que poseen una resistencia interna igual a:
V2
P =
R

−→

V2
R=
Ω = 4Ω
P

---

### Página 89

Sean i1 e i2 las corrientes que circulan por la malla con una y dos ampolletas, respectivamente, en
sentido anti-horario. Así, aplicando las leyes circuitales:
12 + 4(i1 − i2 ) = 0
4i2 + 4(i2 − i1 ) + 4i2 − 12 = 0
Resolviendo,
i1 = −3 A

∧

i2 = 0 A

Como la corriente i2 es igual a cero, significa que no circula corriente por esa rama, i.e. dichas
ampolletas no están encendidas. Como hay una única ampolleta encendida, la potencia disipada es:
Ptotal = I 2 R = (−3)2 · 4 W = 36 W

#### Problema 3.8.
En el circuito de la figura, la corriente I que circula por la rama del medio está dada por:

V

R

R

V
R
R

R

V

V
2R
V
b) I =
4R
3V
c) I =
2R
2V
d) I =
3R
V
e) I =
R
a) I =

Podemos encontrar el circuito equivalente notando que:
Las resistencias en paralelo, en serie con una tercera resistencia, equivalen a Req =

3R

---

### Página 90

Dos fuentes de voltaje en serie generan un voltaje igual a la suma de ellos, Veq = 2V
Con ello,

2V

R

3R/2
I

R

V

Sea i1 e i2 las corrientes que circulan por las mallas superior e inferior, en sentido anti-horario,
respectivamente. Así,
3R
(i1 − i2 ) = 0

R i1 − 2V +

3R
(i2 − i1 ) + R i2 − V

Resolviendo,
i1 =

13V
8R

∧

i2 =

= 0

11V
8R

Como I = i1 − i2 , finalmente:
I = i1 − i2 =

13V
11V
V
−
8R
8R
4R

#### Problema 3.9.
Considere el circuito de la figura,
18Ω
9V

6Ω

I3

I2
I1

3V

La corriente I1 está dada por:
a) I1 = 0.2 A

3Ω

---

### Página 91

b) I1 = 0.6 A
c) I1 = 0.4 A
d) I1 = 0.3 A
e) I1 = 0.5 A
Sean i1 e i2 las corrientes que circulan, en sentido anti-horario, por las mallas izquierda y derecha
respectivamente. Aplicando la ley de mallas,
6(i1 − i2 ) + 18i1 + 9 − 3 = 0
3i2 + 6(i2 − i1 ) + 3 = 0
Resolviendo,
i1 = −0.4 A
Como I1 = −i1 , entonces:

∧

i2 = −0.6 A

I1 = 0.4 A

#### Problema 3.10.
Para el circuito del Problema 3.9, el valor de I2 es:
a) I2 = 0.2 A
b) I2 = 0.6 A
c) I2 = 0.4 A
d) I2 = 0.3 A
e) I2 = 0.5 A
Como I2 = i1 − i2 , entonces:

I2 = 0.2 A

#### Problema 3.11.
En el circuito de la figura, los dos condensadores se cargan inicialmente con 45 V. Después de cerrar el
interruptor S, el tiempo que tarda en reducirse el potencial en ambos condensadores a 10 V es:

---

### Página 92

S
50Ω
20uF

15uF

30Ω
a) 5.3 ms
b) 4.2 ms
c) 7.1 ms
d) 2.3 ms
e) Ninguna de las anteriores
La capacitancia equivalente entre los condensadores en paralelo es:
Ceq = 15 µF + 20 µF = 35 µF
Por otra parte, la resistencia equivalente entre las resistencias en serie es:
Req = 30 Ω + 50 Ω = 80 Ω
Consideremos la siguiente situación:

I

Ceq +
-

Req

Aplicando ley de mallas,
IReq − VC = 0
Q
Ceq

= 0

˙ eq − Q̇
IR
Ceq

= 0

IReq −

,

d
dt

---

### Página 93

Como el condensador se está descargando, −Q̇ = I, por lo que la ecuación diferencial que debemos
resolver es:
I
I˙ +
=0
Req Ceq
cuya solución es:
I(t) = I0 e−t/τ ,

τ = Req Ceq = 2.8 ms

El voltaje en la resistencia equivalente es, por tanto,
VR (t) = Req I(t) = Req I0 e−t/τ = V0 e−t/τ
con V0 = Req I0 = 45 V, pues el voltaje inicial del condensador corresponde al voltaje en ambas
resistencias. Cuando el voltaje en los condensadores sea de 10 V, el mismo valor se tendrá en la
resistencia equivalente, por lo que:
 
−t/τ
= 4.2 ms
10 = 45 e
−→ t = τ ln

#### Problema 3.12.
Se tienen dos condensadores C1 y C2 con cargas iniciales Q1 (0) = Q y Q2 (0) = 0. Los condensadores
están conectados a una resistencia R como indica la figura. En el instante t = 0 se cierra el circuito.
Suponga que C1 = C2 = C. La carga de C2 , Q2 (t), satisface la ecuación diferencial:

Q1(t)

Q2(t)

C1

C2
R

a)

Q − Q2
dQ2
dt
RC

b)

dQ2
Q + 2Q2
dt
RC

c)

dQ2
Q + Q2
dt
RC

d)

Q − 2Q2
dQ2
dt
RC

e) Ninguna de las anteriores

---

### Página 94

Antes que todo, por conservación de la carga eléctrica, se cumple que:
Q1 (t) + Q2 (t) = Q ,

∀t

Consideremos el siguiente esquema, donde hemos dado un sentido a la corriente:

VC2

VC1
+

-

-

+

I
Aplicando la ley de mallas,
IR + VC2 − VC1 = 0
donde los signos ± en los voltajes de los condensadores dependen del sentido de la corriente, dado
que esta siempre circula de un potencial positivo a otro negativo. Reemplazando,
Q2 Q1
−
= 0
C
C
Q2 − Q1
IR +
= 0
C
2Q2 − Q
= 0
IR +
C
Q − 2Q2
I =
RC

IR +

Ahora, como el condensador C2 se está cargando (puesto que la corriente está entrando), entonces
I = Q̇2 , por lo que:
dQ2
Q − 2Q2
dt
RC

#### Problema 3.13.
Para la configuración del Problema 3.12, la carga Q2 (t) en función del tiempo es:


−t/RC
a) Q2 (t) = Q 1 − e


−2t/RC
b) Q2 (t) = Q 1 − e
c) Q2 (t) =


Q
1 − e−2t/RC

---

### Página 95


Q
−t/RC
1−e
d) Q2 (t) =

e) Ninguna de las anteriores
Del resultado del problema anterior,
dQ2
Q − 2Q2
dt
RC ,
ˆ
dQ2
dt
Q − 2Q2
RC

t
+α
− ln (Q − 2Q2 ) =
RC
Q − 2Q2 = β e−2t/RC
Como inicialmente Q2 (0) = 0,
Q − 2Q2 (0) = β
Luego,
Q2 (t) =

−→

β=Q


Q
1 − e−2t/RC

#### Problema 3.14.
Considere el circuito de la figura, el cual cuenta con dos resistencias (R y 2R) y un condensador de
capacitancia C inicialmente descargado.

V

t=0

R

I
I1

C

I2
2R
La corriente a través de la batería inmediatamente después de cerrar el interruptor, I0 , es:
a) I0 =

V
R

b) I0 =

V
3R

---

### Página 96

c) I0 =

3V
2R

d) I0 =

2V
3R

e) Ninguna de las otras alternativas
Como el condensador estaba inicialmente descargado, el condensador se comporta como un cortocircuito (cable sin resistencia), así que toda la corriente circula por dicha ruta, y nada por la rama
inferior. Así, la corriente es:
V
I0 =
R

#### Problema 3.15.
Considere el circuito del Problema 3.14. La corriente a través de la batería después de un tiempo MUY
largo, I∞ , es:
a) I∞ =

V
R

b) I∞ =

3V
2R

c) I∞ =

3V
R

d) I∞ =

2V
3R

e) Ninguna de las otras alternativas
Después de un tiempo MUY largo, el condensador está totalmente cargado y ya no circula corriente
por esa rama. Así, la corriente sería
V
I∞ =
3R

#### Problema 3.16.
Considere el circuito del Problema 3.14. La corriente en función del tiempo que pasa por el condensador,
IC (t), es:
a) IC (t) =

V −3t/(4RC)
e
2R

b) IC (t) =

V −3t/(4RC)
e
R

---

### Página 97

c) IC (t) =

V −3t/(2RC)
e
R

d) IC (t) =

2V −2t/(3RC)
e
3R

e) IC (t) =

V −4t/(3RC)
e
2R

Las ecuaciones del circuito son:
IR + VC − V = 0
2I2 R − VC = 0
I1 + I2 = I
dQ
Como el condensador se está cargando (la corriente I1 entra en el condensador), entonces I1 =
dt
y con ello:
Q
= 0
C
Q
Q
+
= 0
−V + RI1 +
2C C
,
3Q
d
−V + RI1 +
= 0
2C
dt

−V + R(I1 + I2 ) +

I˙1 +

con I1 (0) =

I1 = 0
2RC

V
como condición inicial. Resolviendo,
R
I1 (t) = IC (t) =

V −t/τ
e
,
R

τ=

2RC

#### Problema 3.17.
Para el siguiente circuito, calcule la potencia disipada en la resistencia R:

---

### Página 98

10 V
+
−

1Ω

2Ω

5V

2Ω

+
−

15 Ω

R=2Ω

1/5 Ω

4/3 Ω
a) P = 0.957 W
b) P = 1.500 W
c) P = 2.000 W
d) P = 1.086 W
e) P = 0.840 W
Definimos Req como la resistencia equivalente entre R y 4/3 Ω:
−1

+
= Ω
Req =
2Ω 4Ω
Sean Iu e Id las corrientes de las mallas superior e inferior (considerando la resistencia equivalente),
respectivamente, circulando a favor de las agujas del reloj. Así,
2Iu + 10 + Iu + 2Iu + 15(Iu − Id ) − 5 = 0
∴ 4Iu − 3Id = −1
Id + Id + 5 + 15(Id − Iu ) = 0
∴ 16Id − 15Iu = −5
Escribiendo el sistema anterior de forma matricial,


 

4 −3
Iu
−1
−15 16
Id
−5
Por tanto, y dado que solo nos interesa Id , utilizamos la regla de Cramer:
Id =

−15
−15

−1
−5
−3

=−

A

---

### Página 99

y la corriente Id circula, en realidad, en contra de las agujas del reloj. La diferencia de potencial VR
en la resistencia R es la misma que la diferencia de potencial en la resistencia equivalente Req :



A
Ω =
V
VR =
Finalmente,
PR =

VR 2
(28/19)2
W=
W ≈ 1.086 W
R

#### Problema 3.18.
Determine la corriente I del siguiente circuito:

2Ω

3 Ω (c) 4 Ω
(d)

(b)

+
−

(a)

I

12 V

a) I = 0.9 A
b) I = 12 A
c) I = 13 A
d) I = 1.1 A
e) I = 1.0 A
Notemos que Va = Vc y Vb = Vd . Así, la diferencia de voltaje en cada resistencia es:
V2 Ω = |Vb − Va | = |Vb − Vc | = V3 Ω
= |Vd − Vc | = V4 Ω
por lo que las tres resistencias están en paralelo. Sea R la resistencia equivalente entre las tres. Por
tanto,
−1

+
+
Ω
R=
2Ω 3Ω 4Ω

---

### Página 100

Finalmente, por la ley de Ohm,
I=

V
A = 13 A
R
12/13

#### Problema 3.19.
El siguiente circuito tiene el capacitor inicialmente descargado. En t = 0, el interruptor se cierra. ¿Cuál
es la corriente que atraviesa la batería inmediatamente después de cerrar el interruptor (I0 ) y después
de que el interruptor ha estado cerrado un largo tiempo (I∞ )?

50 V

20 Ω

+
−
5 µF

80 Ω
a) I0 = 2.5 A, I∞ = 0.5 A
b) I0 = 0.5 A, I∞ = 0.625 A
c) I0 = 0 A, I∞ = 0.5 A
d) I0 = 0.5 A, I∞ = 2.5 A
e) I0 = 2.5 A, I∞ = 0 A
Inicialmente el capacitor está descargado, por lo que no hay caída de potencial en él, y la corriente
a través de la resistencia de 80 Ω es cero. Por tanto,
I0 =

50 V
= 2.5 A
20 Ω

Después de un tiempo muy largo, el capacitor está totalmente cargado y no hay corriente a través
de él. En este caso,
50 V
I∞ =
= 0.5 A
20 Ω + 80 Ω

---

### Página 101

#### Problema 3.20.
Considere el siguiente circuito, donde los capacitores están totalmente cargados. ¿Cuál es la energía
almacenada en el capacitor de 3 µF?

2Ω
6 µF
+
−
3V

2Ω

2Ω

3 µF
2V
+
−

a) 0.52 × 10−6 J
b) 0.67 × 10−6 J
c) 0.55 × 10−3 J
d) 0.65 × 10−3 J
e) 0.61 × 10−3 J
Como los condensadores están totalmente cargados, no circula corriente por ellos. Así, es fácil ver
que la corriente que circula por la fuente de voltaje es:
I=

3V
= 1A
2 Ω + (2 Ω k 2 Ω)

Así, la diferencia de potencial entre las resistencias de 2 Ω es:
V2 Ω = IRparalelo = (1 A)(1 Ω) = 1 V
Aplicando ley de mallas a la malla con los condensadores,
V2 Ω = 1 V = 2 V − V6 µF − V3 µF
donde hemos colocado un signo menos a los voltajes en los condensadores pues el voltaje resultante
(1 V) es menor que el voltaje suministrado por la fuente (2 V). Ahora, como los condensadores están
en serie,
Q
Q
V6 µF =
∧
V3 µF =
6 µF
3 µF
Despejando, obtenemos que Q = 2 µC. Así, la energía almacenada en el condensador solicitado es:
U=

(2 × 10−6 )2
Q2
J = × 10−6 J ≈ 0.67 × 10−6 J
−6
2C
2(3 × 10 )

---

### Página 102

Magnetostática

Ecuaciones de Maxwell en uno de los muros exteriores de la Universidad de Varsovia

---

### Página 103

#### Problema 4.1.
Se tiene una espira cuadrada, de lado 2a, por la cual fluye una corriente I. A una distancia a de la espira
se encuentra un alambre MUY largo por el que fluye también una corriente I (ver figura). Entonces, la
magnitud de la fuerza que la espira ejerce sobre el alambre es:

I

I
a

a)

µ0 I 2
3π

b)

2µ0 I 2
3π

c)

µ0 I 2
2π

d)

3µ0 I 2
2π

2a

e) Ninguna de las otras alternativas
Es más fácil calcular la fuerza que el alambre ejerce sobre la espira, que es igual en módulo (pero
de dirección opuesta) a la fuerza pedida. Por la ley de Ampère, el campo magnético generado por
un cable infinitamente largo es:
~ alambre = µ0 I θ̂
B
2πr
Para fijar un sistema de coordenadas, supongamos que el alambre yace en el eje Y , la espira cuadrada
pertenece al plano XY , y el origen O como la proyección del lado de la espira más bajo sobre el
alambre. Ahora bien, la fuerza que el alambre ejerce sobre los lados perpendiculares de la espira
(superior e inferior) se anulan entre sí, ya que la distancia es igual y las corrientes que circulan por
ellos de sentido opuesto. La fuerza sobre el lado más cercano al cable es:
ˆ 2a
~
~
F1 = I
d~ℓ × B
ˆ 2a
µ0 I
k̂
= I
dy ̂ × −
2πa
µ0 I 2
= −
ı̂
π

---

### Página 104

y la fuerza es atractiva. La fuerza sobre el lado más lejano viene dada por:
ˆ 2a
~
~
F2 = I
d~ℓ × B
ˆ 2a
µ0 I
k̂
= I
−dy ̂ × −
6πa
µ0 I 2
ı̂
3π
y resulta ser repulsiva. Así, la fuerza total es:

2µ0 I
F~total = F~1 + F~2 = −
ı̂
3π
con módulo
F = kF~ k =

2µ0 I 2
3π

#### Problema 4.2.
En el alambre de la figura, el radio de la semi circunferencia es r, y las dos ramas rectas se extienden
hasta el infinito. Por el alambre circula una corriente I. En tal caso, el módulo y dirección del campo
magnético en el centro C es:

b

C

I

I

µ0 I
entrando en el papel
4r
µ0 I
entrando en el papel
b)
4πr
µ0 I
c)
entrando en el papel
2r
µ0 I
saliendo del papel
d)
4πr
µ0 I
e)
saliendo del papel
2r
a)

Recordemos la fórmula de Biot-Savart para el cálculo de campo magnético:
~ r ) = µ0
B(~
4π

ˆ

~ × (~r − R)
~
I dR
~ 3
k~r − Rk

---

### Página 105

En este caso, ~r = ~0 tomando un sistema de coordenadas conveniente en el que el origen está en C y
~ yR
~ son paralelos, pues es
el eje Z sale del papel. En el caso de las porciones rectas, los vectores dR
una recta, y por tanto el producto cruz se anula. Así, dichas porciones no crean campo magnético
en C. Por otra parte, para el caso del segmento semicircular,
~ = r ρ̂ ,
R

~ = r dθ θ̂ ,
dR

µ0
~
B(C)
4π

ˆ π

~ 3 = r3
k~r − Rk

Reemplazando,

µ0 I
−Ir dθ θ̂ × (−r ρ̂)
k̂
=−
r
4r

y el campo entra al papel.

#### Problema 4.3.
Por la superficie de un cascarón cilíndrico de largo L y radio R ≪ L circula una corriente de densidad
lineal Js , como se muestra en la figura. El campo magnético en el eje del cilindro es:

a) µ0 Js /L
b) µ0 Js /2
c) µ0 Js L
d) µ0 Js
e) πR2 µ0 Js /L
Como R ≪ L, el campo afuera se puede considerar nulo. Aplicamos la ley de Ampère sobre un
circuito rectangular, con un lado adentro (en el eje, donde queremos calcular el campo) y el otro
lado afuera (en un punto r > R) donde el campo es cero. El alto del circuito rectangular es h. Así,
˛
~ · d~r = B(0)h − B(r)h = µ0 Iencerrado = µ0 Js h
B
Por tanto, la respuesta correcta es:
B(0) = µ0 Js

---

### Página 106

#### Problema 4.4.
Tres alambres rectos están dispuestos en forma paralela como se muestra en la figura. Los alambres
están separados una distancia d uno de otro, y por los tres circula la misma corriente I. Los alambres
están limitados a moverse en el plano. El del centro se encuentra en equilibrio estable si las corrientes
tienen el siguiente sentido:

(A)

(B)

(C)

(D)

a) Caso (A)
b) Caso (B)
c) Caso (C)
d) Caso (D)
e) Nunca se encuentra en equilibrio
Si se permite movimiento en tres dimensiones, los cables nunca están en equilibrio estable. Si se
encuentran obligados a moverse en el plano, hay una posición de equilibrio estable para el alambre
del medio. Se encuentra en equilibrio si al desplazarse hacia un lado la fuerza neta lo hace volver a
su posición original. La situación de equilibrio estable es el Caso (C), puesto que ambos alambres
repelen al del medio; si se acerca a un cable, este lo repele con más intensidad que el que está más
lejos y lo devuelve a su posición.

#### Problema 4.5.
Considere un conductor plano, de espesor despreciable, ubicado en el plano XY . Por este plano circula
una densidad de corriente lineal J0 ı̂ como se muestra en la figura. El campo magnético en la región
z > 0 es:

a) −(µ0 J0 /2) ̂
b) +(µ0 J0 /2) ̂
c) −µ0 J0 ı̂

---

### Página 107

d) +µ0 J0 ı̂
e) −2µ0 J0 ̂
Elegimos aplicar la ley de Ampère al circuito rectangular con un borde fuera, el otro adentro y
dimensiones L, h recorrido anti-horario. Por simetría, el campo es igual en módulo en los dos lados
paralelos que se encuentran equidistantes del plano. Entonces, como el campo magnético apunta en
la misma dirección que ambos segmentos paralelos, nos queda:
2BL = µ0 J0 L
y, por tanto, la alternativa correcta es:
~ = −(µ0 J0 /2) ̂
B
donde el signo y la dirección provienen de la regla de la mano derecha.

#### Problema 4.6.
Considere un cilindro sólido, de radio a y MUY largo, por el cual circula una densidad de corriente con
~
simetría cilíndrica J(r)
= (1 − r 2 /a2 )J0 k̂ paralela al eje Z. El módulo del campo magnético en r > a
es:
a)

µ0 a2 J0
2r

b)

µ0 a2 J0
4r

c) 0 T
d)

µ0 a2 J0

e)

µ 0 r 2 J0
4a

~ r ) = B(r) θ̂. Usando la ley de Ampère, para un circuito
Por simetría, el campo es de la forma B(~

---

### Página 108

en forma de circunferencia de radio r > a en el exterior, encontramos:
˛
~ · d~r = µ0 Ienc
B
¨
2πrB(r) = µ0
J~ · n̂ dS

ˆ 2π ˆ a 
r2
= µ 0 J0
1 − 2 r dr dθ
a
µ0 J0 πa
Con ello, el campo tiene magnitud:
B(r > a) =

µ0 a2 J0
4r

#### Problema 4.7.
En la misma situación del Problema 4.6, el campo magnético en r < a tiene magnitud:
µ 0 J0 r
a)
b)



r2
1− 2
a

µ 0 J0 r



r2
1+ 2
a


r2
µ 0 J0 r
1+ 2
d)
2a


µ 0 J0 r
r2
e)
1− 2
2a
µ 0 J0 r
c)

De la misma forma que en el Problema 4.6,



ˆ 2π ˆ r 
r′2
r2
′
′
2πrB(r) = µ0 J0
1 − 2 r dr dθ = πµ0 J0 r 1 − 2
a
2a
Así,
µ 0 J0 r
B(r < a) =



r2
1− 2
2a

---

### Página 109

#### Problema 4.8.
Dos protones entran con velocidades de distinta magnitud a una zona con campo magnético uniforme,
como muestra la figura.

A
B

¿Qué protón es el más veloz?
a) A es más veloz que B
b) B es más veloz que A
c) A y B son igualmente veloces
d) No se puede decidir porque A y B cambian su rapidez en el campo magnético
e) No se puede decidir porque lo observado no tiene que ver con rapidez
Como la fuerza es radial, podemos afirmar que:
|q|vB =

mv 2
r

−→

v=

|q|rB
m

y, a igual masa y carga eléctrica, la partícula con mayor radio de giro es la que va más rápido, que
en este caso corresponde al protón B.

#### Problema 4.9.
En el experimento de Problema 4.8, si ambos protones entran a la zona con campo magnético al mismo
tiempo, ¿cuál va a salir de esta zona primero?
a) A sale primero
b) B sale primero
c) Ni A ni B salen porque hacen vueltas circulares

---

### Página 110

d) A y B salen al mismo tiempo
e) No se puede decidir
Como la rapidez angular satisface v = ωr, entonces:
ω=

|q|B
m

Así, ambos protones poseen la misma rapidez angular. Como el periodo T (tiempo que le toma dar
2π
una vuelta) es igual a T =
, ambos protones poseen el mismo periodo. Finalmente, y dado que
ω
la trayectoria involucra medio ciclo, ambos protones demoran T /2 en salir de la zona, y lo hacen al
mismo tiempo.

#### Problema 4.10.
Un portador de carga está siendo acelerado desde el reposo, en la posición O, por dos electrodos E1 y E2
con un voltaje (diferencia de potencial) U. Después, entra a una zona con campo magnético uniforme
~ (ver figura). Hay dos aperturas simétricas A y B.
B
L

(A)

E1 E2

a
b

O

(B)

Si el portador de carga es un electrón, ¿qué polaridad deben tener los electrodos? ¿por cuál apertura
puede salir el electrón?
a) E1 negativo, E2 positivo, salida por apertura B
b) E1 positivo, E2 negativo, salida por apertura B
c) E1 positivo, E2 negativo, salida por apertura A

---

### Página 111

d) E1 negativo, E2 positivo, salida por apertura A
e) No puede salir
Elijamos el sistema de coordenadas de modo que el plano del papel coincida con el plano XY , con
el eje Z saliendo del papel. La velocidad inicial es v0 ı̂ y el campo magnético es −B k̂. Por lo tanto,
un carga negativa siente una fuerza dirigida en dirección −̂ y se curva hacia abajo, saliendo por
B. Por otro lado los electrodos E1 y E2 tienen que acelerar la carga. Como se trata de una carga
negativa, que se mueve de potencial bajo hacia potencial alto, E2 tiene que ser el electrodo positivo.

#### Problema 4.11.
Considerando la configuración del Problema 4.10, si el portador de carga es un protón, ¿en qué rango
de voltaje U el protón pasa por una de las aperturas, A o B?
B 2 qb2
B 2 qa2
a)
<U <
8m
8m


 2
B 2 q L2
B 2 q L2
<U <
b)
2m 2a
2m 2b

2

2
B 2 q a2 + L2
B 2 q b2 + L2
<U <
c)
2m
2L
2m
2L

2

2
B 2 q b2 + L2
B 2 q a2 + L2
d)
<U <
2m
2a
2m
2b

2

2
B 2 q ab + L2
B 2 q ab + L2
<U <
e)
2m
2a
2m
2b
En la siguiente figura dibujamos la trayectoria circular de una carga que sale por la parte inferior
de la apertura A. Esta es la trayectoria más veloz que sale por A, ya que si va más rápido, se curva
menos y choca con la pared:

---

### Página 112

R

a

R
b

L
Como sabemos, la carga describe un círculo que satisface:
mv 2
= qvB
R
y su energía cinética es producto de la aceleración que le da el voltaje U, es decir:
mv 2
= qU
Si eliminamos v de estas dos ecuaciones, tenemos:
 2
qB
R2
U=
2m
De la figura se ve que:
R2 = L2 + (R − b)2

−→

R=

L2 + b2
2b

Reemplazando este radio en la fórmula anterior, se obtiene que:

2
qB 2 L2 + b2
U=
2m
2b
Esta es la trayectoria de máxima velocidad, y por lo tanto corresponde al voltaje máximo. La
trayectoria que sale por el extremo superior de la apertura A es la que sale a menor velocidad, y el
desarrollo algebraico es idéntico, intercambiando a ↔ b. Así, la alternativa correcta es:
B 2q
2m

 2
2

2
a + L2
B 2 q b2 + L2
<U <
2a
2m
2b

---

### Página 113

#### Problema 4.12.
~ describiendo
Un electrón (carga q = −e) pasa dentro de una zona con campo magnético uniforme B,
una trayectoria en forma de arco y con distancia recorrida L. ¿Cuánto aumenta su energía cinética?
a) 0 J
b) +eBL
c) −eBL
d) +eBL/2
eBL
e) − √
El movimiento en un campo magnético no cambia la energía cinética de una carga, solo la dirección
de su movimiento.

#### Problema 4.13.
Un portador de carga q y masa m entra a una zona con campo magnético B y campo eléctrico E
paralelos e uniformes, y después sale de ella (ver figura). La velocidad inicial es ortogonal a los campos.
¿Cuánto cambia la energía cinética del electrón en este recorrido?

~v0

~ kE
~
B
a) 0 J

2
E
π
B

2
m
E
π
c) +
B
2

E
d) +2m π
B

m
b) −

---

### Página 114



E
e) −2m π
B

2

Elijamos el sistema de coordenadas de modo que el plano del papel sea el plano XY con el eje Z
saliendo del papel. Al entrar a la región con campos no nulos, la partícula va a girar en el plano XZ
y acelerar en la dirección ̂. La componente vertical de la velocidad será, entonces,
qE
t
m

vy (t) =

ya que inicialmente no tiene velocidad según ̂. El vector que agrupa las componentes ı̂ y k̂ de
la velocidad, (vx , vz ), no cambia de módulo porque el campo magnético no hace trabajo. Sale de
la región una vez que ha realizado un semicírculo en el plano XZ. El tiempo que demora es T /2,
donde T es el periodo del movimiento circular. Como T = 2π/ω, y ω = qB/m, la velocidad vertical
al momento de salir es:
qE π
πE
vy (T /2) =
mω
B
La energí a cinética aumenta

mvy 2
, por lo que la respuesta correcta es:

2
E
m
π
+
B

#### Problema 4.14.
El Sodio, en particular, es un conductor donde la teoría clásica del efecto Hall nos da resultados aproximadamente correctos. Considere un segmento conductor de sodio de espesor b = 1 mm y anchura
a = 2 mm, como se muestra en la figura. El conductor porta una corriente constante de I = −1 A y está
colocado en un campo magnético uniforme de B = 1 T perpendicular al plano a − c. En consecuencia,
se produce un voltaje Hall de −0.25 µV. Determine la concentración de los electrones libres en el sodio,
recordando que e = −1.6 × 10−19 C.

B

c
b
a
I
a) n = 2.00 × 1028 m−3

---

### Página 115

b) n = 2.00 × 10−28 m−3
c) n = 1.25 × 1028 m−3
d) n = 2.50 × 1028 m−3
e) Ninguna de las anteriores
Igualando las fuerzas eléctrica y magnética que actúan sobre los portadores de carga, encontramos:
qE = qvB

−→

E = vB

En este caso, el potencial de Hall está dado por V = Ea, por lo que:
V = avB
Finalmente, la corriente nos ayuda a determinar la velocidad de las cargas, puesto que I = envab.
Así,
V =

BI
enb

−→

n=

BI
1·1
m−3 = 2.50 × 1028 m−3
−19
−6
−3
eV b
1.6 × 10
· 0.25 × 10 · 1 × 10

#### Problema 4.15.
Por un cable coaxial MUY largo circula una corriente I con densidad constante en cada conductor. La
corriente entra por el conductor interno y regresa por el externo. Ambos cables están separados por un
material aislante de permeabilidad µ0 . Determine el campo magnético en un punto b < r < c del eje ρ̂
según indica la figura.

a b c

µ0 I
a)
2πr



r 2 − b2
−1 + 2
c − b2

b) 0 T
c)

µ0 I
2πr

µ0 I
d)
2πr



r 2 + b2
−1 + 2
c + b2

r

---

### Página 116

e)

µ0 I(b − a)
2πr

Elegimos un sistema coordenado en el que el plano del papel coincide con el plano XY , con el eje
~ = B(r) θ̂ y con ello:
Z saliendo de la hoja. De la ley de Ampère, proponemos que B
2πr B(r) = µ0 Ienc

−→

B(r) =

µ0 Ienc
2πr

Como deseamos calcular el campo magnético en un punto b < r < c, notamos que en anillo
amperiano encierra completamente a la corriente interior y solo parte de la corriente del conductor
exterior. Por tanto,
Ienc = −I + J(πr 2 − πb2 )
donde los signos de las corrientes están dados por la regla de la mano derecha y J es la densidad de
corriente en el conductor externo, que al ser constante por enunciado, cumple que:
I

J=

πc2 − πb2

Reemplazando,
µ0 I
B(r) =
2πr



r 2 − b2
−1 + 2
c − b2

#### Problema 4.16.
Una espira circular de radio R = 0.5 cm es colocada cerca a un alambre recto y MUY largo, según
indica la figura. Una corriente estacionaria I = 2 A va de izquierda a derecha por el alambre recto. Si
en la espira circular también hay una corriente estacionaria Iesp , ¿cuál debe ser su magnitud para que
el campo magnético neto sea cero en el centro de la espira?

R

R/2
I

a) 0.42 A
b) 0.15 A
c) 2.00 A
d) 2.54 A

---

### Página 117

e) 0.31 A
Si tomamos un sistema coordenado tal que ambas figuras estén ubicadas en el plano XY , con el eje
Z saliendo del papel y el alambre recto coincidiendo con el eje X. En este sistema de coordenadas,
la el campo magnético que genera el alambre en el origen es:
~ alamb (C) =
B

µ0 Ialamb
µ0 Ialamb
k̂ =
k̂
2π(R + R/2)
3πR

El campo magnético de una espira de radio R en su eje de simetría se obtiene por la ley de Biot~ = R ρ̂ y ~r = z k̂:
Savart, con R
~ × (~r − R)
~
Iesp dR
~ 3
k~r − Rk
ˆ 2π
R dθ θ̂ × (z k̂ − R ρ̂)
µ0 Iesp
4π
(R2 + z 2 )3/2
R2
µ0 I
k̂
2 (R2 + z 2 )3/2

~ esp (z) = µ0
B
4π

ˆ

~ esp (C) = µ0 Iesp k̂
∴ B
2R
Para que el campo sea nulo en el centro de la espira, la corriente Iesp debe circular en el mismo
sentido de las agujas del reloj, y su magnitud debe ser:
Iesp =

2Ialamb
= 0.42 A
3π

#### Problema 4.17.
Una esfera de radio R está cargada uniformemente con una densidad volumétrica de carga ρ constante.
La esfera rota en torno a uno de sus diámetros con velocidad constante ω
~ = ω k̂. Encuentre el campo
magnético en el centro de la esfera.
~
a) B(0)
=−

µ0 ρR2
~ω

~
b) B(0)
=−

2µ0 ρR2
~ω

~
c) B(0)

µ0 ρR2
~ω

2µ0 ρR
~
ω
~
d) B(0)
e) Ninguna de las anteriores

---

### Página 118

Consideraremos que la esfera está compuesta por discos infinitesimales. A su vez, cada una de esos
discos está compuesto por anillos infinitesimales. Cada anillo aporta con un diferencial de campo
magnético:
a2
~ = µ0 dI
k̂
dB
2 (a2 + z 2 )3/2
donde a es el radio del disco y z es la altura de cada anillo, respecto al plano XY . En coordenadas
esféricas,
p
a = x2 + y 2 = r sin θ
∧
z = r cos θ
Por otra parte, el diferencial de corriente viene dado por:
dI =

dq
ρdV
= ωρ r 2 sin θ dθ dr
T
2π/ω

donde ya hemos integrado la componente φ por la simetría rotacional del problema. Juntando los
términos,
ˆ πˆ R 2 2
r sin θ 2
µ
ωρ
~
r sin θ dr dθ k̂
B(C)
r3
ˆ ˆ
µ0 ωρ π R
r sin3 θ dr dθ k̂
µ0 ωρR
k̂

#### Problema 4.18.
Un cable recto MUY largo, colocado a lo largo del eje Z, lleva una corriente I en la dirección positiva
de z. Se coloca un dipolo magnético m
~ = m0 ̂ en el eje X, a una distancia xp del alambre. El torque
sobre m
~ es:
a) ~τ = ~0
b) ~τ =

m0 I
k̂
2πxp

c) ~τ =

m0 I
ı̂
2πxp

d) ~τ =

m0 I
̂
2πxp

e) ~τ = −

m0 I
ı̂
2πxp

---

### Página 119

Recordemos que el campo magnético de un cable infinito es:
~ = µ0 I θ̂
B
2πr
En coordenadas cartesianas,
r=

p
x2 + y 2 ,

x ̂ − y ı̂
θ̂ = p
x2 + y 2

Como deseamos el campo magnético en el punto (xp , 0),

~ dipolo = µ0 I xp ̂
B
2π
Así,

~ dipolo = ~0
~τ = m
~ ×B

#### Problema 4.19.
Un alambre infinito con corriente I1 , en el sentido del eje Z, coincide con dicho eje. Otro alambre infinito,
con corriente I2 , se encuentra en el plano XY a una distancia d constante del eje Y , como indica la
figura. Entonces, la fuerza por unidad de largo de I1 sobre I2 es:

y

I2
z
bb

x

I1
d
a)

dF~
µ 0 I1 I2
y
k̂
dy
4π d + y 2

b)

µ 0 I1 I2
d
dF~
k̂
dy
4π d + y 2

c)

dF~
µ 0 I1 I2
d
k̂
dy
2π d + y 2

d)

µ 0 I1 I2
dF~
y
k̂
dy
2π d + y 2

---

### Página 120

e) Ninguna de las anteriores
El campo magnético de la corriente I1 es:
µ 0 I1
µ 0 I1
~
B(x,
y) =
θ̂ =
(−y ı̂ + x ̂)
2πr
2π(x2 + y 2 )
donde la última igualdad proviene de escribir el campo en coordenadas cartesianas. Ahora bien, el
diferencial de fuerza sobre un segmento del conductor de largo dy es:
~ y) = I2 dy ̂ ×
dF~ = I2 dy ̂ × B(d,

µ0 I1 I2 y dy
µ 0 I1
k̂
(−y ı̂ + d ̂) =
2π(d + y )
2π(d2 + y 2)

#### Problema 4.20.
Se tieneun cascarón
semi-esférico (sin tapa) de radio R a través del cual fluye un campo magnético

~ = B0 ı̂ + 1 ̂ . Entonces, el flujo magnético a través del cascarón es:
B
a) ΦB =

2πR2
B0

b) ΦB = 2πR2 B0
c) ΦB = 0
d) ΦB =

πR2
B0

e) Ninguna de las anteriores
Sea S la superficie descrita en el enunciado, y D la tapa de modo tal que S + D es una superficie
cerrada que encierra un volumen V . Así, por el teorema de la divergencia,
¨
˚
~
~ dV = 0
B · n̂ dS =
∇·B
S+D

V

pues la divergencia del campo magnético siempre es nula. Con ello,
¨
¨
~ · n̂ dS = − B
~ · n̂ dS
ΦB =
B
S

D

con las normales apuntando hacia afuera. La tapa se puede parametrizar como:
T : (r, θ) 7→ (0, r cos θ, r sin θ)

---

### Página 121

Calculando la integral de superficie,
¨
¨
~ · n̂ dS =
~ · ~n dr dθ
B
B
D

D

ˆ R ˆ 2π

B0

= −πR B0




1, , 0 · (−r, 0, 0) dθ dr

Así,
ΦB = πR2 B0

#### Problema 4.21.
Se realiza un experimento con rayos de partículas cargadas que inciden en un campo magnético uniforme
de magnitud B = 0.5 T (ver figura). Se sabe que las partículas inciden con una velocidad de v =
0.5 × 106 m s−1 . Suponga que, al entrar a la zona de campo magnético no nulo, las partículas describen
una órbita semi-circular de radio R = 1.5 m. Despreciando efectos de la gravedad, podemos deducir que
la razón carga/masa es:
b

b

b

b

b

b

b

b

b

b

b

b

2R
b

b

b

b

b

b

b

b

b

b

b

b

b

b

b

b

b

b

b

b

a) q/m = 2/3 × 106 C kg−1
b) q/m = 3/4 × 106 C kg−1
c) q/m = −2/3 × 106 C kg−1
d) q/m = −3/4 × 106 C kg−1
e) Ninguna de las anteriores
Primero que todo, notemos que la regla de la mano derecha nos indica que las partículas deben

---

### Página 122

tener carga negativa para que la trayectoria sea como la descrita en la figura. Ahora bien, respecto
a la magnitud de la carga, tenemos que:
|q|vB =

mv 2
R

−→

|q|
v
0.5 × 106
= × 106 C kg−1
m
BR
0.5 · 1.5

#### Problema 4.22.
Un anillo de radio R y carga Q está rotando con velocidad angular ω en torno al eje Z. La magnitud
del campo magnético en el eje Z, en un punto MUY lejano del anillo (z ≪ R), puede ser aproximado
por:
a)

µ0 QωR2
4πz 3

b)

µ0 QωR
4πz 2

c)

µ0 QωR2
8πz 3

d)

µ0 QωR
8πz 2

e) Ninguna de las anteriores
Si el anillo rota y está cargado, entonces su corriente viene dada por:
I=

Q
Qω
T
2π

con T el periodo de rotación. Ahora bien, el campo magnético producido por una espira de radio R
por la que circula una corriente I en su eje de simetría tiene magnitud:
B(z) =

R2
µ0 I
2 (z 2 + R2 )3/2

Si z ≫ R, entonces podemos aproximar la expresión anterior hasta obtener:
B(z ≫ R) ∼

µ0 I R 2
2 z3

B(z ≫ R) ∼

µ0 QωR2
4πz 3

Reemplazando:

---

### Página 123

#### Problema 4.23.
Una partícula de carga q > 0 y masa m ingresa con velocidad ~v = v ı̂ a una región con un campo
~ constante, como indica la figura. ¿A qué distancia d, del plano de entrada, es detectada
magnético B
la partícula?
b

~
B

~v
L
d

y
x

a) d =

r

mvL
qB

b) d =

r

mvL
− L2
qB

mv
qB
r
2mvL
d) d =
− L2
qB
c) d =

e) d = L
Primero que todo, notamos que la fuerza magnética provoca un movimiento circular tal que:
mv 2
R

qvB =

−→

R=

Por otra parte, tenemos la siguiente situación:

L
d
b

R−L

b

R
b

mv
qB

---

### Página 124

Por Pitágoras,
(R − L)2 + d2 = R2

−→

d=

√

2RL − L2

Reemplazando,
d=

s

2mvL
− L2
qB

#### Problema 4.24.
Una carga Q > 0 entra con posición inicial ~r(0) = ~0 y velocidad ~v (0) = v0 ı̂ en un espacio entre dos
placas paralelas (capacitor), que se encuentran a una distancia d, sometidas a una diferencia de potencial
~ = Bx ı̂ + By ̂. Asumiendo que el
U. Además, en el espacio entre las placas hay un campo magnético B
campo eléctrico en el capacitor es constante, ¿con qué velocidad v0 tiene que entrar la partícula para
que salga en línea recta por la abertura indicada en el lado derecho de la figura?
z
y
x

Q
b

~v

~
B

d

U
a) v0 =

U
Bx d

b) v0 = q
c) v0 =

U
Bx 2 + By 2 d

U
By d

d) v0 = q

U
Bx 2 − By 2 d

e) Ninguna de las anteriores

---

### Página 125

Para que se mueva en línea recta, la suma de fuerzas en el eje Z debe ser igual a cero. Si calculamos
la fuerza neta sobre la carga,
~ + ~v × B)
~
F~ = Q(E
El campo eléctrico tiene magnitud E = U/d, con dirección − k̂ puesto que el potencial crece hacia
~ = v(t)By k̂
arriba. Por otra parte, como la partícula se mueve en línea recta, ~v = v(t) ı̂. Así, ~v × B
y por tanto:


U
F~ = Q − + v(t)By k̂
d
Como la fuerza solo apunta en el eje Z, al ser esta nula la velocidad de la partícula será constante,
i.e. v(t) = v0 . Para que la fuerza sea nula, se debe cumplir que:
v0 =

U
By d

#### Problema 4.25.
La fuerza total sobre la espira de la figura es:

a) F~ = 2πrIB sin θ k̂
b) F~ = 2πrIB cos θ ρ̂
c) F~ = −2πrIB sin θ ρ̂
d) F~ = −2πrIB sin θ k̂
e) F~ = πrIB sin θ k̂

---

### Página 126

La fuerza sobre la espira viene dada por:
F~ = I

ˆ

~
d~ℓ × B

Para describir la situación, utilizaremos coordenadas cilíndricas (r, ϕ, z). Tomemos un segmento del
anillo de largo d~ℓ = −r dϕ ϕ̂, donde el signo menos se debe a la dirección de la corriente (a favor de
las agujas del reloj). Por otra parte, el campo magnético puede escribirse como:
~ = B sin θ ρ̂ + B cos θ k̂
B
Por tanto,


~ = rB dϕ sin θ k̂ + cos θ ϕ̂
d~ℓ × B

Así, integrando entre 0 y 2π, la contribución angular se anulará puesto que ϕ̂ = − sin ϕ ı̂ + cos ϕ ̂.
Por otra parte, la contribución en el eje Z nos dará un factor 2π. Finalmente,
F~ = 2πrIB sin θ k̂

#### Problema 4.26.
La figura muestra la velocidad de una carga puntual negativa y la fuerza magnética que actúa sobre
esta. La dirección del campo magnético en las distintas situaciones es:
F~B

F~B

F~B
~v
(i)

b

~v

~v

(ii)

(iii)

a) (i) hacia abajo, (ii) entra en la página, (iii) sale de la página
b) (i) hacia la derecha, (ii) hacia abajo, (iii) hacia arriba
c) (i) entra en la página, (ii) hacia la derecha, (iii) hacia abajo
d) (i) sale de la página, (ii) hacia la izquierda, (iii) hacia arriba
e) (i) entra en la página, (ii) hacia la izquierda, (iii) hacia abajo
#### Problema 4.27.
Una partícula de carga q = 2 C y masa M = 1 kg se mueve en el plano XY . En t = 0, la partícula se
encuentra en el punto ~r0 = (−1, 0, 0) m y su velocidad es ~v0 = (0.5, 0, 0) m/s. En la región x > 0 hay un
~ = (0, 0, B), donde B = 0.5 (N s)/(C m), como se muestra la figura. ¿En
campo magnético uniforme B
qué instante, aproximadamente, la partícula sale de la región donde hay campo magnético?

---

### Página 127

y
b

b

b

~
B
b

b

b

b

b

b

x

~v0
b

b

b

a) 6.3 s
b) 1.0 s
c) 7.1 s
d) 8.3 s
e) 5.1 s
El tiempo requerido corresponde a la suma del tiempo que la partícula demora en ingresar a la
región con campo magnético (t1 ) y el tiempo que demora en dar media vuelta para salir del campo
(t2 ). Dado que la partícula se mueve con velocidad constante en x < 0,
t1 =

1m
d
= 2s
v0
0.5 m/s

En el caso de t2 , este tiempo corresponde a la mitad del periodo de rotación de la partícula:


3.14 · 1
1 2πm
T
≈
s ≈ 3.14 s
t2 = =
2 qB
2 · 0.5
Por tanto,
∆t = t1 + t2 ≈ 5.14 s

#### Problema 4.28.
Calcule la magnitud del campo magnético creado por el cilindro infinito de la figura, si este porta una
R
densidad de corriente J~ = J0 k̂ en coordenadas cilíndricas.
r

---

### Página 128

R
b

J~

a) B(r < R) = µ0 J0 R y B(r > R) =

µ 0 J0 R 2
r

b) B(r < R) = µ0 J0 r y B(r > R) =

µ 0 J0 r 2
R

c) B(r < R) =

µ 0 J0 R 2
y B(r > R) = µ0 J0 R
r

d) B(r < R) = 2πµ0 J0 R y B(r > R) =

2πµ0 J0 R2
r

e) Ninguna de las anteriores
~ = B(r) θ̂. Así, para un anillo amperiano
De acuerdo a la simetría del problema, proponemos que B
de radio r, la ley de Ampère nos dice que:
˛
µ0 Ienc
~ · d~r = 2πr B(r) = µ0 Ienc
B
−→
B(r) =
2πr
Para r < R,
Ienc =

¨

J~ · n̂ dS = 2πJ0 R

S

ˆ r

r ′ dr ′
= 2πJ0 Rr
r′

con lo que:
B(r < R) = µ0 J0 R
Para r > R,
Ienc = 2πJ0 R

ˆ R

dr ′ = 2πJ0 R2

y, por tanto,
B(r > R) =

µ 0 J0 R 2
r

#### Problema 4.29.
Considere un par de hilos no conductores paralelos, separados a una distancia d y MUY largos (L ≫ d).

---

### Página 129

Ambos poseen una carga distribuida uniformemente con densidad λ. ¿Cuál debe ser la velocidad v
(medida en un sistema inercial) de los hilos para que la fuerza magnética anule la fuerza eléctrica entre
ellos? Recuerde que c = (µ0 ε0 )−1/2 ≈ 3 × 108 m/s es la velocidad de la luz.

λ

λ

v

v
d

a) v = 108 m/s
b) v = 2 × 108 m/s
c) v = 4 × 108 m/s
d) v = 6 × 108 m/s
e) v = 3 × 108 m/s
Supongamos que uno de los alambres se ubica en el eje Z. Así, el campo eléctrico que genera es:
~ =
E

λ
ρ̂
2πε0 r

Con ello, la fuerza eléctrica sobre el segundo cable, ubicado a una distancia d del eje Z, es:
ˆ L
ˆ L
λ2
λ2 L
~
~
FE =
E dq =
dz ρ̂ =
ρ̂
2πε0 d 0
2πε0 d
Por otro lado, el campo magnético generado por el primer alambre será:
~ = µ0 I ρ̂ = µ0 λv ρ̂
B
2πr
2πr
donde la corriente que circula, visto desde un sistema referencial en reposo, es I = λv. La fuerza
magnética sobre el segundo alambre será, entonces,
ˆ
ˆ L
µ 0 λ2 v 2 L
µ 0 λ2 v 2 L
~
~
~
dz ρ̂ = −
ρ̂
FB = I
dℓ × B = −
2πd 0
2πd

---

### Página 130

Finalmente, para que F~B + F~E = ~0, se debe cumplir:
λ2 L
µ 0 λ2 v 2 L
2πε0d
2πd
= v2
µε0
∴ v = √
µ0 ε0

#### Problema 4.30.
Un cable con N vueltas y corriente I enrolla un donut de radios R y a < R como muestra la figura.
¿Cuánto vale el módulo del campo magnético en cualquier punto del plano del donut (punto r de la
figura)?

~ =0
a) kBk

~ = µ0 NI
b) kBk
πr
~ = µ0 NI
c) kBk
2πr
~ = µ0 NI
d) kBk
4πr
e) Ninguna de las anteriores
~ = B(r) θ̂. Consideremos un anillo
La simetría de la configuración nos permite proponer que B
amperiano de radio r en el interior del donut, tal que d~r = r dθ θ̂. Por ley de Ampère,
˛
~ · d~r = 2πr B(r) = µ0 Ienc = NI
B
Por tanto,
~ = B(r) =
kBk

µ0 NI
2πr

---

### Página 131

Inductancias y flujo magnético

Ecuaciones de Maxwell en uno de los muros exteriores de la Universidad de Varsovia

---

### Página 132

#### Problema 5.1.
Asumiendo que en un tiempo t = 0 el condensador se encuentra descargado y que B0 > 0 (el campo
sale de la página), la corriente que circula por el circuito de la figura es, como función del tiempo,

b
a

B(t) = B0 t

R

C


B0 ab 
1 − e−t/RC en sentido anti-horario
R
B0 ab −t/RC
e
en sentido horario
b) I(t) =
R
B0 ab −t/RC
c) I(t) =
e
en sentido anti-horario
R

B0 ab 
1 − e−t/RC en sentido horario
d) I(t) =
R
a) I(t) =

e) Ninguna de las anteriores

Consideremos un sistema de coordenadas en que los ejes X e Y apuntan hacia la derecha y arriba,
~ = B(t) k̂. Consideraremos que la
respectivamente. Con ello, el campo magnético tiene la forma B
normal al plano es n̂ = k̂. Por tanto,
¨
~ · n̂ dS = B0 abt
ΦB =
B
espira

Por la ley de Faraday,
E =−

dΦB
= −B0 ab
dt

Por tanto, el circuito posee una fuente de voltaje constante |E| y se trata de un circuito RC con el
condensador inicialmente descargado, cuya ecuación diferencial ha sido tratada anteriormente. Así,
la la corriente viene dada por:
|E| −t/RC
I(t) =
e
R
Para determinar el sentido de la corriente, notemos que el flujo magnético aumenta en el tiempo.
De acuerdo a la ley de Lenz, se inducirá una corriente que se opone al cambio en el flujo. En ese
sentido, se requiere una corriente tal que reduzca el flujo, lo que se traduce en un cambo que entre
en la página. Para que esto ocurra, la corriente debe circular en forma horaria de acuerdo con la
regla de la mano derecha.

---

### Página 133

#### Problema 5.2.
Considere una espira circular de radio r = 0.2 m, masa M = 3 kg y resistencia R = 4π Ω que se mueve
con velocidad ~v = −v(t) k̂, v(t) > 0, en presencia de un campo magnético no uniforme dado por
Bz = 100z T. Suponga que el plano de la espira siempre es perpendicular a la dirección de movimiento.
¿Cuál es la magnitud de la corriente inducida en la espira en t = t0 si la velocidad en dicho instante es
v(t0 ) = 5 m/s?
a) I(t0 ) = 1 A
b) I(t0 ) = 5 A
c) I(t0 ) = 2 A
d) I(t0 ) = 15 A
e) I(t0 ) = 20 A
Pensemos que la normal de la espira apunta en la dirección positiva del eje Z. El flujo magnético
que atraviesa la espira es:
¨
dz
dΦB
~ · n̂ dS = 100πr 2 z
= −100πr 2
ΦB =
B
−→
E =−
dt
dt
espira

En este caso, dz/dt corresponde a la velocidad con la que cae la espira, −v(t). Con ello, la corriente
inducida viene dada por:
I(t0 ) =

100πr 2v(t0 )
100π · 0.04 · 5
|E(t0)|
A = 5A
R
R
4π

#### Problema 5.3.
Considere dos espiras planas circulares concéntricas de radios a y b, respectivamente, con a ≪ b.
Suponga que la inductancia mutua entre ellas es M. ¿Cuál sería la inductancia mutua entre ellas si
tuviesen radios 2a y 2b respectivamente?
a) M/4
b) M/2
c) M
d) 2M
e) 4M

---

### Página 134

Sea M ′ la nueva inductancia mutua. El campo magnético en el centro de una espira de radio R por
la que circula una corriente I es, en módulo,
B(0) =

µ0 I
R2
µ0 I
3/2
2 (R + z )
2R
z=0

Si la espira concéntrica de radio a es pequeña, con a ≪ b, podemos aproximar el flujo del campo a
través de ella por su valor en el origen:
ΦB = πa2 B(0) =

µ0 πIa2
2b

De este modo, la inducatancia mutua original es:
M=

µ0 πa2
2b

Si se duplica el radio de ambas espiras se obtiene:
M′ =

µ0 πa2
µ0 π(2a)2
= 2M
2(2b)
b

#### Problema 5.4.
Considere las dos bobinas de la figura. Suponga que con ellas se hacen los siguientes experimentos
independientes entre sí:
I. El interruptor S está cerrado y se abre
II. El interruptor S está abierto y se cierra
III. Con el interruptor cerrado, A se acerca a B
IV. Con el interruptor cerrado, A de aleja de B

B

A

I

b

S
b

R

V0

---

### Página 135

De los cuatro experimentos anteriores, la corriente I por la resistencia R circulará en el sentido dibujado:
a) Solamente en el experimento III
b) Solamente en el experimento II
c) Solamente en el experimento I
d) En los experimentos I y IV
e) En los experimentos II y III
Con el interruptor cerrado, la espira A crea un campo dirigido a la izquierda (←). Entonces, al
realizar el experimento I inicialmente hay campo y luego este desaparece. Por lo tanto, la bobina B
tiene que crear campo que compense este cambio induciendo un campo magnético hacia la izquierda
(←), por lo que la corriente I circula en contra de lo indicado. En el experimento II es justo al revés;
la espira B tenía flujo cero y para tratar de mantenerlo crea un campo hacia la derecha (→), por
lo que circula una corriente en el sentido adecuado. En el experimento III, para mantener su flujo
constante, crea un campo hacia la derecha (→). En el experimento IV, por la misma razón, se crea
un campo hacia la izquierda (←).

#### Problema 5.5.
Con un alambre de largo d = 2πa se forma una espira circular de radio a cuya autoinductancia resulta
ser L1 . Con un alambre de largo d = 4πa se forma un circuito que consiste en dos vueltas muy juntas
para formar una espira, también de radio a. La autoinductancia L2 de este circuito de dos vueltas es:
a) L2 = L1 /2
b) L2 = L1
c) L2 = 2L1
d) L2 = 4L1
e) L2 = L1 /4
Recordemos que la autoinductancia L se determina mediante el cociente:
ΦB
L=
I
donde ΦB es el flujo magnético total. Si con una vuelta, una corriente I crea campo B, con dos
vueltas idénticas se crea un campo 2B. Ahora el flujo total corresponde al producto del número de
vueltas con el flujo de una espira. En este caso, el flujo individual se duplica, pues el campo total es
2B, y por tanto el flujo total se cuadruplica. La duplicación del campo más la duplicación del flujo
significa que la autoinductancia se cuadruplica y el resultado es:
L2 = 4L1

---

### Página 136

#### Problema 5.6.
La inductancia mutua entre una espira cuadrada de lado a y un alambre recto MUY largo ubicado a
distancia a/2 en el plano de la espira es:

a

a/2

µ0 a
ln (3)
2π
µ0 a
b) M =
ln (2)
2π
µ0 a
c) M =
ln (3/2)
2π
a) M =

d) M =

µ0 a2
ln (3/2)
2π

µ0 a2
ln (1/2)
e) M =
2π
Sea I la corriente que circula por el alambre, el cual consideraremos infinito. Utilizaremos un sistema
coordenado en que ambas figuras se hallan en el plano XY , con el eje Z saliendo de la hoja, y el
alambre coincidente con el eje Y . Así, el campo magnético producido por dicho alambre viene dado
por:
µ0 I
~
B(x)
k̂
2πx
El flujo magnético a través de la espira cuadrada, con normal k̂, es:
ΦB =

¨

~ · n̂ dS =
B

ˆ a ˆ 3a/2

S

a/2

µ0 Ia
µ0 I
dx dy =
ln (3)
2πx
2π

Finalmente, la inductacia mutua corresponde a:
M=

ΦB
µ0 a
ln (3)
I
2π

#### Problema 5.7.
Considere una barra conductora, de largo L, que se mueve con velocidad una ~v = v ı̂ constante, como

---

### Página 137

~
indica la figura. El sistema se encuentra en presencia de un campo magnético B(t)
= −B0 e−λt k̂
apuntando hacia el papel. Si la barra inicialmente (en t = 0) se encontraba en la posición x = 0, el
voltaje inducido es:

L

~
B(t)

~v

x(t)
a) B(t)Lv
b) B(t)Lv(λt − 1)
c)

B(t)Lv
λt − 1

d) B(t)Lvλt
e) Ninguna de las anteriores
Sea x = x(t) la posición de la barra en el instante t, la cual forma una espira de área A = Lx. Así,
el flujo magnético a través de la espira es:
ΦB = BA = B0 Lx e−λt

−→



dΦB
= B0 L ẋ e−λt − xλ e−λt = B0 L(ẋ − xλ) e−λt
dt

Como la rapidez es constante, x(t) = x(0) + vt = vt y ẋ(t) = v. Por tanto,
dΦB
= B0 L(v − vtλ) e−λt = B0 Lv(1 − λt) e−λt = B(t)Lv(1 − λt)
dt
y con ello:
εind = −

dΦB
= B(t)Lv(λt − 1)
dt

#### Problema 5.8.
Considere una barra conductora de largo L, masa m y resistencia R. Dicha barra cae, por acción de
la gravedad, por dos rieles conductores de resistencia despreciable (ver figura) a un rapidez v(t). El
~ apuntando hacia el papel. Con
sistema se encuentra en presencia de un campo magnético uniforme B
estos datos, se puede afirmar que la magnitud de la corriente inducida en el circuito es:

---

### Página 138

~
B

~g

x(t)

L, m
~v (t)

a) BvL
b)

BvL
2R

c) 2BvL
d) 2

BvL
R

e) Ninguna de las anteriores
Coloquemos un sistema coordenado en que el eje X está indicado con la flecha x(t), el eje Z saliendo
del papel y el eje Y paralelo a la barra, de acuerdo a la ley de la mano derecha. De esta forma, el
flujo magnético es:
¨
¨
~ · n̂ dS =
ΦB =
B
− B k̂ · k̂ dS = −BLx
S

S

donde hemos tomado la normal de la superficie hacia fuera del papel. Ahora bien, de acuerdo a la
ley de Faraday–Lenz,
dΦB
= BLv
εind = −
dt
con lo que la corriente posee una magnitud:
I=

|εind |
BLv
R
R

#### Problema 5.9.
Considere la situación descrita en el Problema 5.8. La fuerza neta sobre la barra está dada por:
a) F~ =



(BL)2 v
mg −
R



ı̂

b) F~ = mg ı̂

---

### Página 139

c) F~ =



BLv
mg −
R



ı̂

d) F~ = (mg − (BL)2 v) ı̂
e) Ninguna de las anteriores
Tomando el sistema de coordenadas descrito anteriormente, notamos que el peso de la barra corres~ = mg ı̂. Por otra parte, al existir un campo magnético y una corriente circulante, la
ponde a W
fuerza magnética viene dada por:

~ ×B
~ = −BIL ı̂ = − v(BL) ı̂
F~m = I L
R
~ tiene magnitud L y su dirección coincide con la circulación de la corriente, ̂. Así, la fuerza
donde L
neta corresponde a:


v(BL)
~ + F~m = mg −
ı̂
F~ = W
R

#### Problema 5.10.
Considere el sistema del Problema 5.8. Después de MUCHO tiempo, la barra alcanzará una velocidad
terminal constante cuya magnitud está dada por:
mg − BLR
BL
mgR
b)
BL
a)

mgR − BL/R
BL
mgR
d)
(BL)2
c)

e) Ninguna de las anteriores
La velocidad terminal corresponde a la velocidad que adquiere un móvil cuando la fuerza neta que
actúa sobre él es cero. Por tanto,
mgR
vterminal =
(BL)2

#### Problema 5.11.
Se tiene un alambre recto MUY largo, por el cual fluye una corriente I(t) = I0 cos (ωt). Entonces, la
magnitud del voltaje inducido en la espira (cuyas dimensiones se indican en la figura) es:

---

### Página 140

L
2L/3
L/3
I(t)
µ0 I0 ωL
sin (ωt)
2π
µ0 I0 ωL
b) εind =
ln (2) sin (ωt)
2π
µ0 I0 ωL
ln (3) sin (ωt)
c) εind =
4π
µ0 I0 ωL
d) εind =
ln (2) sin (ωt)
π
µ0 I0 ωL
e) εind =
ln (3) sin (ωt)
2π
a) εind =

Elegimos un sistema de referencia como el sugerido en la figura. Con ello, el campo magnético es
~ = −B(t) k̂ = − µ0 I0 cos (ωt) k̂
B
2πy
Por tanto, el flujo magnético es:
¨
ˆ Lˆ L
µ 0 I0
µ 0 I0 L
~
ΦB =
B · n̂ dS =
cos (ωt) dy dx =
ln (3) cos (ωt)
2π
L/3 2πy
S

donde la normal de la espira se tomó saliendo del papel, i.e. n̂ = −k̂. Con ello, el voltaje inducido
viene dado por:
µ0 I0 ωL
dΦB
ln (3) sin (ωt)
εind = −
dt
2π

#### Problema 5.12.
Una bobina circular de N vueltas y radio R es ubicada sobre un campo magnético externo. El campo
es oscilatorio, y su magnitud viene dada por:

r 
cos (ωt)
B(r, t) = B0 1 −
2R
donde r es la dirección radial medida desde es centro de la bobina. Si el campo es dirigido perpendicularmente al plano de la bobina, ¿cuál es el voltaje inducido en ella?

---

### Página 141

r

~ t)
B(r,
a)

πωNR2 B0 sin (ωt)

b) ωNR2 B0 sin (ωt)

r 
c) NB0 1 −
ωR2 sin (ωt)
2R

r 
d) NB0 1 −
ωR2 cos (ωt)
2R
e) πωNR2 B0 sin (ωt)
En este caso, el flujo magnético total está dado por:
ˆ 2π ˆ R 
r 
ΦB = NB0 cos (ωt)
dr dθ = πNR2 B0 cos (ωt)
r 1−
2R
Por tanto, el voltaje inducido es:
εind = −

dΦB
= πωNR2 B0 sin (ωt)
dt

#### Problema 5.13.
Se tienen dos bobinas largas, de largos L1 y L2 (L2 < L1 ) y áreas transversales A1 y A2 (A2 < A1 ),
ubicadas como muestra la figura. Notar que ambas bobinas NO están conectadas directamente. La
bobina 1 está conectada a una fuente de corriente I(t) = I0 cos (ωt). La bobina 2, que está al interior
de la bobina 1, se conecta a un voltímetro V . Si las bobinas tienen N1 y N2 vueltas, respectivamente,
¿cuál es el voltaje, en función del tiempo, medido por V ?

---

### Página 142

V

I(t)

a) V =

µ0 A2 N1 I0 ω
sin (ωt)
L1

b) V =

µ0 A2 N1 N2 I0 ω
sin (ωt)
L1

c) V = −

µ0 A2 N1 N2 I0
cos (ωt)
L1

d) V = −

µ0 A2 N1 I0
cos (ωt)
L1

e) V =

µ0 A1 N1 N2 I0 ω
sin (ωt)
L1

El campo magnético al interior de la bobina 1 está dado por:
~ 1 = N1 µ0 I(t) ı̂
B
L1
Así, el flujo total a través de la bobina 2 es:
Φ2 =
Con ello,
V =

N1 N2 µ0 A2
I(t)
L1

µ0 A2 N1 N2 I0 ω
sin (ωt)
L1

#### Problema 5.14.
Dos rieles horizontales y paralelos, separados por una distancia ℓ, están conectados por una resistencia
R como se muestra en la figura. Suponga que cada uno de los rieles tiene una resistencia λ por unidad
de largo. Una barra metálica, ab, de resistencia despreciable se puede deslizar sin fricción sobre los
~ uniforme, perpendicular al plano, que apunta hacia
dos rieles. Existe, además, un campo magnético B
adentro. Suponga que la barra se mueve hacia la derecha con una velocidad v(t) de tal forma que la
corriente I en el circuito permanece constante en el tiempo.

---

### Página 143

a

~v (t)

~
B

R

ℓ

b
x(t)
¿Cuál es la magnitud y dirección de la corriente inducida en la barra?
a) I =

Bℓv
en dirección de b hacia a
2λx

b) I =

RBℓv
en dirección de b hacia a
2λx

c) I =

Bℓv
en dirección de a hacia b
2λx

d) I =

Bℓv
en dirección de b hacia a
2λx + R

e) I =

Bℓv
en dirección de a hacia b
2λx + R

Supongamos un sistema coordenado en que el eje X, indicado por x(t), coincide con la figura, y el
~ = −B k̂. Para la espira, podemos
eje Z sale de la hoja. Así, el campo magnético tiene por forma B
elegir dos direcciones de la normal. Recuerde que la dirección, de acuerdo a la regla de la mano
derecha, indica la dirección en que la corriente es positiva. En este caso, elijamos como normal
n̂ = k̂, que indica que la corriente positiva circula desde b hacia a. Con ello,
ΦB = −Bℓx(t)

−→

εind = −

dΦB
= Bℓv
dt

Ahora bien, la resistencia total del circuito viene dada por la resistencia R y la porción de los dos
rieles, 2λx. Por tanto,
εind
Bℓv
I=
>0
Rtotal
R + 2λx
Como la corriente nos dio positiva, significa que va recorrida desde b hacia a.

#### Problema 5.15.
Considere la situación descrita en el Problema 5.14. ¿Cuál es la aceleración de la barra, en función de
la distancia x? Aquí, a es la aceleración de la barra.

---

### Página 144

a) a =

2I 2 λ(R + 2λx)
B 2 ℓ2

b) a =

2Iλ(R + 2λx)
B 2 ℓ2

c) a =

2I 2 λ
B 2 ℓ2

d) a =

2I 2 λ(R + λx)
B 2 ℓ2

e) a =

2Iλ(R + λx)
B 2 ℓ2

Como la corriente es constante en el tiempo, significa que:
I=

Bℓv
R + 2λx

−→

IR + 2λIx = Bℓv

Derivando con respecto al tiempo, y recordando que ẋ = v y v̇ = a,
2λIv = Bℓv̇

−→

a=

2λIv
Bℓ

Como queremos que el resultado dependa de x y no de v, reemplazamos:
a=

2λI I(R + 2λx)
2λI 2 (R + 2λx)
2λI
v=
Bℓ
Bℓ
Bℓ
B 2 ℓ2

#### Problema 5.16.
Considere la situación descrita en el Problema 5.14. ¿Cuál es la potencia disipada en el circuito? Aquí,
a es la aceleración de la barra.
a) P =

aB 2 ℓ2
λ

aB 2 ℓ2
b) P =
2λ
c) P =

aB 2 ℓ2
2λℓ + R

d) P =

aB 2 ℓ3
2λ

e) P =

aB 2 ℓ3
λ

---

### Página 145

Recordemos que la potencia disipada por una resistencia es:
P = I 2 Rtotal = I 2 (R + 2λx) = I 2

Bℓv
= BIℓv
I

De la ecuación que relaciona la aceleración con la velocidad,
Bℓa
aB 2 ℓ2
P = BIℓv = BIℓ
2λI
2λ

#### Problema 5.17.
Un conductor sólido de radio a, está separado por un material aislante de un conductor delgado de
radio b, de modo tal que forma un cable coaxial. Los dos conductores son MUY largos y conducen una
corriente I en direcciones opuestas. La autoinductancia por unidad de largo del cable coaxial es:

r

b

b

 
b
a
 
b
µ0
ln
b)
4π
a
 
µ0
b
c)
ln
3π
a
 
b
µ0
ln
d)
π
a
µ0
a)
ln
2π

e) Ninguna de las anteriores
Tomaremos una circunferencia de radio r > a en torno al conductor interior. Por simetría, el campo
magnético satisface:
µ0 I
2πr B = µ0 I −→ B =
2πr

---

### Página 146

Para calcular el flujo magnético, tomaremos una sección transversal (coincidente con un radio) de
largo ℓ. Así,
 
ˆ ℓˆ b
µ0 Iℓ
b
µ0 I
dr dℓ =
ln
ΦB =
2π
a
a 2πr
Con ello,
ΦB
µ0 ℓ
L=
ln
I
2π

 
b
a

−→

L
µ0
ln
ℓ
2π

 
b
a

#### Problema 5.18.
El inductor de la figura tiene autoinductancia L = 0.26 H y lleva una corriente en la dirección indicada.
Esta corriente decrece uniformemente en el tiempo, con I˙ = −0.018 A/s. Entonces, el voltaje inducido
Vab = Va − Vb es:

I
(a)

L

(b)

a) 5.12 mV, Vb > Va
b) 4.68 mV, Va > Vb
c) 7.52 mV, Va > Vb
d) 8.12 mV, Va > Vb
e) Ninguna de las anteriores
El voltaje en una inductancia viene dado por:
Vba = LI˙ = −4.68 mV
puesto que se calcula en la dirección en que circula la corriente. Así, Va > Vb .

---

### Página 147

Circuitos de corriente alterna y campos variables en el tiempo

Ecuaciones de Maxwell en uno de los muros exteriores de la Universidad de Varsovia

---

### Página 148

#### Problema 6.1.
Considere el circuito de la figura con una corriente alterna de frecuencia angular ω. El valor de la razón
|V̂out /V̂in | de los respectivos fasores es:

Vin

C

R

L
Vout

a)

s

b)

s

c)

s

d)

s

e)

s

(ωL)2

1 2
+ R2
ωL − ωC
R2

1 2

ωL − ωC

+ R2

(ωL)2 + R2

1 2
ωL − ωC
+ R2
(ωL)2 − R2

1 2
+ R2
ωL − ωC
(ωLR)2

1 2
ωL − ωC
+ R2

La impedancia equivalente Z del circuito es:
+ i ωL + R = |Z| ei θ1 ,
Z=
i ωC

|Z| =

s

R2 +

2

ωL −
ωC

y la fase θ1 no nos interesa por el momento. Por la ley de Ohm, el fasor de corriente que circula por
el circuito es:
V̂in
Iˆ =
Z
Así, el voltaje de salida viene dado por:
p
V̂out = (i ωL + R)Iˆ = (ωL)2 + R2 ei θ2 Iˆ =

s

(ωL)2 + R2
ei(θ2 −θ1 ) V̂in

1 2
ωL − ωC + R

---

### Página 149

Dividiendo y aplicando módulo, finalmente tenemos:
s
(ωL)2 + R2
V̂out

1 2
V̂in
ωL − ωC
+ R2

#### Problema 6.2.
Un inductor, un condensador, una resistencia y una fuente de poder de corriente alterna se conectan
en serie. Si se doblan los valores de la capacidad, la inductancia y la resistencia, ¿qué ocurre con la
frecuencia de resonancia?
a) Se duplica
b) Se cuadruplica
c) Se reduce a la mitad
d) Se reduce a un cuarto
e) Ninguna de las anteriores
Recordemos que la frecuencia de resonancia viene dada por:
ωr = √
Así,
ωr ′ = √

LC

ωr
1 1
= √
2 LC
2L · 2C

#### Problema 6.3.
La diferencia de fase, en grados, entre la corriente y el voltaje de la fuente de poder en la figura es:

L = 0.5H
C = 1.25uF

V0 = 200V
ω = 1000rad/s

R = 400Ω
a) 60.2◦

---

### Página 150

b) 40.1◦
c) 36.9◦
d) 25.3◦
e) 12.3◦
La impedancia equivalente viene dada por:
Z = i ωL +
donde
tan θ =

+ R = |Z| ei θ
i ωC

ωC = − 3
R

ωL −

−→

θ = −36.9◦

Por la ley de Ohm,
V̂
V0 −i θ
Iˆ =
e
Z
|Z|
Con ello,
I(t) = Re{Î} =

V0
cos (ωt − θ)
|Z|

y el desfase entre corriente y voltaje es de |θ| = 36.9◦ , que era lo buscado.

#### Problema 6.4.
~ = E0 sin (kx − ωt) ̂, donde E0 , k, ω son
En una región del espacio hay un campo eléctrico dado por E
constantes. En el plano XZ de esa región, se escoge un camino rectangular C, de lados a y b, que
intersecta al eje X en los puntos x1 y x2 (ver figura). Calcule la circulación del campo magnético a lo
largo del camino C, i.e.
˛
~ · d~r
B
C

---

### Página 151

z

C

b/2

y

x1

x2

x

−b/2
a

h
i
a) µ0 ε0 ωE0 abk sin (kx2 − ωt) − sin (kx1 − ωt)
b)

i
µ0 ε0 ωE0 b h
sin (kx2 − ωt) − sin (kx1 − ωt)
k

c)

µ0 ε0 ωE0 ab
sin (k[x2 − x1 ] − ωt)
k(a + b)

d)

µ0 ε0 ωE0 (a + b)
sin (k[x2 − x1 ] − ωt)
k

e)

µ0 ε0 ωE0
sin (k[x2 − x1 ] − ωt)
kab

De las ecuaciones de Maxwell, se sabe que la ley de Ampère generalizada sin una corriente externa
viene dada por:


˛
¨
~ · d~r = µ0 ε0 d  E
~ · n̂ dS 
B
dt
C

S

con una superficie S tal que ∂S = C. En este caso, tomaremos por S el interior del rectángulo
limitado por C. Por la regla de la mano derecha, la normal de la superficie debe salir de la hoja,
con lo que n̂ = −̂. Así,
¨

~ · n̂ dS = −
E

ˆ b/2 ˆ x2
−b/2

S

Con ello,
˛
C

x1

E0 sin (kx − ωt) dx dz = −

i
E0 b h
cos (kx1 − ωt) − cos (kx2 − ωt)
k

i
µ0 ε0 ωE0 b h
~
sin (kx2 − ωt) − sin (kx1 − ωt)
B · d~r =
k

---

### Página 152

#### Problema 6.5.
Un circuito contiene dos resistencias R, dos inductancias L y una capacitancia C. Estos elementos están
conectados a una fuente de voltaje alterna V (t) = V0 cos(ωt), como en la figura.

R

C

L
VL

V

L

R

¿Cuál es la amplitud I0 de la corriente alterna que provee la fuente?
"
 2
2 #1/2
V0
ω LC − 1
a) I0 =
1+
2R
ωRC
b) I0 =

V0
2R

"
 2
2 #−1/2
ω LC − 12
V0
1+
c) I0 =
2R
ωRC

 2
−1/2
ω LC − 12
V0
d) I0 =
1+
2R
ωRC

 2
−1/2
ω LC − 1
V0
1+
e) I0 =
2R
ωRC
En este circuito, la impedancia equivalente Z viene dada por:


Z = 2R + i 2ωL −
= |Z| ei ϕ
ωC
donde
"



|Z| = (2R)2 + 2ωL −
ωC


2ωL −

ωC 
ϕ = arctan 

2R

Por la ley de Ohm, la corriente que circula es:

V̂
V̂ −i ϕ
Iˆ =
e
Z
|Z|

2 #1/2

---

### Página 153

En el dominio del tiempo,
I(t) =

V0
cos (ωt − ϕ)
|Z|

de modo que la amplitud I0 = V0 /|Z| se puede escribir como:
"
 2
2 #−1/2
ω LC − 12
V0
I0 =
1+
2R
ωRC

#### Problema 6.6.
En el circuito de Problema 6.5, ¿cuál es la frecuencia de resonancia ω0 para la cual la amplitud de la
corriente es máxima?
a) ω0 = √

LC

b) ω0 = √
2 LC
LC
r
d) ω0 =
LC
c) ω0 = √

e) ω0 = √

2LC

La amplitud de la corriente es máxima cuando el módulo de la impedancia equivalente, |Z|, es
mínimo. Esto ocurre cuando la parte imaginaria de la impedancia equivalente se anula:
2ω0 L −

=0
ω0 C

−→

ω0 = √

2LC

#### Problema 6.7.
En el circuito de Problema 6.5, ¿cuál es la amplitud VL del voltaje alterno VL (t)?
a) VL = V0

ωL
2R

b) VL = V0

ωL
2ωL − ωC

---

### Página 154

ωL

c) VL = V0 q

4R2 + ωL − ωC

d) VL = V0 q

4R2 + 2ωL − ωC

e) VL = V0 q

R2 + ωL − ωC

ωL

2

ωL

2

2

La diferencia de potencial pedida corresponde al voltaje en la inductancia, el cual se calcula de la
siguiente forma:
VL (t) = L

dI
= −LωI0 sin (ωt − ϕ) = LI0 ω sin (ωt − ϕ − π)
dt

donde hemos utilizado que − sin (x) = sin (x − π). Con ello, la amplitud del voltaje viene dada por:
VL =

V0 Lω
= V0 q
|Z|

ωL
4R2 + 2ωL − ωC

2

#### Problema 6.8.
En el circuito de Problema 6.5, si la frecuencia ω de la fuente coincide con la frecuencia de resonancia
ω0 , i.e. ω = ω0 , ¿cuál es la potencia promedio P que entrega la fuente?
a) P =

V0 2
2R

b) P =

V0 2
4R

c) P = 0 W
d) P = −
e) P =

V0 2
4R

V0 2
8R

La potencia instantánea del circuito viene dada por:
P(t) = V (t)I(t) = V0 I0 cos (ωt) cos (ωt − ϕ)

---

### Página 155

En la frecuencia de resonancia, ω = ω0 , la parte imaginaria de la impedancia equivalente es nula,
por lo que la fase y la amplitud de la corriente satisfaces que:
ϕ

∧

I0

P(t) = V0 I0 cos2 (ωt)

−→

ω=ω0

=0

V0
2R

P =

V 0 I0

ω=ω0

Así,

Reemplazando,
P =

V0 2
4R
