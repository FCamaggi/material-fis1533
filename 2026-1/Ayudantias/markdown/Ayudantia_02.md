---
title: "Ayudantia 02"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_02.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_02_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 02

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 2
Campo Eléctrico

Resumen
⃗ se define como la fuerza por unidad de carga que se ejerce sobre una carga
El campo eléctrico E
de prueba en cualquier punto (siempre que la carga de prueba sea suficientemente pequeña para no
perturbar a la carga fuente), y matemáticamente corresponde a
⃗1
⃗ = 1 F⃗ = ke q1 ⃗r - r = ke q1 R̂
E
⃗2
q2
|⃗r ´ r⃗1 |3
|R|

(1)

⃗ “ ⃗r ´ r⃗1 . Siendo ⃗r la posición del espacio en la que queremos medir el campo y r⃗1 la posición
Con R
de la carga que produce el campo.
Esto permite estudiar el efecto que una carga fuente puede tener sobre cualquier otra, independiente
de la carga de esta. Por último, una propiedad muy útil, tanto de la fuerza eléctrica como del campo
eléctrico, es que para un conjunto de cargas discretas aplica el principio de superposición, esto es,
que el campo o fuerza neta en un punto es igual a la suma de todos los campos o fuerzas generados
por cada una de las cargas en el espacio, matemáticamente
F⃗neto “

n
ÿ

F⃗i

⃗ neto “
& E

i = 1

n
ÿ
i = 1

⃗i
E

(2)

---

### Página 2

#### Problema 1
Considere la siguiente distribución de carga,

(a) Determine el campo eléctrico en el punto P
(b) Estudie el caso donde r " d. Le puede resultar útil la expansión de taylor,
p1 ` ϵqn = 1 ` nϵ

ϵ!1

(c) Compare este sistema con el más simple de una única carga puntual. ¿Qué campo eléctrico
decae más rápido?
#### Problema 2
Dos cargas puntuales están fijas sobre el eje x:
q1 “ `q

en

x = -a,

q2 “ `4q

en

x “ `a,

con q > 0 y a > 0.
(a) Encontrar todos los puntos del eje x donde el campo eléctrico neto se anula.
(b) Determinar la dirección del campo eléctrico neto en las tres regiones del eje:
x < -a,

´a < x < a,

x > a.

(c) Si se coloca una carga de prueba Q > 0 en el punto donde el campo eléctrico se anula,
discutir qué ocurre si se la desplaza ligeramente hacia la derecha o hacia la izquierda sobre
el eje x. ¿Corresponde este punto a un equilibrio estable o inestable sobre el eje?

---

### Página 3

(d) Calcular la fuerza eléctrica neta que experimenta una carga de prueba Q colocada en el punto
x = 0.
(e) Propuesto: Suponga ahora que la carga de prueba tiene masa m y puede moverse sin rozamiento únicamente a lo largo del eje x. Mostrando que el punto encontrado en (a) corresponde a un equilibrio estable, calcule la frecuencia angular de pequeñas oscilaciones de la
partícula alrededor de ese punto.
#### Problema 3
Dos barras delgadas e iguales de longitud L y carga total Q distribuida uniformemente, están situadas sobre el eje x con una separación d,

Calcule la fuerza que ejerce la barra izquierda sobre la barra derecha.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 2
Campo Eléctrico

Resumen
⃗ se define como la fuerza por unidad de carga que se ejerce sobre una carga
El campo eléctrico E
de prueba en cualquier punto (siempre que la carga de prueba sea suficientemente pequeña para no
perturbar a la carga fuente), y matemáticamente corresponde a
⃗1
⃗ = 1 F⃗ = ke q1 ⃗r - r = ke q1 R̂
E
⃗2
q2
|⃗r ´ r⃗1 |3
|R|

(1)

⃗ “ ⃗r ´ r⃗1 . Siendo ⃗r la posición del espacio en la que queremos medir el campo y r⃗1 la posición
Con R
de la carga que produce el campo.
Esto permite estudiar el efecto que una carga fuente puede tener sobre cualquier otra, independiente
de la carga de esta. Por último, una propiedad muy útil, tanto de la fuerza eléctrica como del campo
eléctrico, es que para un conjunto de cargas discretas aplica el principio de superposición, esto es,
que el campo o fuerza neta en un punto es igual a la suma de todos los campos o fuerzas generados
por cada una de las cargas en el espacio, matemáticamente
F⃗neto “

n
ÿ

F⃗i

⃗ neto “
& E

i = 1

n
ÿ
i = 1

⃗i
E

(2)

---

### Página 2

#### Problema 1
Considere la siguiente distribución de carga,

(a) Determine el campo eléctrico en el punto P
(b) Estudie el caso donde r " d. Le puede resultar útil la expansión de taylor,
p1 ` ϵqn = 1 ` nϵ

ϵ!1

(c) Compare este sistema con el más simple de una única carga puntual. ¿Qué campo eléctrico
decae más rápido?
Solución:Tomamos el eje x horizontal y el eje y vertical. Las cargas se encuentran en
p´d, 0q,

p0, 0q,

pd, 0q

´q,

`2q,

