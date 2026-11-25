---
title: "Problemas de Electromagnetismo - Sebastián Urrutia"
source_pdf: "Electro/material-apoyo/compilados/Problemas de Electromagnetismo - Sebastián Urrutia.pdf"
pages: 153
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Problemas de Electromagnetismo - Sebastián Urrutia

### Página 1

Electricidad y
Magnetismo
Compilado de problemas resueltos

Sebastián Urrutia Quiroga
surrutiaquir@gmail.com
www.surrutiaquir.cl

Tercera Edición – Junio de 2017

---

### Página 2

Disponible en línea: http://www.surrutiaquir.cl/
Sebastián Urrutia Quiroga
Contacto: surrutiaquir at gmail.com
Se autoriza la reproducción total o parcial, con fines académicos, por cualquier medio o procedimiento,
incluyendo la cita bibliográfica que acredita al trabajo y a su autor.
Prohibida su Comercialización

---

### Página 3

Índice
1. Electrostática

1.1. Integrales de Coulomb: fuerza y campo eléctrico . . . . . . . . . . . . . . . . . . . . . .

1.2. Ley de Gauss para el campo eléctrico . . . . . . . . . . . . . . . . . . . . . . . . . . . .

1.3. Potencial eléctrico . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

1.4. Energía potencial electrostática . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

1.5. Conductores y capacitancias . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

2. Electricidad en medios materiales

2.1. Ecuaciones de Laplace y Poisson . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

2.2. Dieléctricos . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

2.3. Corriente eléctrica y ley de Ohm microscópica . . . . . . . . . . . . . . . . . . . . . . .

2.4. Ley de Ohm macroscópica: circuitos fem/R . . . . . . . . . . . . . . . . . . . . . . . . .

2.5. Circuitos RC . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

3. Magnetostática
3.1. Fuerza de Lorentz y torque sobre una espira . . . . . . . . . . . . . . . . . . . . . . . .

3.2. Ley de Biot-Savart . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 101
3.3. Ley de Ampère . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 109
4. Campos variables en el tiempo

4.1. Ley de inducción de Faraday-Lenz . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 118
4.2. Inductancia. Circuitos RL, LC y RLC . . . . . . . . . . . . . . . . . . . . . . . . . . . . 127
4.3. Corriente Alterna . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 136
5. Ecuaciones de Maxwell

5.1. Introducción a la teoría electromagnética . . . . . . . . . . . . . . . . . . . . . . . . . . 144

---

### Página 4

1.

Electrostática

1.1.

Integrales de Coulomb: fuerza y campo eléctrico

(1) Considere la distribución de cargas puntuales de la figura:
b

P

r

−q

+2q
b

b

d

b

−q

d

a) Calcule el campo eléctrico en P
b) Evalué el caso límite r ≫ d, ¿cómo varía la magnitud del campo eléctrico con la distancia en
este caso?
a) El campo eléctrico en P puede ser obtenido utilizando el Principio de Superposición. El campo
eléctrico producido por +2q es simplemente:
~1 =
E

1 2q
̂
4πǫ0 r 2

~ = −d ı̂, entonces el campo producido por la carga de la derecha es:
Si hacemos ~r = r ̂ y R
~
~r − R
r ̂ + d ı̂
q
~2 = − q
E
=−
~ 3
4πǫ0 k~r − Rk
4πǫ0 (r 2 + d2 )3/2
De manera análoga, por simetría, el campo producido por la carga de la izquierda es:
r ̂ − d ı̂
~3 = − q
E
4πǫ0 (r 2 + d2 )3/2
~ P viene dado por:
Así, el campo total E
~P =
E

X
j=1

~j =
E

q
2qr ̂
1 2q
̂ −
3/2
4πǫ0 r
4πǫ0 (r + d )
2πǫ0



r
− 2
r
(r + d2 )3/2



̂

---

### Página 5

b) Para analizar el límite r ≫ d, reescribimos el campo de la siguiente manera:

 2 !−3/2 
d


+
1

r
q


~P =
E
 2−
 ̂

2πǫ0  r
r2


Ahora, utilizando la expansión de Taylor a primer orden

n
1 + ε ≈ 1 + nε , ε ≪ 1

se tiene que:

 2 !−3/2
d
3 d2
1+
≈1−
r
2 r2

Entonces,
~P ≈
E
y por tanto:

q
2πǫ0



3 d2
−
+
r 2 r 2 2r 2 r 2



̂

~ (r≫d) = 3qd ̂
E
P
4πǫ0 r 4

Notar que, para grandes distancias (r ≫ d), esta distribución de carga genera un campo que
decae como 4 , lo que contrasta con el campo de una carga puntual que decae según 2 .
r
r
(2) Dos pequeñas esferas conductoras, de igual masa m y carga q > 0, cuelgan por dos hilos no
conductores sin masa y de largo ℓ. Cada esfera forma un ángulo θ con el eje vertical, como se
muestra en la figura.

b

ℓ

θ θ

+

ℓ

+

r
a) Calcule el valor de la carga q para el equilibrio estático del problema.
b) Suponiendo que las esferas pierden carga a razón λ > 0 C/s, ¿con qué velocidad angular se
acerca una a la otra, para θ ≪ 1?

---

### Página 6

a) Debido a la simetría del sistema, bastará con hacer análisis de fuerzas para una de las cargas.
Consideramos el equilibrio entre las tres fuerzas que actúan: la fuerza de repulsión electrostática
Fe , la tensión sobre el hilo T , y la fuerza de gravedad mg:
X
Fx = 0 −→ T sin θ − Fe = 0
X
Fy = 0 −→ T cos θ − mg = 0
La primera ecuación equivale a
q2
T sin θ = k 2
r

r 2 T sin θ
q =
k

De la segunda ecuación,
T =
Por tanto, y como r = 2ℓ sin θ,
q = 2ℓ sin θ

q = ±r

r

T sin θ
k

mg
cos θ
r

mg tan θ
k

b) Para ángulos pequeños, sin θ ≈ tan θ ≈ θ. Del enunciado, q̇ = −λ pues pierde carga. Así,
r
mg
3/2
q = αθ , α = 2ℓ
k
Derivando con respecto al tiempo,
dq
∂  3/2  dθ
3α √
θ θ̇
αθ
= q̇ =
dt
∂θ
dt

θ̇ = −

2λ
√
3α θ

Finalmente, la velocidad angular de la esfera a la izquierda será:
ω
~ 1 = − θ̇ k̂
Y la de la esfera derecha:
~ω2 = + θ̇ k̂ = −~ω1
(3) Determine el campo eléctrico generado por un alambre infinito con densidad de carga uniforme,
localizado en el eje z.
Consideremos la siguiente situación, en donde λ representa la densidad lineal de carga:

---

### Página 7

~ = z k̂
R

~r

z0 k̂
y

ρρ̂
x

en donde

~ = z k̂, −∞ < z < ∞
R

dR = dz

~r = z0 k̂ + ρ ρ̂

~ = (z0 − z) k̂ + ρ ρ̂
~r − R
Así,
λ
4πε0

~ r) =
E(~

ˆ ∞

h
i1/2
~ = (z0 − z)2 + ρ2
∴ k~r − Rk




ρ
(z0 − z)


h
i3/2 k̂ + h
i3/2 ρ̂ dz
−∞
(z0 − z)2 + ρ2
(z0 − z)2 + ρ2

= Ez k̂ + Eρ ρ̂
con
Ez

Eρ =

ˆ ∞
(z0 − z)
λ
dz
u = z0 − z
4πε0 −∞ [(z0 − z)2 + ρ2 ]3/2
ˆ ∞
λ
u du
(la función es impar)
4πε0 −∞ [u + ρ2 ]3/2
= 0

ˆ ∞
ρ
λ
dz
u = z − z0
4πε0 −∞ [(z0 − z)2 + ρ2 ]3/2
ˆ ∞
λ
ρ du
u = ρ tan θ, du = ρ sec2 θdθ
3/2
4πε0 −∞ [u + ρ ]
ˆ π/2
ρ2 sec2 θ dθ
λ
4πε0 −π/2 [ρ2 (1 + tan2 θ)]3/2
ˆ
ˆ
λ 1 π/2
λ 1 π/2 ρ2 sec2 θ dθ
cos θ dθ
4πε0 ρ −π/2
sec3 θ
4πε0 ρ −π/2
λ 2
4πε0 ρ

---

### Página 8

Resumiendo,
~ r) =
E(~

λ ρ̂
2πε0 ρ

(4) Encuentre el campo eléctrico a una distancia z sobre el centro de un disco circular plano de radio
R, el cual posee una densidad de carga superficial σ constante. ¿Qué pasa con su fórmula en el caso
en que R → ∞? Revise también el caso en que z ≫ R.
Sean: ~r = z k̂ ,

~ = ρ ρ̂. Así,
R

~ = z k̂ − ρ ρ̂
(∗) ~r − R
p
~ = z 2 + ρ2
(∗) k~r − Rk
(∗) dS = ρ dρ dθ

Así,
~
~r − R
dS
~ 3
|~r − R|
ˆ 2π ˆ R
z k̂ − ρ ρ̂
σ
ρ dρ dθ
2 3/2
4πǫ0 0
0 (z + ρ )
~z + E
~ρ
= E

~ r) =
E(~
4πǫ0

¨

σ

Ya sea mediante el cálculo explícito de la integral, o por argumentos de simetría del problema, se
concluye que:
~ ρ ≡ ~0
E
Por otra parte, dado que el vector unitario en la dirección Z es constante, puede salir de la integral:
~ z = Ez k̂, donde
E
ˆ 2π ˆ R
σz
ρ dρ dθ
Ez =
2 3/2
4πǫ0 0
0 (z + ρ )
ˆ R
σz
ρ
dρ
2ǫ0 0 (z + ρ2 )3/2


σz
−√
2ǫ0 |z|
z 2 + R2
Por lo tanto,
σz
~
E(z)
2ǫ0



−√
|z|
z + R2



k̂

Notemos que, si R → ∞, entonces el disco cubrirá todo el plano; por esta razón, el campo eléctrico
de un plano infinito con carga superficial constante es:
Eplano = lím E(z) = ±
R→∞

σ
2ǫ0

---

### Página 9

y en constante, con signo dependiente de si estamos sobre (+) o bajo (−) el plano.
Para z ≫ R > 0, entonces:
√
z
z +R
Con ello,
Ez≫R =



R2
1+ 2
z

−1/2

≈
z



1 R2
1−
2 z2

πR2 σ
1 Q
σz R2
2ǫ0 2z
4πǫ0 z
4πǫ0 z 2

con Q = σπR2 la carga total del disco.

(5) Considere un plano infinito de densidad de carga uniforme σ, con un orificio circular de radio R:
a) Obtenga el campo eléctrico sobre un punto arbitrario del eje –perpendicular al plano– que
pasa por el centro del orificio.
b) Suponga que ahora, a lo largo de este eje, se ubica un hilo no conductor de largo ℓ con densidad
de carga lineal uniforme λ desde z = 0 hasta z = ℓ, con z es la distancia perpendicular al
plano. Encuentre la fuerza eléctrica entre ambos objetos.

a) Para resolver este problema, usamos el Principio de Superposición: el campo eléctrico de la figura
corresponde a la suma de los campos producidos por un plano infinito (con densidad de carga
σ) y un disco de radio R (con densidad de carga −σ). Supongamos que el plano agujereado
se encuentra en el XY ; así, el problema consiste en obtener el campo sobre un punto del eje
z. Del problema anterior, estos campos son conocidos, por lo que:


σ
z
z
z
σ
σ z
~
~
~
√
k̂ −
−√
k̂
k̂ =
E(z) = Eplano + Edisco =
2ǫ0 |z|
2ǫ0 |z|
2ǫ0 z + R2
z +R
b) Por la tercera Tercera Ley de Newton, podemos calcular la fuerza entre ambos elementos como
la fuerza ejercida por el plano agujereado sobre la barra. El elemento de fuerza eléctrica que
el plano ejerce sobre un elemento dq = λ dz del alambre es:
~
~
dF~ = E(z)
dq = λE(z)
dz =

σλ z dz
√
k̂
2ǫ0 z 2 + R2

---

### Página 10

Por tanto, la fuerza sobre el hilo completo es:
ˆ ℓ
F~ =
dF~

σλ
2ǫ0

ˆ ℓ

z dz
√
z 2 + R2
ℓ



k̂

σλ √ 2
z + R2 k̂
2ǫ0

σλ √ 2
ℓ + R2 − R k̂
2ǫ0
(6) Un recipiente hemisférico no conductor, de radio interior a, tiene una carga total Q repartida
uniformemente en su superficie. Encuentre el campo eléctrico en el centro de curvatura.

Tomamos como origen el centro de curvatura de la semiesfera. A partir de esto, podemos determinar
la contribución de un elemento diferencial de carga en la superficie al campo eléctrico en el eje que
~ por simetría, solo
pasa por el centro de curvatura, que coincide con la dirección k̂ (El campo E,
tendrá componente en k̂).
~
~r − R
~ = 1
dE
σdS
~ 3
4πǫ0 k~r − Rk
Un elemento diferencial de superficie sobre la esfera está dado por
dS = a2 sin θ dθ dφ
y, como la carga está uniformemente distribuida, la densidad superficial es simplemente
σ=

Q
2πa2

Con esto, podemos determinar el campo total integrando sobre toda la superficie:
~ r) = a
E(~
4πǫ0

ˆ 2π ˆ π

π/2

sin θ

~
Q ~r − R
dθ dφ
~ 3
2πa2 k~r − Rk

---

### Página 11

Evaluando en ~r = ~0 obtenemos el campo en el centro de curvatura:
ˆ 2π ˆ π

~C = − Q
E
8π 2 ǫ0

sin θ

π/2

~
R
dθ dφ
~ 3
kRk

~ = a ρ̂ = a cos θ k̂ + a sin θ cos φ ı̂ + a sin θ sin φ ̂, entonces |R|
~ = a. Por el argumento
Si tomamos R
de simetría, solo interesa la componente según k̂. De todas formas, se puede verificar calculando
explícitamente las integrales en ı̂, ̂. Con esto,
ˆ π
ˆ π
Q
Q
Q
EC = −
cos
θ
sin
θ
dθ
−
sin
2θ
dθ
4πǫ0 a2 π/2
8πǫ0 a2 π/2
8πǫ0 a2
{z
}
|
= −1

Finalmente,

~ C = EC k̂ =
E

Q
k̂
8πǫ0 a2

1.2.

Ley de Gauss para el campo eléctrico

(1) Considerando la ley de Gauss,
~ · n̂ dS = q
E
ε0

¨
S

~ de una esfera cargada
con q la carga encerrada por la superficie S, determine el campo eléctrico E
uniformemente, de carga Q y radio a.
Primero que todo, calculemos la densidad volumétrica de carga para la esfera:
ρ(r) =

Q
3Q
Q
4 3
V
4πa3
πa

~ = E(r) r̂. Como superficies gaussianas, tomaremos esferas de radio
Por simetría, proponemos que E
r con normal exterior n̂ = r̂. Así,
¨
¨
qenc
~
E · n̂ dS =
E(r)r̂ · r̂ dS = E(r) A(S) = 4πr 2 E(r) =
ε0
S

S

Para calcular la carga encerrada, distinguimos dos casos:
r>a
qenc = Q

E(r) =

Q
4πε0 r 2

---

### Página 12

r<a

 r 3
qenc = ρ(r) · πr 3 = Q
a

E(r) =

Q
r
4πε0 a3

Notar que es continua en r = a. Así, el campo eléctrico tiene la siguiente forma:
E(r)
Q
4πε0 a2

∝r
∝

r2
r

r=a
con:
~
E(r)


Qr


ρ̂ , si r < a

 4πǫ0 a3





Q
ρ̂ , si r ≥ a
4πǫ0 r 2

[Propuesto] Compare este resultado con el cálculo hecho mediante integrales de Coulomb.

(2) Considere un cable coaxial muy largo, compuesto por un cilindro sólido interior –de radio a– que lleva
una densidad de carga volumétrica ρ (constante), y por un cilindro exterior hueco –de radio b > a–
que lleva una densidad de carga superficial σ; esta densidad es tal que hace al cable eléctricamente
neutro. Encuentre el campo eléctrico producido por el cable en todo el espacio.

Establecemos un sistema de coordenadas cilíndricas en el centro del cable. Distinguimos tres regiones:
(i) r > b

(ii) a < r < b

(iii) 0 ≤ r < a

Por simetría, el campo (de existir) debe ser radial, y su magnitud únicamente función del radio
(pues el cable posee una simetría azimutal, i.e. es invariante ante una rotación del ángulo polar).

---

### Página 13

r>b
Dada la simetría, usaremos como superficie gaussiana un cilindro de radio r < b y altura h.
Luego,
¨
¨
¨
~
~
~ · n̂ dS
E · n̂ dS =
E · n̂ dS +
E
S

M anto

T apas

~ = E(r) ρ̂; de esta forma:
Para el manto, n̂ = ρ̂ y E
¨
¨
~
E · n̂ dS = E(r)
dS = 2πrhE(r)
M anto

M anto

~ ⊥ n̂ y por tanto:
Por otro lado, para las tapas, n̂ = ± k̂. De esta forma, E
¨
~ · n̂ dS = 0
E
T apas

Con esto,
Φe = E(r)2πrh
pero como el cable es neutro, qenc = 0. Luego,
E(r)2πrh = 0

E(r) = 0

Notar que: qenc = πa2 hρ + σ2πbh = 0 −→ σ = −

ρa2
2b

a<r<b
Nuevamente utilizaremos como superficie gaussiana un cilindro de radio r y altura h. Por los
mismos argumentos anteriores, la integral de flujo eléctrico se reduce a:
Φe = E(r)2πrh
La carga encerrada en este caso corresponde qenc = ρVa , con Va = πa2 h el volumen del cilindro
sólido interior. Así,
a2 ρ
πa2 h
−→ E(r) =
E(r)2πrh = ρ
ǫ0
2ǫ0 r

0≤r<a
Escogemos la misma superficie gaussiana. Los mismos argumentos de simetría son válidos en
esta región, y por tanto:
Φe = E(r)2πrh , qenc = ρπr 2 h

---

### Página 14

Entonces,
E(r)2πrh = ρ

πr 2 h
ǫ0

E(r) =

ρr
2ǫ0

En resumen (notando que existe una discontinuidad en el campo al atravesar la superficie cargada
r = b),
 ρr

ρ̂ , si 0 ≤ r < a


2ǫ0





a2 ρ
~
E(r) =
ρ̂ , si a < r < b


2ǫ
r





 ~
, si b < r

(3) Considere dos esferas no concéntricas de radio R. La primera de ellas lleva una densidad volumétrica
de carga ρ y la segunda −ρ. Los centros de las esferas están a distancia d < 2R. Si d~ es el vector
que va del centro de la esfera positiva al centro de la negativa, demuestre que el campo eléctrico en
la intersección de las esferas es constante, y encuentre su valor.

b

b

d~

Este problema se resuelve con superposición, recordando antes la fórmula del campo eléctrico generado por una distribución homogénea y esférica de carga (resuelto anteriormente):

Qr


ρ̂ , si r < a

 4πǫ0 a3
~
E(r)


Q


ρ̂ , si r ≥ a
4πǫ0 r 2

donde r es la distancia al centro de la distribución. Ahora, sea P un punto arbitrario dentro de la
región de intersección:

---

### Página 15

P
b

~r ′

~r

ρ
b

b

d~

−ρ

El campo en P producido por la distribución de carga positiva es
~ 1 = ρ ~r
E
3ǫ0
y el de la distribución negativa viene dada por
~ 2 = −ρ ~r ′
E
3ǫ0
Así, por el principio de superposición, el campo eléctrico en P está dado por
~ )=E
~1 + E
~ 2 = ρ ~r − ρ ~r ′
E(P
3ǫ0
3ǫ0
~
Pero d~ + ~r ′ = ~r, de forma que ~r ′ = ~r − d:



~ ) = ρ ~r − ρ ~r − d~ = ρ d~
E(P
3ǫ0
3ǫ0
3ǫ0

El punto P fue escogido arbitrariamente; luego, para todo ~x dentro de la intersección, el campo es
uniforme y está dado por
~ x) = ρ d~
E(~
3ǫ0
Notar que el campo es paralelo a la dirección que une ambos centros
(4) Considere la siguiente distribución volumétrica de carga en coordenadas esféricas
ρ(r) =

k
,
r2

a≤r≤b

Encuentre el campo eléctrico en todo el espacio.
Dado que no existe dirección privilegiada para la densidad de carga, el problema presenta simetría
~ = E(r) ρ̂.
esférica. Por esta razón, es posible argumentar que el campo en cuestión posee la forma E
Ahora, nuestro problema separa al espacio en tres regiones:

---

### Página 16

r<a
Si empleamos una esfera de radio r como superficie gaussiana, entonces la ley de Gauss nos
señala que
¨
~ · n̂ dS = E(r)A(S) = qenc −→ E(r) ≡ 0
E
ǫ0
S

pues no hay carga en dicha zona del espacio.
r>b
El cálculo anteriormente realizado sigue siendo válido en esta región, y por ello:
E(r) =

qenc
A(S)ǫ0

Así, como A(S) = 4πr 2 , nos basta hallar la carga encerrada en este caso:
qenc =

ˆ 2π ˆ π ˆ b

ρ(r)r 2 sin θ dr dφ dθ

a

ˆ b

k 2
r dr
a r
= 4πk(b − a)
= 4π

Por tanto,
E(r) =

4πk(b − a) 1
k(b − a)
ǫ0
4πr
ǫ0 r 2

a<r<b
En este caso, la carga encerrada por la superficie gaussiana –esfera de radio r– es
ˆ r
k 2
r̃ dr̃
qenc = 4π
a r̃
= 4πk(r − a)
De esta forma,
E(r) =

4πk(r − a) 1
k(r − a)
ǫ0
4πr
ǫ0 r 2

(5)

a) Determine la forma diferencial de la ley de Gauss. ¿Qué hipótesis debe adicionar?
b) Una distribución de carga eléctrica produce un campo


~ = c 1 − e−αr ρ̂
E
r2

---

### Página 17

en donde c, α son constantes, y r es la distancia al origen. Encuentre la densidad volumétrica
de carga de la distribución, así como también la carga encerrada dentro de una esfera de radio
r = 1/α.
a) Supongamos que se cumplen las hipótesis del teorema de la divergencia (lo cual es razonable
para los problemas físicos de la mayoría de los casos), y por ello:
¨
~ · n̂ dS = qenc
E
ǫ0
S
˚
˚
~
∇ · E dV =
ρ dV
ǫ0
V
V

˚ 
ρ
~
dV
0 =
∇·E−
ǫ0
V

Como lo anterior fue realizado para un volumen arbitrario, y dado que las funciones son
continuas, entonces se infiere que el integrando debe ser nulo para la que igualdad sea válida
para cualquier volumen. Así,
~ = ρ
∇·E
ǫ0
que el la forma diferencial de la ley de Gauss.
b) Para obtener la densidad volumétrica de carga a partir de un campo, aplicamos la ley de Gauss
en su forma diferencial. Dado que trabajamos en coordenadas esféricas, la divergencia es:

1 ∂ 2 
1 ∂
1 ∂Fφ
∇ · F~ = 2
r Fr +
sin θFθ +
r ∂r
r sin θ ∂θ
r sin θ ∂φ
En este caso, Eφ = Eθ = 0, y por tanto:
−αr

~ = cαe
∇·E
r2

ρ(r) =

ǫ0 cαe−αr
r2

Ahora, la carga encerrada viene dada únicamente por:
Q = 4π

ˆ 1/α



−1
ρ(r)r dr = 4πǫ0 c 1 − e

(6) Considere una esfera aislante de radio a cargada eléctricamente con carga 3Q y, concéntrico a ella,
un cascarón esférico conductor, de radio interior b y exterior c, cargado con carga −Q (ver figura).
Encuentre el campo eléctrico para a < r, siendo r la distancia al centro de la esfera. Encuentre las
densidades de carga interior y exterior en el cascarón conductor.

---

### Página 18

Para calcular el campo usamos la ley de Gauss en coordenadas esféricas. Para a < r usamos
superficies gaussiana esféricas concéntricas de radio r dependiendo de la región de interés. En todos
los casos el campo es, por los mismos argumentos de simetría,
E(r) =

qenc
4πǫ0 r 2

Veamos cada región del espacio:
a<r<b
En este caso el radio r de la superficie gaussiana es tal que la carga encerrada corresponde a
la almacenada en la esfera de radio a, qenc = 3Q. Así,
E(r) =

3Q
4πǫ0 r 2

b<r<c
En este caso el campo eléctrico es nulo, por ser una región dentro de un conductor.
E(r) = 0
c<r
En este caso, el radio de la superficie gaussiana permite que esta encierre tanto la esfera como
al cascarón. Por ende, la carga encerrada es qenc = 3Q + (−Q) = 2Q. El campo es, entonces,
E(r) =

Q
2Q
4πǫ0 r
2πǫ0 r 2

Notar que en r = b, c el campo es discontinuo
Para obtener las densidades de carga en las superficies interior (r = b) y exterior (r = c) del cascarón
conductor, usamos el hecho de que dentro del conductor (b < r < c) el campo es nulo, por lo que
el flujo a través de una superficie gaussiana S esférica concéntrica de radio r entre b y c también se
anula,
¨
~ · n̂ dS = 0
Φe =
E
S

---

### Página 19

Pero, si el flujo se anula, necesariamente la carga encerrada dentro de esta superficie debe anularse.
Esto solo es posible si se inducen cargas en la superficie interior del cascarón, tal que 3Q + Qb = 0.
Luego, Qb = −3Q y la densidad en la superficie interna del cascarón es:
σb = −

3Q
4πb2

Ahora, como la carga neta del cascarón conductor es −Q, necesariamente se debe inducir carga en
la superficie exterior, tal que:
−Q = Qb + Qc = −3Q + Qc
de donde Qc = 2Q, y la densidad de carga en la superficie exterior queda dada por:
σc =

2Q
Q
4πc
2πc2

(7) Calcule la fuerza por unidad de largo que se ejercen una banda muy larga, de ancho b y densidad de
carga σ, y un alambre igualmente largo, con densidad lineal de carga λ, puesto en el mismo plano
que la banda a distancia d del borde inferior, como muestra la figura.

Podemos optar por calcular la fuerza que ejerce la distribución lineal de carga sobre la distribución
plana, o viceversa. Utilizaremos la primera opción, y para ello necesitamos obtener el campo eléctrico
generado por la distribución lineal. Esto puede calcularse con ley de Gauss, considerando la simetría
cilíndrica del campo eléctrico en presencia de una distribución lineal infinita de carga:

Si la superficie gaussiana es un cilindro de radio r y largo h, y utilizamos coordenadas cilíndricas,
entonces:
λh
λ
~
Φe = 2πrhE(r) =
−→ E(r)
ρ̂
ǫ0
2πǫ0 r

---

### Página 20

Dada la simetría del problema, y sin pérdida de generalidad, supondremos que la banda se encuentre
inmersa en el plano XY . Así, dq = σ dx dy. Calcularemos la fuerza que se ejerce sobre una porción
de largo L de la distribución planar:
~ dq = σλ dx dy ̂
dF~ = E
2πǫ0 y
con x ∈ [0, L], y ∈ [d, d + b]. Por lo tanto,
ˆ L

ˆ d+b

σλ
dy ̂
dx
2πǫ0 y
d
ˆ
σλL d+b
dyy ̂
2πǫ0 d


d+b
σλL
̂
ln
2πǫ0
d

F~ =

y, finalmente, la fuerza por unidad de longitud es:


~
F
σλ
d
+
b
f~ =
̂
ln
L
2πǫ0
d

1.3.
(1)

Potencial eléctrico
a) Calcule el potencial eléctrico en un punto P debido a un dipolo. Para ello, considere al dipolo
en el eje vertical, como se muestra en la figura.
b) Determine la energía potencial de un dipolo embebido en un campo eléctrico externo.

Antes que todo, algunas definiciones importantes:

---

### Página 21

(∗) Se define el potencial electrostático de una distribución continua de carga como:
φ(~r) =
4πǫ0

~
ρ(R)
d3 R
~
|~r − R|

˚
R3

(∗) La relación entre potencial y campo eléctrico es:
~ r ) = −∇φ(~r)
E(~
(∗) Se define el potencial electrostático de una distribución discreta de carga como:
N

1 X qj
φ(~r) =
4πǫ0 j=1 |~r − ~rj |
(∗) La interpretación física del potencial se asocia al trabajo realizado para mover una
carga a través de un campo eléctrico:
ˆ ~r2
~ · d~r = q(φ2 − φ1 )
E
W = −q
~
r1

a) Sea d = 2a. Por el principio de superposición,
φ(P ) =
4πε0



q
q
−
R1 R2



Por el teorema del coseno,
R1 2 = r 2 + a2 − 2ar cos (θ)
= r 2 + a2 − 2ar cos (θ)
R2 2 = r 2 + a2 − 2ar cos (π − θ) = r 2 + a2 + 2ar cos (θ)
Así,

r

 a 2

a

cos θ
r
r
Desarrollando en series de Taylor, para r ≫ a, tenemos que:

−1/2


 a 2
a
1  a 2  a 
1+
cos θ
1−
cos θ
−2
≈
+
R1
r
r
r
r
2 r
r
R1 = r

