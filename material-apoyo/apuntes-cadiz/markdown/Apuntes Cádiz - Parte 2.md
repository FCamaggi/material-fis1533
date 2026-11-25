---
title: "Parte 2"
source_pdf: "Electro/material-apoyo/apuntes-cadiz/Apuntes Cádiz - Parte 2.pdf"
pages: 115
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Parte 2

### Página 1

Parte II
Conductores, Ecuaciones de Poisson y
Laplace

---

### Página 2

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 3

#### Capítulo 7
Conductores
Hasta aquí hemos terminado con los problemas donde la distribución de carga es conocida
desde el comienzo. (Integrales de Coulomb). Hasta ahora han sido problemas sin mayores complicaciones que calcular correctamente las integrales. Ahora atacaremos otro tipo de problemas,
la determinación de los campos cerca de conductores.
La materia se puede clasificar gruesamente en conductores y aislantes ( o dieléctricos). Un
material dieléctrico posee electrones fuertemente ligados a los átomos, de manera que ante la
presencia de un campo eléctrico las partículas cargadas pueden cambiar sus posiciones ligeramente, pero se mantienen ligadas a sus moléculas. Por otro lado, un material conductor (como
un metal) es aquél que en su interior posee un gran número de electrones libres, y éstos se
pueden mover libremente en el conductor, responden a campos eléctricos casi infinitesimales y
continúan su movimiento mientras experimentan un campo. Esta corriente de electrones debe
estar constantemente provista de fuentes externas de energía, o sino el movimiento de los electrones se detendrá cuando cancelen el efecto de la fuente que produce el campo original (se
alcanza un equilibrio estático).
Campo eléctrostático dentro de un conductor es nulo
En electrostática, no consideramos fuentes continuas de corriente, de manera que los electrones
se moverán hasta que se arreglen de forma que produzcan un campo eléctrico nulo en cualquier
parte dentro del conductor (esto suele pasar en una fracción de segundo). Si quedara algún
campo dentro del conductor, este campo movería más electrones, luego la única solución electrostática es que el campo es cero en cualquier punto interior del conductor.
La carga en un conductor se distribuye en su superficie
Consecuencia directa de la propiedad anterior es que la carga en un conductor debe distribuírse
en su superficie. De la ley de gauss, es evidente que si existiera una carga neta al interior del
conductor, el flujo eléctrico sobre la superficie de la figura sería distinto de cero, y por lo tanto,
existiría un campo eléctrico en su interior

---

### Página 4

ˆˆ

 ~ 0
~ x0 ) = 0 → qin = 0
x ) · E(~
 dS(~
S

Notar que como el campo eléctrico es cero en el interior de un conductor, entonces
~ =0
−∇φ
Esto significa que al interior de un conductor el potencial es constante.
La dificultad que se presenta cuando hay condutores presentes es evidente. Suponga que estamos en la situación en que se carga un conductor con una carga Q. Ahora no estamos en
condiciones de saber exactamente dónde están las cargas, sólo sabemos que ellas se van a distribuír sobre toda la superficie. ¿Cómo podemos determinar la forma en que se distribuyen las
cargas? Veremos que ellas se deben distribuír de forma que que la superficie del conductor forme
una equipotencial. Si la superficie de un conductor no fuera equipotencial, entonces habría
un campo eléctrico distinto de cero en el interior del conductor, y las cargas en el conductor se
seguirán moviendo hasta que finalmente el campo en su interior se anula. (y se alcanze nuevamente un estado de equilibrio electrostático)
~ en la superficie de un conductor es cero
Componente tangencial de E
Considere la integral de línea sobre el camino cerrado de la figura
˛
~
d~x · E

Como el campo eléctrico es conservativo, la integral de línea sobre el camino cerrado abcda es
cero.
˛
~ = Et (∆l) − En (∆x0 ) + 0(∆l) + En (∆x) = 0
d~x · E
abcda

donde En y Et son las componentes normal y tangencial del campo eléctrico, respectivamente, y hemos escogido el segmento ab paralelo a Et en todos los puntos.
En el límite cuando ∆x0 → 0 y ∆x → 0, se tiene
Et ∆l = 0

---

### Página 5

Como ∆l es una longitud finita, se concluye que la componente tangencial del campo eléctrico sobre la superficie de un conductor es cero. Esto es algo sumamente importante, ya que consecuencia de ésto es que un conductor en equilibrio electrostático es una Superficie equipotencial. Mostrar esto ahora resulta evidente, considere 2 puntos A y B sobre la superficie de
un conductor, y calcule la diferencia de potencial entre estos dos puntos

φB − φA = −

ˆ B
A

~ x) = 0
d~x · E(~

~ sólo tiene componente normal a la curva . Luego, los puntos A y B se encuentran
ya que E
al mismo potencial
~ es normal a la superficie de un conductor
El campo E
Si la componente tangencial del campo fuera distinta de cero, las cargas entonces se moverían
hasta que ésta componente desaparezca. Luego, en un conductor en equilibrio, sólo sobrevive
la componente normal del campo eléctrico. Para obtener el campo eléctrico sobre la superficie
de un conductor, considere la superficie de Gauss de la figura

De la ley de Gauss obtenemos
 ~ 0
~ x0 ) = En A + 0A = σA
x ) · E(~
 dS(~

ˆˆ

0

S

de aquí
En =

σ
0

Es decir, el campo eléctrico justo sobre la superficie de un conductor es normal a ella y su
magnitud está directamente relacionada con la densidad superficial de carga sobre el punto del
conductor. Éstas consecuencias son absolutamente generales. Notar que ésto nos permite determinar la densidad superficial de carga sobre un conductor, sin embargo, ! se requiere conocer
el campo eléctrico ! ¿Cómo podemos determinar el campo eléctrico sin conocer primeramente
la densidad de carga en el conductor?. Veremos más adelante que esto es posible al resolver la
ecuación diferencial que satisface el potencial electrostático
Como conclusión, el campo eléctrico cerca de un conductor tiene la forma de la figura

---

### Página 6

Como ejemplo, considere un campo uniforme en la dirección horizontal en una región del
espacio. Imaginemos que colocamos una esfera conductora en este campo uniforme. Cargas
sobre el conductor se moveran y distribuirán hasta alcanzar un equilibrio electrostático, es
decir, hasta que el campo en su interior se anule y la componente tangencial del campo sobre la
superficie también, de manera que toda las cargas se encuentren en equilibrio en su superficie.
La situación de equilibrio será tal cual muestra la figura

Es decir, el campo eléctrico se ve deformado cerca de la esfera conductora, de manera que
líneas de campo sean normales en su superficie. El potencial electrostático sobre la superficie
esférica es una constante. Otro ejemplo de líneas de campo y superficies equipotenciales se
aprecia en la siguiente figura, donde dos conductores se encuentran cercanos

Una aplicación interesante es que la energía potencial de un conductor es muy simple de
calcular. Esto se debe a que en un conductor toda la carga se concentra en la superficie, y que
sobre ella el potencial es constante. Luego , la energía potencial asociada a un conductor de
carga Q y potencial V está dada por

---

### Página 7

¨
¨
¨
U=
φ(~x )dq(~x ) = φ
dq(~x ) = φ
σ(~x0 )dS(~x0 ) = φQ
2 S
S
S
La energía potencial de un conductor con carga Q y a potencial φ está dada por
U = φQ

7.1.

Condensadores

Un condensador es un dispositivo capaz de acumular carga eléctrica. Éstos pueden variar
en tamaño y forma, pero su configuración básica consiste en 2 conductores cargados con cargas
iguales y opuestas. Los condensadores son de gran importancia en electrónica, y entre sus
aplicaciones más conocidas están el almacenamiento de energía eléctrica, amortiguamiento de
los cambios de voltaje cuando se conectan a resistencias, filtros de frecuencias, reguladores de
tensión y muchas más.

Cuando se encuentran descargados, la carga en ambos conductores es cero. Durante el proceso
de carga, una carga Q se mueve desde un conductor a otro, dándole a uno una carga neta +Q
y al otro carga neta −Q. Una diferencia de potencial entre ambos ∆V se crea, con el conductor
cargado positivamente a un potencial más alto que el conductor cargado negativamente. Notar
que aunque esté cargado o descargado, la carga total del condensador como un todo es cero.
El ejemplo más simple de un condensador consiste de 2 placas conductoras de área A, paralelas
entre sí, separadas a una distancia d

La carga Q almacenada en un condensador es linealmente proporcional a la diferencia de potencial entre los conductores |∆V |. Así
Q = C|∆V |
Donde C es una constante positiva llamada capacidad. Físicamente, es una medida de
la capacidad de almacenar carga eléctrica en sus conductores para una diferencia de potencial
dada ∆V . La unidad de capacidad es C/V (Coulomb/ Volt), también conocida como F (Farad).

---

### Página 8

El Farad es una unidad muy grande, condensadores típicos no poseen una capacidad superior
a 1 µ F.

7.2.

Ecuaciones de Poisson y Laplace

Dadas las ecuaciones fundamentales de la electrostática
~ · E(~
~ x) = ρ(~x)
∇
0
~ × E(~
~ x) = 0
∇
Interesa encontrar una formulación matemática equivalente de este problema. Efectivamente, uno podría relacionar ambas ecuaciones, y obtener una única ecuación general que
permita solucionar cualquier problema electrostático. De la segunda ecuación, se desprende que
~ × E(~
~ x) = 0 → E(~
~ x) = −∇φ(~
~ x)
∇

Utilizando ésto en la primera ecuación
~ · (−∇φ(~
~ x)) = ρ(~x)
∇
0
Se obtiene la Ecuación de Poisson
~ 2 φ(~x) = − ρ(~x)
∇
0
~2=∇
~ ·∇
~ es el conocido Laplaciano. Con esto, hemos logrado reducir
Donde el operador ∇
aún más el problema de la electrostática, y todo consiste en encontrar un campo escalar que
satisfaga la ecuación de Poisson en una región del espacio con las condiciones de borde ade~ x) = −∇φ(~
~ x) y
cuadas. Una vez resuelta esta ecuación, se puede obtener el campo como E(~
luego todo el problema estará completo.
La ecuación de Poisson es una ecuación diferencial parcial, que en coordenadas cartesianas
equivale a
∂ 2 φ(x, y, z) ∂ 2 φ(x, y, z) ∂ 2 φ(x, y, z)
+
+
= − ρ(x, y, z)
∂x
∂y
∂z
0

En regiones del espacio libres de carga (ρ(~x) = 0), se debe resolver la Ecuación de Laplace
con condiciones de borde adecuadas
~ 2 φ(~x) = 0
∇

Las ecuaciones de Poisson y Laplace aparece en diversas ramas de la física, como en gravitación, dinámica de fluídos, propagación del calor, etc

---

### Página 9

Evidentemente, resolver las ecuaciones de Poisson o Laplace puede resultar analíticamente
muy complejo, sin embargo existen casos donde la simetría permite resolver éstas ecuaciones
sin mayor dificultad. En electrostática existen varios métodos para resolver problemas Poisson
- Laplace, algunos de ellos son
Método de las imágenes
Expansión del potencial en polinomios ortogonales
Funciones complejas analíticas, que resuelven Laplace en 2 dimensiones
Método de las funciones de Green
Métodos numéricos
Algunos de estos métodos serán desarrollados en detalle en capítulos siguientes

---

### Página 10

Problema
Una esfera de metal de radio R y carga q está rodeada por un cascarón esférico metálico de
radio interior a y radio exterior b. El cascarón no tiene carga neta
a) Encuentre la densidad superficial de carga en cada superficie
b) Encuentre el potencial en el centro utilizando infinito como punto de referencia
c) Si la esfera exterior se conecta a tierra bajando su potencial a cero (igual que en infinito),
¿Cómo cambian las respuestas anteriores?

#### Solución
a) Como la esfera de radio R es metálica (conductora), toda la carga debe estar concentrada
en su superficie. Dada la simetría esférica del problema, esta distribución de carga debe ser
uniforme, es decir
q
4πR2
Ahora, el cascarón es eléctricamente neutro, sin embargo en sus superficies (Sa y Sb ) se
induce carga de forma que el campo eléctrico en su interior sea nulo
σR =

~ x) = ~0 para a < r < b. Tomando una superficie Gaussiana esférica de
Debe tenerse que E(~
radio r, a < r < b
ˆˆ
 ~ 0
~ x0 ) = 0
x ) · E(~
 dS(~
S

~ x) es nulo en todos los puntos interiores del cascarón. Por otro lado
ya que E(~
ˆˆ
 ~ 0
~ x0 ) = Qint
x ) · E(~
 dS(~
0
S
luego Qint = 0, donde

---

### Página 11

Qint = q + σa 4πa2 = 0
y se obtiene la densidad superficial de carga en la superficie interior del cascarón
σa = −

q
4πa2

Como el cascarón es neutro, debe tenerse que
σa 4πa2 + σb 4πb2 = 0
−q + σb 4πb2 = 0
q
4πb2
Es decir, sobre la superficie interna se induce una carga total −q, y sobre la superficie externa, por supuesto, q.
σb =

b) Distinguimos 4 regiones, como se indica en la figura

Como las regiones I y III están contenidas en el interior de un conductor
~ x) = 0, ~x ∈ I, ~x ∈ III
E(~
Para encontrar el campo eléctrico en las regiones II, y IV , utilizamos la ley de Gauss.
Tomando una superficie esférica de radio r con R < r < a (región II), se tiene
ˆˆ
 ~ 0
~ x0 ) = 4πr2 E(r) = q
x ) · E(~
 dS(~
0
S
~
E(r)
=

q
r̂, R < r < a
4πr2 0

Del mismo modo, para una superficie esférica de radio r, con r > b (región IV ), se tiene
ˆˆ
 ~ 0
~ x0 ) = 4πr2 E(r) = q
x ) · E(~
 dS(~
0
S
~
E(r)
=

q
r̂, b < r
4πr2 0

---

### Página 12

Con esto, podemos calcular el potencial en el origen
ˆ ∞
~ x0 )
φ(0) =
d~x0 · E(~

tomando, por supuesto, un camino radial
~x0 = rr̂
d~x0 = drr̂
r ∈ [r, ∞]
φ(0) =

ˆ ∞

φ(0) =

ˆ R

drE(r) +

ˆ a

~
drr̂ · E(r)r̂
=

ˆ a

drE(r) +

R

drq
φ(0) =
+
R 4π0 r

ˆ ∞

ˆ b

drE(r)

drE(r) +

a

ˆ ∞
b

drq
q
=
4π0 r
4π0

ˆ ∞

drE(r)

b



+ −
b R a



c) Ahora, se tiene

~ x) = 0 para ~x ∈ III (interior de un conductor). Esto
Al igual que antes debe tenerse que E(~
simplemente se traduce en
q + σa 4πa2 = 0
(por ley de Gauss). Es decir, al igual que antes
q
4πa2
Además el potencial ahora es nulo sobre la superficie exterior Sb , esto quiere decir que
ˆ ∞
~ x0 ) = 0
φ(b) =
d~x0 · E(~
σa = −

b

para cualquier camino entre b y el infinito. Por supuesto, esto requiere que
~ x0 ) = 0∀~x ∈ IV
E(~

---

### Página 13

Notar que esto implica que la carga encerrada por una superficie Gaussiana contenida en
IV necesariamente es cero. Es decir, el cascarón ya no es un objeto eléctricamente neutro (se
debe inducir una carga neta en el, igual a −q).
q + σa 4πa2 + σb 4πb2 = q − q + σb 4πb2 = 0
σb = 0

---

### Página 14

Problema
Una esfera metálica se encuentra inicialmente descargada. Ahora imagine que una carga positiva
q es colocada en algún lugar (no necesariamente al medio) dentro de la esfera y sin tocar las
paredes.

a) ¿Qué carga se induce en la pared interior y exterior de la esfera? Indicar cualitativamente la
concentración de densidad de carga inducida . Describir cómo son las líneas de campo eléctrico
dentro y fuera de la esfera
b) Suponga que se mueve la carga q dentro de la cavidad. ¿Cambia la distribución en la superficie
exterior de la esfera?
c) Ahora se coloca la carga q en contacto con la superficie interior de la esfera.¿Cómo queda la
distribución de carga en la superficie interior y exterior?
d) ¿Qué sucede si ahora se acerca otra carga q 0 cerca de la superficie exterior del conductor?
#### Solución
a) La carga q en el interior de la esfera metálica inducirá una separación de carga en el metal. Sea
qint la carga total inducida en la superficie interior, y qout la carga total inducida en la superficie
exterior. Debido a que la esfera inicialmente se encuentra descargada, la ley de conservación de
la carga indica que se debe tener
qin + qout = 0
¿Cuánto vale qint ? Tomemos una superficie Gaussiana contenida enteramente dentro del
cascarón esférico como se muestra en la figura

La carga total encerrada por esta superficfie es
qenc = qint + q
~ es cero en el interior de metal, la ley de Gauss
Pero, debido a que el campo eléctrico E
indica

---

### Página 15

 ~
~ x) = (qint + q) = 0
x) · E(~
 dS(~

ˆˆ

0
De esta forma qint = −q, y entonces qout = q. La distribución de éstas cargas y sus respectivas
líneas de campo son como se aprecia en la siguiente figura

La carga negativa en la superficie interna se concentra mayoritariamente en la parte de la
esfera más cercana a la carga q. En contraste, la carga positiva de la superficie exterior se distribuye uniformemente sobre la superficie exterior. Ésto último debido a que la esfera metálica
es una superficie equipotencial, y la única forma de que esto suceda es que el campo sea radial
y uniforme sobre la superficie exterior
El campo eléctrico fuera de la esfera es
~
E(r)
=

1 q
r̂
4π0 r2

tal como si la carga q se encontrara en el centro del conductor
b) La distribución de carga en el exterior no cambia al mover la carga q en el interior, por
la misma razón anterior. Por supuesto, la carga inducida en el interior de la superficie si se
vuelve a distribuír en la medida que movemos q, para asegurar que el campo en su interior siga
~ = 0. Ésto resulta interesante, pues desde el exterior del conductor podríamos
siendo nulo E
saber cuanta carga se encuentra en el interior, pero no podremos asegurar en que posición se
encuentra.
c) Cuando la carga q toca la superficie interior, la carga inducida −q se concentrará enteramente en el punto de contacto y cancelará la carga q.
d) Si se acerca ahora otra carga q 0 al exterior de la esfera, entonces la carga se distribuirá en
la superficie exterior de forma de ser una equipotencial. La distribución de carga al interior no
cambia debido a la prescencia de una carga en el exterior. En otras palabras, si una cavidad
está encerrada en un conductor, ninguna distribución estática de carga en el exterior podrá producir campos dentro. Este principio se conoce como shielding, y explica el por qué los aparatos
eléctricos se encuentran en cubiertas metálicas. .

---

### Página 16

Problema
Dos cavidades esféricas, de radios a y b están contenidas en el interior de una esfera conductora
neutra de radio R. En el centro de cada cavidad hay una carga puntual qa y qb

a) Encuentre las densidades de carga superficiales
b) ¿ Cuál es el campo eléctrico fuera del conductor?
c) ¿Cuál es el campo dentro de cada cavidad?
#### Solución
a) Sobre las superficies Sa y Sb en cada cavidad se inducirá carga de forma de anular el efecto de
las cargas puntuales en el interior del conductor. Sean dos superficies S1 y S2 como se muestra
en la figura

Como S1 está contenida en el interior del conductor
ˆˆ
 ~ 0