´q

con valores

respectivamente. El punto donde queremos calcular el campo es
P = (0, r).
El campo eléctrico de una carga puntual Q ubicada en ⃗r1 es
⃗ rq “
Ep⃗

Q
p⃗r ´ ⃗r1 q.
4πε0 |⃗r ´ ⃗r |

Campo debido a la carga central `2q
La carga está en p0, 0q, por lo que

---

### Página 3

⃗r - ⃗r1 = (0, r)
y
⃗0 “
E

1 2q
ŷ.
4πε0 r2

Campo debido a la carga en p´d, 0q
El vector desde la carga hasta P es
⃗ - = (d, r),
R
con módulo
⃗ ´| “
|R

?
d2 ` r 2 .

Entonces
⃗´ “
E

´q
pd x̂ ` r ŷq.
4πε0 pd2 ` r2 q3{2

Campo debido a la carga en pd, 0q
El vector desde la carga hasta P es
⃗ ` = p´d, rq
R
y
⃗` “
E

´q
p´d x̂ ` r ŷq.
4πε0 pd ` r2 q3{2

Campo total
El campo eléctrico total es
⃗ = E
⃗0 ` E
⃗´ ` E
⃗ `.
E
Las componentes en x se cancelan por simetría, por lo que el campo solo tiene componente en y:
Ey “
4πε0

2q
2qr
´ 2
r
pd ` r2 q3{2

˙

ˆ

˙

ˆ

.

Por lo tanto,
⃗ q“
EpP

4πε0

2q
2qr
´ 2
r
pd ` r2 q3{2

ŷ

---

### Página 4

(b) Caso r " d
Partimos del resultado obtenido en la parte (a):
⃗ q = 1
EpP
4πε0

ˆ

2q
2qr
´ 2
r
pd ` r2 q3{2

˙
ŷ.

Ahora queremos estudiar esta expresión en el régimen r " d. Para ello, factorizamos r2 dentro del
paréntesis:
ˆ

d `r = r

d2
1` 2
r

˙

ˆ

˙3{2

,

de modo que

2 3{2

pd ` r q

“r

d2
1` 2
r

.

Entonces,
r
r
“ `
“ 2
˘
3{2
3{2
pd ` r q
r
r3 1 ` d

ˆ

r2

d2
1` 2
r

˙´3{2

Sustituyendo esto en la expresión del campo,
«

⃗ q“
EpP

ˆ

d
2q
1´ 1` 2
4πε0 r
r

˙´3{2 ff

Como r " d, se tiene
d2
! 1,
r2
por lo que podemos usar la expansión de Taylor
p1 ` ϵqn « 1 ` nϵ,

ϵ ! 1.

En este caso,
d2
ϵ = 2,
r

n = - ,

de modo que
ˆ

d2
1` 2
r

˙´3{2
«1´

Así,

3 d2
.
2 r2

ŷ.

.

---

### Página 5

ˆ

d2
1´ 1` 2
r

˙´3{2

ˆ

3 d2
«1´ 1´
2 r2

˙
“

3 d2
.
2 r2

Reemplazando esto en el campo eléctrico,
⃗ q«
EpP

2q
4πε0 r2

ˆ

3 d2
2 r2

˙
ŷ.

Simplificando,
⃗ q « 3qd ŷ
EpP
4πε0 r4

pr " dq.

Por lo tanto, en el límite lejano el campo eléctrico decae como 1{r4 .
(c) Comparación con una única carga puntual
Para una única carga puntual Q, el campo eléctrico a una distancia r tiene magnitud del orden de
.
r2
En cambio, en la parte (b) encontramos que para esta distribución de cargas, en el régimen r " d,
el campo se comporta como
Epuntual „

Esistema „

.
r4

Como
r4
decrece más rápidamente que
,
r2
concluimos que el campo eléctrico de esta distribución de cargas decae más rápido que el de una
única carga puntual.
Esto ocurre porque la carga neta total del sistema es nula:
p`2qq ` p´qq ` p´qq = 0.
En conclusión,
Epuntual „

,
r2

Esistema „

y por lo tanto el campo de esta distribución decae más rápido.

r4

---

### Página 6

#### Problema 2
Dos cargas puntuales están fijas sobre el eje x:
q1 “ `q

en

x = -a,

q2 “ `4q

en

x “ `a,

con q > 0 y a > 0.
(a) Encontrar todos los puntos del eje x donde el campo eléctrico neto se anula.
(b) Determinar la dirección del campo eléctrico neto en las tres regiones del eje:
x < -a,

´a < x < a,

x > a.

(c) Si se coloca una carga de prueba Q > 0 en el punto donde el campo eléctrico se anula,
discutir qué ocurre si se la desplaza ligeramente hacia la derecha o hacia la izquierda sobre
el eje x. ¿Corresponde este punto a un equilibrio estable o inestable sobre el eje?
(d) Calcular la fuerza eléctrica neta que experimenta una carga de prueba Q colocada en el punto
x = 0.
(e) Propuesto: Suponga ahora que la carga de prueba tiene masa m y puede moverse sin rozamiento únicamente a lo largo del eje x. Mostrando que el punto encontrado en (a) corresponde a un equilibrio estable, calcule la frecuencia angular de pequeñas oscilaciones de la
partícula alrededor de ese punto.
#### Solución:
Sean dos cargas puntuales fijas sobre el eje x:
q1 “ `q

en

x = -a,

q2 “ `4q

en

x “ `a,

con q > 0 y a > 0.
(a) Puntos del eje x donde el campo eléctrico neto se anula
Como ambas cargas son positivas, el campo eléctrico que produce cada una apunta alejándose de la carga. Por lo tanto, analizamos por regiones:
x < -a,

´a < x < a,

x > a.

En las regiones exteriores, x < -a y x > a, los campos producidos por ambas cargas apuntan
en la misma dirección, así que no pueden cancelarse. Por lo tanto, el único lugar donde el
campo podría anularse es en la región intermedia

---

### Página 7

´a < x < a.
En esa región, el campo debido a q1 “ `q apunta hacia la derecha y el campo debido a
q2 “ `4q apunta hacia la izquierda. Para que el campo neto sea nulo, sus magnitudes deben
ser iguales:
q
4q
“
.
4πε0 px ` aq
4πε0 pa ´ xq2
Cancelando factores comunes,
“
.
px ` aq
pa ´ xq2
Tomando raíz cuadrada en ambos lados,
“
.
x`a
a´x
Entonces,
a - x = 2px ` aq.
Desarrollando,
a - x = 2x ` 2a,

´3x = a,
a
x = - .
Por lo tanto, el único punto donde el campo eléctrico neto se anula es
a
x = - .
(b) Dirección del campo eléctrico neto en las tres regiones
Analizamos la dirección del campo de cada carga en cada región.
Región 1: x < -a
En esta región, el punto está a la izquierda de ambas cargas. Como las dos cargas son positivas, ambos campos apuntan hacia la izquierda. Por lo tanto,

---

### Página 8

⃗ net apunta hacia la izquierda para x < -a.
E
Región 2: -a < x < a
Aquí el campo de la carga `q en x = -a apunta hacia la derecha, mientras que el campo
de la carga `4q en x “ `a apunta hacia la izquierda. Entonces la dirección depende de qué
campo domine.
Ya vimos en (a) que en
x = ´

a

ambos se cancelan. Por lo tanto:
⃗ net apunta hacia la derecha si - a < x < - a
E
y
⃗ net apunta hacia la izquierda si - a < x < a.
E
Región 3: x > a
En esta región, el punto está a la derecha de ambas cargas. Como ambas son positivas, los
dos campos apuntan hacia la derecha. Por lo tanto,
⃗ net apunta hacia la derecha para x > a.
E
(c) Estabilidad del punto de equilibrio sobre el eje x
Colocamos una carga de prueba Q > 0 en el punto donde el campo se anula:
a
x0 = - .
Queremos ver qué ocurre si la desplazamos levemente a izquierda o derecha.
Si la movemos un poco hacia la derecha, quedamos en la región
a
´ < x < a,
donde, según la parte (b), el campo neto apunta hacia la izquierda. Como Q > 0, la fuerza es
⃗
F⃗ = QE,

---

### Página 9

y por lo tanto también apunta hacia la izquierda, es decir, de vuelta hacia el punto de equilibrio.
Si la movemos un poco hacia la izquierda, quedamos en la región
a
´a < x < - ,
donde el campo neto apunta hacia la derecha. Entonces la fuerza sobre Q > 0 apunta hacia
la derecha, nuevamente de vuelta hacia el punto de equilibrio.
Así, un pequeño desplazamiento produce una fuerza restauradora que devuelve la carga hacia
a
x = - .
Por lo tanto, este punto corresponde a un equilibrio estable sobre el eje x.
a
El equilibrio en x = - es estable sobre el eje x.
(d) Fuerza eléctrica neta sobre una carga de prueba Q colocada en x = 0
En x = 0, la distancia a cada carga es a.
Cam(o debido a )1 = `q en x = -a:
Como el punto x = 0 está a la derecha de la carga, el campo apunta hacia la derecha y su
magnitud es
E1 “

1 q
.
4πε0 a2

⃗1 “
E

1 q
x̂.
4πε0 a2

Entonces,

Campo debido a q2 “ `4q en x “ `a:
Como el punto x = 0 está a la izquierda de esta carga, el campo apunta hacia la izquierda y
su magnitud es
E2 “
Entonces,

1 4q
.
4πε0 a2

---

### Página 10

⃗ 2 = - 1 4q x̂.
E
4πε0 a2
Campo neto en x = 0:
⃗
⃗1 ` E
⃗2 “
Ep0q
“E

1 q
1 4q
x̂ ´
x̂.
4πε0 a
4πε0 a2

⃗
Ep0q
“´

3q
x̂.
4πε0 a2

Por lo tanto, la fuerza neta sobre una carga de prueba Q es
⃗
F⃗ = QE(0),
es decir,
3qQ
F⃗ = ´
x̂
4πε0 a2
La fuerza apunta hacia la izquierda.
#### Problema 3
Dos barras delgadas e iguales de longitud L y carga total Q distribuida uniformemente, están situadas sobre el eje x con una separación d,

Calcule la fuerza que ejerce la barra izquierda sobre la barra derecha.
Solución:Por regla general, si queremos conocer el la fuerza eléctrica que ejerce un cuerpo 1 sobre
un cuerpo 2, lo calculamos de la siguiente forma,

---

### Página 11

ż
F1Ñ2 “

E1 dq2

Es decir, para este caso necesitamos conocer el campo eléctrico que genera la barra izquierda en el
espacio; lo calculamos de la siguiente forma,
E“
4πε0

ż

dq1 pr ´ r1 q
|r ´ r1 |3

Necesitamos aprender a diferenciar el r del r1 , SIEMPRE usaremos el r como el lugar donde vamos a querer medir el campo eléctrico y r1 el lugar donde se encuentra nuestra carga. Entonces para
nuestro caso de la barra izquierda,

r = xx̂
r1 = x1 x̂

Ñ

x1 P r0, Ls

pr - r1 q = px - x1 qx̂
|r - r1 |3 = px - x1 q3
Para trabajar con el diferencial de carga, utilizaremos la definición de densidad de carga (Puede ser
lineal, superficial o volumétrica, lo único que cambia es sobre que se integra),
dq
“ λ Ñ dq = λdx1
dx1
Entonces la integral para el campo eléctrico nos quedaría de la forma,
E1 “
4πε0

żL

λpx ´ x1 q 1
dx x̂
1 3
0 |x ´ x |

Podemos deshacernos del valor absoluto del denominador ya que cuando utilicemos valores de x
al momento de calcular la fuerza ejercida en la segunda barra, todos los valores de x serán mayores
que los valores de x1 . Entonces,
E1 “
4πε0

żL

λpx ´ x1 q 1
dx x̂ “
4πε0
0 px ´ x q

żL

λ
dx1 x̂
1 q2
px
´
x

(1)

Esta última integral es bastante directa de calcular, por lo que se obtiene que,
λ
E1 “
4πε0

ˆ

´
x´L x

˙
x̂

Este es nuestro primer resultado, el campo eléctrico de la barra izquierda, ahora volvemos la integral
de la fuerza,

---

### Página 12

ż
F1Ñ2 “

λ2
E1 dq2 “
4πε0

ż d`2L ˆ
d`L

´
x´L x

˙
dxx̂

Nuevamente es una integral bastante directa, el resultado final sale de resolverla.

„
ȷ
λ2
pd ` Lq2
F1Ñ2 “
ln
x̂
4πε0
dpd ` 2Lq

(2)