De manera análoga para R2 ,

Por tanto,

1+

−2



1  a 2  a 
≈
1−
cos θ
−
R2
r
2 r
r





q 1 2a
q
−
cos θ
φ(P ) =
4πε0 R1 R2
4πε0 r r
qd cos θ
4πε0 r 2
p cos θ
4πε0 r 2

---

### Página 22

con p = qd el momento de dipolo eléctrico. Finalmente,
φ(P ) =

p cos θ
4πε0 r 2

b) Supongamos la siguiente situación:

La energía potencial asociada al dipolo será:
U = −qφ(~r) + qφ(~r + ~a)
Podemos desarrollar φ(~r + ~a) en serie de Taylor (hasta el primer orden):
φ(~r + ~a) = φ(~r) +
Así,

∂φ
∂φ
∂φ
ax +
ay +
az = φ(~r) + ∇φ(~r) · ~a
∂x
∂y
∂z

~
U = q~a · ∇φ(~r) = p~ · ∇φ(~r) = −~p · E

(2) Considere un anillo de radio R uniformemente cargado con densidad λ. ¿Cuál es el potencial electrostático a una distancia z sobre el eje del anillo? En seguida, calcule el potencial en el eje de un
anillo de radio interior a, radio exterior b y densidad σ.

---

### Página 23

Tomemos un elemento infinitesimal de longitud en el anillo dℓ = R dθ, el cual posee un elemento de
carga dq = λR dθ. Su contribución al potencial en P es:
dφ(P ) =

1 dq
Rλ dθ
√
4πǫ0 r
4πǫ0 R2 + z 2

Luego, el potencial debido al anillo completo está dado por:
ˆ 2π
2πRλ
Q
√
√
φ(P ) =
dφ =
4πǫ0 R + z
4πǫ0 R + z 2
con Q la carga total del anillo. Es fácil ver que si z ≫ R, se tiene el potencial de una carga puntual
φ(P ) =

1 Q
4πǫ0 |z|

Ahora, para obtener el potencial de un disco de radios a y b, simplemente se considera la superposición de anillos infinitesimales:

Tomamos un anillo de radio r y ancho infinitesimal dr. Sabemos que el potencial en el eje está dado
por:
dQ
√
dφ(P ) =
4πǫ0 r 2 + z 2
donde dQ = σ2πr dr es la carga que contiene dicho anillo. Luego,
dφ(P ) =

r dr
2πσ r dr
σ
√
√
4πǫ0 r 2 + z 2
2ǫ0 r 2 + z 2

Finalmente, el potencial es:
σ
φ(P ) =
2ǫ0

ˆ b
a

√


√
r dr
σ √ 2
b + z 2 − a2 + z 2
2ǫ0
r2 + z2

---

### Página 24

(3) Considere dos cascarones esféricos de radios a y b (a < b). El cascarón interior tiene una carga
homogéneamente distribuida Q, y el exterior −Q. Encuentre la diferencia de potencial entre ambos
objetos.
Consideremos el siguiente esquema:
−Q
a
Q
b

El campo eléctrico en todo el espacio (de existir) es esféricamente simétrico. Lo mismo sucede con
el potencial, que será constante en una superficie esférica. Lo que se pide es
ˆ b
~ · d~r
∆V = φ(b) − φ(a) = −
E
a

Para evaluar la integral, claramente debemos encontrar el campo y elegir un camino desde a hasta
b. Utilizamos una superficie gaussiana esférica de radio r, con a < r < b. Por ley de Gauss:
¨
~ · n̂ dS = 4πr 2 E(r) = Q
E
ǫ0
S

Luego, en la región entre los dos cascarones,
~
E(r)

Q
ρ̂
4πǫ0 r 2

Dada la forma del campo, resulta inteligente elegir un camino radial:
γ : ~r = r ρ̂ ,
Luego,

a≤r≤b

d~r = dr ρ̂

~ · d~r = Q dr
E
4πǫ0 r 2

Entonces:
Q
∆V = φ(b) − φ(a) = −
4πǫ0

ˆ b

b

Q
dr
Q 1
4πǫ0 r a 4πǫ0
a r



1 1
−
b a



Notar que φ(b) − φ(a) < 0 → φ(b) < φ(a), i.e. cuesta más trabajo llevar una
carga hasta a que hasta b desde el infinito

---

### Página 25

(4) Iones de carga q son acelerados desde el reposo hasta una diferencial de potencial ∆V0 , para luego
entrar a una región entre dos electrodos cilíndricos muy largos, A y B, de radios a y b respectivamente
(a < b). El ion recorre media circunferencia de radio r0 describiendo la trayectoria señalada con
línea punteada. Despreciando los efectos de borde, y asumiendo que los cilindros son muy largos en
comparación al espacio que los separa, encuentre la diferencia de potencial ∆VBA .

Primero, debemos encontrar la velocidad con la que los iones ingresan a la región entre los cilindros:
Estos son acelerados a partir del reposo desde una región a potencial φ = V0 hasta otra región a
potencial φ = 0. La energía inicial está dada por
Ei = qV0
mientras que la energía final (justo antes de ingresar entre los electrodos) es
Ef =

mv 2

Así, por conservación de energía,
∆E = 0

v2 =

2qV0
m

Ahora, dentro de la región entre cilindros, existe un campo eléctrico radial que se puede obtener
con la ley de Gauss: utilizando una superficie gaussiana cilíndrica de radio r ∈ [a, b] y altura h, se
tiene:
qenc
2πrhE(r) =
ǫ0
en donde la carga encerrada por la superficie es qenc = σ2πha, donde σ es la densidad superficial
de carga sobre el cilindro de radio a. De aquí,
2πrhE(r) =
En particular,

σ2πha
ǫ0

~ 0 ) = σa ρ̂
E(r
ǫ0 r0

σa
~
E(r)
ρ̂
ǫ0 r

---

### Página 26

Este campo es el responsable de la fuerza que siente el ion (en dirección radial), y que permite su
trayectoria. Por equilibrio de fuerzas,
~ 0 ) = −m
q E(r

v2
ρ̂
r0

(el signo corresponde a la dirección de la fuerza centrípeta)

Despejando,
σ=−

2ǫ0 V0
a

y el campo eléctrico en el interior de los electrodos queda como
2V0
~
ρ̂
E(r)
=−
r
Ahora, la diferencia de potencial entre cilindros es:

 
ˆ b
ˆ b
b
2V0
~
dr = 2V0 ln
∆V = φ(b) − φ(a) = −
E · d~r = −
−
r
a
a
a
en donde hemos tomado un camino radial para realizar la integral de línea.

(5) Encuentre el potencial dentro y fuera de una esfera sólida cargada uniformemente, cuyo radio es R
y su carga total es Q. Use el infinito como punto de referencia.
Es fácil ver, por ley de Gauss, que el campo eléctrico en esta configuración (propuesto) viene dado
por:

Qr


ρ̂ , si r ≤ R

 4πǫ0 R3
~
E(r)


Q


ρ̂ , si r > R
4πǫ0 r 2
Potencial Exterior:
Ahora, para obtener el potencial electrostático, calculamos la siguiente integral del línea:
ˆ r
~ · d~r
φ(r) − φ(∞) = −
E
∞

Como usamos el infinito como referencia, φ(∞) = 0. Usando una trayectoria radial, d~r = dr ρ̂
y –para r > R–,
ˆ r
ˆ r
Q
Q
dr
Q
dr = −
φ(r) = −
4πǫ0 ∞ r
4πǫ0 r
∞ 4πǫ0 r

---

### Página 27

Potencial Interior:
Ahora, para r < R,
φ(r) = −

ˆ R

ˆ r

Eout (r) dr −
Ein (r) dr
R
ˆ r
Q
Q
−
r dr
4πǫ0 R 4πǫ0 R3 R
Q(R2 − r 2 )
Q
−
4πǫ0 R
8πǫ0 R3
Q(3R2 − r 2 )
8πǫ0 R3
∞

(6) Un alambre, cuya densidad lineal de carga es λ, se extiende en el eje z desde z = −d hasta z = d.
a) Calcule el potencial en un punto z > d sobre el eje del alambre.
b) ¿Cuál es el cambio de energía potencial de un electrón si se mueve de z = 4d hasta z = 3d?
c) Si el electrón parte del reposo desde z = 4d, ¿cuál es su velocidad en z = 3d?
Observación: No considere efectos gravitacionales.

~ = r k̂, dR = dr, y con ello ~r − R
~ = (z − r) k̂. Así,
a) Sean ~r = z k̂ y R


ˆ d
λ
λ
z+d
φ(z) =
dr =
ln
4πǫ0 −d z − r
4πǫ0
z−d
b) Un electrón se mueve desde z = 4d hasta z = 3d; luego, su cambio en energía potencial es:
 




eλ
ln
∆U = U(3d) − U(4d) = q φ(3d) − φ(4d) = e φ(4d) − φ(3d) =
4πǫ0

---

### Página 28

c) Por conservación de energía,
✘ = U(3d) + K(3d)
✘✘
U(4d) + ✘
K(4d)

eλ
ln
K(3d) = U(4d) − U(3d) = −∆U =
4πǫ0

 

pues parte del reposo. Así, despejando
v=

s

meλ
ln
2πǫ0

 

(7) Se tiene una distribución rectilínea de carga de densidad λ homogénea. Un punto P está a una
distancia r de la distribución, y su proyección sobre la recta de carga está a las distancias ℓ1 y ℓ2
de sus extremos.

a) Calcule el potencial electrostático en P . Analice los casos límites.
b) Obtenga el potencial en el punto P debido a un alambre infinito de carga.
~ = z k̂, dR = dz y |~r − R|
~ =
a) √
Tomando el origen tal como se muestra en la figura, ~r = r ρ̂, R
z + r . Así,
ˆ ℓ1
λ
dz
φ(P ) =
~
4πǫ0 −ℓ2 |~r − R|
ˆ ℓ1
λ
dz
√
4πǫ0 −ℓ2 r 2 + z 2
 ℓ1

√
λ
ln z + z 2 + r 2
−ℓ2
4πǫ0
!
p
λ
ℓ1 + ℓ1 2 + r 2
p
ln
4πǫ0
−ℓ2 + ℓ2 2 + r 2

---

### Página 29

b) Para calcular el potencial de un alambre infinito, ¿basta con hacer ℓ1 , ℓ1 → ∞? Si lo hacemos,
notamos que el potencial diverge. Esto se debe a que la carga eléctrica total en la distribución
no es finita, y solo en esos casos podemos fijar el potencial igual a cero en infinito. Para resolver
este problema, recordamos que el campo eléctrico producido por un alambre infinito es:
~
E(r)
= E(r) ρ̂ =

λ
ρ̂
2πǫ0 r

Sabemos que:

~ = −∇φ = dφ ρ̂
E
dr
pues la simetría del problema nos sugiere que no hay dependencia angular. Así,
ˆ
λ
φ(r) = − E(r) dr + C −→ φ(r) = −
ln (r) + C
2πǫ0

con C una constante arbitraria. Evaluando en r = 1, obtenemos que φ(1) = C. Luego, la
constante no es más que el potencial de todos los puntos que están sobre el manto cilíndrico
de radio unitario:
λ
φ(r) = −
ln (r) + φ(1)
2πǫ0
(8) Dos cables infinitos, paralelos al eje X, poseen densidades de carga uniformes λ y −λ. Ellos están
a distancia a del origen.
a) Encuentre el potencial en un punto (x, y, z) usando el origen como punto de referencia.
b) Demuestre que las superficies equipotenciales son cilindros circulares.
Tenemos dos alambres infinitos, cada uno a distancia a del origen, como se aprecia en la figura
(notar que el eje X sale de la página)

a) Por el principio de superposición, el potencial total en el punto P será la suma de los potenciales
debidos a cada distribución individual. El potencial debido al alambre de densidad λ es
φ1 (P ) = −

λ
ln (s+ ) + C1
2πǫ0

---

### Página 30

y el potencial debido al alambre de densidad −λ es
φ2 (P ) =

λ
ln (s− ) + C2
2πǫ0

Ahora, como nos piden que la referencia sea el origen, las constantes C1 y C2 deben satisfacer
φ1 (a) = φ2 (a) = 0
y con ello:
λ
λ
ln (a) + C1 −→ C1 =
ln (a)
2πǫ0
2πǫ0
λ
λ
ln (a) + C2 −→ C2 = −
ln (a)
φ2 (a) = 0 =
2πǫ0
2πǫ0
φ1 (a) = 0 = −

Notar que C1 + C2 = 0. El potencial en el punto P es
λ
λ
λ
ln (s+ ) +
ln (s− ) =
ln
φ(P ) = φ1 (P ) + φ2 (P ) = −
2πǫ0
2πǫ0
2πǫ0



s−
s+



Si P = (x, y, z), entonces
s− =
Finalmente,
φ(P ) =

p
(y + a)2 + z 2

λ
ln
2πǫ0

∧

s+ =

p
(y − a)2 + z 2

!
p


(y + a)2 + z 2
(y + a)2 + z 2
λ
p
ln
4πǫ0
(y − a)2 + z 2
(y − a)2 + z 2

b) Las curvas de nivel vienen dadas por:


(y + a)2 + z 2
= η = cte
(y − a)2 + z 2
Desarrollando,



(y + a)2 + z 2 = η (y − a)2 + z 2

y 2 + 2ay + a2 + z 2 = η(y 2 − 2ay + a2 + z 2 )

(1 − η)y 2 + 2(1 + η)yz + (1 − η)z 2 + (1 − η)a2 = 0
Si η = 1, entonces las curvas de nivel son solo puntos, por lo que pueden considerarse como
círculos de radio cero. Para η 6= 1,


1+η
y +z +a +2
ya = 0
1−η
Recordamos la ecuación de una circunferencia con centro en y0 y radio R:
(y − y0 )2 + z 2 = R2

←→

y 2 + z 2 − 2yy0 + (y0 2 − R2 ) = 0

De aquí, es claro que –en planos perpendiculares a los alambres– las superficies equipotenciales
son circunferencias con
√
2a η
η+1
∧
R=
y0 = a
η−1
|η − 1|

En definitiva, las superficies equipotenciales son cilindros:

---

### Página 31

(9) Considere un plano infinito con densidad superficial de carga uniforme positiva σ, el cual tiene una
perforación circular de radio R, tal como muestra la figura. Se define un sistema de coordenadas
cartesianas con origen en el centro del orificio, tal que la distribución de carga se encuentra en el
plano cartesiano Y Z. Calcule el trabajo que debe realizar un agente externo para llevar una carga
negativa desde el centro del disco hasta un punto sobre el eje X ubicado a una distancia D del
origen.

Primero que todo, recordemos que el trabajo realizado por un agente externo para llevar una carga
Q desde un punto a hasta un punto b está dada por:


W = Q φ(b) − φ(a)
Con anterioridad calculamos el campo eléctrico debido a esta configuración, el cual solo tenía una
componente no nula en la dirección ı̂:
σ
x
~
√
E(x)
ı̂
2ǫ0 x2 + R2

---

### Página 32

Por tanto, la diferencia de potencial entre el origen y el punto D en el eje X es:
ˆ D
~ · d~r
φ(D) − φ(0) = −
E
ˆ D
x
σ
√
= −
dx
2ǫ0 x + R2


σ √ 2
D +R −R
= −
2ǫ0
Así, el trabajo será:
W =−

1.4.


qσ √ 2
D + R2 − R
2ǫ0

Energía potencial electrostática

(1) Calcular la energía potencial electrostática de sistema de tres o cuatro cargas positivas, cada una
+q, que se colocan en las siguientes configuraciones:
a) Cada carga en las esquinas de un triángulo equilátero de lado a.
b) Cada carga en los vértices de un cuadrado de lado ℓ.
Recordemos que:
(∗) Para un sistema de n cargas, la energía potencial asociada al sistema es:
n

1X
qi Vi =
U=
2 i=1



4πǫ0

X
n X

n
qi qj
1 X X qi qj
ri,j
4πǫ0 i=1 j>i ri,j
i=1 j6=i

donde ri,j es la distancia que separa a las cargas qi y qj
(∗) Para un sistema continuo de cargas, la energía potencial asociada al sistema es:
˚
ρ(~r)φ(~r) d3 r
U=
V

(∗) La energía potencial almacenada en un campo eléctrico es:
˚
ǫ0
E 2 (~r) d3 r
U=
R3

---

### Página 33

a) En este caso, es fácil ver que:


q1 q2 q1 q3 q2 q3
U =
+
+
4πǫ0 r1,2
r1,3
r2,3
 2

q
q
q
+
+
4πǫ0 a
a
a
 2
3q
4πǫ0
a
b) El ejercicio es análogo, salvo por el cambio en las distancias:
r1,2 = ℓ
√
r1,3 =
2ℓ
r1,4 = ℓ
r2,3 = ℓ
√
2ℓ
r2,4 =
r3,4 = ℓ
Con ello,

√
4+ 2
= +√ =
r
ℓ
ℓ
2ℓ
i,j
i=1 j>i

4 X
X

Así, finalmente tenemos que:
q2
U=
4πǫ0

√ !
4+ 2
ℓ

(2) Cuatro partículas, dos de las cuales poseen carga +q y las otras dos −q, están ubicadas como indica
la figura. Si cada una posee masa m y se suelta de los vértices del cuadrado a partir del reposo, se
pide calcular sus velocidades cuando el largo del cuadrado vale ℓ. Suponga que todas las cargas se
mueven con la misma rapidez.

---

### Página 34

Por el principio de la conservación de energía, se cumple que
Einicial = Efinal
Si calculamos la energía inicial, notaremos que posee una contribución cinética y otra potencial,
por lo que:
Einicial = Kinicial + Uinicial
Como el sistema parte del reposo, se tiene que Kinicial = 0. La energía potencial inicial está dada
por:


qA qB qA qC
qA qD qB qC
qB qD qC qD
Uinicial =
+
+
+
+
+
4πǫ0 rA,B
rA,C
rA,D
rB,C
rB,D
rC,D


q2
q2
−4 ·
+2· √
4πǫ0
a
2a
!
√
2−4
q2
4πǫ0
a
Para la situación final, si cada una se mueve con velocidad v y poseen masa m, la energía cinética
final es:
X
mv 2
mi 2
vi = 4
= 2mv 2
Kfinal =
i=1
La energía potencial final se consigue cambiando a por ℓ, por lo que:
√
q2
2−4
Ufinal =
4πǫ0
ℓ
Así,

Uinicial = 2mv + Ufinal
Finalmente,
v=

s

v=

r

Uinicial − Ufinal
2m

 1 1
q 2 √
−
2−4
8mπǫ0
a ℓ

(3) Calcular la energía potencial electrostática del siguiente sistema de cargas puntuales:

---

### Página 35

El problema es fácil de abordar si se considera que hay:
12 pares de cargas, como A y B, con separación b entre ellas
√
12 pares de cargas, como A y C, con separación 2b entre ellas
√
4 pares de cargas, como A y H, con separación 3b entre ellas
√
3b
8 pares de cargas, como A y O, con separación
entre ellas
La energía total del sistema es la suma de las energías de cada par de cargas:


(−e)(−e)
(−e)(−e)
(−e)(−e)
(−e)(+2e)
12 ·
+ 12 · √
+4· √
+8· √
U =
4πǫ0
b
2b
3b
3b/2


√
e
12 + 6 2 − √
4bπǫ0
(4) Muestre que la energía potencial almacenada en una esfera sólida, de radio R, cargada uniformemente con una carga Q es


Q2
U=
5 4πǫ0 R
Utilizando coordenadas esféricas, la densidad de carga en la esfera está dada por:
ρ(r, ϕ, θ) = ρ(r) =

Q
3Q
4πR /3
4πR3

Como hemos calculado anteriormente, el potencial al interior de una esfera sólida con carga uniformemente distribuida es:
Q(3R2 − r 2 )
φ(r, ϕ, θ) = φ(r) =
8πǫ0 R3

---

### Página 36

De esta forma, dado que las cantidades no tienen dependencia angular,
ˆ
ˆ R
U =
dΩ
ρ(r) φ(r) r 2 dr
ˆ R
3Q
Q
· 4π ·
·
(3R2 − r 2 )r 2 dr
4πR 8πǫ0 R 0
3Q
4R5
·
16πǫ0 R6


Q
5 4πǫ0 R
(5) Una esfera de radio R posee una densidad de carga radial ρ(r) = kr, con k una constante. Encuentre
la energía potencial de esta configuración.
Calculemos el campo eléctrico en todo el espacio utilizando la ley de Gauss:
r>R
qenc =

ˆ

dΩ

ˆ R

ρ(r)r dr = 4π

¨

~ · n̂ dS = 4πr 2 E(r)
E

ˆ R

kr 3 dr = πkR4

Por otra parte,
S

Con ello,
4πr 2 E(r) =
r<R
qenc =

ˆ

dΩ

ˆ r

qenc
ǫ0

′

′2

′

E(r) =

ρ(r )r dr = 4π

ˆ r

kr ′ dr ′ = πkr 4

De manera análoga,
4πr 2 E(r) =

kR4
4ǫ0 r 2

qenc
ǫ0

E(r) =

kr 2
4ǫ0

Para el cálculo de la energía potencial, haremos uso del hecho de que el campo eléctrico no tiene

---

### Página 37

dependencia angular, por que tenemos:
ˆ
ˆ ∞
ǫ0
dΩ
E 2 (r) r 2 dr
U =
ˆ R

ˆ ∞
= 2πǫ0
E (r) r dr +
E (r) r dr

R

2 4 2

ˆ R

ˆ ∞

k 2 R8
k r
r
dr
+
r 2 dr
2πǫ0
2r4
16ǫ
16ǫ
R
ˆ R
ˆ ∞ 
k π
dr
r 6 dr + R8
8ǫ0
R r


k 2 π R7
+ R7
8ǫ0
πk 2 R7
k 2 π 8R7
·
8ǫ0
7ǫ0

!

1.5.

Conductores y capacitancias

(1) Para una distribución homogénea y esférica de carga, calcular:
a) El potencial en todos los puntos interiores
b) La energía potencial electrostática
a) Sabemos que, dentro de la esfera, el potencial debe satisfacer la ecuación de Poisson:
∇2 φ = ∆φ = −

ρ
ǫ0

Debido a la simetría esférica del problema, el potencial tendrá una dependencia radial con respecto al centro de la esfera. Así, φ = φ(r), y resolvemos la ecuación de Poisson en coordenadas
esféricas:


ρ
1 d
2 dφ
r
=−
r dr
dr
ǫ0
Esto es,
d
dr



ρr 2
2 dφ
r
=−
dr
ǫ0

r2

ρr 3
dφ
=−
+ c1
dr
3ǫ0

Integrando nuevamente,
φ(r) = −

ρr 2 c1
− + c2
6ǫ0
r

dφ
ρr
c1
=−
+ 2
dr
3ǫ0 r

---

### Página 38

Como calculamos el potencial dentro de la esfera, este debe ser finito en el origen; para ello,
debe cumplirse que c1 = 0. Con ello:
φ(r) = −

ρr 2
+ c2
6ǫ0

Para hallar c2 , le aplicamos continuidad al potencial en la frontera r = R:
φin (R) = −

ρR2
1 4/3πR3ρ
+ c2 =
= φout (R)
6ǫ0
4πǫ0
R

Finalmente,
ρ
φ(r) =
2ǫ0

c2 =

ρR2
2ǫ0



r2
R −

b) La Energía potencial asociada a una distribución de carga se puede obtener como:
U=

˚
V

ρ
φ dq =

˚

ρ
φ dV =

V

˚

4πρ
φr dr dΩ =

V

ˆ R

φ(r)r 2 dr =

4πρ2 R5
15ǫ0

(2) Una esfera de metal de radio R y carga q está rodeada por un cascarón esférico metálico de radio
interior a y radio exterior b. El cascarón no tiene carga neta.
a) Encuentre la densidad superficial de carga en cada superficie
b) Encuentre el potencial en el centro, utilizando infinito como punto de referencia
c) Si la esfera exterior se conecta a tierra bajando su potencial a cero (igual que en infinito),
¿Cómo cambian las respuestas anteriores?
a) Consideremos el siguiente esquema:

---

### Página 39

Como la esfera de radio R es metálica (conductora), toda la carga debe estar concentrada
en su superficie. Dada la simetría esférica del problema, esta distribución de carga debe ser
uniforme, es decir:
q
σR =
4πR2
Ahora, el cascarón es eléctricamente neutro; sin embargo, en sus superficies (Sa y Sb ), se induce
~
carga de forma tal que el campo eléctrico en su interior sea nulo, i.e. E(r)
= ~0, si a < r < b.
Tomando una superficie gaussiana en el interior del cascarón,
¨
~ · n̂ dS = 0 = Qint −→ Qint = 0
E
ǫ0
S

Así, como Qint = q + σa 4πa2 , es claro que:
σa = −

q
4πa2

Como el cascarón es neutro, debe cumplirse que
σa 4πa2 + σb 4πb2 = 0

q
a2
σb = − 2 σa =
b
4πb2

b) Distinguimos cuatro regiones, como se aprecia en la figura:

~ = ~0 y su potencial es constante
Como las regiones I, III están dentro de un conductor, E
(pueden ser distintos entre sí, pero iguales en todo punto de cada región). Para encontrar el
campo eléctrico en las regiones II, IV utilizamos la ley de Gauss. Tomando una superficie
esférica de radio r con R < r < a (región II), se tiene:
Φe = 4πr 2 E(r) =

q
ǫ0

E(r) =

1 q
4πǫ0 r 2

Del mismo modo, para r > b (región IV ), se cumple que:
E(r) =

1 q
4πǫ0 r 2

Con esto, podemos calcular el potencial en el origen
ˆ 0
ˆ ∞
✟
~ · d~r =
~ · d~r
✟ =−
φ(0) − ✟
φ(∞)
E
E
∞

---

### Página 40

tomando una trayectoria radial:
ˆ ∞
φ(0) =
E(r) dr
ˆ R
ˆ a
ˆ b
ˆ ∞
E(r) dr +
E(r) dr +
E(r) dr +
E(r) dr
R
a
b
ˆ ∞
ˆ a
q dr
q dr
+
4πǫ0 r 2
b
R 4πǫ0 r


q
+ −
4πǫ0 b R a
c) Ahora, tenemos que:

Hasta antes de la frontera r = b, el campo eléctrico y la densidad de carga se mantienen
intactos. Por otra parte, el potencial es nulo sobre la superficie exterior Sb , lo que implica que
ˆ ∞
φ(b) =
E(r) dr = 0
b

para cualquier camino que una al infinito con el punto b, pues el campo es conservativo. Luego,
como el integrando es continuo y vale cero para cualquier camino γ, por teoría de la integración,
debe cumplirse que
~ r ) = ~0 , ∀~r ∈ IV
E(~
Notar que lo anterior implica que la carga encerrada por una superficie gaussiana contenida
en IV necesariamente es cero. Es decir, el cascarón ya no es un objeto eléctricamente neutro
(se debe inducir una carga neta en él, igual a −q).
q + σa 4πa2 + σb 4πb2 = q − q + σb 4πb2 = 0

σb = 0

(3) Una esfera metálica hueca, con espesor no nulo, se encuentra inicialmente descargada. Ahora, imagine que una carga positiva q es colocada en algún lugar (no necesariamente al medio) dentro de la
esfera, sin tocar las paredes.

---

### Página 41

a) ¿Qué carga se induce en la pared interior y exterior de la esfera? Indicar cualitativamente la
densidad de carga inducida. Describir cómo son las líneas de campo eléctrico dentro y fuera
de la esfera.
b) Suponga que se mueve la carga dentro de la cavidad. ¿Cambia la distribución en la superficie
exterior de la esfera?
c) Ahora, se coloca la carga en contacto con la superficie interior de la esfera. ¿Cómo queda la
distribución de carga en la superficie interior y exterior?
d ) ¿Qué sucede si ahora se acerca otra carga Q cerca de la superficie exterior del conductor?
a) La carga q en el interior de la esfera metálica inducirá una separación de carga en el metal. Sea
qi la carga total inducida en la superficie interior, y qo la carga total inducida en la superficie
exterior. Debido a que la esfera inicialmente se encuentra descargada, la ley de conservación
de la carga indica que se debe tener
qi + qo = 0
Para determinar el valor de qi , tomemos una superficie gaussiana contenida enteramente dentro
del cascarón esférico. La carga total encerrada por esta superficie es qenc = q + qi . Debido a
que el campo eléctrico es nulo dentro de un conductor, la Ley de Gauss indica que:
Φe =

q + qi
=0
ǫ0

qi = −q, qo = −qi = q

La carga negativa en la superficie interna se concentra en la parte de la esfera más cercana a
la carga q. En contraste, la carga positiva de la superficie exterior se distribuye uniformemente
sobre la superficie exterior. Esto último debido a que la esfera metálica es una superficie
equipotencial, y la única forma de que esto suceda es que el campo sea radial y uniforme sobre
la superficie exterior.
La distribución de las cargas, y sus respectivas líneas de campo, son similares a como se aprecia
en la siguiente figura:

---

### Página 42

El campo fuera de la esfera es
~
E(r)

1 q
ρ̂
4πǫ0 r 2