~ x0 ) = 0 = Qint
x ) · E(~
 dS(~
0
S
se obtiene
Qint = 0 = qa + σa 4πa2 = 0
se obtiene la densidad superficial de carga inducida en la cavidad
σa =

−qa
4πa2

Del mismo modo, y utilizando la ley de Gauss con la superficie S2 , se obtiene
qb
4πb2
Como el conductor es neutro, se inducirá carga en la superficie exterior, de forma que
σb = −

−qa − qb + σR 4πR2 = 0
σR =

qa + q b
4πR2

---

### Página 17

b) El efecto de las cargas puntuales qa y qb es anulado mediante las cargas inducidas en las
cavidades. Con esto, el campo exterior posee una simetría esférica, y se puede obtener por la
ley de Gauss

 ~ 0
~ x0 ) = 4πr2 E(r) = qa + qb
x ) · E(~
 dS(~

ˆˆ

0

S

qa + q b
~
r̂, r > R
E(r)
=
4πr2 0
c) Dentro de la cavidad a, el campo es simplemente el de la carga puntual qa
~a =
E

qa r̂a
4π0 ra2

donde ra es la distancia desde un punto interior a la cavidad a a la carga puntual qa . Del
mismo modo, dentro de la cavidad b
~b =
E

qb r̂b
4π0 rb2

---

### Página 18

Problema
Un sistema de dos esferas de radio a y b (con a > b) conductoras cargadas posee una carga total
Q. Si ellas están separadas por una gran distancia y se les conecta con un alambre conductor de
dimensiones despreciables, calcule la carga total sobre cada esfera y la magnitud aproximada
del campo eléctrico sobre la superficie de cada una.

#### Solución
Sabemos lo siguiente: Cada esfera tiene una carga desconocida, pero su suma sí lo es
QA + QB = Q
Notemos que el sistema entero es un conductor, y por lo tanto, es un equipotencial. Además,
como las esferas están separadas por una gran distancia, entonces el campo producido por una
afecta de manera despreciable el campo de la otra. En la vecindad exterior de A, el campo es
de la forma
QA
r̂
2 A
4π0 rA

~A =
E
y en la vecindad de B es de la forma

QB
r̂
2 B
4π0 rB

~B =
E

Ahora usemos el hecho que el sistema completo es un conductor, y por lo tanto φ(a)−φ(b) =
ˆ a

~ A · d~l = QA
E
4πa0
∞
ˆ b
~ A · d~l = QB
φ(b) = −
E
4πb0
∞

φ(a) = −

De donde
QB
QA
=
4π0 a
4π0 b
Lo que equivale a
QA = QB

a
b

y usando que Q = QA + QB
QA =

aQ
a+b

---

### Página 19

bQ
a+b
Con esto, el campo eléctrico sobre la superficie de la esfera A tiene como magitud
QB =

EA =

aQ
4π0 (a + b)a2

EA =

Q
4π0 (a + b)a

~B =
E

bQ
4π0 (a + b)b2

~B =
E

Q
4π0 (a + b)b

y para la esfera B

De esta forma,
b
EA
= <1
EB
a
Es decir, el campo eléctrico sobre la esfera de radio menor es mayor que el campo sobre la
esfera de radio mayor. Los campos están en proporción inversa de los radios.
Éste es un efecto muy conocido, y ocurre cuando se carga un conductor que no es esférico, por
ejemplo, alguno que tenga una punta o un lado muy puntiaguido, como el de la figura

Entonces una cantidad relativamente pequeña de carga acumulada en la punta puede generar una densidad superficial de carga muy grande, y como consecuencia, un mayor campo justo
afuera. Este resultado es técnicamente muy importante, por que por ejemplo el aire se vuelve
conductor si el campo es demasiado grande.
Lo que sucede es que un ion cerca de la punta es acelerado por este campo intenso, y si
el campo es lo suficientemente grande, el ion puede obtener suficiente energía cinética antes
que golpee otro atomo y entonces podrá arrancar otro electrón de éste atomo. Como resultado,
se producen más y más iones. Este movimiento constituye una descarga. Si se desea cargar
entonces un conductor a un potencial alto y que no se produzcan descargas sobre él en el aire,
hay que asegurarse que la superficie sea suave, de forma que no hayan partes donde el campo
sea anormalmente alto

---

### Página 20

Problema
Considere dos placas metálicas conductoras de igual área A y separadas una distancia d. La
placa superior posee carga Q mientras que la placa inferior tiene carga −Q. Encontrar la capacidad del sistema

#### Solución
Para encontrar la capacidad C, primero debemos conocer la forma del campo eléctrico en
el interior del condensador (y luego determinar la diferencia de potencial entre placas). Por
supuesto que un condensador real tiene un largo finito, luego, las líneas de campo cerca del
borde de las placas se deforman, y el campo no está contenido totalmente entre las placas. En
la figura se aprecian las líneas de campo considerando el efecto de los bordes

De todas formas, ignoraremos éste tipo de efectos asumiendo una situación ideal, en donde
las líneas de campo son rectas . En el límite cuando las placas tienen largo infinito (o bien un
largo mucho mayor que la separación), el campo tendrá simetría plana y entonces podemos
usar la ley de Gauss para determinar su magnitud
ˆˆ
 ~ 0
~ x0 ) = qin
x ) · E(~
 dS(~
0
S

Elegimos una superficie de Gauss con forma de caja, de área A0 , tal como muestra la figura

---

### Página 21

Como el campo en el interior del conductor es nulo, sólo hay flujo sobre una de las tapas, de
esta forma la ley de Gauss queda
ˆˆ
 ~ 0
~ x0 ) = EA0 = qin = σA
x ) · E(~
 dS(~
0
0
S
de donde el campo eléctrico al interior del condensador tiene magnitud igual a
E=

σ
0

Ahora, la diferencia de potencial entre las placas del condensador se obtiene integrando el
campo sobre una curva que va desde la placa positiva hasta la placa negativa. Por supuesto
elegimos una trayectoria paralela en todo instante al campo
ˆ −
~ · d~l = −Ed
E
∆V = φ− − φ+ = −
+

Para obtener la capacidad, el término relevante es el valor absoluto de esta diferencia de
potencial, digamos
| ∆V |= Ed
De esta forma, la capacidad de un condensador plano está dada por
C=

Q
0 A
=
| ∆V |
d

Claramente depende únicamente de la geometría del condensador, y aumenta linealmente
con el área de las placas. Mientras mayor área, mayor capacidad de almacenar carga tiene para
una misma diferencia de potencial entre sus placas. Además es inversamente proporcional a la
distancia d entre placas, esto debido a que mientras menor es la distancia, menor es la diferencia
de potencial entre ambas para una carga fija Q.
Ahora, si tenemos un condensador plano de área cuadrada y de lado 10 cm, tendremos
A = 0, 1 × 0, 1 = 0, 01 m2
Suponiendo un ancho d = 1 cm, tenemos que la capacidad vale
C=

9 × 10−12 × 0, 01
0, 01

C = 9 × 10−12 F
Como ejemplo, si al condensador se aplica una diferencia de potencial de 1, 5 Volts (pila
2A), será capaz de almacenar una carga igual a
Q = C∆V = 1, 5 × 9 ∗ 10−12 = 1, 35 × 10−11

---

### Página 22

Problema
Considere un cilindro sólido de radio a rodeado por una cáscara cilíndrica de radio interior
b. La longitud de ambos cilindros es L y consideramos que este largo es mucho mayor que las
dimensiones de b−a, la separación entre cilindros, de manera que se puede despreciar los efectos
de borde. El condensador se carga de forma que el cilindro interior posea carga Q y el exterior
carga −Q. ¿Cuál es la capacidad?

#### Solución
Para obtener la capacidad debemos primero obtener el campo eléctrico en cualquier parte en
la región entre ambos conductores. Debido a la simetría cilíndrica del sistema, elegimos por
supuesto una superficie Gaussiana como un cilindro coaxial con longitud l < L y radio r donde
a < r < b. Usando la ley de gauss, tenemos

ˆˆ

ˆˆ


 ~ 0
~ x0 ) = 
x ) · E(~
 E(r)r̂ · dS r̂ = E(r)2πrl
 dS(~
S

S

Ahora, notar que por la simetría, para que los cilindros sean equipotenciales, el campo debe
ser radial a sus superficies, y luego, deben tener una densidad superficial de carga uniforme σ.
La carga encerrada por el cilindro de Gauss es, simplemente
2πalσ
0

qin =
Con esto,

aσ
0 r
Notar que el campo eléctrico es diferente de cero únicamente en la region a < r < b. Para
r < a la carga encerrada es qenc = 0 ya que la carga neta del conductor de radio a debe ubicarse
sobre su superficie. Del mismo modo, para r > b, la carga total encerrada es 0, debido a que un
condensador en su totalidad es neutro, es decir, cualquier superficie que encierre completamente
al condensador encierra una carga total igual a cero.
E(r) =

La diferencia de potencial está dada por
∆V = φb − φa = −
aσ
φb − φa = −
0

ˆ b
a

ˆ b

~ · d~l = −
E

ˆ b

dr
aσ
= − ln
0
a r

Er dr

a

 
b
a

---

### Página 23

donde el camino de integración tiene la dirección radial del campo eléctrico. Como era
de esperarse, el conductor exterior con carga negativa tiene menor potencial. De esta forma
tenemos
C=

Q
2π0 L
σ2πaL0
=
=
b
∆V
ln(b/a)
aσln( a )

Claramente sólo función de los factores geométricos. Consideremos un condensador cilíndrico de largo L = 5 cm
b = 0, 5 cm, a = 0, 1cm
C=

2π9 × 10−12 × 0, 05
= 1, 75 ∗ 10−12 F
ln(5)

Si conectamos una bateria de 5 Volt a este condensador, se almacenará una carga de
Q = C∆V = 8, 784 × 10−12 C

---

### Página 24

Problema
Considere un condensador esférico, que consiste de 2 esféras concéntricas de radios a y b. La
cáscara interior posee carga Q distribuída uniformemente sobre su superficie, y la esfera exterior
posee una carga igual pero opuesta −Q. Cuál es la capacidad de esta configuración?

#### Solución
El campo eléctrico sólo es distinto de cero en la región a < r < b. Usando la ley de Gauss con
una superficie esférica y de radio r como se muestra en la figura

 ~ 0
~ x0 ) = Er A = Er 4πr2 = Q
x ) · E(~
 dS(~

ˆˆ

0

S

de donde

1 Q
4π0 r2
La diferencia de potencial entre las dos cáscaras conductoras es
ˆ b
~
d~l · E
∆V = φb − φa = −
E(r) =

a

Q
φb − φa = −
4π0
de donde obtenemos

ˆ b

Q
dr
=−
4π0
a r



1 1
−
a b

Q
= 4π0
C=
| ∆V |





ab
b−a

Q
=−
4π0




b−a
ab



Ahora, para un conductor esférico aislado, también se puede hablar de capacidad, ésta se
obtiene tendiendo el radio b a infinito, luego, la capacidad de la esfera conductora de radio a es


ab
a
Ca = lím C = 4π0 lím
= 4π0 lím
a = 4π0 a
b→∞
b→∞
b→∞ (1 − )
b−a
b
Luego, para una esfera conductora de radio R, su capacidad es
C = 4π0 R

---

### Página 25

Este resultado también se podría obtener considerando que una esfera de radio R con carga
Q uniformemente distribuída sobre su superficie posee un potencial φ = 4πQ0 R , usando infinito
como referencia para el potencial, esto da
C=

Q
Q
=
= 4π0 R
| ∆V |
Q/4π0 R

---

### Página 26

Problema
Considere un conductor esférico de radio a dentro de otro de radio b. En el espacio entre ambos conductores se introduce un cascarón esférico (concéntrico) conductor de radios interno y
externo c y d, respectivamente. Si el conductor de radio a tiene carga Q y el exterior de radio
b tiene −Q, discuta que ocurre con la capacidad al introducir el cascarón

#### Solución
En el problema anterior se obtuvo que la capacidad de un condensador esférico está dada por


Q
ab
C=
= 4π0
| ∆V |
b−a

Veamos que ocurre cuando se introduce un conductor neutro entre a y b. Distinguimos 3
regiones, como se indica en la figura

Claramente el campo (de existir) en todo el espacio presenta una dependencia radial. Por
ley de Gauss,utilizando una superficie esférica de radio r, con a < r < c
ˆˆ
 ~ 0
~ x0 ) = E(r)4πr2 = Q
x ) · E(~
 dS(~
0
S
~
E(r)
=

Q
r̂, a < r < c
4π0 r2

Para la región II, dada por c < r < d
~ x) = 0, ∀~x ∈ II
E(~
pues corresponde al interior de un conductor. En consecuencia, se induce una carga −Q
sobra la superficie interna del cascarón. Dado que éste es neutro, sobre su superficie exterior sei
induce carga Q. Para la región III, exactamente el mismo resultado encontrado en la región I

---

### Página 27

~
se obtiene para el campo eléctrico E(r),
d < r < b. Vemos que este conductor altera el campo
eléctrico en el interior (con respecto al caso en que no está), donde la única diferencia es que
se anula para cierta región interior, claramente disminuyendo la diferencia de potencial entre el
conductor de radio a y el conductor de radio b, en consecuenctia, aumentará la capacidad del
sistema. En efecto
ˆ b
ˆ b
~
~
∆V = φa − φb =
d~x · E(~x) =
d~r · E(r)
a

a

donde se ha utilizado un camino radial para calcular la integral de línea, dada la naturaleza
del campo
ˆ c
ˆ d
ˆ b
~
~
~
∆V =
d~r · E(r) +
d~r · E(r) +
d~r · E(r)
a

c

d

~
y como E(r)
= 0 ∀c < r < d
∆V =

ˆ c

∆V =

ˆ c

a

∆V =
Pero c < d, entonces

ˆ b

~
d~r · E(r)

Q
+
4π0 r2

ˆ b

dr

Q
4π0 r2

1 1 1 1
− + −
a c d b



Q
4π0

dr

a

∆V =

~
d~r · E(r)
+




d

d

1 1 1 1
− + −
a b d c



Q
4π0

1 1
> ⇒ − <0
c
d
d c
En consecuencia, la diferencia de potencial entre el conductor interior y exterior disminuye
en comparación al caso en que no está el cascarón. De esta forma
C=

Q
∆V

es mayor que el del condensador esférico original

---

### Página 28

Problema
Tres cáscaras esféricas conductoras concéntricas muy delgadas poseen radios a,b, y c, respectivamente, siendo a < b < c. Inicialmente la cáscara interior está descargada, la del medio posee
una carga total negativa −Q y la externa una carga total positiva Q

a) Encuentre el potencial electrostático en cada una de las cáscaras conductoras
b) Si las cáscaras interior y exterior son conectadas mediante un alambre conductor muy delgado que está aislado al pasar por la cáscara central, ¿Cuál es ahora el potencial eléctrico de
cada una de las cáscaras? ¿Cuál es la carga en cada una de las esferas?
#### Solución
Distinguimos naturalmente tres regiones del espacio, dadas por I : r < a, II : a < r < b,
III : b < r < c, IV : r > d. En cada una de ellas el campo eléctrico posee dirección radial y su
magnitud depende únicamente de la distancia r al centro del conductor interno. Utilizando la
ley de Gauss para la región I : r < a
ˆˆ
 ~ 0
~ x0 ) = 0, ∀S ∈ I
x ) · E(~
 dS(~
S

~ x) = 0 ∀~x ∈ I (interior de un conductor). Para la región II
pues E(~
ˆˆ
 ~ 0
~ x0 ) = Qint = 0
x ) · E(~
 dS(~
0
S
pues la cáscara de radio a se encuentra inicialmente descargada. De esta forma, el campo
~ x) = 0 ∀~x ∈ II. Del mismo modo, utilizando una
eléctrico también es nulo en esta región, E(~
superficie esférica de radio r, con b < r < c
ˆˆ
 ~ 0
~ x0 ) = 4πr2 E(r) = −Q
x ) · E(~
 dS(~
0
S
−Q
~
r̂
E(r)
=
4π0 r2
Por último, para r > d
ˆˆ

 ~ 0
~ x0 ) = 0, ∀S ∈ IV
x ) · E(~
 dS(~
S

pues la carga encerrada por cualquier superficie contenida en la región IV es cero. En
resumen

si r < b
 0
−Q
~
r̂
si
b<r<c
E(r) = 4π0 r2

sir > c

---

### Página 29

El potencial en la cáscara exterior es
φ(c) =

ˆ ∞
c

~ x)
d~x0 · E(~

tomando por supuesto un camino radial ~x = rr̂, d~x0 = drr̂, r ∈ (c, ∞)
ˆ ∞
~
drr̂ · E(r)
=0
φ(c) =
c

El potencial en la cáscara de radio b es
ˆ ∞
ˆ c
−Q
φ(b) =
drr̂ · E(r)r̂ =
dr
4π0 r2
b
b
ˆ c
dr
Q
Q c
φ(b) = −
=
4π0 b r2
4π0 r b


Q
b−c
φ(b) =
4π0
bc

por último, el potencial en r = a es
ˆ b
ˆ c
ˆ ∞
ˆ ∞
drr̂ · E(r)r̂ =
drE(r) +
drE(r) +
drE(r)
φ(a) =
a

a

φ(a) =

ˆ c

b

drE(r) = φ(b) =

b

Q
4π0

c



b−c
bc



b) Ahora se tiene la siguiente configuración

Los conductores de radio a y c se encuentran unidas al mismo potencial. De esta forma,
la carga contenida inicialmente en estos dos conductores se distribuirá, donde por supuesto se
debe tener
Qa + Qc = Q
Definiendo las mismas regiones anteriores, nuevamente se tiene
~ x) = 0, ∀~x ∈ I
E(~
~ x) = 0, ∀~x ∈ IV
E(~

(región I es el interior de un conductor y la carga total del sistema sigue siendo nula). El
campo en la región II se obtiene con la ley de Gauss (superficie esférica de radio r, a < r < b)

---

### Página 30

 ~ 0
~ x0 ) = E(r)4πr2 = Qa
x ) · E(~
 dS(~

ˆˆ

0

S

Qa
r̂
4π0 r2
y del mismo modo, tomando una superficie esférica de radio r, b < r < c
ˆˆ
 ~ 0
~ x0 ) = E(r)4πr2 = −Q + Qa
x ) · E(~
 dS(~
0
S
~
E(r)
=

Qa − Q
~
r̂
E(r)
=
4π0 r2
El potencial en r = c es, por supuesto, nulo
ˆ ∞
drE(r) = 0
φ(c) =
c

además
ˆ c

ˆ c

Qa − Q
4π0 r2
b
b
b


ˆ
Qa − Q c 1
Qa − Q c − b
φ(b) =
dr 2 =
4π0
r
4π0
bc
b

φ(b) =

y

ˆ ∞

φ(a) =

drE(r) =

ˆ ∞

drE(r) =

drE(r) =

a

ˆ b

dr

drE(r) + φ(b)

a

ˆ b

Qa
Qa
φ(a) = φ(b) +
dr
=
φ(b)
+
4π0 r2
4π0
a
pero las cargas inducidas en a y c deben ser tal que



b−a
ab



=0



φ(a) = φ(c) = 0
luego
Qa − Q
φ(a) =
4π0



c−b
bc



Qa
+
4π0

b−a
ab

c−b
b−a
+ Qa
=0
bc
ab


c−b b−a
c−b
=Q
+
Qa
bc
ab
bc




c−b
ac − ab + bc − ac
b(c − a)
=Q
= Q(c − b)
→ Qa
Qa
abc
bc
a
φ(a) = (Qa − Q)

Finalmente



Qa = Q

a(c − b)
b(c − a)

---

### Página 31

Problema
Considere un condensador de placas paralelas cargadas con densidades σ y −σ , como muestra
la figura. Se arroja una carga q horizontalmente por el espacio entre las placas con velocidad
vx . Encuentre la trayectoria seguida por la partícula cargada y el ángulo que forma su vector
velocidad con la horizontal al momento de salir, considerando que l es lo suficientemente grande
como para que la carga no choque con alguna de las placas. Considere además que en todo
instante la carga q siente una fuerza electrostática

#### Solución
El campo eléctrico en la región entre placas, despreciando efectos de borde y considerando
d >> l está dado por
~ x) = σ ĵ + σ ĵ
E(~
20
20
~ x) = σ ĵ
E(~
0
Así, la fuerza electrostática que siente la carga q está dada por
σ
F~ = q ĵ
0
Notar que estrictamente esto es válido únicamente cuando q está quieta, sin embargo consideraremos que esta fuerza de interacción se mantiene a medida que la carga se mueve. De la
segunda ley de Newton
~a =

1 ~
qσ
ĵ
F =
m
m0

De esta forma, la cinemática de la carga está descrita por
x(t) = vx t
y(t) =

1 qσ 2
t
2 m0

y las velocidades
Vx (t) = vx
qσ
Vy (t) = at =
t
m0
donde el origen coincide con la posición inicial de la carga la momento de ingresar a la
región. Para obtener la trayectoria, utilizamos
t=

x(t)
vx

---

### Página 32

y entonces
y(x) =

1 qσ x2
2 m0 vx2

la trayectoria es una parábola en el plano x − y

El tiempo que demora la carga en llegar al extremo derecho es
d
vx
con esto, la velocidad vertical en el momento en que sale es
td =

Vy (td ) = atd =

qσ d
m0 vx





y el ángulo α está dado por
−1

α = tan

−1

α = tan



Vy (td )
Vx (td )
qσd
m0 vx2



---

### Página 33

Problema
Dos cilindros muy largos y concéntricos, de radios a y b, con b > a, se encuentran inicialmente
descargados. La región entre ambos se llena con una densidad homogénea de carga ρ, y luego
cada uno de los cilindros se conectan a tierra. Calcule, resolviendo a -la- Poisson, el potencial
y el campo eléctrico en la región interior.

#### Solución
En la región interior a ambos cilindros, es decir a < r < b, el potencial satisface la ecuación de
Poisson
~ 2 φ(~x) = − ρ(~x)
∇
0
Si usamos coordenadas cilíndricas, el potencial podría depender de ϑ, r y z. Sin embargo,
de la simetría del problema es evidente que
∂φ
=0
∂ϕ
con lo que φ = φ(r, z). Además, debido a que la longitud de los cilindros es mucho mayor a
(b−a), el potencial también debe ser simétrico con respecto a z. De esta forma, podemos despreciar efectos de borde y considerar que el potencial es sólo una función radial de la forma φ = φ(r)
Ahora, el Laplaciano en coordenadas cilíndricas para una función que sólo depende de r es
~ 2 φ(r) = 1 ∂ (r ∂φ(r) )
∇
r ∂r
∂r
De esta forma, la ecuación de Poisson se transforma en
ρ
1 ∂ ∂φ
(r ) = −
r ∂r ∂r
0
Equivalentemente

Luego

∂ ∂φ
rρ
(r ) = −
∂r ∂r
0
∂φ
r
=−
∂r

ˆ

dr

rρ
+C
0

∂φ
r2 ρ
+C
r
=−
∂r
20
∂φ
rρ
C
=−
+
∂r
20
r

---

### Página 34

Finalmente
φ(r) = −

ˆ

rρ
dr
+
20

ˆ

dr

C
r

r2 ρ
+ C ln r + A
40
Esta es la solución general de la ecuación de Poisson para un potencial de simétría cilíndrica,
dependencia radial, y densidad de carga constante. Ahora debemos imponer las condiciones de
borde adecuadas para que la solución sea única (Problema Poisson-Dirichlet)
φ(r) = −

Tenemos φ(a) = 0 Equivale a imponer que la superficie cilíndrica de radio a es una equipotencial conectada a tierra. Luego
φ(a) = −

a2 ρ
+ C ln a + A = 0
40

Además, φ(b) = 0, con esto
b2 ρ
+ C ln b + A = 0
40
Restando ambas ecuaciones, obtenemos
φ(b) = −

(b2 − a2 )ρ
0 = C(ln a − ln b) +
40
De donde obtenemos la constante C
C=

(a2 − b2 )ρ
40 ln(a/b)

De la primera condición despejamos A
A=
A=

a2 ρ
(a2 − b2 )ρ
− ln a
40
40 ln(a/b)

a2 ln(a/b)ρ − lna(a2 − b2 )ρ
40 ln(a/b)
A=

ρ(b2 ln a − a2 ln b)
40 ln(a/b)

Con esto, la solución del potencial para a < r < b es
φ(r) = −

r2 ρ
(a2 − b2 )ρ
ρ(b2 ln a − a2 ln b)
+
ln r +
40 40 ln(a/b)
40 ln(a/b)

Hermoso resultado. Ahora, para obtener el campo eléctrico, usamos el hecho
~ x) = −∇φ(~
~ x)
E(~
el operador gradiente en coordenadas cilíndricas para una función que sólo depende de r es
∂φ(r)
~
r̂
∇φ(r)
=
∂r
de manera que

---

### Página 35

∂φ
~
E(r)
= − r̂
∂r


(a
rρ
−
b
)ρ
~
−
E(r)
=
r̂
20 40 r ln(a/b)

~ es nulo, ya
que es el campo eléctrico para a < r < b. Para r < a es claro que el campo E
que no hay carga encerrada por el conductor interior.
Calculemos las densidades de cargas sobre los conductores. Para el conductor interior, tenemos que el campo eléctrico sobre su superficie tiene magnitud
E(a) =

(a2 − b2 )ρ
aρ
−
20 40 a ln(a/b)

La densidad de carga sobre la superficie de un conductor se relaciona con el campo eléctrico
según
σ
E=
0
Con esto la densidad de carga será


(a2 − b2 )ρ
aρ
−
σ1 = 0
20 40 a ln(a/b)
El campo eléctrico en la superficie del conductor exterior tiene magnitud
E(b) =

(a2 − b2 )ρ
bρ
−
20 40 b ln(a/b)



(a2 − b2 )ρ
bρ
−
20 40 b ln(a/b)

y la densidad de carga será
σ2 = 0



---

### Página 36

Problema
Considere el siguiente dispositivo

a) Determine el potencial y el campo eléctrico entre las placas.
b) Determine la capacidad por unidad de largo.
Desprecie los efectos de borde.
#### Solución
a) Sabemos que las líneas equipotenciales deben respetar la geometría del dispositivo. De esta
forma, las equipotenciales serán rectas radiales, es decir

Por lo tanto, las líneas de campo, al ser perpendiculares a las equipotenciales, deben seguir la
dirección θ̂, es decir, son arcos concéntricos.

Si suponemos que el dispositivo es muy largo en la dirección Z, entonces se puede suponer que
~ = E(r, ϑ)ϑ̂
E
Pero
∂φ
1 ∂φ
~ = −∇φ(r,
~
E
ϑ) = − r̂ −
ϑ̂
∂r
r ∂ϑ

---

### Página 37

Como el campo tiene dirección θ̂, ∂φ
=0
∂r
Luego, se tiene que el potencial sólo depende de ϑ, lo cual era de esperarse.
Planteamos la ecuación de Laplace en coordenadas cilíndricas:

~ 2φ = 0 = 1 ∂ φ = 0
∇
r2 ∂ϑ2
φ(ϑ) = Aϑ + B
Pero la placa inferior está conectada a tierra
φ(0) = 0 → B = 0
φ(ϑ0 ) = φ0 → A =
Finalmente
φ(ϑ) =

φ0
ϑ0

φ0
ϑ
ϑ0

~ ϑ) = − 1 φ0 ϑ̂
E(r,
r ϑ0
b)Calculemos la capacidad por unidad de largo.
Q
V
La carga por unidad de largo, Q, de una de las placas puede calcularse a partir de la
densidad de carga σ que aparece en cada placa del condensador. Su valor puede determinarse
directamente del campo eléctrico
C=

~ · n̂ = σ
E
0
De donde obtenemos
σ=

0 V0
r θ0

Así, el valor de Q es
Q=1

ˆ b

σ(r)dr =

a

ˆ b

0 φ0
φ0
b
dr = 0 ln( )
ϑ0
a
a r ϑ0

Finalmente
C=

b
0
ln( )
ϑ0
a

---

### Página 38

Problema
El campo eléctrico sobre la superficie de la Tierra está dado por la expresión
~
E(z)
= −(ae−αz + be−βz )k̂
Con α, β > 0, y z la altura desde la superficie de la tierra.
a) Determine la densidad de carga
b) Calcule la cantidad total de carga contenida en una columna vertical de sección S que se
extiende teóricamente desde x=0 hasta x = ∞

#### Solución
a) Para obtener la densidad de carga, utilizamos la forma diferencial de la ley de Gauss
~ · E(~
~ x) = ρ(~x)
∇
0
En este caso
~ · E(~
~ x) = ∂Ex + ∂Ey + ∂Ez
∇
∂x
∂y
∂z
~ en x e y son nulas, así
Las componentes de E
αae−αz + βbe−βz =

ρ(z)
0

Finalmente
ρ(z) = 0 (αae−αz + βbe−βz )

b) La carga total contenida en una columna vertical de sección S será
˚
ˆ ∞
ˆ ∞
Q=
ρ(z)d x = S
ρ(z)dz = S
0 (αae−αz + βbe−βz )dz

Q = S0 (a + b)

---

### Página 39

Problema
Se tienen dos cilindros conductores coaxiales, uno de radio a y el otro de radio b, conectados a
una diferencia de potencial V0 .
~ x) y φ(~x) en todo el espacio y σ en cada superficie.
Calcule ρ(~x),E(~

#### Solución
Utilizaremos la ecuacion de Laplace, esto es
~ 2 φ(r) = 0
∇
El laplaciano en coordenadas cilíndricas es
~ 2 φ = 1 ∂ (r ∂φ ) + 1 ∂ φ + ∂ φ
∇
r ∂r ∂r
r2 ∂φ2 ∂z 2

Si suponemos que el par de conductores cilíndricos es mucho más alto que su radio, entonces
se puede afirmar que el potencial no debe depender de la coordenada z, y por lo tanto ∂V
= 0.
∂z
Así mismo, como las características de los conductores no varían con el ángulo φ, también debe
cumplirse que ∂V
= 0.
∂φ
De esta forma la ecuación diferencial que debemos resolver es
1 ∂ ∂φ
(r ) = 0
r ∂r ∂r
Con condiciones de borde
φ(a) = V0 , φ(b) = 0
Esta ecuación se puede resolver integrándola directamente
φ(r) = A ln r + B
Esta solución general más las condiciones de borde nos entregan un sistema lineal de ecuaciones
A ln(a) + B = V0
A ln(b) + B = 0
De donde obtenemos
A=

V0
ln(a/b)

---

### Página 40

B=−

V0
ln b
ln(a/b)

Y el potencial entre las placas conductoras es
φ(r) =

V0
ln(r/b)
ln(a/b)

Válida solo entre a < r < b
~ x) = −∇φ(~
~ x), es decir
El campo eléctrico se puede calcular como E(~
E(r) = −

∂φ(r)
V0 1
=
,a < r < b
∂r
ln(b/a) r

~
E(r)

V0 1
r̂, a < r < b
ln(b/a) r

~ · E,
~ pero
La densidad de carga es ρ(r) = 0 ∇
~ · ( r̂ ) = 0
∇
r
Con lo que ρ(r) = 0, es decir, no hay densidad de carga entre los conductores.
Para determinar las densidades de carga superficial en cada conductor hay que usar el hecho
de que el campo en la superficie de un conductor cumple
~ · n̂ = σ
E
0
De esta forma, para el conductor a
σa = 0

V0
a ln(b/a)

Y para el conductor b
σb = −0

V0
b ln(b/a)

Todo el desarrollo anterior es válido para a < r < b.
En el cilindro interno, (r < a)
~
E(r)
=0
ya que dentro de un conductor en equilibrio electrostático el campo eléctrico es siempre
nulo. De esta forma
φ(r) = V0
ρ(r) = 0
Ahora, si r > b, para calcular el campo utilizamos
φ(b) − φ(∞) =

ˆ b
∞

~ · d~l =
E

ˆ b
∞

drE(r)

---

### Página 41

Pero φ(b) = 0, con lo que
E(r) = 0
Si el campo es 0, entonces φ = cte = φ(b) = 0, y ρ(r) = 0

---

### Página 42

Problema
Dos conos conductores concéntricos, cuyas ecuaciones en coordenadas esféricas son ϑ1 = π/6,
y ϑ2 = π/4 respectivamente, se muestran en la figura. Los conos son de extensión infinita y en
r = 0 están separados por una distancia infinitesimal. Si el cono interior está a un potencial de
~ en la región interior a
0 V, y el exterior a 50 V , determinar el potencial y el campo eléctrico E
ambos conductores

#### Solución
Sea V la región delimitada por ϑ1 < ϑ < ϑ2 . Si no hay densidad de carga libre en V , el potencial
satisface la ecuación de Laplace en V
~ 2φ = 0
∇
Dada la geometría del problema, es conveniente utilizar coordenadas esféricas




∂2φ
1 ∂
∂
∂φ
2 ∂φ
~
∇ φ(r, ϑ, ϕ) = 2
r
+ 2
sin ϑ
+ 2 2
r ∂r
∂r
r sin ϑ ∂ϑ
∂ϑ
r sin ϑ ∂ϕ2
El problema posee una clara simetría azimutal (el potencial claramente no depende del
ángulo polar ϕ). Además, debe existir una independencia en la coordenada r, pues la extensión
de los conos es infinita. De esta forma, el potencial debe ser únicamente función de ϑ, y se debe
resolver


∂φ
∂
~
∇ φ(r, ϑ, ϕ) = 2
sin ϑ
=0
r sin ϑ ∂ϑ
∂ϑ
Equivalentemente
∂
∂ϑ



∂φ
sin ϑ
∂ϑ

sin ϑ



=0

∂φ
= C1
∂ϑ

∂φ
= C1 cscϑ
∂ϑ
ˆ
dϑ
φ(ϑ) = C1
+ C2
sin ϑ
Además

ˆ

dϑ
= ln (tan ϑ/2) + C
sin ϑ

---

### Página 43

En efecto
d
(ln (tan ϑ/2) + C) =
sec2 ϑ/2 =
=
dϑ
tan ϑ/2
2 cos ϑ/2 sin ϑ/2
sin ϑ
con esto
φ(ϑ) = C1 ln (tan ϑ/2) + C2
Debemos imponer las condiciones de borde en las superficies conductoras. Se tiene
φ(ϑ1 ) = 0

φ(π/6) = C1 ln (tan π/12) + C2 = 0
Además
φ(ϑ2 ) = 50

φ(π/4) = C1 ln (tan π/8) + C2 = 50

Resolviendo el sistema para C1 y C2
50 = C1 (ln (tan π/8) − ln (tan π/12))
50 = C1 ln

C1 =
y

ln




tan π/8
tan π/12
tan π/8
tan π/12





C2 = −C1 ln (tan π/12)
Evaluando
C1 = 114,78834
C2 = 151,171411
y la solución es
φ(ϑ) = 114,78834 ln (tan ϑ/2) 151,171411

---

### Página 44

Para encontrar el campo eléctrico, utilizamos que
~ x) = −∇φ(~
~ x)
E(~
En coordenadas esféricas, y considerando que φ solo depende de ϑ
~ ϑ) = − 1 ∂φ ϑ̂
E(r,
r ∂ϑ
~ ϑ) = − 1 114,78834 ϑ̂
E(r,
r 2 sin ϑ

---

### Página 45

7.3.

Almacenamiento de Energía en un condensador

Los condensadores se suelen utilizar para el almacenamiento de energía eléctrica. La cantidad
de energía almacenada se puede pensar como el trabajo necesario para cargar al condensador,
así, durante el proceso de carga, una fuente de voltaje realiza el trabajo para mover cargas
desde una placa a la otra.

Imaginemos que el condensador está inicialmente descargado. En cada placa del condensador
hay muchas cargas negativas y positivas, pero estan en equilibrio, por lo que la carga total en
ambas es cero, y por consiguiente no existe ningún campo eléctrico entre ellas.
Comencemos extrayendo una carga positiva +dq de la placa inferior, llevándola hasta la superior. Al hacer esto, la placa de abajo queda con carga neta −dq. Se repite este proceso una
y otra vez, de esta manera cargamos el condensador y creamos un campo eléctrico donde no
había inicialmente.
Supongamos que la cantidad de carga en la placa superior en un instante dado es +q, y la
diferencia de potencial correspondiente es ∆V = q/C. Para traer otro elemento de carga +dq
a la placa superior, el trabajo necesario será dU = ∆V dq (Recordar la interpretación física
del potencial!). Si al final del proceso la carga en cada placa es de Q (en módulo), entonces el
trabajo realizado (energía entregada al sistema) durante el proceso es
U=

ˆ Q
O

dU =

ˆ Q

dq∆V =

ˆ Q

dq

q
1 Q2
=
C
2C

Esto es igual a la energía potencial eléctrica almacenada en un condensador
1 Q2
U=
= Q∆V = C∆V 2
2C

7.4.

Fuerzas entre conductores cargados

Pensemos ahora en una aplicación directa de esta idea de energía electrostática. ¿Cuál será la
fuerza entre las placas de un condensador cargado? Evidentemente debe existir una fuerza, ya
que ambas placas están cargadas con cargas de signo opuesto. Esta fuerza es fácil de obtener
usando el resultado para la energía electrostática de un condensador, usando el principio de
trabajo virtual.
Usemos este método para determinar la fuerza entre las placas de un condensador de placas
paralelas. Si imaginamos que el espacio entre las placas es incrementado una pequeña cantidad,
digamos ∆z, entonces el trabajo mecánico realizado para moverlas será
W = F ∆z

---

### Página 46

donde F es la fuerza entre las placas. Este trabajo debe ser igual al cambio en la energía
electrostática del condensador. Notando que
U=

1 Q2
2C

El cambio en la energía ( si la carga permanece constante) es
∆U = Q2 ∆( )
C
Luego, se tiene
F ∆z =

Q2
∆( )
C

Esto se puede reescribir como
F ∆z = −

Q2
∆C
2C 2

Esta fuerza, por supuesto, resulta de la atracción de las cargas en las placas, pero vemos que
no nos tenemos que preocupar en detalle sobre como están distribuídas, lo único que necesitamos
conocer es la capacidad C. En el límite cuando ∆z → 0
Q2 dC
F =− 2
=−
2C dz
En general





~
~
F = − ∇U

dU
dz



Q=cte

Q=cte

Notar que para éste cálculo hemos asumido que la carga en el condensador permanece
constante (es decir el condensador se encuentra aislado y no está eléctricamente conectado a
otros objetos, de forma que la carga total no cambia). Supongamos que en vez de eso hubieramos
imaginado que el condensador es mantenido a una diferencia de potencial constante y utilizamos
el desplazamiento virtual. Entonces habríamos tenido
U = CV 2
y entonces
F ∆z = V 2 ∆C
que en el límite equivale a
1 dC
F = V2
=
dz
En general





~
~
F = ∇U

dU
dt



V =cte

V =cte

---

### Página 47

7.5.

Condensadores en circuitos eléctricos

Un condensador se puede cargar al conectar sus terminales a una batería, que mantiene una
diferencia de potencial ∆V entre sus placas.

La conexión resulta de compartir cargas entre los terminales y las placas. Por ejemplo, si la
placa se conecta al terminal positivo, adquirirá carga positiva. Esto produce una reducción
momentánea de carga en los terminales, y por lo tanto decrece el potencial entre éstos. Luego,
reacciones químicas dentro de la batería transfieren más carga desde un terminal al otro para
compensar la pérdida y mantener el voltaje en su nivel inicial. La batería se puede pensar
entonces como una bomba de carga que trae carga Q de una placa a la otra

7.5.1.

Conexión en paralelo

Si tenemos dos condensadores, de capacidad C1 y C2 y con cargas Q1 y Q2 y se conectan
en paralelo, como en la figura

Las placas izquierdas de cada condensador son conectadas al terminal positivo de la batería y
están al mismo potencial que la terminal positiva. De forma similar, las placas derechas están
conectadas al terminal negativo y poseen el mismo potencial de éste. La diferencia de potencial
entre las placas de ambos condensadores es la misma, luego
C1 =

Q1
| ∆V |

Q2
| ∆V |
Estos condensadores se pueden ver como un condensador equivalente de capacidad equivalente
Ceq , con una carga Q administrada por la batería. Debe tenerse que
C2 =

de forma que

Q = Q1 + Q2 = C1 | ∆V | +C2 | ∆V |= (C1 + C2 ) | ∆V |
Ceq =

Q
= C1 + C2
| ∆V |

---

### Página 48

Luego, condensadores conectados en paralelo suman su capacidad, en general
Ceq = C1 + C2 + C3 + ... + CN =

N
X

Ci

i=1

7.5.2.

Conexión en serie

Supongamos que tenemos dos condensadores inicialmente descargados C1 y C2 conectados
en serie. Una diferencia de potencial | ∆V | se aplica entre ambos condensadores. La placa
izquierda del condensador 1 está conectada al terminal positivo y se carga positivamente con
+Q, mientras que la placa derecha del condensador 2 se conecta al terminal negativo y se
carga negativamente con −Q. ¿Qué sucede con las placas interiores? Ellas estaban inicialmente
descargadas, ahora ambas placas exteriores tienen cargas iguales pero opuestas. De esta forma
la placa derecha del condensador 1 adquirirá carga −Q y la placa izquierda del condensador 2
+Q

Las diferencias de potencial en los condensadores son
| ∆V1 |=

Q
C1

Q
C2
respectivamente. Vemos que la diferencia de potencial ∆V es simplemente la suma de las
diferencias individuales en cada condensador
| ∆V2 |=

| ∆V |=| ∆V1 | + | ∆V2 |
Estos dos condensadores se pueden reemplazar por un único condensador equivalente
Ceq =
Luego

Q
| ∆V |

Q
Q
Q
=
+
Ceq
C1 C2
y la capacidad equivalente para dos condensadores en serie está dada por
=
+
Ceq
C1 C2
En general
N
X
=
+
+ ... +
=
Ceq
C1 C2
CN
Ci
i=1

---

### Página 49

Problema
Considere la configuración de la figura. Encuentre la capacidad equivalente asumiendo que
todos los condensadores tienen la misma capacidad C

#### Solución
Para los condensadores conectados en serie, la capacidad equivalente esta dada por
N
X
=
+
+ ... +
=
Ceq
C1 C2
Cn
Ci
i=1

Por otro lado, para los condensadores conectados en paralelo, la capacidad equivalente es
Ceq = C1 + C2 + ... + CN =

N
X

Ci

i=1

Con esto, se obtiene el siguiente circuito equivalente

Notar que ahora tenemos 3 condensadores en paralelo. La capacidad equivalente es
Ceq = C(1 +

1 1
+ )= C
2 3

---

### Página 50

Problema
Se tiene un condensador plano con capacidad C1 y un condensador esférico con capacidad C2 .
El primero tiene cargas eléctricas q1 y −q1 y el segundo tiene cargas eléctricas q2 y −q2 . Luego
se conectan ambos condensadores como lo muestra la figura

a) Obtenga las nuevas cargas q10 , −q10 , q20 , −q20 una vez obtenido el equilibrio eléctrico
b) ¿Cuánto vale la pérdida de energía potencial eléctrica?
c) Según su sentido físico ¿dónde se pierde dicha energía?
d) Se coloca un dipolo eléctrico p~ entre las dos esferas del condensador eléctrico. ¿Qué sucede
con él?
#### Solución
a) Por conservación de la carga eléctrica, al conectar ambos condensadores, la carga total sólo
debe distribuírse, luego
q1 + q2 = q10 + q20
Al producirse el equilibrio eléctrico, los conductores unidos quedan a un mismo potencial,
digamos V , luego la diferencia de potencial entre sus terminales es común para ambos condensadores (están conectados en paralelo), esto es
q10 = C1 V
q20 = C2 V
Luego