tal como si la carga q se encontrara en el centro del conductor.
b) La distribución de carga en el exterior no cambia al mover la carga q en el interior, por la misma
razón anterior. Por supuesto, la carga inducida en el interior de la superficie sí se redistribuye
en la medida que movemos q, para asegurar que el campo en su interior siga siendo nulo.
Esto resulta interesante, pues desde el exterior del conductor podríamos saber cuánta carga se
encuentra en el interior, pero no podremos asegurar en qué posición se encuentra.
c) Cuando la carga q toca la superficie interior, la carga inducida −q se concentrará enteramente
en el punto de contacto y cancelará la carga q.
d ) Si se acerca ahora otra carga Q al exterior de la esfera, entonces la carga se distribuirá en la
superficie exterior de forma de ser una equipotencial. La distribución de carga al interior no
cambia debido a la presencia de una carga en el exterior. En otras palabras, si una cavidad
está encerrada en un conductor, ninguna distribución estática de carga en el exterior podrá
producir campos dentro. Este principio se conoce como shielding, y explica el por qué los
aparatos eléctricos se encuentran en cubiertas metálicas.
(4)

a) Considere dos placas metálicas conductoras de igual área A, y separadas por una distancia d.
La placa superior posee carga Q, mientras que la placa inferior posee carga −Q. Encontrar la
capacidad del sistema.
b) Considere un cilindro sólido de radio a rodeado por una cáscara cilíndrica de radio interior
b. La longitud de ambos cilindros es L tal que permite despreciar los efectos de borde. El
condensador se carga de forma que el cilindro interior posea carga Q y el exterior, carga −Q.
¿Cuál es su capacidad?
c) [Propuesto] Probar que la capacidad de una configuración esférica, compuesta de dos esferas
concéntricas de radios a y b, es


ab
C = 4πǫ0
b−a

---

### Página 43

a) Para encontrar la capacidad C, primero debemos saber la forma del potencial eléctrico en el
interior del condensador (y luego determinar la diferencia de potencial entre ambas placas).
Ignorando el efecto del borde del capacitor –producto a su largo finito–, se puede entender al
campo producido por ambas placas como el campo producto de un plano infinito: Para todo
punto fuera de la región interna del capacitor, se cumplirá que:
~ out = E
~ +Q + E
~ −Q = σ k̂ + −σ k̂ = ~0
E
2ǫ0
2ǫ0
Para todo punto dentro del capacitor, se cumple que:
~ in = E
~ +Q + E
~ −Q = σ k̂ + σ k̂ = σ k̂
E
2ǫ0
2ǫ0
ǫ0
Ahora, la diferencia de potencial entre las placas del condensador se obtiene integrando el
campo sobre una curva que va desde la placa positiva hasta la negativa; por simplicidad,
elegimos una trayectoria normal a cada superficie:
ˆ −
~ · d~r = −Ed = − σd −→ |∆V | = σd
∆V = φ− − φ+ = −
E
ǫ0
ǫ0
+
De esta forma, la capacidad de un condensador de placas planas y paralelas será:
C=

Q
ǫ0 A
|∆V |
d

Es claro como la capacitancia solo depende de factores geométricos (esta conclusión es válida
para cualquier sistema).
b) Para obtener la capacidad, debemos primero obtener el campo eléctrico en cualquier parte en
la región entre ambos conductores. Debido a la simetría cilíndrica del sistema, elegimos por
superficie gaussiana un cilindro coaxial con longitud ℓ < L y radio a < r < b. Usando la ley
de Gauss, con un campo radial, tenemos
Φe = E(r)2πℓr =

qenc
2πaℓσ
ǫ0
ǫ0

E(r) =

aσ
ǫ0 r

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
 
ˆ
aσ b dr
b
aσ
= −
= − ln
ǫ0 a r
ǫ0
a

donde el camino de integración tiene la dirección radial del campo eléctrico. De esta forma,
tenemos que:
2πǫ0 L
σ2πaL
Q
= aσ
C=
|∆V |
ln (b/a)
ln (b/a)
ǫ0

---

### Página 44

(5) Considere un condensador de placas paralelas cargadas con densidades σ y −σ , como muestra la
figura. Se arroja una carga q horizontalmente, por el espacio entre las placas, con velocidad vx .
Encuentre la trayectoria seguida por la partícula cargada y el ángulo que forma su vector velocidad
con la horizontal al momento de salir, considerando que ℓ es lo suficientemente grande como para
que la carga no choque con alguna de las placas. Desprecie efectos gravitacionales.

σ
k̂. Por tanto, la fuerza eléctrica ejercida sobre
ǫ0

~ =
EL campo eléctrico dentro del capacitor es E
la carga viene dada por la ley de Coulomb:

~ = qσ k̂
F~ = q E
ǫ0
De la segunda ley de Newton,
F~ = m~a

~a =

qσ
k̂
mǫ0

Separando la ecuación anterior en componentes, i.e. ~a = az k̂ + ax ı̂, tenemos:
ax = 0
x′′ = 0

x(t) = at + b

∗ Reemplazando las condiciones iniciales, x(0) = 0, x′ (0) = vx , obtenemos:
x(t) = vx t

az = β
z ′′ = β

z(t) =

β 2
t + bt + c

∗ Reemplazando las condiciones iniciales, i.e. z(0) = z ′ (0) = 0, concluimos que:
1 qσ 2
t
2 mǫ0

z(t) =

donde el origen coincide con la posición inicial de la carga al momento de entrar en el capacitor.
De las ecuaciones anteriores, es claro que la trayectoria de la partícula es una parábola en el plano
XZ. Ahora, el tiempo que demora en llegar al extremo derecho del capacitor será
x(t∗ ) = d

t∗ =

d
vx

---

### Página 45

Con esto, las componentes de velocidad en cada eje serán:
Vx (t∗ ) = x′ (t∗ ) = vx

Vz (t∗ ) = z ′ (t∗ ) =

∧

qσ d
mǫ0 vx

Finalmente, el ángulo está dado por
α = arctan



Vz (t∗ )
Vx (t∗ )



= arctan



qdσ
mvx 2 ǫ0



(6) Considere la configuración de la figura. Encuentre la capacidad equivalente, asumiendo que todos
los condensadores poseen la misma capacidad C.

Para los condensadores conectados en serie, la capacidad equivalente está dada por:
n
X
+
+ ...+
Ceq
C1 C2
Cn
Ck
k=1

Por otro lado, para los condensadores en paralelo, la capacidad equivalente es:
Ceq = C1 + C2 + . . . + Cn =

n
X

Ck

k=1

Para la segunda y tercera fila existen capacitancias equivalentes en serie, C2 , C3 respectivamente:
−1
−1


C
C
+
∧
C3 =
+ +
C2 =
C C
C C C

---

### Página 46

Ahora, los capacitores C, C2, C3 están en paralelo. Así,
Ceq = C + C2 + C3 =

C

(7) Se tiene un condensador plano, con capacidad C1 y un condensador esférico, con capacidad C2 . El
primero tiene cargas eléctricas q1 y −q1 , y el segundo tiene cargas eléctricas q2 y −q2 . Luego, se
conectan ambos condensadores como lo muestra la figura:

a) Obtenga las nuevas cargas Q1 , −Q1 , Q2 , −Q2 una vez obtenido el equilibrio eléctrico.
b) ¿Cuánto vale la pérdida de energía potencial eléctrica?

c) Según su sentido físico ¿dónde se pierde dicha energía?
d ) Se coloca un dipolo eléctrico p~ entre las dos esferas del condensador. ¿Qué sucede con él?
a) Por conservación de la carga eléctrica, al conectar ambos condensadores, la carga total solo
debe distribuirse, luego:
q1 + q2 = Q1 + Q2
Al producirse el equilibrio, los conductores unidos quedan al potencial V ; luego, la diferencia de
potencial entre sus terminales es común para ambos condensadores (que ahora están conectados
en paralelo):
Q1
C1
Q1 = C1 V , Q2 = C2 V
Q2
C2
Reemplazando en la primera igualdad,
Q1 =

C1 (q1 + q2 )
C1 + C2

∧

Q2 =

C2 (q1 + q2 )
C1 + C2

---

### Página 47

b) La energía inicial está dada por:
Ui =
Y la energía final es:

1 q1 2 1 q2 2
+
2 C1
2 C2

(Q1 + Q2 )2
1 Q1 2 1 Q2 2
Uf =
+
2 C1
2 C2
2(C1 + C2 )

Así, la energía perdida es la resta entre ambas cantidades:
−∆U = Ui − Uf =

1 (q1 C2 − q2 C1 )2
2 C1 C2 (C1 + C2 )

c) La pérdida de energía se produce debido a que, al conectar ambos condensadores, se produce
una redistribución de carga en ellos (y entonces, en un intervalo de tiempo corto, circula
una corriente eléctrica en los conductores). La energía que se pierde corresponde a la energía
disipada, en forma de calor, por los conductores.
d ) El dipolo gira para orientarse en el sentido del campo eléctrico entre ambas cáscaras esféricas.
Además, como el campo no es uniforme en esta región, el dipolo se desplaza hacia donde el
campo eléctrico es más intenso, i.e. hacia la cáscara negativa.
(8) Se tiene un circuito como el que se muestra en la figura:

1 uF

3 uF

S2

4 uF

+
−

2 uF

S1

12 V

a) Encontrar la carga de cada condensador cuando se cierra el interruptor S1 .
b) Lo mismo que lo anterior, ahora con S2 también cerrado.

---

### Página 48

a) Cuando S1 está cerrado, los dos capacitores superiores están en serie, así como también los
dos inferiores. Las capacidades equivalentes son:

−1
−1

1 1
Cupper = 1 +
µF = µF
µF = µF
∧
Clower =
+
2 4
Por último, Cupper y Clower están en paralelo, por lo que la capacidad total será:
Ct = Cupper + Clower =

µF

Con esto, podemos determinar la carga total suministrada por la fuente: Q = V C = 25 µC.
Ahora, sean Qi y Vi la carga y diferencia de potencial –respectivamente– del i−ésimo condensador, numerados en orden creciente respecto a su capacitancia. Por estar en serie, Q1 =
Q3 , Q2 = Q4 . Así:
Q1 = 1µV1 ,

Q2 = 2µV2 ,

Q3 = 3µV3 = Q1 ,

Q4 = 4µV4 = Q2

Además, los voltajes satisfacen
12 = V1 + V3 = V2 + V4
Resolviendo el sistema,
Q1 = V1 = 36 − 3V1 ,

Q2 = 2V2 = 48 − 4V2

V1 = 9, V2 = 8, V3 = 3, V4 = 4

Por último,
Q1 = 9 µC, Q2 = 16 µC, Q3 = 9 µC, Q4 = 16 µC
Se comprueba que Q1 + Q2 = Q3 + Q4 = 25 µC = Q.
b) En este caso, los condensadores C1 y C2 están en paralelo, al igual que C3 y C4 :
Clef t = C1 + C2 = 3 µF

∧

Cright = C3 + C4 = 7 µF

Ceq =

µF

La carga suministrada por la fuente será:
Q = Ceq V = 25.2 µC
Además, se tiene V1 = V2 , V3 = V4 , ya que se encuentran en paralelo. Así,
V1 =

= V2 =
,
Q1
Q2

V3 =

= V4 =
Q3
Q4

Con esto, 2Q1 = Q2 y 4Q3 = 3Q4 . También debe darse que Q1 + Q2 = Q3 + Q4 = 25.2 µC, y
por tanto:
2Q1 = Q2 = 25.2 − Q1 −→ Q1 = 8.4 µC, Q2 = 16.8 µC
Q3 = 25.2 − Q4 = 25.2 − Q3 −→ Q3 = 10.8 µC, Q4 = 14.4 µC

---

### Página 49

(9) Dos placas conductoras cuadradas de lado a se disponen paralelas y muy próximas entre sí. La
distancia horizontal entre las placas es x, mientras que una de ella se encuentra z unidades elevada
respecto a la otra (ver proyección lateral en la figura). Si se coloca una diferencia de potencial
constante Vo entre ellas, calcule la fuerza sobre la placa B en las direcciones x̂ y ẑ.

La energía almacenada en el condensador es:
U=

CVo 2

donde la capacidad está dada por
C=

ǫ0 A
ǫ0 a(a − z)
x
x

¿Cómo calculamos la fuerza? Un sistema conectado a una batería no esta aislado, pues la carga
cambia para mantener la diferencia de potencial (que es constante). Así,
dWsist + dUsist = dWbat
Notamos que es posible variar la energía potencial U sin que el sistema haga trabajo, si es que la
V0 dQ
y dWbat = V0 dQ
batería lo hace. En este caso, dUsist =
V0 dQ
Entonces, dWsist =
= dUsist , y en este caso F~sist = ∇U. Aquí no ocurre que la fuerza que
hace el sistema sea para lograr un estado de menor energía (eso es solo ocurre en un sistema aislado
a Q constante). De esta forma,
∂U
Vo 2 ǫ0 a  a − z
∂U
1 
~
F = ∇U =
k̂ = −
ı̂ +
ı̂ + k̂
∂x
∂z
x2
x

---

### Página 50

2.

Electricidad en medios materiales

2.1.

Ecuaciones de Laplace y Poisson

(1)

a) Considere dos cascarones cilíndricos conductores de radios a y b > a coaxiales, cargados a los
potenciales Va y Vb , respectivamente. Encuentre el potencial entre los cascarones.
b) Considere dos cascarones esféricos conductores de radios a y b > a concéntricos, cargados a
los potenciales Va y Vb , respectivamente. Encuentre el potencial entre los cascarones, y fuera
de ellos.
Para este, y todos los problemas del mismo estilo, conviene usar las ecuaciones de Laplace o de
Poisson. Estas ecuaciones describen microscópicamente el potencial en todo el espacio, en el sentido
de que dada la densidad de carga en un punto, se puede obtener el potencial en ese punto (desde
luego, también se puede partir del potencial, para obtener la densidad).
a) Dada la geometría del problema, empleamos coordenadas cilíndricas, con el eje z coincidente
con el eje de los cascarones. En este caso estamos, interesados en cualquier punto dentro de
la región entre ambos cascarones. En cualquiera de estos puntos no existen cargas (dicha
región es vacía), por lo que ahí ρ = 0. Por lo tanto, debemos resolver la ecuación de Laplace,
∇2 V = 0. Ahora, dada la simetría del problema, sabemos que el potencial debe depende solo
de la distancia al eje de ambos cilindros, por lo que esperamos que V = V (r). Así la ecuación
de Laplace queda muy simplificada:




1 d
dV
d
dV
r
= 0 −→
r
=0
r dr
dr
dr
dr
pues r 6= 0. Resolvemos la EDO:
r

dV
=A
dr

dV
A
dr
r

V (r) = A ln (r) + B

Las constantes A y B las determinan las condiciones de borde. En particular, sabemos que
V (a) = Va y V (b) = Vb , por lo cual:
Va = A ln (a) + B ,

Vb = A ln (b) + B

Restando ambas ecuaciones, obtenemos
Va − Vb = A ln

a
b

A=

Va − Vb
ln (a/b)

Por otra parte, multiplicando la primera ecuación por ln (b) y la segunda por ln (a), y restando,
 
Vb ln (a) − Va ln (b)
b
−→ B =
Va ln (b) − Vb ln (a) = B ln
a
ln (a/b)
que nos entrega el valor del potencial.

---

### Página 51

b) Por los mismos argumentos de ítem anterior, debemos resolver la ecuación de Laplace en
ambas regiones (entre y fuera de los cascarones). Esta vez, por simetría, usamos coordenadas
esféricas. A priori sabemos que el potencial no puede depender de los ángulos, o sea, V = V (r).
La ecuación de Laplace que hay que resolver es entonces:


1 d
A
2 dV
r
−→ V (r) = − + B
r dr
dr
r
Las condiciones de borde son las que nuevamente entregan los valores únicos de las constantes.
En este caso, debemos separar cada región de interés:
a<r<b
Las condiciones de borde relevantes aquí son: V (a) = Va y V (b) = Vb . Esto implica que
Va = −

A
+B ,
a

Vb = −

Despejando:
ab(Va − Vb )
A=−
,
b−a

B=−

en la región entre los cascarones.



A
+B
b

Va Vb
−
b
a



ab
b−a

b<r
Esta vez, las condiciones de borde relevantes son V (b) = Vb y que el potencial sea nulo en
el infinito, V (r → ∞) = 0. Esto implica que
Vb = −

A
+B ,
b

V∞ = B = 0

Es claro que
A = −bVb
en la región fuera de los cascarones.
Una pregunta propuesta al lector: ¿Es el potencial continuo en la interfaz? ¿Por qué?
(2) Dos conos conductores concéntricos, cuyas ecuaciones en coordenadas esféricas son θ1 = π/6 y
θ2 = π/4, se muestran en la figura. Los conos son de extensión infinita y en r = 0 están separados
por una distancia infinitesimal. Si el cono interior está a un potencial de 0 V, y el exterior a 50 V,
determinar el potencial y el campo eléctrico en la región interior a ambos conductores.

---

### Página 52

Sea V la región delimitada por θ1 < θ < θ2 . Si no hay densidad de carga libre en V, el potencial
satisface la ecuación de Laplace ∆V = 0. Dada la geometría del problema, es conveniente utilizar
coordenadas esféricas. El problema posee una clara simetría azimutal (el potencial no depende del
ángulo polar φ). Además, debe existir independencia de r, pues la extensión de los conos es infinita.
De esta forma, el potencial debe ser únicamente función de θ:


dV
d
∆V = 2
sin θ
=0
r sin θ dθ
dθ
o, equivalentemente,


dV
d
sin θ
=0
dθ
dθ

sin θ

dV
= C1
dθ

dV
= C1 csc θ
dθ

Recordando que la integral de la cosecante es ln (tan θ/2) + cte, entonces:
V (θ) = C1 ln (tan θ/2) + C2
Debemos imponer las condiciones de borde en las superficies conductoras. Se tiene que
V (θ1 ) = C1 ln (tan π/12) + C2 = 0 ,

V (θ2 ) = C1 ln (tan π/8) + C2 = 50

El despeje queda propuesto al lector. Para encontrar el campo eléctrico, utilizamos que
~ = −∇V
E
(3) [Propuesto] Suponga que el potencial V0 (θ) sobre la superficie de una esfera de radio R es dado.
Demuestre que la densidad de carga en la esfera es:
∞

ε0 X
σ(θ) =
(2l + 1)2 Cl Pl (cos θ)
2R l=0
donde
Cl =

ˆ π

V0 (θ)Pl (cos θ) sin θ dθ

Supongamos un potencial con simetría azimutal, de modo tal que V (r, θ, φ) = V (r, θ). Aplicando el
método se separación de variables, afirmamos que existen funciones R(r), A(θ) tales que V (r, θ) =
R(r)A(θ) para todo r ∈ (0, ∞), θ ∈ (0, π). Así, la Ecuación de Laplace toma la siguiente forma:

---

### Página 53

∆V = 0 →
→
→
→





∂V
∂
1 ∂
2 ∂V
r
+ 2
sin θ
=0
r 2 ∂r
∂r
r sin θ ∂θ
∂θ




.
R(r) ∂
∂A
A(θ) ∂
2 ∂R
r
+ 2
sin θ
=0
· R(r)A(θ)
r 2 ∂r
∂r
r sin θ ∂θ
∂θ




.
∂A
∂
∂
2 ∂R
r
+ 2
sin θ
=0
· r2
r 2 R(r) ∂r
∂r
r A(θ) sin θ ∂θ
∂θ




1 ∂
∂A
∂
2 ∂R
+
=0
r
sin θ
R ∂r
∂r
A sin θ ∂θ
∂θ
|
{z
} |
{z
}
λ

−λ

El método de separación de variables nos sugiere que λ es constante. Para hallar la componente
angular del potencial, resolvemos la parte derecha de la ecuación:


1 d
dA
sin θ
+ λA = 0
sin θ dθ
dθ
Con el cambio de variables t = cos θ y X = A(θ) tenemos que:




d
d
2 dX
2 dX
sin θ
+ λX = 0 −→
(1 − t )
+ λX = 0
dt
dt
dt
dt
que es justamente la Ecuación diferencial asociada a los polinomios de Legendre. Por tanto, X(t) =
Pl (t) y λ = l(l + 1). Para R(r), sugerimos que esta solución es de la forma R(r) = r n , y por tanto:


d 2 dR
r
− l(l + 1)R = 0 → r 2 n(n − 1)r n−2 + 2rnr n−1 − l(l + 1)r n = 0
dr
dr

→ n(n + 1) + 2n − l(l + 1) r n = 0
→ n(n + 1) + 2n − l(l + 1) = 0
→ n1 = l, n2 = −(l + 1)
Así, Rl (r) = al r l + bl r −(l+1) . Finalmente, el potencial posee como solución general:
V (r, θ) =

∞
X

l=0


al r l + bl r −(l+1) Pl (cos θ)

Volvamos al problema en cuestión. Notar que, tanto en la región interior como exterior de la esfera,
existen las siguientes condiciones
∆V = 0
V (R, θ) = V0 (θ)

---

### Página 54

lo que se conoce como Problema de Dirichlet. Para solucionarlo, definimos los potenciales internos
y externos a la esfera, a saber Vi n(r, θ) y Vout (r, θ) respectivamente. Del curso de Electricidad y
Magnetismo, sabemos que ambos potenciales deben satisfacer que:
Vin (R, θ) = Vout (R, θ) = V0 (θ)


∂Vout ∂Vin
σ(θ)
=−
−
∂r
∂r
ε0
r=R
Al interior de la esfera, la física del problema nos exhorta a buscar una solución que no diverja. Por
tanto, el término bl debe ser idénticamente nulo y con ello:
Vin (r, θ) =

∞
X

l=0


al r l Pl (cos θ)

Lo mismo ocurre fuera de la esfera, y por tanto al ≡ 0 y así:
∞
X
 −(l+1) 
bl r
Pl (cos θ)
Vout (r, θ) =
l=0

Analicemos la relación que existe entre al y bl en ambos potenciales. Como en la frontera (i.e. r = R)
éstos deben ser iguales, se cumple que:
∞
∞
X
X
 −(l+1) 


bl R
Pl (cos θ)
al Rl Pl (cos θ) =
l=0

l=0

bl = al R2l+1 , ∀l

Al mismo tiempo, como el potencial en la frontera tiene una forma determinada previamente en el
enunciado,
,ˆ
∞
π
X


al Rl Pl (cos θ) = V0 (θ)
Pm (cos θ) sin θ dθ

l=0

∞
X
l=0

al Rl

ˆ π

Pl (cos θ)Pm (cos θ) sin θ dθ =

ˆ π

V0 (θ)Pm (cos θ) sin θ dθ

∞
X
l=0

al Rl

δl,m = Cm
2l + 1
2m + 1
Cm
2Rm
Rm+1
Cm
= (2m + 1)

am =
∴ bm

Así, utilizando la condición para la densidad de carga se cumple que:

---

### Página 55


σ(θ)
∂Vout ∂Vin
= −
−
∂r
∂r
ε0
r=R
∞ h
i
X
σ(θ)
− (l + 1)bl R−(l+2) − lal Rl−1 Pl (cos θ) = −
ε0
l=0
∞
i
2l + 1
σ(θ)
1 Xh
l−1
(l + 1) (2l + 1)Rl+1 Cl R−(l+2) + l
Pl (cos θ) =
C
R
l
l
R
ε0


l=0

∞

σ(θ)
1 X
(2l + 1)2 Cl Pl (cos θ) =
2R l=0
ε0

Finalmente,
∞

ε0 X
σ(θ) =
(2l + 1)2 Cl Pl (cos θ)
2R
l=0

(4) [Propuesto] Una esfera de metal de radio R descargada es colocada en una región del espacio con
~ = E0 k̂. Note que, debido a las cargas inducidas en la superficie de la
campo eléctrico uniforme E
esfera, el campo eléctrico cambia en la vecindad de la esfera. Encuentre el potencial electrostático
fuera de la esfera. HINT: Para r ≫ R, V → −E0 z + C.
Consideremos a la esfera como una superficie equipotencial, donde fijaremos un potencial igual
a cero sobre la superficie de la misma. Así, la función potencial a encontrar debe satisfacer los
siguientes requerimientos:
V =0
V → −E0 z + C

si
si

r=R
r≫R

Considerando ambas condiciones, es claro que C = 0. Hagamos z = r cos θ para facilitar el análisis.
De la primera condición, notamos que:
∞
X

l=0


al Rl + bl R−(l+1) Pl (cos θ) = 0

y por tanto
al Rl + bl R−(l+1) = 0
Ahora,

bl = −al R2l+1





∞
X
R2l+l
R2l+l
l
l
V (r, θ) =
al r − l+1 Pl (cos θ) =
al r 1 − 2l+1 Pl (cos θ)
r
r
l=0
l=0

Si r ≫ R, entonces

∞
X

R
≪ 1 y dicha potencia es despreciable. Así,
r

---

### Página 56

∞
X
l=0

al r l Pl (cos θ) = −E0 z = −E0 cos θ

Por ortogonalidad (y dado que P1 (cos θ) = cos θ) es posible visualizar que, para l 6= 1 → al ≡ 0,
mientras que a1 = −E0 . Finalmente, el potencial fuera de la esfera tiene la siguiente forma:


R3
V (r, θ) = −E0 r − 2 cos θ
r

2.2.

Dieléctricos

(1) Calcular la capacidad del condensador de la figura, suponiendo que la placa intermedia posee una
discontinuidad en el medio.

El problema se puede tratar como dos condensadores en paralelo, uno formado por dos dieléctricos
de constante κ1 y κ2 , y el otro formado por dieléctrico de constante κ3 y vacío. A su vez, el primer
condensador (C1 ), se puede ver como dos condensadores en serie, llenos de los dieléctricos 1 y 2,
así:
+
C1
C11 C12
con
C11 =

κ1 ǫ0 S1
,
d1





Luego:
C1
ǫ0 S1

d1 d2
+
κ1 κ2

C12 =

κ2 ǫ0 S1
d2

C1 =

κ1 κ2 ǫ0 S1
d1 κ2 + d2 κ1

De manera similar, para el condensador C2 ,
+
C2
C21 C22
con
C21 =

ǫ0 S2
,
d1

y por ende
C2 =

C22 =

κ3 ǫ0 S2
d1 κ3 + d2

κ3 ǫ0 S2
d2

---

### Página 57

Finalmente, como C1 y C2 están en paralelo, la capacidad total será:
C = C1 + C2 =

κ1 κ2 ǫ0 S1
κ3 ǫ0 S2
+
d1 κ2 + d2 κ1 d1 κ3 + d2

(2) Considere una esfera conductora de radio interior a y radio exterior c. El espacio entre las dos
superficies es llenado con 2 dieléctricos distintos, de manera que la constante dieléctrica es κ1 entre
a y b, y κ2 entre b y c. Determine la capacitancia del sistema.

El sistema se puede tratar como dos capacitores conectados en serie, ya que la diferencia de potencial total a través de los capacitores es la suma de las diferencias de potencial a través de cada
condensador individual. La capacitancia equivalente para un capacitor esférico de radio interior r1
y radio exterior r2 lleno de dieléctrico de constante κ está dado por:
r1 r2
C = 4πǫ0 κ
r2 − r1
Así, la capacitancia equivalente del sistema es:


κ2 c(b − a) + κ1 a(c − b)
b−a c−b
+
C
4πǫ0 κ1 ba
κ2 bc
4πǫ0 κ1 κ2 abc
Finalmente:
C=

4πǫ0 κ1 κ2 abc
κ2 c(b − a) + κ1 a(c − b)

Notemos el caso límite en que κ1 , κ2 → 1, la expresión se reduce a
C=

4πǫ0 abc
4πǫ0 ac
4πǫ0 abc
c(b − a) + a(c − b)
b(c − a)
c−a

que concuerda con la capacitancia de un condensador esférico de radios a y c en el vacío.

(3) Un condensador cilíndrico de altura ℓ, y cuyos conductores tienen radios a y b (b > a), está cargado
con una carga Q, i.e. una armadura tiene carga +Q y la otra −Q. Entre ellas existe vacío. La
armadura es un cilindro metálico macizo. Este dispositivo se sumerge en un líquido dieléctrico de
densidad constante ρ y permitividad ǫ, a una profundidad h. Determinar la altura x que sube el
nivel del líquido que queda dentro del condensador, en relación al líquido externo (basta llegar a la
ecuación correspondiente).

---

### Página 58

La diferencia de nivel ∆h estará dada por el equilibrio entre la fuerza eléctrica sobre el líquido y su
peso. La fuerza electrostática es:
∂U
Fx = −
∂x
Como la carga es constante,
U=

1 Q2
2 C(x)

con C(x) la capacitancia del condensador cuando el líquido está a una altura x. De esta forma, el
problema se traduce en determinar la capacidad del condensador en función de la altura x.

La figura muestra que el condensador puede considerarse como dos condensadores conectados en
paralelo, uno de altura ℓ − x y otro de altura x. La capacidad total será la suma de las capacidades
C1 , C2 . Podemos hacer esta suposición (equivalente con 2 condensadores en paralelo) si despreciamos
los efectos de borde y la deformación del campo eléctrico cerca de la superficie del líquido:
C1 =

2πǫ0 (ℓ − x)
ln (b/a)

∧

C2 =

2πǫx
ln (b/a)

La capacitancia total será
C = C1 + C2 =
La energía eléctrica será
C=


2π 
ǫx + ǫ0 (ℓ − x)
ln (b/a)

1 Q2 ln (b/a)
4π x(ǫ − ǫ0 ) + ℓǫ0