q10
C1
=
q2
C2

Con esto
q10 =

C1 (q1 + q2 )
C1 + C2

q20 =

C2 (q1 + q2 )
C1 + C2

Ui =

1 q12
1 q22
+
2 C1 2 C2

b) La energía inicial está dada por

Y la energía final por

---

### Página 51

Uf =

1 q102 1 q202
+
2 C1 2 C2

La diferencia de energía es


1 q12
q22
q102
q202
Ui − Uf =
+
−
−
2 C1 C2 C1 C2


1 q12
q22
C1 (q1 + q2 )2 C2 (q1 + q2 )2
+
−
−
Ui − Uf =
2 C1 C2
(C1 + C2 )2
(C1 + C2 )2


1 q12
q22
(q1 + q2 )2
+
−
Ui − Uf =
2 C1 C2
C1 + C2

Ui − Uf =

1 (q1 C2 − q2 C1 )2
2 C1 C2 (C1 + C2 )

Esta es la pérdida de energía
c) La pérdida de energía se produce debido a que al conectar ambos condensadores, se produce una redistribución de carga en ellos (y entonces en un intervalo de tiempo breve circula
una corriente eléctrica en los conductores). La energía que se pierde corresponde a la energía
disipada en forma de calor en los conductores
d) El dipolo gira para orientarse en el sentido del campo eléctrico entre ambas cáscaras
esféricas. Además, como el campo no es uniforme en esta región, el dipolo se desplaza hacia
donde el campo eléctrico es más intenso, es decir, hacia la cáscara negativa

---

### Página 52

Problema
Hay dos condensadores con capacidades C1 y C2 conectados a una batería de potencial Vo . A
continuación se desconectan de la batería y se unen como en la figura de abajo

Calcular la nueva diferencia de potencial entre las placas en función de C1 , C2 y Vo
#### Solución
Se tiene que inicialmente C1 y C2 están conectados en serie, luego su capacidad equivalente es
+
=
Ceq1
C1 C2
Con esto

C1 C2
C1 + C2
Si Q1 es la carga almacenada por el sistema (igual en cada condensador), entonces
Ceq1 =

Ceq1 =
Q1 = Ceq1 Vo =

Q1
Vo
C1 C2
Vo
C1 + C2

Ahora, los condensadores se conectan en paralelo, por lo que en esta situación la capacidad
equivalente es
2Q1
V
Ojo! El factor 2 se debe a que inicialmente la carga total es 2Q1 (en cada condensador
inicialmente se almacena carga Q1 ). V es la nueva diferencia de potencial en los condensadores.
Ademas se tiene que
Ceq2 = C1 + C2
Ceq2 =

Así
C1 + C2 = 2



C1 C2
C1 + C2



Vo

V

---

### Página 53

de aquí obtenemos que
V =2
Finalmente



C1 C2
C1 + C2

V =2


Vo

C1 + C2

C1 C2
Vo
(C1 + C2 )2



---

### Página 54

Problema
Se tiene un circuito como el que se muestra en la figura.

a) Encontrar la carga de cada condensador cuando se cierra el interruptor S1.
b) Cuando se cierra también el interruptor S2
#### Solución
a) Cuando sólo se cierra el interruptor 1, se tiene

En este caso, C1 y C3 están en serie, asi como también C2 y C4 .
La capacidad equivalente entre C1 y C3 está dada por
=
+
= 1 + µ = (µF )−1
Ceq1
C1 C3
Con lo que

Ceq1 = µF
Del mismo modo, para la capacidad equivalente entre C2 y C4
1 1
=
+
= + (µF )− 1 = (µF )−1
Ceq2
C2 C4
2 4
Así
Ceq2 = µF
Por último, Ceq1 y Ceq2 están en paralelo, por lo que la capacidad total será
Ceq = Ceq1 + Ceq2 =

3 4
+ = µF
4 3

---

### Página 55

Con esto podemos determinar la carga total suministrada por la fuente, dada por
µF = 25µC
Ahora, sea Qi la carga acumulada por el condensador i. Se tiene que Q1 = Q3 , Q2 = Q4 , ya
que se encuentran en serie. Sea Vi la diferencia de potencial entre los terminales del condensador
i. Así
Q = ∆V C = 12

Q1 = 1µV1
Q2 = 2µV2
Q3 = 3µV3 = Q1
Q4 = 4µV4 = Q2

Además, los voltajes están relacionados según
12 = V1 + V3 = V2 + V4
Resolviendo este sistema, se tiene
Q1 = V1 , Q2 = 2V2 , Q1 = 36 − 3V1 , Q2 = 48 − 4V2
Así,
V1 = 36 − 3V1 , 2V2 = 48 − 4V2
De donde se obtiene finalmente
V1 = 9V, V2 = 8V, V3 = 3V, V4 = 4V
Por último
Q1 = 9µC
,Q2 = 16µC. Q3 = 9µC, Q4 = 16µC
Se comprueba que Q1 + Q2 = Q3 + Q4 = 25µC = Q
b) Ahora se tiene lo siguiente

---

### Página 56

Aquí, se tiene a los condensadores C1 y C2 en paralelo, lo mismo sucede con C3 y C4
Ceq1 = C1 + C2 = 3µF
Ceq2 = C3 + C4 = 7µF

Y estos dos se encuentran en serie, por lo que
1 1
= + (µF )− 1 = (µF )− 1
Ceq
3 7
Así
Ceq =

µF

Y la carga suministrada por la fuente será
Q=

21 · 12
V =
=
= 25, 2µC

Además, se tiene V1 = V2 , V3 = V4 , ya que se encuentran en paralelo. Así
V1 =

1µ
2µ
= V2 =
Q1
Q2

V3 =

3µ
4µ
= V4 =
Q3
Q4

Con esto
2Q1 = Q2
4Q3 = 3Q4
También debe tenerse que
Q1 + Q2 = Q3 + Q4 = 25, 2µC
Así
2Q1 = Q2 = 25, 2 − Q1 → Q1 = 8, 4µC
Q3 = 25, 2 − Q4 = 25, 2 − Q3 → Q3 = 10, 8µC
Q4 = Q3 = 14, 4µC

---

### Página 57

Problema
Considere el circuito de la figura

Primero se carga C1 cerrando el interruptor S1 . Después este interruptor es abierto, y el condensador cargado se conecta al otro condensador descargado cerrando al interruptor S2 . Calcule
la carga final en cada uno de los condensadores
#### Solución
Al cerrar el interruptor S1 , se conecta el condensador C1 a los terminales de la fuente de voltaje,
luego éste acumula una carga igual a
Q = CV = 6µ20 = 120µ(C)
Ahora, se abre el interruptor S1 y se cierra el interruptor S2 , es decir, se desconecta la fuente
de voltaje y se conectan ambos condensadores en paralelo. Básicamente lo que ocurre aquí es
una redistribución de la carga almacenada.
Sea Q1 la carga final en el condensador 1 , y Q2 la carga final en el condensador 2. Se sabe
que la carga total debe conservarse, es decir
Q = Q1 + Q2 = 120µ(C)
Y en cada condensador se tiene
Q1 = 6µV1
Q2 = 3µV2
Como están en paralelo, V1 = V2 , así
Q2
Q1
Q1
=2
=
→
6µ
3µ
Q2
De donde se obtiene, Q1 = 80µ (C), y Q2 = 40µ

---

### Página 58

Problema
Dos placas conductoras cuadradas de lado a se disponen con sus caras paralelas y muy próximas
entre sí. La distancia entre las placas es x, como se indica en la figura. Calcule la fuerza sobre
la placa B en las direcciones x y z cuando la diferencia de potencial entre las placas es Vo

#### Solución
La energía almacenada en el condensador es
U = CVo2
donde la capacidad está dada por
C(x, z) =

o a(a − z)
o A
=
x
x

De esta forma
~ = dU î + dU k̂
F~ = ∇U
dx
dz




(a
−
z)a
a
o
î +
k̂
F~ = − Vo
x2
x

1 o (a − z)a
1 o a
F~ = − Vo2
k̂
î − Vo2
x
x

---

### Página 59

#### Capítulo 8
Ecuaciones de Poisson y Laplace
Hemos concluído nuestra revisión de la electrostática demostrando que la teoría es completa.
En efecto, hemos visto que la conducta de un campo electrostático queda totalmente descrita por
dos ecuaciones diferenciales de primer orden, las cuales son consecuencia de la ley de Coulomb
y el principio de superposición
~ x) = ρ(~x)
~ · E(~
∇
0
~ × E(~
~ x) = ~0
∇
Ahora comenzaremos un estudio sobre la teoría del potencial. Esta nos brindará las herramientas matemáticas necesarias para resolver los problemas electrostáticos que se nos presentan en la práctica. Notar que la teoría electrostática ya está competa (es una teoría de
estructura muy simple, en efecto): solamente nos falta ampliar nuestra capacidad de aplicarla

8.1.

Ecuaciones de Poisson y Laplace

La segunda ecuación
es equivalente a

~ × E(~
~ x) = 0
∇
~ x) = −∇φ(~
~ x)
E(~

Combinada con la primera, se obtiene una ecuación diferencial de segundo orden
~ 2 φ(~x) = − ρ(~x)
∇
0
Esta es la ecuación de Poisson. En regiones libres de cargas tenemos
~ 2 φ(~x) = 0
∇
la ecuación de Laplace.

---

### Página 60

Interpretación del teorema fundamental
~2
∇

= −4πδ(~x − ~x0 )
| ~x − ~x0 |

Esta es la ecuación de Poisson para una carga q = 4π0 puntual localizada en el punto ~x0 .
(Ecuación singular de Poisson). Hemos establecido que
~ x) = −∇φ(~
~ x)
E(~
a partir de la ley de Coulomb
~ x) =
E(~

4π0

˚

d3 x0 ρ(~x0 )

R3

~x − ~x0
| ~x − ~x0 |3

utilizando el siguiente argumento
~x − ~x0
~
= −∇
| ~x − ~x |
| ~x − ~x0 |
~ x) = −∇
~ 1
E(~
4π0

˚

d3 x0

R3

Ahora lo vamos a demostrar directamente
Teorema

φ(x) =
4π0

˚

d3 x0

R3

ρ(~x0 )
| ~x − ~x0 |

ρ(~x0 )
| ~x − ~x0 |

es la solución de la ecuación de Poisson con condiciones de contorno adecuadas en el infinito,
es decir
~ 2 φ(~x) = − ρ(~x0 )
∇
0
C.C.S(∞)



⇔ φ(x) =
4π0

˚

d3 x0

R3

ρ(~x0 )
| ~x − ~x0 |

Demostración
1) Sea
φ(x) =
4π0
Luego

˚

d3 x0

R3

ρ(~x0 )
| ~x − ~x0 |

ρ(~x0 )
| ~x − ~x0 |
R3
˚
˚
4π
3 0
0 ~2
~
∇ φ(~x) =
=−
d x ρ(~x )∇
d3 x0 ρ(~x0 )δ(~x − ~x0 )
4π0
| ~x − ~x0 |
4π0
R3
R3
~ 2 φ(~x) = ∇
~2 1
∇
4π0

˚

d3 x0

~ 2 φ(~x) = − ρ(~x)
∇
0

---

### Página 61

2) Sea
~ 2 φ(~x) = − ρ(~x)
∇
0
~ 02 φ(~x0 )
∇
ρ(~x0 )
=−
~x − ~x0
0 | ~x − ~x0 |

con esto

~ 02 φ(~x0 )

=−
dx
| ~x − ~x |
0
R3

˚
pero

3 0∇

˚

d3 x0

R3

ρ(~x0 )
| ~x − ~x0 |

~ 0 φ(~x0 )
~0·∇
∇
| ~x − ~x0 |
| ~x − ~x0 |
R3
R3
˚
˚
o
n
~ 0 φ(~x0 )
∇
3 0 ~0
3 0~ 0
~
x
·
∇
+
d x ∇ φ(~x ) · ∇
d
=−
| ~x − ~x0 |
| ~x − ~x0 |
R3
R3
˚

=

˚

~0·∇
~0
d x φ(~x )∇
3 0

R3

=

˚

R3

~ 02
d x φ(~x )∇
3 0

~ 02 φ(~x0 )

3 0∇

dx

−
| ~x − ~x0 |

˚

=

˚

d3 x0


~0
d x ∇ · φ(~x0 )∇
3 0~ 0

R3

 ˆˆ
~0

~ x0 ) · ∇ φ(~x )
+
d
S(~


| ~x − ~x0
| ~x − ~x0 |
S(∞)

ˆˆ
ˆˆ
~ 0
~x − ~x0


~
~ x0 ) · E(~x )
+
φ(~
x
d
S(~
x
)
·
)
−
d
S(~




| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
S(∞)
S(∞)

Ahora supondremos que las condiciones de borde son apropiadas (y que entonces las integrales de superficie son nulas)
˚
˚
x0 )
3 0 ρ(~
−
= −4π
dx
d3 x0 φ(~x0 )δ(~x − ~x0 ) = −4πφ(~x)
0
| ~x − ~x |
R3
R3
˚
ρ(~x0 )
d3 x0
φ(~x) =
4π0
| ~x − ~x0 |
R3

8.1.1.

Acerca de las condiciones en el infinito

Veremos que
ˆˆ



lím φ(~x) = 0 ⇒  

|~
x|→∞

S(∞)

~ x0 ) ·
dS(~

ˆˆ

~
lím | ~x || ∇φ(~x) |= 0 ⇒  

|~
x|→∞

~x − ~x0
φ(~x0 ) = 0
| ~x − ~x0 |3

S(∞)

~ x0 ) ·
dS(~

~ x0 )
E(~
| ~x − ~x0 |

la segunda de ellas ya se discutió en el teorema de completitud de Helmholtz. Lo que se hace
es escoger como superficie de integración una esfera centrada en ~x y de radio a =| ~x − ~x0 |→ ∞

ˆˆ




S(∞)

~ x0 ) ·
dS(~

ˆˆ
˛ 4π
~x − ~x0

φ(~x ) = lím   dΩ(n̂)φ(~x + an̂) =
dΩ(n̂) lím φ(~x0 )
a→∞
a→∞
| ~x − ~x0 |3
S(a)

---

### Página 62

luego debe tenerse que
lím

|~
x−~
x0 |→∞

φ(~x0 ) = 0 ⇒ lím φ(~x) = 0
|~
x|→∞

del mismo modo
ˆˆ
~ x0 )
E(~

~
~ x + an̂)
= lím   dΩ(n̂)an̂ · E(~
dS(~x ) ·
a→∞
|
~
x
−
~
x
|
S(∞)
S(a)
˛ 4π
~ x + an̂)
dΩ(n̂) lím an̂ · E(~
=

ˆˆ




a→∞

luego basta tener

~ x) = 0
lím ~x · E(~

|~
x|→∞

y

~ x) ≤ lím | ~x | · | E(~
~ x) |
lím ~x · E(~

|~
x|→∞

8.1.2.

|~
x|→∞

Corolario: Condición de validez para ρ(~x)

De la condición necesaria para el potencial
lím φ(~x) = 0

|~
x|→∞

|~
x|→∞ | ~
|~
x|→∞
x − ~x0 |
R3
˚
˚
3 0
=
= lím
d x ρ(~x ) lím
d3 x0 ρ(~x0 ) = 0
|~
x|→∞ | ~
x | |~x|→∞ | ~x |
R3
R3
lím

si

ρ(~x0 )
=
dx
| ~x − ~x0 |
R3

˚

3 0

−∞ <

¨

R3

˚

d3 x0 ρ(~x0 ) lím

d3 x0 ρ(~x0 ) < ∞

Basta que la carga total de las fuentes sea finita (razonable!)
Luego, como corolario

˚
~ 2 φ(~x) = − ρ(~x0 )
x0 )
∇
3 0 ρ(~

˝
d
x
⇒
φ(x)
=
4π0
| ~x − ~x0 |
d3 x0 | ρ(~x0 ) |< ∞
R3
R3
Pero en la práctica, éste no es el problema de contorno típico de la electrostática
Nota sobre el potencial en el infinito
Es bien sabido que a la función potencial siempre es posible sumarle una constante arbitraria
finita, ya que, obviamente, semejante adición no modifica en nada el campo electrostático que
ese potencial determina. Sumarle una constante al potencial equivale a cambiar arbitrariamente
su valor en el infinito. Sin embargo, pareciera concluirse de nuestro análisis previo que el valor
del potencial en el infinito está perfectamente determinado por la naturaleza de las fuentes

---

### Página 63

cargadas. Esta situación, aparentemente paradojal, merece ser estudiada con cierto cuidado.
Sea

~ 2 φ(~x) = − ρ(~x0 )
∇
0
˝
d3 x0 | ρ(~x0 ) |< ∞
R3
Luego

˚
ρ(~x0 )
φ(~x) =
d3 x0
4π0
| ~x − ~x0 |
R3
lím ρ(~x) = 0
|~
x|→∞

~ x) |= 0
lím | ~x || ∇φ(~

|~
x|→∞

Transformemos este potencial
φ(~x) → ψ(~x) = φ(~x) + ψ∞
Se tiene ahora
a)
~ 2 ψ(~x) = ∇
~ 2 [φ(~x) + ψ∞ ] = ∇
~ 2 φ(~x)
∇
~ 2 ψ(~x) = − ρ(~x)
∇
0
b)
ψ(~x) =
4π0

˚

d3 x0

R3

ρ(~x0 )
+ ψ∞
| ~x − ~x0 |

c) lím|~x|→∞ ψ(~x) = lím|~x|→∞ (φ(~x) + ψ∞ ) = lím|~x|→∞ φ(~x) + ψ∞
lím ψ(~x) = ψ∞

|~
x|→∞

~ [φ(~x) + ψ∞ ] = ∇φ(~
~ x)
d) ψ(~x) = ∇
~ x) |= 0
lím | ~x || ∇ψ(~

|~
x|→∞

Veamos ahora si todo ésto es consistente
˚

R3

−4π

˚

R3

~ 02 ψ(~x0 )

3 0∇

dx

| ~x − ~x0 |
ˆˆ


d x ψ(~x )δ(~x − ~x ) +  
3 0

= −4π

S(∞)

˚

d3 x0

R3

ρ(~x0 )
| ~x − ~x0 |
ˆˆ



dΩ(~x , ~x)ψ(~x ) +  

S(∞)

= −4πψ(~x) + 4πψ∞ + 0

luego hay consistencia y no hay paradoja alguna!

~ x0 ) ·
dS(~

~ 0 ψ(~x0 )
∇
| ~x − ~x0 |

---

### Página 64

8.2.

Ecuación Integral de Poisson: Teoremas de Green

A) Problemas simples de la electrostática
Los problemas formalmente más simples de la electrostática consisten en calcular φ(~x) para
todos los puntos del espacio, habiéndose dado la distribución de las fuentes eléctricas ρ(~x) (por
lo general, localizadas dentro de una región V ), sin condiciones de contorno prescritas para
~ x) en el infinito
φ(~x) o E(~

la solución de estos problemas simples es, formalmente, inmediata
˚
ρ(~x0 )
φ(~x) =
d3 x0
4π0
| ~x − ~x0 |
V
~ x) = −∇φ(~
~ x)
E(~

B) Problemas de contorno
Pero, por lo general, los problemas prácticos de la electrostática se refieren a regiones (finitas
o infinitas) que solamente abarcan una porción del espacio, con o sin cargas en su interior, y
con condiciones de contorno presecritas en las superficies que las limitan. (Por ejemplo, esta
superficie de contorno puede representar un conductor a un potencial fijo). La solución formal
de éstos problemas de contorno no es tan sencilla. Para manejar los problemas de contorno
necesitaremos nuevas herramientas matemáticas que procedemos a construír

8.3.

Teoremas de Green

A partir del teorema de la divergencia
˚
ˆˆ

3 0~
~
d x ∇ · A = 
V

S(V )

~ ·A
~
dS

y utilizamos un campo vectorial de la forma
~ = φ∇ψ
~
A
con φ, ψ, dos campos escalares. Recordar que


~ ·A
~=∇
~ · φ∇ψ
~
~ · ∇ψ
~ + φ∇
~ 2ψ
∇
= ∇φ

---

### Página 65

˚

V



~2



ˆˆ


~ · ∇ψ
~ + φ∇ ψ = 
d x ∇φ

3 0

S(V )

Se obtiene la Primera Identidad de Green
˚
 ˆˆ


3 0 ~
~ + φ∇
~ ψ = 
d x ∇φ · ∇ψ

V

~ · ∇ψφ
~
dS

dSφ

S(V )

∂ψ
∂n

donde

~ = ∂ψ
n̂ · ∇ψ
∂n
es la derivada direccional de ψ en la dirección normal a S(V )
~ = ψ ∇φ,
~ y obtenemos el siguiente par de identidades
Ahora, también es posible escoger A
de Green
˚
 ˆˆ

∂ψ

3 0 ~
~
~
d x ∇φ · ∇ψ + φ∇ ψ =   dSφ
∂n
S(V )
V
ˆ
ˆ
˚


∂φ

~ · ∇φ
~ + φ∇
~ 2φ = 
d3 x0 ∇ψ
  dSψ
∂n
V
S(V )
Restándolas, obtenemos el Teorema de Green
˚
n
o ˆˆ

~
~
d x φ∇ ψ − ψ ∇ φ =  



∂ψ
∂φ
ds φ
−ψ
∂n
∂n
S(V )

V

8.3.1.

Ecuación Integral de Poisson

Usaremos el teorema de Green para transformar la ecuación de Poisson en una ecuación
integral en la región de interés. Elijamos
ψ(~x, ~x0 ) =
Sea

| ~x − ~x0 |

~ 02 φ(~x0 ) = − ρ(~x )
∇
0
~ 02 ψ(~x, ~x0 ) = −4πδ(~x − ~x0 )
∇

Luego, integrando sobre la región de interés V
˚

V


˚
o
n
0 ~ 02
0 ~ 02
3 0
d x φ(~x )∇ ψ(~x, ~x ) − ψ(~x, ~x )∇ φ(~x ) = −4π
d x φ(~x0 )δ(~x − ~x0 ) −
3 0

V



x, ~x0 )
x0 )
0 ∂ψ(~
0 ∂φ(~
dS(~x ) φ(~x )
− ψ(~x, ~x )
=
∂n0
∂n0
S(V )
(
)
ˆˆ
∂φ(~
x0 )

0 ∂
∂n0
=   dS(~x ) φ(~x ) 0
−
∂n | ~x − ~x0 | | ~x − ~x0 |
S(V )
ˆˆ




ρ(~x0 )
4π0 | ~x − ~x0 |



---

### Página 66

Se obtiene la ecuación integral de Poisson

φ(~x)

d x δ(~x−~x ) =
4π0
V

˚

3 0

)
( ∂φ(~x0 )
ˆˆ
1 
ρ(~x0 )
∂
∂n
+
− φ(~x ) 0
dx
x)
  dS(~
| ~x − ~x0 | 4π S(V )
| ~x − ~x0 |
∂n | ~x − ~x0 |
V

˚

3 0

Consideremos ~x ∈ V
~x ∈ V →
dS(~x0 )

˚

V

d3 x0 δ(~x − ~x0 ) = 1

∂
~0
~ x0 ) · ~x − ~x
)n̂(~
x
)
·
∇
=
dS(~
x
=
d
S(~
∂n0 | ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |3

dS(~x0 )

∂
~ x0 ) · ~x − ~x
=
−d
S(~
∂n0 | ~x − ~x0 |
| ~x0 − ~x |3

dS(~x0 )

∂φ(~x0 )
~ x0 ) · ∇
~ 0 φ(~x0 )
= dS(~
∂n0

y entonces la ecuación interior es
φ(~x) =

ˆˆ
ˆˆ
~ x0 ) · ∇
~ 0 φ(~x0 )
1   dS(~
1 
ρ(~x0 )
~ x0 ) · ~x − ~x φ(~x0 )
dx
d
S(~
+
+




| ~x − ~x0 | 4π S(V )
| ~x − ~x0 |
4π S(V )
| ~x0 − ~x |3
V

˚

3 0

Primera Observación
Si V = R3 , S(V ) → S(∞)
ˆˆ




S(V )

~ x0 ) ·
dS(~

~x0 − ~x
φ(~x0 ) →
| ~x0 − ~x |3

ˆ 4π

dΩ(x̂) lím
φ(~x0 )
|~
x |→∞

y también
ˆˆ
~ x0 ) · ∇
~ 0 φ(~x0 )
~ 0 x0 ) |
dS(~

0 | ∇ φ(~
|
|≤
dS(~
x
)

| ~x − ~x0 |
| ~x − ~x0 |
S(V )
S(V )
ˆˆ
ˆ 4π
dS(~x0 )

~
~ 0 φ(~x0 ) |
= 
| ~x − ~x || ∇ φ(~x ) |→
dΩ(x̂) lím
| ~x − ~x0 || ∇
0 |2
0 |→∞
|~
x
|
~
x
−
~
x
S(V )
ˆˆ




Luego

ˆˆ



lím
φ(~x ) = 0 ⇒  

|~
x |→∞

S(∞)

~ x0 ) ·
dS(~

~x0 − ~x
φ(~x0 ) = 0
| ~x − ~x |

~ x0 ) · ∇
~ 0 φ(~x0 )
dS(~
| ~x − ~x0 |
S(∞)

ˆˆ

~
lím
| ~x || ∇ φ(~x ) |= 0 ⇒  

|~
x |→∞

y entonces
φ(~x) =
4π0

ρ(~x0 )
dx
| ~x − ~x0 |
R3

˚

3 0

---

### Página 67

esto impone sobre ρ las condiciones de consistencia dadas que ya conocemos
˚
d3 x0 | ρ(~x0 ) |< ∞
R3

Segunda observación
Si la región de interés V está libre de cargas
~x ∈ V : ρ(~x) = 0
entonces, se obtiene la ecuación integral de Laplace
( ∂φ(~x0 )
)
ˆˆ
∂
1 
∂n
x)
φ(~x) =
− φ(~x ) 0
  dS(~
4π S(V )
| ~x − ~x0 |
∂n | ~x − ~x0 |

8.4.

Condiciones de Contorno: Unicidad de las soluciones

A) Los problemas de contorno en electrostática son de la forma
~ 2 φ(~x) = −
~x ∈ V : ∇

ρ(~x)
0

∂φ
~x ∈ S(V ) : Condiciones de contorno para φ o para ∂n

o bien
~ 2 φ(~x) = 0
~x ∈ V : ∇

∂φ
~x ∈ S(V ) : Condiciones de contorno para φ o para ∂n

Surge la cuestión sobre cuáles son las condiciones de contorno adecuadas para que dentro
del volumen de interés V la solución sea matemáticamente única, y físicamente razonable.
La experiencia física nos hace esperar que un problema único de potencial se obtiene:
a) Especificando el potencial φ(~x) sobre una superficie cerrada S(V ) que limita la región de
interés V (problema de Dirichlet)
~x ∈ S(V ) : φ(~x) = φD (~x)

~ x) sobre el contorno cerrado S(V ) de la región de
b) Especificando el campo eléctrico E(~
interés V (problema Neumann)
~ x) = E
~ N (~x)
~x ∈ S(V ) : E(~

En efecto vamos a demostrar que tanto el problema de Dirichlet como el problema de Neumann dan origen a una solución única

---

### Página 68

8.4.1.

Unicidad para problemas de contorno Dirichlet

El problema Poisson Dirichlet tiene la siguiente forma
~ 2 φ(~x) = − ρ(~x)
~x ∈ V : ∇
0
~x ∈ S(V ) : φ(~x) = φD (~x)
Sean φ1 (x) y φ2 (x) dos soluciones de este problema. Se define
ψ(~x) = φ2 (~x) − φ1 (~x)
Evidentemente ψ(~x) es solución de la ecuación de Laplace con condiciones de contorno
Dirichlet Homogéneas
~ 2 ψ(~x) = 0
~x ∈ V : ∇

~x ∈ S(V ) : ψ(~x) = 0

Usemos la primera identidad de Green
˚
n
o ˆˆ

~
~
~
d x ∇ψ · ∇ψ + ψ ∇ ψ =  
V

dSψ

S(V )

˚

V

~ · ∇ψ
~ =
d3 x∇ψ

Pero
˚

V

˚

V

∂ψ
=0
∂n

~ |2 = 0
d3 x | ∇ψ

~ |≥ 0
| ∇ψ
~ |2 = 0 ⇒ ∇ψ(~
~ x) = ~0, ~x ∈ V
d3 x | ∇ψ

Luego ψ(~x) es constante para ~x ∈ V . Pero entonces, como
se tiene

ψ(~x) = 0, ~x ∈ S(V )
ψ(~x) = 0, ~x ∈ V

y por lo tanto

Luego, para ~x ∈ V

ψ(~x) = φ2 (~x) − φ1 (~x) = 0, ~x ∈ V
φ2 (~x) = φ1 (~x)

Obsérvese el importante resultado

y también


~ 2 ψ(~x) = 0
~x ∈ V : ∇
⇒ ψ(~x) = 0, ~x ∈ V
~x ∈ S(V ) : ψ(~x) = 0

~ 2 ψ(~x) = 0
∇
⇒ ψ(~x) = 0, ∀x
~x ∈ S(∞) : ψ(~x) = 0

---

### Página 69

8.4.2.

Unicidad para condiciones de contorno de Neumann

El problema Poisson-Neumann tiene la forma
~ 2 φ(~x) = −
~x ∈ V : ∇
~x ∈ S(V ) :

ρ(~x)
0

∂φ(~x)
= −EN (~x)
∂n

El desarrollo es análogo al caso anterior. Sean
φ1 (~x), φ2 (~x)
dos soluciones del problema Poisson-Neuman en V . Definimos
ψ(~x) = φ2 (~x) − φ1 (~x)
Entonces ψ(~x) es solución de la ecuación de Laplace con condiciones de contorno de Neumann Homogéneas
~ 2 ψ(~x) = 0
~x ∈ V : ∇
~x ∈ S(V ) :

∂φ(~x)
=0
∂n

Ahora
˚

V

ˆˆ

~
d x | ∇ψ | =  

dSψ

S(V )

∂ψ
=0
∂n

luego
~ = ~0
∇ψ
y ψ(~x) es constante para ~x ∈ V . Pero ahora
∂ψ
= 0, ~x ∈ S(V )
∂n
Por lo tanto
ψ(~x) = C, ~x ∈ S(V )
luego
φ2 (~x) = φ1 (~x) + C, ~x ∈ V
Observemos que

)
~ 2 ψ(~x) = 0
~x ∈ V : ∇
⇒ ψ(~x) = C, ~x ∈ V
x)
=0
~x ∈ S(V ) : ∂ψ(~
∂n

La constante aditiva C es arbitraria y carece de importancia física pues no altera al campo
~ x)
eléctrico E(~

---

### Página 70

8.4.3.

Condiciones de Contorno de Cauchy

Un problema Poisson-Cauchy tendría la siguiente forma
~ 2 φ(~x) = − ρ(~x)
~x ∈ V : ∇
0

φ(~x) = φC (~x)
~x ∈ S(V ) ∂φ(~x)
= −EC (~x)
∂n
Pero este problema lo podemos desglosar

~ 2φ = − ρ
~x ∈ V : ∇
0
⇒ φ(~x) = φD (~x), ~x ∈ V
~x ∈ S : φ = φC
Este problema de Poisson Dirichlet posee solución única!
)
~ 2φ = − ρ
~x ∈ V : ∇
0
⇒ φ(~x) = φN (~x), ~x ∈ V
∂φ
= −EC
~x ∈ S : ∂n
Este problema de Poisson Neumann también posee solución única. Los datos de Cauchy son
{φC , EC } sobre S. (Ambas son funciones arbitrarias). Al resolver el problema Poisson Dirichlet
~ C , al resolver el problema Poisson
obtenemos una solución φD , haciendo caso omiso del dato E
Neumann obtenemos φN , haciendo caso omiso de φC . Es obvio que, en general, resultará
 ∂φD (~x)