Derivando, se obtiene la fuerza que tiende a subir al líquido:
Fx =

1 Q2 ln (b/a)(ǫ − ǫ0 )

2
4π
x(ǫ − ǫ0 ) + ℓǫ0

---

### Página 59

Por otra parte, el empuje del líquido es:
g(x − h)π(b2 − a2 )ρ = Ex
Finalmente, es posible determinar x a partir de
|Fx | = |Ex |
(4) Una esfera de radio R, con carga libre q, está sumergida en un medio dieléctrico homogéneo de
constante κ y de extensión teóricamente infinita. Calcular:
a) Los vectores de campo eléctrico y polarización a una distancia r > R
b) La densidad de carga de polarización
~ D
~ y P~ son todos paralelos entre sí en cada punto, y por la simetría esférica,
a) Debido a que E,
la naturaleza radial del campo no cambia por la presencia del medio dieléctrico. Además, estos
vectores pueden depender solo de la distancia al centro de la esfera y no de alguna coordenada
angular. Usando la ley de Gauss, con una superficie esférica de radio r > R concéntrica:
¨
¨
¨
q
~
D · n̂ dS =
D(r) dS = D(r)
dS = qlibre = q −→ D(r) =
4πr 2
S

S

S

Es claro que
~
D(r)

q
ρ̂
4πr 2

El campo eléctrico y la polarización pueden evaluarse fácilmente:
~ = κǫ0 E
~
D

~
E(r)

q
ρ̂
4πκǫ0 r 2

además,
~ = ǫ0 E
~ + P~
D

q(κ − 1)
~
ρ̂
P~ (r) = (ǫ − ǫ0 )E(r)
4πκr 2

b) Claramente, el dieléctrico ha debilitado la magnitud del campo eléctrico (en comparación al
espacio vacío). El campo eléctrico es originado por toda la carga, la de polarización y la carga
libre. La carga libre es solo la carga de la esfera q. Sin embargo, la carga de polarización se
forma de dos contribuciones: una densidad volumétrica
ρP = −∇ · P~
y una densidad superficial

σP = P~ · n̂

sobre la superficie del dieléctrico en contacto con la carga puntual.

---

### Página 60

Es claro que, en todos los puntos del dieléctrico,
~ =0
∇·E

∇ · P~ = 0

Usando que
q(κ − 1)
ρ̂
P~ (r) =
4πκr 2
la densidad superficial será
q(κ − 1)
σ = P~ · n̂ = P~ (R) · − ρ̂ = −
4πκR2
y la carga superficial es
Qs =

¨

σ dS = −4πR2

q(κ − 1)
q(κ − 1)
=−
4πκR
κ

S

Notar que la carga total será:
Qtotal = Qlibre + Qs = q −

q
q(κ − 1)
κ
κ

(5) Se tiene un condensador plano con placas cuadradas de largo a, distancia d entre placas, y una
carga total Q. Calcular la fuerza que se ejerce sobre un material dieléctrico cuando se encuentra a
una distancia x del punto O.

La energía potencial asociada a esta configuración es
U(x) =

1 Q2
2 C(x)

Notar que es función de la posición x, puesto que la capacitancia total también lo es. El sistema se
puede ver como dos condensadores en paralelo, uno de ellos con un dieléctrico de constante κ. Así,
Ceq = C1 + C2 =

ǫ0 a(x + κ[a − x])
ǫ0 ax κǫ0 a(a − x)
+
d
d
d

Con esto, la energía potencial eléctrica almacenada es:
U(x) =

Q2 d
2 ǫ0 a(x + κ[a − x])

---

### Página 61

¿Cómo obtenemos la fuerza? Para un sistema aislado a Q = cte, la conservación de energía nos dice
que el trabajo que hace el sistema más la variación de energía del sistema es cero. O sea, si está
aislado, el trabajo que haga el sistema es a costa de su propia energía. Entonces,
dWsist + dUsist = 0
Como dWsist = F~sist · d~r y dUsist = ∇U · d~r, esto implica que F~sist = −∇U. Así, la fuerza que se
ejerce sobre el dieléctrico será:
Fx ı̂ = −

dU
ı̂
dx

Fx =

Q2 d
1−κ
2ǫ0 a (x + κ[a − x])2

Notar que 1 − κ < 0, i.e. la fuerza apunta según −ı̂. Esto significa que la placa dieléctrica es atraída
hacia el interior del condensador. En este caso que es conservativo, la fuerza que hace el sistema
es para ir a una configuración de menor energía, y tira al dieléctrico hacia adentro (a Q constante,
Q2
U=
, así que con dieléctrico tiene menor energía).
2C
Una nota adicional. ¿Qué pasaría si el problema no consistiese en un sistema no aislado, i.e. a
V = cte? En este caso, la conservación de energía nos dice que el trabajo que hace el sistema más
la variación de energía del sistema es igual al trabajo realizado por la batería:
dWsist + dUsist = dWbat
En este caso,

Con ello,

dUsist = V0 dq

∧

dWbat = V0 dq

dWsist = dWbat − dUsist = V0 dq = dUsist

→

F~sist = +∇U

Aquí no ocurre que la fuerza que hace el sistema sea para lograr un estado de menor energía; eso es
solo para el sistema aislado a Q constante. En este caso, obviamente, la fuerza que hace el sistema
es la misma, es para tirar el dieléctrico hacia adentro:
A Q constante:

A V0 constante:



Q2
2C



CV0 2
~
F =∇



= V0 2 ∇C

F~ = −∇


1 Q2
∇C
2 C2

y, utilizando la relación Q = CV0 , se constata que son iguales.

(6) Un cilindro conductor hueco sin espesor, de radio r1 y largo ℓ, lleva una carga q uniformemente
distribuida. Alrededor de él, otro cilindro conductor hueco sin espesor es colocado de forma coaxial,
de radio r2 y mismo largo, tal como indicado en la figura. Este nuevo cilindro lleva una carga −q,
también uniformemente distribuida. Se llena la región entre los dos cilindros con un material cuya
constante dieléctrica es función de la distancia al eje de los cilindros, κ = κ(r). Considere ℓ ≫ r1 , r2 .

---

### Página 62

a) Encuentre una expresión para κ(r) que lleva un campo electrostático radial independiente de
la distancia al eje
b) Calcule la capacidad del condensador cilíndrico correspondiente
c) Calcule la densidad superficial de cargas de polarización en la superficie del material dieléctrico
a r = r1 y r = r2 , para el κ(r) calculado en el ítem (a)


~ = 1 ∂ rAr , calcular la densidad
d ) Considerando que, en coordenadas cilíndricas , ∇ · A
r ∂r
volumétrica de cargas de polarización en el dieléctrico
e) Calcular la cantidad total de cargas de polarización, incluyéndose cargas en la superficie y en
el volumen del dieléctrico
f ) Calcule la energía potencial electrostática almacenada en el condensador
g) Suponiendo que uno puede sacar el material dieléctrico de entre r1 y r2 deslizándolo fácilmente
sin roce, a lo largo del eje del sistema, calcule el trabajo necesario para remover el material de
entre las placas
a) Para obtener el campo electrostático en el interior, utilizamos la ley de Gauss para dieléctricos,
con una superficie cilíndrica de radio r ∈ (r1 , r2 ) y largo ℓ:

~ = D(r) ρ̂. Con esto,
Por simetría, es evidente que D
¨
~ · n̂ dS = 2πrℓD(r) = qlibre −→
D

D(r) =

q
2πrℓ

S

Así,
~ = 1D
~ = D(r) ρ̂
E
ǫ
κ(r)ǫ0

~
E(r)

Para que el campo no dependa de r, κ debe ser de la forma
κ(r) =

a
r

q
2πκ(r)ℓrǫ0

---

### Página 63

Con ello,
~ =
E

q
2πℓǫ0 a

b) En este caso, la capacitancia será la misma que un condensador cilíndrico, considerando que
ǫ = κ(r)ǫ0 . Así,
ˆ B
~ · d~r = φ(A) − φ(B) = ∆V
E
A
ˆ r2
q
ρ̂ · dr ρ̂
r1 2πℓǫ0 a
ˆ r2
q(r2 − r1 )
q
dr =
2πℓǫ0 a r1
2πℓǫ0 a
∴ C =

q
2πℓǫ0 a
∆V
r2 − r1

c) La densidad superficial de cargas de polarización está dada por:
σ = P~ · n̂
y
Sobre la superficie interior:

a

~
~
~
P = (ǫ − ǫ0 )E =
− 1 ǫ0 E
r

n̂ = − ρ̂ ,
y entonces,

P~ =



a
−1
r1




q
ρ̂
2πℓa

a
=−
σ1 = P~ · n̂
−1
r=r1
r1
Sobre la superficie exterior:



q
2πℓa

---

### Página 64



a
−1
r2



P~ =

n̂ = ρ̂ ,
y entonces,
σ2 = P~ · n̂

r=r2



a
−1
r2

q
ρ̂
2πℓa


q
2πℓa

d ) La densidad volumétrica de carga de polarización es
ρ = −∇ · P~
Como P~ = P (r) ρ̂ ya fue calculado anteriormente, simplemente se debe calcular la divergencia
como se sugiere en en el enunciado. Así,
q
ρ=
2πℓar
e) La carga total de polarización es
Qp =

˚

ρ dV +

¨

V

σ1 dS +

S1

¨

σ2 dS

S2

Como σ1 , σ2 son constantes en cada superficie respectiva, entonces:


¨
q
q
a
−1
· 2πℓr1 = −(a − r1 )
σ1 dS = σ1 · A1 = −
r1
2πℓa
a
S1

¨

σ2 dS = σ2 · A2 =

S2



a
−1
r2



q
q
· 2πℓr2 = (a − r2 )
2πℓa
a

Por otra parte, con dV = r dr dϕ dz,
˚
ˆ
ˆ
q
q r2
dr = (r2 − r1 )
ρr dr dϕ dz = 2πℓ ρr dr =
a r1
a
V

Así,

q
q
q
Qp = (r2 − r1 ) − (a − r1 ) + (a − r2 ) = 0
a
a
a
Esto siempre se cumple, pues un dieléctrico es eléctricamente neutro.

f ) La energía almacenada por el condensador es:
U=
donde
C=
y por tanto,

1 q2
2C

2πℓǫ0 a
r2 − r1

1 q 2 (r2 − r1 )
U=
2 2πℓǫ0 a

---

### Página 65

g) Tenemos que, la energía inicial viene dada por:
Ui =

1 q 2 (r2 − r1 )
2 2πℓǫ0 a

Por otra parte, la energía final será
Uf =

1 q2
2 Cf

donde Cf es la capacidad final (en el vacío):
Cf =

2πℓǫ0
ln (r2 /r1 )

Uf =

1 q 2 ln (r2 /r1 )
2πℓǫ0

Finalmente, el trabajo necesario para remover el dieléctrico es:
  

1 q2
r2 − r1
r2
W = Uf − Ui =
ln
−
2 2πℓǫ0
r1
a
(7) Se tienen tres esferas conductoras concéntricas de radios a, b, y c. El espacio entre las dos primeras
está lleno con un dieléctrico de constante κ. Inicialmente, la esfera de radio a está descargada y las
esferas de radios b y c tienen carga q1 y q2 , respectivamente. La esfera interior de radio a se conecta
con la esfera de radio c con un cable aislado delgado.

a) Calcular la carga libre en cada esfera
b) Calcular la carga de polarización en la superficie externa y en la superficie interna del dieléctrico
a) Definimos las siguientes cuatro regiones:

---

### Página 66

Al conectar las esferas de radios a y c, éstas distribuirán la carga en ambas de modo que
queden al mismo potencial, luego
q2 = qa + qc
Ahora, para la Región I,

~ < a) = ~0
E(r

pues corresponde al interior de un conductor. Para la Región II, a < r < b, se utiliza la ley de
Gauss para dieléctricos:
˚
qa
qa
~ · n̂ dS = 4πr 2D(r) = qa −→ D(r)
~
~
D
ρ̂
E(r)
ρ̂
4πr 2
4πκǫ0 r 2
Sr

Para la Región III, b < r < c,
˚
~ · n̂ dS = 4πr 2 E(r) = qa + q1
E
ǫ0

Sr

qa + q1
~
E(r)
ρ̂
4πǫ0 r 2

Por último, para la Región IV con r > c, tenemos:
q1 + q2
q1 + qa + qc
~
ρ̂ =
ρ̂
E(r)
4πǫ0 r
4πǫ0 r 2
Se sabe que la diferencia de potencial entre las esferas de radios a y c es nula, puesto que
ambas están unidas por un cable. Así,
ˆ c
ˆ b
ˆ c
~
~
~ · d~r = 0
0 = φ(c) − φ(a) = −
E · d~r −→
E · d~r +
E
a

donde

ˆ b
a

~ · d~r +
E

ˆ c
b

a

~ · d~r =
E

qa
4πκǫ0

b

ˆ b

dr qa + q1
+
4πǫ0
a r

ˆ c
b

dr
r2

Luego,




qa
1 1
qa + q1 1 1
+
= 0
−
−
4πκǫ0 a b
4πǫ0
b c




c−b
b−a
+ κ(qa + q1 )
= 0
qa
ab
bc
∴ qa




aκ(c − b)
= −
q1
c(b − a) + aκ(c − b)

---

### Página 67

Finalmente,




aκ(c − b)
qc = q2 − qa = q2 +
q1
c(b − a) + aκ(c − b)

b) Sobre la superficie interna del dieléctrico,

σ = P~ · n̂

r=a

,

~ ,
P~ = (ǫ − ǫ0 )E

n̂ = − ρ̂

Así,
σa = −

(ǫ − ǫ0 )qa
(κ − 1)qa
=−
4πκǫ0 a
4πκa2

Sobre la superficie externa,

σ = P~ · n̂

r=b

,

n̂ = ρ̂

σb =

(ǫ − ǫ0 )qa
(κ − 1)qa
4πκǫ0 b
4πκb2

2.3.

Corriente eléctrica y ley de Ohm microscópica

(1) Dos esferas metálicas concéntricas, de radios a y b, están separadas por un material conductor de
conductividad σ constante.

---

### Página 68

a) Si estas esferas son mantenidas a una diferencia de potencial V constante, encuentre la corriente
que va de una a la otra
b) Encuentre la resistencia entre las esferas
c) Observe que, en el caso anterior, se cumple R ∝ 1/C, donde C es la capacidad. Demuestre que
dicha fórmula el válida para dos conductores cualesquiera, separados por un material conductor
de conductividad σ constante
a) Al establecer una diferencia de potencial sobre los conductores
V = φ(a) − φ(b)
se inducirán cargas Q y −Q sobre las superficies r = a y r = b, respectivamente. El campo
eléctrico en la región interior se puede determinar a partir de la Ley de Gauss debido a la
simetría esférica del problema:
¨
Q
~
~ · n̂ dS = qenc −→ E(r)
ρ̂ , a < r < b
E
ǫ0
4πǫ0 r 2
Ω

Por otro lado,
V =

ˆ b
a

~ · d~r =
E

ˆ b

Q dr
Q
4πǫ0
a 4πǫ0 r

donde se ha elegido una trayectoria radial. Con ello,
Q=

4πǫ0 abV
b−a

~
E(r)



1 1
−
a b



V ab
ρ̂
(b − a)r 2

Debido a que la zona a < r < b está llena con un material conductor, el campo eléctrico dará
origen a un movimiento de cargas (corriente), en donde la densidad está relacionada con el
campo mediante la Ley de Ohm Microscópica
~ =
J~ = σ E

σV ab
ρ̂
(b − a)r 2

La corriente que fluye entre los conductores se puede obtener integrando sobre una superficie
esférica S de radio r, a < r < b:
¨
4πσV ab
I=
J~ · n̂ dS = 4πr 2J(r) =
(b − a)
S

---

### Página 69

b) La resistencia vendrá dada por la Ley de Ohm Macroscópica, V = IR, y con ello:


V
1 1
R=
−
I
4πσ a b
c) Recordando que la capacidad de un condensador esférico es
C=

4πǫ0 ab
b−a

entonces, se tiene que:
R=

ǫ0
σC

Veamos que esto se cumple en el caso general: Sean 1 y 2 dos conductores cualesquiera, separados por un material de conductividad σ:

Se tendrá un flujo de corriente dado por:
¨

I=

J~ · n̂ dS

Ω

Por ley de Ohm,

~
J~ = σ E

Reemplazando,
I=σ

~ · n̂ dS = σ Q
E
ǫ0

¨
Ω

por ley de Gauss. Por otro lado, si C es la capacidad del sistema, se cumple que
Q = CV
Reemplazando,
I=

σ
CV
ǫ0

R=

V
ǫ0
I
σC

(2) Considere un conductor perfecto, inicialmente con carga Q0 , y completamente rodeado por un medio
uniforme de conductividad σ y constante dieléctrica ǫ.

---

### Página 70

a) Si el conductor es una esfera de radio a, muestre que su carga como función del tiempo es
Q(t) = Q0 e−σt/ǫ
b) Muestre que el resultado anterior es válido independientemente de la forma del conductor
a) Sea Q(t) la carga sobre la superficie esférica en el instante t. Esta generará un campo eléctrico
esféricamente simétrico para r > a:
~ t) = Q(t) ρ̂
E(r,
4πǫr 2
Al ser el medio circundante un conductor, se tendrá una densidad de corriente como respuesta
a dicho campo:
~ t) = σ E(r,
~ t) = σQ(t) ρ̂
J(r,
4πǫr 2
Esta es una corriente que fluye isotrópicamente de forma radial. La corriente se obtiene de
integrar J~ sobre una superficie cerrada que contenga a la esfera conductora, en particular se
puede tomar una esfera de radio r > a:
¨
σQ(t)
I(t) =
J~ · n̂ dS =
ǫ
esfera

Por otro lado, sabemos que
dQ
= −I(t)
dt

dQ
σQ
=−
dt
ǫ

Q(t) = Q0 e−σt/ǫ

donde el signo aparece por tratarse de una descarga.
b) El resultado anterior es válido sin importar la forma de los conductores. En efecto, sea S una
superficie cerrada que contenga completamente al conductor. La corriente que se genera está
dada por:
¨
¨
~ · n̂ dS = σ Q
I=
J~ · n̂ dS = σ E
ǫ
S

S

donde hemos utilizado la ley de Ohm y la ley de Gauss. Es claro que
I =−

dQ
σQ
dt
ǫ

y se obtiene la misma ecuación diferencial que en el caso anterior.
(3) Entre dos cilindros conductores coaxiales muy largos, de radios a y c > a, se llena con materiales
de conductividades σ1 y σ2 , y permitividades ǫ1 y ǫ2 , como muestra la figura.

---

### Página 71

a) Encuentre la resistencia entre el núcleo y el conductor externo.
b) Si se conecta una diferencia de potencial V0 entre el núcleo y el conductor externo, calcule la
densidad de corriente J y la corriente I que circula.

a) Asumimos que la corriente circula radialmente desde la placa interna a la externa, de tal forma
que una corriente I se relaciona con la densidad como:
¨
¨
~
I=
J · n̂ dS =
J(r) dS
S

S

en donde S es el manto de un cilindro de radio r coaxial con los cascarones conductores. Por
simetría, la densidad de corriente sale de la integral. Si ℓ denota el largo de los cables, entonces
¨
I
I = J(r) dS = 2πrℓ J(r) −→ J(r) =
2πrℓ
S

Suponiendo válida la ley de Ohm en este material, el campo eléctrico podemos calcularlo
fácilmente. No obstante, debemos ser cuidadosos pues la conductividad varía en cada región
llena de material conductor. El campo en las regiones queda, respectivamente,
E1 =

I
,
2πσ1 rℓ

E2 =

I
2πσ2 rℓ

ambos en dirección radial. La diferencia de potencial entre ambas placas es
ˆ c
ˆ b
ˆ c
I ln (b/a) I ln (c/b)
|∆V | =
E(r) dr =
+
E1 (r) dr +
E2 (r) dr =
2πσ1 ℓ
2πσ2 ℓ
a
a
b
y, por tanto, la resistencia es:
R=

ln (b/a) ln (c/b)
+
2πσ1 ℓ
2πσ2 ℓ

Observación. Notar que |∆V | = |∆V1 | + |∆V2 |, por lo que R = R1 + R2 . Esto demuestra que
el sistema pudo haberse
P considerado como dos resistores en serie, para el cual sabemos que
vale la relación R = Rk .
k

---

### Página 72

b) Por la ley de Ohm, si se aplica una diferencia de potencial V0 entre las placas, la corriente que
fluirá de una a la otra es
2πℓV0
V0
I=
ln (b/a) ln (c/b)
R
+
σ1
σ2
y la densidad de corriente es
J(r) =

V0
I
ln (b/a) ln (c/b) r
2πℓr
+
σ1
σ2

(4) Suponga que se construye una cuña (figura abajo izquierda) usando material de resistividad ρ.
Determine la resistencia del cuerpo entre las caras A y B mostradas en la figura. Repita para el
cono truncado mostrado abajo a la derecha. El material es el mismo que en el primer resistor.

A
a
B
a+b

h

A

a

d

L

a+b
B

Para este problema debemos saber que la resistencia de un conductor de área transversal A y largo
L, hecho con un material de resistividad ρ, está dada por R = ρ L/A. La idea consiste en que, si
la corriente circula como indica el enunciado, el resistor se puede considerar como una sucesión de
resistores de área A(x) y ancho dx:

A(x)
a+b
h(x)

a

x=0

dx

x=L

---

### Página 73

La resistencia neta del cuerpo se obtiene sumando todas estas contribuciones, dado que podemos
P
considerar la sucesión como muchos resistores en serie, para lo cual sabemos que se cumple R = Ri
i
con:


ρ dx
b
A = A(x) = h(x) d = a + x d −→ dR =
L
A(x)
Por lo tanto,
R=

ˆ L

ρ

ρL
 dx =

bx
d
a+
L

ˆ 1



ρL
b
dt
ln 1 +
a + bt
bd
a

Para el caso del cono truncado,
x=0

a

A(x)

dx
r(x)

a+b

x=h

2

b
A = A(x) = πr (x) = π a + x
h

ˆ h

ρh
dt
(a + b t)
bπ

Así,
R=

ρ
dR =
π

ˆ h



ρh
2 =
π
bx

dx
a+

h

ˆ 1

dR =

ρ dx
2

bx
π a+
h


−
a a+b



(5) [Propuesto] En un diodo de vacío, los electrones son = evaporados” en un cátodo caliente, a potencial cero, y acelerados a través de una separación con el ánodo, que se mantiene a potencial
positivo V0 . La nube de electrones que se mueven dentro de la separación (llamados carga espacial )
rápidamente confluyen al otro lado. A partir de entonces existe una corriente constante entre las
placas. Supongamos que las placas son relativamente grandes comparadas con la separación entre
placas (A ≫ d2 en la figura), de modo tal que se pueden despreciar los efectos de borde. Entonces
V , ρ, and v (la velocidad de los electrones) son solo funciones de x:

---

### Página 74

a) Escriba la ecuación de Poisson para la región entre las placas.
b) Asumiendo que los electrones parten del reposo, ¿cuál es su velocidad en el punto x, donde el
potencial es V (x)?
c) En el estado estacionario, I es independiente de x. ¿Cuál es, entonces, la relación entre ρ y v?
d ) Use los tres resultados anteriores para obtener la ecuación diferencial para V , luego de eliminar
ρ y v.
e) Resuelva esta ecuación para V como función de x, V0 , and d. Grafique V (x), y compare con el
resultado sin carga espacial. Además, encuentre ρ y v como funciones de x.
f ) Muestre que
I = K V0 3/2
y encuentre la constante K. Esta ecuación es llamada Ley de Child-Langmuir. Note que el
diodo de carga espacial es no-lineal, y por tanto no obedece la ley de Ohm.

a) Como el potencial es solo función de x, entonces

ρ
d2 V
=−
dx
ǫ0

b) De la conservación de energía,
mv 2
qV =

v=

r

2qV
m

c) Es claro que:
dq = ρ dV = ρ A dx

dx
dq
= ρA
dt
dt

Así,
I = ρAv
Nota: ρ, y por tanto también I, son negativos.
d ) Ahora,

r
m
ρ
I
I
d2 V
d2 V
−
−
−
= β V −1/2
dx2
ǫ0
ǫ0 A v
ǫ0 A 2qV
dx2
r
I
m
con β = −
. Nota: I es negativa, entonces β es positivo; q es positivo.
ǫ0 A 2q

---

### Página 75

e) Multiplicando por V ′ =
V

′ dV

′

dx

=βV

dV
,
dx

−1/2 dV

dx

ˆ

′

V dV = β

ˆ

V −1/2 dV

V′ 2
= 2β V 1/2 + cte

Pero V (0) = V ′ (0) = 0 (el cátodo está a potencial cero, y el campo en el cátodo es cero), y
entonces la constante es cero. Así,
p
p
dV
= 2 β V 1/4 −→ V −1/4 dV = 2 β dx
V ′ = 4β V 1/2 −→
dx
p
∴ V 3/4 = 2 β x + cte
Pero V (0) = 0, y esta nueva constante también es nula. Así,

4/3
 2/3
1/3

3p
9β
3p
81I 2m
4/3
3/4
4/3
β x −→ V (x) =
β
x =
V
x4/3
x =
32ǫ0 2 A2 q
En términos de V0 , en vez de I,

V (x) = V0

 x 4/3
d

Sin la carga espacial, el potencial crecería linealmente con la distancia: V (x) = V0

x
d

Por otra parte,
d2 V
1 4 x−2/3
4ǫ0 V0
−ǫ
V
−
dx2
d4/3 3 3
9(d2 x)2/3
r
 x 2/3
p
2q √
v=
V = 2qV0 /m
m
d

ρ = −ǫ0

f)
V (d) = V0 =



81I 2 m
32ǫ0 2 A2 q

1/3

d4/3

V0 3 =

81md4 2
I
32ǫ0 2 A2 q

I2 =

32ǫ0 2 A2 q 3
V0
81md
| {z }
= K2

y por tanto,
I = K V0 3/2

---

### Página 76

2.4.

Ley de Ohm macroscópica: circuitos fem/R

(1) Determine la resistencia equivalente, o de Thevenin, entre los puntos a y b:
R
R

a

R

R

b

R

Optaremos por un método muy sencillo: aplicando una corriente I al circuito, sea V el voltaje entre
los puntos a, b. Así,
V = Va − Vb = I Req
Sean c, d los nodos intermedios. De las Reglas de Kirchhoff,
X

ik = 0

nodo a

X

Vd − Va Vc − Va
+
=0
R
R

ik = 0

ia→c + ib→c + id→c =

Va − Vc Vb − Vc Vd − Vc
+
+
=0
R
R
R

ik = 0

ia→d + ib→d + ic→d =

Va − Vd Vb − Vd Vc − Vd
+
+
=0
R
R
R

nodo c

X

I + id→a + ic→a = I +

nodo d

X

ik = 0

nodo b

−I + id→b + ic→b = −I +

Vd − Vb Vc − Vb
+
=0
R
R

De las dos ecuaciones intermedias, es claro que Vc = Vd y por tanto ic→d = id→c = 0. Así, llamando
Vo al voltaje en los nodos c, d:
I+

Vo − Va Vo − Va
+
=0
R
R

↔

Va =

IR
+ Vo

−I +

Vo − Vb Vo − Vb
+
=0
R
R

↔

Vb = −

V = Va − Vb = IR

Req = R

IR
+ Vo

Por lo tanto,
(2) Una batería descargada se carga conectándola a la batería cargada de otro automóvil mediante
cables para corriente. Determine la corriente del motor de arranque y en la batería descargada.

---

### Página 77

Utilizaremos la Ley de Voltajes de Kirchhoff (LVK) para cada malla:

Malla 1.
−12 + 0.01 · I1 + 1 · (I1 − I2 ) + 10 = 0
Malla 2.
−10 + 1 · (I2 − I1 ) + 0.06 · I2 = 0
De la primera ecuación se obtiene que
I2 = 1.01 I1 − 2
Reemplazando,
0.0706 I1 − 2.02 = 10

I1 = 170.25 A

Con esto,
I2 = 169.95 A
I2 es la corriente a través del motor de arranque, mientras que la corriente a través de la batería
descargada será, según nuestra convención,

---

### Página 78

Ibatery = I3 = I1 − I2 = 0.2975 A
(3) Tomando R = 1 kΩ y ε = 250 V en la figura, determine la dirección y magnitud de la corriente en
el cable horizontal entre los puntos a y e.

Definamos las siguientes corrientes:
I1 la corriente que circula por el △ abc en dicho orden

I2 la corriente que circula por el △ cde en dicho orden
I3 la corriente que circula por el △ cea en dicho orden
Utilizando la LVK, se cumple que:
−ε + I1 R + 4R(I1 − I3 ) = 0 ,

2RI2 + 2ε + 3R(I2 − I3 ) = 0 ,

4R(I3 − I1 ) + 3R(I3 − I2 ) = 0

Escribiendo el sistema en forma matricial,


 

5R
−4R
I1
ε
 0
5R −3R   I2  =  −2ε 
I3
−4R −3R 7R
Así, I3 viene dada por:

I3 =

5R
ε
5R −2ε
−4R −3R 0
5R
−4R
5R −3R
−4R −3R 7R

5R(0 − 6εR) + ε(0 + 20R2 )
−10εR2
ε
=−
= −50 mA
5R(35R − 9R ) − 4R(0 + 20R )
50R
5R

y con ello sabemos que va en dirección a → e.
(4)

a) Se tiene un circuito de infinitos resistores, cada uno con resistencia R, como muestra la figura.
Calcular la resistencia equivalente entre los puntos A y B.

---

### Página 79

A

...

...
B
b) Lo mismo para la siguiente configuración:

...

...
a) La idea es la siguiente: si hacemos un corte luego del primer elemento del patrón de resistencias,
notaremos que el resto de ellas es exactamente igual al caso antes de hacer el corte (pues son
infinitas resistencias) y por tanto son iguales a la resistencia equivalente pedida.

R
R

Req

R
De acuerdo a las reglas para combinar resistencias en serie y en paralelo, se establece la
ecuación:
Req = R + R + R k Req −→ Req 2 − 2RReq − 2R2 = 0
Resolviendo,
Req = R(1 +

√

3)

b) Repetimos el cálculo anterior, hasta obtener que:
Req = ϕ R
con ϕ el número áureo. Para mayor información se sugiere revisar aquí.
(5) Una batería real puede modelarse por una f.e.m. ε ideal y una resistencia interna en serie R. Una
resistencia de carga R2 se conecta a los terminales de la batería.
a) Determine el valor de R2 tal que la diferencia de potencial aplicada a los terminales sea máxima

---

### Página 80

b) Determine el valor de R2 para obtener una corriente máxima en el circuito
c) Determine el valor de R2 para que la potencia consumida por ésta sea la máxima posible
d ) Determine el valor de R para que la potencia consumida por R2 sea la máxima posible

a) Primero que todo, determinamos la corriente circulante,
−ε + IR + IR2 = 0

I=

ε
R + R2

Así, la diferencia de potencial entre los extremos de la batería es:
V = IR2 =

R2 ε
ε
R + R2
1 + RR2

Luego, la diferencia de potencial será máxima cuando R2 → ∞ y valdrá ε, igual que la f.e.m.
b) Teníamos que

ε
R + R2
Luego, la corriente será máxima si R2 = 0, y equivale a cortocircuitar los terminales de la
batería.
I=

c) La potencia consumida por R2 está dada por
ε
R2 ε2
R2 ε
P = IV =
R + R2 R + R2
(R + R2 )2
Para maximizar,

∂P
ε2 (R + R2 )2 − 2(R + R2 )R2 ε2
=0
∂R2
(R + R2 )4

Así,
(R + R2 )2 − 2(R + R2 )R2 = 0

R2 + R − 2R2 = 0

Finalmente, la potencia será máxima si
R2 = R
es decir, se debe colocar una resistencia igual a la resistencia interna de la batería.

---

### Página 81

d ) Se puede repetir el cálculo anterior, pero es más fácil optar por la intuición: si R es distinta
de cero, entonces ésta consumirá parte de la potencia que suministra la fuente. Así, para que
la resistencia de carga consuma toda la potencia suministrada por la fuente, se debe cumplir
que:
R=0
(6) El amperímetro ideal de la figura mide 2 A. Determine I1 , I2 y ε. Obtenga la potencia disipada en
cada resistencia.

Suponemos que la corriente fluye como muestra la figura. Por la ley de nodos aplicada al nodo de
la izquierda, se debe cumplir que
−I1 − I2 + 2 = 0

I1 + I2 = 2

en donde 2 A es la corriente que, por enunciado, pasa por el amperímetro. La ley de las mallas
aplicada a la malla superior entrega
2 · 5 − 15 + 7I1 = 0

y por tanto
I2 = 2 − I1 =

I1 =

A

A

La misma ley aplicada a la malla de abajo implica
2 · 5 − ε + 2I2 = 0

ε=

V

La potencia en cada resistencia la obtenemos a partir del Efecto Joule, P = I 2 R:
P7 Ω =

·7W =
W,

P5 Ω = 4 · 5 W = 20 W ,

P2 Ω =

·2W =
W

---

### Página 82

(7) El circuito de la figura es llamado Puente de Wheastone y se usa para calibrar resistencias. El dispositivo está formado por 3 resistencias, de las cuales 2 son ajustables, y un galvanómetro (dispositivo
que sirve para medir corrientes). Para realizar la medida, se ajustan las resistencias variables R1
y R2 hasta que el galvanómetro marque cero. Exprese el valor de Rx en función de las otras 3
resistencias. Modele al galvanómetro como una resistencia Rg .

La corriente que circula por el galvanómetro es:
Ig =

Va − Vb
Rg

Para que sea nula, debe cumplirse que: Va = Vb . Luego, aplicando LCK,
Nodo a:

Nodo b:

Igualando, obtenemos:

Va − 0
V − Va
R1
Rx

V − Va =

R1
Va
Rx

Vb − 0
V − Vb
R2
R3

V − Vb =

R2
Vb
R3

R1
R2
Va =
Vb
Rx
R3

Rx =

R1 R3
R2

2.5.

Circuitos RC

(1) En el circuito de la figura, suponga que el interruptor ha estado abierto por un tiempo muy largo,
y en t = 0 se cierra.

---

### Página 83

R1

ε

+
−

C
R2

a) ¿Cuál es la constante de tiempo antes de que se cerrara el interruptor?
b) ¿Cuál es la constante de tiempo después de que se cierra el interruptor?
c) Encuentre la corriente a través del interruptor como función del tiempo una vez que el interruptor se ha cerrado
a) Antes que el interruptor se cerrara, las dos resistencias R1 y R2 están en serie con el condensador. Debido a que la resistencia equivalente es Req = R1 + R2 , la constante de tiempo está
dada por
τ = Req = (R1 + R2 )C
y la carga almacenada en el condensador es


−t/τ
q(t) = Cε 1 − e
b) Una vez que el interruptor se cierra, el circuito cerrado a la derecha se vuelve un circuito RC
de descarga del capacitor que decae con constante de tiempo τ = R2 C. La carga comienza a
decaer acorde a
q(t) = Cε e−t/τ
c) La corriente a través del interruptor consiste en 2 fuentes: la corriente constante I1 del circuito
izquierdo, y la corriente que decae I2 del circuito RC. Las corrientes están dadas por
I1 (t) =
I2 (t) = −

ε
R1

dq
Cε −t/τ
ε −t/τ
e
e
dt
τ
R2

Así, la corriente total será:
IT (t) = I1 (t) + I2 (t) =

ε −t/τ
ε
+
e
R1 R2

(2) En el circuito de la figura, el interruptor se encuentra cerrado durante un tiempo muy largo.

---

### Página 84

C

ε

R3

R2

+
−
R1

a) ¿Cuál es la corriente en cada resistencia?
b) ¿Cuál es la carga en el condensador?
c) En t = 0 se abre el interruptor. Encuentre la corriente que pasa por la resistencia R2 en función
del tiempo
d ) ¿Cuánto tiempo debe pasar para que la carga en C disminuya hasta 4/5 del valor en t = 0?
a) El interruptor ha estado cerrado durante un tiempo muy largo, esto significa que el condensador
se ha cargado completamente. Cuando esto sucede, el condensador equivale a un circuito
abierto y no pasa corriente a través de él. Bajo estas circunstancias, solo habrá corriente por
la primera malla:

ε

+
−

I1

R2

R3

R1
I1 =

ε
ε
Req
R1 + R2

que es la corriente circulante por R1 y R2 . La corriente por R3 es nula.
b) Para obtener la carga en el condensador, primero debemos obtener el voltaje a través del mismo
y luego utilizar la relación que relaciona el voltaje con la carga acumulada C VC (t) = q(t). Nos
interesa la carga final del condensador, esto es
lím q(t) = C VC (t → ∞)

t→∞

Como ya vimos, después de un tiempo suficientemente largo no hay corriente por la malla
derecha, por lo que no hay diferencia de potencial entre los extremos de R3 . Por lo tanto, el
voltaje en el capacitor será igual a la caída de voltaje en R2 ,
VC (t → ∞) = VR2 = I1 R2 =
Con ello,
q(t → ∞) =

ε R2
R1 + R2

ε C R2
R1 + R2

---

### Página 85

c) Notemos que, al abrir el interruptor, no pasa corriente por la malla de la izquierda y se inicia
un proceso de descarga en el condensador:

C
+

ε

+
−

R2

-

R3

I2

R1
q(t)
C
Notemos que I2 es positiva; esto significa que las cargas positivas están dejando la placa positiva
y están llegando a la placa negativa. Es decir, la carga entre las placas está disminuyendo a
medida que I2 sea positiva:
dq
I2 = −
dt
I2 R3 − VC (t) + I2 R2 = 0

I2 (R2 + R3 ) = VC (t) =

Así, obtenemos una EDO de primer orden para q(t):
−

dq
q
(R2 + R3 ) =
dt
C

q(t) = q0 e−t/C(R2 +R2 )

con q0 la carga inicial del condensador, calculada en el apartado anterior.
d ) Para determinar el tiempo que debe pasar para obtener 4/5 de la carga inicial, resolvemos la
ecuación:
∗
q0 = q0 e−t /C(R2 +R3 )
t∗
ln (4/5) = −
C(R2 + R3 )
con lo que
t∗ = C(R2 + R3 ) ln (5/4)
(3) Dos condensadores de capacidades C1 y C2 están conectados a dos resistencias iguales R, como
muestra la figura. En t = 0 el condensador C1 posee una carga Q0 , mientras que C2 está descargado.

R

C1

C2
R

a) Obtenga las cargas de los condensadores en función del tiempo

---

### Página 86

b) ¿Cuál es la energía disipada por las resistencias?
c) Encuentre la energía disipada total hasta que se alcance el equilibrio. ¿De qué depende dicha
cantidad? Corrobore o refute su hipótesis y explique el por qué de ello
a) Intuitivamente, esperamos que en presencia de las resistencias, y ausencia de baterías externas,
el condensador inicialmente cargado se descargue, traspasando parte de su carga al condensador
inicialmente descargado. Veamos el comportamiento general de las cargas en cada condensador,
como función del tiempo. Aplicando la ley de las mallas, y tomando como sentido de la corriente
el de la figura, vemos que:

R
+Q1(t)

+Q2(t)

C1 -Q1(t)

C2 -Q2(t)
R

IR +

Q1
Q2
+ IR −
=0
C2
C1

La corriente que viaja por la malla es la misma, por lo que la tasa a la que se carga o descarga
cada condensador es exactamente I. En ese caso, tenemos que
I(t) = −

dQ1
dQ2
dt
dt

Note que ambas cargas no son independientes, ya que están supeditadas a la ley de conservación de carga:
Q0 = Q1 (t) + Q2 (t) , ∀t
Reemplazando en la primera ecuación,
2R

dQ2 Q2 Q0 − Q2
+
−
=0
dt
C2
C1

dQ2
Q2
Q0
+
dt
2RC0
2RC1

con C0 −1 ≡ C1 −1 + C2 −1 . La EDO anterior puede ser resuelta con su método favorito del
curso de Ecuaciones Diferenciales; en este caso, utilizaremos la Transformada de Laplace: Sea
F (s) = L{Q2 (t)}, así
s F (s) − Q2 (0) +

F (s)
Q0 /2RC1
2RC0
s

F (s) =

Q0 C0 /C1
Q0 /2RC1
s(2RC0 s + 1)
s(s + 1/2RC0 )

ya que Q2 (0) = 0. Aplicando fracciones parciales,



Q0 C0 
Q0 C0 1
−t/2RC0
−
e
−
−−
→
Q
(t)
F (s) =
C1
s s + 1/2RC0
C1
L−1

---

### Página 87

Por tanto,
Q2 (t) =


Q0 C0 
1 − e−t/2RC0
C1

∧


Q0 C0 
1 − e−t/2RC0
C1

Q1 (t) = Q0 −

Las cargas finales de los condensadores serán:


C0
,
Q1,f = Q0 1 −
C1

Q2,f = Q0

C0
C1

b) Del problema anterior, podemos obtener la corriente circulante por la malla:
I(t) =

dQ2
Q0 −t/2RC0
e
dt
2RC1

La potencia que disipa ambas resistencias es, por lo tanto,
P = P(t) = 2I 2 R =

Q0 2 −t/RC0
e
2RC1 2

c) La energía disipada corresponde a la integral de la potencia disipada por las resistencias desde
t = 0 hasta el infinito, cuando se alcanza el equilibrio. Así,
ˆ ∞
ˆ ∞
Q0 2
Q0 2 C0
−t/RC0
∆E =
P(t) dt =
e
dt
2RC1 2 0
2C1 2
que es independiente de R. La energía neta disipada es la diferencia entre la energía inicial y
la final del sistema. Por una parte, la energía inicial corresponde a la energía almacenada en el
condensador cargado, la cual es por supuesto, independiente de R. Por otra parte, la energía
final corresponde a la energía almacenada ahora en ambos condensadores, cargados con sus
respectivas cargas finales. Nuevamente, nada depende de R, por lo que la diferencia de energía
tampoco lo hará. Por ello esperamos que la energía disipada sea independiente de R. Note que
Ei =
de donde

Q0 2
,
2C1

Ef =

Q1,f 2 Q2,f 2
+
2C1
2C2

Q0 2 C0
∆E = Ef − Ei =
2C1 2

(4) En t = 0 el interruptor del circuito mostrado abajo se cierra. Obtenga las cargas en los capacitores, y
las corrientes que fluyen por las resistencias, si los condensadores inicialmente estaban descargados.

R1

C1

R2

C2

S

ε

---

### Página 88

Supongamos que la corriente circula como muestra la figura de abajo, y apliquemos ley de las mallas
a la malla del borde exterior:

R1

+ Q1 - Q1

I1
I2
+ Q2

- Q2

R2

I(t)
ε

−ε + I1 R1 +
Mientras que en la malla interior,
−ε +

Q1
=0
C1

Q2
+ I2 R2 = 0
C2

Claramente, la tasa a la que se carga cada condensador es igual a la corriente que pasa por dicho
condensador. Así,
dQ1
dQ2
I1 =
, I2 =
dt
dt
Reemplazando en las ecuaciones,
−ε + R1

dQ1 Q1
=0,
+
dt
C1

−ε +

Q2
dQ2
+ R2
=0
C2
dt

Resolveremos detalladamente la primera ecuación mediante Separación de variables:

ε
Q1
1 
dQ1
εC1 − Q1
−
dt
R1 R1 C1
R1 C1
Así,
ln (εC1 − Q1 ) = −

dQ1
dt
εC1 − Q1
R1 C1

t
+A
R1 C1

Tomando la exponencial, y definiendo B = eA , una nueva constante,
Q1 (t) = εC1 − B e−t/R1 C1
Como inicialmente el condensador estaba descargado, B = εC1 , y por tanto:


Q1 (t) = εC1 1 − e−t/R1 C1

---

### Página 89

Para el segundo condensador es un proceso análogo,


Q2 (t) = εC2 1 − e−t/R2 C2
Derivamos para obtener las corrientes,
ε −t/R1 C1
I1 (t) =
e
,
R1

I2 (t) =

ε −t/R2 C2
e
R2

∆V y se abre cuando ∆Vc < ∆V . El voltímetro
ideal mide la diferencia de potencial graficada en la figura (b). ¿Cuál es el periodo T de la onda en
función de R1 , R2 y C?

(5) El switch en la figura (a) se cierra cuando ∆Vc >

Partamos en el punto cuando el voltaje recién ha alcanzado el valor de ∆V y el switch acaba de
cerrarse. El voltaje es ∆V y decae hacia 0 con una constante de tiempo R2 C:
∆Vc (t) = ∆V e−t/R2 C
Queremos hallar t1 cuando ∆Vc alcanza el valor de
∆V = ∆V e−t/R2 C
Después se abre el switch, el voltaje es
(R1 + R2 )C:

∆V . Así,

t1 = R2 C ln (2)

∆V y crecerá hasta ∆V con una constante de tiempo

∆Vc (t) = ∆V −

∆V e−t/(R1 +R2 )C

---

### Página 90

Ahora, queremos hallar t2 cuando ∆Vc alcanza el valor de
∆V = ∆V − ∆V e−t/(R1 +R2 )C

∆V . Así,
t2 = (R1 + R2 )C ln (2)

Finalmente,
T = t1 + t2 = (R1 + 2R2 )C ln (2)
(6) [Propuesto] Considere el siguiente circuito, donde todas las resistencias tienen un valor de R y el
condensador vale C:

V(t)

+
−

Si V (t) = Vo H(t), con H el escalón unitario, determine el valor de la corriente inicial (t = 0) y
final (t → ∞) que circula por la fuente de voltaje, considerando que el capacitor está inicialmente
descargado.
Notemos lo siguiente:
R

2R
R
2R

+
−

+
−

+
−

R

R

R

R

En t = 0, el condensador se comporta como un cortocircuito, por lo cual la resistencia en paralelo
con ella no influye en el circuito, y por tanto la corriente será limitada solo por la resistencia restante
en serie. Así,
Vo
I(t = 0) =
R

---

### Página 91

Por otra parte, en el infinito el condensador se comporta como un circuito abierto, por lo cual la
resistencia equivalente será la suma de las resistencias en serie, 2R, y por tanto la corriente será
I(t → ∞) =

Vo
2R

Comprobemos lo anterior: Consideremos la ecuación básica del condensador
Q=CV

I=C

dV
dt

−−→ I(s) = sC V (s) − V (0)
L

como Q(0) = 0, entonces V (0) = 0. En el dominio de Laplace,
Z(s) =

V (s)
I(s)
sC

y se comporta como una resistencia. Para evitar la confusión, diremos que el condensador y
la resistencia son ejemplos de impedancias, i.e. elementos resultantes del cociente entre voltaje y
corriente en Laplace. Con esto en mente, podemos definir una impedancia equivalente:
−1

2R + s R2 C
+ sC
Zeq = R + (R k C) = R +
R
1 + s RC
Así,

Vo
1 + s RC
2R + s R C s
Vo
RCVo
· +
2R + s R C s 2R + s R2 C
Vo /R2 C 1
Vo /R
· +
s + 2/RC s s + 2/RC

V (s)
I(s) =
Zeq



Aplicando la transformada inversa,


Vo
Vo −2t/RC
1 − e−2t/RC
I(t) =
+
e
R C
2/RC
R
 V
Vo 
o −2t/RC
1 − e−2t/RC +
e
2R
R

Vo 
1 + e−2t/RC
2R
que corrobora nuestro análisis inicial.

---

### Página 92

3.

Magnetostática

3.1.

Fuerza de Lorentz y torque sobre una espira

(1) Se lanza un electrón (e− ) con velocidad inicial ~v en el medio de dos placas entre las cuales existe
~ constante (entrando a la hoja). Ignore todo efecto gravitacional.
un campo magnético B

a) ¿Hacia dónde se deflecta la trayectoria?
b) ¿Cuál es la magnitud de la velocidad si la partícula choca exactamente con el fin de la placa?
a) La fuerza de Lorentz corresponde a la unión entre electromagnetismo y mecánica clásica, y
establece que:


~
~
~
F = q E + ~v × B

~ ≡ ~0. Dado que la velocidad inicial es perpendicular al campo
En este caso, q = −e y E
magnético, la trayectoria será una circunferencia en el plano XY :

Para analizar hacia dónde se deflectará la partícula, basta con analizar lo que ocurre en el
instante inicial t = 0,
~ = v0 ı̂ × −B k̂ = v0 B ̂
~v (0) × B
Luego, la fuerza inicial es:

F~ (0) = −ev0 B ̂

y, por tanto, se deflectará hacia abajo.
b) Dado que el electrón impactará al extremo derecho de la placa inferior, entonces debe realizar
una trayectoria como la siguiente:

---

### Página 93

La magnitud de la fuerza magnética está dada por F = ev0 B, y su dirección es radial (apuntando hacia el centro de curvatura). Por mecánica clásica, se tendrá:
ev0 B =

mv0 2
R

De trigonometría plana, se sabe que:
2

d
= R2
l + R−
Igualando,

mv0
l2 d
= +
eB
d

R=

mv0
eB

R=

eB
v0 =
m

l2 d
+
d

 2

l
d
+
d

(2) Suponga que la figura representa esencialmente los componentes de un espectrómetro de masas. Este
aparato se usa para medir la masa de partículas cargadas. En una fuente se produce un ion de masa
m y carga q, el cual parte del reposo y es acelerado por una diferencia de potencial ∆V , entrando en
una sección con un campo magnético uniforme (entrando a la hoja), y un campo eléctrico deflector.
Solo partículas con velocidad ~v constante abandonan la sección (es un selector de velocidades). Las
partículas emergentes entran a una segunda región donde existe otro campo magnético (entrando
a la hoja), donde ellas siguen una trayectoria circunferencial hasta estrellarse en un detector a
distancia 2r del punto de entrada.
a) Encuentre la velocidad ~v
~ yB
~
b) Encuentre el la relación entre E
c) Finalmente, encuentre la masa m de la partícula

---

### Página 94

a) La velocidad v con que el ion entra al selector se obtiene por conservación de energía:
q ∆V =

mv 2

donde el cambio en energía potencial se traduce en un aumento en la energía cinética. Así,
r
2q ∆V
~v =
̂
m
b) Para que la velocidad de la partícula permanezca constante y salga a través del selector, se
requiere que la fuerza de Lorentz actuando sobre ella sea nula. Se tiene:
~ = E ı̂ ,
E
qE ı̂ − qv ̂ × B k̂ = ~0

~ = −B k̂ , ~v = v ̂
B


qE − qvB ı̂ = ~0 −→

E = vB

~ 0 , la partícula describe una circunferencia
c) Luego de ingresar a la región de campo magnético B
de radio r. La magnitud de la fuerza magnética es qvB0 . Por dinámica circular,
r
mv 2
m 2q ∆V
qvB0 =
−→ qB0 =
r
r
m
y finalmente:
m=

qB0 2 r 2
2 ∆V

(3) Una partícula de carga q y masa m entra con velocidad v en un campo magnético uniforme B como
se muestra en la figura. ¿Cuánto tiempo transcurre entre que la carga ingresa al campo magnético
y sale?

---

### Página 95

Es sabido que la fuerza magnética sobre una carga en movimiento q está dada por la fuerza de
Lorentz. Esta fuerza es siempre perpendicular a ~v ; luego, se sigue que esta fuerza no ejerce trabajo. Con esto, la energía cinética de la partícula es constante y entonces su rapidez también. La
trayectoria que sigue la partícula bajo este campo magnético uniforme es una hélice:

Si se observa el movimiento proyectado en un plano perpendicular al campo magnético, la trayectoria
describe una semicircunferencia, hasta volver a salir de la región donde se encuentra el campo
magnético. Sea R el radio de ésta, luego podemos determinar el tiempo que demora en salir como
T =

πR
v′

con v ′ la componente de velocidad perpendicular al plano. De la segunda ley de Newton,
mv ′ 2
= F = qvB sin (π/4) = qv ′ B
R
Finalmente,
T =

R=

mv ′
qB

πm
qB

---

### Página 96

(4) Considere el circuito cerrado de la figura que lleva una corriente I en el sentido contrario al reloj. Un
campo magnético uniforme apuntando en la dirección ̂ es aplicado. Encuentre la fuerza magnética
que actúa sobre el elemento rígido y el arco semicircular.
y
~
B

d~r

I
R

I
ϕ

x

I

~ = B ̂ , llamemos F~1 y F~2 a las fuerzas actuando sobre el
Tenemos un campo uniforme dado por B
segmento rígido y la parte semicircular, respectivamente. La fuerza sobre el segmento rígido es:
ˆ R 
ˆ R 
F~1 = I
d~r × B ̂ = I
dr ı̂ × B ̂ = 2IRB k̂
−R

−R

Ahora, para calcular F~2 , notamos que elemento infinitesimal en el semicírculo se puede escribir
como:


d~r = dr θ̂ = R dϕ − sin ϕ ı̂ + cos ϕ ̂

La fuerza que actúa sobre un elemento d~r es:


~
~
dF2 = I d~r × B = IR dϕ − sin ϕ ı̂ + cos ϕ ̂ × B ̂ = −IBR sin ϕ dϕ k̂
Integrando sobre el arco semicircular, tenemos:
ˆ π

F~2 = −IBR
sin ϕ dϕ k̂ = −2IBR k̂

Así, la fuerza neta que actúa sobre el circuito completo es
F~neta = F~1 + F~2 = ~0
Consistente con el hecho de que la fuerza sobre un circuito cerrado en un campo magnético uniforme
es siempre nula.

---

### Página 97

~ y a un campo
(5) Considere una partícula de carga q y masa m, sometida a un campo eléctrico E
~ ambos uniformes y perpendiculares entre si. Suponga que inicialmente (t = 0) la
magnético B,
carga se encuentra en el origen y en reposo.
a) Describa cualitativamente el movimiento posterior (t > 0) seguido por la partícula. Haga un
dibujo de la trayectoria.
b) Resuelva las ecuaciones de movimiento, sujetas a las condiciones iniciales mencionadas. Usando
esta solución, describa el movimiento de la partícula y compare con el apartado anterior.
a) Sea q > 0. Supongamos, sin pérdida de generalidad, que el campo eléctrico y el campo
magnético están dados por
~ = E ̂ , B
~ = B k̂
E
Dado que en t = 0 la velocidad inicial de la partícula es nula, no hay fuerza magnética (instante
A en la figura). La fuerza eléctrica, en cambio, apunta en la dirección ̂, acelerando la partícula.
La partícula comienza a moverse aumentando su velocidad, y con ello la fuerza magnética. Esta
última deflecta la partícula hacia x > 0 según la regla de mano derecha. A diferencia de los
problemas anteriores, esta vez el movimiento no es circunferencial. A medida que la fuerza
magnética va aumentando, también cambia su dirección de acción: cada vez se alinea más a la
fuerza eléctrica (que actúa en el eje Y ), frenando la partícula en esta dirección. Dado que entre
los instantes A y B la partícula desacelera en la dirección señalada, ésta se mueve barriendo
una suerte de arco = alargado”. En el punto B la fuerza magnética ha sido tal que se opone
justo a la fuerza eléctrica, y la partícula comienza a volver hacia y, z = 0 (instantes entre B y
C). A partir de este instante, el campo eléctrico es el que ahora intenta frenar a la partícula,
por lo que la rapidez disminuye y con ello la fuerza magnética, hasta llegar a C, instante en el
cual la partícula está en reposo, lista para un nuevo ciclo:
y
~
E

q
u

B
u

~
B

A

C

z

b

x

---

### Página 98

b) De la ley de Newton,


F~ = m~a = q E ̂ + ~v × B k̂






vx ′
B vy
 vy ′  = q  E − B vx 
m
vz ′


La última ecuación, vz ′ = 0 con z(0) = vz (0) = 0 nos dice que
z(t) ≡ 0

y el movimiento es en el plano. Si definimos ω = qB/m, entonces el sistema de 2 × 2 queda
como:
 


 ′  
0 ω
vx
vx
+
vy
ωE/B
−ω 0
vy ′

Notamos que el sistema es de la forma ~x ′ = A~x + f~, y podemos resolverlo mediante Variación
de Parámetros:
ˆ t
At
~x(t) = e ~x0 +
eA(t−s) f~(s) ds

De Álgebra Lineal, sabemos que:
At

e

=V



eλ1 t 0
0 eλ2 t



V −1

con V la matriz de vectores propios y λk los valores propios asociados. En este caso,




−i i
i 1
−1
λ1 = ω i , λ2 = −ω i , V =
, V =
1 1
2 −i 1
Por lo tanto,
At

e



eiωt + e−iωt −ieiωt + ie−iωt
ieiωt − ie−iωt
eiωt + e−iωt





cos ωt sin ωt
− sin ωt cos ωt



Como la velocidad inicial es nula, la solución homogénea es
 
~xh =
mientras que la solución particular es



ˆ 
ωE t sin ω(t − s)
E 1 − cos ωt
~xp =
ds =
sin ωt
cos ω(t − s)
B 0
B
Por tanto,



E
E
1 − cos ωt , vy (t) =
sin ωt
vx (t) =
B
B
He integrando para obtener la posición,


E 
E 
x(t) =
ωt − sin ωt , y(t) =
1 − cos ωt
ωB
ωB
que de Cálculo II sabemos que corresponde a la parametrización de una cicloide. Para mayor
información se sugiere visitar aquí. Notar que podemos escribir, haciendo R = E/ωB,

2 
2
x(t) − Rωt + y(t) − R = R2
que corresponde a un círculo cuyo centro se mueve con velocidad constante v = ωR en x.

---

### Página 99

(6) Un loop rectangular de masa despreciable, soportando una masa m, se mantiene verticalmente con
la parte superior en un campo magnético uniforme, como muestra la figura. El campo apunta hacia
dentro del papel. Suponga que la gravedad actúa uniformemente hacia abajo.

a) Encuentre la corriente I (magnitud y dirección de circulación) para la cual el loop mantiene a
la masa m sin que se mueva
b) Suponga que aumentamos la magnitud de la corriente, sin variar el sentido de circulación
anterior. Naturalmente, esperamos que el loop suba, llevando la masa consigo. Es correcto
afirmar entonces que se realiza trabajo para que la masa pueda subir. Una expresión de este
trabajo (errada) sería W = F~mag · ~h cuando m sube una altura h. Sin embargo, sabemos que
la fuerza magnética NO realiza trabajo. ¿Qué ocurre en este caso? ¿Quién realiza el trabajo?
c) Suponga ahora que al loop rectangular le cambiamos la forma arbitrariamente (segunda parte
de la figura). Muestre que la fuerza magnética sobre este loop es la misma que la obtenida en
el apartado inicial, sin importar la forma del loop.
a) La fuerza magnética que ejerce un campo sobre una corriente que circula sobre un tramo C es
ˆ
~
~
F = I d~r × B
C