x)
N (~
6= ∂φ∂n
= −EC (~x)
∂n
~x ∈ S(V ) :
φN (~x) 6= φD (~x) = φC (~x)
Luego no hay consistencia: no existe, en general, solución de la ecuación de Poisson con
condiciones de contorno de Cauchy sobre una superficie cerrada

8.5.

Funciones de Green: Solución formal a los problemas de contorno

El problema típico en electrostática es resolver un problema de contorno de la forma
~ 2 φ(~x) = − ρ(~x)
~x ∈ V : ∇
0
~ 2 φ(~x) = 0
~x ∈ V : ∇
con condiciones de borde de Dirichlet
~x ∈ S(V ) : φ = φD
o de Neumann
~x ∈ S(V ) :

∂φ
= −EN
∂n

la solución de este problema es única.
Una carga puntual (positiva) 4π0 ubicada en el punto ~x se representa por la densidad de carga
singular
ρ(~x0 ) = 4π0 δ(~x − ~x0 )
y su potencial en el punto ~x0 es

---

### Página 71

ψ(~x, ~x0 ) =

| ~x − ~x0 |

Obsérvese que el rol de ~x y ~x0 puede invertirse. Este potencial unitario satisface la ecuación
de Poisson singular
~ 02
= −4πδ(~x − ~x0 )
∇
| ~x − ~x |
Vamos a generalizar esta idea

Funciones de Green G(~x, ~x0)

8.6.

En general, son aquellas funciones que satisfacen la ecuación de Poisson singular
~ 02 G(~x0 , ~x) = −4πδ(~x, ~x0 ), ~x0 ∈ V
∇

Sea L(~x0 , ~x) una solución de la ecuación de Laplace en el interior de una región V , ~x0 ∈ V
~ 02 L(~x0 , ~x) = 0
∇
entonces podemos considerar
G(~x, ~x0 ) =

+ L(~x, ~x0 )
| ~x − ~x |

Esta es una función de Green dentro de la región V . Consideremos la estructura
~x0 ∈ V

~ 02 φ(~x0 ) = − ρ(~x )
∇
0
~ 02 G(~x0 , ~x) = −4πδ(~x − ~x0 )
∇
G(~x0 , ~x) =

| ~x0 − ~x |

+ L(~x0 , ~x)

~ 02 L(~x, ~x0 ) = 0
∇
Entonces, usando la segunda identidad de Green
˚



∂φ(~x0 )
x0 , ~x)
0 ∂G(~
dS(~x ) G(~x , ~x)
− φ(~x )
∂n0
∂n0
S(V )

n
o ˆˆ

0 ~ 20
~
d x G(~x , ~x)∇ φ(~x ) − φ(~x )∇ G(~x , ~x) =  
3 0

V

para ~x ∈ V , resulta


˚
d x − G(~x , ~x)ρ(~x ) + 4πφ(~x )δ(~x − ~x) = −
d3 x0 ρ(~x0 )G(~x0 , ~x) + 4πφ(~x)


V
V

˚

3 0

=



∂φ(~x0 )
x0 , ~x)
0 ∂G(~
dS(~x ) G(~x , ~x)
− φ(~x )
∂n0
∂n0
S(V )

ˆˆ




---

### Página 72

o sea, con ~x ∈ V en general se tiene
φ(~x) =
4π0

ˆˆ
ˆˆ
1 
x0 )
1 
x0 , ~x)
0 ∂φ(~
0 ∂G(~
d x ρ(~x )G(~x , ~x)+
dS(~
x
)
G(~
x
,
~
x
)−
dS(~
x
)φ(~
x
)


4π S(V )
∂n0
4π S(V )
∂n0
V

˚

3 0

Apliquemos este resultado a los problemas de contorno de Dirichlet y de Neumann

8.6.1.

Solución formal del problema Dirichlet

Hay que resolver


~ 2 φ(~x) = − ρ(~x)
~x ∈ V : ∇
0
~x ∈ S(V ) : φ(~x) = φD (~x)

Resolvamos entonces
 0
~ 02 GD (~x0 , ~x) = −4πδ(~x0 − ~x)
~x ∈ V : ∇
~x ∈ V
~x ∈ S(V ) : GD (~x0 , ~x) = 0
o sea, resolvamos el problema
~x ∈ V

(

~ 02 LD (~x0 , ~x) = 0
~x0 ∈ V : ∇
~x0 ∈ S(V ) : LD (~x0 , ~x) = − |~x01−~x|

y hacemos
GD (~x0 , ~x) =

| ~x0 − ~x |

+ LD (~x0 , ~x)

GD (~x0 , ~x) es la función de Green del problema Dirichlet. La solución formal es
˚
ˆˆ
1 
∂GD (~x0 , ~x)
3 0
φ(~x) =
d x ρ(~x )GD (~x, ~x ) −
x0 )φD (~x0 )
  dS(~
4π0
4π S(V )
∂n0
V

8.6.2.

Solución formal del problema de Neumann

Hay que resolver

(

~ 2 φ(~x) = − ρ(~x)
~x ∈ V : ∇
0
x)
=
−E
x)
~x ∈ S(V ) : ∂φ(~
N (~
∂n

Resultaría ventajoso resolver
(
~ 02 GN (~x0 , ~x) = −4πδ(~x0 − ~x)
~x0 ∈ V : ∇
~x ∈ V
~x0 ∈ S(V ) : ∂GN∂n(~x0 ,~x) = 0
pero ésto es, en general, imposible. En efecto, el teorema de Gauss nos da
˚
˚
3 0 ~ 02
~ 0 GN (~x0 , ~x)
~0·∇
d x ∇ GN (~x , ~x) =
d3 x0 ∇
V

V

---

### Página 73

=

ˆˆ




~0

S(V )

ˆˆ

~ x ) · ∇ GN (~x , ~x) =  
dS(~



dS(~x0 )

S(V )

= −4π

˚

V

d3 x0 δ(~x0 − ~x) = −4π

luego
ˆˆ




∂
GN (~x0 , ~x)
∂n

dS(~x0 )

∂
GN (~x0 , ~x) = −4π
∂n

ˆˆ

dS(~x0 ) = S

S(V )

ahora bien, puesto que



S(V )

con S el área total de S(V ), la condición de contorno más simple es
~x0 ∈ S(V ) :

∂GN (~x0 , ~x)
4π
=−
∂n
S

Luego, debemos resolver
(
~ 02 GN (~x0 , ~x) = −4πδ(~x0 − ~x)
~x0 ∈ V : ∇
~x ∈ V
~x0 ∈ S(V ) : ∂GN∂n(~x0 ,~x) = − 4π
S
o sea, resolvemos
~x ∈ V

(

~ 02 LN (~x0 , ~x) = 0
~x0 ∈ V : ∇
∂L
∂
− ∂n
~x0 ∈ S(V ) : N∂n(~x0 ,~x) = − 4π
0 |~
S
x0 −~
x|

puesto que
GN (~x0 , ~x) =

| ~x0 − ~x |

+ LN (~x0 , ~x)

la solución formal del problema de Neumann es
φ(~x) =
4π0

ˆˆ
1 
d x ρ(~x )GN (~x , ~x) −
x0 )EN (~x0 )GN (~x0 , ~x) + hφiS
  dS(~
4π S(V )
V

˚

3 0

donde hφiS es el valor medio del potencial sobre toda la superficie S(V )
ˆˆ
1 
x)φ(~x)
hφiS =
  dS(~
S S(V )
~ en V
La presencia de este término es un inconveniente. Pero no afecta E

---

### Página 74

Problema
El promedio temporal del potencial de un átomo de hidrógeno neutro es dado por
1 e−αr 
αr 
φ(r) =
q
1+
4π0 r
donde q es la magnitud de la carga del electrón y α = a0 /2, siendo a0 el radio de Bohr.
Encuentre la distribución de cargas (continua y discreta) correspondiente a este potencial e
interprete físicamente su resultado
#### Solución
~ 2φ = − ρ
∇
0
En coordenadas esféricas, el operador laplaciano es
~2= 1 ∂ r+ 1∇
~ 2 (ϑ, φ)
∇
r ∂r2
r2

Sea
ψ(r) =
f (r) =
o sea

r


αr 
qe−αr 1 +
4π0
φ(r) =

f (r)
r

y utilizamos la identidad


~ · ∇ψf
~
~ · ψ ∇f
~ + f ∇ψ
~
~ 2 ψf = ∇
=∇
∇
~ 2f + f ∇
~ 2 ψ + 2∇ψ
~ · ∇f
~
~ 2 ψf = ψ ∇
∇
r =| ~x |

(

~ 2ψ = ∇
~ 2 1 = −4πδ(~x)
∇
r
~ =∇
~ 1 = − ~x3 = − r̂2
∇ψ
r
|~
x|
r

~ 2 f (r) = 1 d rf (r) = 1 d (rf 0 + f )
∇
r dr2
r dr

=
y

con todo esto

(rf 00 + 2f 0 ) = f 00 + f 0
r
r

~ = − 2 ∂ f = − 2 f0
~ · ∇f
~ = − 2 r̂ · ∇f
2∇ψ
r
r2 ∂r
r2
~ 2 φ = 1 f 00 + 2 f 0 − 4πf (r)δ(~x) − 2 f 0
∇
r
r2
r2
1 d2 f (r)
= −4πf (0)δ(~x) +
r dr2

y
f (0) =

q
4π0

---

### Página 75



αr 
−αr α
=
−α 1+
f =
qe
qe−αr
4π0
4π0

f0 = −
f 00 = −



α2 r
α
−α−

1 αq −αr
e
(1 + αr)
4π0 2

1 αq −αr
e
(α − α(1 + αr))
4π0 2

f 00 = −


1 αq −αr
e
α − α − α2 r)
4π0 2
f 00 =

1 α3 q −αr
re
4π0 2

finalmente
~ 2 φ = − ρ = − q δ(~x) + 1 qα e−αr
∇
0
0
4π0 2

Luego
ρ(~x) = qδ(~x) −

qα3 −αr
e
8π

La interpretación física es la siguiente
qδ(~x)
representa al protón en el origen. Mientras que
qα3 −αr
e
8π
es la densidad (media-temporal) de la nube orbital electrónica
−



---

### Página 76

Problema: Teorema del valor medio
Demuestre que para un espacio sin cargas, el potencial electrostático en cualquier punto es igual
al potencial promedio sobre cualquier esfera centrada en ese punto
#### Solución
Utilizaremos el teorema de Green
˚

 ˆˆ



~ ψ − ψ∇
~ φ = 
~
~
d x φ∇
ds
n̂
·
∇ψφ
−
ψn̂
·
∇φ

V

δV

En electrostática, el potencial escalar satisface
~ 2 φ(~x) = − ρ(~x)
∇
0
y se define la función de Green-Dirichlet
~ 2 GD (~x, ~x0 ) = −4πδ(~x − ~x0 ), ~x, ~x0 ∈ V
∇
~ D (~x, ~x0 ) = 0, ~x0 ∈ δV
G

del teorema de Green
˚

3 0

V



0 ~ 02

~ 02 0

d x φ ∇ GD (~x, ~x ) − GD (~x, ~x )∇ φ

−

˚

V

3 0

d x 4πδ(~x − ~x )φ +

φ(~x) =
π0






~ 0 GD (~x, ~x0 ) − GD (~x, ~x0 )n̂0 · ∇
~ 0 φ0
=   ds0 φ0 n̂0 · ∇
ˆˆ

δV

ˆˆ
ρ(~x0 )

~ 0 GD (~x, ~x0 )
d x GD (~x, ~x )
=   ds0 φ0 n̂0 · ∇
ε
V
δV

˚

3 0

ˆˆ
1 
~ 0 GD (~x, ~x0 )
d x GD (~x, ~x )ρ(~x ) −
x0 )φ(~x0 )n̂(~x0 ) · ∇
  dS(~
4π
V
δV

˚

3 0

ahora, si V es una región libre de cargas
ˆˆ
1 
~ 0 GD (~x, ~x0 )
x0 )φ(~x0 )n̂(~x0 ) · ∇
φ(~x) = −
  dS(~
4π δV
Escogemos ahora V como una esfera de radio a centrada en ~x, de forma que la función de
Green queda
GD (~x, ~x0 ) =
de esta forma

−
| ~x − ~x | a

~ 0 GD (~x, ~x0 ) =
∇

~x − ~x0
| ~x − ~x0 |3

---

### Página 77

Luego, para ~x0 ∈ S(V )

Así

~ 0 GD (~x, ~x0 ) = ~x − ~x · ~x − ~x = −
n̂(~x0 ) · ∇
=− 2
| ~x − ~x | | ~x − ~x |
| ~x − ~x |
a

ˆˆ
1 
φ(~x) =
x0 )φ(~x0 ) = φ(~x, a)
  dS(~
4πa2 δV
con V : (~x, a)
Observación
La única condición sobre la esfera es que ella quede totalmente contenida en el vacío

---

### Página 78

Problema
Demuestre el siguiente corolario del teorema del valor medio. El campo electrostático en el vacío
satisface idénticamente las siguientes relaciones
~ x0 ) · E(~
~ x0 )
dS(~
=0
| ~x − ~x0 |
S(~
x)

ˆˆ




˚

V (S)

~ x0 ) ·
d3 x0 E(~

~x − ~x0
=0
| ~x − ~x0 |3

donde S es la superficie de una esfera de radio arbitrario con centro en ~x, y V (S) es su
volumen
#### Solución
En el espacio vacío de cargas
~ 2 φ(~x) = 0
∇
Utilizando el teorema de Green con
ψ(~x0 , ~x) =

˚

3 0

dx

V (~
x)

(

~ 02 φ(~x0 )
∇
~ 02
− φ(~x0 )∇
| ~x − ~x |
| ~x − ~x0 |
=

ˆˆ




dS(~x0 )

S(~
x)

(

| ~x0 − ~x |

)

= 4π

˚

V (~
x)

d3 x0 φ(~x0 )δ(~x − ~x0 ) = 4πφ(~x)

∂φ(~
x0 )
∂n0

∂
− φ(~x0 ) 0
| ~x − ~x |
∂n | ~x − ~x0 |

)

luego


ˆˆ
ˆˆ
~ x0 ) · ∇
~ 0 φ(~x0 )
1 
1   dS(~
~
~
dS(~x ) · ∇
φ(~
x
φ(~x) = −
)
+



4π S(~x)
| ~x − ~x0 |
4π S(~x)
| ~x − ~x0 |
ˆˆ
ˆˆ
~ x0 ) · E(~x0 )
1  ~ 0
~x0 − ~x
1   dS(~
φ(~x) =
x)· 0
φ(~x ) −
  dS(~

4π S(~x)
| ~x − ~x |3
4π S(~x) | ~x − ~x0 |
ˆˆ
ˆˆ
~ x0 ) · E(~x0 )
1 
1   dS(~
φ(~x) =
dS(~
x
)φ(~
x
)
−


4πa2 S(~x)
4π S(~x) | ~x − ~x0 |
donde a =| ~x − ~x0 | es el radio de la esfera. (Independiente de ~x0 ).
Por el teorema del valor medio
ˆˆ
1 
φ(~x) =
x0 )φ(~x0 )
  dS(~
4πa2 S(~x)
Luego
~ x0 ) · E(~
~ x0 )
dS(~
=0
| ~x − ~x0 |
S(~
x)

ˆˆ




---

### Página 79

Además

˚
~ x0 )
~ x0 )
E(~
E(~
3 0~ 0
~ x)·
dS(~
d
x
·
∇
=
| ~x − ~x0 |
| ~x − ~x0 |
S(~
x)
V (S)
(
)
˚
~ 0 · E(~
~ x0 )
∇
~0
~ x0 ) · ∇
d3 x0
=
+ E(~
0 |
|
~
x
−
~
x
| ~x − ~x0 |
V (S)


˚
~x − ~x0
ρ(~x0 )
3 0
~
+ E(~x ) ·
dx
=
0 | ~x − ~x0 |
| ~x − ~x0 |3
V (S)
˚
~ x0 ) · ~x − ~x = 0
d3 x0 E(~
=−
| ~x0 − ~x |3
V (S)

ˆˆ




---

### Página 80

Problema
Demuestre que el campo electrostático en el vacío satisface idénticamente la siguiente relación
~ ·
∇

˚

V (~
x)

d3 x0

~ x0 )
E(~
=0
| ~x − ~x0 |

donde V (~x) es el volumen de una esfera de radio arbitrario y centro en ~x
#### Solución
Sabemos que, en el vacío

~x0 − ~x
=0
| ~x0 − ~x0 |3
V (~
x)
˚
˚
~ x0 )
E(~
3 0~
3 0~
~
=
d x E(~x ) · ∇
d
x
∇
·
0=
| ~x − ~x0 |
| ~x − ~x0 |
V (~
x)
V (~
x)
˚
~ x0 )
E(~
~
0=∇·
d3 x0
| ~x − ~x0 |
V (~
x)
˚

~ x0 ) ·
d3 x0 E(~

---

### Página 81

#### Capítulo 9
Solución de la Ecuación de Poisson y
Laplace
9.1.

Método de las Imágenes

La solución formal de los problemas de contorno en electrostática se logra mediante el método de las Funciones de Green. En los problemas prácticos no siempre es fácil descubrir o
calcular la función de Green correcta. Para ello se usan algunas técnicas especiales, como el
método de las imágenes o la expansión en funciones ortogonales. El método de las imágenes
se usa en problemas de una o más cargas puntuales en presencia de superficies de frontera, se
trata de conductores conectados a tierra o mantenidos a un potencial fijo. Este método de las
imágenes nos ayuda a encontrar la función de Green adecuada en los problemas de contorno
Dirichlet con φD = cte

Se trata de resolver el siguiente problema Dirichlet

~ 2 φ(~x, ~x0 ) = − qδ(~x−~x0 )
~x ∈ V : ∇
0
~x ∈ V :
~x ∈ S(V ) : φ(~x, ~x0 ) = φD

Bajo condiciones geométricas favorables (simetría) es posible infrerir que un número pequeño
de cargas puntuales, de magnitud apropiada, y ubicadas adecuadamente en la región externa
Ve , pueden simular las condiciones de contorno requeridas, estas son las cargas imágenes
Sean
V : región interior
Ve : región externa (conductor)
qi0 = qi0 (q, ~x0 ) = carga imagen
~x0i = ~x0i (q, ~x0 )= posición de la imagen

---

### Página 82

Además debe tenerse que
~x0i (q, ~x0 ) ∈ Ve

Las cargas imágenes deben ser externas a la región de interés V , de manera que su potencial
sea una solución de la ecuación de Laplace en V . En efecto

~ 2 φ(~x, ~x0 ) = − qδ(~x − ~x )
∇
0
X
1 X 0~ 2
qi0
~2 1
qi ∇
∇
=
4π0 i | ~x − ~xi |
4π0 i
| ~x − ~x0i |
=−
Luego

1 X
qi δ(~x − ~x0i ) = 0
0 i

δ(~x − ~x0i ) = 0, ∀~x ∈ V

Carga puntual q ubicada frente a un conductor plano a potencial cero, y de
extensión infinita

9.2.

Funciones Ortogonales y Expansiones

Una técnica muy poderosa de la física matemática es la representación de soluciones físicas
mediante expansiones en términos de funciones ortogonales. En cada problema se elige un
particular conjunto de funciones ort
ogonales adaptadas a la simetría del sistema. Revisemos las propiedades más generales de
las funciones ortogonales y veamos su uso en la representación de funciones mediante series
Sea ξ una variable real independiente, de rango
a≤ξ≤b
y {un (ξ)} un conjunto infinito numerable de funciones complejas definidas en (a, b), con
n = 1, 2, ... tales que
1. Todas ellas son de cuadrado integrable en (a, b)
ˆ b
a

dξ | un (ξ) |2 ≤ ∞

donde
| un (ξ) |2 = u∗n (ξ)un (ξ)

2. Además satisfacen la condición de ortogonalidad en (a, b)
m 6= n →

ˆ b
a

dξu∗m (ξ)un (ξ) = 0

---

### Página 83

Normalización
Sea
Nn =

ˆ b
a

dξ | un (ξ) |2

0 < Nn < ∞
Definamos

ûn (ξ) = √ un (ξ)
Nn

Entonces el conjunto
{ûn (ξ), n = 1, 2, ..}
es un conjunto de funciones ortonormales en (a, b). La condición de ortonormalidad es
ˆ b
a

dξ û∗n (ξ)ûn (ξ) = δmn

Expansión
Sea f (ξ) una función arbitraria, en general compleja, de cuadrado integrable en (a, b)
ˆ b
a

dξ | f (ξ) |2 < ∞

Supongamos que, dado el número natural N , la serie finita
fN (ξ) =

N
X

an ûn (ξ)

n=1

sea una representación aproximada de la función f (ξ) en (a, b). Si modificamos los coeficientes an , n = 1, 2, ...N , modificamos la bondad de la aproximación. Surge entonces el problema
de ajustar los coeficientes de tal manera que la aproximación sea óptima. Luego requerimos que
el error cuadrático medio MN sea mínimo
MN =

ˆ b
a

dξ | f (ξ) − fN (ξ) |2

Se tiene
MN =

ˆ b
a

MN =

ˆ b
a

MN =

ˆ b
a

dξ | f (ξ) | −

N
X

m=1

"

dξ | f (ξ) −

dξ f ∗ (ξ) −

am

ˆ b
a

N
X

N
X
n=1

an ûn (ξ) |2

#"

a∗n û∗n (ξ)

n=1

f (ξ) −

N
X

m=1

#

am û∗m (ξ)

ˆ b
ˆ b
N
N X
N
X
X
∗
∗
∗
dξf (ξ)ûm (ξ)−
an
dξf (ξ)ûn (ξ)+
an am
dξ û∗n (ξ)ûm (ξ)
∗

n=1

Utilizando la ortonormalidad

a

n=1 m=1

a

---

### Página 84

MN =

ˆ b
a

dξ | f (ξ) | −

N
X

am

ˆ b
a

m=1

∗

dξf (ξ)ûm (ξ) −

N
X

a∗n

n=1

ˆ b

dξf (ξ)ûn (ξ) +

a

N
X

a∗n an

n=1

Entonces, la condición para el mínimo es
ˆ b
∂MN
=−
dξ û∗k (ξ)f (ξ) + ak = 0
∂a∗k
a
ˆ b
∂MN
=−
dξ ûk (ξ)f ∗ (ξ) + a∗k = 0
∂ak
a
Luego, los mejores coeficientes de la representación aproximada son
ˆ b
an =
dξ û∗n (ξ)f (ξ)
a

se llaman los coeficientes de Fourier de la expansión
Completitud
El conjunto de funciones ortonormales {ûn (ξ)} es completo en (a, b) si, para cualquier función
f (ξ) de cuadrado integrable en (a, b), existe un número natural N0 [f ] tal que, dado  > 0
arbitrario, se tiene
N > N0 [f ] → MN [f ] < 
o sea que
lím MN [f ] = 0, ∀f

N →∞

siendo MN el error cuadrático medio mínimo
Convergencia en la media
Si el conjunto de funciones ortonormales {ûn (ξ)} es completo en (a, b) entonces se puede demostrar que la representación en serie
∞
X

an ûn (ξ) = S [f ]

n=1

con

an =

ˆ b
a

S [f ] =

∞
X
n=1

dξ û∗n (ξ)f (ξ)

un (ξ)

ˆ b
a

dξ 0 û∗n (ξ 0 )f (ξ 0 )

converge en la media a f (ξ) en (a, b). Vale decir que siendo f (ξ) una función acotada y
continua a trazos en (a, b) (por lo tanto de cuadrado integrabe) se tiene
1. En todo punto de continuidad
S [f ] = f (ξ)

---

### Página 85

2. En un punto de discontinuidad ordinaria
f (ξ + 0) + f (ξ − 0)

S [f ] =

Para todos los conjuntos de fnciones ortonormales que suelen usarse en física se ha demostrado su completitud
Relación de completitud
f (ξ) =

∞
X

an ûn (ξ)

n=1

f (ξ) =

∞
X

ûn (ξ)

a

n=1

f (ξ) =

ˆ b

ˆ b

∞
X

dξ f (ξ )

a

f (ξ) =

a

û∗n (ξ 0 )ûn (ξ)

n=1

por otro lado
ˆ b

dξ 0 û∗n (ξ 0 )f (ξ 0 )

dξ 0 f (ξ 0 )δ(ξ 0 − ξ), ∀f

Luego, la suma total de los términos bilineales û∗n (ξ)ûn (ξ) debe darnos una representación
de la delta de Dirac
∞
X
n=1

û∗n (ξ 0 )ûn (ξ) = δ(ξ 0 − ξ)

También vemos que, necesariamente
N
X

û∗n (ξ 0 )ûn (ξ) =

n=1

N
X

û∗n (ξ)ûn (ξ 0 )

n=1

es real, y que
N
X
n=1

û∗n (a)ûn (b) = 0, a 6= b

Luego, un conjunto de funciones ortonormales completo queda caracterizado por
ˆ b
dξ û∗m (ξ)ûn (ξ) = δmn
a

---

### Página 86

∞
X

û∗n (ξ)ûn (ξ 0 ) = δ(ξ − ξ 0 )

n=1

Identidad de Parseval
Sea
f (ξ) =

∞
X

an ûn (ξ)

n=1

Consideremos

ˆ b
a

dξ | f (ξ) | =
=

ˆ b

∞
∞ X
X

dξ

a∗m û∗m (ξ)

a

m=1

a∗m an

ˆ b

m=1 n=1

∞ X
∞
X

=

∞
X

a

ˆ b
a

an ûn (ξ)

n=1

dξ û∗m (ξ)ûn (ξ)

a∗m an δmn =

m=1 n=1

Luego

∞
X

∞
X

a∗m an

n=1

dξ | f (ξ) | =

Teorema de Multiplicación
Sean
f (ξ) =

∞
X

∞
X
n=1

| an |2

an ûn (ξ)

n=1

g(ξ) =

∞
X

bn ûn (ξ)

n=1

ˆ b

∗

dξf (ξ)g(ξ) =

a

ˆ b

dξ

a

=

∞
∞ X
X

m=1 n=1

=

a∗m û∗m (ξ)

m=1

a∗m bn

∞
∞ X
X

∞
X

ˆ b
a

(f, g) =

ˆ b

bn ûn (ξ)

n=1

dξ û∗m (ξ)ûn (ξ)

a∗m bn δmn =

m=1 n=1

Con esto

∞
X

∞
X

a∗n bn

n=1

∗

dξf (ξ)g(ξ) =

a

∞
X
n=1

Caso bidimensional
Sea
f = f (ξ, η)
a ≤ ξ ≤ b, c ≤ η ≤ d

a∗n bn

---

### Página 87

Elegimos dos conjuntos completos ortonormales
 ´b
dξ û∗ (ξ)ûn (ξ) = δmn
{ûn (ξ)} → P∞a ∗ m
n=1 ûn (ξ)ûn (ξ ) = δ(ξ − ξ )
 ´d
dηv̂ ∗ (η)v̂n (η) = δmn
{v̂n (η)} → P∞c ∗ m
n=1 v̂n (η)v̂n (η ) = δ(η − η )

entonces el conjunto (producto tensorial)

{ûm (ξ)v̂n (η)} = {ŵm,n (ξ, η)}
satisface
ˆ bˆ d
a

c

∞ X
∞
X

m=1 n=1

dξdηû∗k (ξ)v̂l∗ (η)ûm (ξ)v̂n (η) = δkm δln

û∗m (ξ)v̂n∗ (η)ûm (ξ 0 )v̂n (η 0 ) = δ(ξ − ξ 0 )δ(η − η 0 )

Luego cualquier función f (ξ, η) de cuadrado integrable en (a, b) × (c, d) se puede representar
como
f (ξ, η) =

∞
∞ X
X

amn ûm (ξ)v̂n (η)

m=1 n=1

amn =

ˆ bˆ d
a

c

dξdηû∗m (ξ)v̂n∗ (η)f (ξ, η)

9.3.

Series de Fourier

9.3.1.

Condiciones de Dirichlet

Sea la función f (x) que satisface las siguientes condiciones (de Dirichlet)
(1) f (x) está definida en a < x < a + T
(2) f (x) y f 0 (x) son continuas a trazos (seccionalmente continuas) en a < x < a + T
(3) f (x) es periódica con período T en −∞ < x < ∞
f (x) = f (x + T )
Observación: la función f (x) se puede definir a partir de una función acotada F (x) definida
en −∞ < x < ∞ siendo F (x) y F 0 (x) continuas a trazos en a < x < a + T . En efecto
f (x) =



F (x)
si a < x < a + T
f (x + T ) si − ∞ < x < ∞

Teorema de la serie de Fourier
Si f (x) satisface las condiciones de Dirichlet en a < x < T entonces

---

### Página 88

(1) En todo punto de continuidad




∞ 
A0 X
2πnx
2πnx
f (x) =
+ Bn sin
An cos
+
T
T
n=1
(2) En un punto de discontinuidad ordinaria

donde





∞ 
f (x + 0) + f (x − 0)
2πnx
2πnx
A0 X
+ Bn sin
=
+
An cos
T
T
n=1
An =
T

ˆ a+T

Bn =
T

ˆ a+T

dx cos

a

dx sin

a





n2πx
T
n2πx
T





f (x)
f (x)

para n = 0, 1, 2, 3, .... Las condiciones de Dirichlet son suficientes (pero no necesarias) para
la convergencia en la media de la serie de Fourier. Sin perder generalidad, si f (x) satisface las
condiciones de Dirichlet en −T /2 < x < T /2 se tiene




∞ 
A0 X
2πnx
2πnx
f (x) =
An cos
+ Bn sin
+
T
T
n=1


ˆ
2 T /2
2πnx
dx cos
f (x)
An =
T −T /2
T


ˆ
2πnx
2 T /2
dx sin
Bn =
f (x)
T −T /2
T

Relaciones de ortogonalidad



2πnx
T
dx cos
cos
= δmn
T
−T /2




ˆ T /2
T
2πnx
2πmx
sin
= δmn
dx sin
T
T
−T /2




ˆ T /2
2πmx
2πnx
dx sin
cos
=0
T
T
−T /2


 ˆ T /2

ˆ T /2
2πmx
2πnx
dx cos
dx sin
=
=0
T
T
−T /2
−T /2
ˆ T /2

2πmx
T





---

### Página 89

9.4.

Ecuación de Laplace en Coordenadas Rectangulares


∂2
∂2
∂2
+
+
∇ φ(~x) =
∂x2 ∂y 2 ∂z 2
utilizamos el método de separación de variables
~2



φ(x, y, z) = 0

φ(x, y, z) = X(x)Y (y)Z(z)
Se tiene entonces

1~2
1 d2 X
1 d2 Y
1 d2 Z
∇ φ=
+
+
=0
φ
X dx2
Y dy 2
Z dz 2

luego
1 d2 X
1 d2 Y
1 d2 Z
=−
−
= −α2
X dx
Y dy
Z dz
1 d2 Y
1 d2 Z
=
α
−
= −β 2
Y dy 2
Z dz 2
1 d2 Z
= α2 + β 2 = −γ 2
Z dz 2
Resulta
d2 X
+ α2 X = 0
dx
d2 Y
+ β 2Y = 0
dy 2
d2 Z
+ γ2Z = 0
dz

con

α2 + β 2 + γ 2 = 0
Consideremos
X(x) = e±iαx
Y (y) = e±iβy
Z(z) = e±iγz
pero


γ 2 = − α 2 + β 2 = i2 α 2 + β 2 )
p
γ = ±i α2 + β 2

φαβ (x, y, z) = e±iαx±iβy±

√

α2 +β 2 z

es un conjunto de soluciones linealmente independientes de la ecuación de Laplace. La
ecuación de Laplace es lineal y homogénea, luego, por superposición
√
√
XX
XX
− i(αx+βy)− α2 +β 2 z
+ i(αx+βy)+ α2 +β 2 z
φ(x, y, z) =
Aαβ e
+
Aαβ e
α

α

β

β

−
es también una solución de la ecuación de Laplace. Las constantes α, β, A+
αβ , Aαβ están a
nuestra disposición. Ellas se determinan mediante las condiciones de contorno

---

### Página 90

9.4.1.

Problema en 2 dimensiones

En ciertos problemas, la simetría permite establecer que el potencial es sólo función de dos
variables, digamos x e y. En este caso se debe resolver
 2

∂
∂
~ φ(~x) =
+
φ(x, y) = 0
∇
∂x2 ∂y 2
La lógica es la misma, utilizando el método de separación de variables
φ(x, y, z) = X(x)Y (y)
Se tiene entonces

1~2
1 d2 X
1 d2 Y
∇ φ=
+
=0
φ
X dx2
Y dy 2

luego
1 d2 X
1 d2 Y
=
−
= −α2
X dx2
Y dy 2
1 d2 Y
= α2
Y dy 2
Resulta
d2 X
+ α2 X = 0
dx
d2 Y
− α2 Y = 0
dy 2
Las soluciones son de la forma
X(x) = e±iαx
Y (y) = e±αy

La solución general de la ecuación de Laplace está dada por la familia de funciones
X(x) = Aα cos (αx) + Bα sin (αx)
Y (y) = Cα eαy + Dα e−αy
con Aα , Bα , Cα , Dα constantes reales.

---

### Página 91

Problema
Potencial en una Caja

Resolver

~ 2 φ(~x) = 0
~x ∈ V : ∇









φ(0, y, z) = 0
φ(a, y, z) = 0
φ(x, 0, z) = 0
~x ∈ S(V ) :
φ(x, b, z) = 0




φ(x, y, 0) = 0



φ(x, y, c) = φD (x, y)
#### Solución
φ(x, y, z) =

XX
α

β


√
√
− − α2 +β 2 z
α2 +β 2 z
A+
ei(αx+βy)
e
+
A
e
αβ
αβ

Esto se puede reescribir como
φ(x, y, z) =

XX
α≥0

β

 √α2 +β 2 z iβy
 −√α2 +β 2 z iβy
+
− iα
−
iαx
−iαx
−iα
A+
e
e
e
+
A
e
e
+
A
e
+
A
e
e
αβ
−αβ
αβ
−αβ

Se tiene
±
φ(0, y, z) = 0 → A±
αβ + A−αβ = 0

Luego
φ(x, y, z) =

XX
α≥0

β

iαx
− e−iαx
A+
αβ e

 √α2 +β 2 z iβy
 −√α2 +β 2 z iβy
iαx
−iαx
e + A−
−
e
e
e
e
e
αβ

---

### Página 92

Además
φ(a, y, z) = 0 → eiαa − e−iαa = 2i sin αa = 0
Esto limita los valores posibles que puede tomar α
aα = mπ → m = 0, ±1, ±2, ...
α=

mπ
→ m = 0, ±1, ±2, ...
a

2i sin

 mπ 


√
√
−
α2 +β 2 z
− α2 +β 2 z
e
+
A
e
x eiβy A+
mβ
mβ
a

Así
∞ X
X

φ(x, y, z) =

m=1

β

y se puede escribir como

φ(x, y, z) =

∞ X
X

2i sin

m=1 β≥0

 mπ  
 −√α2 +β 2 z 
 √α2 +β 2 z
+
−
−
iβy
−iβy
iβy
−iβy
x
A+
e
e
e
+
A
e
+
A
e
+
A
e
mβ
m−β
mβ
m−β
a

Se cumple además
±
φ(x, 0, z) = 0 → A±
αβ + Aα−β = 0

 mπ  

√
√
+
−
α2 +β 2 z
− α2 +β 2 z
2i sin
+ Amβ 2i sin(βy)e
φ(x, y, z) =
x Amβ 2i sin(βy)e
a
m=1 β≥0
∞ X
X

y
φ(x, b, z) = 0 → 2i sin βb = 0
Esto limita los valores posibles que puede tomar β
bβ = nπ → n = 0, ±1, ±2, ...
β=

nπ
→ n = 0, ±1, ±2, ...
b

En resumen, α y β satisfacen
nπ
mπ
,β =
a
b
r 
p
m 2  n 2
α2 + β 2 = π
+
= γmn
a
a
α=

m, n = 0, ±1, ±2, ...
y la solución general queda
φ(x, y, z) =

 nπy 
 πmx 

γmn z
−
−γmn z
(2i)2 A+
e
+
A
e
sin
sin
mn
mn
a
b
m=1 n=1
∞ X
∞
X

El potencial también debe ser nulo en z = 0

---

### Página 93

(2i)

−
A+
mn + Amn



sin

 πmx 

sin

a

 πny 
b

=0

−
A+
mn + Amn = 0

Sea

2 −
Amn = (2i)2 A+
mn = −(2i) Amn

luego
 1

γmn z
−
−γmn z
γmn z
−γmn z
(2i)2 A+
A
=
e
e
+
A
e
−
e
mn
mn
mn
= Amn sinh γmn z
Con todo esto, la solución toma la forma
φ(x, y, z) =

∞ X
∞
X

Amn sin

m=1 n=1

Por último, la condición en z = c entrega
φ(x, y, c) = φD (x, y) =

∞ X
∞
X

 πmx 
a

sin

 nπy 
b

(Amn sinh γmn ) sin

m=1 n=1

Esta es una doble serie de Fourier

sinh γmn z

 πmx 
a

sin

 nπy 
b


πnξ
f (ξ) =
Bn sin
L
n=1


ˆ
πnξ
2 L
dξ sin
Bn =
f (ξ)
L 0
L


∞
X

Luego la solución del problema es
φ(x, y, z) =

∞
∞ X
X

Amn sin

m=1 n=1

con

Amn =
ab sinh γmn c

ˆ a

dx

ˆ b

γmn = π

 πmx 
a

dy sin

r 
m 2
a

sin

 nπy 

 πmx 
a

+

 n 2
b

b

sin

sinh γmn z

 πny 
b

φD (x, y)

c

---

### Página 94

Problema
Determinar el potencial en la región que comprende el interior de una caja rectangular de
longitud infinita, cuya sección transversal se aprecia en la figura

#### Solución
Dado que la longitud de la caja es muy larga, el potencial tendrá la misma forma para cualquier
sección transversal. Se debe resolver entonces la ecuación de Laplace
~ 2 φ(x, y) = 0
∇
con las condiciones de borde

φ(0, y) = 0



φ(b, y) = 0
~x ∈ S(V ) :
φ(x,
0) = 0



φ(x, a) = V0
La solución general de la ecuación de Laplace es
φ(x, y) = X(x)Y (y)
donde X(x) e Y (y) pertenecen a las familias de funciones
X(x) = Aα cos (αx) + Bα sin (αx)
Y (y) = Cα eαy + Dα e−αy
Para cualquier α real, φ(x, y) es solución de la ecuación de Laplace. Sin embargo, las condiciones de borde limitarán los valores posibles de α. En efecto, debe cumplirse que

de forma que

φ(0, y) = 0 → X(0) = 0
Aα = 0

es decir
X(x) = Bα sin (αx)
Además, debe tenerse
es decir

φ(b, y) = 0 → Bα sin (αb) = 0
αb = nπ, n = 0, 1, 2, ...

---

### Página 95

luego

nπ
, n = 0, 1, 2, ...
b
Es decir, la familia de funciones que satisfacen la ecuación de Laplace y cumplen con
φ(0, y) = φ(b, y) = 0 está dada por
α=

φ(x, y) = X(x)Y (y)
 nπ 
x , n = 0, 1, 2, ...
X(x) = sin
b
nπ

nπ

Y (y) = An e b y + Bn e− b y , n = 0, 1, 2, ...
La solución general toma la forma
φ(x, y) =

∞
X

sin

n=1

 nπ 
nπ
nπ 
x An e b y + Bn e− b y
b

además se tiene φ(x, 0) = 0
φ(x, 0) =

∞
X

sin

n=1

Luego

 nπ 
x (An + Bn ) = 0
b

An = −Bn
y entonces
φ(x, y) =

∞
X

sin

n=1

φ(x, y) =

∞
X

sin

n=1

φ(x, y) =

 nπ 
nπ
nπ 
x An e b y − e− b y
b

∞
X

 nπ 
 nπ 
x 2An sinh
y
b
b

Cn sin

n=1

 nπ 
 nπ 
x sinh
y
b
b

Donde Cn = 2An . Por último, la condición de borde φ(x, a) = V0 entrega
φ(x, a) =

∞
X

Cn sin

n=0

V0 =

∞
X
n=0

 nπ 
 nπ 
x sinh
a = V0
b
b

Cn sin

 nπ 
 nπ 
x sinh
a
b
b

¿Cómo podemos encontrar los Cn ?. La clave está en notar que esta es una expansión en
series de Fourier. Si F : [−b, b] → R es una función de cuadrado integrable en [-b,b], admite
una expansión en series
 nπ  X
 nπ 
a0 X
F (x) =
An cos
Bn sin
+
x +
x
b
b
n=1
n=1
con

Bn =
b

ˆ b

−b

dxF (x) sin

 nπ 
x , n = 0, 1, 2...
b

---

### Página 96

 nπ 
x , n = 0, 1, 2...
dxF (x) cos
b
−b

ˆ b

An =
b

En particular, si F es una función impar sobre [−b, b], An = 0 ∀n, y entonces
 nπ 
X
x
F (x) =
Bn sin
b
n=1
con

Bn =
b

ˆ b

dxF (x) sin

 nπ 
x , n = 0, 1, 2...
b

Interpretemos ahora el resultado que hemos obtenido
∞
 nπ  X
 nπ 
 nπ 
V0 =
x sinh
a =
x
Cn sin
Bn sin
b
b
b
n=0
n=0
∞
X

Es justamente la expansión en serie de Fourier de V0 . Entonces
ˆ
 nπ  2V ˆ b
 nπ 
2 b
Bn =
dxV0 sin
dx sin
x =
x
b 0
b
b 0
b
 nπ  b
2V0 b
V0
=2
cos
x
(1 − cos (nπ))
Bn = −
b nπ
b
nπ
V0
para n impar. Además,
Notar que Bn = 0 para n impar, mientras que Bn = 4 nπ
Bn = Cn sinh
Luego

 nπ 
Bn

a → Cn =
b
sinh nπ
a
b
Cn = 0, n par

Cn =

4V0
 , n impar
nπ sinh nπ
a
b

y la solución para el potencial queda
∞

4V0 X
 sin

φ(x, y) =
π n=1 (2n − 1) sinh (2n−1)πa
b



(2n − 1)πx
b



sinh



(2n − 1)πy
b



---

### Página 97

La siguiente figura es un gráfico de las curvas de nivel para a = b = 5 y V0 = 1 [V]

---

### Página 98

Problema
Encuentre el potencial para la región 0 ≤ x ≤ a, y ≥ 0, con las condiciones de borde de Dirichlet

φ(0, y) = 0



φ(a, y) = 0
~x ∈ S(V ) :
límy→∞ φ(x, y) = 0



φ(x, 0) = V (x)

#### Solución
El potencial en V satisface la ecuación de Laplace
~ 2 φ(x, y) = 0
∇
cuya solución está dada por
φ(x, y) = X(x)Y (y)
donde
X(x) = Aα cos (αx) + Bα sin (αx)
Y (y) = Bα eαy + Cα e−αy
La condición de borde φ(0, y) = 0 implica

Además, debe tenerse

X(0) = Aα = 0 → X(x) = Bα sin (αx)
φ(a, y) = 0 → X(a) = 0
sin (αa) = 0

Entonces
α=

nπ
, n = 0, 1, 2, ...
a

Entonces la solución toma la forma
 nπ 
nπ
nπ 
sin
x An e a y + Bn e− a y
φ(x, y) =
a
n=1
∞
X

---

### Página 99

La condición en el infinito es
lím φ(x, y) = 0

y→∞

de forma que An = 0, ∀n = 0, 1, 2, ...
φ(x, y) =

∞
X

Bn sin

n=1

Por último, la condición φ(x, 0) = V (x) es
φ(x, 0) =

∞
X

Bn sin

n=1

 nπ  nπ
x e− a y
a

 nπ 
x = V (x)
a

Ahora, consideremos F (x), −a ≤ x ≤ x. Si F (x) es cuadrado integrable en [−a, a], entonces
existe su serie de Fourier

donde

∞
∞
 nπ  X
 πn 
a0 X
+
x +
x
F (x) =
An cos
Cn sin
a
a
n=1
n=1

 nπ 
x , n = 0, 1, 2, ...
a
−a
ˆ
 nπ 
1 a
Cn =
dxF (x) sin
x , n = 0, 1, 2, ...
a −a
a

An =
a

ˆ a

dxF (x) cos

Si F (x) es impar, entonces An = 0 ∀n, de forma que
F (x) =

∞
X

Cn sin

n=1

con

Cn =
a

Con esto,

 πn 
x
a

 nπ 
x , n = 1, 2, ...
dxF (x) sin
a

ˆ a

φ(x, 0) =

∞
X

Bn sin

n=1

 nπ 
x = V (x)
a

corresponde a la expansión en serie de Fourier de V (x), −a < x < a, con V (−x) = −V (x)
(por supuesto que físicamente sólo interesa V (x) para 0 ≤ x ≤ a). Así, la solución del problema
es

con

 nπ  nπ
φ(x, y) =
Bn sin
x e− a y
a
n=1
∞
X

Bn =
a

ˆ a

dxV (x) sin

 nπ 
x , n = 1, 2, ...
a

Supongamos que φ(x, 0) = V (x) = V0 (constante). Luego
ˆ
 nπ 
 nπ  a
2V0 a
2V0 a
dx sin
, n = 1, 2, 3...
x =−
cos
x
Bn =
a 0
a
a nπ
a

---

### Página 100

Bn =

Finalmente

2V0
(1 − cos (nπ)) , n = 1, 2, 3...
nπ

0 si n par
Bn = 4V0
si n impar
nπ

∞
X

4V0
sin
φ(x, y) =
(2n − 1)π
n=1




(2n−1)π
(2n − 1)π
x e− a y
a

El gráfico muestra la solución para V0 = 0,1, a = 5, y tomando 50 términos en la serie

---

### Página 101

9.5.

Ecuación de Laplace en coordenadas Cilíndricas

9.5.1.

Problema bidimensional

Supongamos un problema de Laplace plano, en donde la geometría del problema permite
que sea más favorable utilizar coordenadas polares


∂φ
1 ∂2φ
1 ∂
~
∇ φ=
r
+ 2 2 =0
r ∂r
∂r
r ∂ϕ
Utilizando el método de separación de variables, es decir
φ(r, ϕ) = R(r)Ψ(ϕ)
De forma que



1 ∂
∇ φ=Ψ
r ∂r
~2

∂R(r)
r
∂r



1 ∂ 2 Ψ(ϕ)
+ R(r) 2
=0
r ∂ϕ2

Multiplicando por rφ (si φ nunca es cero)


r ∂
∂R(r)
1 ∂ 2 Ψ(ϕ)
=0
r
+
R(r) ∂r
∂r
Ψ ∂ϕ2
o, equivalentemente

r ∂
R(r) ∂r



∂R(r)
r
∂r



=−

1 ∂ 2 Ψ(φ)
Ψ(ϕ) ∂ϕ2

La única forma de que esto último sea posible es que ambas expresiones sean una constante


dR(r)
1 ∂ 2 Ψ(φ)
r d
= α2
r
=−
R(r) dr
dr
Ψ(ϕ) ∂ϕ2
de forma que

r d
R(r) dr



dR(r)
r
dr



= α2

1 d2 Ψ(ϕ)
= −α2
Ψ(ϕ) dϕ2
1. Primer caso, α 6= 0
La solución para Ψ es inmediata
Ψ(ϕ) = e±iαϕ
y para R(r), con α 6= 0
r d
R(r) dr



dR(r)
r
dr
r



r
=
R(r)



dR(r)
d2 R(r)
+r
dr
dr2

d2 R(r)
dR(r)
= R(r)α2
+ r2
dr
dr2



= α2

---

### Página 102

Esta ecuación pertenece al tipo Cauchy, la solución es de la forma
R(r) = ra
En efecto, es solución si
rara−1 + r2 a(a − 1)ra−2 = ra α2
ara + a(a − 1)ra = ra α2

a + a(a − 1) = α2 → a2 = α2
Entonces
a = ±α
y la solución para R(r), con α 6= 0 es
R(r) = Aα rα + Bα r−α

2. Segundo caso, α = 0
Aquí,
r d
R(r) dr
luego

y



dR(r)
r
dr





dR(r)
r
dr



=0

= 0 → R(r) = a0 + b0 ln r

1 d2 Ψ(ϕ)
=0
Ψ(ϕ) dϕ2

Ψ(ϕ) = A0 + B0 ϕ

Finalmente, la solución general a la ecuación de Laplace en coordenadas polares es la familia
de soluciones

φ(r, ϕ) = (a0 + b0 ln r) (A0 + B0 ϕ) + Aα rα + Bα r−α (Cα sin (αϕ) + Dα cos (αϕ))

---

### Página 103

Problema
Determine el potencial electrostático al interior de la región limitada por un conductor de
extensión infinita cuya forma se muestra en la figura. El conductor se encuentra a potencial V

#### Solución
Dada la geometría, es natural utilizar coordenadas polares para resolver este problema. Si en
la región Ω : 0 ≤ ϕ ≤ β no hay carga, entonces el potencial satisface
~ 2 φ = 0, enΩ
∇
La solución general de la ecuación de Laplace en coordenadas polares está dada por

φ(r, ϕ) = (a0 + b0 ln r) (A0 + B0 ϕ) + Aα rα + Bα r−α (sin (Cα αϕ) + Dα cos (αϕ))

El potencial debe ser finito en el origen r = 0, de forma que Bα = 0, ∀α, igualmente b0 = 0.
La solución que nos interesa toma la forma
φ(r, ϕ) = (A0 + B0 ϕ) + Aα rα (Cα sin (αϕ) + Dα cos (αϕ))

La condición de borde φ(r, 0) = V implica
φ(r, 0) = A0 + Aα rα Dα = V
Lo cual se cumple para todo r si A0 = V , Dα = 0. Así
φ(r, ϕ) = (V + B0 ϕ) + Aα rα sin (αϕ)
Además, la condición de borde en = β entrega
φ(r, β) = (V + B0 β) + Aα rα sin (αβ) = V

---

### Página 104

B0 β + Aα rα sin (αβ) = 0
lo cual se cumple para todo r si
B0 = 0
nπ
, n = 0, 1, 2, ...
sin (αβ) = 0 → α =
β
Finalmente, la solución queda
φ(r, ϕ) = V +

∞
X

n

An r sin

n=0



nπ
ϕ
β



---

### Página 105

9.6.

Ecuación de Laplace en Coordenadas Esféricas
~ 2 φ(r, ϑ, ϕ) = 0
∇
1 ∂
r2 ∂r



r

2 ∂φ

∂r



∂
+ 2
r sin ϑ ∂ϑ

Notar que
1 ∂
r2 ∂r
y



r

2 ∂φ

1 ∂
1 ∂2
(rφ)
=
r ∂r2
r ∂r
luego

∂r






∂φ
sin ϑ
∂ϑ



=

∂ 2 φ 2 ∂φ
+
∂r2
r ∂r

+

∂2φ
r2 sin2 ϑ ∂ϕ2


∂φ
∂ 2 φ 2 ∂φ
r
+φ = 2 +
∂r
∂r
r ∂r

1 ∂ 2∂
1 ∂2
r
r
=
r2 ∂r ∂r
r ∂r2

Así, la ecuación de Laplace queda de la forma


1 ∂2
∂φ
1 ∂2φ
∂
(rφ)
+
=0
sin
ϑ
+
r ∂r2
r2 sin ϑ ∂ϑ
∂ϑ
r2 sin ϑ ∂ϕ2
supongamos
R(r)
Θ(ϑ)Φ(ϕ)
φ(r, ϑ, ϕ) =
r
resulta


ΘΦ d2 R
dΘ
RΘ d2 Φ
RΦ d
sin ϑ
+ 3 2
+ 3
=0
r dr2
r sin ϑ dϑ
dϑ
r sin ϑ dϕ2

r2 sin2 ϑ d2 R sin ϑ d
+
R
dr2
Θ dϑ



dΘ
sin ϑ
dϑ



=−

1 d2 Φ
= m2
Φ dϕ2

La ecuación para Φ es inmediata
d2 Φ
+ m2 Φ = 0
dϕ2
cuya solución es
Φ(ϕ) = e±imϕ

Es evidente que esta función debe ser periódica
Φ(ϕ ± 2π) = Φ(ϕ)
es decir
e±im(ϕ+2π) = e±i2πm e±imϕ = e±imϕ

---

### Página 106

e±i2πm = cos(2πm) ± i sin(2πm) = 1
luego m = 0, ±1, ±2, ...
Φm (ϕ) = eimϕ
m = 0, ±1, ±2, ...
Con esto
r2 d2 R
d
=
−
R dr2
Θ sin ϑ dϑ
Luego



dΘ
sin ϑ
dϑ



+

m2
= l(l + 1)
Φ sin2 ϑ

d2 R l(l + 1)
−
R=0
dr2
r2

Esta ecuación pertenece al tipo Cauchy
x2 y 00 (x) + αxy 0 (x) + βy(x) = 0
cuya solución es de la forma
y(x) = xa → y 0 (x) = axa−1 → y 00 (x) = a(a − 1)xa−2
luego
a(a − 1)xa + αaxa + βxa = 0
a2 + (α − 1)a + β = 0

√
(1−α)+ (1−α −4β

a1 =
√2 2
a=
(1−α)− (1−α −4β

a2 =

Por superposición , tenemos que la solución general es
y(x) = Axa1 + Bxa2
En nuestro caso
R(r) = ra
a2 − a − l(l + 1) = 0
p

√

1 + 4l + 4l2
p

1 ± (2l + 1)2
1 ± (2l + 1)
l+1
=
=
a=
−l
a=

1±

1 + 4l(l + 1)
1±
=

---

### Página 107

Luego
Rl (r) = Al rl+1 + Bl r−l
Nos queda únicamente la ecuación para Θ

 

dΘ
m2
1 d
sin ϑ
+ l(l + 1) −
Θ=0
sin ϑ dϑ
dϑ
sin2 ϑ
Sea µ = cos ϑ, 0 ≤ ϑ ≤ π → −1 ≤ µ ≤ 1

P (µ) = Θ(ϑ)
dΘ
dµ dP
dP
=
= − sin ϑ
dϑ
dϑ dµ
dµ
1 d
d
=−
dµ
sin ϑ dϑ
Luego la ecuación es
d
dµ



dP
(1 − µ )
dµ





m2
+ l(l + 1) −
1 − µ2



P =0

Esta es la ecuación generalizada de Legendre, sus soluciones se llaman funciones asociadas
de Legendre. Estudiaremos primero la ecuación ordinaria de Legendre
m=0
Esto equivale a resolver el problema de Laplace para casos en que existe simetría azimutal
(es decir, donde el potencial no depende de la variable ϕ). En este caso
 dP
d
1 − µ2
+ l(l + 1)P (µ) = 0
dµ
dµ
Las soluciones deben ser monovalentes, finitas, y continuas en −1 ≤ µ ≤ 1. Estos son los
polinomios de Legendre

9.7.

Problemas de Contorno con Simetría Azimutal

Para problemas con simetría esférica y simetría azimutal (es decir, el potencial no depende
de ϕ)
R(r)
Θ(ϑ)
r
La solución general a la ecuación de Laplace queda en términos de potencias de r y polinomios de Legendre
φ = φ(r, ϑ) =

φ(r, ϑ) =

∞
X
l=0


Al rl + Bl r−(l+1) Pl (cos ϑ)
Al , Bl

---

### Página 108

se determinan usando las condiciones de contorno
Problema :Potencial en una esfera

El problema a resolver es
~x ∈ S(a) : φ(~x) = φD (ϑ)
~ 2 φ(~x) = 0
~x ∈ V : ∇

a) Problema interno (r ≤ a)
Se requiere que φ(| ~x |= 0) sea finito, de forma que Bl = 0 (l = 0, 1, 2, ...)
φ(r, ϑ) =

∞
X

Al rl Pl (cos ϑ)

l=0

La condición de contorno es

φ(a, ϑ) = φD (ϑ) =

∞
X

Al al Pl (cos ϑ)

l=0

es una serie de Legendre. Luego
2l + 1
Al =
2al

ˆ π

dϑ sin ϑPl (cos ϑ)φD (ϑ)

b) Problema externo (r ≥ a)
Se debe tener
lím φ(~x) = 0

|~
x|→∞

con lo que
Al = 0, l = 0, 1, 2, ...
luego
φ(r, ϑ) =

∞
X
Bl
l=0

rl+1

Pl (cos ϑ)

---

### Página 109

el potencial debe ser continuo en el contorno, por lo que
φ(a, ϑ) =

∞
X
Bl
l=0

de donde

2l + 1 l+1
Bl =
a

al+1

ˆ π

Pl (cos ϑ) = φD (ϑ)

dϑ sin ϑPl (cos ϑ)φD (ϑ)

---

### Página 110

Problema
Se tiene una esfera conductora cuyos hemisferios se encuentran a distinto potencial



φ0 si 0 ≤ ϑ ≤ π/2
−φ0 si π/2 ≤ ϑ ≤ π

φD (ϑ) =

Encontrar el potencial electrostático en el interior de la esfera, y la densidad superficial de cargas
#### Solución
Se trata de un problema con simetría azimutal donde el potencial satisface la ecuación de
Laplace excepto en el contorno r = a. Para el problema interno, el potencial es de la forma
φ(r, ϑ) =

∞
X

Al rl Pl cos(ϑ)

l=0

(se ha exigido que debe ser finito en r = 0). Además se cumple
φ(a, ϑ) =

∞
X

Al al Pl cos(ϑ) = φD

l=0

de donde se obtiene

2l + 1
Al =
2al

2l + 1
Al =
2al

ˆ π/2

2l + 1
Al = φ0
2al

ˆ π

dϑ sin ϑPl (cos ϑ)φD (ϑ)

dϑ sin ϑPl (cos ϑ)φ0

ˆ π

)

dϑ sin ϑPl (cos ϑ)

dµPl (µ) −

ˆ −1


dµPl (µ)

dµPl (µ) −

ˆ 0

dϑ sin ϑPl (cos ϑ)φ0 −

(ˆ
π/2

π/2

dϑ sin ϑPl (cos ϑ) −

2l + 1
Al = −φ0
2al
2l + 1
Al = φ0
2al

ˆ 0

ˆ 1

!

ˆ π

π/2

−1


dµPl (µ)

Si l es par, Pl (µ) = Pl (−µ), mientras que si l es impar, Pl (µ) = −Pl (−µ). Luego, Al = 0
para l par, y
ˆ
φ0 1
Al = (2l + 1) l
dµPl (µ)
a 0
para l impar. Además, se tiene que para l = 2n − 1, n = 1, 2, 3...

---

### Página 111

ˆ 1

dµP2n−1 (µ) = (−1)n+1

(2n − 3)!!
2n n!

Luego
φr,ϑ = φ0

∞
X
(−1)n+1 (4n − 1)(2n − 3)!!

a2n−1 2n n!

n=1

r2n−1 P2n−1 (cos ϑ)

Con esto es posible encontrar la densidad superficial de cargas, puesto que
~ ϑ) · r̂ = −0 ∇φ(r,
~
σ(ϑ) = 0 E(a,
ϑ)
σ(ϑ) = −0

r=a

· r̂

∂φ(r, ϑ)
∂r
r=a

∞
X
∂φ
(−1)n+1 (4n − 1)(2n − 1)!! 2n−2
P2n−1 (cos ϑ)
= φ0
r
∂r
a2n−1 2n n!
n=1

luego

∞

σ(ϑ) = 0

φ0 X (−1)n+2 (4n − 1)(2n − 1)!!
P2n−1 (cos ϑ)
a n=1
2n n!

Fig. 9.1: Equipotenciales para φ0 = 100 [V] y usando 10 términos en la expansión

---

### Página 112

Problema
Encuentre el potencial en todo el espacio de un anillo de radio R cargado con carga Q uniforme
#### Solución
El potencial en todo el espacio (excepto sobre el anillo) cumple
~ 2 φ(~x) = 0
∇

Ya fue resuelto anteriormente el valor del potencial sobre el eje z
φ(z) =

Q
√
4π0 z 2 + R2

Es claro que el problema posee una simetría azimutal (el potencial no depende del ángulo
polar ϕ). Con esto
φ(r, ϑ) =

∞
X
l=0


Al rl + Bl r−(l+1) Pl (cos ϑ)

Se deben imponer las condiciones de contorno adecuadas. Como conocemos el potencial
sobre el eje z, es decir para ϑ = 0
φ(r, 0) =

φ(r, 0) =

Q
√
4π0 r2 + R2

∞
∞
X
X


Q
l
−(l+1)
l
−(l+1)
A
P
A
=
r
+
B
r
(1)
=
r
+
B
r
l
l
l
l
l
4π0 (r2 + R2 )1/2
l=0
l=0

pues Pl (1) = 1 para todo l = 0, 1, 2, ...
∞
X

Q
Al rl + Bl r−(l+1)
φ(r, 0) =
=
1/2
4π0 (r2 + R2 )
l=0

Separamos en dos casos
1) r > R

Q 1
Q

1/2 =

4π0
4π0 r
r 1 + Rr

 2 !−1/2
R
1+
r

---

### Página 113

−1/2

Como R/r < 1, la expansión en serie de potencias de (1 + (R/r)2 )
por

con

 2 !−1/2
∞
X
dl
xl
R
−1/2
= (1 + x)
=
1+
f (x)
r
dx
x=0 l!
l=0
f (x) = (1 + x)−1/2

se tiene
f (x)

x=0

=1

=−
x=0
  
f 00 (x)
=
x=0
   
f 000 (x)
=−
x=0
    
=
f 4 (x)
x=0
f 0 (x)

En general

f l (x)

x=0

=

(−1)l (2l − 1)!!
2l

de forma que

Entonces

 2 !−1/2 X
 2l
∞
R
R
l (l − 1)!!
1+
=
(−1)
l
r
2 l!
r
l=0
∞
2l
Q X
Q
l (l − 1)!! R
(−1)

2 1/2 = 4π0
4π0
2l l! r2l+1
l=0
r 1 + Rr
∞
X

l

Al r + Bl r

−(l+1)

l=0



∞

2l
Q X
l (l − 1)!! R
=
(−1)
4π0 l=0
2l l! r2l+1

Por supuesto que debe tenerse
lím φ(~x) = 0

|~
x|→∞

por lo que
Al = 0, ∀l
∞
X
l=0

∞

Bl r

−(l+1)

(l − 1)!! R2l
Q X
=
(−1)l
4π0 l=0
2l l! r2l+1

de aquí se obtiene que Bl = 0 para l impar, luego

converge, y está dada

---

### Página 114

∞
X

∞

B2l r−(2l+1) =

l=0

B2l =

Q X
(l − 1)!! R2l
(−1)l
4π0 l=0
2l l! r2l+1

Q (−1)l (2l − 1)!! 2l
R
4π0 2l
l!

y entonces el potencial queda, para r > R
∞
X
Q (−1)l (2l − 1)!! 2l −(2l+1)
φ(r, ϑ) =
P2l (cos ϑ)
R r
4π0 2l
l!
l=0

2) caso en que r < R
Aquí el potencial será de la forma
φ(r, ϑ) =

∞
X
l=0


Cl rl + Dl r−(l+1) Pl (cos ϑ)

Se requiere que el potencial sea finito, luego Dl = 0 para todo l = 0, 1, 2... la condición de
contorno en el eje z, z > 0 entrega
φ(r, 0) =

∞
X

Cl rl =

l=0

Q
4π0 R (1 + (r/R)2 )−1/2

Como r/R < 1, está garantizada la convergencia de la serie de potencias de
1 + (r/R)2
∞
X

−1/2

∞
Q 1X
(2l − 1)!! r2l
Cl r =
(−1)l
4π0 R l=0
2l l! R2l
l=0

∞
X

l

∞

Q X
(2l − 1)!! r2l
Cl r =
(−1)l
4π0 l=0
2l l! R2l+1
l=0
l

de aquí es inmediato que Cl = 0 para l impar
∞
X

∞

(2l − 1)!! r2l
Q X
C2l r =
(−1)l
4π0 l=0
2l l! R2l+1
l=0
2l

C2l =

(2l − 1)!!
Q
(−1)l l 2l+1
4π0
2 l!R

Finalmente, el potencial está dado por
∞
X
Q
(2l − 1)!!
φ(r, ϑ) =
(−1)l l 2l+1 rl P2l (cos ϑ), r < R
4π0
2 l!R
l=0

---

### Página 115

φ(r, ϑ) =

∞
X
Q (−1)l (2l − 1)!! 2l −(2l+1)
P2l (cos ϑ), r > R
R r
l
4π
l!
l=0

Fig. 9.2: La figura muestra la solución para r > R, tomando 40 términos

Fig. 9.3: La figura muestra la solución para r < R