Notemos que no todo el loop está dentro del campo. La fuerza sobre los segmentos verticales
se cancelan, así que solo aporta el segmento horizontal superior. Necesitamos que la fuerza sea
hacia arriba, para que se oponga al peso del cuerpo de masa m. Para ello, notemos que eso solo
se cumple si la corriente circula en sentido horario, en cuyo caso d~r va en dirección ı̂ (hacia la
~ va en dirección −k̂ (entra al papel) y por ende F~ va en dirección ̂ (hacia arriba).
derecha), B
Para este segmento tenemos
ˆ

F~ = IB
dr ̂ = IBa ̂
Necesitamos que esta fuerza sostenga al peso, por lo que
IBa = mg

I=

mg
Ba

---

### Página 100

b) Como la fuerza magnética jamás realiza trabajo, alguien o algo debe estar haciéndolo para
que efectivamente la energía potencial de la masa aumente.
Cuando el loop comienza a moverse, las cargas en los segmentos horizontales ya no se mueven
más de forma horizontal, ya que adquieren una componente vertical ~u asociada a la subida del
loop, por lo que su velocidad será ~v ′ . La fuerza magnética ya no apuntará directamente hacia
arriba, sino que apuntará diagonalmente hacia la izquierda. Si q = λ a denota la carga neta en
un segmento de largo a, evidentemente la componente horizontal de la fuerza magnética sería
quB = λ auB, que se opone al sentido de la corriente, frenando las cargas:

Lo que sea que mantiene la corriente estacionaria (una batería quizás) debe entonces EMPUJAR estas cargas para mantener la corriente estacionaria, para que no sean frenadas por esta
nueva fuerza horizontal. Si v denota la componente horizontal de la velocidad de las cargas,
entonces el trabajo hecho por el agente externo empujando las partículas es
W = Fhorizaontal d = λ auBvt = IaBut
donde d = vt es la distancia horizontal recorrida por las cargas en un instante t. Notemos que
I = λ v es la corriente. Finalmente, notemos que h = ut es la distancia vertical que recorren
las cargas (mientras sube el loop), por lo que el trabajo queda como sigue:
W = IaBh
que es la misma expresión que si se calculase usando un argumento físico erróneo, i.e. suponiendo que la fuerza magnética trabaja. ¿Quién hace trabajo? El agente externo, una batería,
o lo que sea que mantiene la corriente estacionaria en el tiempo.
c) La fuerza en un caso general viene dada por:
F~ =

ˆ
C



~ =I
I d~r × B

ˆ
C



~
d~r × B

en donde hemos sacado el campo por ser uniforme. Notemos que:
ˆ
d~r = ~rfinal − ~rinicial = ~a = a ı̂
C

según nuestro sistema. Luego la fuerza es la misma que la del inciso inicial, sin importar la
forma de la curva C.

---

### Página 101

(7) En un experimento diseñado para medir el campo magnético de la Tierra usando el efecto Hall, una
barra de cobre de 0.5 cm de espesor es posicionada a lo largo de un eje que va de este a oeste. Asuma
que la densidad de electrones es n = 8.46 × 1028 electrones por metro cúbico, y que el plano de la
barra es puesto perpendicular a la dirección del campo magnético de la Tierra. Si una corriente de
8 A en el conductor resulta en un voltaje de Hall de 5.1 × 10−12 V, ¿Cuál es la magnitud del campo
magnético terrestre en el lugar del experimento?
~ uniforme es aplicado perpenComo sabemos, el efecto Hall ocurre cuando un campo magnético B
dicularmente al plano de un cable plano por el que circula una corriente I. Este campo produce una
fuerza magnética sobre las cargas en movimiento, las cuales se desvían y acumulan en los bordes
del conductor (figura de abajo).

La figura muestra el caso real: los electrones (cargas negativas) son los portadores de corriente, y
por ende, quienes se ven afectados por el efecto Hall. El exceso de cargas en cada borde produce una
diferencia de potencial, y un consecuente campo eléctrico que apunta a lo ancho del conductor. Esta
desviación en la trayectoria de las cargas ocurre hasta que la fuerza eléctrica es capaz de oponerse
a la fuerza magnética. Notar del dibujo que la fuerza magnética y eléctrica se oponen (el campo
eléctrico apunta en una dirección, pero si las cargas son negativas, la fuerza apunta contraria al
campo). En dicho caso, si v representa la velocidad de los electrones, entonces el equilibrio requiere
que:
V
qv B = qE = qℓ V −→ v =
ℓB
en donde se usó que V = ℓE es la diferencia de potencial entre los bordes, y ℓ es el ancho. A esta
diferencia de potencial se le conoce como voltaje de Hall. Por otra parte, si I denota la corriente
que circula, entonces:
I = JA = Jℓw = ρvℓw = newvℓ
en donde n es el número de partículas por unidad de volumen, ρ = ne es la densidad de carga, y
J = ρv la densidad de corriente. Es posible entonces expresar el voltaje de Hall en función de la
corriente que circula,
new V
BI
−→ B =
V =
new
I
En este problema buscamos el valor del campo magnético de la Tierra, el cual apunta perpendicular a
nuestro conductor en el laboratorio. Es directo porque tenemos todos los datos numéricos. El campo

---

### Página 102

que mediremos será:
B=

8.46 × 1028 m−3 · 1.6 × 10−19 C · 0.5 × 10−2 m · 5.1 × 10−12 V
≈ 4 × 10−5 T
8A

(8) Un circuito cuadrado rígido, de lado L y masa M, está pivoteado en torno a uno de sus ejes en
~ uniforme, y el campo gravitatorio. El circuito lleva una corriente
presencia de un campo magnético B
I que es capaz de mantenerlo en equilibrio en un ángulo θ. Encuentre el sentido y magnitud de
dicha corriente:

Para el equilibrio, se requiere que el torque neto sobre la espira con respecto a algún punto de
aceleración nula sea cero. Se escoge como origen el punto O ubicado en una de las esquinas de la
espira, como se muestra en la figura.

Para el torque que ejerce el peso, usamos que la fuerza de gravedad se puede concentrar en el centro
de masa

---

### Página 103


MgL
L
sin θ ı̂ − cos θ ̂ × −Mg ̂ = −
sin θ k̂
~τ = ~r × F~ =
Por otro lado, el torque que ejerce la fuerza magnética es
~
~τ = ~µ × B
donde ~µ es el momento magnético de la espira,
~µ = IAn̂ = IL2 n̂
Requerimos en primer lugar que este torque tenga dirección k̂. Luego n̂ debe tener la dirección de
~µ en el dibujo

~ = IL2 B cos θ k̂
~τ = ~µ × B
El equilibrio exige entonces



L
Mg sin θ − IL B cos θ k̂ = ~0

Luego, la corriente I debe ser

Mg tan θ
2LB
La dirección debe ser acorde con la dirección del momento magnético, la cual se muestra en la
siguiente figura
I=

---

### Página 104

3.2.

Ley de Biot-Savart

(1) Un alambre delgado y rígido, que lleva una corriente I, es colocado a lo largo del eje X. Calcular
el campo magnético en el punto P . Analice el caso particular en que el alambre es simétrico con
respecto al eje Y . ¿Qué sucede cuando ℓ → ∞?

Recordemos la Ley de Biot-Savart:
~ r ) = µ0
B(~
4π

ˆ

~ × (~r − R)
~
I dR
~ 3
k~r − Rk

~ = dx ı̂ que lleva una corriente I en la dirección X. Por
Consideremos un elemento diferencial dR
otra parte, ~r = a ̂ y por tanto:
√
~ × (~r − R)
~ = aI dx k̂
~ = a ̂ − x ı̂ , k~r − Rk
~ = a2 + x2 , I dR
~r − R
Los límites de integración serán −x1 y x2 tales que x1 + x2 = ℓ y
a
a
x1 =
∧
x2 =
tan θ1
tan θ2
Por lo tanto,

~ ) = µ0 Ia
B(P
4π

ˆ x2

−x1

dx
(a2 + x2 )3/2

k̂

---

### Página 105

Usando el cambio de variable x = a tan θ,
ˆ
ˆ

µ0 I π/2−θ2
µ0 Ia arctan cot θ2 a sec2 θ dθ
µ0 I 
~
k̂
B(P ) =
cos
θ
dθ
k̂
cos
θ
+
cos
θ
2 k̂
4π − arctan cot θ1 a3 sec3 θ
4πa θ1 −π/2
4πa
recordando que sin (π/2 − t) = cos (t). En el caso simétrico, θ1 = θ2 y por tanto cos θk = p
y así,

ℓ/2
(ℓ/2)2 + a2

~ sim (P ) = µ0 I p ℓ
B
k̂
4πa ℓ2 /4 + a2

Si ℓ → ∞, entonces θk → 0 y por tanto:

~ ∞ (P ) = µ0 I k̂
B
2πa
Notemos que en este límite, el sistema posee simetría cilíndrica, y las líneas de campo magnético
son circulares. Este resultado se comprobará más adelante con la Ley de Ampère.
(2) Considere la espira de corriente formada por segmentos radiales y arcos de circunferencia como se
~ en el punto P .
muestra en la figura. Obtenga el campo magnético B

Si fijamos el origen en P , notamos inmediatamente que las contribuciones de los segmentos 1 y 5
~ es paralelo al vector ~r − R,
~ con ~x = ~0. Para el sector
son nulas, ya que en ambos casos el vector dR
2:
~r = ~0 ,

~ = b ρ̂ ,
R

~ = b dθ θ̂
dR

~ × (~r − R)
~ = b2 dθ k̂
dR

Por lo tanto,
~ 2 = µ0 I
B
4πb

ˆ φ

dθ k̂ =

µ0 φ I
k̂
4πb

De manera análoga, para el segmento 4 ,
~ 4 = − µ0 φ I k̂
B
4πa

∧

~ =b
k~r − Rk

---

### Página 106

Por último, para la sección 3 , es fácil notar que su contribución es nula, ya que en este caso el
~ apunta en la dirección contraria al vector unitario radial en coordenadas polares, y a
vector dR
~ apunta en la dirección radial, de esta forma, el producto cruz entrega al vector nulo.
su vez dR
Resumiendo, solo los segmentos pares contribuyen al campo en P , y el campo total será la suma
de ambas contribuciones:


µ0 φ I 1 1
~
~
~
B = B2 + B4 =
k̂
−
4π
b a
(3) Considere una espira circular que lleva corriente I en el sentido indicado por la figura. Calcule el
campo magnético a una distancia z en el eje de simetría de la espira.

En este caso,
~r
~
R
~
dR
~
k~r − Rk

z k̂
R ρ̂
R dθ θ̂
√
z 2 + R2

~ × (~r − R)
~ = zR dθ ρ̂ + R2 dθ k̂
dR
Como ρ̂ = cos θ ı̂ + sin θ ̂, entonces:
~ =
dB

µ0 I R2 k̂ + zR cos θ ı̂ + zR sin θ ̂
dθ
4π
(z 2 + R2 )3/2

Las integrales en el plano XY son nulas por estar integradas entre 0 y 2π, con lo que:
µ0 I
R2
~
B(z)
k̂
2 (R2 + z 2 )3/2

---

### Página 107

que es consistente con los argumentos de simetría.

(4) Considere un disco muy delgado que tiene una densidad de carga superficial σ uniformemente
distribuida. El disco se pone a girar a velocidad angular ω en torno a su eje. Encuentre el campo
magnético en el eje del disco.

Se tiene una distribución de carga en movimiento, y por tanto una corriente, de forma que ésta
generará un campo magnético. Anteriormente se determinó el campo en el eje de un anillo de radio
r con corriente I.
Podemos ver el disco como una superposición de anillos con corriente de ancho infinitesimal dr, de
modo que el campo magnético total será la suma de las contribuciones de estos anillos. Veamos que
ocurre en la porción de disco comprendida entre r y r + dr, con r ∈ [0, R]:

q = σ πr 2

dq = 2πσr dr

La carga dq da una vuelta completa en un tiempo
∆t =

2π
f
ω

---

### Página 108

La rotación del anillo genera una corriente:
dI =

dq
= σω r dr
∆t

Así, el campo magnético a una distancia z sobre el eje del disco generado por este anillo es:
µ0 σω
r3
µ dI
r2
dr
dB = 2
(r + z 2 )3/2 2
2 (r 2 + z 2 )3/2
El campo total es:
µ0 σω
~
B(z)

ˆ R

r3
dr k̂
(r 2 + z 2 )3/2

Haciendo el cambio de variables t2 = r 2 + z 2 , t dt = r dr obtenemos la siguiente integral:

ˆ
ˆ 2
ˆ 
ˆ
r2
t − z2
z2
z2
r3
dr
r
dr
t
dt
−
dt
t
+
+ c1
(r 2 + z 2 )3/2
(r 2 + z 2 )3/2
t3
t2
t
Volviendo a las variables originales,
ˆ R

r3
dr =
(r 2 + z 2 )3/2


√

z2 + r2 + √

Finalmente,
µ0 σω
~
B(z)



√

z2
z2 + r2

R

R2 + z 2 + √

√

R2 + z 2 + √

z2
− 2|z|
R2 + z 2



z2
− 2|z|
R2 + z 2

k̂

(5) Considere dos bobinas de N espiras de igual radio R, separados por una distancia 2b como muestra
la figura. En ambas bobinas circula una corriente I en el mismo sentido.

a) Obtenga el campo magnético en el punto medio P entre las dos bobinas, y muestre que en
este punto la primera derivada del campo es nula
b) Escoja una distancia 2b tal que la segunda derivada del campo se anule en P
c) Muestre que con la elección anterior, la tercera derivada se anula en P

---

### Página 109

a) De algún problema anterior, sabemos que para una espira circular con corriente I, radio R y
a una altura z de su centro, el campo en el eje de simetría es:
µ0 I
R2
~
B(z)
k̂
2 (z 2 + R2 )3/2
Como esta bobina consta de N espiras circulares, separadas por una distancia despreciable
con respecto a z, podemos utilizar el principio de superposición y obtener el campo resultante:
R2
µ0 I N
~
k̂
B(z)
2 (z 2 + R2 )3/2
Ahora, localicemos el origen en P . Sea un punto en el eje a una distancia z del origen; el campo
provocado por la bobina de abajo es:
R2
~ down (z) = µ0 I N
B
k̂
2 (R2 + (z + b)2 )3/2
mientras que la bobina de arriba contribuye con:
R2
~ up (z) = µ0 I N
k̂
B
2 (R2 + (z − b)2 )3/2
Así, el campo magnético total, por el principio de superposición, es:


R2
R2
µ0 I N
~
+
k̂ = B k̂
B(z) =
(R2 + (z − b)2 )3/2 (R2 + (z + b)2 )3/2
Si derivamos una vez,


dB
3µ0 I N 
=−

dz
2R



z+b

5/2 + 
5/2 
1 + ([z − b]/R)2
1 + ([z + b]/R)2
z−b

vemos que al evaluar en P –origen con z = 0– la derivada será:
dB
=0
dz z=0

b) Para escoger la distancia, vemos la segunda derivada. Derivando lo anterior,



2 !−5/2
2 !−5/2

z−b
dB
3µ0 I N 
z+b

1+
= −
+ 1+
dz
2R
R
R


2 !−7/2
2 !−7/2


z−b
z+b
5(z + b)
3µ0 I N  5(z − b)

1+
1+
+
+
2R
R
R
R
R

---

### Página 110

Evaluado en el origen,
" 
−5/2

−7/2 #
b2
b2
3µ0 I N
10b2
d2 B
2 1+ 2
(0) = −
− 2 1+ 2
dz 2
2R
R
R
R
Necesitamos que esta expresión sea nula. Imponer esto nos lleva a una ecuación que nos permite
despejar b como función de R:


b2
b2
2 1 + 2 = 10 2 −→ 2b = R
R
R
Esto significa que si escogemos la separación entre las bobinas igual al radio de las mismas,
entonces la segunda derivada también se anula en P .
c) Volviendo a la segunda derivada, reemplazando 2b = R y derivando por tercera vez, se ve que
en P la tercera derivada también es nula. Todos estos cálculos nos sirven para mostrar que el
campo en la vecindad de P es aproximadamente uniforme. En efecto, si expandimos en Taylor
el campo cerca del origen,
B(z) = B(0) + B ′ (0) z +

B ′′ (0) 2 B ′′′ (0) 3 B (iv) (0) 4
z +
z +
z + ...
2!
3!
4!

Reemplazando las derivadas antes calculadas,
B (iv) (0) 4
B(z) ≈ B(0) +
z
4!
Esta configuración se conoce como Helmholtz coils (bobinas de Helmholtz). El segundo término
es de orden de z 4 , lo cual es muy pequeño. Es por esto que el campo en la vecindad de P
resulta muy uniforme. La figura de abajo muestra el campo real dentro de las bobinas:

(6) Considere dos alambres, de longitud ℓ, paralelos separados por una distancia a ≪ ℓ y que llevan
corrientes I1 e I2 en la dirección y. Calcule la fuerza entre ambos conductores.
La fuerza magnética F~1 , que ejerce el alambre 2 sobre el alambre 1, se puede obtener como
ˆ
~
~2
F1 = I1 d~r1 × B

---

### Página 111

~ 2 es el campo magnético creado por el conductor 2. Usando el resultado del primer probledonde B
ma, para alambres suficientemente largos, las líneas del campo magnético debido a I2 son círculos
concéntricos con el alambre 2, con el campo apuntando en la dirección tangencial. Así, en un punto
arbitrario P sobre el alambre 1, tenemos
~ 2 = µ0 I2 k̂
B
2πa
Al ser este campo uniforme a lo largo del conductor 1, y siendo éste un alambre rectilíneo, la fuerza
que experimenta está dada por:


µ 0 ℓ I1 I2
µ 0 I2
~
~
~
k̂ =
ı̂
F1 = I1 ℓ × B2 = I1 ℓ ̂ ×
2πa
2πa
Claramente esta fuerza apunta hacia el conductor 2. Resulta evidente que F~2 = −F~1 . De esta
forma, dos cables paralelos que llevan corriente en la misma dirección se atraerán. Por otro lado, si
las corrientes fluyen en direcciones opuestas, la fuerza resultante será repulsiva.

---

### Página 112

(7) ¿Cuál debe ser la velocidad v (medida en un sistema inercial) de dos hilos paralelos muy largos y
no conductores, cargados uniformemente con densidad λ, y separados una distancia d, para que la
fuerza magnética anule la fuerza eléctrica ejercida entre los hilos?
Sabemos que el campo magnético generado por el cable es:
µ0 I
~
θ̂
B(r)
2πr
Con este campo es fácil calcular la fuerza que ejerce un cable sobre otro cable igual, con la misma
corriente, situado a una distancia d. El campo magnético que ejerce el primero sobre el segundo es
constante a lo largo de todo el segundo cable, debido a que depende solo de la distancia, y todos
los puntos del segundo cable están a la misma distancia, d. Así,

µ0 I L
F~m = ILB(d) k̂ × θ̂ = −
ρ̂
2πd
en donde L es el largo de cada cable. El signo negativo implica que la fuerza es atractiva. En el
caso de dos cables muy largos cargados que se mueven, evidentemente la corriente corresponde a
I = λv, en donde v es la velocidad del cable. La fuerza magnética entre dos cables cargados con
densidad de carga λ es entonces Fm = µ0 λ2 v 2 L/2πd. Por otra parte, el campo eléctrico que ejerce
una línea de carga muy larga es, usando la ley de Gauss,
λ
ρ̂
2πǫ0 r

~
E(r)

y claramente ese campo ejerce una fuerza repulsiva sobre otro cable exactamente igual situado a
una distancia d:
ˆ
λ2 L
~
~
Fe = λE(d)
dℓ =
ρ̂
2πǫ0 d
Para que la fuerza magnética anule la eléctrica tiene que ocurrir que:
µ 0 λ2 v 2 L
λ2 L
2πd
2πǫ0 d

v=√

=c
µ0 ǫ0

Evaluando numéricamente este resultado vemos que v ≈ 3 × 108 m/s, que es la velocidad de la
luz. Evidentemente los alambres nunca podrán viajar tan rápido, por lo que siempre predomina la
fuerza eléctrica por sobre la magnética.

3.3.

Ley de Ampère

(1) Considere un conductor cilíndrico de radio R y de extensión infinita, que lleva una corriente I con
una densidad de corriente no uniforme J = α r, donde α es una constante desconocida, y r es la
distancia de un punto interior en el conductor al eje de simetría. Encuentre el campo magnético en

---

### Página 113

todo el espacio.
La Ley de Ampère nos dice que
˛

~ · d~r = µ0 Ienc
B

γ

en donde Ienc representa la corriente encerrada por la curva cerrada γ. Esta ley es análoga a
la ley de Gauss de electrostática, y no depende de la forma de γ. Aunque esta ley siempre es
válida, no siempre es útil, y tal como ocurre con la ley de Gauss, se usa en situaciones de alta
simetría. Para aplicarla, es preciso saber en qué dirección debe apuntar el campo, de modo tal
que la integral de línea se simplifique considerablemente. Saber en qué dirección apunta el campo
magnético generalmente no es difícil, y solo requiere entender bien la naturaleza vectorial del mismo.
En particular, el campo siempre debe ser perpendicular a la corriente, y su sentido no debe depender
del sistema coordenado que se use.
Para una corriente que circula en la dirección z (coordenadas cilíndricas) es sencillo establecer en
qué dirección debe ir el campo. Primero, no puede tener una componente en la dirección z, porque el
campo no puede ser paralelo a la corriente. Por otra parte, si tuviera componente radial, cambiaría
el sentido de la misma si se invierte el sentido de la corriente. Pero invertir el sentido de la corriente
es, físicamente, lo mismo que escoger el eje z en la dirección opuesta a la inicial. Entonces se deduce
que la componente radial del campo depende de la elección del eje z, lo cual contradice el hecho de
que las magnitudes físicas no pueden depender de la elección de coordenadas. Por ende, tampoco
puede tener componente radial. Se concluye que el campo debe estar en la dirección tangencial, y
debe únicamente depender del radio por la simetría axial del problema
~ = B(r) θ̂
B
Sea γ una circunferencia de radio 0 < r < R, cuyo centro coincide con el eje de simetría del cilindro.
Así,
~r = r ρ̂ −→ d~r = r dθ θ̂
Con ello,
˛

~ · d~r = B(r)r
B

γ

En este caso,
Ienc (r) =

ˆ 2π ˆ r

De esta forma,

ˆ 2π

dθ = 2πr B(r) = µ0 Ienc

J(u)u du dθ = α

ˆ 2π

dθ

∧

Bin ∝ r 2

~ in (r) = µ0 α r θ̂
B

ˆ r

u2 du =

2πα r 3

Para el exterior, r > R, lo único que cambia es que ahora debemos considerar toda la corriente que
circula por el cable, que ya no depende del radio:
2πα R3
Ienc = I =

α=

3I
2πR3

---

### Página 114

Finalmente,

~ out (r) = µ0 I θ̂
B
2πr

∧

Bout ∝

r

(2) Calcule el campo magnético dentro de un solenoide ideal de largo ℓ, N vueltas y que lleva una
corriente estacionaria I.
Un solenoide es una bobina enrollada en forma helicoidal. La figura muestra las líneas de campo
magnético de un solenoide con corriente constante I:

Vemos que si las vueltas están muy cercanas espacialmente, el campo magnético resultante dentro
del solenoide es parcialmente uniforme, siempre que la longitud del solenoide sea mucho mas grande
que su diámetro. Para un solenoide ideal, que es infinitamente largo con vueltas infinitesimalmente
cercanas, el campo magnético dentro es uniforme y paralelo al eje x, utilizando la ley de la mano
derecha, y es nulo fuera del solenoide. Podemos utilizar la ley de Ampère para calcular el campo
magnético dentro de un solenoide ideal. Una vista transversal de un solenoide ideal se muestra en
la figura:

Consideremos el camino rectangular de largo ℓ y ancho w y en sentido contra-reloj. La integral de
línea del campo a través de este camino es
˛
˛
˛
˛
˛
~
~
~
~
~ · d~r
B · d~r = B · d~r + B · d~r + B · d~r + B


←

↓

→

↑

Ahora, la integral sobre ← es nula, ya que el campo es nulo en el exterior del solenoide. Las integrales
sobre ↑ y ↓ también son nulas, ya que el campo a lo largo de estas trayectorias es perpendicular a d~r.

---

### Página 115

Con esto, podemos estirar el camino cerrado de manera que encierre todo el solenoide,notando que
la corriente total que atraviesa la superficie encerrada por la trayectoria es NI, con N el número
de vueltas del solenoide
˛
~ · d~r = Bℓ = µ0 NI −→ B = µ0 NI
B
ℓ


(3) La figura muestra la sección transversal de un cable compuesto por dos cilindros concéntricos. Asuma
que una corriente I, de densidad constante, = sale de la página” por el cilindro central (r ≤ R1 ) y
~ en todo
“entra en la página” por el cilindro exterior (R2 ≤ r ≤ R3 ). Calcule el campo magnético B
el espacio.

La ley de Ampère nos dice que:
˛

~ · d~r = µ0 Ienc
B

C

~ = B θ̂ y por tanto:
En nuestro caso, por la simetría axial del problema, B
B=

µ0 Ienc
2πr

r < R1
I
J1 =
πR1 2

y con ello:
B1 =

Ienc = I
µ0 I r
2πR1 2

R1 < r < R2
B2 =

µ0 I
2π r



r
R1

2

---

### Página 116

R2 < r < R3
J2 = −

I
π(R3 − R2 2 )

y con ello:
µ0 I
B3 =
2π r



Ienc = I − I

R3 2 − r 2
R3 2 − R2 2

r 2 − R2 2
R3 2 − R2 2



r > R3
B4 = 0
(4) Un cable de radio R lleva una densidad de corriente J~ = J0 k̂. El cable tiene una cavidad cilíndrica
de radio α paralelo al eje del cable, a distancia b de él. Muestre que el campo magnético dentro de
la cavidad es uniforme.

Resolvemos el problema por superposición de dos corrientes, una del cilindro completo con densidad
de corriente J0 k̂, y otra en la cavidad con densidad −J0 k̂. El campo magnético al interior de un
cable con densidad de corriente J~ = J0 k̂ se puede obtener fácilmente con la ley de Ampère: Tomando
la curva circular de radio r, y dada la simetría cilíndrica de la distribución de corriente, el campo
magnético es constante y tangente sobre la curva. Así:
˛
¨
µ 0 J0 r
~
~ · d~r = B(r) 2πr = µ0 J~ · n̂ dS = µ0 J0 πr 2 −→ B(r)
B
θ̂
∂S

S

Sea entonces un punto arbitrario al interior de la cavidad, como muestra la figura:

---

### Página 117

~rk = rk ρ̂k ,
Por superposición,

k = {1, 2}

~ ) = µ0 J0 r1 θ̂ 1 − µ0 J0 r2 θ̂ 2
B(P

pero
θ̂ 1 = k̂ × ρ̂1

∧

θ̂ 2 = k̂ × ρ̂2

y por tanto,
 µJ

 µJ
µ 0 J0 
0 0
0 0
~
B(P ) =
r1 k̂ × ρ̂1 − r2 k̂ × ρ̂2 =
k̂ × ~r1 − ~r2 =
k̂ × ~b
el cual es un campo uniforme.

(5) Se tiene dos corrientes, ambas con igual sentido (en el dibujo, saliendo de la hoja). Una de ellas
circula por el plano infinito y tiene
Js , y la otra es una corriente cilíndrica infinitamente
 magnitud
r
larga cuya densidad es J = J0 1 −
. Se define al punto P como el punto ubicado a distancia
R
R/2 bajo el centro del cilindro, por el eje de simetría que es perpendicular al plano:

a) Encuentre el campo magnético, en P , generado por Js
b) Encuentre el campo magnético, en P , generado por J

---

### Página 118

c) Encuentre el valor de J0 (Js ), que hace que el campo magnético resultante en el punto P sea
nulo
a) Podemos pensar la región de corriente como una superposición de conductores paralelos que
llevan corrientes en la dirección ı̂:

Primero analizamos en qué dirección debiese ir el campo. ¿Puede el campo tener componente
en x? No, porque el campo no puede ser paralelo a la dirección de la corriente que lo genera.
¿Puede tener componente en z? Otra vez no. Si suponemos que la superficie se compone de
muchos hilos delgados, como muestra la figura, la componente z de la contribución al campo,
generada por uno de estos hilos ubicado en y > 0, se cancela con su hilo opuesto en y < 0. Por
ello es que no puede tener componente z. Por tanto,
~ = ± B ̂
B
donde el signo dependerá si estamos sobre o bajo la región, donde el sentido vendrá dado por la
regla de la mano derecha. Ahora, podemos utilizar la ley de Ampère para encontrar el campo
magnético debido a esta distribución de corriente. Tomaremos la curva cerrada que aparece en
la figura. La corriente que atraviesa la superficie limitada dicha curva es:
IC = Js bℓ
Notando que, en la integral de línea, los segmentos verticales no contribuyen (d~r perpendicular
al campo)
˛
~ · d~r = B 2ℓ = µ0 IC = µ0 Js bℓ −→ B = µ0 Js b
B
C

Así,

~ ) = − µ0 Js b ̂
B(P

b) Para el cilindro, utilizamos nuevamente la ley de Ampère. Dada su extensión infinita, por
simetría, el campo magnético en su interior debe ser función únicamente de la coordenada

---

### Página 119

radial, y su dirección es tal que es tangente en todo punto a una curva circular concéntrica al
cilindro:

 2

˛
ˆ 2π ˆ r 
r
r3
t
~
B · d~r = 2πr B(r) = µ0 Ienc = µ0
t dt = 2πµ0 J0
dθ
−
J0 1 −
R
3R
C

Así,
~
B(r)
= µ 0 J0



r2
r
−
2 3R



θ̂

~ ) = µ 0 J0
B(P



R
R2
−
12R



̂ =

µ 0 J0 R
̂

c) En el punto P , se tendrá la superposición de ambos campos:


µ 0 J0 R µ 0 Js b
~
Bres (P ) =
̂
−
Para tener un campo magnético nulo, debe tenerse entonces:
J0

R
bJs

J0 =

3bJs
R

~ = K ı̂.
(6) Considere un plano infinito por el que circula una corriente superficial uniforme K
a) Encuentre el campo magnético en todo el espacio. Para ello, realice un análisis que permita
saber a priori en qué dirección debe apuntar el campo.
b) Calcule el flujo magnético a través del manto de un cono de altura h y radio basal R, situado
en la región sobre el plano del inciso anterior, con su eje perpendicular al mismo.
c) Obtenga la fuerza magnética por unidad de área que el plano del inciso (a) ejerce sobre otro
plano paralelo situado a una distancia d del primero, por el que circula la misma corriente
~ = K ı̂.
K
a) Con un análisis idéntico al problema anterior, es posible probar que el campo es:


 − µ0 K ̂ z > 0
~ =
B
µK

 + 0 ̂ z < 0

El campo magnético ejercido por este plano resulta uniforme. Note que el campo posee un
salto de discontinuidad de µ0 J entre la región bajo y sobre el plano. La analogía con el campo
eléctrico ejercido por un plano infinito cargado es total.

b) Un hecho experimental muy importante es que, hasta ahora, no existen los monopolos
magnéticos. Por ejemplo, no podemos separar un imán en un polo norte y un polo sur. Si
rompemos un imán a la mitad, cada pedazo se transformará = misteriosamente” en un nuevo
imán, con polo norte y polo sur. Como no podemos encontrar monopolos magnéticos, no es

---

### Página 120

posible encontrar líneas de campo magnético abiertas. Las líneas siempre serán cerradas, o
bien, comenzarán y terminarán en el infinito. Consecuencia de esto es que, a través de una
superficie cerrada, siempre el flujo magnético es cero, porque toda línea que entra debe salir,
por ser cerrada. Así,
˛
~ · n̂ dS = 0
B
S

Esta ecuación es la ley de Gauss del magnetismo. Si en cambio se pudiera encontrar un monopolo
magnético, las líneas comenzarán o terminarán en una suerte de = carga magnética” qm , análogo
al flujo eléctrico. En ese caso, las líneas ya no serán cerradas, y se obtendría una ley de Gauss
del tipo
˛
~ · n̂ dS = k qm
B
S

Sin embargo, este hecho nunca ha sido confirmado experimentalmente; así que asumimos que
el flujo magnético sobre una superficie cerrada siempre es cero. Basados en este hecho, consideremos un cono sobre el plano del inciso (a). Si lo ponemos con el eje perpendicular al plano,
~ El flujo neto,
entonces claramente no hay flujo a través de la base. Esto porque ahí n̂ ⊥ B.
que tiene que ser siempre cero, queda
˛
˛
˛
~
~
~ · n̂ dS
0=
B · n̂ dS +
B · n̂ dS =
B
tapa

manto

manto

de donde se concluye que el flujo a través de manto es, por sí solo, igual a cero.
~ ejerce sobre una línea de corriente,
c) Análogamente a la fuerza que un campo magnético B
´
~ es posible decir que la fuerza magnética que este mismo campo ejerce sobre
F~ = C Id~r × B,
~ y volumétricas J~ es:
corrientes superficiales K
¨
¨
~
~
~
~
~ dV
F =
K × B dS
∧
F =
J~ × B
S

V

~ es la fuerza por unidad de largo, K
~ ×B
~ representa la
luego deducimos que, así como Id~r × B
~ es la fuerza por unidad de volumen sobre V .
fuerza por unidad de superficie sobre S y J~ × B
En nuestro problema, nos interesa la fuerza magnética por unidad de superficie sobre un plano
~ = K ı̂. Si este plano se encuentra sobre el plano del
infinito por el que circula una corriente K
~ = − µ0 K ̂ y la fuerza por unidad de area es:
inciso (a), entonces el campo que siente es B

~ ×B
~ = − µ0 K ı̂ × ̂ = − µ0 K k̂
f~m = K
Note el signo negativo. Esto indica que la fuerza apunta hacia abajo, por lo que se concluye
que dicha fuerza es atractiva. Si, por el contrario, la corriente de los planos corriera en sentidos opuestos, la fuerza sería repulsiva, análogamente a la fuerza magnética entre dos hilos
conductores rectos por los que pasa corriente.

---

### Página 121

4.

Campos variables en el tiempo

4.1.

Ley de inducción de Faraday-Lenz

(1) Este es un problema meramente cualitativo. Si los imanes se mueven de la forma descrita en la
figura, determine la dirección de la corriente inducida en cada una de las espiras.

Recordemos la Ley de Lenz:
Una f.e.m inducida siempre generará una corriente cuyo campo magnético se oponga
al cambio original en el flujo magnético.

En el caso de la izquierda, el movimiento del imán tiende a aumentar el flujo magnético, por lo que
se generará una corriente que cree un campo magnético que se oponga a este hecho. Para reducir
~ que apunte fuera de la espira y, por la
el flujo magnético, debe aparecer un campo magnético B
regla de la mano derecha, la corriente circulará en dirección anti-horaria.
En el caso de la derecha, el flujo disminuye; por tanto, se deberá generar un campo magnético que
entre a la espira, de modo tal que se oponga a la reducción de flujo. De esta forma, la corriente
circulante tendrá dirección horaria.
Finalmente,

~ = Bı̂.
(2) La espira rectangular de la figura se encuentra sumergida en un campo magnético uniforme B
Si la espira gira con velocidad angular ω utilizando el eje z como eje de rotación, y asumiendo que
en t = 0 la espira se encuentra en el plano Y Z, determine la fem inducida y la corriente inducida
en la espira.

---

### Página 122

Calculamos en flujo magnético, considerando que n̂ = −θ̂,
¨
Φ = − B ı̂ · θ̂ dS = BS sin θ −→

dθ
dΦ
= BS cos θ
dt
dt



Notemos que

dθ
=ω
dt

θ = ωt + θ0

Dada la condición inicial, es claro que θ0 = π/2. A partir de la ley de inducción de Faraday, podemos
obtener la magnitud de la fem inducida en la espira:
ε=−

dΦ
= −Bωab cos (ωt + π/2)
dt

La magnitud de la corriente es, simplemente
I=

|ε|
Bωab
cos (ωt + π/2)
R
R

(3) Considere el experimento del siguiente video: Si coloca un solenoide alrededor de un núcleo de hierro
(el hierro es solo para reforzar el campo magnético) y coloca un anillo metálico en él, al prender la
fuente de voltaje, el anillo saltará varios metros en el aire ¿Por qué? Si repite el experimento con
un anillo con un corte a todo lo alto del anillo, éste no se elevará. ¿Por qué?

---

### Página 123

Antes que circule corriente, el flujo a través del anillo es cero. Después de encender el aparato,
aparece un flujo (hacia arriba en la figura) y la fem generada en el anillo hará circular una corriente
(en el anillo) que, de acuerdo con la Ley de Lenz, será en dirección tal que el campo magnético
generado tienda a anular el nuevo flujo. Esto significa que que la corriente circulará en sentido
opuesto a la corriente en el solenoide. Corrientes opuestas se repelen, y el anillo saltará.
En el segundo caso, el anillo está cortado y no permite que circule una corriente por el perímetro,
y por tanto el efecto antes descrito no se generará.
(4) Considere un loop circular conductor de diámetro D, masa M y resistencia R que cae por acción
de la gravedad desde una gran altura h, en una región en donde existe un campo magnético no
uniforme con componente Bz = B0 (1+kz), siendo z la altura respecto del suelo y k alguna constante.
Suponga que el plano del loop se mantiene horizontal en toda la caída. Ignore efectos de roce con
el aire.
a) Explique por qué se induce una corriente en el loop. Calcule su magnitud e indique su sentido.
b) Describa cualitativamente la caída del loop. ¿Cuál es la velocidad terminal del mismo?
~ = Bx ı̂ +
a) En la región en donde se encuentra el loop circular, existe un campo magnético B
By ̂ + Bz k̂, cuyas componentes x e y no son nulas. Esto se puede deducir notando que, si
el campo solo tuviese la componente z señalada en el enunciado, su divergencia claramente
no es nula, contradiciendo lo que se sabe de los campos magnéticos físicamente plausibles. No
obstante, si imponemos que el loop se mantiene horizontal toda la caída, solo la componente
vertical Bz será relevante en el calculo del flujo magnético a través del área que encierra el
mismo. Por otra parte, ya que esta componente no es uniforme, dependerá del tiempo, y lo
mismo ocurrirá con el flujo magnético. Por la ley de Lenz, una variación en el flujo magnético
induce una fem en el circuito:


˛
¨
~ · d~r = ε = − ΦB = − d  B
~ · n̂ dS 
E
dt
dt
C

S

Es MUY IMPORTANTE entender la convención que se usa para el sentido en que se recorre
la integral de línea. La convención es simple: regla de mano derecha, la misma de Cálculo en
Varias Variables:

---

### Página 124

Veamos este problema. El flujo a través del loop que cae horizontalmente, es debido solo a la
componente vertical, por lo que tomando el vector n̂ = k̂, obtenemos:
¨
¨
¨
~
ΦB =
B · n̂ dS =
Bz dS = Bz dS = B0 (1 + kz)A
S

S

S

en donde hemos usado que la componente normal, al depender solo de la altura z, es constante
sobre toda la superficie, la cual se encuentra horizontal, así que sale de la integral. En este
caso, A es el área de la espira. La variación en este flujo es:
dΦB
dz
= B0 kA
dt
dt
y vemos que no es nulo. Notemos que z ′ es la velocidad con que cae el loop, y dado que escogimos
el eje z hacia arriba, esta velocidad resulta negativa (la coordenada z del loop disminuye en el
tiempo). Por Lenz, la fem inducida en la espira es:
ε=−

dΦB
= −B0 kA z ′
dt

un valor positivo cuando k > 0. Por nuestra convención, entonces vemos que la corriente
fluye en el mismo sentido en que se recorre C, tal que n̂ = k̂: anti-horario visto desde la parte
superior del loop. Su módulo es evidentemente
I=

|ε|
B0 kA z ′ (t)
=−
R
R

~ =B
~ k +B
~z,
b) Haremos esto un poco explícito. Podemos descomponer el campo magnético como B
en donde Bk es la componente que vive en el plano XY . Al circular una corriente, el campo
ejerce una fuerza magnética sobre el loop, dada por:
˛
~
~
F =
I d~r × B
= I

˛

~k +
d~r × B

˛

~z
d~r × B



˛
˛
~


d~r × Bz + I (dx ı̂ + dy ̂) × (Bx ı̂ + By ̂)
= I


˛
= I  By dx − Bx dy  k̂

Recordemos que no conocemos la forma de las otras componentes del campo magnético, pero
aun así, podemos deducir que la fuerza neta apunta en la dirección z es F~B = I(t)η k̂, en donde
η la integral de línea.
El desarrollo anterior nos convence de que sobre el anillo, además de actuar la fuerza de
gravedad, actúa una fuerza que resulta ser proporcional a la corriente, y por ende, proporcional
a la velocidad con que cae el anillo. Cualitativamente, esperamos que esta fuerza proporcional

---

### Página 125

aumente conforme aumenta la rapidez con que cae el loop. La fuerza magnética aumentará hasta
que llegue a ser igual al peso del cuerpo, una fuerza siempre constante. En ese momento la
aceleración del loop será cero, y el mismo caerá con velocidad constante. Este es un movimiento
totalmente análogo a un cuerpo que cae con roce en el aire. La velocidad final con que termina
moviéndose el objeto, se conoce como velocidad terminal. Aceptando toda esta descripción del
movimiento, es posible obtener la velocidad terminal al menos de dos formas distintas:
Cuando el loop caiga con velocidad igual a la terminal, su aceleración será nula. En este
estado, la fuerza magnética será igual al peso,
Iterm η =

B0 Akvterm
η = Mg
R

en donde Iterm es la corriente terminal (constante) que circula por el loop. En principio,
para calcular η necesitamos explícitamente las componentes Bx , By de campo magnético
para evaluar la integral; sin embargo, no las conocemos. No obstante, hay una manera
astuta de calcular esta integral de todas formas: usando el Teorema de Green,
˛
¨
∂Bx ∂By
η = By dx − Bx dy = −
+
dS
∂x
∂y
pero
~ =0
∇·B

∂Bx ∂By
∂Bz
+
=−
∂x
∂y
∂z

Así:
η = B0 k

¨

dS = B0 kA

Por ende, la velocidad terminal resulta ser
vterm =

MgR
B0 2 A2 k 2

Cuando el loop cae, la variación en la energía potencial gravitatoria se compensa con la
energía disipada por efecto Joule en el loop. Si en un intervalo ∆t ha caído una distancia
∆h, entonces
Mg∆h = I 2 R∆t
∆h
pero si la velocidad es constante en el tramo, entonces v =
. Aplicando esto a cuando
∆t
el loop se mueva con velocidad terminal,
Iterm 2 R = Mgvterm
Reemplazando la corriente Iterm =

B0 Akvterm
,
R
vterm =

MgR
B0 2 A2 k 2

---

### Página 126

(5) Una barra conductora de masa m desliza entre 2 rieles conductores, sin fricción, que forman un
ángulo θ con la horizontal, están separados una distancia ℓ y unidos por una resistencia R. Un
~ es aplicado verticalmente. La barra se suelta del reposo y desliza
campo magnético uniforme B
hacia abajo.

a) Determine la corriente inducida en la barra. ¿En qué dirección fluye, de a hacia b o de b hacia
a?
b) Calcule la velocidad terminal de la barra.
c) Una vez alcanzada la velocidad terminal, ¿Cuál es la corriente inducida?
d ) ¿A qué tasa se disipa energía en la resistencia?
e) ¿Cuál es la tasa de variación de trabajo por unidad de tiempo asociada a la gravedad?
a) Antes que todo, coloquemos el eje de forma usual, y no sobre el plano inclinado. Supongamos
que, en un instante dado, la barra se encuentra a una distancia x del extremo, como se ve en
la figura:

El circuito formado por los rieles y la barra que desliza encierra una superficie plana cuya
normal es:
n̂ = sin θ ı̂ + cos θ ̂
y el flujo a través de esta espira es:
ΦB =

¨

~ · n̂ dS = Bxℓ cos θ
B



Con esto, la fem inducida en los extremos de la barra es:
ε=−

dx
dΦB
= −Bℓ cos θ
dt
dt

---

### Página 127

Así, la corriente inducida será
Bℓ
dx
|ε|
cos θ
R
R
dt
La dirección se ve de la siguiente forma: el flujo está aumentando, por lo que se requiere inducir
una corriente tal que su campo magnético apunte hacia abajo y se contraponga al cambio en
el flujo. de esta forma, por la regla de la mano derecha, la corriente debe circular en dirección
b → a.
I=

b) La fuerza magnética que ejerce el campo sobre la barra es:
~ ×B
~ = Iℓ k̂ × B ̂ = −BIℓ ı̂
F~m = I L
La fuerza de gravedad viene dada por:
F~g = −mg ̂
Haciendo suma de fuerzas en el eje x (proyectando paralelamente sobre la superficie):
mx′′ = mg sin θ − BIℓ cos θ = mg sin θ −

B 2 ℓ2
cos2 θx′
R

v′ = α − β v
con v = x′ , α = g sin θ y β = B 2 ℓ2 cos2 θ/mR. Resolviendo,
dv
dt =
α−β

t − t0 =

ˆ v





ln (a − β v) ln (a − β v0 )
ds
=−
+
β
β
v0 α − β s

como t0 = 0, v0 = 0:
βv
−β t = ln 1 −
α

Por tanto,
vt = lím v(t) =
t→∞


α
−β t
v(t) =
1−e
β

α
mgR sin θ
= 2 2
β
B ℓ cos2 θ

c) La corriente terminal es:
It =

mg tan θ
Bℓ
cos θ vt =
R
Bℓ

d ) El módulo de la fem inducida en este caso es:
|εt | =

mgR tan θ
Bℓ

Por tanto, la potencia disipada es:
m2 g 2 R tan2 θ
Pelec = |εt |It =
B 2 ℓ2

---

### Página 128

e) La potencia asociada a la gravedad es:
Pgrav = Wk vt =

m2 g 2 R tan2 θ
B 2 ℓ2

con Wk = mg sin θ la componente del peso en la dirección de desplazamiento. Vemos que el
valor de esta potencia es la misma que la potencia que disipa la resistencia. Esto se debe al
principio de conservación de la energía.
(6) Note la similitud entre la ley de Ampère
˛

~ · d~r = µ0 I
B

C

y la ley de Faraday-Lenz
˛

~ · d~r = − dΦB
E
dt

C

Nada nos impide aplicar los métodos de = anillos amperianos” al cálculo de campos eléctricos generados por campos magnéticos variables, de forma análoga al cálculo de campos magnéticos producidos
por corrientes estacionarias. Suponga un solenoide largo y recto, de radio a y con n vueltas por
unidad de largo, por el que circula una corriente I(t). Si la corriente varía en el tiempo, encuentre
el campo eléctrico que se induce dentro y fuera del solenoide.
Como ya calculamos previamente, el campo magnético producido por el solenoide recto es:

µ0 nI(t) k̂ r < a
~
B=
~0
r>a
en donde hemos usado coordenadas cilíndricas, siendo el eje z coincidente con el eje del solenoide.
Supongamos un loop circular de radio r < a como muestra la figura. El flujo magnético encerrado
por ese loop es

---

### Página 129

ΦB = B(t)πr 2 = µ0 πr 2 nI(t)
y la variación de flujo queda como
dΦB
˙
= Ḃ(t)πr 2 = µ0 πr 2 nI(t)
dt
Por la ley de Faraday-Lenz,
˛

~ · d~r = −Ḃ(t)πr 2 = −µ0 πr 2 nI(t)
˙
E

Dado que el campo magnético es paralelo al eje z, el campo eléctrico inducido será perpendicular
~ = E θ̂. Para una descripción más detallada de este
a éste, en la dirección tangencial, por lo que E
argumento, revisar el inicio del problema siguiente. Así, la fem inducida será
˛
˛
~
ε = E · d~r = E θ̂ · dr θ̂ = 2πr E(r)
y por ende

˙
2π E(r) = −µ0 πr 2 nI(t)

Con ello,

˙ θ̂
~ in = − µ0 nr I(t)
E

Este es el campo dentro del solenoide. El campo fuera se obtiene de forma análoga, pero el loop
ahora encierra todo el solenoide. El flujo es
ΦB = B(t)πa2 = µ0 nπa2 I(t)
Por la ley de Faraday-Lenz,
Y finalmente:

dΦB
˙
= µ0 nπa2 I(t)
dt

˙
2πr E(r) = −µ0 nπa2 I(t)

~ out = − µ0 na I˙ θ̂
E
2r

lo cual concluye el problema.

(7) Un cable recto infinitamente largo porta una corriente con pequeñas perturbaciones I(t). Determine
el campo eléctrico inducido, en función de la distancia s desde el cable. Hint: use el anillo amperiano
de la figura.

---

### Página 130

Primero que todo, de la ley de Faraday en su forma diferencial, es posible concluir que el campo
~ –dado que, en este caso, al derivar no cambio en la dirección
eléctrico inducido circulará en torno a B
del campo– de manera análoga al caso de un hilo de corriente y la ley de Ampère:

Así, de manera análoga a lo que ocurre en un solenoide al calcular el campo magnético, el campo
eléctrico inducido será paralelo al eje. En la aproximación cuasiestática, el campo magnético tiene
magnitud µ0 I/2πs y circula alrededor del cable. Para el anillo amperiano de la figura,
˛
¨
d
~
~ · n̂ dS
E · d~r = E(s0 )ℓ − E(s)ℓ = −
B
dt
ˆ
µ0 ℓ dI
µ0 ℓ dI s ds′
−
(ln s − ln s0 )
= −
2π dt s0 s′
2π dt
Por tanto,
~
E(s)



µ0 dI
ln s + K
2π dt



k̂

donde K es una constante (independiente de s, pero podría depender de t). El resultado anterior
implica que E diverge cuando s → ∞. Esto no puede ser cierto... ¿Qué está incorrecto? Respuesta: Hemos sobrepasado los límites de la aproximación cuasiestática. Como veremos en el capítulo
final, las = noticias” electromagnéticas se propagan a la velocidad de la luz, y a largas distancias
~ depende no de la corriente ahora, sino de la corriente que era en un tiempo anterior. Si τ es el
B
tiempo que le toma a I cambiar sustancialmente, entonces la aproximación cuasiestática debe ser
correcta solo para
s ≪ cτ
y nuestra solución no es válida para valores grandes de s.

4.2.
(1)

Inductancia. Circuitos RL, LC y RLC
a) Considere dos circuitos circulares de radios a y b ≫ a separados una distancia z, como muestra
la figura. Los centros de ambos circuitos se encuentran sobre el eje z y el plano del circuito
menor está inclinado en un ángulo α. Este mismo circuito tiene resistencia R. ¿Cuál es la
inductancia mutua del sistema?

---

### Página 131

b) Considere dos espiras coplanares y concéntricas, de radios R1 y R2 ≪ R1 . Encuentre la inductancia mutua entre ambas espiras.

Como sabemos, la inductancia mutua se define como
M=

Φ12
I1

en donde Φ12 es el flujo a través de la espira 2, del campo magnético producido por la corriente I1
en la espira 1 (ver figura abajo).

Es posible demostrar que la inductancia mutua es la misma si se invierten los roles del loop 1 y el
loop 2, por lo que
Φ21
Φ12
M=
I1
I2
Es por esto que para calcular la inductancia mutua podemos escoger uno u otro flujo. Evidentemente, siempre se escoge el flujo cuyo cálculo sea el más simple.

---

### Página 132

a) En este caso, podemos suponer que el anillo menor, al ser de radio mucho más pequeño,
se encuentra contenido en un punto z sobre el eje vertical. Por ser ínfimo, el campo que lo
atraviesa (producido por el anillo mayor) es, en esencia, uniforme e igual al visto en problemas
anteriores:

−3/2
µ0 I
z2
~
B=
1+ 2
k̂
2b
b
en donde hemos supuesto que por el anillo mayor circula una corriente I. El flujo a través del
anillo menor es, entonces,
Φ=

¨
S

~ · n̂ dS =
B

¨

B cos α dS = B cos α

S

¨

µ0 IS cos α
dS =
2b

S


−3/2
z2
1+ 2
b

~ ·n̂dS = B cos αdS. Dividiendo
con S = πa2 el área de la espira menor. Aquí hemos usado que B
por la corriente, obtenemos la inductancia mutua,
µ0 πa2 cos α
M=
2b



z2
1+ 2
b

−3/2

b) Este es un caso particular del anterior, con α = 0 y z = 0. Por tanto,
M=

µ0 πR2 2
2R1

(2) Considere un toroide de N vueltas y de sección rectangular de lado h, radio interior a y radio
exterior b.

a) Calcule la autoinductancia y discuta qué ocurre cuando a ≫ b − a
b) Calcule la energía magnética almacenada en el toroide

a) Utilizando la ley de Ampère, el campo magnético dentro del toroide se obtiene como
˛
~ · d~r = 2πr B = µ0 NI −→ B = µ0 NI
B
2πr

---

### Página 133

donde se ha integrado el campo sobre una circunferencia de radio r ubicada en el centro del
toroide. El flujo magnético sobre una vuelta del toroide se puede obtener al integrar sobre
todas las secciones rectangulares, con dS = h dr como elemento diferencial de área:
¨
ˆ b
µ0 NI
µ0 NIh
una vuelta
~ · n̂ dS = h
ΦB
B
dr =
ln (b/a)
2πr
2π
a


y el flojo total sobre el toroide será ΦB = N ΦB una vuelta . Con esto, la autoinductancia será
L=
Cuando a ≫ b − a, te tiene que

ΦB
µ0 N 2 h
ln (b/a)
I
2π




Llim =

µ0 N 2 h b − a
2π
a

b−a
ln (b/a) = ln 1 +
a
y la inductancia sería

≈

b−a
a

Recordando que el área de un solenoide es S = h(b − a),
Llim =

µ0 N 2 S
2πa

y con ℓ = 2πa,

µ0 N 2 S
ℓ
que es, justamente, la autoinductancia de un solenoide.
Llim =

b) La energía almacenada en el toroide es simplemente
U=

LI 2
µ0 N 2 I 2 h
ln (b/a)
4π

(3) Considere el siguiente circuito LC. Suponga que el condensador tiene una carga inicial Q0 . En t = 0,
el interruptor se cierra.

C

L

Q0

a) Encuentre la ecuación diferencial para la carga en el condensador mediante consideraciones
energéticas.

---

### Página 134

b) Utilizando las leyes de Kirchhoff, encuentre I(t) y Q(t)
a) En ausencia de una resistencia, la energía total se transforma constantemente en energía
eléctrica y magnética, fenómeno conocido como oscilación electromagnética. Le energía total
del circuito LC en un instante arbitrario es
L I2
Q2
+
2C

Etotal = U = UC + UL =
Por el principio de conservación de la energía,


dU
d Q2
L I2
=0
+
dt
dt 2 C

Q dQ
dI
+ LI
=0
C dt
dt

Además, hay que notar que: Para ver la relación entre carga del condensador y corriente por
la inductancia, hagamos el siguiente análisis:
Si la corriente por la inductancia es positiva, y circula positivamente, entonces significa
que el condensador se descarga. Por tanto,
I =−

dQ
dt

Si la corriente por la inductancia es negativa, entonces circula en la otra dirección y por
tanto está cargando al condensador. Así,
I =−

dQ
dt

Por tanto:

dI
Q
d2 Q
Q
I + LI
= 0 −→
+L 2 =0
C
dt
C
dt
que es la ecuación diferencial para la carga en el condensador.
−

b) Utilizando la ley de voltajes de Kirchhoff,

C

+

+

-

-

L

dI
Q
+L
=0
C
dt
Aquí nuevamente usamos la relación entre variación de carga y corriente. Por tanto,
−VC + VL = −

Q
d2 Q
+L 2 =0
C
dt

Q′′ +

Q=0
LC

---

### Página 135

que posee por solución general
Q(t) = Q0 cos (ωt + φ)
donde la frecuencia angular ω está dada por
ω=√

LC

La corriente por la inductancia es
I(t) = −

dQ
= ωQ0 sin (ωt + φ) = I0 sin (ωt + φ)
dt

con I0 = ωQ0 . De las condiciones iniciales Q(0) = Q0 e I(0) = 0, la fase es simplemente φ ≡ 0.
Con esto, las soluciones para la carga y la corriente en el circuito LC son:
Q(t) = Q0 cos (ωt)

∧

I(t) = I0 sin (ωt)

Notar que, con U = UC + UL , se cumple que:
Q0 2
LI0 2
Q0 2
Q0 2
Q0 2
Q2 (t) LI 2 (t)
+
cos (ωt) +
sin (ωt) =
cos (ωt) +
sin (ωt) =
U=
2C
2C
2C
2C
2C
(4) Considere el circuito RLC en serie, que consta de una resistencia, una inductancia, y un condensador:

C

L
R

Mediante consideraciones energéticas, encuentre la ecuación diferencial para la carga en el condensador.
La energía, en un instante arbitrario t, está dada por
U = UC + UL =

LI 2
Q2
+
2C

A diferencia del circuito LC, parte de la energía del circuito será disipada por la resistencia. Esto
es, la tasa a la cual la energía es disipada es
dU
= −I 2 R
dt

---

### Página 136

donde el signo negativo implica que la energía total disminuye en el tiempo. Así,
dU
Q dQ
dI
+ LI
= −I 2 R
dt
C dt
dt
Nuevamente Q̇ = −I, y con ello
dI
Q
= −I 2 R
− I + LI
C
dt

−

Q
dI
+ L = −IR
C
dt

−

Q
d2 Q
dQ
−L 2 =R
C
dt
dt

Finalmente, la EDO para la carga es:
L

dQ Q
d2 Q
+R
+ =0
dt
dt
C

(5) En la figura, el interruptor se cierra en t < 0 y se establece una condición de estado estable. El
interruptor se abre después en t = 0.
R1
a
R2

ε

L
+
−

b

a) ¿Cuál es la energía almacenada en la bobina justo antes de abrir el interruptor?
b) Encuentre la diferencia de potencial en la bobina justo después de abrir el interruptor. ¿Cuál
extremo de la bobina está a mayor potencial, a o b?
c) Realice gráficas a mano de las corrientes en las resistencias, como funciones del tiempo. Muestre
valores antes y después de t = 0.
d ) ¿Cuánto tiempo después de t = 0 la corriente en R2 es i?
a) Cuando se ha alcanzado un equilibrio estable, la corriente en un circuito LR ya no varía en el
tiempo, y por ende ya no hay diferencia de potencial entre los extremos de la bobina. Decimos
en ese caso la bobina se comporta como un cortocircuito. En ese caso el circuito de la figura
es simplemente una pila con dos resistencias. Suponiendo que la corriente circula en sentido
horario en la malla derecha, y anti-horario en la izquierda, la ley de las mallas –aplicada a la
malla derecha– implica que:
−ε + I1 R1 = 0

---

### Página 137

en donde I1 es la corriente que pasa por R1 . Esta es la misma corriente que pasa por la bobina,
IL = ε/R1 . La energía en la bobina es, entonces,
UL =

Lε2
LIL 2
2R1 2

b) Justo después de cambiar el estado del circuito abriendo el interruptor, la corriente a través
de la bobina es la misma que justo antes, pues la bobina se opone a los cambios en la corriente
circulante. Esta es, por ende, la corriente que circula en toda la malla exterior. Note que la
corriente en R2 se ha invertido. La ley de mallas nos indica entonces que, en t = 0+ ,
−εL (0+ ) + I(0+ )R1 + I(0+ )R2 = 0
con I(0+ ) = ε/R1 . Despejando la diferencia de potencial,
εL (0+ ) =

R1 + R2
ε
R1

y como la corriente circula en sentido horario –en la malla externa–, el potencial en b es mayor
que en a.
c) Para un instante t > 0, la ley de las mallas nos dice que
−εL + I(R1 + R2 ) = 0
˙ por Lenz. La ecuación queda
en donde εL = −LI,
R
I˙ + I = 0
L

(D + α)I = 0

con α = R/L y R = R1 + R2 . Usando el Método del operador diferencial aprendido en el curso
de Ecuaciones Diferenciales,
I(t) = Ke−αt
Reemplazando I(0) = ε/R1 ,
I(t) =

ε −αt
e
R1

Este resultado era el esperado: en ausencia de una fem externa, la corriente decae exponencialmente en un circuito LR. Toda la energía almacenada en el inductor es disipada por la
resistencia. Esta corriente es la misma que circula en ambas resistencias. Un bosquejo de ambas
corrientes es parecido al que aparece a continuación. Los números corresponden a ε = 18 V,
R1 = 2 kΩ, R2 = 6 kΩ y L = 0.4 H.

---

### Página 138

Note que, en R2 , la corriente se vuelve negativa. Esto es porque el sentido se ha invertido
respecto de su sentido original.
d ) Sea t∗ el instante en el cual la corriente vale i. Matemáticamente, I(t∗ ) = i. Reemplazando en
la ecuación de la corriente, podemos despejar el tiempo en función de la corriente deseada,
i = I(t∗ ) =

ε −αt∗
e
R1

iR1
∗
= e−αt
ε

Tomando logaritmo y despejando el tiempo,




L
ε
iR1
∗
ln
t = − ln
α
ε
R1 + R1
iR1
(6) Considere el circuito de la figura

L

R3
I3
R2

I2

I1

+
−

R1
ε

Determine la corriente por cada resistencia:
a) Inmediatamente después de cerrar el interruptor
b) Después de que ha pasado mucho de tiempo de cerrado el interruptor
c) Suponga que el interruptor es reabierto después de que ha estado mucho tiempo cerrado,
encuentre nuevamente las corrientes:
(i) Inmediatamente después de que es abierto
(ii) Después de un largo tiempo
a) Inmediatamente después de que el interruptor es cerrado, la corriente a través de la inductancia
es cero ya que la fem autoinducida evita que la corriente crezca abruptamente. Así, I3 = 0.
Debido a que I1 = I2 + I3 , se tiene que I1 = I2 . Utilizando las leyes de Kirchhoff,
−ε + I1 R1 + I1 R2 = 0

I1 = I2 =

ε
R1 + R2

---

### Página 139

b) Después de un largo tiempo, no hay fem autoinducida en la inductancia y las corrientes pasan
a ser constantes. Para la malla inferior, se tiene ahora
−ε + I1 R1 + I2 R2 = 0
y para la malla superior,
I3 R3 − I2 R2 = 0
por último, por la ley de nodos, I1 = I2 + I3 . Resolviendo, se obtiene
I1 =

(R2 + R3 )ε
R1 R2 + R1 R3 + R2 R3

R3 ε
R1 R2 + R1 R3 + R2 R3
R2 ε
I3 =
R1 R2 + R1 R3 + R2 R3
I2 =

c)

(i) Inmediatamente después de que el interruptor es abierto nuevamente, la corriente a través
de R1 es 0, I1 = 0. Esto implica que I2 +I3 = 0. La malla superior ahora forma un circuito
RL que decae e I3 tiende a mantenerse en el tiempo. Así,
I3 = −I2 =

R2 ε
R1 R2 + R1 R3 + R2 R3

(ii) Después de mucho tiempo, toda la energía se ha disipado, y por tanto todas las corrientes
son cero:
I1 = I2 = I3 = 0

4.3.

Corriente Alterna

(1) El resultado visto en clases, respecto a un transformador, nos permite obtener un voltaje de salida
determinado cambiando el número de espiras en las bobinas dentro del transformador. Por ejemplo,
si N2 > N1 , el voltaje de salida resulta mayor al voltaje de entrada. ¿Viola esto el principio de
conservación de energía? El problema consiste en convencerse de que la respuesta es no. Para ello,

N1 N2
V1

V2
Transformador

a) Demuestre que M 2 = L1 L2 , en donde M es la inductancia mutua, y Li=1,2 son las autoinductancias.

---

### Página 140

b) Suponiendo que la fem en la bobina primaria es −ε1 = V1 cos ωt, y que la secundaria se conecta
a una resistencia R, demuestre que las corrientes satisfacen las ecuaciones
L1 I˙1 + M I˙2 = V1 cos ωt ,

L2 I˙2 + M I˙1 = −I2 R

c) Obtenga las corrientes como función del tiempo, asumiendo que I1 (t) es una corriente puramente alterna.
d ) Muestre que el voltaje de salida y el voltaje de entrada satisfacen
N1
Vin
Vout
N2
e) Finalmente, muestre que la potencia entrante promediada en un ciclo T = 2π/ω es igual a la
potencia saliente promediada en el mismo intervalo temporal.
a) Si todas las espiras de ambas bobinas son cruzadas por el mismo flujo, digamos Φ, entonces el
flujo neto en la espira primaria se puede escribir como una contribución de autoinductancia e
inductancia mutua,
Φ1 = N1 Φ = L1 I1 + MI2

Φ=

L1
M
I1 +
I2
N1
N1

Φ=

L2
M
I2 +
I1
N2
N2

Lo mismo se puede hacer para la bobina secundaria,
Φ2 = N2 Φ = L2 I2 + MI1

Igualando ambas ecuaciones,
L1
M
L2
M
I1 +
I2 =
I2 +
I1
N1
N1
N2
N2
De aquí vemos que, si la corriente en la bobina primaria es nula, entonces M/N1 = L2 /N2.
Si, en cambio, la corriente en la bobina secundaria es nula, vemos que L1 /N1 = M/N2 . Multiplicando ambas ecuaciones, se prueba que M 2 = L1 L2 . Este resultado deja de ser válido si el
flujo en distintas espiras es diferente.
b) Por la ley de Lenz, la fem inducida en cada bobina es
−ε1 = L1 I˙1 + M I˙2 ,

−ε2 = L2 I˙2 + M I˙1

Del enunciado hemos de suponer que −ε1 = V1 cos ωt. Por otra parte, si se conecta una resistencia R a la bobina secundaria, debemos tener por Kirchhoff, ε2 − I2 R = 0. Inmediatamente
obtenemos las ecuaciones
L1 I˙1 + M I˙2 = V1 cos ωt ,

L2 I˙2 + M I˙1 = −I2 R

---

### Página 141

c) Para resolver estas ecuaciones, multiplicamos la primera por L2 , la segunda por M y restamos,
recordando que M 2 = L1 L2 . Obtenemos:
I2 = −

MV1
L2 V1
cos ωt = −
cos ωt
L1 R
MR

Insertando este resultado en la primera ecuación,
ωL2 V1
sin ωt
L1 I˙1 = V1 cos ωt − M I˙2 = V1 cos ωt −
R
Integrando,
L1 I1 =

L2 V1
V1
sin ωt +
cos ωt + A
ω
R

en donde A es una constante de integración. Del enunciado, debemos suponer que la corriente
por la bobina primaria es puramente alterna, lo que implica que no puede tener componentes continuas, representados matemáticamente por términos constantes; por ende A = 0. La
corriente 1 queda:
L2 V1
V1
sin ωt +
cos ωt
I1 =
ωL1
L1 R
d ) El voltaje de entrada es, por el enunciado, Vin = V1 cos ωt. El voltaje de salida es el de la
resistencia, Vout = I2 R = −L2 V1 /M cos ωt. La razón pedida es
M
Vin
V1 cos ωt
=−
= L2 V1
Vout
L2
− M cos ωt
Usando la parte (a), M/N1 = L2 /N2 , vemos que:
N1
Vin
Vout
N2
e) La potencia de entrada es
V1 2
Pin (t) = Vin I1 =
L1




sin ωt cos ωt L2
+
cos ωt
ω
R

La potencia de salida es
Pout (t) = Vout I2 =

L2 2 V1 2
cos2 ωt
M 2R

Definición. El promedio temporal de una función periódica, de periodo T , es:
ˆ
1 T
h f (t) i =
f (t) dt
T 0

---

### Página 142

Con ello, es posible demostrar (y queda propuesto para el lector) que:
h sin2 ωt i = h cos2 ωt i =

,

h sin ωt cos ωt i = 0

en donde ωT = 2π. Por ende, vemos que:
V1 2 L2
h Pin (t) i =
,
2L1 R

V1 2 L2 2
h Pout (t) i =
2M 2 R

y usando M 2 = L1 L2 , demostramos que
h Pin (t) i = h Pout (t) i
luego, la energía disipada en cada ciclo por la resistencia, es compensada con la potencia de
entrada en la bobina primaria, y por tanto, NO hay violación al principio de conservación de
energía.
(2) Considere el circuito de la figura, donde V (t) = Vo cos ωt. Si S1 y S2 se cierran inicialmente, encuentre
(los datos son R, L, Vo y ω):

S1

L
R
C

S2

V(t)
a) La corriente en función del tiempo
b) La potencia promedio entregada al circuito
c) La corriente en función del tiempo mucho después de que S1 se abre
d ) La capacidad C si S1 y S2 se abren y después de un tiempo largo, la corriente y el voltaje
están en fase
e) La impedancia cuando S1 y S2 se abren
f ) La energía máxima almacenada en el condensador y la inductancia
g) La diferencia de fase entre voltaje y corriente si se dobla la frecuencia ω
h) La frecuencia para la cual la reactancia inductiva es igual a un medio de la reactancia capacitiva

---

### Página 143

a) Al cerrar ambos interruptores, no circulará corriente por la inductancia ni por el condensador.
La impedancia equivalente en este caso es Zeq = R de modo que la corriente es, simplemente:
I(t) =

Vo
cos ωt
R

b) La potencia instantánea consumida por la resistencia es:
P(t) = V (t)I(t) =

Vo 2
cos2 ωt
R

Claramente una función periódica, y por tanto el promedio temporal es:
ˆ
1 T
Vo 2
h P(t) i =
P(t) dt =
T 0
2R
c) Cuando se abre S1 , se conecta la inductancia al circuito. La impedancia equivalente en este
caso es


√
ωL
iθℓ
Zeq = R + iωL = R + ω L e , θℓ = arctan
R
Luego, la corriente es:
V̂
Vo
Iˆ =
=√
e−iθℓ
Zeq
R + ω 2 L2
Así,
I(t) = Re {Iˆ eiωt } = √

Vo
cos (ωt − θℓ )
R2 + ω 2 L2

d ) Ahora se conecta también el condensador, de modo que la impedancia equivalente en este caso
es




ωL − 1/ωC
iφ
= |Z| e , φ = arctan
= R + i ωL −
Zeq = R + iωL +
iωC
ωC
R
Como no hay desfase entre voltaje y corriente, φ = 0 y el circuito está en resonancia:
ωL =
e) Es claro que:
|Z| =

ωC

s

C=



R2 + ωL −
ωC

ω2L

2

=R

y es puramente resistiva, como se esperaba por ser resonante.
f ) En este caso, la corriente circulante por el circuito será
I(t) =

Vo
cos ωt
R

---

### Página 144

En el caso particular del condensador,
I(t) =

dQ
dt

Q(t) =

Vo
sin ωt
ωR

Por lo tanto, la energía es:
Uc (t) =

Q(t)2
Vo 2
LVo 2
sin
ωt
sin2 ωt
2C
2ω 2 R2 (1/ω 2L)
2R2

Uc,máx =

LVo 2
2R2

En el caso de la inductancia,
LI(t)2
LVo 2
Uℓ (t) =
cos2 ωt
2R2

LVo 2
Uℓ,máx =
2R2

g) Si la frecuencia es ahora
ω
e = 2ω = √

LC

el ángulo de desfase entre corriente y voltaje es:
φ = arctan



ω
e L − 1/e
ωC
R

h) Finalmente, la frecuencia para que XL =
ω1/2 L =

1 1
2 ω1/2 C



2R

= arctan

r !
L
C

XC
debe cumplir
ω1/2 = √

ω
=√
2LC

(3) El circuito de la figura se denomina filtro RC pasa-altos porque transmite con mayor amplitud las
señales de alta frecuencia que las de baja. Si la tensión de entrada es Vin = Vo cos ωt, demostrar
que la de salida es Vout = VR cos (ωt − φ), donde
VR = s
y estudie los casos en que ω ≪

1+

Vo


ωRC

2

,ω=
yω≫
.
RC
RC
RC

C
Vin

R
Vout

---

### Página 145

La impedancia equivalente está dada por:
i
=R−
Z =R+
iωC
ωC

r

R2 +

eiφ ,
ω C2

φ = − arctan



ωRC



Luego, la corriente fasorial circulante por el circuito es:
V̂
Vo
Iˆ =
=r
Z
R2 +

e−iφ

ω2C 2

Finalmente, Vout es el voltaje entre los extremos de la resistencia,
ˆ =r
V̂out = IR

RVo

Vo
e−iφ = r
e−iφ
R2 + 2 2
1+ 2 2 2
ω C
ω RC

Con esto,
Vout (t) = Re {V̂out eiωt } = s

1+

Vo


ωRC

2 cos (ωt − φ)

s



Estudiemos los casos pedidos:
ω≪

RC
ω≪
RC

1≪
ωRC

Luego,
Vout (t) ≈

1+

ωRC

2

≈

=K
ωRC

Vo
cos (ωt − φ)
K

y, como K ≫ 1, el voltaje de salida se atenúa en gran cantidad. Por tanto, para bajas frecuencias, las señales se atenúan.
ω=

RC
Vo
Vout (t) = √ cos (ωt − φ)

lo que en Circuitos Eléctricos se conoce como frecuencia de corte del circuito.
ω≫

RC
ω≫
RC

1≫
ωRC

s

1+



ωRC

2

≈1

---

### Página 146

Luego,
Vout (t) ≈ Vo cos(ωt − φ)
y el voltaje de salida preserva su amplitud. Por tanto, para altas frecuencias, las señales se
transmiten.
Finalmente, el circuito selecciona las altas frecuencias y las transmite, mientras que las bajas frecuencias son filtradas: filtro pasa-altos.

(4) ¿Qué condición debe cumplirse, en el circuito de la figura, para que el cociente entre voltajes de
salida y entrada no dependa de la frecuencia?

Vin

R1

L1

R2

L2
Vout

Es claro que:
V̂out
V̂in
Como
Rk k Lk =



R2 k L2
R1 k L1 + R2 k L2

+
Rk iωLk

−1

iωLk Rk
Rk + iωLk

entonces:
L2 R2
iωL2 R2
L2 R2
V̂out
R2 + iωL2
R2 + iωL2


iωL1 R1
L1 R1
iωL2 R2
L2 R2
1 + iωL2 /R2
V̂in
+
+
L1 R2
+ L2 R2
R1 + iωL1 R2 + iωL2
R1 + iωL1 R2 + iωL2
1 + iωL1 /R1
Necesitamos que el paréntesis se anule:
1 + iωL1 /R1 = 1 + iωL2 /R2

L1
L2
R1
R2

---

### Página 147

5.

Ecuaciones de Maxwell

5.1.

Introducción a la teoría electromagnética

(1) Considere las leyes de la electrodinámica que hemos usado en el curso:
~ =
(i) ∇ · E

ρ
ǫ0

~ =0
(ii) ∇ · B
~
~ = − ∂B
(iii) ∇ × E
∂t
~ = µ0 J~
(iv) ∇ × B
Discuta su validez y analice la contribución de Maxwell.
Recordando que la divergencia del rotor es cero, analicemos la consistencia de la ecuación (iii):
!
~
~ = ∇ · − ∂ B = − ∂ (∇ · B)
~
∇ · (∇ × E)
∂t
∂t
El lado izquierdo es cero porque la divergencia del rotor es nula; el lado derecho es cero debido a la
ecuación (ii). Si aplicamos el mismo razonamiento a la ecuación (iv):
~ = µ0 (∇ · J)
~
∇ · (∇ × B)
El lado izquierdo sigue siendo cero; pero el lado derecho, en general, no lo es. Para corrientes
estacionarias, la divergencia de J~ es nula, pero en otros casos hay una error en la ley de Ampère.
Existe otra forma de ver que la ley de Ampère falla para corrientes no estacionarias. Supongamos
que estamos en el proceso de carga de un capacitor, y deseamos aplicar la ley de Ampère al loop de
la figura:

¿Cómo determinar Ienc ? Bueno, es la corriente total que pasa por el loop, o más precisamente, la
corriente que atraviesa la superficie que tiene como frontera a dicho loop. En este caso:

---

### Página 148

Si tomamos la superficie que yace en el plano del loop, Ienc = I
Si tomamos la segunda superficie dibujada en la figura, entonces no hay corriente a través de
ella, e Ienc = 0
Este problema aparece porque la situación no es estática, y ya sabemos que Ampère se restringe a
la magnetostática, pero nos hace pensar en la fuerte dependencia de la superficie que elegimos: la
física debiese ser la misma, sin importar el loop o superficie que elijamos.
¿Qué hizo Maxwell? Mezclemos la ley de Gauss y la ecuación de continuidad:
!


~
∂
E
∂
∂ρ
~ = −∇ · ǫ0
ǫ0 ∇ · E
=−
∇ · J~ = −
∂t
∂t
∂t
~ en la ley de Ampère, lograremos eliminar el término extra
Combinando este último término con J,
de la divergencia. Así,
~
~ = µ0 J~ + µ0 ǫ0 ∂ E
∇×B
∂t
Maxwell llamó a este término extra corriente de desplazamiento:
~
∂E
J~d ≡ ǫ0
∂t
La confirmación real de la teoría de Maxwell ocurrió en 1888 con los experimentos de Hertz sobre
ondas electromagnéticas. Así, las actuales Leyes de Maxwell son:
~ = ρ
(i) ∇ · E
ǫ0
~ =0
(ii) ∇ · B
~ =−
(iii) ∇ × E

~
∂B
∂t

~
~ = µ0 J~ + µ0 ǫ0 ∂ E
(iv) ∇ × B
∂t
(2) Considerando que una onda satisface la ecuación
a2 ∆u = utt ,
con a la velocidad de la onda, pruebe que los campos eléctricos y magnéticos en un medio no
conductor y libre de fuentes satisfacen la ecuación de onda.

---

### Página 149

En este caso, las ecuaciones de Maxwell son:
~ =0
(i) ∇ · E
~ =0
(ii) ∇ · B
~
~ = − ∂B
(iii) ∇ × E
∂t
~
~ = µ0 ǫ0 ∂ E
(iv) ∇ × B
∂t
Utilizaremos ahora la conocida identidad
∇ × (∇ × f~) = ∇(∇ · f~) − ∆f~
con ∆f~ es el laplaciano aplicado a cada componente del vector. De esta forma,
~ = ∇(∇ · E)
~ − ∆E
~
∇ × (∇ × E)
~ = 0, como indica la primera ecuación de Maxwell. Por
Pero en las regiones libres de fuente, ∇ · E
otro lado,
!
!
~
~
~
∂
B
∂
∂
E
∂2E
∂
~ =∇× −
~ =−
∇ × (∇ × E)
= − (∇ × B)
µ0 ǫ0
= −µ0 ǫ0 2
∂t
∂t
∂t
∂t
∂t
Igualando,
~ =
c2 ∆E
definiendo
c= √

~
∂2E
∂t2

µ0 ǫ0

Descubrimos que el campo se propaga con velocidad c, que corresponde a la velocidad de la luz en
el vacío, lo que indica que la luz no es otra cosa que una onda electromagnética. La deducción para
el campo magnético es la misma, y queda propuesta al lector.
(3) En este problema estudiaremos la invariancia de gauge del electromagnetismo. Hasta situaciones
~ B
~ a través de los potenciales φ, A
~ tal
estáticas, sabemos que que es posible estudiar los campos E,
que
~ = −∇φ
~ =∇×A
~
E
∧
B
~
~ = −∇φ − ∂ A
a) Estudie por qué, para situaciones dinámicas, se hace necesario que E
∂t
′ ~ ′
~
b) Pruebe que los campos E , B asociados a
~′ =A
~ + ∇f
A

∧

~ =E
~′yB
~ =B
~ ′ . ¿Qué puede concluir?
satisfacen E

φ′ = φ−

∂f
∂t

---

### Página 150

c) Usando alguna gauge fixing condition, establezca condiciones para los potenciales, de modo tal
que sean consistentes con las ecuaciones de Maxwell
a) De la ley de Faraday-Lenz, si solo consideramos el aporte estático:
~ = ∇ × (−∇φ) = ~0
∇×E
que no es cierta en casos dinámicos; pero, al considerar la sugerencia del enunciado,

~
~
∂B
∂
∂A
~
~
∇ × A − ~0 = −
− ∇ × ∇φ = −
∇ × E = −∇ ×
∂t
∂t
∂t

que sí es consistente.

b) Partiendo por el campo magnético,
~ ′ =∇×A
~′ =∇×A
~ + ∇ × ∇f = ∇ × A
~=B
~
B
Para el campo eléctrico,
~′
∂A
E = −∇φ −
= −∇φ + ∇
∂t
~′

′



∂f
∂t



−

~
~
∂A
∂A
∂ 
~
∇f = −∇φ −
−
=E
∂t
∂t
∂t

Lo anterior nos hace pensar dos conclusiones importantes: (1) los potenciales no son magnitudes
físicas medibles unívocamente determinadas; muy por el contrario, podemos tener infinitas
funciones potencial que darán origen a los mismos campos físicos. (2) por la libertad concedida
por la función f , podemos elegir los potenciales que más nos acomoden para resolver problemas,
dando origen a la misma física: esto se conoce como invariancia de gauge.
c) Apliquemos la ley de Gauss:

~
∂
∂A
~
~
∇·A
= −∆φ −
∇ · E = −∇ · ∇φ − ∇ ·
∂t
∂t

Por otra parte, la ley de Ampère para una densidad de corriente total J~ es:
~ =∇×∇×A
~ = ∇(∇ · A)
~ − ∆A
~
µ0 J~ = ∇ × B
~ = 0. Así, las ecuaciones
En ambos casos, podemos fijar la condición de Gauge de Coulomb: ∇· A
pedidas son:
ρ
~ = −µ0 J~
∧
∆A
∆φ = −
ǫ0
(4) Un cable ancho, de radio a, porta una corriente constante I, uniformemente distribuida sobre su
sección transversal. Una estrecha separación en el cable, de ancho w ≪ a, forma un capacitor de
placas paralelas, como muestra la figura. Encuentre el campo magnético en la separación, a distancia
s < a del eje.

---

### Página 151

Sabemos que la densidad de corriente de desplazamiento es:
~
∂E
I
I
J~d = ǫ0
= = 2 k̂
∂t
A
πa
Dibujando un loop amperiano de radio s,
˛
~ · d~r = B 2πs = µ0 Idenc = µ0 I · πs2 = µ0 I s
B
πa2
a2
Por lo tanto,

~ = µ0 Is θ̂
B
2πa2

(5) El problema anterior fue un modelo artificial para un capacitor cargándose. Para un modelo más
realista, considere cables delgados que se conectan al centro de placas metálicas, como en la Figura
(a). Nuevamente, la corriente I es constante, el radio del capacitor es a, y la separación de las placas
es w ≪ a. Asuma que las corriente fluye fuera de las placas de modo tal que la carga superficial es
uniforme, para toto tiempo, y es nula en t = 0.

a) Encuentre el campo eléctrico entre las placas, como función del tiempo t
b) Halle la corriente de desplazamiento a través de un círculo de radio s en el plano intermedio
entre las placas. Usando este círculo como loop amperiano, y la superficie que lo extiende, halle
el campo magnético a una distancia s del eje
c) Repita la parte anterior, pero ahora empleando una superficie cilíndrica, como muestra la Figura (b), que se extiende desde la izquierda y atraviesa la placa, terminando fuera del capacitor.
Note que la corriente de desplazamiento a través de esta superficie es cero, y que hay dos
contribuciones para Ienc .

---

### Página 152

~ = σ(t) k̂, con:
a) En este caso, E
ǫ0
σ(t) =

It
Q(t)
= 2
A
πa

Luego,
~
E(t)

It
k̂
πσ0 a2

b) En este caso,
Idenc = Jd πs2 = ǫ0
Por otra parte,
˛

~ · d~r = µ0 Idenc
B

~
∂E
s2
πs2 = I 2
∂t
a

s2
B 2πs = µ0 I 2
a

~ = µ0 Is θ̂
B
2πa2

c) Una corriente superficial fluye radialmente fuera de la placa izquierda; sea I(s) la corriente
total que cruza el círculo de radio s. La densidad de carga (al tiempo t) es:
σ(t) =

[I − I(s)]t
πs2

Como dijimos que era independiente de s, entonces I − I(s) = βs2 , para alguna constante β.
Pero I(a) = 0, entonces βa2 = I, o β = I/a2 . Entonces, I(s) = I(1 − s2 /a2 ).
s2
B 2πs = µ0 Ienc = µ0 [I − I(s)] = µ0 I 2
a

~ = µ0 Is θ̂
B
2πa2

(6) Una de las consecuencias de las leyes de Maxwell es que las cargas aceleradas pierden energía en
forma de radiación electromagnética (luz). Para velocidades pequeñas comparadas con la velocidad
de la luz, la tasa de pérdida de energía en el tiempo viene dada por la fórmula de Larmor:
dE
q 2 a2
=−
dt
6πǫ0 c3
donde a es la aceleración de la carga y c = 3 × 108 m/s es la velocidad de la luz. Suponga que en el
tiempo t = 0, el electrón de masa m y carga −e que orbita al protón de carga +e se ubica a una
distancia a0 = 5.3 × 10−11 m de este último. Muestre que existe un tiempo finito tf en el que dicho
electrón alcanza el núcleo, lo que implica que los átomos no son estables clásicamente hablando.
Calcule el valor de tf , la llamada vida media clásica del átomo de Hidrógeno.
Supondremos que el núcleo atómico se encuentra fijo en el origen. Un electrón de carga −e y masa

---

### Página 153

m en una órbita de radio r en torno a un núcleo con carga +e siente una fuerza dada por la Ley de
Coulomb. Utilizando la segunda Ley de Newton,
ma = macentr =

mv 2
e2
r
4πǫ0 r 2

en la aproximación en que la órbita permanece casi circular en todo instante y que la aceleración
tangencial es despreciable frente a la aceleración radial (centrípeta). De esta forma, la pérdida de
energía por radiación viene dada por
e6
2re 3 mc3
dE
=−
−
dt
96π 3 ǫ0 3 m2 c3 r 4
3r 4
donde re = e2 /(4πǫ0 mc2 ) = 2.8 × 10−15 m es el llamado radio clásico del electrón. La energía total
del electrón (cinética y potencial) es:
E=

mv 2
e2
e2
re mc2
−
=−
=−
4πǫ0 r
8πǫ0 r
2r

Tomando la derivada temporal de la expresión anterior, y utilizando la fórmula de Larmor,
dE
re mc2 dr
2re 3 mc3
−
dt
2r 2 dt
3r 4
Simplificando,
dr
4re 2 c
= − 2
dt
3r
3r 2 dr = −4re 2 c dt
r 3 (t) − r 3 (0) = −4re 2 c t

1/3
∴ r(t) = a0 3 − 4re 2 c t
Por tanto, existe un tiempo tf tal que:
r(tf ) = 0

tf =

a0 3
= 1.6 × 10−11 s
4re 2 c

Este tiempo es del orden de magnitud de la vida media de un átomo de Hidrógeno excitado, cuyo
estado fundamental parece tener una vida media infinita, a diferencia de lo que predice la Física
Clásica. Esta fue una de las motivaciones de Bohr para proponer su modelo atómico, que marca el
comienzo de la Física Cuántica.
