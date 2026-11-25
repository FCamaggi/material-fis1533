---
title: "Problemas Resueltos de Electromagnetismo - Rodrigo Chi"
source_pdf: "Electro/material-apoyo/compilados/Problemas Resueltos de Electromagnetismo - Rodrigo Chi.pdf"
pages: 383
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Problemas Resueltos de Electromagnetismo - Rodrigo Chi

### Página 1

Problemas Propuestos y
Resueltos de Electromagnetismo

+

-

Rodrigo Chi Durán
Versión Marzo 2017

---

### Página 2

Rodrigo Chi - Marzo 2017

---

### Página 3

Índice general

I

Electrostática

1. Distribuciones Discretas de Cargas

2. Distribuciones Continuas de Cargas

3. Ley de Gauss

4. Conductores

5. Ecuación de Laplace y Poisson

6. Dipolo Eléctrico

7. Dieléctricos

II

Corriente Eléctrica

8. Medios Conductores

9. Circuitos Eléctricos

i

---

### Página 4

ÍNDICE GENERAL

III

Magnetostática

10.Ley de Biot-Savart

11.Fuerza de Lorentz

12.Ley de Ampère

13.Potencial y Momento Magnético

14.Medios Magnéticos

IV

Campos Electromagnéticos Variantes en el Tiempo

16.Inductancia y Energía Magnética

17.Corriente Alterna

18.Leyes de Maxwell

Rodrigo Chi - Marzo 2017

15.Ley de Faraday-Lenz

ii

---

### Página 5

ÍNDICE GENERAL

Prólogo
El Electromagnetismo es posiblemente una de las ramas más bonitas de las física, la cual tiene
muchas aplicaciones cotidianas de las cuales no nos damos cuenta: prender la luz, llamar por
celular o usar el computador. El estudio de esta área en el último siglo ha provocado un avance
considerable en la tecnología y nos entrega un mayor bienestar diariamente.
El apunte aquí presente, nace como una recopilación de problemas propuestos y resueltos durante
el tiempo que he sido Profesor Auxiliar en la Universidad de Chile y mi breve paso por la Universidad de los Andes. La mayoría de los problemas disponibles han sido extraídos de evaluaciones
(controles, ejercicios, tareas, etc) y de guías de problemas propuestos que elaboré para que mis
alumnos estudiaran. Aclaro que la mayoría de los problemas presentes no son de mi autoría sino
de los profesores de la Facultad de Ciencias Físicas y Matemáticas de la Universidad de Chile y
algunos otros inspirados en la bibliografía.
Mi principal objetivo con este apunte es entregar un buen material de estudio para las personas que
necesiten estudiar y/o que simplemente quieran aprender. Además, el hecho de reunir el material
que confeccioné durante varios semestres en un solo lugar hace que el trabajo sea mucho más útil
y duradero para las personas que quieran utilizarlo.
Este compilado posee dos tipos de problemas: algunos con su solución completa y otros que solamente poseen su respuesta final. Como siempre es recomendado, es importante que al momento
de usar este apunte se den el tiempo de pensar el problema antes de mirar su solución (si es que
la posee). Un rol activo en la resolución de problemas les traerá muy buenos resultados durante
este curso.

Dado lo reciente de esta recopilación, probablemente existan errores de los cuales han pasado
desapercibidos. Les pido por favor a los estudiantes que los encuentren que me los notifiquen, así
ganarán buen karma y otros futuros estudiantes se los agradecerán.
¡Mucho Éxito!

iii

Problemas Propuestos y Resueltos de Electromagnetismo

He querido ser detallista en la selección de problemas, de modo que en la mayoría de los capítulos
he intentado plasmar un espectro representativo de los de problemas que suelen ser preguntados
en la FCFM (aunque hay profesores que su ingenio siempre puede más).

---

### Página 6

ÍNDICE GENERAL

Agradecimientos
Quiero agradecer a las personas que han hecho posible realizar este proyecto, a los profesores
Pablo Zegers, Daniel Escaff, Simón Casassus, Carlos Cartes, Takeshi Asahi, Matías Montesinos y
en particular, a Marcel Clerc y Claudio Romero.
A mis compañeros auxiliares que aportaron con problemas y soluciones: Susana Márquez y Luis
Mateluna.

Rodrigo Chi - Marzo 2017

Y finalmente a Matías Mattamala por su ayuda en la confección de la portada.

iv

---

### Página 7

ÍNDICE GENERAL

Notas de la Edición - Marzo 2017
La presente versión cuenta con 18 capítulos, donde existen 222 problemas propuestos de
los cuales 111 tienen solución.
Cada capítulo posee un resumen de fórmulas que le serán útiles.
Los problemas tienen una simbología de acuerdo a su dificultad:
-

-

-

significa que un problema es sencillo y debería ser resuelto en forma rápida.
significa que el problema intermedio y requiere un mayor análisis o trabajo algebraico.
significa que es un problema difícil, que requiere un análisis prolongado.

Todos los problemas del apunte cuentan con su respectiva respuesta al final de cada capítulo.
Se indica su solución con el símbolo X .
En el enunciado de cada problema se detalla si este tiene solución mediante el símbolo S .
En caso que el problema no posea solución, este contará con indicaciones I que lo ayudarán
a resolverlo.
Cualquier error o corrección, por favor contactarse al correo rchi@ing.uchile.cl .

Problemas Propuestos y Resueltos de Electromagnetismo

v

---

### Página 8

Rodrigo Chi - Marzo 2017

ÍNDICE GENERAL

vi

---

### Página 9

Parte I
Electrostática

---

### Página 10

Rodrigo Chi - Marzo 2017

---

### Página 11

Distribuciones Discretas de Cargas

I.

Resumen Teórico

Ley de Coulomb
La fuerza entre dos cargas q1 y q2 separadas una distancia r, es directamente proporcional al
producto de las cargas e inversamente al cuadrado de la distancia que las separa.
|F~ | =

1 q 1 q2
4πε0 r2

(1.1)

Definición de Campo Eléctrico
~ en un punto dado por el vector posición ~r2 provocado por una carga q1 en
El campo eléctrico E
una posición ~r1 , puede ser determinado como
~
~ = F = q1 ~r2 − ~r1
E
q2
4πε0 |~r2 − ~r1 |3

(1.3)

Principio de Superposición
~ existente en un punto del espacio es igual a la suma de todos los campos
El campo eléctrico E
eléctricos generados por todas las distribuciones de cargas existentes en ese espacio.

Problemas Propuestos y Resueltos de Electromagnetismo

Si las cargas son de distinto signo la fuerza es atractiva, en caso contrario, la fuerza es repulsiva.
Vectorialmente, si las cargas q1 y q2 se encuentran en las posiciones ~r1 y ~r2 , respectivamente, la
fuerza que siente la carga q1 es
q1 q2 ~r2 − ~r1
(1.2)
F~ =
4πε0 |~r2 − ~r1 |3

---

### Página 12

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS

Campo Eléctrico por Cargas Puntuales
El campo eléctrico en una posición ~r provocado por N cargas puntuales q1 , q2 , . . . , qN ubicadas
respectivamente en las posiciones ~r1 , ~r2 , . . . , ~rN se encuentra dado por
N
qi (~r − ~ri )
1 X
4πε0 i=1 |~r − ~ri |3

~ r) =
E(~

(1.4)

Conservación del Campo Eléctrico
El campo eléctrico debido a cargas estáticas es conservativo, es decir
~ ×E
~ =0
∇

(1.5)

O equivalentemente para cualquier camino cerrado Γ
˛
~ =0
~ · dl
E

(1.6)

Γ

Por otro lado, esto implica que existe una función escalar V tal que
~ = −∇V
E

(1.7)

La función V se denomina Potencial Eléctrico.

Rodrigo Chi - Marzo 2017

Potencial y Trabajo Eléctrico
El trabajo eléctrico de mover una carga q desde un posición A a otra ubicación B bajo la oposición
~ está dado por
de un campo eléctrico E
ˆB

ˆB
~ = −q
F~ · dl

W =−
A

~
~ · dl
E

(1.8)

A

Físicamente, el potencial eléctrico es el trabajo por unidad de carga que es necesario aplicar para
mover una carga desde una posición inicial A (conocida como referencia) a otra final B. Usando
las Ecuaciones 1.7 y 1.8, se obtiene que
ˆB
~
~ · dl
E

V (B) − V (A) = −
A

(1.9)

---

### Página 13

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS

Potencial Eléctrico por Cargas Puntuales
El potencial eléctrico debido a una carga puntual q es
V (~r) =

q
4πε0 r

(1.10)

donde r es la distancia de la carga al punto donde se quiere conocer el potencial.

Potencial Eléctrico por Cargas Puntuales
Por principio de potencial eléctrico, para N cargas puntuales está dado por
V (~r) =

N
qi
1 X
4πε0 i=1 |~r − ~ri |

(1.11)

Recomendaciones
Nunca olvidar que el campo eléctrico es un campo vectorial (a todo punto en el espacio se
le asigna un vector) y el potencial un campo escalar (a todo punto en el espacio se le asigna
un número real).

Para distribuciones finitas de carga, como las cargas puntuales, se suele tomar de referencia
el infinito, ie. V (A −→ ∞) = 0. Esto siempre puede ser tomado así excepto cuando exista
carga en el infinito (distribuciones infinitas de carga).

Problemas Propuestos y Resueltos de Electromagnetismo

Es muy importante tomar la intuición que el campo eléctrico de una carga puntual es siempre
radial al punto donde se quiere conocer el campo.

---

### Página 14

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS

II.

Problemas Propuestos

#### Problema 1.1

X S

Considere una partícula puntual con carga q y masa
m la cual está sujetada mediante un péndulo de largo
`. En el espacio donde se encuentra la carga existe un
~ que forma un ángulo α
campo eléctrico conocido E
con respecto a la vertical (ver Figura).
a) Encuentre en ángulo de equilibrio θ0 el cual
tendrá la carga.

g

q

`

q, m

a

~E

b) Si la carga es perturbada débilmente de su posición equilibrio, ¿Cuál será su frecuencia de pequeñas oscilaciones?.
#### Problema 1.2

X I

Considere dos partículas puntuales de carga positiva
q1 y q2 y masas m1 y m2 , respectivamente. Ambas
cargas se encuentran sobre una plataforma circular de
radio R sin roce y bajo el efecto de la gravedad. En
el equilibrio las partículas forman ángulos θ1 y θ2 con
respecto a la vertical.
a) Determine la relación de las entre las masas m1
y m2 .

Rodrigo Chi - Marzo 2017

b) Demuestre que m1 = m2 es condición necesaria
y suficiente para que θ1 = θ2 , independiente del
valor de las cargas q1 y q2 .
c) Ahora, suponga que q1 = q2 , m1 = m2 y por
ende θ1 = θ2 = θ. Si ambas cargas se dejan caer
desde un ángulo θ
1 y éstas pierden carga a
= −α [C/s]. ¿A qué velocidad ~v (θ) se
razón dq
dt
acercan ambas partículas?.

q1

q2

~g
R

q 1 , m1
q 2 , m2

---

### Página 15

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS

e
#### Problema 1.3

X S

En los vértices de un triángulo equilátero de lado L se
han situado tres cargas negativas −e. Si en el centro
de gravedad del triángulo se sitúa una carga de magnitud Q, determine el valor que debe poseer esa carga
para mantener el sistema en equilibrio.

L

L
Q
L

e

#### Problema 1.4

e

X I

Un electroscopio es un instrumento para determinar si
un objeto se encuentra cargado. Un modelo simplificado para explicar su funcionamiento son dos esferas
metálicas de igual masa m las cuales cuelgan por dos
hilos conductores de largo L. Estas esferas adquieren
igual carga q al momento en que se toca el objeto
cargado con la esfera metálica superior.

~g

w

q q
L

L
q

q

a) Determine el valor de la carga q de las esferas si
experimentalmente se ha medido que θ = 30◦ .

#### Problema 1.5

z

X I

En los vértices de un cubo de lado a se han puesto
ocho cargas puntuales de igual carga q como se indica
en la Figura. Sea P el punto ubicado en el centro de la
cara del cubo que yace sobre el plano xy. Determine

a
a

a) El campo eléctrico en P .
b) Determine el trabajo necesario para traer desde
el infinito una carga Q y dejarla en el punto P .

a
x

P

y

Problemas Propuestos y Resueltos de Electromagnetismo

b) El sistema se hace girar con una velocidad angular ω observándose que el ángulo de equilibrio
cambia a θ = 60◦ . Determine el valor de ω.

---

### Página 16

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS
#### Problema 1.6

X I

+q

Considere un polígono regular de lado a y 2n vértices,
donde consecutivamente se han puesto n cargas positivas q y luego n cargas negativas −q. En la Figura
se muestra el caso n = 3. Determine
a) El campo eléctrico y el potencial eléctrico en el
centro de hexágono (n = 3).

q

+q
y

a

x
q

+q

b) El módulo del campo eléctrico en el centro del
polígono para el caso general de n vértices.

q

z
#### Problema 1.7

X I

q

z=a

Considere dos cargas positivas q puestas sobre en el eje
z. Si las cargas se ubican z = a y z = −a determine el
lugar geométrico de los puntos los cuales maximizan
el módulo del campo eléctrico sobre el plano xy.

y
x

#### Problema 1.8

q

z= a

X S

Suponga que en lugar de la Ley de Coulomb, uno
hubiera encontrado experimentalmente que la fuerza
entre dos cargas puntales fuera

Rodrigo Chi - Marzo 2017

F~12 =

q1 q2 (1 −
4πε0

q

α|~r2 − ~r1 |)

|~r2 − ~r1 |3

q2

(~r2 − ~r1 )

donde α es una constante.
a) Escriba el campo eléctrico a una carga puntual.
Coloque el origen de coordenadas en la carga
puntual.
b) Elija una trayectoria cerrada alrededor de la car¸
~ Compare el re~ · dl.
ga y calcule la integral E
sultado obtenido con la Ley de Coulomb.
‚
~ so~ · dS
c) Encuentre en valor de la integral
E
bre una superficie esférica centrada en la carga.
Compare el resultado obtenido con la Ley de
Coulomb.

~F21
~r2

q1
~F12

~r1

O

---

### Página 17

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS
#### Problema 1.9

X S

Líquido Cargado

En un recipiente metálico existe un líquido cargado el
cual se encuentra a un potencial V0 constante. El recipiente posee muy pequeño orificio por el cual caen
gotas esféricas de radio a hacia otro recipiente esférico
de radio R el cual posee una pequeña abertura. Este
segundo recipiente se encuentra inicialmente descargado y muy alejado del otro recipiente.
a) Determine la carga que posee cada gota al momento de caer del primer recipiente.

R

b) Determine el potencial al cual se encuentra el
recipiente esférico una vez que está completamente lleno.

X S

La cohesión en los cristales iónicos se debe a las fuerzas eléctricas de atracción entre los iones positivos y
negativos. Considere un modelo unidimensional de un
cristal de Cloruro de Sodio (NaCl) que consiste en una
línea recta infinita en que están colocados los iones,
alternándose los iones positivos de Na y los iones negativos de Cl. La distancia entre iones vecinos es a.
Los iones positivos tienen carga +e y los iones negativos −e. Calcule la energía que hay que entregarle a un
ion positivo de Na para sacarlo de su lugar y llevarlo
a una distancia muy grande respecto a a.

Na

a

Cl
Na
Cl
Na
Cl

Problemas Propuestos y Resueltos de Electromagnetismo

#### Problema 1.10

---

### Página 18

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS

III.

Soluciones

Solución 1.1

P X

Para enfrentar este problema es necesario fijar un sistema de referencia cómodo, para luego
plantear las ecuaciones de movimiento.

y

g

x q

`
~Ey

q, m

a

~Ex

~E

Figura 1.1: Descomposición del campo eléctrico.
~ x = E cos αx̂ y E
~ y = E sin αŷ. Notése que hay tres
Según la Figura 1.1 es posible afirmar que E
fuerzas actuando sobre la carga: el peso, la fuerza eléctrica y la tensión de la cuerda. Ahora, se
procede a volver a descomponer las fuerzas anteriormente nombradas según r̂ y θ̂ en coordenadas
cilíndricas.
X
F~ = qE(cos αx̂ + sin αŷ) + mgx̂ − T r̂
m~a =
Como x̂ = cos θr̂ − sin θθ̂ y ŷ = sin θr̂ + cos θθ̂ la expresión anterior puede ser reescrita como

Rodrigo Chi - Marzo 2017

m~a = ((qE cos α + mg) cos θ + qE sin α sin θ)r̂ + (−(qE cos α + mg) sin θ + qE sin α cos θ)θ̂
En el equilibrio debe cumplirse ~a = 0, por lo cual el ángulo de equilibrio puede ser determinado a
partir de anular la componente en θ̂ de la aceleración, por lo tanto
−(qE cos α + mg) sin θ0 + qE sin α cos θ0 = 0 =⇒ tan θ0 =

qE sin α
qE cos α + mg

Para encontrar las pequeñas oscilaciones del péndulo hay que hallar una ecuación diferencial de
la forma
θ̈ + ω 2 θ = cte
Para ello se usa nuevamente la componente en θ̂ de la aceleración, de modo que
m`θ̈ = −A sin θ + B cos θ
donde se ha definido por simplicidad A = qE cos α + mg y B = qE sin α. De la expresión anterior
es necesario linealizar las funciones no lineales f1 (θ) = sin θ y f2 (θ) = cos θ para llegar a la

---

### Página 19

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS
ecuación deseada. Para encontrar la expresión es necesario usar una aproximación de Taylor al
primer orden entorno a θ0 el cual está dado por
f (θ) ≈ f (θ0 ) +

df
· (θ − θ0 )
dθ θ=θ0

Luego, se tiene que
sin θ ≈ sin θ0 + cos θ0 (θ − θ0 )
cos θ ≈ cos θ0 − sin θ0 (θ − θ0 )
Entonces, la ecuación de movimiento de la carga se transforma en
m`θ̈ = −A(sin θ0 + cos θ0 (θ − θ0 )) + B(cos θ0 − sin θ0 (θ − θ0 ))
Operando algebraicamente la expresión anterior se obtiene que
!

A cos θ0 + B sin θ0
θ̈ +
θ=K
m`
donde K es un valor constante. Trabajando nuevamente con la expresión
!

θ̈ + cos θ0

A + B tan θ0
θ=K
m`

Finalmente reemplazando los valores conocidos de A, B, tan θ0 y dado cos θ0 = √

1+tan2 θ0

se

concluye que
q

ω2 =

(qE cos α + mg)2 + (qE sin α)2
m`

En este problema se aprecia una simetría con respecto a la carga Q, ya que todas las cargas
negativas sienten la misma fuerza de atracción/repulsión. Por ejemplo, haciendo el DCL a la
carga superior se obtiene lo siguiente
Las fuerzas F~1 y F~2 son repulsivas (generadas por las otras cargas negativas), mientras que la
fuerza F~3 generada por la carga Q positiva es atractiva. Usando el sistema de referencia de la
Figura 1.2 y la Ley de Coulomb, es posible descomponer las fuerzas de la siguiente forma
F~1 =

e2
π
π
−x̂
cos
+
ŷ
sin
,
4πε0 L2




F~2 =

e2
π
π
x̂
cos
+
ŷ
sin
,
4πε0 L2




eQ
F~3 = −
ŷ
4πε0 d2

donde d es la distancia desde cualquier vértice al centro del triángulo. Usando el Teorema del
Coseno, es posible despejar d como
L2 = d2 + d2 − 2d2 cos

2π
L2
=⇒ d2 =

Problemas Propuestos y Resueltos de Electromagnetismo

P X

Solución 1.3

---

### Página 20

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS
~F1

y

~F2

e

x

~F3

L

L
Q

e

L

e

Figura 1.2: DCL Sobre la Carga Superior
por lo tanto la fuerza total vale
!

e2
π
3eQ
sin
−
ŷ
2πε0 L2
3 4πε0 L2

F~T =

Dado que se desea el sistema en equilibrio se impone F~T = 0, obteniéndose que
√
e2
π
3eQ
e 3
e
√
sin
−
=
=⇒
Q
=
=
2πε0 L2
3 4πε0 L2

Solución 1.8

P X

a) Colocando la carga q1 en el origen se obtiene ~r1 = 0. Luego llamando q1 = q y recordando
~ se puede obtener que
que F~ = q2 E,
q

q

Rodrigo Chi - Marzo 2017

(1 − α|~r2 |)
q2 q (1 − α|~r2 |)
~ = q ·
F~ =
r
~
=⇒
E
~r2
·
4πε0
|~r2 |3
4πε0
|~r2 |3
Como la dirección de la fuerza y el campo es radial podemos decir que ~r2 = rr̂. Finalmente
√
q
(1 − αr)
~
E=
r̂
·
4πε0
r2
b) Basta tomar una trayectoria cerrada Γ, por ejemplo, una circunferencia de radio R alrededor
de la carga. En ese caso se tiene que la curva queda parametrizada como:
˛

ˆ2π
~ · d~l =
E

Γ

~ · Rdθθ̂ = 0
|E|r̂

Para el caso de la ley de˛Coulomb se tiene que el campo es siempre conservativo, es decir
~ = 0, por lo cual
~ · d~l = 0 para cualquier camino cerrado Γ. Se concluye que la
∇×E
E
Γ

ley de Coulomb y la ley encontrada experimentalmente entregan el mismo resultado.

---

### Página 21

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS
c) Para este caso hay que calcular una integral de flujo. Por simplicidad se elige una esfera de
radio R centrada en el origen. Luego el flujo sobre su superficie es
"

ˆ2π ˆπ
~ · dS
~=
E

Ω

√
√
(1 − αR) 2
q
q
·
(1
−
αR)
r̂R
sin
θdθdϕr̂
=
4πε0
R2
ε0

Para el caso de la ley de Coulomb, se sabe que esa integral es conocida ya que coincide con
la Ley de Gauss, es decir
"
~ · dS
~= q
E
ε0
√
Para la nueva ley se tiene que difiere en un factor (1 − αR) , además el flujo no es
constante como en la Ley de Gauss y depende de la superficie esférica que se tome.

Solución 1.9

P X

a) Dado que las gotas tienen forma esférica caen con un potencial inicial V0 con respecto al
infinito. Suponiendo que caen con una carga Q, es conocido que el campo eléctrico que
produce la gota para puntos fuera de ella es:
~ =
E

Q
r̂
4πε0 r2

Lo anterior implica potencial de la esfera es
V (a) =
a

Q
Q
dr =
= V0 =⇒ Q = 4πε0 V0 a
4πε0 r
4πε0 a

b) Sea QT la carga del recipiente esférico una vez que se llena. Suponiendo que la carga se
distribuye de forma uniforme en el recipiente, la densidad de carga del agua total que se
acumule en el recipiente esférico debe ser igual a la de cada gota, es decir
Carga de una gota
Carga total en el recipiente
=
Volumen de una gota
Volumen del recipiente esférico
De lo anterior se deduce que
QT
Q
R3
R3
=
=⇒
Q
=
Q
=
· 4πε0 V0
T
g
a3
a2
πR3
πa3
Luego, usando el resultado de la primera parte, el potencial está dado por
V (R) =

QT
R2
= 2 V0
4πε0 R
a

Problemas Propuestos y Resueltos de Electromagnetismo

ˆ∞

---

### Página 22

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS

y
e Na

Cl

Na

Cl

Cl

Na

Cl

e

e

e

e

e

e

3a

2a

a

a

2a

3a

x

Figura 1.3: Cadena de NaCl
Solución 1.10

P X

Para resolver este problema es útil definirse un sistema de referencia conveniente.
La energía necesaria para mover el ion positivo y llevarlo a un punto muy lejano con respecto a
la distancia a es el equivalente al trabajo necesario para mover la carga desde el origen hacia el
infinito (ver Figura 1.3). Dado lo anterior, el valor buscado es
ˆ∞
W =−

ˆ∞
~ = −e (−∇V ) · dl
~ = e(V (∞) − V (0)) = −eV (0)
~ · dl
eE

Rodrigo Chi - Marzo 2017

El problema se reduce a encontrar el potencial en el origen, para ello se usa la superposición de los
potenciales de cada carga puntual e y −e de la cadena infinita. Como las cargas están ubicadas
en forma simétrica al eje y, el potencial en el origen es dos veces el potencial que genera un solo
lado de la cadena, por lo tanto
∞
∞
e(−1)i
e X
(−1)i
2 X
=
V (0) =
4πε0 i=1 ai
2πε0 a i=1 i

Finalmente, recordando que ln(1 + x) =

∞
X
(−1)n−1
n=1

U = −eV (0) = −e · −

n

xn se tiene que

∞
e X
(−1)i−1
e2
=
ln(2)
2πε0 a i=1
i
2πε0 a

---

### Página 23

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS

IV.

Indicaciones Problemas Sin Solución

Indicación 1.2

P X

Determine las fuerzas que se aplican a ambas cargas, para ello trace la línea imaginaria que
une ambas cargas y determine su longitud mediante el teorema del coseno. Note que se
forma un triángulo isósceles debido a que la distancias a las cargas es R desde el centro
de la circunferencia. La dificultad de este problema se radica en poder relacionar en forma
correcta los ángulos.
Una vez determinada la relación entre las masas, analice que sucede cuando m1 = m2 y
cuando θ1 = θ2 . ¿Influye el valor de las cargas?.
dq dθ
= dθ
. Pueden ser
Para la última parte, determine el valor de q(θ) y luego note que dq
dt
dt
útiles las aproximaciones sin θ ≈ θ y tan θ ≈ θ para θ
1.

Indicación 1.4

P X

Analice las fuerzas aplicadas sobre la carga considerando θ = 30◦ . Dado que el sistema se
encuentra en equilibrio estático la fuerzas aplicadas deben sumar cero.

Indicación 1.5

P X

Para encontrar el campo eléctrico en se recomienda determinar primero el campo que provocan las cuatro cargas en el plano xy en P . Luego, determine el campo eléctrico que genera
una de las cuatro cargas en z = a. Finalmente, por simetría, el resultado debe apuntar sólo
en la dirección de ẑ con lo cual puede concluir el resultado.
Basta con determinar el potencial en P . Recuerde que el trabajo está dado por W = QV (P ).

Indicación 1.6

P X

Superponga los campos eléctricos en el centro de hexágono y sume los vectores.

Problemas Propuestos y Resueltos de Electromagnetismo

Cuando el sistema comienza a rotar la aceleración ya no es nula como en la parte anterior.
Modifique las ecuaciones de movimiento imponiendo lo anterior y considerando que el nuevo
ángulo es θ = 60◦ . Se recomienda trabajar en coordenadas cilíndricas.

---

### Página 24

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS
Generalizando el resultado anterior, intente encontrar alguna relación entre los 2n campos eléctricos superpuestos en el origen y luego sume. La sumatoria puede ser reducida
algebraicamente.

Indicación 1.7

P X

Rodrigo Chi - Marzo 2017

El lugar geométrico debe ser una circunferencia. Suponga un radio r para esa circunferencia
y luego derive e iguale a cero para encontrar el máximo.

---

### Página 25

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS

V.

Respuestas
Problema

P

1.1

sin α
a) tan θ0 = qEqE
cos α+mg
√
(qE cos α+mg)2 +(qE sin α)2
b) ω 2 =
m`

a)

P

1.2

P

1.3

P

Respuestas

16πε0 L2 g
m1 −m2
sin( θ2 −θ
m1 m2 =
q1 q2
2 )(1 − cos(θ1 + θ2 ))

c) |v(θ)| = √

1.4

α
4πε0 mgθ

Q = √e3
q√
a) q = ` 33 πε0 mg
b) ω = 4g
3`

P

1.6

√
~
a) E(0)
= 4πεq0 a2 (2 3x̂ − 2ŷ), V (0) = 0
π

kπ
kπ
~ = q(1−cos2 n ) Pn
b) E
k=0 sin n x̂ + cos n ŷ
πε0 a

P

1.7

P

x2 + y 2 = a2 es una circunferencia de radio r = √a2

Problemas Propuestos y Resueltos de Electromagnetismo

1.5

3
~ total = − q 2 2 2 ẑ
a) E
πε0 a
√ √
Qq 2
b) W = 3πε
( 3 + 1)
0a

---

### Página 26

CAPÍTULO 1. DISTRIBUCIONES DISCRETAS DE CARGAS
Problema

Respuestas
√

~ = q · (1− 2 αr) r̂
a) E
4πε0
r

P

1.8

¸
~ = 0 para
~ · dl
b) Si Γ es una circunferencia de radio R sobre el plano xy entonces Γ E
ambos campos eléctricos (experimental y coulombiano).
√
!
~ · dS
~ = q (1 − αR). Para el caso
c) Para una esfera de R centrada en la carga, Ω E
ε0
!
~ · dS
~= q.
de un campo tradicional por Coulomb:
E
Ω

a) Q = 4πε0 V0 a

P

1.9

P

1.10

b) V = R
a2 V0

Rodrigo Chi - Marzo 2017

ln(2)
U = e2πε
0a

ε0

---

### Página 27

Distribuciones Continuas de Cargas

I.

Resumen Teórico

Campo Eléctrico por Continuos de Carga
Para distribuciones continuas de carga, el campo eléctrico puede ser determinado como
ˆ
~r − ~r 0
~
E=
dq(~r 0 )
4πε0
|~r − ~r |

(2.1)

Ω

donde ~r es la posición dónde se desea conocer el campo eléctrico, ~r 0 es la parametrización del
continuo de carga y dq(~r 0 ) es el elemento diferencial de línea/superficie/volumen, donde
dq(~r 0 ) = λ(~r 0 )dl = σ(~r 0 )dS = ρ(~r 0 )dV

(2.3)

Línea

~ r) =
E(~

¨

4πε0

~r − ~r 0
σ(~r 0 )dS
|~r − ~r 0 |3

(2.4)

~r − ~r 0
ρ(~r 0 )dV
|~r − ~r 0 |3

(2.5)

Superficie

~ r) =
E(~

4πε0

˚

Volumen

Potencial Eléctrico por Continuos de Carga
Para distribuciones continuas de carga, el potencial eléctrico puede ser determinado como
ˆ
dq(~r 0 )
V (~r) =
(2.6)
4πε0
|~r − ~r 0 |
Ω

Problemas Propuestos y Resueltos de Electromagnetismo

Usando la expresión anterior, el campo eléctrico puede ser determinado como
ˆ
~r − ~r 0
~
E(~r) =
λ(~r 0 )dl
4πε0
|~r − ~r 0 |3

(2.2)

---

### Página 28

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
Análogamente al caso del campo eléctrico, el potencial puede ser determinado como
ˆ
λ(~r 0 )dl
V (~r) =
4πε0
|~r − ~r 0 |

(2.7)

Línea

¨

V (~r) =
4πε0

σ(~r 0 )dS
|~r − ~r 0 |

(2.8)

ρ(~r 0 )dV
|~r − ~r 0 |

(2.9)

Superficie

V (~r) =
4πε0

˚

Volumen

La expresión anterior considera el infinito como referencia, por lo que no debe usarse cuando exista
carga en el infinito.

Recomendaciones

Rodrigo Chi - Marzo 2017

A pesar que siempre es posible determinar el campo eléctrico mediante la Ecuación 2.1, no
siempre será fácil hacerlo. De hecho, debido a la complejidad de algunas parametrizaciones,
las integrales pueden tomar una dificultad muy alta haciéndolas imposibles de resolver.

---

### Página 29

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS

II.

Problemas Propuestos

#### Problema 2.1

Z

X S

Casquete Semiesférico

Un disco de radio a completa un casquete semiesférico de radio a. Ambas superficies tienen densidad de
carga uniforme σ . Calcule el campo eléctrico en un
punto a2 sobre el eje Z.

s
a

s

Hint:

Y

d
r − z cos(x)
(z − r cos x) sin x
√
=
dx z 2 r2 − 2rz cos x + z 2
(r sin2 x + (z − r cos x)2 ) 2 Disco




X

#### Problema 2.2

l

X S

#### Problema 2.3

X S

~g
q

l
m, q

Q

Un anillo de radio R0 tiene una carga Q positiva, la
cual está distribuida de manera uniforme sobre el anillo, como se ilustra en la figura. Considere una carga
puntual de carga negativa q (q < 0) y masa m, la cual
es depositada en reposo sobre el eje central del anillo
cerca del centro representado por el punto A, además
la carga está soldada a un resorte ideal de constante
elástica k0 y largo natural cero con extremo fijo en el
punto A. Calcule la frecuencia de oscilación partícula puntual. Indicación: Considere que la partícula se
mueve sobre el eje central del anillo.

R0
k0
A

q

Problemas Propuestos y Resueltos de Electromagnetismo

Considere una barra infinita de densidad de carga lineal λ. Sobre esta barra se cuelga un péndulo ideal
de largo l y una masa puntual m y carga q, bajo la
influencia del campo gravitatorio como se ilustra en la
figura. Encuentre el ángulo de equilibrio del péndulo
y determine cuál es ángulo límite cuando el valor de
q crece infinitamente.

---

### Página 30

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
#### Problema 2.4

X S

Una densidad de carga lineal λ está repartida de forma
homogénea a lo largo de un semicircunferencia BD
centrada en C y de radio R. Una carga puntual q
está ubicada en punto A como se indica en la Figura.
(CA = R).
a) Calcule el potencial eléctrico en el punto C,
V (C).

l
R
B

C

D
R

b) Por argumentos de simetría, determine la direc~
~
ción del campo eléctrico E(C).
Calcule E(C).

A q

c) Determine la relación entre λ y q tal que
~
E(C)
=0

#### Problema 2.5

X S

Se tienen dos anillos coaxiales del mismo radio a, contenidos en planos paralelos y separados entre sí una
distancia L. Uno de los anillos tiene densidad de carga
uniforme +λ y el otro −λ.

l

a) Calcule el campo eléctrico en el eje común de
los anillos, o sea en el eje O0 O en la figura.

l

O

R
L

O

Rodrigo Chi - Marzo 2017

b) Calcule la diferencia de potencial entre los centros O0 y O de los anillos.

#### Problema 2.6

X S

y

Un alambre semi-infinito cargado yace sobre el semieje positivo x. El alambre posee una densidad lineal
homogénea λ0 .

A

a) Determine el valor del campo eléctrico en el
punto A de la figura el cual está ubicado sobre el eje y a una distancia a del origen.
b) Determine el valor del campo eléctrico en el
punto B de la figura el cual está ubicado so- B
bre el eje x a una distancia a del origen.

a
l0
a

O

x

---

### Página 31

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
l

#### Problema 2.7

X S

R

Considere un alambre muy delgado como el de la figura, éste esta compuesto por dos rectas infinitas y una
arco de circulo de 135◦ . El alambre tiene una densidad lineal de carga λ constante. Encuentre el campo
producido en el punto P .

#### Problema 2.8

P

X S

Dos barras delgadas e iguales de longitud L y carga
total Q distríbuida uniformemente, están situadas sobre el eje x, separadas una distancia d como se indica
en la figura.
a) Calcule el campo eléctrico producido por la carga de la izquierda para un punto situado sobre
~
el eje x, es decir E(x).
b) Calcule la fuerza que ejerce la carga de la izquierda sobre la carga de la derecha.

y

+Q

+Q
x
L

d

c) Pruebe que si d
L la fuerza entre las barras
equivale a la de dos cargas puntuales de carga
Q. Puede ser útil la aproximación ln(1 + x) ≈
x − x2 si |x|
1.

#### Problema 2.9

X I

Considere un plano infinito el cual tiene un forado
circular de radio a. Sobre el plano existe una densidad
superficial de carga dada por σ(r) = σ0 ar donde r es
la distancia desde el centro del agujero. A distancia
b sobre el eje del forado existe una barra de largo a,
masa M y carga desconocida, la cual reposa inmóvil
en esa posición a pesar de la gravedad. Suponiendo
que la densidad de carga es uniforme, determine la
carga que posee la barra.

a
b
~g

M
a

s (r)

Problemas Propuestos y Resueltos de Electromagnetismo

L

---

### Página 32

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
#### Problema 2.10

X I

La contaminación por compuestos químicos de un lago
de forma circular ha dejado su densidad superficial de
carga que, expresada en coordenadas polares se puede
escribir como
σ(r) = −

z

σ 0 a3
(r2 + a2 )

donde = a” y σ0 son constantes conocidas. Aquí el origen de coordenadas es el centro del lago. Se pide:
a) Determine el campo eléctrico que afectará la vida en el lago. Suponga que los peces sólo viven
en las cercanías del centro del lago (eje z) y a
profundidades mucho menores que la extensión
del lago, por lo cual éste puede considerarse infinito.

s (r)

a

b) Suponga que debido a esta contaminación, un
pez adquiere una carga Q. Determine el trabajo
electrostático que debe efectuar el pez para llegar al centro del lago si se encontraba nadando
a una distancia = a” profundidad sobre el eje z
de la Figura.
Hint:
#

"

Rodrigo Chi - Marzo 2017

r
−(a2 + 2r2 + z 2 )
d
p
=
dr (a − z ) (a + r )(z + r )
((a + r )(z 2 + r2 )) 2

V?

#### Problema 2.11

X I

h

Considere un cono de altura h y radio basal h. La superficie (manto) del cono está cargada uniformemente
con una densidad σ0 . Calcule el potencial en el centro
de la base del cono.

h

---

### Página 33

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
z
s = s (q )

#### Problema 2.12

X I

R
q

Calcular el campo electrostático que genera un casquete esférico de centro O y radio R que porta una
densidad superficial de carga σ = σ0 cos θ (en coordenadas esféricas) en su mismo centro.

#### Problema 2.13

a

X I

Calcule el campo eléctrico creado por un cono macizo
de altura h y semi ángulo α, uniformemente cargado con una densidad volumétrica de carga ρ0 en su
vértice.

h

r0

X I

En una primera aproximación, una montaña puede ser
modelada como un cono de altura h y semi ángulo α
de masa total M distribuida uniformemente. Geofísicos han determinado que la gravedad en su cima tiene
un valor ~g1 = −g1 ẑ la cual está a una distancia h sobre el nivel suelo. Los mismos científicos saben que si
la montaña no existiese el campo gravitacional terrestre en el mismo punto sería ~g0 = −g0 ẑ . Determine
∆~g = ~g1 −~g0 . (Hint: Puede ser útil el Problema 2.13)

a a
h

z

Problemas Propuestos y Resueltos de Electromagnetismo

#### Problema 2.14

x

O

---

### Página 34

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS

#### Problema 2.15

P1

X S

h

Considere un cilindro macizo de radio R y largo L
como se muestra en la Figura. El cilindro posee una
densidad de carga volumétrica ρ0 . Determine
a) El módulo del campo eléctrico en un punto P1
ubicado una distancia h sobre su base superior
y sobre el eje del cilindro.

R
r0

L

h

b) El módulo del campo eléctrico en un punto P2
ubicado una distancia h > R del eje cilindro,
justo a la mitad de la altura del cilindro.

#### Problema 2.16

P2

X I

Un bloque infinito posee una densidad de carga uniforme ρ que ha sido localizado entre x = −a y x = a.
Este bloque es infinito en la dirección y y z (saliendo de página). Dos planos infinitos son localizados en
x = −b y x = b, los cuales poseen una densidad de
carga σ1 y σ2 , respectivamente. Al medir el campo
eléctrico se observa que:
Rodrigo Chi - Marzo 2017

L

x < −b
−b < x < −a
~ =
E

−E
x̂
a
<x<b



x>b




 +E x̂

y

b

s1

a) Calcule la densidad de carga ρ del bloque infinito.
b) Calcule las densidades de carga superficiales σ1
y σ2 de los planos a la izquierda y derecha del
bloque respectivamente.

a

a

r

b

s2

x

---

### Página 35

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS

III.

Soluciones

Solución 2.1

P X

Todos los problemas donde se pida determinar el campo eléctrico se pueden abordar mediante la
definición. Sin embargo, no en todos los problemas siempre será fácil usar esta técnica (ya que
se pueden llegar a integrales bastante complejas). En general en todos los problemas donde se
pida determinar el campo eléctrico en un punto o en un eje (y no en todo el espacio) se pueden
abordar por definición.
Dado que este problema cumple con esa característica, se debe tener claro como parametrizar la superficie para poder usar la definición. Sin embargo, no es claro que haya una fórmula
matemática con que se pueda representar de una sola vez a la unión casquete-disco. La parametrización anterior se ve solucionada usando el principio de superposición; primero se calcula
el campo eléctrico generado por el disco y luego el del casquete semiesférico, para luego sumar
ambos resultados y obtener el campo final en el punto.
Campo generado por el disco.
Usando definición:
~ = 1
E
4πε0

ˆ

~r − ~r 0
· dq
|~r − ~r 0 |3

Ω

- ~r : Es el vector que señala dónde se quiere conocer el campo eléctrico (puede ser un
punto en específico, un eje, un superficie, etc.).
- ~r 0 : Es el vector que señala dónde está lo que genera el campo eléctrico. Este vector
es variable y no representa un punto por sí solo en distribuciones continuas de
carga ya que parametriza una línea/superficie/volumen.
- dq : Es el diferencial de carga, y puede valer dq = λdl = σdS = ρdV , eventualmente
las densidades de carga λ, σ y ρ no necesariamente son constantes y podrían depender
del vector ~r 0 (ie. depende de alguna variable de integración).
- Ω : Es el espacio de integración de la línea/área/volumen de lo que está generando el
campo eléctrico. Establece los límites de todas las integrales.
Luego, aplicado lo anterior al disco de radio a se tiene que (en coordenadas cilíndricas):
a
~r = ẑ
~r 0 = rr̂

Problemas Propuestos y Resueltos de Electromagnetismo

Se debe tener claro que:

---

### Página 36

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
dq = σdS
Donde los límites de integración serán r ∈ [0, a] , θ ∈ [0, 2π] (¡qué es la parametrización
del disco!).
Z

Trozo infinitesimal de disco

a

~r

~r

s

~r

~r 0
Y

X

Figura 2.1: Campo Eléctrico generado por un disco.
Calculando la integral:
~ =
E

4πε0

¨

~r − ~r 0
σdS
|~r − ~r 0 |3

Ω

=

σ
4πε0

ˆ2π ˆa

Rodrigo Chi - Marzo 2017

=

σ
4πε0

σ
=
4πε0

a
ẑ − rr̂

ˆ2π ˆa
0 0
ˆ2π ˆa

a
ẑ − rr̂

3 rdrdθ

a
ẑ − rr̂
3 rdrdθ
a 2
(( 2 ) + r2 ) 2
a
ẑ − r(cos θx̂ + sin θŷ)
rdrdθ
(( a2 )2 + r2 ) 2

~ de modo que
En este caso se separará por cada componente del vector E,
~x = σ
E
4πε0

ˆ2π ˆa

σ
=−
4πε0

−r cos θ
(( a2 )2 + r2 ) 2

ˆ2π

ˆa
cos θdθ ·

|

r2

{z

=0

rdrdθ

(( a2 )2 + r2 ) 2

dr

}

Dado que la integral del coseno en un período es nula, se tiene que el campo eléctrico no
~y ,
tiene componente según x. Análogamente, sucede lo mismo al momento de calcular E

---

### Página 37

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
por lo que tampoco existe una coordenada según y. Luego
ˆ2π ˆa
a
ẑ
σ
~
E=
3 rdrdθ
a
4πε0
(( 2 ) + r2 ) 2

σaẑ
=
8πε0

ˆ2π

ˆa

=

σaẑ
·
4ε0

Nótese que

(( a2 )2 + r2 ) 2

ˆa

r
(( a2 )2 + r2 ) 2



r

dθ ·

dr

dr



d 
r
=
−q a
3 por lo tanto
a
dr
(( 2 )2 + r2 ) 2
( )2 + r 2

~ = σaẑ · − q 1
E
4ε0
( a )2 + r2

r=a

r=0





σaẑ 
=
· −q a
+ a
4ε0
( )2 + a2

!

σ
=
1 − √ ẑ
2ε0
Campo generado por el semicasquete

dq = σdS = σa2 sin θdθdϕ
Donde los límites de integración serán ϕ ∈ [0, 2π] , θ ∈ [0, π2 ].
¨
~r − ~r 0
~ =
E
σdS
4πε0
|~r − ~r 0 |3
Ω
π

=

σ
4πε0

ˆ2π ˆ2

a
ẑ − rr̂
a
ẑ − ar̂

3a

sin θdθdϕ

π

=

σ
4πε0

ˆ2π ˆ2

a
ẑ − a(sin θ cos ϕx̂ + sin θ sin ϕŷ + cos θẑ)
a
ẑ − a(sin θ cos ϕx̂ + sin θ sin ϕŷ + cos θẑ)

3a

sin θdθdϕ

π

σ
=
4πε0

ˆ2π ˆ2

a
ẑ − a(sin θ cos ϕx̂ + sin θ sin ϕŷ + cos θẑ) 2
a sin θdθdϕ
(a2 sin2 θ + ( a2 − a cos θ)2 ) 2

Problemas Propuestos y Resueltos de Electromagnetismo

Al igual que el caso anterior debe procederse a calcular los vectores ~r, ~r 0 y dq, en este caso
se tiene que (en coordenadas esféricas):
a
~r = ẑ
~r = ar̂

---

### Página 38

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
En este caso vuelve a ocurrir lo mismo que pasó cuando se calculó el campo que genera un
disco, ya que se anulan las componentes en x e y debido a que aparecen un cos ϕ y sin ϕ
integrados en un período.
En general, uno también puede argumentar por simetría que algunas componentes del campo eléctrico son nulas, no siempre es necesario el cálculo (siempre se llegará a funciones
sinuosoidales integradas en un período).
Por lo tanto el valor del campo generado por el semicasquete es:
π

~ = σẑ
E
4πε0

ˆ2π ˆ2

σa2 ẑ
=
4πε0

a
− a cos θ
3 a sin θdθdϕ
a
(a sin θ + ( 2 − a cos θ) )
π

ˆ2π

ˆ2
dϕ

( a2 − a cos θ) sin θ

(a2 sin2 θ + ( a2 − a cos θ)2 ) 2

dθ

a − a2 cos θ
σa2 ẑ
=
· 2π · a q a
4πε0
( )2 ( )2 − 2 · a · a · cos θ + a2



θ= π2

θ=0



a
a
2σẑ 
=
· q a
− q 2a 
ε0
( 2 )2 + a2
( 2 )2

2σ
=
ε0

!

√ − 1 ẑ

Dado los resultados anteriores, se procede a sumarlos para encontrar el campo final en el punto
!

~ total = σ 1 − √1 ẑ + 2σ
E
2ε0
ε0

Rodrigo Chi - Marzo 2017

Solución 2.2

!

σ
√ − 1 ẑ =
2ε0

!

√ − 3 ẑ

P X

Para encontrar el ángulo de equilibrio, se debe considerar que la suma de fuerzas que actúan
sobre la masa m deben anularse, por consiguiente se hace un DCL para deducir las ecuaciones de
movimiento. Con lo anterior las ecuaciones de movimiento son:
mẍ = Fe − T sin θ = 0
mg
cos θ
~ se calculará el campo E
~ a una distancia d = l sin θ producido por la barra infinita
Como F~e = q E,
de densidad de carga lineal λ. Considerando que
ˆ
~r − ~r 0
~
E=
dq
4πε0
|~r − ~r 0 |3
mÿ = T cos θ − mg = 0 ⇒ T =

l

---

### Página 39

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
l
~g
q

l

~T

~Fe
m~g

Figura 2.2: DCL para masa m.
Donde ~r = dx̂ = l sin θx̂ correspondiente a la posición donde se quiere calcular el campo, ~r 0 = z ẑ
correspondiente a quien genera el campo, y dq = λdz dónde z ∈ (−∞, +∞). Además se considera
que por la simetría del problema, el campo será el mismo independiente de la posición en ẑ de la
~ sólo tiene componente en x̂. Con lo anterior la ecuación anterior queda:
masa, por lo que E
~ = 1
E
4πε0

ˆ∞

l sin θx̂

((l sin θ)2 + z 2 ) 2

−∞

λl sin θ
x̂
=
4πε0

ˆ∞

λdz

dz

−∞

((l sin θ)2 + z 2 ) 2

Se hace el cambio de variable z = (l sin θ) tan φ, lo cual implica que dz = (l sin θ) sec2 φdφ, y los
límites de integración cambian de z ∈ (−∞, +∞) ⇒ φ ∈ (− π2 , + π2 ). Luego:
~ = λl sin θ x̂
E
4πε0

− π2
π

λl sin θ
x̂
=
4πε0

(l sin θ) sec2 φdφ
((l sin θ)2 + (l sin θ)2 tan2 φ) 2

ˆ

− π2

(l sin θ) sec2 φdφ

(l sin θ)3 (1 + tan2 φ) 2
π

=

λ
x̂
4πε0 (l sin θ)

ˆ2

− π2

sec2 φdφ
sec3 φ

π

=

λ
x̂
4πε0 (l sin θ)

ˆ2

cos φdφ

− π2

π
λ
x̂ sin φ|−2 π
4πε0 (l sin θ)
λ
=
x̂
2πε0 (l sin θ)

=

Problemas Propuestos y Resueltos de Electromagnetismo

π

ˆ2

---

### Página 40

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
λ
x̂. Dicho valor en las ecuaciones de
2πε0 (l sin θ)

Como ya se conoce el campo, luego F~e = q
movimiento y despejando T , se llega a:
mẍ = Fe − T sin θ = q

λ
mg
sin2 θ
qλ
−
sin θ = 0 =⇒
=
= qK
2πε0 (l sin θ) cos θ
cos θ
2πε0 lmg

Se usa la identidad trigonométrica sin2 θ = 1 − cos2 θ:

1 − cos θ
= qK =⇒ cos2 θ + qK cos θ − 1 = 0 =⇒ cos θ =
cos θ

−qK ±

q

(qK )2 + 4

Como se espera que θ ∈ (0, π/2) (el péndulo no dará la vuelta completa),
cos θ > 0, luego se
q
escoge la solución positiva. Finalmente si q −→ ∞, se cumple que (qK) + 4 ≈ qK, entonces
cos θ =

−qK + qK
=0

El resultado anterior implica que θ = π2 , esto es esperable ya que al ser una carga positiva se
alejará lo más posible de quién genere el campo y eso de logra a la mayor distancia, es decir, con
el ángulo encontrado.
P X

Solución 2.3

La fuerza sobre la carga q es F~q = F~e + F~r donde Fe corresponde a la fuerza que el anillo ejerce
sobre q, y Fr , la fuerza que ejerce el resorte.
La fuerza que ejerce el campo eléctrico que genera el anillo sobre la carga q está dada por

Rodrigo Chi - Marzo 2017

~A
F~e = q E
Entonces el campo eléctrico que genera el anillo en su eje es:
ˆ
~r − ~r 0
~
dq
EA =
4πε0
|~r − r~0 |3
Donde ~r = z ẑ, ~r 0 = R0 r̂ (en coordenadas cilíndricas) y dq = λR0 dθ con θ ∈ (0, 2π). Además,
dado que la carga total en e anillo es Q y se distribuye homogéneamente, λ se puede calcular
como:
Q
Q
λ=
=
L
2πR0
con lo anterior:
~A =
E

4πε0

ˆ2π

ˆ2π

ˆ2π



z ẑ − R0 r̂
(z 2 + R02 ) 2

λR0 dθ =

1 

4πε0

z ẑ
(z 2 + R02 ) 2

λR0 dθ −



R0 r̂
(z 2 + R02 ) 2

λR0 dθ


---

### Página 41

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
Nótese que por la simetría del anillo la segunda integral se anulará. También se puede justificar
notando que r̂ = sin θx̂ + cos θŷ, y como la integral de sin θ y cos θ se anulan en un intervalo
entre (0, 2π), el segundo sumando se anula. Luego:
~A =
E

ˆ2π

λR0 z ẑ
4πε0 (z 2 + R02 )

dθ =

λR0 z ẑ

2ε0 (z 2 + R02 ) 2

Finalmente, sustituyendo λ, se concluye el valor de F~e :
R0 z ẑ
qQz ẑ
Q
~
F~e = q E~A = q
3 =⇒ Fe =
2πR0 2ε0 (z 2 + R0 ) 2
4πε0 (z 2 + R02 ) 2
Nótese que como q < 0 esta fuerza apunta en en la dirección −ẑ.
Por otro lado, la fuerza elástica para una distancia z (notar que el resorte se mueve sólo en el
eje), es la que genera el resorte de constante k0 , la cual está dada por
F~r = −k0 z ẑ
Dado los cálculos anteriores, la fuerza total sobre q es:
F~q =

!

qQ

4πε0 (z 2 + R02 ) 2

− k0 z ẑ

Por otra parte, la fuerza en el eje ẑ esta dada por:
F~q = mz̈ ẑ

!

mz̈ =

!

qQ
qQ
−
− k0 z =⇒ z̈ +
+ k0 z = 0
4πε0 R0
m
4πε0 R03

y como la ecuación de la frecuencia en pequeñas oscilaciones cumple z̈ + ω 2 z = 0
v
u
u1
ω=t

qQ
−
+ k0
m
4πε0 R03

Solución 2.4

!

P X

a) Es necesario calcular el potencial generado por la semicircunferencia y el creado por la carga
puntual. Para el caso de la semicircunferencia se puede calcular usando la expresión
ˆ
dq
V (~r) =
4πε0
|~r − ~r 0 |

Problemas Propuestos y Resueltos de Electromagnetismo

Si se desea encontrar la frecuencia para pequeñas oscilaciones, se considera que para z
1 se
tiene que z 2 ≈ 0. Finalmente

---

### Página 42

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
en este caso ~r = 0 y ~r 0 = Rr̂ con θ ∈ [0, π] y dq = λdl = λRdθ. Luego
λ
Valambre (0) =
4πε0

ˆπ

Rdθ
λ
=
| − Rr̂|
4ε0

Adicionalmente es sabido que el potencial que genera una carga puntual esta dado por
Vcarga (0) =

q
4πε0 R

Por lo tanto el potencial pedido es la superposición de los resultados anteriores
V (C) =

λ
q
+
4πε0 R 4ε0

b) Por simetría las componentes en horizontales se anulan en el punto C, por ende en ese
punto sólo existe la superposición de de componentes verticales. El campo generado por el
alambre vale
ˆ
(~r − ~r 0 )
dq
E(~r) =
4πε0
|~r − ~r 0 |3
nuevamente se tiene que ~r = 0 y ~r 0 = Rr̂ con θ ∈ [0, π] y dq = λdl = λRdθ, por lo que
~ alambre (0) = λ
E
4πε0

ˆπ

(0 − Rr̂)Rdθ
λ
=−
| − Rr̂|
4πε0 R

ˆπ
[cos θx̂ + sin θŷ] dθ = −

λ
ŷ
2πε0 R

al igual que la parte anterior el campo eléctrico generado por la carga está dado por
~ carga (0) =
E

q
ŷ
4πε0 R2

Finalmente, el campo total es
Rodrigo Chi - Marzo 2017

!

~
E(C)
=

q
λ
−
ŷ
4πε0 R2 2πε0 R

~
c) Imponiendo E(C)
= 0, se tiene que
q
λ
=
=⇒ q = 2Rλ
4πε0 R
2πε0 R

Solución 2.5

P X

a) Inicialmente determinaremos el potencial que genera un anillo por si sólo y luego se usará
~ = −∇V para determinar el campo eléctrico. De este modo el potencial de
el hecho que E

---

### Página 43

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
un sólo anillo de radio a y densidad homogénea λ y con su centro en el origen provoca un
potencial dado por:
ˆ
dq
V (~r) =
4πε0
|~r − ~r 0 |
donde ~r = z ẑ, ~r 0 = ar̂ y dq = λadθ con θ ∈ [0, 2π]. Por ende
V (z) =
4πε0

ˆ2π

λadθ
λa
√
√
=
z 2 + a2
2ε0 z 2 + a2

Extrapolando este resultado al problema se tiene que los anillos están a distancia L, de
modo que suponiendo que el origen está en el punto de medio de su separación, el potencial
en el eje es
λa
λa
r
r
−
V (z) =
2
2
2ε0 z − L2 + a2 2ε0 z + L2 + a2




=

λa 
r
2ε0  

z − L2

2

+ a2

− r

z + L2

2

+ a2





Dado que
~ = −∇V = − ∂V ẑ
E
∂z
Por lo que finalmente

~ = λa 

E
2ε0  



z − L2



z − L2

2

+ a2

 3 − 

z + L2
z + L2

2

+ a2



ẑ
3 
2 

b) Considerando lo obtenido en a)
!

L
λa
V (O ) = V z =
=
2ε0

−√ 2
a
L + a2

L
λa
V (O) = V z = −
=
2ε0

√
−
a
L +a









Por lo que la diferencia vale:
λa
V (O) − V (O ) =
− +√ 2
ε0
a
L + a2

!

!

Problemas Propuestos y Resueltos de Electromagnetismo



---

### Página 44

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
Solución 2.6

P X

a) Recordando, que el campo eléctrico producido por una distribución de carga dq(~r 0 ) vale:
ˆ
~r − ~r 0
~
E(~r) =
dq(~r 0 )
4πε0
|~r − ~r 0 |3
Luego se tiene que: ~r = aŷ; ~r 0 = xx̂; dq = λdx, por lo tanto:


~
E(aŷ)
=

λ 
ŷ
4πε0

ˆ∞

ˆ∞

adx
(a2 + x2 )

− x̂



xdx

(a2 + x2 ) 2




Realizando el cambio de variable:
x = a tan θ =⇒ dx = a sec2 θdθ
Resulta:

π



~
E(aŷ)
=

λ 
 ŷ
4πε0 

ˆ2

π

a sec θdθ
− x̂
a3 sec3 θ



π



a tan θ sec θdθ 


a3 sec3 θ

π



~
E(aŷ)
=

ˆ2

λ 
ŷ
4πε0 a 

ˆ2

ˆ2



cos θdθ − x̂

sin θdθ


Obteniendo, finalmente que:
~
E(aŷ)
=

λ
(ŷ − x̂)
4πε0 a

b) Nuevamente usando la definición se tiene que ~r = −ax̂; ~r 0 = xx̂; dq = λdx
Rodrigo Chi - Marzo 2017



~
E(−ax̂)
=

λ 
x̂
4πε0

ˆ∞



−a − x

dx
| − a − x|3

Manejando algebraicamente la expresión se obtiene que
λ
~
E(−ax̂)
=−
4πε0

ˆ∞

dx
λ
1 ∞
λ
=
−
x̂
·
−
=−
x̂
(x + a)
4πε0
x+a 0
4πε0 a

Solución 2.7

P X

Separando el problema en dos partes:

---

### Página 45

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
i) Campo producido por las rectas semi-infinitas: Sean (x̂0 ; ŷ 0 ) el sistema de referencia para
la recta superior en la figura, y (x̂00 ; ŷ 00 ) para la recta inferior, orientados de manera que
coincidan con el sistema de referencia de la parte a) entonces:
~1 =
E

λ
(−x̂0 + ŷ 0 )
4πε0 R

λ
(−x̂00 + ŷ 00 )
4πε0 R

~2 =
E

Ahora descomponiendo en los ejes x̂ e ŷ (x̂ horizontal hacia la derecha, ŷ vertical hacia
arriba):
π
π
x̂0 = cos x̂ + sin ŷ
3π
3π
ŷ 0 = cos x̂ − sin ŷ
π
π
x̂00 = cos x̂ − sin ŷ
3π
3π
ŷ 00 = cos x̂ + sin ŷ
3π
π
Como cos 8 = sin 8 , y superponiendo los campos, entonces:
~ 1 +E
~2 =
E

π
3π
λ
x̂ − cos + cos
2πε0 R




π
π
λ
x̂ − cos + sin
=
2πε0 R




√

3π
λ
x̂
2 cos
=−
2πε0 R

Otra forma mucho más rápida de resolver esta parte es la siguiente:
√
2λ
~ 1 | = |E
~ 2| =
|E
4πε0 R
Entonces, debido a la simetría con respecto al eje x, las componentes en ŷ de los campos
producidos por las dos rectas se anulan, y se obtiene que:

ii) Campo producido por el sector circular: Calculando por definición, de manera similar a la
parte anterior:
ˆ
~r − ~r 0
~ 3 (~r) =
dq(~r 0 )
E
4πε0
|~r − ~r 0 |3
Con: ~r = 0 ; ~r 0 = Rr̂ ; dq = λRdθ. Entonces:
11π

~ 3 (0) = −
E

λ
4πε0 R

ˆ8

r̂dθ
5π

Descomponiendo r̂ en los ejes cartesianos, y por la paridad e imparidad del coseno y seno,
la integral en ŷ se anula (también se puede comprobar esto último debido a la simetría con
respecto a x̂) resulta:
11π

~ 3 (0) = − λ
E
4πε0 R

ˆ8

λx̂
x̂ cos θdθ =
2πε0 R

5π

ˆ 3π

cos θdθ

Problemas Propuestos y Resueltos de Electromagnetismo

~1 + E
~ 2 = −2|E
~ 1 | cos 3π = − √ λx̂ cos 3π
E
2πε0 R

---

### Página 46

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
Luego:
~ 3 (0) =
E

λx̂
3π
λx̂
π
λx̂
5π
11π
sin
=
cos =
sin
− sin
2πε0 R
2πε0 R
4πε0 R




Finalmente, sumando todos los campos, se obtiene que el campo eléctrico total en el punto P
vale:
!


3π cos 3π
λx̂
λx̂
π √
π
~
sin
− √
ET =
=
cos − 2 sin
πε0 R 2
2πε0 R

Solución 2.8

P X

a) Primero debe usarse el campo eléctrico por definición para hallar una expresión
E(~r) =
4πε0

ˆ

(~r − ~r 0 )dq
|~r − ~r 0 |3

.
En la fórmula anterior ~r = xx̂, ~r 0 = x0 x̂ y dq = λdx0 con x0 ∈ [0, L] donde λ = Q
L
Analizando por intervalos
- x>L
λx̂
~
E(x)
=
4πε0

ˆL

x − x0
dx0
(x − x0 )3

Rodrigo Chi - Marzo 2017

λx̂
1 L
·
4πε0 x − x0 0


λ
−
x̂
=
4πε0 x − L x
=

- x<0

Análogo a lo anterior:
~ =− λ
E
4πε0

- 0≤x≤L



x̂
−
x−L x


En este caso el campo eléctrico es infinito ya se cae en un punto de carga infinita.
Esto puede verse en la integral, ya que si x = x0 diverge.

---

### Página 47

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
~
~
b) En este caso un diferencial de fuerza está dado por dF~ = E(x)dq
= E(x)λdx
, por lo tanto
λ2 x̂
F~ =
4πε0

2L+d
ˆ 

−
dx
x−L x


L+d

"

!

λ x̂
L+d
2L + d
=
ln
− ln
4πε0
d
L+d
!
λ2
(L + d)2
=
ln
x̂
4πε0
d(2L + d)

!#

c) Para la última parte debe notarse lo siguiente
(L + d)2
ln
d(2L + d)

!

L2 + 2Ld + d2
= ln
2Ld + d2

!

L2
= ln 1 +
2Ld + d2

!

L2
≈ ln 1 + 2
d

!

≈

L2
d2

De lo anterior se termina deduciendo que
F~ ≈

1 (λL)2
1 Q2
x̂
=
x̂
4πε0 d2
4πε0 d2

Que coincide con la fuerza que sienten dos cargas puntuales de carga Q = λL.

Solución 2.15

P X

!

~ = σ 1− √ z
ẑ
E
2ε0
z 2 + R2
Ahora, usando este resultado se considerará z = 0 en el punto P1 creciendo hacia arriba. A
partir de esto, el cilindro está compuesto por la superposición infinitesimal de discos (uno
~ que provoca uno de estos discos de
encima del otro). El aporte de campo eléctrico dE
ancho infinitesimal es
!
ρ0 · dz
z
~
dE =
1− √ 2
ẑ
2ε0
z + R2
Por lo que el campo total en el punto está dado por
~ 1 ) = ρ0 ẑ
E(P
2ε0

ˆ−h



q
√
z
ρ0
1− √ 2
dz =
L − ( h + R − (L + h) + R ) ẑ
2ε0
z + R2
!

−(L+h)

Problemas Propuestos y Resueltos de Electromagnetismo

a) En este caso, se usará el resultado conocido del campo eléctrico que genera un disco de
radio R y densidad de carga σ, el cual corresponde a

---

### Página 48

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS

L

l0

L

h
P2

Figura 2.3: Situación análoga al cilindro.
b) Para resolver este problema, se usará una técnica de analogías. Este problema es un poco
difícil planteando las integrales correspondientes, pero se puede usar otro resultado conocido
como el que genera una barra de densidad lineal λ0 de largo L sobre un punto ubicado un
eje perpendicular a ella justo en su mitad.
En este caso, tomando el eje z coincidente con eje de la barra y el origen su punto medio,
se obtiene ~r = hr̂, ~r 0 = z ẑ con z ∈ [− L2 , L2 ] y dq = λ0 dz. Entonces
L

~ 2) =
E(P

4πε0

ˆ2
−L

hr̂ − z ẑ
(h2 + z 2 )

λ0 dz =

λL
√0
r̂
2πε0 h 4h2 + L2

Ahora, volviendo al problema, si V es el volumen de un cilindro es posible afirmar que

Rodrigo Chi - Marzo 2017

λ0 =

dq dV
dq
dV
d
=
= ρ0
= ρ0 (πR2 z) = ρ0 πR2
dz
dV dz
dz
dz

El valor obtenido es equivalente a la carga por unidad de largo que tiene el cilindro del problema.
Finalmente el campo es
ρ0 R2 L
~ 2) =
√
E(P
r̂
2ε0 h 4h2 + L2

---

### Página 49

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS

IV.

Indicaciones Problemas Sin Solución

Indicación 2.9

P X

Determine el campo eléctrico en todo el eje donde se encuentra la barra. Para ello ~r = rr̂
en coordenadas cilíndricas donde r ∈ [a, ∞).
~
Un diferencial de fuerza sobre la barra puede ser determinado como dF~ = E(z)dq
=
~
E(z)λdz. Integre el diferencial anterior en toda la barra y determine la fuerza que ejerce el
plano sobre ella.
Determinada la fuerza eléctrica esta debe ser igual al peso. Despeje de ahí el valor de λ y
luego Q.

Indicación 2.10

P X

Usando la definición integre la densidad de carga sobre el plano, en este caso ~r 0 = rr̂ con
r ∈ [0, ∞]. Noté que σ tiene una dependencia radial por lo cual quedará una integral más
complicada de resolver.

Indicación 2.11

Este problema puede ser planteado tanto en coordenadas esféricas como cilíndricas.

De usar coordenadas cilíndricas, puede ser útil la siguiente igualdad (h−z)2 +z 2 = (2z−h)2 +h
y el cambio de variables 2z − h = h tan θ.

Indicación 2.12

P X

Use la definición de campo eléctrico para el campo eléctrico en el centro de la esfera. En
este caso dq = σ0 cos θdS = σ0 R2 cos θ sin θdθdϕ en coordenadas esféricas.

Indicación 2.13

P X

Este problema puede ser planteado tanto en coordenadas esféricas como cilíndricas.

Problemas Propuestos y Resueltos de Electromagnetismo

P X

---

### Página 50

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
De usar coordenadas cilíndricas, recuerde que para un punto r̂ 0 = rr̂ + z ẑ y que r(z) =
z tan α.

Indicación 2.14

P X

Note la analogía entre la Ley de Coulomb y la Ley de Gravitación Universal.
|FE | =

1 q1 q2
4πε0 r2

|FG | = G

m1 m2
r2

Tal como existe el campo eléctrico creado por un continuo de carga, también es posible
determinar el campo gravitacional de un continuo de masa en forma muy parecida.
Con ayuda del resultado obtenido en el Problema 2.13 concluya el problema.

Indicación 2.16

P X

El problema debe ser abordado por definición de los campos provocados por los planos
infinitos de densidad σ1 y σ2 y el bloque de densidad ρ.
Por integración directa determine el campo eléctrico que genera un plano infinito.
El campo eléctrico que genera el bloque para puntos fuera de él puede ser determinado
mediante la integración del resultado del plano infinito. Recuerde que el bloque es una
superposición de planos uno al lado del otro.

Rodrigo Chi - Marzo 2017

Determine los campos eléctricos en todas las zonas en el intervalo |x| > a en función de
σ1 , σ2 y ρ. Concluya el problema igualando con los campos eléctricos entregados en el
enunciado.

---

### Página 51

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS

V.

Respuestas
Problema

Respuestas

P

2.1

~ total = σ
E
2ε0

P

2.2

cos θeq =

s

P

P

2.3

ω=

m

a) V (C) =
2.4





√7 − 3

−qK +


k+

ẑ

p

(qK )2 + 4
con K = 2πε0λlmg , θ(q → ∞) = π2

qQ
4πε0 R3



q
λ
+
4πε0 R 4ε0

b)

~
E(C)
=



λ
q
−
4πε0 R2
2πε0 R


ŷ

c) q = 2Rλ

~ =
a) E

λa 

2ε0 


z − L2

L 2

 23 − 

z + L2

L 2

2.5

+ a2
z+ 2


λa 1
−√
b) V (O) − V (O ) =
ε0 a
L2 + a2

P

2.6

~
a) E(A)
=

P

2.7

~ =
E

z− 2

+ a2

λ
λ
~
(ŷ − x̂) b) E(B)
=
x̂
4πε0 a
4πε0 a

λx̂ 
π √
π
cos − 2 sin
2πε0 R

Problemas Propuestos y Resueltos de Electromagnetismo

P


 32  ẑ

---

### Página 52

CAPÍTULO 2. DISTRIBUCIONES CONTINUAS DE CARGAS
Problema




λ

x>L
− x1 x̂

 4πε0 x−L


~
λ
a) E(x)
=
− 4πε0 x−L − x x̂ x < 0



∞
0≤x≤L


(L+d)
λ2
ln d(2L+d)
x̂
b) F~ = 4πε




(L+d)2
1 Q
c) ln d(2L+d)
≈ ln 1 + Ld2 ≈ Ld2 entonces F~ ≈ 4πε
2 x̂
0 d

P

2.8

P

2.9

P

2.10

P

2.11

V =

P

2.12

σ
~
E(0)
=−
ẑ
3ε0

P

2.13

~ = ρh (1 − cos α)ẑ
E
2ε0

P

2.14

6GM cos2 α
∆~g = − 3
ẑ
h (1 + cos α)

P

Rodrigo Chi - Marzo 2017

Respuestas

q=
σ0 a ln

g
 2ε0 M
√
a+

√

a+

~
a) E(z)
=−

a2 +b2



a2 +(a+b)2

σa2 (a − z)
2ε0 (a + z)

b)

W =−

√
σh
ln (1 + 2)
2ε0

h
i
p
√
~ 1 )| = ρ0 L − ( h2 + R2 − (L + h)2 + R2 )
a) |E(P
2ε0
2.15

ρ√
0R L
~ 2 )| =
b) |E(P
2ε h 4h2 +L2

P

3Qσ0 a
4ε0

2.16

a) ρ = − ε0aE0
b) σ1 = σ2 = ε0 E0

---

### Página 53

Ley de Gauss

I.

Resumen Teórico

Ley de Gauss (Forma Integral)
La ley de Gauss en su forma integral enuncia que
¨

~ = qenc
~ · dS
E
ε0

(3.1)

Ω

Para cualquier superficie cerrada Ω. En otras palabras, para cualquier superficie cerrada el flujo
de campo eléctrico a través de ella será igual a la carga encerrado divida por la permitividad del
vacío.

Por otro lado, también existe la Ley de Gauss en su forma diferencial la cual enuncia que
~ ·E
~ = ρ
∇
ε0

(3.2)

~ yV
Continuidad del E
El campo eléctrico no es necesariamente continuo. Las discontinuidades del campo son
provocadas generalmente por cargas puntuales o superficies cargadas.
El potencial eléctrico es siempre continuo, ya que es la integral del campo eléctrico (la
integral es siempre una función continua).

Problemas Propuestos y Resueltos de Electromagnetismo

Ley de Gauss (Forma Diferencial)

---

### Página 54

CAPÍTULO 3. LEY DE GAUSS

Recomendaciones
La ley de Gauss es sumamente poderosa, usualmente se usa sólo para determinar campo
eléctrico pero sus extensiones son mucho mayores. Los problemas en los cuales se determina
campo eléctrico mediante ley de Gauss son más bien acotados, y responden a las simetrías
esféricas, cilíndricas y planas.
Nótese que deben existir las simetrías necesarias para aplicar ley de Gauss directamente en
la determinación de campo eléctrico. Casos típicos:
- Carga puntual q.

- Alambre infinito de densidad λ constante.

- Cilindro macizo de densidad constante o ρ(r) (r distancia desde el eje del cilindro).
- Casquete cilíndrico de densidad σ constante.

- Esfera maciza de densidad constante o ρ(r) (r distancia del centro de la esfera).
- Casquete esférico de densidad σ constante.

- Plano infinito de densidad σ constante.

Rodrigo Chi - Marzo 2017

- Bloque infinito en el plano xy y de espesor conocido en z con densidad de carga ρ(z).

---

### Página 55

CAPÍTULO 3. LEY DE GAUSS

II.

Problemas Propuestos

#### Problema 3.1

X S

Una distribución de carga esférica ρ se extiende desde
r = 0 a r = R, con
ρ = ρ0

r2
1− 2
R

!

R

Calcular:
a) La carga total Q.
b) El campo eléctrico en todo el espacio.
c) El potencial eléctrico en todo el espacio.

#### Problema 3.2

X I

#### Problema 3.3

R1

R2
R3
R4

R4,ρ4

R1,ρ1=0
R2,ρ2
R3,ρ3=0

X I

Se tiene una placa infinita no conductora de espesor
despreciable la cual posee una densidad superficial de
carga −σ, y continua a ella, un bloque infinito de
espesor D con una densidad de carga uniforme +ρ.
Todas las cargas están fijas. Calcule la dirección y la
magnitud del campo eléctrico:
a) a una distancia h encima de la placa cargada
negativamente.
b) dentro del bloque a una distancia d debajo de
la placa cargada negativamente (d < D).
c) a una distancia H bajo fondo del bloque.

s

+r

D

Problemas Propuestos y Resueltos de Electromagnetismo

Considere un cable coaxial infinito y rectilíneo, el cual
está compuesto por un cilindro central y diferentes
casquetes cilíndricos, de radios R1 , R2 , R3 y R4 respectivamente, como se ilustra en la figura. Cada material tiene respectivamente una densidad de carga volumétrica ρ1 , ρ2 , ρ3 y ρ4 (Ver Figura). En el caso que
el cilindro y segundo casquete cilíndrico (de radio R3 )
tienen densidad de carga cero (ρ1 = ρ3 = 0). Encuentre el campo eléctrico en todo el espacio.

---

### Página 56

CAPÍTULO 3. LEY DE GAUSS
X I

#### Problema 3.4

Considere la siguiente distribución de volumétrica de
carga en coordenadas esféricas
(

ρ(r) =

r

−nρ 0 < r < a
ρ
a≤r≤b

a

nr

b

Donde ρ es una constante y n es un entero no negativo. Encuentre el campo eléctrico en todo el espacio.

#### Problema 3.5

X I

Rodrigo Chi - Marzo 2017

Considere el sistema de la figura compuesta por dos
placas paralelas cargadas con densidad +σ y −σ. Las
placas son cuadradas de lado d y separación 2h donde d
2h. En el plano intermedio de las placas se
disparan protones y electrones de carga −e y e, respectivamente con velocidad vx paralela a los planos.
Ignorado efectos de borde y considerando la atracción
gravitacional, determine la relación que debe haber
entre la carga/masa de los protones y electrones para
que éstos logren escapar.

#### Problema 3.6

s

vx x̂

+s
d

z

X S

Considere una carga q en el origen de un sistema de
coordenadas cartesianas. En el mismo sistema de referencia existe un rectángulo paralelo al plano xz de
ancho 2a y altura 2z0 ubicado en y = a (ver Figura).
a) Usando la ley de Gauss en forma adecuada, determine el flujo sobre el rectángulo si z0 = a.
b) ¿Cuántas veces aumenta el flujo de la parte anterior en el caso z0 → ∞?

z0

a

q
a

a

x

z0

y

---

### Página 57

CAPÍTULO 3. LEY DE GAUSS

#### Problema 3.7

X I

a

O0

Considere una esfera maciza de densidad de carga ρ0 y
radio R la cual posee una perforación esférica de radio
a < R2 a una distancia de d entre sus centros. Demuestre que el campo eléctrico es constante en cualquier
punto dentro de la cavidad y determine su valor.

#### Problema 3.8

X S

R

(a)

Considere dos cilindros infinitos de radios R0 los cuales
poseen sus ejes paralelos al eje z (entran y salen de la
hoja de papel). Las densidades de carga volumétricas
de los cilindros son ρ y −ρ y sus ejes centrales pasan
por los puntos (x0 , 0) y (−x0 , 0), respectivamente.
Considerando que x0 < R0 .
a) Determine el campo eléctrico en la zona de intersección.

#### Problema 3.9

y

+r
R0

x0

y

s (q )

(b)
q

x

Cilindro Equivalente (x0 ⌧ R0 )

X I

Dentro de una esfera de radio a centrada en el origen
hay un campo eléctrico
~ ≤ a) = E0
E(r

 2

r
a

r̂

Para r > a hay vacío. Se pide determinar
a) La distribución de carga ρ(r) para r ≤ a.
~ y el potencial eléctrico para r > a
b) El campo E
c) El potencial eléctrico V (r < a).

x

x0

r(r)?

a

Problemas Propuestos y Resueltos de Electromagnetismo

b) Si x0
R0 , ambos cilindros quedan infinitesimalmente cerca, creando un único cilindro equivalente de radio R0 con una densidad de superficial de carga σ(θ). Encuentre el valor de esa
densidad.

r

d~

O

---

### Página 58

CAPÍTULO 3. LEY DE GAUSS

#### Problema 3.10

z

X S

Un cilindro infinito de radio R tiene su eje coincidente
con el eje z. El cilindro posee una densidad volumétrica ρ(r) = ar donde a es una constante positiva y r es
la distancia desde el eje del cilindro.
a) Calcule la carga contenida en un cilindro centrado en el eje z, de radio r y altura h para los
casos r < R y r > R.

r(r) =

r
a

~
b) Determinar el campo eléctrico E(r)
en todo el
espacio.
c) Calcular el potencial eléctrico V (r) en todo el
espacio. Tome como referencia V (r = 0) = 0.
~
d) Grafique |E(r)|
y V (r) en función de r.
#### Problema 3.11

R

X I

l0

Considere un cable infinito cargado con una densidad
lineal de carga λ0 rodeada por un casquete cilíndrico
infinito de radio R de densidad superficial homogénea
σ0 . Si la densidad lineal coincide con el eje del cilindro,
determine:
a) El campo eléctrico en todo el espacio, ¿es continuo el campo eléctrico?.

s0

Rodrigo Chi - Marzo 2017

b) El potencial eléctrico en todo el espacio, ¿es
continuo el potencial eléctrico?. (Use como referencia V (r = R) = 0)
c) Si el alambre se desplazara una distancia δ del
eje del cilindro, ¿cómo determinaría el nuevo
valor del campo eléctrico?.
#### Problema 3.12

R

X I

Use el teorema de Gauss para encontrar el campo
eléctrico debido a una distribución de carga
ρ = ρ0 e−k|z|
con ρ0 y k constantes positivas. Muestre que el campo
~ = E(z)ẑ, con E(−z) = −E(z)
es de la forma E
para z > 0 y encuentre el campo eléctrico en todo el
espacio.

z

r(z)

---

### Página 59

CAPÍTULO 3. LEY DE GAUSS
l

#### Problema 3.13

X S

Se tiene una fuente cargada que consiste en una recta
infinita cargada, con densidad uniforme λ y un plano
infinito cargado con densidad de carga uniforme σ. La
recta forma un ángulo agudo 2α con el plano. Considere un punto P está a una altura h sobre el plano.
Determine

a
a

s

P

Q

h

(a) Vista Isométrica

a) El campo eléctrico total en un punto P sobre
la recta que bisecta al ángulo entre la recta y el
plano.
b) El trabajo necesario para mover una carga puntual q0 desde el punto P hasta el punto Q el cual
está ubicado a una distancia h2 sobre el plano.

Q
a

a

P

h

s
h

(b) Vista Frontal

X S

Un electrón de carga −e < 0 y masa m e inicialmente
en reposo, se encuentra en el centro de un cilindro macizo infinito de radio a y densidad de carga uniforme
ρ0 > 0.
a) Determine el campo y potencial eléctrico que
genera solamente el cilindro macizo en todo el
espacio. Utilice como referencia V (r = 0) = 0.
b) Encuentre el valor U0 correspondiente a la
energía del electrón cuando se encuentra justo
en el borde del cilindro r = a.
c) Calcule el tiempo que le toma al electrón llegar
al borde si comienza con la energía U0 calculada
en (b).

z
a
r0

e

Problemas Propuestos y Resueltos de Electromagnetismo

#### Problema 3.14

---

### Página 60

CAPÍTULO 3. LEY DE GAUSS

III.

Soluciones

Solución 3.1

P X

a) La carga total en el átomo está dada por
˚
Q=

ρ(r)dV
ˆ2π ˆπ ˆR

=

!

r2
1 − 2 r2 sin θdrdθdϕ
R

ρ0

ˆR

!

r4
r − 2 dr
R

= 4πρ0

= 4πρ0
=

R3 R3
−

!

8π
ρ0 R 3

En general Q 6= 43 πa3 · ρ(r) (hacer esto es un error muy común en el curso). Esto es verdad
solamente cuando ρ(r) = cte.

Rodrigo Chi - Marzo 2017

b) El campo eléctrico está dado por Ley de Gauss, para ello se deben considerar dos posibles
casos (dentro y fuera de la esfera). En ambos casos se asume por simetría esférica que
~ = E(r)r̂.
E

r

R

r

R

W2

W1

Figura 3.1: Superficie Gaussiana Ω1 para r ≥ R Figura 3.2: Superficie Gaussiana Ω2 para r < R

- r ≥ R: En este caso se toma como superficie Gaussiana Ω1 , la cual representa un

---

### Página 61

CAPÍTULO 3. LEY DE GAUSS
casquete esférico de radio r > R.
¨
~ · dS
~ = qenc
E
ε0
Ω1

4πr E(r) =
ε0

ˆ2π ˆπ ˆR

!

r2
1 − 2 r2 sin θdrdθdϕ
R

ρ0

2ρ0 R3
~
r̂
E(r)
=
15ε0 r2
- r < R: En este caso se toma como superficie Gaussiana Ω2 , la cual representa un
casquete esférico de radio r < R.
¨
~ · dS
~ = qenc
E
ε0
Ω2

4πr2 E(r) =
ε0

ˆ2π ˆπ ˆr

!

r2
1 − 2 r2 sin θdrdθdϕ
R

ρ0

r5
4πρ0 r
−
4πr2 E(r) =
ε0
5R2
!
ρ0 r
r3
~
E(r) =
−
r̂
ε0 3 5R2

!

Notar que dado que r es arbitrario, el lado de izquierdo de la ecuación de ley de Gauss
valdrá siempre 4πr2 en problemas de simetría esférica.
c) Mientras que el potencial (considerando V (r → ∞) = 0)
ˆr
V (r) = −

E(r ≥ R)dr
∞
ˆr

=−
∞

2ρ0 R3
dr
15ε0 r2

2ρ0 R3
=
15ε0 r
- r<R

ˆR
V (r) = −

ˆr
E(r ≥ R)dr −

∞

ˆR
=−
∞

E(r < R)dr
R

2ρ0 R3
dr −
15ε0 r2

ˆr

ρ0
ε0

!

r
r3
−
dr
3 5R2

R

2ρ0 R
ρ0
=
−
15ε0
ε0



1 2
(r − R2 ) −
(r4 − R4 )
20R2



Problemas Propuestos y Resueltos de Electromagnetismo

- r≥R

---

### Página 62

CAPÍTULO 3. LEY DE GAUSS
Solución 3.6

P X

a) Usando la Ley de Gauss en el caso z0 = a, la carga puede ser encerrada por un cubo de
lado 2a. Dado que la carga queda en el centro del cubo, entonces por las seis caras sale el
mismo valor del flujo. Luego
Qenc
Qenc
=⇒ Φcara =
ε0
6ε0

Φtotal =

b) Se tiene que considerar que el campo eléctrico esta dado por
~ =
E

q ~r − ~r 0
4πε0 |~r − ~r 0 | 23

Los puntos de la cinta infinita están dados por ~r = xx̂ + aŷ + z ẑ dónde x ∈ (−a, a) y
z ∈ (−∞, ∞). Además ~r 0 = 0. Luego el campo eléctrico esta dado por
q xx̂ + aŷ + z ẑ
4πε0 (x2 + a2 + z 2 ) 32

~ =
E
Para calcular el flujo se recuerda que

¨
~
~ · dS
E

Φ=
S

~ debe tener la dirección de la normal, es decir dS
~ = dzdxŷ. Con lo anterior
En este caso dS
ˆa ˆ∞
Φ=
−a −∞

!

xx̂ + aŷ + z ẑ

q
4πε0

(x2 + a2 + z 2 ) 2

q
· (dzdxŷ) =
4πε0

ˆa ˆ∞

adzdx

(x2 + a2 + z 2 ) 2

−a −∞

Rodrigo Chi - Marzo 2017

Notemos que denominador se puede escribir de la siguiente forma:

(x + a + z ) = (x + a )

z2
1+ 2
x + a2

!3

Con lo anterior
qa
Φ=
4πε0

ˆa ˆ∞
−a −∞

(x2 + a2 )

·

dz
1 + x2z+a2

Se usa el cambio de variable tan θ =
θ ∈ (− π2 , π2 )
qa
Φ=
4πε0

ˆa

qa
 3 dx =
4πε0

−a

ˆ∞

(x2 + a2 )

(x2 +a2 ) 2

−∞

(x2 + a2 ) 2

1 + x2z+a2

 3 dx

, dz = (x2 +a2 ) 2 sec2 θ, y como z ∈ (−∞, ∞),
ˆπ/2

dz


z

−a

ˆa

(x2 + a2 ) 2 sec2 θdθ

−π/2

(1 + tan2 θ) 2

dx

---

### Página 63

CAPÍTULO 3. LEY DE GAUSS
Pero (1 + tan2 θ) = sec2 θ y cos θ = sec−1 θ
Φ=

qa
4πε0

qa
=
4πε0
=

=

2qa
4πε0
qa
2πε0

ˆa

π

(x + a )

ˆ2

cos θdθdx

−a

ˆa
−a
ˆa

(x2 + a2 ) 2

− π2
π

sin θ
dx
x +a
− π2

dx
x 2 + a2

−a
ˆa

dx
x 2 + a2

−a

Nuevamente, usando el cambio de variable u = xa , dx = adu, y como x ∈ (−a, a),
u ∈ (−1, 1)
qa
Φ=
2πε0
=

q
2πε0

ˆ1
−1
ˆ1

adu
(au)2 + a2
du
u2 + 1

−1

q
q
=
arctan u
(arctan(1) − arctan(−1))
2πε0
2πε0
−1


q
π −π
−
=
2πε0 4

=

Φ=

q
4ε0

por lo que el flujo aumenta 0,5 veces.

Solución 3.8

P X

a) Primero se debe calcular el campo eléctrico producido por un cilindro infinito cargado (radio
R, densidad ρ constante) centrado en el origen. Usando Ley de Gauss:
~ = E(r)r̂ en coordenadas cilíndricas, luego:
Dada la geometría del problema: E
Para r < R:

¨

ˆ2π ˆh
~ · dS
~=
E

Erdθdz = 2πrhE =

Q
ε0

Problemas Propuestos y Resueltos de Electromagnetismo

Finalmente

---

### Página 64

CAPÍTULO 3. LEY DE GAUSS
Por otro lado
˚
Q=

ρdV = ρπr2 h =⇒ 2πrhE =

ρπr2 h
~ < R) = ρr r̂
=⇒ E(r
ε0
2ε0

El caso r > R es irrelevante para esta pregunta, luego no es necesario calcularlo ya que la
zona donde se pide calcular el campo es tal que r < R siempre.

y

r

+r

~r1

~r2
2x0 x̂

x

Figura 3.3: Vectores posición en el área de intersección
~1 y E
~ 2 los campos producidos por los cilindros
Ahora volviendo al problema original, sean E
cargados con −ρ y +ρ respectivamente, usando el resultado anteriormente encontrado:
~ 1 = − ρr1 r̂1 = − ρ~r1
E
2ε0
2ε0
~ 2 = ρr2 r̂2 = ρ~r2
E
2ε0
2ε0

Rodrigo Chi - Marzo 2017

Donde los vectores ~r1 y ~r2 se miden desde el centro del cilindro correspondiente a cada uno
de ellos (Figura 3.3). Finalmente, usando que:
~r1 − ~r2 = 2x0 x̂
Se obtiene:

~ =E
~1 + E
~ 2 = ρ (~r2 − ~r1 ) = − ρx0 x̂
E
2ε0
ε0

b) Si x0
R entonces en el borde del = Cilindro equivalente” posee un espesor ∆r = r1 − r2 .
Donde los segmentos de r1 , r2 y 2x0 forman un triángulo, cuyo ángulo opuesto al lado r2
es θ. Así, usando el teorema del coseno (y, por simplicidad, definiendo d = 2x0 ) :
r2 =

q

r12 + d2 − 2r1 d cos θ

Luego como xd0 → 0 entonces se realiza una aproximación de Taylor en torno a d = 0, de
lo que resulta:

---

### Página 65

CAPÍTULO 3. LEY DE GAUSS

r2 ≈ r1 + q
(2d − 2r1 cos θ)|d=0 (d − 0) = r1 − d cos θ
2 r12 + d2 − 2r1 d cos θ
Por lo tanto:
∆r = r1 − r2 ≈ d cos θ
Por otra parte, en un pequeño volumen dV en el borde del = Cilindro equivalente” existe
una carga ∆Q, que cumple:
∆Q = ρdV = ρ∆A∆r = ρ∆Ad cos θ
Finalmente, de la relación anterior es posible definir una densidad de carga superficial en el
borde del = Cilindro equivalente” cuando x0
R:
σ = ρ∆r ⇒ σ = ρd cos θ = 2x0 ρ cos θ
Nota: observar que dicha densidad σ es consistente en sus signo con la distribución de las
cargas en el = Cilindro equivalente” pues es proporcional a cos θ.

Solución 3.10

P X

a) La carga contenida será para r ≤ R:
˚
Qenc (r ≤ R) =

ˆh ˆ2π ˆr
ρ(r)dV =

r
2πhr3
· rdrdθdz =
a
3a

˚
Qenc (r > R) =

ˆh ˆ2π ˆR
ρ(r)dV =

2πhR3
r
· rdrdθdz =
a
3a

b) Usando la ley de Gauss para r ≤ R:
¨
r2
~ = Qenc =⇒ E(r) · 2πrh = 2πhr =⇒ E(r)
~ · dS
~
E
=
r̂
ε0
3aε0
3aε0
De igual forma, para r > R:
¨
R3
~ = Qenc =⇒ E(r) · 2πrh = 2πhR =⇒ E(r)
~ · dS
~
E
=
r̂
ε0
3aε0
3aε0 r
c) El potencial V (r), usando como referencia V (r = 0) = 0 , estará dado por
ˆr
V (r) = V (r) − V (0) = −

E(r)dr

Problemas Propuestos y Resueltos de Electromagnetismo

mientras tanto, en el caso r > R

---

### Página 66

CAPÍTULO 3. LEY DE GAUSS
Para un radio r ≤ R el potencial está dado por
ˆr
V (r) = −

r2
r3
dr = −
3aε0
9aε0

de forma parecida, el potencial para un radio r > R es
ˆR
V (r) = −

r2
dr −
3aε0

ˆr

R3
R3
r
dr = −
ln
+
3aε0 r
3aε0
R








R

d) Los gráficos están dados por

V (r)

|~E(r)|

R
r

R2
3ae0
R3
9ae0

r

R

Figura 3.5: Potencial Eléctrico

Figura 3.4: Campo Eléctrico

Rodrigo Chi - Marzo 2017

Solución 3.13

P X

a) Dado que el sistema está compuesto por una recta infinita y un plano infinito, se determina
cual es el campo eléctrico que genera cada uno de ellos y luego se procederá a la rotación
del resultado. Como resultados generales para un plano infinito y una recta se tiene que:
¨
σ
~ = Qenc =⇒ 2AE(z) = σA =⇒ E(z)
~ · dS
~
E
=
ẑ
ε0
ε0
2ε0
¨

λ
~ = Qenc =⇒ 2πrLE(r) = λL =⇒ E(r)
~
~ · dS
E
=
r̂
ε0
ε0
2πrε0

En este problema se debe tomar como referencia la siguiente Figura
Se toma un punto P arbitrario a una distancia y desde la bisectriz hasta el plano. Sobre
~1 y E
~ 2 provocados por el plano y por la recta,
ese punto actúan dos campos eléctricos (E
respectivamente), de modo que la superposición de ambos campos es el campo total en el
punto. Usando el sistema de referencia de la Figura 3.6, el campo total vale:
~ T = |E
~ 1 |ŷ − |E
~ 2 | cos(2α)ŷ + |E
~ 2 | sin(2α)x̂
E

---

### Página 67

CAPÍTULO 3. LEY DE GAUSS
l

y

~E1

y
a
a

2a

y

~E2
s

x

Figura 3.6: Campos Eléctricos en un punto sobre la bisectriz
Donde

σ
~ 2| = λ
, |E
2ε0
2πyε0
Nótese que dado la recta donde se quiere conocer el campo es bisectriz, la distancia del plano
al punto debe ser igual a la de la recta cargada a la bisectriz (congruencia de triángulos).
Finalmente el campo total cuando y = h vale
~ 1| =
|E

!

~ T (h) = λ sin (2α) x̂ + σ − λ cos (2α) ŷ
E
2πhε0
2ε0
2πhε0
b) El trabajo necesario para mover la carga está dado por la siguiente expresión
~
~ T (y) · dl
E

W = −q
A

En esta caso A = h y B = h2 , además dado que no es ni un camino horizontal ni vertical, se
~ = dxx̂ + dy ŷ, donde en la recta bisectriz se cumple que dy = tan α (pendiente
tiene que dl
dx
de la bisectriz). Reemplazando
h

ˆ2
W = −q

! !

λ sin (2α)
σ
λ cos (2α)
dy
x̂ +
−
ŷ ·
x̂ + dy ŷ
2πyε0
2ε0
2πyε0
tan α

h

 h

ˆ2



= −q 

h

h

λ sin (2α) dy
+
2πyε0 tan α

ˆ2


!


σ
λ cos (2α)
−
dy 

2ε0
2πyε0

h

"

!#

λ sin (2α)
σh
λ cos (2α)
=q
ln(2) +
−
ln(2)
2πε0 tan α
4ε0
2πε0


qσh qλ ln(2) sin 2α
=
+
− cos 2α
4ε0
2πε0
tan α

!

Problemas Propuestos y Resueltos de Electromagnetismo

ˆB

---

### Página 68

CAPÍTULO 3. LEY DE GAUSS
Solución 3.14

P X

a) Por ley de Gauss, se tiene que el campo eléctrico para r > a es
¨
~ = qenc =⇒ E(r) · 2πrL = ρ0 πa L =⇒ E
~ · dS
~ = ρ0 a r̂
E
ε0
ε0
2rε0
Mientras que para r < a
¨
~ = qenc =⇒ E(r) · 2πrL = ρ0 πr L =⇒ E
~ = ρ0 r r̂
~ · dS
E
ε0
ε0
2ε0
Luego el potencial para r < a es
ˆr
V (r) = V (r) − V (0) = −

ρ0 r
ρ0 r 2
dr = −
2ε0
4ε0

y para r > a
ˆa
V (r) = V (r) − V (0) = −

ρ0 r
dr −
2ε0

ˆr
a

ρ 0 a2 ρ 0 a2
r
ρ0 a2
dr = −
−
ln
2rε0
4ε0
2ε0
a

 

b) Dado que la energía inicial es nula ya que el electrón está en reposo y el potencial es nulo
en r = 0, la energía en r = a será igual al trabajo realizado para mover el electrón a r = a.
Luego
ˆa
eρ0 a2
ρ0 r
dr =
U0 = W = e
2ε0
4ε0

Rodrigo Chi - Marzo 2017

c) Usando la segunda ley de Newton, se tiene que para r < a
~ =⇒ mr̈ = − eρ0 r =⇒ r̈ + eρ0 r = 0
F~ = m~a = −eE
2ε0
2ε0 m
La ecuación diferencial anterior corresponde a un movimiento armónico simple de frecuencia
angular
s
eρ0
ω=
2ε0 m
Al ser un movimiento oscilatorio e iniciar con la energía determinada en (b), el electrón
podrá llegar como máximo al borde r = a y luego se dirigirá al punto diametralmente
opuesto. En conclusión, el tiempo que se demorará en llegar a r = a será un cuarto del
periodo de oscilación, es decir
T
1 2π
π
t= =
=
4 ω

s

2ε0 m
eρ0

---

### Página 69

CAPÍTULO 3. LEY DE GAUSS

IV.

Indicaciones Problemas Sin Solución

Indicación 3.2

P X

Aplique la ley de Gauss sobre el cable coaxial. Este problema posee simetría cilíndrica.
Debe ponerse en cinco posibles casos donde existe campo eléctrico.

Indicación 3.3

P X

En este problema debe usar el principio de superposición. Determine en primera instancia
determine cuanto vale el campo eléctrico que provoca el plano infinito y el bloque infinito
mediante Ley de Gauss.
Note que los campo eléctrico que provoca un plano infinito es constante (independiente de
la altura). Lo mismo ocurre para los puntos fuera del bloque de ancho D.

Indicación 3.4

P X

Aplique ley de Gauss a la esfera, debe ponerse en tres posibles casos.

Indicación 3.5

P X

Determine el campo eléctrico dentro de las placas paralelas mediante superposición.
Determine la ecuación de movimiento para el caso del electrón y el protón. Las fuerzas
aplicadas sobre las cargas son el peso y la fuerza eléctrica.

Indicación 3.7

P X

El problema debe ser abordado mediante el principio de superposición. El campo dentro de
la cavidad puede ser determinado como la resta de otros dos.

Problemas Propuestos y Resueltos de Electromagnetismo

Recuerde que la ley de Gauss sólo ve la carga encerrada, por lo que puede ignorar la carga
que esta afuera de la superficie Gaussiana que este tomando.

---

### Página 70

CAPÍTULO 3. LEY DE GAUSS
Es necesario conocer cuanto es el campo eléctrico dentro de una esfera de densidad constante
ρ0 . Puede ser muy útil recordar que ~r = rr̂.
Deje expresado el campo eléctrico dentro de la cavidad en función de dos sistemas de
referencia (uno con respecto al centro de la esfera y otro con respecto al centro de la
cavidad). Finalmente, use el vector d~ para relacionarlos y concluir el problema.

Indicación 3.11

P X

Note que tanto el alambre como la superficie cilíndrica tienen simetría cilindra. Luego es
posible aplicar ley de Gauss en forma directa a la configuración.
Al mover el alambre una distancia δ el problema pierde la simetría del punto anterior. ¿Cómo
debe calcularse el campo eléctrico en este caso?.

Indicación 3.12

P X

Dado que la geometría del problema es infinita en x e y, sólo puede tener dependencia de
una sola variable.
Note que la densidad de carga es simétrica con respecto al plano xy, lo cual afecta directamente al campo.

Rodrigo Chi - Marzo 2017

La superficie gaussiana que puede tomar para determinar el campo eléctrico puede ser un
paralelepípedo o un cilindro de altura 2z (desde −z hasta z).

---

### Página 71

CAPÍTULO 3. LEY DE GAUSS

V.

Respuestas
Problema

Respuestas

P

P

3.1

3.2

a) Q = 8πρ150 R
( ρ
15R2 ε0 (5R r − 3r )r̂ r ≤ R
~
b) E(r) =
2ρ0 R
r>R
15ε0 r 2 r̂
(
ρ0 (r 2 −R2 ) (7R2 −3r 2 )
2ρ0 R2
r≤R
15ε0 − 15ε0 R2
c) V (r) =
2ρ0 R3
r>R
15ε0 r




ρ2 (r 2 −R12 )


r̂

2ε0 r

ρ2 (R22 −R12 )
~
r̂
E(r) =
2ε0 r


ρ2 (R22 −R12 )+ρ4 (r 2 −R32 )

r̂

2ε0 r


 ρ2 (R22 −R12 )+ρ4 (R42 −R32 )
r̂
2ε0 r

0 < r < R1
R1 ≤ r ≤ R2
R 2 ≤ r ≤ R3
R3 ≤ r ≤ R4
r ≥ R4

~ = − σ ẑ + ρD ẑ
a) E
2ε0
2ε0

P

3.3

~ = + σ ẑ + ρ(D−2d) ẑ
b) E
2ε0
2ε0
~ = + σ ẑ − ρD ẑ
c) E
2ε0
2ε0

3.4

0<r<a
a≤r≤b
r≥b

v2 h

P

3.5

P

3.6

v2 h

Protón: εσ0 (g − 2 dx2 ) < mep < εσ0 (g + 2 dx2 )
2hv 2

Electón: mee < εσ0 ( d2 x − g)
Q
a) ΦE = 6ε

b) Aumenta 1, 5 veces.

Problemas Propuestos y Resueltos de Electromagnetismo

P

 nρr

 − 3ε0 r̂

ρ
a3
~
r
−
(n
+
1)
r̂
E=
3ε0
r


 ρ
r̂
3ε0 r 2 b − (n + 1)a

---

### Página 72

CAPÍTULO 3. LEY DE GAUSS

P
P

Problema

Respuestas

3.7

~ = ρ0 d~
E
3ε0

3.8

~ = − ρx0 x̂
a) E
ε0
b) σ(θ) = 2x0 ρ cos θ
a) ρ(r) = 4ε0aE2 0 r

P

3.9

~ > a) = E02a2 r̂, V (r > a) = E0 a2
b) E(r
r
r


c) V (r ≤ a) = E30 4a − ar 2
(

2πhr 3
3a
2πhR3
3a

r≤R
r>R

(

r2
3aε0 r̂
R3
3aε0 r r̂

r≤R
r>R

(

r
− 9aε
0 
R3
− 3aε
ln

a) Q(r) =

P

3.10

~
b) E(r)
=

c) V (r) =

(
~
a) E(r)
=


P

3.11

b) V (r) =
nuo.

r
R



Rσ
λ
2πε0 r + ε0 r



+ 31

λ

2πε0 r r̂

r≤R
r>R



r<R
r̂

λ
R
2πε0 ln r

λ
ε0 2π + Rσ ln

r>R



R
r



El campo eléctrico es discontinuo en r = R.

r≤R
El potencial eléctrico es siempre contir>R

Rodrigo Chi - Marzo 2017

c) En este caso no puede volverse a usar la ley de Gauss para ambas distribuciones
de forma simultánea ya que pierde la simetría cilíndrica. En este caso debe
determinarse el campo eléctrico por separado y luego superponer.

P

P

3.12

3.13

~
E(z)
= kερ0 (1 − e−kz )ẑ
~ T (h) = λ sin (2α) x̂ +
a) E
2πhε0
qλ ln(2)
b) W = qσh
4ε0 + 2πε0

( ρr

2ε0 r̂
ρ0 a2
2rε0 r̂

~
a) E(r)
=

P

3.14

b) U0 = W = e

´a ρ0 r

c) t = π2

q



λ cos (2α)
σ
2ε0 − 2πhε0

sin 2α
tan α − cos 2α

r≤a
r>a

2ε0 dr =

eρ0 a2
4ε0

2ε0 m
eρ0

ŷ



(
V (r) =



0r
− ρ4ε

0a
0a
− ρ4ε
− ρ2ε
ln

r≤a
r
a



r>a

---

### Página 73

Conductores

I.

Resumen Teórico

Conductores
Un conductor es un material que cumple las siguientes propiedades:
El campo eléctrico es nulo en todos los puntos dentro del conductor. Consecuencia de esto,
el conductor es una equipotencial (todos sus puntos tienen el mismo potencial).
La carga en un conductor sólo se acumula en su/s superficie/s (ie. no existen densidades
de carga volumétricas en un conductores).

Condensadores
Un condensador es un dispositivo el cual tiene la capacidad de almacenar carga. Puede estar
compuesto por uno o dos conductores de forma arbitraria.
Matemáticamente la capacidad de un condensador se define como
C=

Q
|∆V |

(4.1)

Algunas capacitancias conocidas:
Condensador de Placas Paralelas:
C=

ε0 A
d

(4.2)

Problemas Propuestos y Resueltos de Electromagnetismo

~ = σ n̂.
El campo eléctrico es siempre perpendicular a la superficie de un conductor y vale E
ε0
Donde σ es la densidad de carga sobre el conductor y n̂ la normal del conductor.

---

### Página 74

CAPÍTULO 4. CONDUCTORES
Donde A es el área de las placas y d la distancia de separación.
Condensador Cilíndrico:
C=

2πε0 L
ln( ab )

(4.3)

Donde L es el largo del condensador, a radio interior y b radio exterior del condensador.
Condensador Esférico:

4πε0 ab
b−a
Donde a radio interior y b radio exterior del condensador.
C=

(4.4)

Los condensadores pueden ser asociados en serie o paralelo dependiendo de como se conecten.
En caso de la capacidad equivalente cuando están conectados en serie es


Ceq =

+
C1 C2

−1

(4.5)

Mientras que cuando están asociados en paralelo, la capacidad equivalente es
Ceq = C1 + C2

(4.6)

Energía Electrostática
La energía electrostática de un sistema es el equivalente a la suma de todos los trabajos que
fueron necesarios para formar ese sistema de cargas, ya sea discreto o continuo.
Para un sistema de N cargas puntuales, la energía del sistema está dado por

Rodrigo Chi - Marzo 2017

U=

N
1X
qi V (~ri )
2 i=1

(4.7)

Donde V (~ri ) es el potencial evaluado en cada posición ~ri de una de las N carga. Para un sistema
continuo de carga, la energía puede ser análogamente determinada como
ˆ
U=
dq(~r 0 )V (~r 0 )
(4.8)
Otra forma equivalente para distribuciones continuas de carga es
˚
ε0
~ 2 dV
U=
|E|

(4.9)

Todo el
Espacio

Para el caso de un condensador, la energía puede ser obtenida a partir de
U=

1 Q2
= CV 2 = QV
2C

(4.10)

---

### Página 75

CAPÍTULO 4. CONDUCTORES

Recomendaciones
Dentro de los materiales que se estudian en un curso tradicional de electromagnetismo, los
conductores tienen la gracia de poseer sólo = carga libre” (sin ligaduras a otra carga ). Al
ser un conductor una equipotencial, la carga puede moverse libremente entre las superficies
del conductor.
La capacidad de un condensador sólo depende de la geometría de éste. La capacidad es una
constante del sistema (ie. si la diferencia de potencial entre los dos conductores aumenta al
doble, la carga sobre los conductores también lo hará).
Las Ecuaciones 4.8, 4.9 y 4.10 son equivalentes, todas deberían llevar al mismo resultado.
Cuál usar dependerá del problema y de los datos que se entreguen.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 76

CAPÍTULO 4. CONDUCTORES

II.

Problemas Propuestos

#### Problema 4.1

X S

a) Calcule la fuerza eléctrica que actúa sobre las
placas de un condensador de placas planas, cargado con carga Q.

Q
+Q

b) Considere que la carga Q sobre las placas del
condensador se mantiene y que su capacidad
es C. Calcule el trabajo que se realiza al llevar
las placas a la mitad de la distancia original,
manteniendo la carga constante. Puede suponer
que las placas poseen una área A muy grande.
c) Este nuevo condensador se conecta en paralelo
con otro condensador inicialmente descargado
e igual al condensador de la parte (a). Calcule
la diferencia de potencial entre las placas del
condensador equivalente.
#### Problema 4.2

l

X S

Un alambre infinito tiene una distribución lineal de
carga λ > 0. El alambre se encuentra ubicado en el
centro de una superficie cilíndrica conductora infinita
muy delgada de radio R conectada a tierra como se
muestra en la Figura.

Rodrigo Chi - Marzo 2017

a) Encuentre la densidad de carga superficial inducida σ en la superficie interior conductora.
b) Encuentre el campo eléctrico en todo el espacio.
c) Encuentre el potencial eléctrico en todo el espacio.

R

---

### Página 77

CAPÍTULO 4. CONDUCTORES
#### Problema 4.3

X S

Se desea diseñar un condensador esférico a partir de
un casquete conductor esférico de radio exterior a, que
sea capaz de almacenar la mayor cantidad de energía
posible, sujeto a la restricción que el campo eléctrico en la superficie de la esfera conductora interior,
concéntrica con el casquete y de radio b < a, no pueda exceder un valor dado E0 . Calcule, en función de
E0 , a y constantes, el valor que debe tener el radio b
y la magnitud de la energía que puede almacenar el
conductor.

#### Problema 4.4

a

b

X S
R1

Le
j
uy
M

R2

X S

Un ión es acelerado desde el reposo hasta una diferencia de potencial V0 para luego entrar en una región
entre dos electrodos cilíndricos muy largos A y B,
de radios a y b respectivamente (a < b). El ión recorre una media circunferencia de radio r0 haciendo
una trayectoria circular. Despreciando efectos de borde y asumiendo que los cilindros son muy largos en
comparación al espacio que los separa, encuentre la
diferencia de potencial VBA .

r0
B
V =0

A

V = VO

Fuente de Iones

a

b

Problemas Propuestos y Resueltos de Electromagnetismo

#### Problema 4.5

os

Se tienen dos esferas conductoras de radio R1 y R2 separadas entre si una distancia suficientemente grande
que asegura que cualquier carga sobre ellas se distribuye uniformemente, sin que la presencia de una esfera
afecte a la otra. Se desea distribuir una carga Q entre
las dos esfera de manera que la energía potencial electrostática del sistema de las dos esferas sea mínima.
Claramente, en una esfera habrá Q − q y en la otra q.
¿Cuánto vale q, cuál es energía total y cuál es el potencial de cada esfera cuándo se alcanza la condición
de energía mínima?.

---

### Página 78

CAPÍTULO 4. CONDUCTORES
#### Problema 4.6

X I

Una esfera maciza conductora de radio R tiene un
cavidad esférica de radio a dentro de ella (a < R).
Dentro de la cavidad existe una carga puntual q la
cual se ubica en un punto dentro de ella (no necesariamente el centro).
a) Determine la carga total inducida en la superficie de la cavidad esférica de radio a. Indique
cualitativamente como es la densidad superficial
de carga sobre ella.

a

R

q

b) Determine la carga total inducida en la superficie exterior de la esfera de radio R. Indique cualitativamente como es la densidad superficial de
carga sobre ella.
c) Indique cambian las respuestas anteriores si: (i)
se acerca una carga q 0 a distancia 2R del centro
de la esfera de radio R (ii) se conecta la esfera
de radio R a una fuente de tensión V0 .

Rodrigo Chi - Marzo 2017

#### Problema 4.7

X I

Uno de los primeros modelos de átomo, como un ente
compuesto de partes cargadas, lo propuso el descubridor del electrón Joseph John Thomson en 1904. Este
modelo, también conocido como el modelo del pastel
de fresas, concibe al átomo como una esfera de carga
positiva, en la cual están incrustados los electrones.
En el espíritu del modelo del pastel de fresas, modelemos un átomo de hidrógeno (en equilibrio estático)
como una esfera de radio R1 de carga negativa −e
uniformemente distribuida en su volumen (el electrón
fresa), rodeada de una esfera más grande (concéntrica
a la primera), de radio R2 > R1 , con carga positiva +e
uniformemente distribuida en el volumen comprendido entre R1 y R2 . Determine la energía de formación
de este átomo (i.e. el trabajo necesario para formarlo
trayendo las cargas desde el infinito).

+

-

R1

R2

---

### Página 79

CAPÍTULO 4. CONDUCTORES
#### Problema 4.8

X S

Considere una esfera maciza conductora de radio a se
encuentra a un potencial V0 en toda su superficie con
respecto al infinito. La esfera esta recubierta por un
casquete esférico conductor de radio interno b y radio
externo c.

c

a

a) Determine el campo eléctrico y el potencial
eléctrico en todo el espacio. Además encuentre
las densidades de carga inducidas en los conductores.

b

b) Si el casquete esférico se conecta a tierra,
¿cómo cambian sus respuestas anteriores?.

#### Problema 4.9

X I

Considere dos esferas conductoras de radios a y b.
Las esferas están lo suficientemente lejos una de otra
como para despreciar su interacción, (i.e. el equilibrio
electrostático de una esfera no se ve afectado por el
campo que genera la carga contenida en la otra).

b) Considere ahora que las esferas están descargadas y desconectadas. Suponga ahora que la distancia que separa las esferas es d
a, b desde
sus centros. Considerando que dos conductores
cualesquiera pueden formar un capacitor, determine la capacitancia de esta configuración.

Interruptor

b

Problemas Propuestos y Resueltos de Electromagnetismo

a) Suponga que las esferas tienen cargas Q1 y Q2 ,
respectivamente. Las esferas se ponen en contacto mediante un cable lo suficientemente largo, el cual posee un interruptor. Se conectan
las dos esferas y se espera hasta que el sistema
alcance el equilibrio electrostático, para luego
desconectar el interruptor. Determine la carga
que posee cada esfera luego que se desconecta el interruptor. ¿Qué esfera queda con mayor
carga?.

a

---

### Página 80

CAPÍTULO 4. CONDUCTORES

#### Problema 4.10

X S

Considere una esfera maciza conductora de radio R
con una burbuja esférica excéntrica de radio c. El centro de la burbuja está a una distancia b del centro de
la esfera metálica. La esfera tiene una carga Q. Determine el potencial en el interior de la burbuja. ¿Cómo
se modifica el resultado si la burbuja no es esférica?

R

c
b

A

#### Problema 4.11

B

X I

Considere dos condensadores cilíndricos como se indican en la figura. Los condensadores tienen radios R1 y
R2 y el otro R3 y R4 (ver figura), determine la capacitancia equivalente entre los puntos A y B. Suponga
que R1 , R2 , R3 , R4
L.

L

R2

R4
R3

R1

Rodrigo Chi - Marzo 2017

#### Problema 4.12

X S

Un sistema consiste de dos cascarones conductores
cilíndricos concéntricos de longitud L
d (a, b, c,
d definidos en la figura). El cascarón interior contiene
una carga total +Q y el exterior una carga total −Q.
Determine:

L
(a) Vista Exterior

a) La densidad carga en cada una de las cuatro
superficies conductoras.
a

b) El potencial en todo el espacio.

b

d

c) La diferencia de potencial de los conductores
cilíndricos.

c
(b) Vista Interior

---

### Página 81

CAPÍTULO 4. CONDUCTORES
#### Problema 4.13

X I

Una carga +Q se encuentra inserta en un alambre
conductor de largo L y radio R0 muy pequeño. Un
cascarón cilíndrico conductor neutro de radios interno
R1 y externo R2 y largo L es ubicado simétricamente
alrededor del alambre (ver figura). Tener en cuenta
que: R0
R1 , R2
L. Calcule:
a) La densidad lineal de carga λ del alambre.
b) La densidad superficial de carga en la capa interna y externa del cascarón; y la densidad volumétrica de carga dentro del conductor.
c) El campo eléctrico en todo el espacio.

R2

Ahora deposite una carga −Q en el cascarón cilíndrico, calcule:

R1

R0

d) Las nuevas densidades de carga superficiales en
las capas interna y externa del cascarón, y también la densidad volumétrica dentro de éste.
e) El nuevo campo eléctrico en todo el espacio.
f) La diferencia de potencial entre el cilindro y el
alambre ∆V = Vcilindro − Valambre .

h) La capacidad C 0 si ahora el alambre tiene carga
+2Q y el cascarón tiene carga -2Q.

#### Problema 4.14

X S

Una esfera maciza de radio a y carga Q uniformemente distribuida es blindada por una capa conductora de
espesor uniforme a. La carga neta de la capa es nula.
Calcule y grafique el potencial V (r) en todo el espacio. Considere V (r) nulo infinitamente lejos de la
esfera.

Q

a
2a

Problemas Propuestos y Resueltos de Electromagnetismo

g) La capacidad (o capacitancia) del sistema y la
energía almacenada en el sistema.

---

### Página 82

CAPÍTULO 4. CONDUCTORES
X S

#### Problema 4.15

Un bloque macizo infinito en sus coordenadas x e y,
posee su espesor entre z = a y z = −a. En el espacio
existe una densidad de carga dada por



ρ(z) = 



 |z| > a
z+a
z−a
ρ0 exp −
+ exp
|z| ≤ a
δ
δ




z

con ρ0 y δ constantes positivas conocidas.
a) El campo eléctrico en todo el espacio.

z=a
r(z)

b) Si δ
a, determine nuevamente el campo
eléctrico en el espacio ¿qué tipo de comportamiento presenta el material?. Justifique su respuesta. Dibuje las líneas de campo en la proximidad del material considerando la aproximación.

y

z= a

c) Usando el campo eléctrico calculado en b) determine el potencial electrostático en todo el
espacio. Use como referencia V (z = −a) = V0 .
Dibuje claramente las superficies equipotenciales.

Rodrigo Chi - Marzo 2017

#### Problema 4.16

X S

Sean dos cilindros infinitos concéntricos conductores,
uno de ellos macizo de radio R1 , y el otro un cascarón
de radios R4 y R5 conectado a tierra, como muestra
la figura. Se coloca una densidad volumétrica de carga
ρ0 entre los cilindros de ancho (R3 − R2 ).
a) Determine el campo eléctrico en todo el espacio y las densidades de cargas inducidas en las
superficies conductoras.
b) Calcule la diferencia de potencial entre los conductores.

r0

R1

R2
R3
R4
R5

---

### Página 83

CAPÍTULO 4. CONDUCTORES

III.

Soluciones

Solución 4.1

P X

a) La energía de un condensador es U = 12 QC , dado que un condensador es de placas paralelas
su capacitancia está dada por C = Aεz 0 donde A es el área de las placas y z la distancia
que las separa, por lo que la fuerza es
1 Q2
1 Qσ
∂U
ẑ = −
ẑ = −
ẑ
F~ = −
∂z
2 ε0 A
2 ε0
b) Si se desea disminuir a la mitad la distancia entre las placas del condensador C = Aεz 0 , se
tiene que la nueva capacitancia vale
C0 =

Aε0
z

= 2C

Por lo que el trabajo puede ser calculado por la diferencia de energías que experimenta el
condensador
1 Q2
Q2
1 Q2
−
=−
W = Ufinal − Uinicial =
2 2C 2 C
4C
c) En este caso los condensadores son conectados en paralelo, por lo que la capacitancia del
condensador equivalente es
Ceq = C + 2C = 3C

∆V =

Solución 4.2

Q
3C

P X

a) Para iniciar el problema hay calcular el campo eléctrico usando la ley de Gauss. Para r ≤ R
se tiene que:
¨
~ = q =⇒ E(r)2πrL = λL =⇒ E
~ · dS
~ = λ r̂
E
ε0
ε0
2πε0 r
De este resultado ya puede deducirse la densidad de carga, dado que en el borde de un
~ = σ n̂ = σ (−r̂). El resultado anterior tiene que ser igual a
conductor se tiene que E
ε0
ε0
λ
~
r̂, por lo que
E(R)
=
2πε0 R
λ
σ=−
2πR

Problemas Propuestos y Resueltos de Electromagnetismo

donde la diferencia de potencial queda determinada por

---

### Página 84

CAPÍTULO 4. CONDUCTORES
b) Luego para r > R : Dado que la capa externa del conductor está conectada a tierra, éste
posee potencial cero en toda su superficie lo que provoca que solamente exista la carga
negativa anteriormente calculada. Por lo tanto, volviendo a usar ley de Gauss:
¨
λ
~ = q = λL + (− 2πR ) · 2πRL = 0 =⇒ E
~ dS
~ =0
E
ε0
ε0
Notar que la conexión a tierra provoca físicamente una descarga de la capa exterior del
conductor.
c) Para el cálculo de potenciales hay que notar que para r > R se tiene que
~ = −∇V = 0 =⇒ V (r) = cte.
E
Luego como el potencial es continuo y V (R) = 0 (conexión a tierra) se deduce que
V (r) = V (R) = 0
Finalmente para r < R se tiene que:
ˆr
V (r) = V (r) − V (R) = −

ˆr
E(r)dr = −

R

Solución 4.3

λ
r
λ
dr = −
ln
2πε0 r
2πε0
R




R

P X

Suponiendo una carga Q en la superficie conductora de radio b, entonces el campo eléctrico a
una distancia r del origen será de la forma:

Rodrigo Chi - Marzo 2017

Q
Q
=⇒ V =
E(r) =
4πε0 r
4πε0



1 1
−
b a



Donde V es la diferencia de potencial entre la superficie de radio interior y exterior. De esta
manera, se obtiene la capacidad del sistema:
C=

Q
4πε0 ab
=
V
a−b

Por otro lado, tomando el caso límite r = b en el cual el campo eléctrico alcanza su máximo valor
posible E(r = b) = E0 , se tiene:
E0 =

σ
b2 E0
=⇒ Q = 4πb2 σ = 4πb2 ε0 E0 =⇒ E(r) = 2
ε0
r

Luego se usan estos valores obtenidos para calcular la energía del sistema:
U=

Q2
2πε0 b3 E02 (a − b)
=
2C
a

---

### Página 85

CAPÍTULO 4. CONDUCTORES
Ahora para encontrar su máximo (o mínimo):
dU
2πε0 E02
3a
=
(3ab2 − 4b3 ) = 0 =⇒ b =
db
a
Luego calculando la segunda derivada:
d2 U
3a
2πε0 E02
2πε0 E02
(6ab − 12b ) =⇒ U b =
=
=
db2
a
a






18a2 − 27a2

!

<0



Por lo tanto, U b = 3a
es máximo, con:


Solución 4.4

3a
27πε0 E02 a3
=


U b=

P X

Se supondrá que la esfera conductora de radio R1 tiene una carga Q−q y que la esfera conductora
de radio R2 tiene una carga q. Los campos eléctricos que generan ambas esferas son
~ 1 (r1 > R1 ) = Q − q r̂1
E
4πε0 r12

~ 2 (r2 > R2 ) =
E

q
r̂2
4πε0 r22

Todo el Espacio

ε0
=

ˆ2π ˆπ ˆ∞

0 R1

(Q − q)2
=
8πε0

ˆ∞

R1

Q−q
4πε0 r12

!2

r12 sin θdr1 dθdϕ

dr1
r12

=

(Q − q)
8πε0 R1

Análogamente, se tiene que U2 =

q2
. Luego, la energía total es
8πε0 R2

UT = U1 + U2 =

(Q − q)2
q2
+
8πε0 R1
8πε0 R2

Dado que se desea encontrar un mínimo o un máximo
Q − q∗
q∗
QR2
dUT
=
−
+
= 0 =⇒ q ∗ =
dq
4πε0
R1
R2
R1 + R2




Problemas Propuestos y Resueltos de Electromagnetismo

Donde r̂1 y r̂2 son vectores unitarios en coordenadas esféricas con origen en las esferas R1 y R2 ,
respectivamente. Dado que las dos esferas están muy alejadas entre sí, se considera que el campo
eléctrico de una no afecta sobre la otra, por lo que la energía de la esfera de radio R1 es
˚
ε0
|E1 |2 dτ
U1 =

---

### Página 86

CAPÍTULO 4. CONDUCTORES
Lo que es efectivamente mínimo ya que
d2 UT
+
>0
=
dq
4πε0 R1 R2




Por lo que la energía mínima total está dada por
Umin =

(Q − q ∗ )2
q∗2
Q2
+
=
8πε0 R1
8πε0 R2
8πε0 (R1 + R2 )

Por lo tanto, los potenciales a mínima energía son
ˆ∞
V1 (R1 ) =

E1 (r1 )r̂1 · dr1 r̂1 =

Q − q∗
Q
=
4πε0 R1
4πε0 (R1 + R2 )

E2 (r2 )r̂2 · dr2 r̂2 =

q∗
Q
=
4πε0 R2
4πε0 (R1 + R2 )

R1

ˆ∞
V2 (R2 ) =
R2

Solución 4.5

P X

Dada la configuración de la figura, se llamará VA y VB a los potenciales de la placa interior y
exterior respectivamente. Dado que inicialmente el ión de masa m y carga q se encuentra en
reposo y es acelerado mediante una diferencia de potencial, se tiene que por conservación de la
energía

Rodrigo Chi - Marzo 2017

1 2
1 2
+ qVinicial = mvfinal
+ qVfinal
Uinicial + Kinicial = Ufinal + Kfinal =⇒ mvinicial
De este modo si vinicial = 0, Vinicial = V0 , Vf inal = 0, se obtiene que la velocidad con la cual el
ión entra a las placas cilíndricas es
s
2qV0
v=
m
Por otra parte, si se supone una densidad de carga σa (a priori desconocida) en el electrodo interior
y se obvian efectos de borde, el campo eléctrico que existe dentro de los electrodos semicilíndricos
es el mismo en el que existiría en un capacitor cilíndrico completo, por lo tanto por ley de Gauss
para r ∈ [a, b] se tiene que
¨
σa a
~ = q =⇒ E(r) · 2πrL = σa · 2πaL =⇒ E(r)
~ · dS
~
E
=
r̂
ε0
ε0
ε0 r
Volviendo a analizar el movimiento del ión, si se desea que cumpla un movimiento circunferencia
de radio r0 , su aceleración en coordenadas cilíndricas debe estar dada por
~a = −r0 θ̇2 r̂ =⇒ ~a = −

v2
r̂
r0

---

### Página 87

CAPÍTULO 4. CONDUCTORES
Por Newton

~ 0 ) = m~a =⇒ q · σa a = −m · v =⇒ σa = − 2V0 ε0
F~ = q E(r
ε0 r 0
r0
a

Reemplazando
2V0
~
E(r)
=−
r̂
r
Finalmente

ˆb
VB − VA =

b
2V0
dr = 2V0 ln
r
a

!

a

P X

Solución 4.8

a) Se supondrá conocida la densidad de carga σa de la esfera de radio a. Dada la simetría
esférica y que el conductor de radios b y c está descargado se tiene por ley de Gauss que
¨

~ · dS
~ = E(r) · 4πr2 = 4πa σa =⇒ E(r) = σa a
E
ε0
ε0 r 2

En resumen






 σa a2 r̂

0<r<a
a≤r<b
ε0 r2
~
E(r)
=

b≤r<c



 σa a2 r̂ r ≥ c
ε0 r2

Luego dado que el potencial sobre en la esfera es V0 se tiene que
ˆa

ˆc
~ =−
~ · dl
E

V0 = −
∞

∞

σa a2
r̂ · drr̂ −
ε0 r 2

ˆb

ˆa
0 · drr̂ −

c

σ a a2
σa a2
r̂ · drr̂ =
ε0 r 2
ε0



1 1 1
− +
c b a



b

De la última expresión
σa =

a2



ε0 V 0

−
+
c
b
a

Dado que esta carga induce las otras cargas de inducción en el otro conductor, se cumple
que
4πa2 σa = −4πb2 σb (inducción de carga en la superficie interior)
4πb2 σb = −4πc2 σc

(inducción de carga en la superficie exterior)

Problemas Propuestos y Resueltos de Electromagnetismo

En los intervalos [0, a) ∪ [b, c) el campo eléctrico es 0 debido a que en ese espacio hay un
conductor.

---

### Página 88

CAPÍTULO 4. CONDUCTORES
Por lo tanto
a2
ε0 V 0
σb = − 2 σa = −  1 1 1 
b
b2 − +
c

b

a

b2
ε0 V0
σc = − 2 σb =  1 1 1 
c
c
− +
c

b

a

Usado lo calculado en la parte anterior se tiene que el campo eléctrico es
- Si r ∈ [0, a) ∪ [b, c)

~ =0
E

- Si r ∈ (a, b] ∪ (c, ∞).

V0
~ = σa a r̂ = 
 r̂
E
ε0 r 2
− 1 + 1 r2
c

b

a

El potencial estará dado por intervalos
- Si r ∈ (c, ∞).
ˆr
V (r) = −

σ a a2
V0
σ a a2
r̂
·
drr̂
=
= 1 1 1
ε0 r
ε0 r
− + r
c

∞

b

a

- Si r ∈ (b, c].
ˆc
V (r) = −

Rodrigo Chi - Marzo 2017

∞

σ a a2
r̂ · drr̂ −
ε0 r 2

ˆr
c

V0
σa a2
= 1 1 1
0r̂ · drr̂ =
ε0 c
− + c
c

b

a

- Si r ∈ (a, b].
ˆc
ˆb
ˆr


σa a2
σa a2
σa a2 σa a2 1
V (r) = −
r̂ · drr̂ − 0r̂ · drb̂ −
r̂ · drr̂ =
+
−
ε0 r 2
ε0 r 2
ε0 c
ε0
r
b
∞

c

b

V0 ( 1 − 1 + 1 )
V (r) =  1 c 1 b 1 r
−b+a
c
- Si r ∈ [0, a].
V (r) = V0
b) La conexión a tierra provoca los siguientes cambios:

---

### Página 89

CAPÍTULO 4. CONDUCTORES
- La conexión a tierra provoca por definición potencial nulo en cada punto del conductor,
luego para que esta condición se cumpla es necesario que cargas negativas suban de la
tierra y anulen la carga que existe en la capa de radio c del conductor. En consecuencia
se tendrá σc = 0, con lo cual se cumple que el potencial es nulo en el conductor, ya que
σb anula el campo eléctrico es producido por σa (las cuales se mantienen constantes).
De esta forma, el potencial es nulo para cualquier radio r > c.
- El campo eléctrico en ese caso vale
◦ Si r ∈ (0, a) ∪ [b, ∞).

~ =0
E
◦ Si r ∈ [a, b).
V0
 r̂
−
+
r2
c
b
a

~ =
E
- El potencial en este caso vale
◦ Si r ∈ [b, ∞).

V (r) = 0
◦ Si r ∈ [a, b).
1 1
−
V (r) =  1 1 1 
r b
−
+
c
b
a



1 1
−
V (r) =  1 1 1 
a b
−
+
c
b
a



V0



◦ Si r ∈ [0, a).

Solución 4.10



P X

La esfera conductora tiene una carga +Q que se puede distribuir tanto en su superficie exterior
como dentro de la cavidad interior. Dado que no existe ninguna carga dentro de la burbuja,
la carga que se acumula en el borde de la misma es nula. Luego, la carga +Q se distribuye
homogéneamente en la superficie exterior de radio R.
De lo anterior, también se deduce que el campo eléctrico es nulo en cualquier punto dentro de la
esfera (r ≤ R), incluyendo los puntos dentro de la burbuja.
Entonces, el campo eléctrico para r ≥ R puede ser determinado por Ley de Gauss
¨
~ = Qenc =⇒ E
~ · dS
~ = Q r̂
E
ε0
4πε0 r2

Problemas Propuestos y Resueltos de Electromagnetismo

V0

---

### Página 90

CAPÍTULO 4. CONDUCTORES
Lo anterior implica que el potencial en V (R) es
ˆR
V (R) = −
∞

Q
Q
dr =
4πε0 r
4πε0 R

Como el campo eléctrico es nulo en todos los puntos r ≤ R, el potencial es constante en todos
los puntos (incluyendo la cavidad) y tiene un valor de V (R) (valor del borde). Nótese el hecho
que no es necesario una forma esférica para que este análisis siga siendo válido.

Solución 4.12

P X

a) Dada la simetría cilíndrica del problema, es posible usar la Ley de Gauss. Para encontrar las
densidades de cargas inducidas en las superficies conductoras σa y σb se aplica Gauss para
un r ∈ [a, b]
¨
~ = qenc = σa · 2πaL
~ · dS
E
ε0
ε0
˜
~ = 0. Luego se
~ = 0, por lo que
~ · dS
Por una parte dentro de un conductor siempre E
E
debe cumplir que
σa · 2πaL
= 0 =⇒ σa = 0
ε0
Como el conductor interior está cargado con +Q, las densidades de sobre sus superficies
deben cumplir que
Q
σa · 2πaL + σb · 2πbL = Q =⇒ σb =
2πbL
Análogamente, al aplicar Gauss para r ∈ [c, d] se tiene que
¨
~ = qenc = Q + σc · 2πcL = 0 =⇒ σc = − Q
~ · dS
E
ε0
ε0
2πcL

Rodrigo Chi - Marzo 2017

Finalmente como el conductor está cargado −Q se tiene que
σc · 2πcL + σd · 2πdL = −Q =⇒ σd = 0
b) Para determinar el potencial, previamente hay que determinar el campo eléctrico. En base
a lo anterior para r < b se tiene qenc = 0, luego
~ =0
E
Para r ∈ (b, c) se tiene qenc = Q, por lo que
¨
Q
~ = qenc =⇒ E(r) · 2πrL = Q =⇒ E
~ · dS
~ =
E
r̂
ε0
ε0
2πε0 rL
Luego para r > c nuevamente qenc = 0 (notar que toda la carga −Q se acumula en la
superficie en r = c), entonces
~ =0
E

---

### Página 91

CAPÍTULO 4. CONDUCTORES
Entonces tomando el potencial V (r −→ ∞) = 0, se obtiene que
ˆr
~
~ · dl
E

V (r) = −
∞

Para un r > c se tiene que
ˆr
~ =0
~ > c) · dl
E(r

V (r) = −
∞

Para r ∈ [b, c] se tiene que
ˆc

ˆr
~ −
~ > c) · dl
E(r

V (r) = −
∞

ˆr
~ =−
~ < r < c) · dl
E(b

c

c

c
Q
Q
dr =
ln
2πε0 rL
2πε0 L
r

 

Finalmente para r < b
ˆc
V (r) = −

ˆb
ˆr
ˆb
~
~
~ =−
~ > c)·dl−
~ < r < c)·dl−
~ < b)·dl
E(r
E(b
E(r

∞

c

c

b

Q
c
Q
dr =
ln
2πε0 Lr
2πε0 L
b

 

c) La diferencia de potencial está dada por
Q
c
ln
V (c) − V (b) =
2πε0 L
b

 

P X

Para iniciar este problema se debe primero intuir como será el potencial en todo el espacio, para
ello se debe notar lo siguiente:
La función potencial V (r) es continua en todo el espacio.
Un conductor es una equipotencial, por lo que en cualquier punto dentro de él la función
φ tendrá el mismo valor. Por lo tanto para r ∈ [a, 2a] la función V (r) valdrá un valor V0
constante.
La Ley de Gauss es ciega, sólo le importa la cantidad de carga encerrada dentro
de la superficie gaussiana que se este tomando (respetando la simetría del problema)
por lo que para r > 2a el campo eléctrico será el mismo si existiese o no el conductor.
Evidentemente pasará lo mismo para r < a .
Dadas las consideraciones anteriores y la simetría esférica, procedemos a calcular el campo eléctrico
en todo el espacio (para luego calcular el potencial).

Problemas Propuestos y Resueltos de Electromagnetismo

Solución 4.14

---

### Página 92

CAPÍTULO 4. CONDUCTORES
W

Q

a

Q

r

r

Figura 4.2: Campo Eléctrico para r < a

Figura 4.1: Campo Eléctrico para r > 2a

¨

2a

W

2a

Para r > 2a.

a

Q
~ = Q =⇒ E(r) · 4πr2 = Q =⇒ E(r)
~ dS
~
r̂
E(r)
=
ε0
ε0
4πε0 r2

Ω

Para a < r < 2a.
~
E(r)
=0
Para r < a.
¨

Qr
~ = qencerrada =⇒ E(r) · 4πr2 = Qr =⇒ E(r)
~ dS
~
E(r)
=
r̂
ε0
ε0 a
4πε0 a3

Ω

Luego el potencial estará dado por

Rodrigo Chi - Marzo 2017

Para r > 2a.

ˆ

ˆr
~ =−
~ dr
E(r)

V (r) =

∞

Γ

Q
Q
dr =
4πε0 r
4πε0 r

Para a ≤ r ≤ 2a. Dado que el potencial es continuo, tendrá el mismo valor que tiene en la
frontera para el caso anterior, es decir:
V (r) = V (2a) =

Q
8πε0 a

Para r < a.




ˆr

ˆ2a

ˆa
ˆr




Q
Qr
Q
Q(a2 − r2 )

=
V (r) = − E(r)dr = − 
dr
+
E(r)dr
+
dr
+
4πε0 r2
4πε0 a3 
8πε0 a
8πε0 a3


∞

∞
a
2a
|
{z
}
=0

---

### Página 93

CAPÍTULO 4. CONDUCTORES
Finalmente el gráfico estará dado por
f (r )
Q
4pe0 a

Q
8pe0 a

a

2a

r

Figura 4.3: Gráfico de la función V (r)

Solución 4.15

P X

Problemas Propuestos y Resueltos de Electromagnetismo

a) Usando la geometría del problema, se puede deducir que el campo eléctrico es de la forma
~ = E(z)ẑ. En particular cabe notar que como ρ(z) = ρ(−z) el campo eléctrico en
E
un punto z0 sobre el eje z apuntará en el sentido inverso en punto −z0 de modo que
~
~
~
|E(−z
0 )| = |E(z0 )| =⇒ E(−z0 ) = −E(z0 )ẑ (ie. existe una simetría del campo eléctrico
con respecto al plano xy). Para encontrar el valor del campo eléctrico es necesario usar la
ley de Gauss tomando un cilindro centrado en origen con tapas de área A. Luego

---

### Página 94

CAPÍTULO 4. CONDUCTORES
- Para |z0 | ≤ a

E(z0 )ẑ
A
z=a
z = z0
z = z0
z= a
A
E(z0 )ẑ

Figura 4.4: Superficie Gaussiana para |z| ≤ a

Usando ley de Gauss para calcular el campo eléctrico en punto z0 ∈ [−a, a]
¨
~ = qencerrada
~ · dS
E
ε0
Tapas
˚
E(z0 )ẑ · Aẑ + −E(z0 )ẑ · −Aẑ =
ρ(z)dV
ε0
2A · E(z0 ) =

A
ε0

Cilindro
ˆz0 

Rodrigo Chi - Marzo 2017

z−a
z+a
+ exp
δ
δ






dz

−z0



E(z0 ) =



ρ0 exp −

ρ0 

2ε0

ˆz0



exp −

z+a
dz +
δ


−z0

"

ˆz0




exp

z−a

dz 
δ


−z0


z + a z0

ρ0
z−a
=
+ δ exp
−δ exp −
2ε0
δ
δ
−z0





ρ0 δ
z0 + a
z0 − a
+ exp
=
− exp −
ε0
δ
δ





ρ0 δ
z0 + a
z0 − a
=−
− exp
exp −
ε0
δ
δ




 z0 #
−z0

~ 0 ) = E(z0 )ẑ para z0 ∈ [0, a] y E(z
~ 0 ) = −E(z0 )ẑ
Ahora se puede concluir que E(z
para z0 ∈ [−a, 0], pero dado que E(−z0 ) = −E(z0 ) , se resume que
~ 0 ) = − ρ0 δ exp − z0 + a − exp z0 − a
E(z
ε0
δ
δ










ẑ

---

### Página 95

CAPÍTULO 4. CONDUCTORES
- Para |z0 | > a
E(z0 )ẑ
A

z=a

z = z0

z= a
z = z0
A
E(z0 )ẑ

Figura 4.5: Superficie Gaussiana para |z| > a

Tapas

E(z0 ) =
2ε0

ˆa

z+a
z−a
ρ0 exp −
+ exp
δ
δ








ˆa

ρ0 

2ε0

exp −

"





ˆa

z+a
dz +
δ


exp


z+a a

ρ0
=
−δ exp −
2ε0
δ



ρ0 δ
2a
=
1 − exp −
ε0
δ
Por lo que se concluye que











z−a

dz 
δ


−a

−a

~ 0) =
E(z

dz

−a



=



z−a
+ δ exp
δ
−a

ρ0 δ
2a
1 − exp −
ε0
δ








ẑ







ρ0 δ
2a


1 − exp −
ẑ
 −

ε0

δ

z0 > a
z0 < −a

 a #
−a

Problemas Propuestos y Resueltos de Electromagnetismo

Análogo al cálculo anterior, se tiene que para un punto z0 fuera del bloque macizo se
tiene
¨
~ = qencerrada
~ · dS
E
ε0

---

### Página 96

CAPÍTULO 4. CONDUCTORES
a
b) La aproximación dice que δ
a por lo que se asumirá que → ∞. Para |z| > a, se tiene
δ
que:
ρ0 δ
2a
E(z0 ) =
1 − exp −
ε0
δ






≈

ρ0 δ
ε0

Por lo tanto

~ 0) =
E(z

ρ0 δ
ẑ
ε0












ρ0 δ


ẑ
 −

ε0

z0 > a
z0 < −a

Para el caso |z| < a se puede hacer de más de una forma, una es analizando la expresión
ρ0 δ
z0 + a
z0 − a
E(z0 ) =
− exp −
+ exp
ε0
δ
δ




 
a
ρ0 δ
z0
z0
exp −
=
− exp −
+ exp
ε0
δ
δ
δ










a
Se tiene que exp −
→ 0, por lo que E(z0 ) → 0. Sin embargo hay que tener cuidado
δ
 
z0
−
ya que cuando z0 → a (en las cercanías del borde), el valor de exp
se vuelve muy
δ
grande y anula el efecto anterior dejando E(z0 → a) constante (¡la aproximación provoca
que la función E(z0 ) crezca muy rápido en las cercanías de a− !).




El análisis también en válido para z0 → −a por simetría.

Rodrigo Chi - Marzo 2017

Otra forma mucho más claro para verlo es usar una aproximación según Taylor al primer
orden, es decir
z0 − a
ρ0 δ
z0 + a
− exp −
+ exp
E(z0 ) =
ε0
δ
δ









ρ0 δ
a
z0
a
z0
a
a
≈
− exp −
+ exp −
+ exp −
+ exp −
ε0
δ
δ
δ
δ
δ
δ


2ρ0 z0
a
≈
exp −
ε0
δ










Si examina la expresión, se sabe que el valor z0 está acotado por = a” por lotanto la exprea
sión no puede crecer infinitamente y no puede contrastar el hecho que exp −
→ 0.
δ
~ = 0 para z0 ∈ (−a, a).
Se concluye que E

---

### Página 97

CAPÍTULO 4. CONDUCTORES
Como ya se vio, los casos interesantes ocurren en los valores z0 = a o z0 = −a, en el
cual aparece una discontinuidad entre los valores de campo eléctrico. Dado los resultados
anteriores, podemos que concluir que el material se comporta como un bloque conductor,
~ = 0 y fuera de él se tiene un valor constante (debido a la carga en
dentro de él se tiene E
sus caras). El término ρ0 δ → σ corresponde a la densidad de carga superficial en las caras
del conductor. Las líneas de carga se representan en la Figura 4.6.
z

z=a
r(z)

y
z= a

Figura 4.6: Líneas de Campo perpendiculares al bloque (en azul).

c) Usando de referencia V (z = −a) = V0 se tiene que la expresión genérica para el potencial
eléctrico es
ˆz
V (z) − V (−a) = −

ˆz
E(z)dz =⇒ V (z) = −

−a

E(z)dz + V0

−a

Analizando por intervalos:
- −a ≤ z ≤ a

ˆz
V (z) = −
−a

- z>a

ˆa

V (z) = −
−a

E(z) dz + V0 = V0
| {z }

ˆz
E(z) dz −
| {z }

ˆz
E(z)dz + V0 = V0 −

a

a

ρ0 δ
ρ0 δ
dz = V0 −
(z − a)
ε0
ε0

Problemas Propuestos y Resueltos de Electromagnetismo

Las líneas de campo poseen esta forma debido a que siguen la dirección del campo eléctrico
(paralelo al eje z). Dentro del conductor no hay líneas debido a que no hay campo eléctrico.

---

### Página 98

CAPÍTULO 4. CONDUCTORES
- z < −a

ˆz
V (z) = −

ˆz
E(z)dz + V0 = V0 −

−a

−
−a

ρ0 δ
ρδ
dz = V0 +
(z + a)
ε0
ε0

Notar que el valor del potencial es simétrico con respecto al plano xy en el caso que
|z| > a, ya que se cumple que V (−z0 ) = V (z0 ). Lo anterior es intuitivo, ya que el
trabajo de mover una carga desde el origen hasta z0 será el mismo que del origen a
−z0 , todo debido a la simetría.
z

z=a
r(z)

y
z= a

Figura 4.7: Equipotenciales paralelas al plano xy (en rojo).

Rodrigo Chi - Marzo 2017

Las equipotenciales son las mostradas en la Figura 4.7, estas superficies son planos paralelos
al xy, ya que el potencial depende sólo del valor de la altura z.

Solución 4.16

P X

a) Se consideran los distintos casos según la distancia r desde el centro de la esfera interior.
~ < r < R1 )
- E(0
Dado que el cilindro interior es un conductor,
~ =0
E
~ 1 < r < R2 )
- E(R
Considerando la simetría del problema, se puede hacer uso de la Ley de Gauss:
¨
~ = Qenc
~ · dS
E
ε0
S

---

### Página 99

CAPÍTULO 4. CONDUCTORES
Nótese que no hay carga encerrada en el interior de un radio r < R2 , antes de la
densidad de carga. Luego se tiene:
¨
~ = 0 =⇒ E
~ · dS
~ =0
E
S

La densidad de carga sobre un conductor puede ser obtenida de
~ 1 ) = σ(r = R1 ) r̂ =⇒ σ(r = R1 ) = 0
E(R
ε0
~ 2 < r < R3 )
- E(R
Haciendo uso de la Ley de Gauss con un procedimiento análogo al anterior, se tendrá
que:
¨
~ = Qenc
~ · dS
E
ε0
S

ˆ2π ˆh

Erdθdz =
ε0

2πrhE =

ˆr ˆ2π ˆh
ρ0 rdrdθdz

R2 0 0
ρ0 π (r2 − R22 ) h

ε0
~ = ρ0 (r − R2 ) r̂
E
2rε0

S
2π
ˆ ˆh

Erdθdz =
ε0

~ =
E

ˆR3 ˆ2π ˆh
ρ0 rdrdθdz

R2 0 0
ρ0 (R32 − R22 )

2rε0

r̂

~ 4 ) = σ(r=R4 ) (−r̂) =⇒ σ(r = R4 ) = − ρ0 (R3 −R2 ) .
Por otro lado, E(R
ε0
2R4

~ 4 < r < R5 )
- E(R
Por tratarse del espacio interior entre conductores,
~ =0
E
~ 5 < r)
- E(R
Como en R5 se tiene un casquete conectado a tierra, para r ≥ R5 el campo se anulará.
Por lo cual σ(r = R5 ) = 0.

Problemas Propuestos y Resueltos de Electromagnetismo

~ 3 < r < R4 )
- E(R
Haciendo un cálculo similar al anterior, pero considerando que como r > R3 , la carga
encerrada se considerará siempre hasta R3 . Luego:
¨
~ = Qenc
~ · dS
E
ε0

---

### Página 100

CAPÍTULO 4. CONDUCTORES
b) La diferencia de potencial esta dada por la integral de camino del campo entre R1 y R4 :
ˆR4
~
~ · dr
E

∆V = −
R1

ˆR3
=−

ρ0 (r2 − R22 )
dr −
2rε0

R2

ρ0 (R32 − R22 )
dr
2rε0

R3



ρ0 

2ε0

ˆR3

ˆR3
rdr +

R2

R22
r

ˆR4
dr +

R2

R32 − R22
r



dr


R3

R3
R32 − R22
R4
+ R22 ln
+ (R32 − R22 ) ln
R2
R3




Rodrigo Chi - Marzo 2017

ρ0
=−
2ε0

ˆR4

E(R3 < r < R4 )dr
R3

R2

R1

=−

E(R2 < r < R3 )dr −

E(R1 < r < R2 )dr −

=−

ˆR4

ˆR3

ˆR2



!

---

### Página 101

CAPÍTULO 4. CONDUCTORES

IV.

Indicaciones Problemas Sin Solución

Indicación 4.6

P X

Recuerde que el campo eléctrico dentro de un material conductor siempre es nulo. Luego,
la carga inducida en el borde de la cavidad debe anular a lo que tiene adentro. La densidad
de carga sobre un conductor se distibuye siempre intentando acercase lo más posible a la
carga que la induce.
Para la superficie exterior de la esfera, la carga inducida en ese lugar no ve lo que tiene
adentro (efecto conocido como jaula de Faraday).

Indicación 4.7

P X

Puede determinar el campo eléctrico en todo el espacio y luego la energía electrostática
mediante alguna de las fórmulas de energía electrostática.

Indicación 4.9

P X

a

b

problema puede concluirse imponiendo que la carga se conserva, es decir Q1 +Q2 = Q01 +Q02 .
Para determina la capacidad, asuma cargas Q y −Q en las esferas. Con ese dato, determine
la diferencial de potencial entre ellas y concluya el problema.

Indicación 4.11

P X

Asuma una carga +Q sobre el conductor de radio R1 y −Q sobre el radio R3 por lo
cual puede determinar los campos eléctricos dentro de los condensadores. A partir de los
anterior, determine diferencia de potencial entre R1 y R3 . Recuerde que el cable que conecta
los conductores de radio R2 y R4 provoca que ambos estén a igual potencial.

Problemas Propuestos y Resueltos de Electromagnetismo

Imponga que Q01 y Q02 son las cargas finales de las esferas. El hecho que las dos esferas queden
´∞
´∞
~ = E
~ El
~ 1 · dl
~ 2 · dl).
conectadas por un cable provoca que estén al mismo potencial (ie. E

---

### Página 102

CAPÍTULO 4. CONDUCTORES
Indicación 4.13

P X

El cable R0 es lo suficientemente delgado para que pueda considerarlo como un cable infinito.

Rodrigo Chi - Marzo 2017

El problema apunta en poder determinar el campo eléctrico. Recuerde que en los conductores
sólo se acumula carga en su superficie.

---

### Página 103

CAPÍTULO 4. CONDUCTORES

V.

Respuestas
Problema

Respuestas

4.1

1 Q
a) F~ = − ∂U
∂z ẑ = − 2 ε0 A ẑ b)

P

4.2

λ
a) σ = − 2πR
 λ
2πε0 r r̂r̂ r ≤ R
~
b) E(r)
=
0r̂
r>R


λ
ln Rr
r≤R
− 2πε
c) V (r) =
r>R

P

4.3

b = 3a
4 entonces U =

P

4.4

Q
q = RQR
, Umin = 8πε0 (R
, V1 (R1 ) = V2 (R2 ) = 4πε0 (RQ1 +R2 )
1 +R2
1 +R2 )

P

4.5

VB − VA = 2V0 ln

P

Q
W = − 4C

c)

Q
∆V = 3C

27πε0 E02 a3

b
a



a) qint = −q, la densidad de carga interior es mayor en los puntos más cercanos a la
carga.
b) qext = −q, la densidad exterior es homogénea.
4.6

P

4.7

c) (i) qint = −q y la densidad de carga no cambia, por otro lado qext = q pero la
densidad de carga deja de ser homogénea (ii) qint = −q y la densidad de carga
no cambia, por otro lado qext = 4πRV0 y la densidad de carga es homogénea.
La conexión a la fuente carga a la esfera.

e
U = 8πε

n

5R1 + (R23 −R13 )1

h

R26



R1 − R2



− R23 (R22 − R12 ) +

R25 −R15

io

Problemas Propuestos y Resueltos de Electromagnetismo

P

---

### Página 104

CAPÍTULO 4. CONDUCTORES
Problema

Respuestas




 1 1V0 1 2 r̂
( c − b + a )r
~
a) E(r)
=



V0

r̂r̂
( 1c − 1b + a1 )r2

P

4.8

0<r<a
a≤r<b
b≤r<c
r≥c



 V0 1 1 1


V ( − + )

 0 1 c− 1 b+ 1 r
(c b a)
V (r) =
V0


( 1c − 1b + a1 )c



 1 V1 0 1
( c − b + a )r

0<r<a
a≤r<b
b≤r<c
r≥c

0 V0
0 V0
0 V0
σa = a2 1ε−
, σ = − b2 1ε−
y σc = c2 1ε−
( c 1b + a1 ) b
( c 1b + a1 )
( c 1b + a1 )


V0

−
<
r
<
a

a
b


( − + )


V0
 c Vb0 a 1 1 

r̂ a ≤ r < b
−b
−
+
r
~
)
(
c
b
a
( 1c − 1b + a1 ) r
V (r) =
b) E(r) =


b
≤
r
<
c




 0
r≥c

0<r<a
a≤r<b
b≤r<c
r≥c

0 V0
0 V0
σa = a2 1ε−
, σ = − b2 1ε−
y σc = 0
( c 1b + a1 ) b
( c 1b + a1 )

P

a
b
a) Qfinal
= a+b
(Q1 + Q2 ), Qfinal
= a+b
(Q1 + Q2 ), como b > a entonces Qfinal
> Qfinal

4.9

b) C = 1 − 1 +1 1 − 1
a

b

d−a

P

4.10

El potencial al interior de la burbuja es V = 4πεQ0 R , independiente si es o no esférica.

P

4.11

0L
C = ln(R12πε
R3 /R2 R4 )

P

Rodrigo Chi - Marzo 2017

d−b

4.12

Q
Q
, σc = 2πcL
, σd = 0
a) σa = 0, σb = 2πbL

 Q
c
 2πε0 L ln b  r < b
Q
b) V (r) =
ln rc
b≤r<c
 2πε0 L
r>c

c) V (c) − V (b) = 2πεQ0 L ln cb

a) λ = Ql
−Q
Q
b) σ1 = 2πR
; σ2 = 2πR
1L
2L

~ < R0 ) = E(R
~ 1 < r < R2 ) = 0; E(R
~ 0 < r < R1 ) = Q ρ̂ = E(r
~ > R2 )
c) E(r
2πρLε0

P

4.13

−Q
d) σ10 = 2πR
; σ20 = 0
1L

~ > R2 ) = 0, en el resto de las zonas el campo permanece igual.
e) E(r
−Q
f) V = 2πε
ln( R
R0 )
0L

Q
R1
g) C = 2πεR01L U = 4πε
ln( R
)
0L
ln( R )

h) C = C

---

### Página 105

CAPÍTULO 4. CONDUCTORES
Problema

P

4.14

Respuestas

V (r) =


Q
Q

 8πε0 a + 4πε0 a3 (a − r )



~ 0) =
a) E(z

P

4.15

~ 0) =
b) E(z

4.16








0<r<a
a ≤ r < 2a
r ≥ 2a




2a
ρ0 δ
1 − exp −
ẑ
ε0
δ






ρ0 δ
2a


1 − exp −
ẑ
 −
ε0
δ

ρ0 δ


ẑ z0 > a

 ε0

z0 > a

z0 < −a



ρ δ

 − 0 ẑ z0 < −a
ε0

V0
−a ≤ z ≤ a





V0 − ρε00δ (z − a) z > a
c) V (z) =





V0 + ρε00δ (z + a) z < −a

~
a) E(r)
=

P

Q
8πε0 a
Q
4πε0 r






 ρ0 (r2 −R22 ) r̂
2rε0

r < R2
R2 ≤ r ≤ R3

ρ0 (R3 −R2 )


r̂


 0 2rε0

R3 ≤ r ≤ R4
r > R4

Problemas Propuestos y Resueltos de Electromagnetismo

ρ0 (R32 −R22 )
, σ(r = R5 ) = 0
σ(r = R1 ) = 0, σ(r = R4 ) = −
2R4
 
 2 2
 
R3 −R2
ρ0
R3
R4
b) V (R4 ) − V (R1 ) = − 2ε
+
R
ln
+
(R
−
R
)
ln
R2
R3

---

### Página 106

Rodrigo Chi - Marzo 2017

CAPÍTULO 4. CONDUCTORES

---

### Página 107

Ecuación de Laplace y Poisson

I.

Resumen Teórico

Ecuación de Poisson y Laplace
La ecuación de Poisson puede ser obtenida juntando las ecuaciones 1.7 y 3.2, de modo que
∇2 V = −

ρ
ε0

(5.1)

En el caso particular de espacios donde ρ = 0 se tiene la Ecuación de Laplace
∇2 V = 0

(5.2)

Primer Teorema de la Unicidad del Potencial: = La solución de la Ecuación Laplace en un volumen
V está únicamente determinada si el potencial es conocido sobre la(s) superficie(s) que rodea(n)
el volumen”
Segundo Teorema de la Unicidad del Potencial: = El campo eléctrico está únicamente determinado
si da la carga total en cada conductor y el valor de la distribución de carga en las regiones entre
los conductores”

Método de las Imágenes
El método de las imágenes es una forma de resolver la ecuación de Laplace y encontrar el potencial
en todo un espacio. El método se basa en el Primer Teorema de Unicidad del Potencial, el
cual presenta que existe un único potencial V (x, y, z) que cumpla la ecuación de Laplace y las
condiciones de borde dadas. El método busca una situación = equivalente” en el cual se cumpla la

Problemas Propuestos y Resueltos de Electromagnetismo

Teoremas de Unicidad del Potencial

---

### Página 108

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
ecuación de Laplace y a su vez las condiciones de borde del problema original. Consecuencia del
teorema de unicidad, la solución V (x, y, z) del potencial será la misma. Casos típicos:
Carga puntual sobre un plano conductor conectado a tierra.
Carga puntual entre dos planos infinitos conectados a tierra que forman un ángulo π/n
radianes con n ∈ N.
Carga puntual en frente de una esfera conductora conectada a tierra, a un potencial fijo V0
o cargada con carga Q.
¡Tenga cuidado! No necesariamente debe ser una carga lo que se ponga en frente de las geometrías
anteriormente descritas, por ejemplo, un cable infinito frente un plano conductor infinito conectado
a tierra también puede ser resuelto por el método de las imágenes.

Método de Separación de Variables
El método de separación de variables se usa cuando el potencial posee una depende dos o más
variables. En particular, para el caso de dos variables en coordenadas cartesianas se puede asumir
que la solución de la Ecuación de Laplace es de la forma
V (x, y) = X(x)Y (y)

(5.3)

Rodrigo Chi - Marzo 2017

Es decir, es posible afirmar que el potencial V (x, y) que resuelve la solución de Laplace es el
producto de una función dependiente sólo de x y otra sólo de y. Al reemplazar la Ecuación 5.3
en 5.2 se puede llegar a que
1 d2 Y
1 d2 X
=
−
= −α2
(5.4)
X dx
Y dy
donde α ∈ R. A partir de lo anterior, la soluciones de X(x) e Y (y) están dadas por
X(x) = A cos αx + B sin αx

(5.5)

Y (y) = C cosh αy + D sinh αy

(5.6)

Donde los valores A, B, C, D y α pueden ser obtenidos a partir de las condiciones de borde del
problema respectivo.

Recomendaciones
La Ecuaciones de Poisson y Laplace son sumamente poderosas y reduce el problema físico
de la electrostática a una ecuación diferencial.
El método de las imágenes suele ser algo incompresible en primera instancia y requiere
tiempo para poder comprenderse a cabalidad. El método es poco intuitivo, por lo cual es
necesario que el estudio incluya todos los casos más básicos. La moraleja del método es:
todo lo que ocurra en una situación, también pasará en la otra equivalente.

---

### Página 109

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

II.

Problemas Propuestos
z

X S

#### Problema 5.1

Una lámina no conductora coincide con el plano xy.
Las únicas cargas en el sistema están sobre la lámina.
Se sabe que en el semiespacio z > 0 el potencial es
V (x, z) = V0 e−kz cos kx, donde V0 y k son constantes.
a) Verifique que este potencial satisface la ecuación de Laplace en el semiespacio z > 0.

y

b) Encuentre la ecuación para las líneas de campo
eléctrico
c) Encuentre la distribución de carga sobre la lámina.

x

X I

#### Problema 5.2

La parte medular de una memoria RAM y otros dispositivos semiconductores es la = juntura np”, que puede
modelarse con la distribución de carga bosquejada en
la figura, en que la linea punteada representa el plano
x = 0:





−ρ0

Material Tipo n

si − a < x < 0
si 0 < x < a
en el resto del espacio

r(x) = 0

a) Determine la diferencia de potencial entre el
seno de la zona n y el de la zona p (es decir,
entre un punto x1 < −a y otro x2 > a).
b) Si a = 300 nm y ρ0 = 1200 C/m3 , calcule
numéricamente el valor de la diferencia de potencial (considere ε0 ≈ 9 · 10−12 F/m).

Material Tipo p

r(x) 6= 0

x= a

r(x) = 0

x=a

Problemas Propuestos y Resueltos de Electromagnetismo

ρ(x) =




+ρ0

x

---

### Página 110

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
a

a

#### Problema 5.3

X I

Considere dos placas paralelas infinitas conectadas a
tierra separadas una distancia 2a, la mitad del volumen entre las placas se ha llenado con una densidad
de carga ρ(x) = ρ0ax mientras que la otra mitad se ha
dejado vacía. Usando la ecuación de Poisson y Laplace, determine el potencial en todos los puntos dentro
de las placas.

Rodrigo Chi - Marzo 2017

#### Problema 5.4

r(x)
x

X S

Considere una esfera maciza de radio a con carga
desconocida, la cual se encuentra totalmente inmersa en un fluido que posee una densidad volumétrica de carga con simetría radial dada por ρ(r) =
−ε0 k 2 V (r) (r > a) donde k es una constante, ε0
la permitividad del vacío y V (r) el potencial eléctrico.
Experimentalmente se ha determinado que el potencial en el borde de la esfera es V0 con respecto al
infinito (V (∞) = 0) y la distribución volumétrica de
carga dentro de la esfera es uniforme. Determine la
densidad de carga ρ(r) y el potencial eléctrico Φ(r)
en todo el espacio. Hint: Definir W = rV (r) puede
ser útil.

a

+

#### Problema 5.5

X S

V

Considere dos placas conductoras cuadradas de lado
a, las cuales forman un pequeño ángulo α. Las placas
están a una distancia d del vértice como se ilustra la
figura y se encuentran una diferencia de potencial V .
Determine la capacidad del sistema.

a
d

a

---

### Página 111

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

#### Problema 5.6

X S

R1

Considere dos condensadores formado por dos casquetes esféricos conductores concéntricos de radios
R1 ,R2 ,ρ1 ,ρ2 respectivamente. Cada conductor en su
polo sur tiene una pequeña perforación para conectar
el casquete inferior (ver figura). Si apropiadamente se
conecta cables a los casquetes exteriores y a los interiores, como se ilustra en la figura, encuentre usando
la ecuación de Laplace la capacitancia del condensador entre los puntos A y C.

#### Problema 5.7

R2

A
r1

C

r2

X S

Considere un plano conductor z = 0, conectado a
tierra y frente al cual se ha colocado una carga q en
el punto x = 0, y = 0, z = h.

Z
q

a) Calcule la densidad de carga sobre el plano. Exprese su resultado en función de la distancia del
origen a un punto cualquier sobre el plano.

Y

X

c) Calcule el trabajo que es necesario realizar para
llevar una carga q desde x = 0, y = 0, z = h
hasta x = 0, y = 0, z = 2h, en presencia del
plano conectado a tierra.

#### Problema 5.8

X S

+s

Considere un casquete esférico cargado de radio R y
con una densidad de carga superficial σ. Si el centro
del casquete esférico se sitúa a una distancia horizontal a y vertical b con respecto a un plano conductor
infinito doblado en 90◦ . Encuentre la densidad de carga σx y σy sobre los ejes y bosqueje su forma aproximada.

b

R

a

Problemas Propuestos y Resueltos de Electromagnetismo

b) Calcule la carga encerrada en un disco de radio
d dibujado sobre el plano conductor con centro en el origen. ¿Para qué valor de d la carga
encerrada pro el disco es − 2q ?.

h

---

### Página 112

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

#### Problema 5.9

X I

Considere una carga puntual q, la cual es colocada
en la bisectriz de dos conductores ideales planos que
forman un ángulo de 45◦ grados (ver figura). Si la
carga tiene una una distancia d a los conductores,
encuentre la forma del potencial electrostático entre
los conductores.

#### Problema 5.10

d
d

45o

X S

R

Una carga puntual q se ha puesto a una distancia d del
centro de una esfera maciza metálica. Si la esfera se
encuentra conectada a tierra, determine la densidad
de carga sobre la esfera y la carga total inducida en
ella.

#### Problema 5.11

d

Q

X S

R

Una carga puntual q se ha puesto a una distancia d
del centro de una esfera maciza metálica. Si la esfera
posee una carga neta Q, determine la fuerza que siente
la carga q.

q
d

X S

Considere una esfera metálica de radio R que se encuentra conectada a una fuente a potencial V0 . Frente
a ella se coloca un péndulo de largo ` atado a una muralla a distancia d del centro de la esfera. El péndulo
lleva en su extremo una carga puntual q de masa m
que forma un ángulo φ con respecto a la horizontal.
Despreciando todos los efectos de la gravedad.
a) Determine el módulo de la fuerza electrostática
que siente la carga.
b) Considere ahora que la fuente se apaga (V0 =
0). Determine la frecuencia de pequeñas oscilaciones del péndulo si es perturbado débilmente
con respecto a la horizontal.

q, m

R

`
f

V0

+

Rodrigo Chi - Marzo 2017

#### Problema 5.12

q

d

---

### Página 113

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
#### Problema 5.13

X I

En un túnel minero existe un cable que atraviesa toda
su longitud, a una distancia d del techo del túnel. El
túnel puede ser modelado como un cilindro infinito de
radio R, de modo que el cable se mantiene siempre
paralelo al eje imaginario del túnel. En cierto instante,
el cable adquiere una densidad de carga lineal +λ en
toda su extensión.

d
R
q

a) Encontrar una expresión para el potencial
V (r, θ) dentro del túnel, en términos de r y θ
(coordenadas polares).
b) Determinar la densidad de carga σ(θ) en la pared del túnel.
c) ¿Cuál es la carga total por unidad de longitud
inducida en la pared del túnel?
d) ¿Cuál es la fuerza por unidad de largo que siente
el cable?

X S

a

Considere una guía de onda, la cual es una tubería
metálica de sección rectangular de ancho a y alto b.
Las placa inferior y laterales están conectadas a tierra,
es decir, a potencial cero. La placa metálica superior
tiene una tensión periódica de período 2πn
(donde n
a
es un número entero), V (x, y = b) = V0 cos( 2πn
x),
a
V0 da cuenta de la intensidad de la tensión. Encuentre
la tensión al interior, V (x, y).

✓

2p
x
a

◆

b
y
x

Problemas Propuestos y Resueltos de Electromagnetismo

#### Problema 5.14

V = V0 cos

---

### Página 114

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
V = V0
+

#### Problema 5.15

X I

+

Se tiene una guía rectangular infinita de lados a y
b, compuesta por cuatro láminas planas conductoras.
Dos de ellas se conectan a tierra, mientras que en las
restantes existe un potencial contante de valor V0 , tal
como se indica en las Figuras.

V = V0

a) ¿Cuáles son las condiciones de borde del problema?

b

b) Calcule una expresión general para el potencial
entre las placas usando el método de separación
de variables. Muestre todos los casos posibles e
indique el caso que cumplen las CB. Realice el
cálculo considerando que cada lado actúa por
si solo y finalmente superponga las soluciones
encontradas.

V = V0

a

V =0

V =0

V = V0

Rodrigo Chi - Marzo 2017

#### Problema 5.16

X I

y

Usando el método de separación de variables, calcular
el potencial V (x, y) en el interior de un recinto plano
como el indicado en la Figura, con las siguientes conb
diciones de borde:
V (0, y) = 0;

V (x, 0) = 0;

∂V
= 0;
∂x x=a

∂V
= −E0
∂y y=b

a

x

---

### Página 115

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

III.

Soluciones

Solución 5.1

P X

a) Se debe verificar que el potencial V (x, z) = V0 e−kz cos kx, cumple la ecuación de Laplace.
En efecto,
∂ 2 V (x, z) ∂ 2 V (x, z)
+
∂x2
∂z 2
∂
∂
=
(−V0 e−kz k sin kx) + (−V0 ke−kz cos kx)
∂x
∂z
= (−V0 e−kz k 2 cos kx) + (V0 k 2 e−kz cos kx)
=0

∇2 V =

b) En primera instancia, el campo eléctrico para z > 0 es
~ = −∇V = V0 e−kz k sin kx · x̂ + V0 ke−kz cos kx · ẑ
E
Luego las líneas de campo están dadas por la solución de la siguiente EDO
Ez
cos kx
ln(| sin kx|)
dz
=
=
=⇒ z(x) =
+C
dx
Ex
sin kx
k
con C ∈ R.

donde E1n = −E2n = V0 k cos kx, se tiene que
σ = 2ε0 V0 k cos kx

Solución 5.4

P X

Consideremos inicialmente el caso r > a, por Poisson debe cumplirse que
∇2 V = −

ρ(r)
ε0

Problemas Propuestos y Resueltos de Electromagnetismo

c) Dado que el plano es no conductor, la líneas de campo deben ser simétricas con respecto
a él tanto para z > 0, como para z < 0. De este modo, el campo eléctrico generado por
la densidad superficial de carga sobre el plano debe ser simétrico con respecto al plano xy.
Luego, usando la condición de borde sobre la componente normal del campo eléctrico, es
decir
σ
En1 − En2 =
ε0

---

### Página 116

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
adicionalmente como ρ(r) = −ε0 k 2 V (r) y hay simetría esférica, entonces la ecuación anterior se
transforma en
!
1 ∂
2 ∂V
r
= k2V
r ∂r
∂r
Usando el cambio de variables a V (r) = r−1 W (r), la ecuación se transforma en
1 ∂
∂W (r)
r2 −r−2 W (r) + r−1
r ∂r
∂r

!!

∂
∂W (r)
= k r W =⇒
−W (r) + r
∂r
∂r
2 −1

!

= k 2 rW (r)

Volviendo a derivar nuevamente
−

∂W (r) ∂W (r)
∂ 2 W (r)
∂ 2 W (r)
+
+r
=
k
rW
(r)
=⇒
− k 2 W (r) = 0
∂r
∂r
∂r2
∂r2

La última ecuación diferencial tiene por solución W (r) = Aekr + Be−kr , donde A y B son
constantes por determinar. Devolviéndose con con el cambio de variables
V (r) = (Aekr + Be−kr )
r
Por condiciones de borde V (r −→ ∞) = 0, es decir, debe cumplirse que A = 0 (el potencial no
puede diverger en el infinito). Por otro lado V (a) = V0 , luego B = V0 aeka , por lo que el potencial
y la densidad de carga para r > a vale
V (r) =

V0 a k(a−r)
V0 a k(a−r)
e
=⇒ ρ(r) = −k 2 ε0
e
r
r

Rodrigo Chi - Marzo 2017

Para r < a existe una densidad de carga uniforme (o constante) la cual se denotará como ρ0 (por
determinar). El campo eléctrico dentro de una esfera de radio a, debe valer
¨
~ = Qenc =⇒ E(r) · 4πr2 = 4πr ρ0 =⇒ E
~ · dS
~ = ρ0 r r̂
E
ε0
3ε0
3ε0
Dado que no existen densidades de carga superficiales en r = a, el campo eléctrico debe ser
continuo en ese punto. De modo que se cumple que
ρ0 a
∂
=−
3ε0
∂r



V0 a k(a−r)
e
r



=⇒ ρ0 =
r=a

3ε0 V0 (ka + 1)
a2

Finalmente, el potencial para r < a estará dado por
ˆr
V (r) − V0 = −

V0 (ka + 1)r
V0 (ka + 1)
dr
=
−
a2
a2

a

=⇒ V (r) = V0 −

V0 (ka + 1)(r2 − a2 )
2a2

r 2 a2
−

!

---

### Página 117

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
Solución 5.5

P X

Solución 1:
Para encontrar la solución debe usarse la ecuación de Laplace. Se supone a priori que los efectos
de borde del condensador son nulos porque el ángulo α es pequeño (entre más separadas estén las
placas del condensador el campo eléctrico fuera del condensador deja de volverse despreciable).
Sea ϕ la función potencial entre las placas, en el espacio dentro del condensador se cumple la
ecuación de Laplace ∇2 ϕ = 0, donde ϕ(θ = 0) = 0 y ϕ(θ = α) = V . Por geometría del
problema, el potencial dentro de las placas debe ir aumentando desde θ = 0 hasta θ = α con una
dependencia única del ángulo (en coordenadas cilíndricas). Luego
∇2 ϕ =

1 ∂ 2ϕ
= 0 =⇒ ϕ(θ) = Aθ + B
r2 dθ2

donde A y B son constantes por determinar. Usando las condiciones de borde, se obtiene que
A = Vα y B = 0, por lo que
V
ϕ(θ) = θ
α
Por consiguiente, el campo eléctrico es
~ = −∇ϕ = − V θ̂
E
αr
conocido el campo eléctrico dentro de las placas, puede despejarse el valor de la densidad de carga
sobre la placa inferior como

borde

~ = 0) · ŷ = − ε0 V ŷ · ŷ = − ε0 V
· n̂ = ε0 E(θ
αx
αx

La carga total de una placa del condensador es
¨
Q=

!
ˆa ˆd+a
ε0 V
ε0 aV
d+a
σdS =
−
dxdy = −
ln
αx
α
d

d

Finalmente, la capacitancia es
|Q|
ε0 a
d+a
C=
=
ln
V
α
d

!

Solución 2:
El condensador de placas no paralelas puede descomponerse en pequeños condensadores de placas
paralelas en paralelo (Figura 5.1) . Cada uno de estos pequeños condensadores tiene un ancho

Problemas Propuestos y Resueltos de Electromagnetismo

~
σ = ε0 E

---

### Página 118

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
infinitesimal dx, un espesor a y una separación de placas x tan α, de esta forma cada pequeño
condensador tiene una capacidad
dC =

ε0 A
ε0 a · dx
=
d
x tan α

La capacitancia final del condensador de placas no paralelas va a ser la suma infinita de las
capacitancias de todos los pequeños condensadores. Finalmente, dado que α es pequeño tan α ≈
α, por lo que se concluye que
ˆ
C=

ˆa+d
dC =

ε0 a
d+a
ε0 a · dx
=
ln
xα
α
d

!

d

y

x tan a
a

x
a

d

dx

Rodrigo Chi - Marzo 2017

Figura 5.1: División Infinitesimal del Condensador.

Solución 5.6

P X

En primera instancia se puede notar que ambos condensadores siguen la misma geometría esférica,
por lo que bastaría calcular la capacitancia de uno y el resultado sería análogo para el otro. Además,
dada las conexiones de los condensadores, el circuito puede ser modelado de forma que se indica
en la Figura 5.2.
Los condensadores C1 (radios R1 y R2 ) y C2 (radios ρ1 y ρ2 ) están en paralelo, por lo que
capacitancia total entre entre A y C es CT = C1 + C2 .
La capacitancia de C1 (y también la de C2 ), al ser un condensador esférico, depende netamente
de su geometría. Para determinar la capacitancia de un condensador de este tipo debe suponerse
que una diferencia de potencial conocida entre las placas, sin perdida de generalidad se asume
que el potencial en el casquete interior es V0 y el exterior 0. Entre las placas se cumple la ecuación

---

### Página 119

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

C1

A

C
C2

Figura 5.2: Modelo equivalente de los condesadores
V =0
—2V = 0
V = V0
R1

R2

Figura 5.3: Capacitor Esférico C1

1 ∂
∂V
∇V = 2
r2
r ∂r
∂r

!

= 0 =⇒ V (r) = −

A
+B
r

Aplicando las condiciones de borde se obtiene que
V (r) =

V0 R1
V0 R1 R2
−
r(R2 − R1 ) R2 − R1

Luego, el campo eléctrico es
~ = −∇V =
E

V0 R1 R2
r̂
r (R2 − R1 )

Por lo que la densidad superficial de carga sobre el conductor interior es
~
σ = ε0 E

borde

Luego la capacitancia de C1 es
Q
C1 =
=
∆V
V0

· n̂ =

ε0 V0 R2
R1 (R2 − R1 )

¨
σdS =
Casquete

4πε0 R1 R2
R2 − R1

Problemas Propuestos y Resueltos de Electromagnetismo

de Laplace (ya que no hay densidades volumétricas de carga), es decir

---

### Página 120

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
Finalmente la capacitancia total está dada por
CT =

Solución 5.7

4πε0 R1 R2 4πε0 ρ1 ρ2
+
R2 − R1
ρ2 − ρ1

P X

Z
q
h

Y

X
Figura 5.4: Configuración Original
a) La carga imagen de este problema debe ir a una distancia h bajo el plano, tal como indica
la Figura 5.5.

Z
q

Rodrigo Chi - Marzo 2017

h

Y
h

X

q

Figura 5.5: Configuración Equivalente con Carga Imagen
Conocida esa configuración, se puede calcular el campo que habría justo en la superficie del
plano superponiendo el campo eléctrico producido por la carga más su carga imagen. Dado

---

### Página 121

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
que la carga q se encuentra en la posición (0, 0, h) y la carga imagen −q en (0, 0, −h) se
concluye que el campo eléctrico en un punto sobre el plano xy estará dado por:
"

xx̂ + y ŷ + (z + h)ẑ
q
xx̂ + y ŷ + (z − h)ẑ
~
E(x,
y, 0) =
3 −
4πε0 (x + y + (z − h) ) 2
(x2 + y 2 + (z + h)2 ) 2

#

~ = 0+ ) = σ ẑ se
Entonces, usando el hecho que en el borde del conductor se tiene que E(z
ε0
puede despejar el valor de σ:
σ(x, y) =

−qh

2π(x2 + y 2 + h2 ) 2

b) Conocido σ se integra en un circulo de radio d, para ello se usa el cambio de variables de
coordenadas cartesianas a coordenadas cilíndricas con r2 = x2 + y 2 y dxdy = rdrdθ
ˆ2π ˆd
Qdisco =

−qh

Luego si se desea Qdisco = −

2π(r2 + h2 ) 2

qh
rdrdθ = √ 2
−q
d + h2

q
se iguala con la expresión anterior, dando por resultado:

√
qh
q
√
=⇒
d
=
h
−
q
=
−
d2 + h2

q
−q 2z ẑ
~
=−
ẑ
E(z)
=
4πε0 (2z)
16πε0 z 2
Luego, la carga es movida por un agente externo desde z = h a z = 2h bajo la oposición
del campo eléctrico variable ya calculado, lo que matemáticamente resulta como
ˆ2h
∆V = V (2h) − V (h) = −

q
q
−
dz =
16πε0 z
16πε0

h

Finalmente como el trabajo está dado como W = q∆V
q2
W =
16πε0



q2
−
=
h 2h
32πε0 h





−
h 2h



Problemas Propuestos y Resueltos de Electromagnetismo

c) Para esta parte del problema se debe considerar que cuando la carga es movida una distancia
hacia arriba en la dirección +ẑ su carga imagen se mueve la misma distancia en la dirección
−ẑ. Por consiguiente, si la carga se pusiese en la posición ~r = z ẑ su carga imagen se
encontrará en ~r0 = −z ẑ, por lo que el campo eléctrico que sentirá la carga en ese punto
será:

---

### Página 122

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
Solución 5.8

P X

El problema nos presenta la siguiente configuración:

+s
R

b

a

Figura 5.6: Plano rectangular frente a una esfera

En primera instancia, y haciendo un análisis sólo en el plano xy, se tiene que ∇2 V = 0, V (x, 0) =
V (0, y) = 0 para x, y ≥ 0 y que V (||(x, y)|| → ∞) = 0. Ahora, el problema equivalente que
sigue las mismas condiciones anteriores es mostrado en la Figura 5.7.

s

+s
b

Rodrigo Chi - Marzo 2017

a

R

a

b
s

+s

Figura 5.7: Configuración de las Imágenes

En ambos casos tanto el potencial eléctrico como el campo eléctrico, tendrán el mismo valor para
los puntos que cumplan x, y ≥ 0. La configuración de imágenes están dada por 3 esferas de radio
R (una con carga +σ y dos con carga −σ) ubicadas como se muestra en la Figura 5.7. Para un
manto esférico de radio R y densidad σ se puede determinar el campo eléctrico generado por ley

---

### Página 123

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
de Gauss de la siguiente forma:
¨
~ = qenc =⇒ E(r) · 4πr2 = 4πR σ =⇒ E
~ · dS
~ = σR r̂
E
ε0
ε0
ε0 r 2
Dado que todas las esferas están descentradas, la forma general para determinar el campo que
generan será
~ = σR (~r − ~ri )
E
ε0 |~r − ~ri |3
dónde ~r es la posición donde se desea conocer el campo y ~ri es la posición donde se encuentra
el centro de la esfera. Para el problema se tiene que ~r1 = (a, b), ~r2 = (−a, b), ~r3 = (−a, −b)
y ~r4 = (a, −b), y que ~r = (x, y). Usando el principio de superposición se tiene que el valor del
campo es
(−1)i−1 (~r − ~ri )
σR2 X
~
E(x, y) =
ε0 i=1
||~r − ~ri ||3
σR
~
E(x,
y) =
ε0
+

(x − a, y − b)
((x − a)2 + (y − b)2 )

(x + a, y + b)

((x + a)2 + (y + b)2 ) 2

−

−

(x + a, y − b)

((x + a)2 + (y − b)2 ) 2
!

(x − a, y + b)

((x − a)2 + (y + b)2 ) 2

En particular en los ejes x e y se tiene que el campo eléctrico es, respectivamente:
σR2
~
E(x,
0) =
ε0

((x − a)2 + b2 ) 2
(−2a, 0)

(a2 + (y − b)2 ) 2

+

+

!

(0, 2b)

((x + a)2 + b2 ) 2

!

(2a, 0)

(a2 + (y + b)2 ) 2

~
Finalmente como en el borde de un conductor se cumple que σ = ε0 E

borde

(0, −2b)

(0, 2b)

!

(−2a, 0)

(2a, 0)

!

· n̂ , se tiene que

· (0, 1)
3 +
((x − a)2 + b2 ) 2
((x + a)2 + b2 ) 2
!
= 2bσR −
3 +
((x − a)2 + b2 ) 2
((x + a)2 + b2 ) 2

σx (x) = σR

· (1, 0)
3 +
(a2 + (y − b)2 ) 2
(a2 + (y + b)2 ) 2
!
= 2aσR −
3 +
(a2 + (y − b)2 ) 2
(a2 + (y + b)2 ) 2

σy (y) = σR

Las variaciones de densidad en los ejes se muestran a continuación (en ambos casos la funciones
σx y σy son siempre negativas y tiene sus mínimos en los valores de a y b, respectivamente).

Problemas Propuestos y Resueltos de Electromagnetismo

~ y) = σR
E(0,
ε0

(0, −2b)

---

### Página 124

sy (y)

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

+s
R

b

a

sx (x)

Figura 5.8: Variaciones de σx y σy en los ejes
Solución 5.10

P X

En este caso se debe usar el método de las imágenes para reemplazar la esfera conductora. Se
propone una carga q 0 a una distancia d0 , del centro de la esfera como imagen (ver Figura 5.9).
P
r
R

q0

q
d

r1

r2

q
z

Rodrigo Chi - Marzo 2017

d

Figura 5.9: Configuración Carga Imagen Esfera conectada a tierra
Para encontrar en valor de la carga imagen y del potencial, se determina previamente cual es el
valor del potencial que generan la superposición de estas dos cargas en el espacio:
V (r, θ) =
4πε0
Por teorema del coseno r1 =

√

V (r, θ) =
4πε0

q
q0
+
r1 r2

r2 + d2 − 2rd cos θ y r2 =

!

√
r2 + d02 − 2rd0 cos θ, por lo tanto

q
q0
√
√
+
r2 + d2 − 2rd cos θ
r2 + d02 − 2rd0 cos θ

!

---

### Página 125

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
Ahora tiene que considerarse que V (r = R, θ) = 0, ya que se supone que la esfera está conectada
a tierra.
√
q
R2 + d2 − 2Rd cos θ
= − 0 = cte.
V (R, θ) = 0 =⇒ √ 2
q
R + d − 2Rd cos θ
De aquí se deduce que, dado que el valor de las cargas es fijo, el lado izquierdo de la ecuación no
debe depender de θ ya que para cualquier ángulo el cuociente tiene un valor fijo. Se debe escoger
un valor de d0 de tal forma que la expresión de izquierda deje de depender de θ.
Reescribiendo

q

d( Rd + d − 2R cos θ)

q

d0 ( Rd0 + d0 − 2R cos θ)

= cte.

Para que la expresión anterior deje de depender de θ (es decir, poder simplificar el factor depen2
diente de cos θ), se puede elegir d0 = d (no sirve ya que implica q = −q 0 ) o d0 = Rd . Por lo que
se deduce que q 0 = − Rd q que es la carga efectiva de la esfera. La densidad de carga σ(θ), puede
ser determinada como
~
σ = ε0 E

borde

· n̂ = −ε0 ∇V |r=R · r̂ = −ε0

∂V
∂r r=R

Finalmente la densidad de carga es


σ(θ) =

R − Rd



q

4π(R2 + d2 − 2Rd cos θ) 2

Como último comentario, cabe mencionar que

R
σ(θ)R2 sin θdθdϕ = − q
d

Es decir, la carga total inducida en la esfera es igual a la de la carga imagen.
Nota: Existe más de un método para determinar el valor de las cargas imágenes en este tipo de
problema. Otra posibilidad, es haber igualado la expresión del potencial para dos ángulos distintos
(por ejemplo V (R, θ = 0) = V (R, θ = π) = 0) y despejar los valores q 0 y d0 .

Solución 5.11

P X

El problema puede ser analizado de la siguiente forma, suponga que la esfera estuvo inicialmente
descargada y conectada de tierra. Habrá sobre la esfera una carga q 0 (imagen) distribuida en forma
no homogénea sobre la superficie (debido a la presencia de q). Ahora, suponga que se desconecta
la esfera y se pone una carga Q − q 0 sobre el conductor (de modo que su carga total sea Q),
la carga puesta se distribuye homogéneamente sobre la superficie del conductor debido a que las

Problemas Propuestos y Resueltos de Electromagnetismo

ˆ2π ˆπ

---

### Página 126

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
fuerzas electrostáticas presentes ya han sido anuladas gracias a la carga q 0 (visto de otra forma,
esa carga es puesta sobre una superficie equipotencial, por que se repartirá en forma equilibrada
sobre ella). Por lo tanto, el potencial debido a Q − q 0 será el mismo que el debido a una carga
puntual de ese valor puesta en el origen, por lo que la configuración de cargas imágenes es la que
se propone en la Figura 5.10.

R

q0

q

q
x

d

d

Figura 5.10: Configuración Esfera Conductora Cargada
En conclusión, la esfera de radio R y carga Q es reemplazada por dos cargas imágenes q 0 y q 00
puestas en x = d0 y en x = 0, respectivamente. Los valores de cada uno de los términos anteriores
son
qR
qR
R2
q =− ,
q =Q+
,
d =
d
d
d
Luego, por ley de Coulomb la fuerza sobre la carga q es
q
F~ =
4πε0

Rodrigo Chi - Marzo 2017

Solución 5.12

q0
q 00
+
x̂
d2 (d − d0 )2
!

P X

a) Para resolver el problema debe colocarse dos cargas imágenes: una carga que anule el
potencial en el borde y otra que lo suba al borde de la esfera, de modo que se cumpla
∇2 V = 0, V (r = R) = V0 , V (r → ∞) = 0.
La primera carga imagen se coloca en la línea recta entre la carga y el centro de la esfera
(el objetivo de√esta carga es V (r = R) = 0. La distancia entre el centro de la esfera y la
carga es L = d2 + `2 − 2d` cos φ. Sea q 0 el valor de la carga imagen y L0 su distancia al
centro. Se debe cumplir que:
V (A) =

q0
q
+
=0
4πε0 (L + R) 4πε0 (L + R)

V (B) =

q0
q
+
=0
4πε0 (R − L0 ) 4πε0 (L − R)

---

### Página 127

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

L
L0

q, m

`

B

q0

f

A

Figura 5.11: Configuración Carga Imagen Esfera Cargada
Resolviendo para q 0 y L0 se obtiene:
R
R2
q0 = − q
L0 =
L
L
La segunda carga imagen debe elevar el potencial en r = R a V0 , luego se debe cumplir:
Vq00 (R) =

q 00
= V0 =⇒ q 00 = 4πε0 V0 R
4πε0 R

Con estas dos cargas q 0 y q 00 se cumplen la condiciones de borde (solución única). Finalmente
la fuerza es por Coulomb:
qq 0
qq 00
+ 2
(L − L0 )2
L

|F | =
4πε0

!

Fr̂
f
F

✓

L

Ft̂

q, m

`
f

✓

V0

+

d

Figura 5.12: DCL al péndulo
y tangencial al péndulo. Dado que se pide pequeñas oscilaciones, se usar la componente
tangencial (o normal) de la fuerza
|F⊥ | = |F | sin(φ + θ)

Problemas Propuestos y Resueltos de Electromagnetismo

qq
b) Si V0 = 0 =⇒ q 00 = 0, luego |F | = 4πε
0 2 . La fuerza se descompone en radial
0 (L−L )

---

### Página 128

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
Usando el teorema del Seno se tiene:
sin φ
sin θ
sin(π − (φ + θ))
sin(φ + θ)
d
=
=
=
=⇒ sin(φ + θ) = sin φ
L
`
d
d
L
Luego se tendrá:
d
sin φ
L
qq 0
d
=
sin φ
4πε0 (L − L0 )2 L

|F⊥ | = |F |

Reemplazando q 0 = − R
q y L0 = RL
L
|F⊥ | =

−q 2 Rd
−q 2 Rd
sin
φ
=
sin φ


4πε0 L − R2 2 L2
4πε0 (L2 − R2 )2
L

Ahora
m`φ̈ =

q 2 Rd
−q 2 Rd2
sin φ
sin
φ
=⇒
φ̈
+
=0
4πε0 (L − R )
4πε0 m` (L − R2 )2

Si φ ≈ 0, sin φ ≈ φ y cos φ ≈ 1. Con la última aproximación se tiene para el valor de L:
L2 = d2 + l2 − 2d` cos φ ≈ d2 + `2 − 2d` = (d − `)2 . Con lo que finalmente se concluye:
q 2 Rd
q
φ̈ +
φ = 0 =⇒ ω =
4πε0 m`((d − `) − R )
(d − `)2 − R2
|

Rodrigo Chi - Marzo 2017

Solución 5.14

{z

ω2

s

Rd
4πε0 m`

}

P X

En este caso se puede usar la ecuación de Laplace dentro de la guía de ondas ya que no existen densidades volumétricas de carga. Matemáticamente el problema puede ser planteado de la
siguiente forma
∂ 2V
∂ 2V
+
=0
∇2 V (x, y) =
∂x2
∂y 2
Sujeto a las siguientes condiciones de frontera
V (x, 0) = V (0, y) = V (a, y) = 0
2πx
V (x, b) = A cos
a




para 0 ≤ x ≤ a y 0 ≤ y ≤ b.
En este tipo de problemas se usa el método de separación de variables, es decir, se supone que el
potencial es de la forma V (x, y) = X(x)Y (y), lo cual implica que
∇2 V = Y

d2 X
d2 Y
1 d2 X
1 d2 Y
+
X
=
=⇒
=
−
dx2
dy 2
X dx2
Y dy 2

---

### Página 129

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
En este punto se puede notar que las variables están = separadas”(no hay dependencia entre ellas,
el lado izquierdo de la igualdad depende sólo de x y el derecho sólo de y). Por lo tanto, ambos
lados de la igualdad deben ser iguales a una misma constante, es decir
1 d2 X
1 d2 Y
=
−
=k
X dx2
Y dy 2
Ahora se debe analizar por casos:
k = 0 En este caso las soluciones son de la forma
X(x) = Ax + B
Y (y) = Cy + D
Usando las condiciones de borde
V (0, y) = B(Cy + D) = 0 =⇒ B = 0 o C = D = 0
En el primer caso C = D = 0, entonces Y (y) = 0 por lo que V (x, y) = 0. Dado que no
se buscan soluciones no triviales de V (x, y) ese caso no sirve. Luego V (x, y) = Ax(Cy+D).
Usando la segunda condición de borde
V (x, 0) = ADx = 0 =⇒ A = 0 o D = 0
Nuevamente si A = 0 se obtiene V (x, y) = 0 por lo que V (x, y) = ACxy.

V (a, y) = ACay = 0
De aquí es directo que A o C debe ser 0, por lo cual necesariamente se tendrá V (x, y) = 0.
Finalmente se deduce que este caso no arroja soluciones.
k > 0 Suponiendo que k = α2 se tiene que en este caso las soluciones son de la forma
X(x) = A cosh αx + B sinh αx
Y (y) = C cos αy + D sin αy
Usando las condiciones de borde y recordando que cosh 0 = 1 y sinh 0 = 0
V (0, y) = A(C cos αy + D sin αy) = 0 =⇒ A = 0 o C = D = 0
Nuevamente si C = D = 0, entonces Y (y) = 0 por lo que V (x, y) = 0. Luego
V (x, y) = B sinh αx(C cos αy + D sin αy)

Problemas Propuestos y Resueltos de Electromagnetismo

Aplicando la última condición de borde

---

### Página 130

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
Usando la segunda condición de borde
V (x, 0) = BC sinh αx = 0 =⇒ B = 0 o C = 0
Nuevamente si B = 0 se obtiene V (x, y) = 0 por lo que V (x, y) = BD sinh αx sin αy.
Aplicando la última condición de borde
V (a, y) = BD sinh αa sin αy = 0
Nuevamente se tiene que B o D deben ser 0, por lo cual necesariamente se tendrá V (x, y) =
0. Este caso tampoco arroja soluciones.
k < 0 En el último caso, suponiendo que k = −α2 se tiene que las soluciones son de la
forma
X(x) = A cos αx + B sin αx
Y (y) = C cosh αy + D sinh αy
Aplicando que
V (0, y) = A(C cosh αy + D sinh αy) = 0 =⇒ A = 0 o C = D = 0
Al igual que los casos anteriores, el valor válido es A = 0, de modo que
V (x, y) = B sin αx(C cosh αy + D sinh αy)
Ahora aplicando que
V (x, 0) = BC sin αx = 0 =⇒ B = 0 o C = 0
Nuevamente el valor válido es C = 0, por lo que la forma general de la solución es
Rodrigo Chi - Marzo 2017

V (x, y) = BD sin αx sinh αy
Aplicando la condición de borde
V (a, y) = BD sin αa sinh αy = 0 =⇒ αa = nπ =⇒ α =

nπ
, n∈N
a

Finalmente se deduce este caso si provoca soluciones y son una combinación lineal de la
forma




∞
X
nπ
nπ
V (x, y) =
Kn sin
x sinh
y
a
a
n=1
Para encontrar los términos Kn es necesario usar la última condición de borde
∞
X

nπ
nπb
V (x, b) =
Kn sin
x sinh
a
a
n=1




!

2πx
= V0 cos
a




---

### Página 131

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
Ahora se usará el hecho que
ˆa



sin


0

si n 6= m
si n = m

nπ
mπ
x sin
x dx = a

a
a






La expresión anterior debe multiplicarse a ambos lados por sin



mπ
x
a



∞
X
2π
mπ
nπ
mπ
nπb
V0 cos
x sin
x =
Kn sin
x sin
x sinh
a
a
a
a
a
n=1

















!

e integrando en 0 y a (y suponiendo que la integral entra sin problemas a la sumatoria)
ˆa

ˆa



∞
X

2π
mπ
V0 cos
x sin
x dx =
Kn 

a
a
n=1










nπ
nπb
mπ
sin
x sin
x dx
 sinh
a
a
a








!

La serie de la derecha tiene puros términos nulos excepto cuando n = m, por lo tanto
ˆa
V0

2π
mπ
a
mπb
cos
x sin
x dx = Km · sinh
a
a
a








!

Pero

ˆa



cos

2π
mπ
am(cos(πm) − 1)
x sin
x dx = −
∀n 6= 2
a
a
π(m2 − 4)






ˆa

2πx
a
2πx
2πx
cos
sen
=−
cos2
a
a
4π
a










a

=−


a  2
cos (2π) − cos2 (0) = 0
4π

Luego
Kn = −

2V0
sinh



nπb
a



n(cos(πn) − 1)
∀n 6= 2
π(n2 − 4)

Finalmente
V (x, y) = −

∞
X

2V0
n(cos(πn) − 1)
sin
π n=1,n6=2
(n2 − 4)





 sinh nπ y
nπ
a


x

a

sinh

nπ
b
a

Problemas Propuestos y Resueltos de Electromagnetismo

y para n = 2 se tiene:

---

### Página 132

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

IV.

Indicaciones Problemas Sin Solución

Indicación 5.2

P X

Plantee la Ecuación de Laplace/Poisson con el fin de encontrar en primera instancia el
campo eléctrico en todas las zonas.
Debido a las mismas ecuaciones o a la simetría del problema es fácil concluir que para
|x| > a el valor del campo eléctrico es nulo.
El campo eléctrico es continuo la x = −a, x = a y en x = 0. Una vez determinado el
campo debe integrarlo para encontrar la diferencia de potencial pedida.

Indicación 5.3

P X

Plantee la ecuación de Poisson para 0 < x < a y la ecuación de Laplace para a < x < 2a.
Una vez determinado la forma de estos potenciales imponga condiciones de borde, las cuales
están en x = 0 y x = 2a.
Adicionalmente, recuerde que el potencial es continuo en x = a y que la derivada del
potencial también es continua en x = a (ie. el campo eléctrico es continuo en la interfase).

Indicación 5.9

P X

Rodrigo Chi - Marzo 2017

En este caso debe poner siete cargas imágenes (ocho en total), alternando en signo cada
una. Estas ocho cargas forman un octógono de lado 2d.
Una vez identificadas las posiciones de las cargas y sus valores, usar la definición de potencial
eléctrico para cargas puntuales.

Indicación 5.13

P X

La carga imagen en este caso es un alambre paralelo al original. El alambre imagen está
sobre el eje y fuera del túnel.
Conocido el potencial, la densidad de carga puede ser encontrada en forma inmediata determinando la componente radial del campo eléctrico en r = R. En este caso se cumple
~
σ(θ) = ε0 E(R,
θ) · (−r̂) .

---

### Página 133

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
La densidad carga por unidad de largo inducida en el túnel es la misma que la posee el
alambre imagen.
~ = λEdl
~
La fuerza por unidad de largo puede ser obtenida a partir de dF~ = dq E

Indicación 5.15

P X

Se recomienda abordar este problema por superposición, es decir, como dos guías de ondas
donde tres lados están a potencial nulo y uno a V0 .
Para aplicar la superposición es cómodo darse dos sistemas de referencias y luego encontrar
su transformación para dejar todo en función de uno solo.

Indicación 5.16

P X

Este problema se resuelve de la misma forma el Problema 5.14, con la única precaución que
es necesario derivar para imponer la tercera condición de borde.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 134

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

V.

Respuestas
Problema

P

P

P

5.1

Respuestas
kx|)
b) z(x) = ln(| sin
+ C con C ∈ R.
k

c) σ = 2ε0 V0 k cos kx

5.2

a) ∆V = ρ0εa0

b) ∆V = 12 [V].

5.3

 ρ x x2
a
3 ( 2a − 3 ) 0 < x < a
V (x) =
ρ0 x
a < x < 2a
6 (x − 2a)
 3ε0 V0 (ka+1)

P

5.4

ρ(r) =

P

5.5

C = ε0da ln

P

5.6

4πε0 ρ1 ρ2
0 R1 R2
CT = 4πε
R2 −R1 + ρ2 −ρ1

a2

−k 2 ε0 Vr0 a ek(a−r)

a) σ(x, y) =

P

5.7

d+a
d

r≤a
V (r) =
r>a

(



−qh

2π(x2 +y 2 +h2 ) 2

√
− q, d = h 3
b) Qdisco = √dqh
2 +h2

q
c) W = 32πε
0h

Rodrigo Chi - Marzo 2017


σx (x) = 2bσR2 −

P

5.8


σy (y) = 2aσR2 −

3 +



((x−a)2 +b ) 2

((x+a)2 +b2 ) 2

3 +

(a2 +(y−b) ) 2



(a2 +(y+b)2 ) 2

−a )
V0 − V0 (ka+1)(r
2a2
V0 a k(a−r)
r e

r≤a
r>a

---

### Página 135

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON
Problema

P

5.9

Respuestas
(−1)i−1
q P8
V (x, y, z) = 4πε
r1 = (d cot( π8 ), d, 0),~r2 =
i=1 ||(x,y,z)−~
ri || , donde: ~
π
π
(d, d cot( 8 ), 0), ~r3 = (−d, d cot( 8 ), 0), ~r4 = (−d cot( π8 ), d, 0), ~r5 =
(−d cot( π8 ), −d, 0), ~r6 = (−d, −d cot( π8 ), 0), ~r7 = (d, −d cot( π8 ), 0), ~r8 =
(d cot( π8 ), −d, 0) y x ≥ y > 0.

R− Rd

P

5.10

σ(θ) =

P

5.11

q
F~ = 4πε

5.12

q

4π(R2 +d2 −2Rd cos θ) 2

 00

q
q0
d2 + (d−d0 )2



, qind = − R
dq

qR
R
x̂ donde q 0 = − qR
d , q =Q+ d , d = d


p
qq 0
qq 00
+
, L = d2 + `2 − 2d` cos φ y L0 = RL
(L − L )
L
r
q
Rd
b) ω =
(d − `)2 − R2 4πε0 m`
a) |F | =

P



4πε0



λ
ln
a) V (r, θ) = 4πε





r 2 +h2 −2rh sin θ
r 2 +(R−d)2 −2r(R−d) sin θ

R
donde h = R−d

P

5.13

(2R−d)
b) σ(θ) = − 2πR(Rλ(d
2 +d2 −2dR sin θ)

c) λinducido = −λ

(R−d)
d) F~ = − λ2πε
2 ŷ
0d

P∞

5.14

V (x, y) = − 2Vπ0

P

5.15

V (x, y) = Vπ0

P∞

P

5.16

V (x, y) = −

P∞

n=1,n6=2

n(cos(πn)−1)
sin
(n2 −4)

(1+(−1)n+1
n=1 n senh(nπb/a)



sen

nπx
a

 sinh( nπ
a y)
sinh( nπ
a b)

nπ
a x



senh

nπy
a



+ sen



nπ(a−x)
a

π(2n+1)
8aE0
n=0 (2n+1)2 π 2 cosh(αb) sin(αx) sinh(αy), α =
2a



senh



nπ(b−y)
a



Problemas Propuestos y Resueltos de Electromagnetismo

P

---

### Página 136

Rodrigo Chi - Marzo 2017

CAPÍTULO 5. ECUACIÓN DE LAPLACE Y POISSON

---

### Página 137

Dipolo Eléctrico

I.

Resumen Teórico

Momento Dipolar
El dipolo eléctrico es una distribución de carga que puede ser continua o discreta. El caso más
básico de un dipolo eléctrico son dos cargas puntuales +q y −q separadas una distancia d, el cual
se le asocia un vector p~ llamado momento dipolar y se define como
p~ = qdt̂

(6.1)

donde t̂ es el vector unitario del eje que pasa por las dos cargas. t̂ apunta de la carga negativa a
la positiva.

p~ =

N
X

qi~ri

(6.2)

dq(~r 0 )~r 0

(6.3)

i=1

y en configuraciones continuas

ˆ
p~ =

Potencial y Campo Dipolar
El potencial debido a un momento dipolar está dado por
V (~r) =

p~ · ~r
4πε0 r3

(6.4)

Mientras que el campo eléctrico está dado por la expresión
~ =
E
4πε0 r3

!

3(~p · ~r)~r
− p~
r2

(6.5)

Problemas Propuestos y Resueltos de Electromagnetismo

Para distribuciones más complejas, el momento dipolar puede ser determinado en configuraciones
discretas como

---

### Página 138

CAPÍTULO 6. DIPOLO ELÉCTRICO

Torque y Energía de un Dipolo
~ experimenta un torque el cual tiende
Un dipolo p~ bajo la influencia de un campo eléctrico E
alinearlo con el campo. El torque está dado por
~
~τ = p~ × E

(6.6)

Por otro lado, la energía que posee un dipolo para mantener su posición bajo el mismo campo
eléctrico es
~
U = −~p · E
(6.7)

Recomendaciones

Rodrigo Chi - Marzo 2017

La idea del dipolo eléctrico es poder determinar como se comporta (en una primera aproximación) el potencial y campo eléctrico que genera una distribución de carga para puntos
muy lejanos a ella. Todas las distribuciones de carga tienen asociado un momento dipolar
que en algunos casos podría ser nulo.

---

### Página 139

CAPÍTULO 6. DIPOLO ELÉCTRICO

II.

Problemas Propuestos

#### Problema 6.1

X I

z

Considere dos esferas de radio b y densidades de carga
ρ0 y −ρ0 , las cuales están dispuestas en el eje z, a una
distancia 2a entre ellas, según se muestra en la figura.
Se pide:

2b

a) Estimar el potencial en el punto (0, L, 0), suponiendo L
a, b

r0
2a

c) Calcule el trabajo necesario para llevar la carga
desde la posición (0, L, 0) a (L, 0, 0).

#### Problema 6.2

y

L

b) Si se ubica una carga q en la posición (0, L, 0),
estime la fuerza sobre la carga.

r0
x

X S

Considere un aro de radio R sobre el plano xy, el cual
tiene una de sus mitades con una densidad lineal de
carga uniforme λ (y > 0), y la otra con la densidad
opuesta −λ (y < 0), tal como se muestra en la Figura.

z

b) Determine el valor del campo eléctrico en el
plano xz usando la aproximación del campo lejano del punto anterior. ¿Es consistente este resultado con el valor obtenido para el potencial
en dicho plano?.
c) En general, o sea no necesariamente lejos del
aro, ¿Cuál es el valor del potencial en el plano
xz?

l

x

R

l
y

Problemas Propuestos y Resueltos de Electromagnetismo

a) Calcule el momento dipolar del aro y potencial
electrostático en la aproximación del campo lejano. ¿Cuál es el valor del potencial en el plano
xz?.

---

### Página 140

CAPÍTULO 6. DIPOLO ELÉCTRICO
#### Problema 6.3

X S

Un dipolo está compuesto por dos cargas opuestas.
Para modelar un dipolo considere dos esferas macizas
de radios R, de densidad de carga constante respectivamente ρ0 y −ρ0 , las cuales están conectadas en un
punto (ver figura).

r0

r0
R
z

a) Encuentre el campo eléctrico en todo el espacio, use como origen el punto de contacto entre
ambas esferas.
b) Para distancias muy lejanas, ¿De que forma decae el campo eléctrico?.

#### Problema 6.4

P

X S

Considere dos cables infinitos paralelos con densidad
de carga longitudinal λ y −λ separados una distancia
`
r, tal como se ilustra en la Figura. Encuentre el
~ θ) y el potencial eléctrico V (r, θ)
campo eléctrico E(r,
a una distancia r
`, en el límite ` → 0, λ → ∞ y
λ` → Q.

Rodrigo Chi - Marzo 2017

#### Problema 6.5

r
l

l

q

`

X I

Considere una barra de largo 2L, la cual se encuentra
sobre el eje x desde x = −L hasta x = L. La barra
posee una densidad de carga λ(x) = 56 αx3 donde α
es una constante y una masa M distribuida uniformemente en su largo. En el espacio donde se encuentre la
~ = E0 x̂.
barra existe un campo eléctrico constante E
a) Determine el momento dipolar de la barra.
b) Si la barra puede rotar con respecto a su centro,
determine la frecuencia con que oscilará la barra
si es perturbada débilmente de su posición de
equilibrio.

y

l (x)
L

L
~E

x

---

### Página 141

CAPÍTULO 6. DIPOLO ELÉCTRICO
#### Problema 6.6

X S

Se ha encontrado un asteroide esférico de masa M
y radio R cargado con una distribución superficial de
carga σ(θ) = σ0 cos θ. Con el objeto de estudiar el asteroide, se ha enviado una sonda espacial cuya trayectoria de acercamiento se encuentra en el plano θ = π2 ,
según muestra la Figura.

z

Asteroide

a) Determine el momento dipolar del asteroide.
b) Estime el campo eléctrico que afectará a la sonda, si ésta se encuentra muy alejada del asteroide.
c) Si la sonda puede modelarse como una carga
puntual Q, determine el trabajo que debe realizar para poder estar una distancia L
R
del centro de asteroide. Considere que la sonda
comienza su viaje en el infinito.

#### Problema 6.7

y
x

s (q ) = s0 cos q
Sonda

z

X S

~p
z0

x

X I

Considere un plano conductor infinito conectado a tierra coincidente con el plano xy. Una barra de largo L
yace a lo largo del eje z, de tal forma su extremo inferior se encuentra muy cercano al origen sin tocar
el plano (ver figura). Si la densidad de carga lineal
de la barra es λ(z) = αz, donde α es una constate,
determine:
a) La densidad de carga superficial σ sobre el plano
conductor.
b) El potencial electrostático para puntos muy lejanos del plano, mostrando claramente los términos monopolar y dipolar.

z

L

l (z)
y

x

Problemas Propuestos y Resueltos de Electromagnetismo

Un dipolo de momento dipolar p~ = px̂ está colocado a una distancia z0 de un plano conductor infinito
conectado a tierra tal como indica la Figura. Determinar el potencial eléctrico en cualquier punto (x, y, z)
del espacio y la densidad superficial de carga inducida
sobre un punto del plano conductor.

#### Problema 6.8

q R

---

### Página 142

CAPÍTULO 6. DIPOLO ELÉCTRICO

#### Problema 6.9

X I

r1

En cierto lugar del espacio existen dos planetas de
igual masa M y radio R alejados una distancia d
R.
Debido a los minerales que componen los asteroides
estos adquieren una densidad volumétrica de carga
dada por
(

ρ1 (θ) = ρ2 (θ) =

~v

q

R

m

d

ρ0 0 < θ < π2
−ρ0 π2 < θ < π

Rodrigo Chi - Marzo 2017

Considere que ambos planetas comparten su eje polar
(ver Figura). Un asteroide de masa m
M choca
con uno de los planetas provocando que este invierta
sus polos. ¿A qué velocidad chocó el astoroide para
lograr ese efecto?. Desprecie los efectos gravitaciones
por ser mucho menores que los electrostáticos.

r2

q

R

---

### Página 143

CAPÍTULO 6. DIPOLO ELÉCTRICO

III.

Soluciones

Solución 6.2

P X

El momento dipolar está dado por

ˆ
~r 0 dq

p~ =
dónde ~r 0 = Rr̂ y dq = Rλ(ϕ)dϕ, ϕ ∈ [0, 2π]
ˆ2π

ˆ2π
R2 λ(ϕ)(cos ϕx̂ + sin ϕŷ)dϕ

Rr̂ · Rλ(ϕ)dϕ =

p~ =

En x̂:
ˆ2π
R2 λ(ϕ)(cos ϕdϕ

|p~x | =

ˆπ
= R2

ˆ2π
λ0 cos ϕdϕ + R2

−λ0 cos ϕdϕ
π

=0
En ŷ:
R2 λ(ϕ) sin ϕdϕ

|p~y | =

ˆπ
=R

ˆ2π
λ0 sin ϕdϕ + R

−λ0 sin ϕdϕ
π

= 4R λ0
Con lo anterior se concluye
p~ = |p~x |x̂ + |p~y |ŷ = 4R2 λ0 ŷ
La aproximación del potencial en puntos lejanos es:
V (r) =

p~ · r̂
· 2
4πε0 r

donde p~ = 4R2 λ0 ŷ, r̂ = (sin θ cos ϕ, sin θ sin ϕ, cos θ) y r =
V (r) =

√ 2
x + y2 + z2

4R2 λ0
sin θ sin ϕ
· √ 2
4πε0 ( x + y 2 + z 2 )2

Problemas Propuestos y Resueltos de Electromagnetismo

ˆ2π

---

### Página 144

CAPÍTULO 6. DIPOLO ELÉCTRICO
Pero

y
y
=⇒ sin ϕ = √ 2
x
x + y2

tan ϕ =

√ 2
√ 2
x + y2
x + y2
=⇒ sin θ = √ 2
tan θ =
z
x + y2 + z2
Luego
V (x, y, z) =

4λ0 R2
y
λ0 R 2 y
·
=
4πε0 (x2 + y 2 + z 2 ) 23
πε0 (x2 + y 2 + z 2 ) 2

En el plano xz se tiene y = 0
=⇒ V (x, z) = 0
Usando el potencial anterior se calcula el campo
~ = −∇V
E
~ = − ∂V x̂ − ∂V ŷ − ∂V ẑ
E
∂x
∂y
∂z
!
λ0 R
3xy
x2 − 2y 2 + z 2
3xy
=
x̂ −
5 ŷ +
5 ẑ
πε0 (x2 + y 2 + z 2 ) 52
(x2 + y 2 + z 2 ) 2
(x2 + y 2 + z 2 ) 2
En el plano P , y = 0
λ0 R2 x2 + z 2
−λ0 R2
~
E(x,
z) = −
5 ŷ =
3 ŷ
πε0 (x2 + z 2 ) 2
πε0 (x2 + z 2 ) 2
El campo es independiente de y, por ende el campo eléctrico es constante para un y fijo, lo cual
implica que para cualquier plano paralelo a xz es una equipotencial. El potencial para puntos no
necesariamente lejanos es:
ˆ
dq
V (~r) =
4πε0
|~r − ~r 0 |

Rodrigo Chi - Marzo 2017

Donde dq = λ(ϕ)Rdϕ, ~r = xx̂ + z ẑ y ~r 0 = Rr̂
R
V (x, z) =
4πε0

ˆ2π

λ(ϕ)dϕ
|(x − R cos ϕ)x̂ + R sin ϕŷ + z ẑ|





ˆπ


ˆ2π





q
− q

(x − R cos ϕ) + R sin ϕ + z
(x − R cos ϕ) + R sin ϕ + z 
0

π
{z
}
|
{z
} |

λ0 R 

=
4πε0 


dϕ

I2

I1

Analizando las integrales por separado:
ˆπ
I1 =

dϕ
q

dϕ

(x − R cos ϕ)2 + R2 sin2 ϕ + z 2

---

### Página 145

CAPÍTULO 6. DIPOLO ELÉCTRICO
al usar el cambio de variable α = ϕ − π, dα = dϕ
ˆ0
I1 =

dα
q

−π

Por otro lado

(x + R cos α)2 + R2 sin2 α + z 2

ˆ2π
I2 =

dϕ
q

π

(x − R cos ϕ)2 + R2 sin2 ϕ + z 2

al usar el cambio de variable α = π − ϕ, dα = −dϕ
ˆ−π
I2 = −

ˆ0

dα
q

=

(x + R cos α)2 + R2 sin α + z 2

dα
q

−π

(x + R cos α)2 + R2 sin2 α + z 2

= I1

Con lo que se concluye
V (x, z) = 0

Solución 6.3

P X

a
r

a
r

r

r

Figura 6.1: Casos de cálculo de campo eléctrico para r < a y r ≥ a
Por ley de Gauss r < a (puntos dentro de la esfera):
¨
˚
q
ρr
ρ~r
~
~
~
E · dS =
=
ρdV =⇒ E(r)4πr2 = πr3 ρ =⇒ E(r)
=
r̂ =
ε0
ε0
3ε0
3ε0

Problemas Propuestos y Resueltos de Electromagnetismo

a) Es importante notar que el problema carece de simetría esférica (ie. no puede suponerse que
~ = E(r)r̂), por lo tanto es imposible determinar el campo eléctrico
el campo es de la forma E
usando directamente ley de Gauss. Para abordar el problema es necesario primero analizar
el campo eléctrico que genera una esfera por sí sola (independiente del problema actual),
para ello se calculará el campo a una esfera de radio a y densidad de carga homogénea ρ .

---

### Página 146

CAPÍTULO 6. DIPOLO ELÉCTRICO
y para r ≥ a (puntos fuera de la esfera)
¨

~ = q = 1
~ · dS
E
ε0
ε0

˚

ρa3
ρa3~r
~
ρdV =⇒ E(r)4πr2 = πa3 ρ =⇒ E(r)
=
r̂
=
3ε0 r2
3ε0 |~r|3

En ambos resultados se ha dejado en función del vector posición ~r medido desde el centro
de la esfera, de modo que sea más fácil determinar el valor del campo eléctrico en un punto
para un problema que se tenga más de un sistema de referencia. Volviendo al problema
original, si se desea calcular el campo eléctrico en punto P arbitrario, existen 3 posibilidades
en el espacio:
- Caso 1: Fuera de ambas esferas

- Caso 2: Dentro de la esfera positiva y fuera de la esfera negativa
- Caso 3: Dentro de la esfera negativa y fuera de la esfera positiva
Para cada uno de estos casos, cada esfera provoca un campo eléctrico en el punto P , por
lo cual hay que usar el principio de superposición basándose en los resultados ya obtenidos
para una esfera cualquiera.
- Caso 1
Fuera de ambas esferas se tiene la siguiente configuración que se muestra en la Figura
6.1.

P

Rodrigo Chi - Marzo 2017

~r

~r

O

~r+

z

O+

O

Figura 6.2: Campo Eléctrico para un punto fuera de ambas esferas
En este caso se tiene que el campo eléctrico en el punto P es:

~ ) = ρ0 R ~r+ − ρ0 R ~r−
E(P
3ε0 |~r+ |3 3ε0 |~r− |3

---

### Página 147

CAPÍTULO 6. DIPOLO ELÉCTRICO
Notando además que ~r+ = ~r − Rẑ y ~r− = ~r + Rẑ por lo que
~ ) = ρ0 R
E(P
3ε0

~r − Rẑ
~r + Rẑ
−
|~r − Rẑ|3 |~r + Rẑ|3

!

- Caso 2
De forma parecida al caso anterior se toma un punto dentro de la esfera positiva y
fuera de la negativa, lo que resulta como

~ ) = ρ0~r+ − ρ0 R ~r−
E(P
3ε0
3ε0 |~r− |3
Luego
!

R3
~ ) = ρ0 (~r − Rẑ) −
(~r + Rẑ)
E(P
3ε0
|~r + Rẑ|3

- Caso 3
Finalmente el último caso está dado por un punto dentro de la esfera negativa y fuera
de la positiva, es decir
~ ) = ρ0 R ~r+ − ρ0~r−
E(P
3ε0 |~r+ |3
3ε0
de modo que
~ ) = ρ0
E(P
3ε0

!

R3
(~r + Rẑ) − (~r + Rẑ)
|~r − Rẑ|3

b) En este caso hay que hacer un análisis para distancias mucho más grandes de R. Para ello
se debe hacer previamente una aproximación según Taylor de los términos que componen
la expresión. Es decir,
|~r ± Rẑ|

− 23

= (|~r| + R ± 2R~r · ẑ)
≈ 3 1−
|~r|

2R~r · ẑ
R2
= 3 1+ 2 ±
|~r|
|~r|
|~r|2

R2
2R~r · ẑ
±
|~r|
|~r|2

!− 3

!!

Dado que se está estudiando el caso |~r|
R se obtiene que el segundo término de la
expresión puede ser ignorado (R2 /|~r|2 → 0). Por lo tanto
"

~ = ρ0 R (~r − Rẑ) 1 + 3R~r · ẑ
E
3ε0
|~r|3
|~r|5

!

3R~r · ẑ
− (~r + Rẑ)
−
|~r|
|~r|5

!#

Manejando algebraicamente la expresión y volviendo a hacer la aproximación anterior, se
llega a
!
!
ρ0 R 3
2Rẑ 6R(~r · ẑ)
ρ0 R3
2Rẑ 6R(r̂ · ẑ)
~
E=
− 3 +
~r =
− 3 +
r̂
3ε0
|~r|
|~r|5
3ε0
|~r|
|~r|3
Por lo que el campo eléctrico desciende como 1/r3 para distancias muy grandes con respecto
al radio de las esferas.

Problemas Propuestos y Resueltos de Electromagnetismo

−3

---

### Página 148

CAPÍTULO 6. DIPOLO ELÉCTRICO
Solución 6.4

P X

En primera instancia, hay que determinar el campo eléctrico y el potencial que genera un cable
infinito con densidad lineal λ en el espacio. Suponiendo que el cable tiene un largo L, se toma
una superficie Gaussiana cilíndrica de radio r alrededor de él (Figura 6.3). Por ley de Gauss se

L
l

r
~E(r)
Figura 6.3: Superficie Gaussiana para determinación del campo eléctrico de un alambre.
tiene

¨

~ = Qenc =⇒ E(r) · 2πrL = λL =⇒ E
~ · dS
~ = λ r̂
E
ε0
ε0
2πε0 r

Ahora dado que
~ = −∇V = − ∂V r̂ =⇒ V (r) = − λ ln r
E
∂r
2πε0
r0
Donde r0 es una constante arbitraria la cual se usa como referencia. Llevando este resultado al




P

Rodrigo Chi - Marzo 2017

r+

r
q

`

+l

l

Figura 6.4: Posición del Punto P con respecto a los cables
problema, se obtiene por superposición que el potencial en un punto cualquiera del espacio es
λ
r
ln
2πε0
r0



|

}



V =

{z

Potencial Cable Negativo

λ
r+
−
ln
2πε0
r0


|

{z



λ
r
=
ln
2πε0
r+

!

}

Potencial Cable Positivo

Por comodidad se ha fijado la misma referencia r0 para ambos cables. Por el teorema del coseno,
se tiene además que
r+
= r2 + `2 + 2r` cos θ

---

### Página 149

CAPÍTULO 6. DIPOLO ELÉCTRICO
Por lo tanto
r2
λ
V (r, θ) = −
ln +2
4πε0
r

!



`
λ
ln 1 +
=−
4πε0
r

!2



`
+ 2 cos θ
r

Dado que se desea analizar para r
`, se puede usar un desarrollo de Taylor entorno a 0 de la
función f (ε) = ln(1 + ε) donde ε = r` :
ln(1 + ε) = ε −

ε2 ε3
+ + ...

Despreciando todos los términos de orden superior, la expresión del potencial puede ser aproximada
a
Q cos θ
λ` cos θ
=−
V (r, θ) ≈ −
2πε0 r
2πε0 r
Finalmente el campo vale
~ = −∇V = −
E

Solución 6.6

Q
(cos θr̂ + sin θθ̂)
2πε0 r2

P X

a) El momento dipolar del asteroide puede ser determinado como
¨
σ(θ)R2 sin θdθdϕ·Rr̂ = σ0 R3

cos θ sin θdθdϕ(sin θ cos ϕx̂+sin θ sin ϕŷ+cos θẑ)

Por asuntos de simetría las componentes en x e y se anulan. La única componente que
aporta al momento dipolar es z , luego
ˆπ

ˆ2π

p~ = σ0 R ẑ

cos θ sin θdθ

4π
σ0 R3 ẑ
dϕ = σ0 R3 ẑ · − (cos3 π − cos3 0) =

b) El campo eléctrico que genera un dipolo está dado por
~ =
E
4πε0 r3

!

3(~p · ~r)~r
− p~
r2

Dado que la sonda se acerca sobre el plano definido por θ = π2 este coincide con el plano
xy, se define entonces ρ como la distancia del centro del asteroide a la sonda. Por lo tanto
~ =
E
4πε0 ρ3

3( 4π
σ R3 ẑ · ρρ̂)ρρ̂ 4π
σ0 R 3
3 0
−
σ
R
ẑ
=
−
ẑ
ρ2
3ε0 ρ3
!

Problemas Propuestos y Resueltos de Electromagnetismo

p~ =

ˆ2π ˆπ

---

### Página 150

CAPÍTULO 6. DIPOLO ELÉCTRICO
c) Finalmente, para encontrar el trabajo basta recordar que si la carga se trae desde el infinito
este está dado por
W = QV (L)
Entonces el potencial que genera un dipolo en L es
4π

V (L) = 3

σ0 R3 ẑ · Lρ̂
=0
4πε0 L3

Este resultado es bastante interesante, pero es natural pensarlo ya que la fuerza que siente
la sonda apunta en la dirección de z y la sonda se mueve en una plano perpendicular a la
fuerza, luego el trabajo debe ser nulo.

Solución 6.7

P X

Usando el método de las imágenes, se obtiene la configuración equivalente mostrada en la siguiente
Figura 6.5
z

~p
z0

x

Rodrigo Chi - Marzo 2017

z0

~p

Figura 6.5: Configuración Equivalente con dipolo-imagen
El dipolo se refleja de modo que su imagen tiene un momento dipolar −~p y se encuentra en
z = −z0 . Luego el potencial en un punto ~r = xx̂ + y ŷ + z ẑ está dado por la superposición del
potencial dipolo y su imagen, es decir
V (x, y, z) =

px̂ · (xx̂ + y ŷ + (z − z0 )ẑ) −px̂ · (xx̂ + y ŷ + (z + z0 )ẑ)
+
4πε0 |xx̂ + y ŷ + (z − z0 )ẑ|3
4πε0 |xx̂ + y ŷ + (z + z0 )ẑ|3
|

{z

}

Vdipolo

|

{z

Vimagen

}

---

### Página 151

CAPÍTULO 6. DIPOLO ELÉCTRICO
px
V (x, y, z) =
4πε0

−

(x2 + y 2 + (z − z0 )2 ) 2

!

(x2 + y 2 + (z + z0 )2 ) 2

~ = E(x, y)ẑ ya que éste
Ahora, el campo eléctrico sobre el plano xy debe ser de la forma E
debe ser siempre perpendicular a la superficie de un conductor, luego basta saber solamente la
derivada según z de V (x, y, z) para conocer el campo eléctrico que existe sobre un punto en el
plano infinito.
~ z = − ∂V ẑ = 3px
E
∂z
4πε0

z − z0

(x2 + y 2 + (z − z0 )2 ) 2

−

!

z + z0

(x2 + y 2 + (z + z0 )2 ) 2

ẑ

Finalmente, dado que el plano es conductor, se tiene que
~ · ẑ
σ(x, y) = ε0 E

z=0

=−

3pz0 x

2πε0 (x2 + y 2 + z02 ) 2

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 152

CAPÍTULO 6. DIPOLO ELÉCTRICO

IV.

Indicaciones Problemas Sin Solución

Indicación 6.1

P X

Determine el momento dipolar de la configuración de cargas.
Usando lo anterior, determine cuanto el potencial genera ese dipolo sobre los puntos que se
le solicitan en el problema.
Recuerde que el trabajo puede ser determinado como W = q(Vfinal − Vinicial )

Indicación 6.5

P X

Determine el momento dipolar de la barra según la distribución de carga que posee.
Dado que la barra tiene masa M distribuida en forma homogénea, determine el momento
de inercia de la barra.
A partir de lo anterior, determine torque que siente el dipolo debido al campo eléctrico
constante en el cual esta sumergido. Luego, relacione la expresión recién calculada con
~τ = I ω
~˙ .
Encuentre la ecuación de movimiento de la barra con respecto a θ y concluya el problema.

Rodrigo Chi - Marzo 2017

Indicación 6.8

P X

Para enfrentar este problema debe usar el método de las imágenes. La carga imagen en este
caso es otra barra simétrica a la original desde z = 0 hasta z = −L. Tenga precaución con
la densidad de carga de la barra imagen.
Una vez encontrada la configuración equivalente, determine el momento dipolar de la distribución y determine el potencial que genera ese dipolo para puntos muy alejados.

Indicación 6.9

P X

Determine el momento dipolar que tienen los planetas.
Utilizando lo anterior, determine el campo eléctrico al cual está afecto el primer planeta
debido al segundo.

---

### Página 153

CAPÍTULO 6. DIPOLO ELÉCTRICO
Conocido el campo eléctrico que afecta al primer planeta, determine el trabajo que realizó
el choque para hacer que éste girará. Recuerde que W = ∆U .
El trabajo que adicionó energía al sistema fue debido a la energía cinética que traía el
asteroide. Relacione esto con la velocidad al momento del choque.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 154

CAPÍTULO 6. DIPOLO ELÉCTRICO

V.

Respuestas
Problema

Respuestas
a) Vdip (0, L, 0) = 0

P

6.1

0b
b) F~ = 2qaρ
3ε0 L3 ẑ

c) W = 0
a) p~ = 4λR2 ŷ, Vdip (x, 0, z) = 0

P

6.2

~ dip (x, 0, z) =
b) E

λR2

πε0 (x2 +z 2 ) 2

ŷ

c) V (x, 0, z) = 0
a) ~r = (x, y, z)
~ = ρ0 R 3
Fuera de las dos esferas: E
3ε0

P

6.3



~
r −Rẑ
~
r +Rẑ
||~
r −Rẑ||3 − ||~
r +Rẑ||3



R3
~ = ρ0 (~r − Rẑ) −
Dentro de la esfera positiva: E
(~
r
+
Rẑ)
3ε0
||~
r +Rẑ||


R3
~ = ρ0
r + Rẑ) − (~r + Rẑ) .
Dentro de la esfera negativa: E
3ε0
||~
r −Rẑ||3 (~
b) El campo eléctrico decae como 1/r3 .

P

Rodrigo Chi - Marzo 2017

P

6.4

6.5

cos θ
V (r, θ) = − Q2πε
0r

~ = − Q 2 (cos θr̂ + sin θθ̂)
E
2πε0 r
a) p~ = 13 αL5 x̂
q
b) ω = 2L αLE
M
a) p~ = 4π
3 σ0 R ẑ

P

6.6



~ = − σ0 R33 ẑ
b) E
3ε0 ρ
c) V (L) = 0

---

### Página 155

CAPÍTULO 6. DIPOLO ELÉCTRICO
Problema

P

Respuestas
px
V (x, y, z) = 4πε

6.7

σ(x, y) = −

a)

P

6.8

P

6.9

α
σ(x, y) = − 2π



3 −

(x2 +y 2 +(z−z0 ) ) 2
3pz0 x


,

(x2 +y 2 +(z+z0 ) ) 2

2πε0 (x2 +y 2 +z02 ) 2

 √

x2 +y 2 +L2 +L
√
ln
− √ 2 L2
x2 +r 2



x +y +L2

cos θ
b) V (r) = αL
6πε0 r 2

v = R dρ0

q

π
2ε0 md

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 156

Rodrigo Chi - Marzo 2017

CAPÍTULO 6. DIPOLO ELÉCTRICO

---

### Página 157

Dieléctricos

I.

Resumen Teórico

Vector de Polarización
Dada la composición de dipolos eléctricos que poseen los materiales, es posible definir el vector
de polarización P~ como
P
p~i
~
P = lím
(7.1)
∆V →0 ∆V
El cual se define como la densidad de momento dipolar por unidad de volumen dentro de un medio
material.

Densidades de Carga de Polarización

σp = P~

borde

· n̂

(7.2)

donde n̂ es la normal de la superficie dieléctrica. Por otro lado, la densidad de carga volumétrica
de polarización está dada por
~ · P~
ρ p = −∇
(7.3)

Propiedades Eléctricas de los Materiales
Los materiales dieléctricos pueden ser clasificados de acuerdo a sus distintas propiedades eléctricas.
~
Un material lineal es aquel que cumple que en todos sus puntos |P~ | = α|E|.
~
Un material isótropo es aquel que P~ = αE.
Un material homogéneo cumple que α tiene el mismo valor en todos los puntos del material.

Problemas Propuestos y Resueltos de Electromagnetismo

La densidad de carga de polarización superficial está dada por

---

### Página 158

CAPÍTULO 7. DIELÉCTRICOS

Ley de Gauss Generalizada
Para incluir el aporte de los materiales en electrostática se define el vector desplazamiento como
~ = ε0 E
~ + P~
D

(7.4)

En general, si se trabaja con materiales lineales, isótropos y no homogéneos, es posible afirma que
~ = ε(~r 0 )E
~
D

(7.5)

donde ε(~r 0 ) es conocida como la constante dieléctrica del material. A partir de este nuevo vector,
se generaliza la Ley de Gauss de la siguiente forma
¨
~ = Qlibre
~ · dS
D
(7.6)
O equivalentemente en su forma diferencial
~ ·D
~ = ρlibre
∇

(7.7)

Energía con Dieléctricos
Como generalización para el cálculo de energía, esta puede ser determinada como
˚
~ · DdV
~
U=
E

(7.8)

Todo el
Espacio

Rodrigo Chi - Marzo 2017

Condiciones de Borde
La condiciones de borde en electrostática están dadas por
E1t = E2t

(7.9)

D2n − D1n = σlibre

(7.10)

Recomendaciones
Es muy importante diferenciar la carga libre con la carga de polarización. Por ejemplo, los
conductores sólo pueden tener carga libre en su superficie.
A veces puede ser algo confuso como determinar la normal n̂ de las densidades superficiales
de polarización. Recuerde que es siempre la normal exterior, que siempre apunta desde el
dieléctrico hacia fuera.

---

### Página 159

CAPÍTULO 7. DIELÉCTRICOS

II.

Problemas Propuestos

#### Problema 7.1

X S

Considere una esfera conductora de radio R1 , cargada
con Q. La cual está rodeada de un manto dieléctrico
de permitividad ε y radio R2 (con respecto al centro de
la esfera), el resto del espacio está vacío. Determine:

e
R1

a) El campo eléctrico en todo el espacio.

Q

b) Las densidades de carga libre e inducidas por la
polarización en las interfaces (cambios de medio).

R2

c) La diferencia de potencial entre la esfera conductora e infinito. ¿Aumenta o disminuye está
tensión debido producto a la presencia del
dieléctrico?.
#### Problema 7.2

X S

Una esfera conductora de radio R flota hasta la mitad
en un medio dieléctrico de permitividad eléctrica ε1 .
La región sobre la esfera es un gas de permitividad
eléctrica ε2 . La esfera está cargada con una carga
igual a Q.

e2

b) Calcule la densidad de carga libre superficial en
la esfera conductora, y la densidad superficial de
carga de polarización de ambos medios dieléctricos en la interfaz con la esfera.

e1

c) Si el medio en el cual flota la esfera es agua
(ε1 ≈ 79ε0 ) y el gas que hay sobre ella es aire
(ε2 ≈ ε0 ). Obtenga la relación (en módulo)
entre la carga total de polarización en la interfaz
con la esfera y la carga libre de la esfera, ¿qué
signo tiene la carga neta sobre la esfera? .

R

Problemas Propuestos y Resueltos de Electromagnetismo

a) Calcule el campo eléctrico en todo el espacio.

---

### Página 160

CAPÍTULO 7. DIELÉCTRICOS
#### Problema 7.3

X S

V =0

Entre dos placas infinitas paralelas (horizontales) separadas por una distancia 2a hay un campo el eléctrico
perpendicular a las placas, lo que implica una diferen- a e1
cia de potencial V0 . El espacio entre ellas está lleno
con un dieléctrico aislante con contante dieléctrica ε1
hasta la mitad de la altura y de ahí hacia arriba hay a e2
un material aislante con constante dieléctrica ε2 . Determine el valor que debe tener la densidad de carga
libre que hay en la interfaz si se mide que la densidad
de carga total en ese plano interfacial es nula.
#### Problema 7.4

slibre

V = V0

X S

a

b
Dieléctrico 1

En un condensador cilíndrico de radios a y b y de
largo L (
a, b) se han puesto dos dieléctricos tal
como se muestra la Figura. Si el condensador posee
carga +Q y −Q en sus superficies y los dieléctricos
e1
poseen permitividades ε1 y ε2 (ε1 < ε2 ), calcule la
fuerza necesaria que hay que aplicar al sistema para Condensador e2
que el dieléctrico de permitividad ε1 permanezca una
distancia 12 L dentro del condensador. Considere que
ambos dieléctricos son muy largos y se extienden más
allá del largo del condensador.

Dieléctrico 2

X S

Se tiene dos placas conductoras paralelas muy grandes, separadas una distancia d. El espacio entre las
placas está lleno con un material dieléctrico de permitividad ε(x), tal que ε(x = 0) = ε1 . Se encuentra que
el potencial electrostático entre las placas satisface la
ecuación diferencial

x

d2 V
dV
+k
=0
dx
dx

e(x)

donde k es una constante positiva.

+

Rodrigo Chi - Marzo 2017

#### Problema 7.5

L

a) El potencial electrostático V (x) dentro de las
placas.
b) La permitividad ε(x).
c) La densidad de carga libre que reside en la superficie conductora a potencial V0 .

x=0

x=d

V0

---

### Página 161

CAPÍTULO 7. DIELÉCTRICOS
#### Problema 7.6

X I

El espacio entre dos discos paralelos conductores de
radio R y separados una distancia d
R es puesto un
dieléctrico no uniforme, de modo que su permitividad
varía linealmente en función de la distancia del centro
de los discos
ε(r) = ε0 + (ε1 − ε0 )

r
R

R
e(r)

d

. Si los discos se encuentran a una diferencia de potencial V0 :
a) Determine el campo eléctrico, el vector
desplazamiento y las densidades superficiales/volumétricas de polarización.
b) ¿Cuánto vale la capacidad del sistema?.
#### Problema 7.7

X S

a) La capacidad del condensador para un x dado,
despreciando los efectos de borde (i.e. b
a, x)
b) La penetración x del dieléctrico para el condensador tenga una carga Q∗ (dado el voltaje de la
batería V0 ).
c) ¿Cuál es la fuerza que siente el condensador en
esa posición?.
d) ¿Cuál es el rango de carga Q∗ que puede ser
almacenado en el condensador?.

V0

+

b
a
x
e

Problemas Propuestos y Resueltos de Electromagnetismo

Un dispositivo de uso frecuente en muchos artefactos
eléctricos de uso diario son los condensadores variables. Este tipo de condensador posee una geometría
que es fácil de modificar mecánicamente, con lo cual
se puede ajustar su capacidad a gusto. Existen muchos diseños de este tipo de dispositivos, un ejemplo
simple e idealizado es el que se muestra en la Figura.
El cual consiste en dos placas paralelas y cuadradas
de largo a y separadas una distancia b. Entremedio de
las cuales se introduce parcialmente un dieléctrico de
permitividad ε, el cual penetra una distancia x de uno
de los bordes del condensador. Suponga que dispone
de una batería que da un voltaje V0 , y desea almacenar una carga Q∗ en el condensador. Para ajustarlo,
calcule

---

### Página 162

CAPÍTULO 7. DIELÉCTRICOS
#### Problema 7.8

X S

r(r)

Una esfera dieléctrica de radio b y permitividad de
carga ε contienen en un interior una densidad de carga
libre
(
ρ0 r 0 < r < b
ρ(r) =
0 r>b

b
e

a) Calcule las densidades de carga de polarización
en volumen ρp y superficial σp en las zonas donde existan.
b) Calcule la energía electrostática del sistema de
cargas.
#### Problema 7.9

X I

Tres láminas dieléctricas de permitividades ε1 , ε2 y ε3
están apiladas sobre otra como se indica en la Figura.
El campo eléctrico E~1 forma un ángulo θ1 con la normal en la interfase entre los medios 1 y 2. Suponga
que los campos eléctricos permanecen constantes en
magnitud y dirección al interior de cada medio.
~3
a) Encuentre el ángulo θ3 que forma el campo E
con la normal cuando emerge en el medio 3.
Suponga que no hay densidades de carga superficial libre en la interfase entre los medios
dieléctricos.

e3
~E3
e2

e1

~E2

~E1

q1

Rodrigo Chi - Marzo 2017

b) Encuentre la densidad de carga superficial libre
que habría que poner en la interfase entre los
~ 3 fuera paramedios 2 y 3 para que el campo E
~
lelo a E1 .
#### Problema 7.10

z

X I

Una esfera dieléctrica se radio a está uniformemente
polarizada, con un vector de polarización P~ = P0 ẑ
uniforme.
a) Calcule las densidades de carga de polarización
(volumétrica y superficial) en la esfera.
b) Calcule la dirección y magnitud del campo
eléctrico en el centro de la esfera.
c) Determine el potencial eléctrico V (r, θ) para
puntos r
a.

~P

a

---

### Página 163

CAPÍTULO 7. DIELÉCTRICOS

A

a
#### Problema 7.11

X I

Dos condensadores cilíndricos de radio interior a y exterior 3a, y largo L, han sido llenados con dos materiales dieléctricos ε1 y ε2 de distinta forma (ver figura). Si
los condensadores son conectados de la forma que se
indica en la figura, determine la capacidad equivalente
entre los puntos A y B.

e1
e2

e1

2a
3a

a

e2

3a

#### Problema 7.12

B

X I

d1

d2

e0

e

a) Cuando ambas placas de condensador están en
reposo, calcule la densidad de carga sobre cada
placa conductora.

s0

b) Considere que la placa de izquierda se acerca al
dieléctrico con una velocidad constante v0 . Calcule la diferencia de potencial que genera entre
los extremos de la resistencia en función de la
distancia d1 y el resto de los datos del problema.

R

Problemas Propuestos y Resueltos de Electromagnetismo

Un condensador de placas paralelas y área A tiene
una lámina dieléctrica de espesor d2 y permitividad
eléctrica ε adosada a una de sus placas. Un espacio
vacío de ancho d1 separa al dieléctrico de la otra placa
conductora. La superficie del dieléctrico en contacto
con el vacío está cargada con una densidad superficial de carga libre uniforme σ0 . Esta carga no puede
moverse. Las placas están conectadas a través de una
resistencia R, tal como se indica en la figura. Desprecie efectos de borde.

---

### Página 164

CAPÍTULO 7. DIELÉCTRICOS

#### Problema 7.13

V0

X S

+

Dos condensadores iguales, planos de placas paralelas
(ancho w, largo ` y separación d), están conectados
en paralelo a una fuente fem V0 . En un cierto tiempo
t0 , la fuente fem se desconecta de los condensadores
accionando un interruptor S. Posteriormente se introduce un trozo de material dieléctrico en uno de los
condensadores hasta llenarlo completamente.

d

`

a) Calcule la carga que es transferida de un condensador a otro al pasar de la situación inicial a
la situación final.
b) Calcule la diferencia de potencial que existe entre las placas de los condensadores en la situación final.
c) Calcule la corriente que circula en el circuito en
el instante en el que el dieléctrico llena la mitad
del condensador y se mueve con velocidad v0 .

#### Problema 7.14

d

`

x

e

X I

Un largo y sólido dieléctrico de forma cilíndrica de
radio a es está permanentemente polarizado tal que
su vector de polarización está dado por la expresión
P~ = 12 P0 rr̂.
Rodrigo Chi - Marzo 2017

S

a) Encuentre las densidades de cargas de polarización.
b) El campo eléctrico en todo el espacio.
c) Si el cilindro empieza a rotar con velocidad angular ω (con respecto a su eje) , determine el
campo magnético en todos los puntos dentro y
fuera del cilindro. a .
a
Solamente para la última parte de la pregunta es necesario
saber campo magnético

a

w

---

### Página 165

CAPÍTULO 7. DIELÉCTRICOS

III.

Soluciones
P X

Solución 7.1

a) Dada la simetría esférica del problema, es posible usar ley de Gauss de la siguiente forma
- r≤R

¨
~ = Qlibre = 0 =⇒ D
~ · dS
~ =0
D

~ = 0 (es un conductor)
Por lo tanto E
- R1 ≤ r ≤ R2

¨

Q
~ = Qlibre =⇒ D(r) · 4πr2 = Q =⇒ D(r)
~ · dS
~
D
=
r̂
4πr2

Por lo tanto

- r ≥ R2

~ = 1D
~ = Q r̂
E
ε
4πεr2
¨

Q
~ = Qlibre =⇒ D(r) · 4πr2 = Q =⇒ D(r)
~ · dS
~
r̂
D
=
4πr2

Por lo tanto

b) Las densidades de polarización están ubicadas en
σpol (R1 ) = P~ (R1 ) · (−r̂) =

(ε − ε0 ) Q
(ε − ε0 ) Q
r̂ · (−r̂) = −
ε
4πR1
ε
4πR12

(ε − ε0 ) Q
(ε − ε0 ) Q
σpol (R2 ) = P~ (R2 ) · r̂ =
r̂ · r̂ =
ε
4πR2
ε
4πR22
Mientras que la densidad de carga libre es
~ 1 ) · r̂ =
σlibre (R1 ) = D(R

Q
Q
r̂ · r̂ =
4πR1
4πR12

c) La diferencia de potencial entre el infinito y la esfera es
ˆ∞

ˆR2
~ =
~ · dl
E

V1 (R1 ) =
R1

Q
dr +
4πεr2

R1

ˆ∞
R2

Q
Q
Q
=
−
+
4πε0 r2
4πε R1 R2
4πε0 R2




Problemas Propuestos y Resueltos de Electromagnetismo

~ = 1D
~ = Q r̂
E
ε0
4πε0 r2

---

### Página 166

CAPÍTULO 7. DIELÉCTRICOS
En ausencia de dieléctrico se tendría que la tensión V2 es
V2 (R1 ) =

Q
Q
=
4πε0 R1
4πε0



Q
−
+
R1 R2
4πε0 R2


Nótese que el último término para ambos potenciales es igual, por lo que el término
que indica cual es mayor es el primer término de la suma, ahora dado que ε > ε0 , se
tiene que
Q
> =⇒
ε0
ε
4πε0



−
R1 R2



Q
>
−
4πε R1 R2




=⇒ V2 (R1 ) > V1 (R1 )

El potencial en la esfera es mayor en ausencia del dieléctrico.

Solución 7.2

P X

~ = 0 ya que es un conductor. Para r > R es necesario usar ley de
a) Para r < R se tiene E
Gauss de la siguiente forma
¨
~ = Qlibre =⇒ D1 (r) · 2πr2 + D2 (r) · 2πr2 = Q
~ · dS
D

Rodrigo Chi - Marzo 2017

Adicionalmente, dado que por simetría el campo eléctrico es completamente tangencial
~1 = E
~2 = E
~ . Luego D1 (r) = ε1 E(r) y
a la interfase de los medios, se tiene que E
D2 (r) = ε2 E(r), por lo que se puede despejar la expresión del campo eléctrico para r > R
como
Q
~
r̂
E(r)
=
2πr (ε1 + ε2 )
b) La densidad de carga libre dependerá del hemisferio de la esfera, de modo que para el
hemisferio inferior
ε1 Q
~ 1 (r) · n̂
r̂ · r̂
σl1 = D
=
r=R
2πR (ε1 + ε2 )
y de la misma forma para el hemisferio superior
~ 2 (r) · n̂
σl2 = D

r=R

=

ε2 Q
r̂ · r̂
2πR (ε1 + ε2 )

En cuanto a las cargas de polarización, hay que calcular previamente el vector polarización
en cada medio
~ = ε0 E
~ + P~ = εE
~ =⇒ P~ = (ε − ε0 )E
~
D
De modo que
~ = (ε1 − ε0 )Q r̂
P~1 = (ε1 − ε0 )E
2πr2 (ε1 + ε2 )
Entonces,
σP 1 = P~1 (r) · n̂

r=R

=

(ε1 − ε0 )Q
(ε1 − ε0 )Q
r̂
·
(−r̂)
=
−
2πR2 (ε1 + ε2 )
2πR2 (ε1 + ε2 )

---

### Página 167

CAPÍTULO 7. DIELÉCTRICOS
De forma análoga
σP 2 = −

(ε2 − ε0 )Q
2πR2 (ε1 + ε2 )

Notar el hecho que la normal en el caso de la densidad de carga libre apunta desde el
conductor al dieléctrico y en el caso de la densidad de carga de polarización apunta en el
sentido inverso.
c) La carga de polarización total está dada por
QP = 2πR2 σP 1 + 2πR2 σP 2 = −

QP
ε1 + ε2 − 2ε0
(ε1 + ε2 − 2ε0 )Q
=
=⇒
≈
(ε1 + ε2 )
Q
ε1 + ε2

Luego la carga neta vale
Qneta = Q + QP =

Q
>0

.

Solución 7.3

P X

V =0

a

~D1

e1

slibre

z
a

e2

~D2
V = V0

Figura 7.1: Condensador con dos medios.

Problemas Propuestos y Resueltos de Electromagnetismo

Para iniciar el problema hay que analizar lo que se pide, ¿qué significa que la carga total en la
interfase sea nula? en la interfase existen tres densidades de carga que viven juntas: la densidad de
carga libre, la densidad de carga de polarización del dieléctrico ε1 y la del dieléctrico ε2 . La suma de
esas tres densidades superficiales de carga debe ser nula y para ello hay que determinar el campo
eléctrico que existe dentro de las placas conductoras. Dado que las geometrías que componen
este problema son planas, los vectores desplazamiento y campo eléctrico son constantes en cada
~ 1 = D1 ẑ = ε1 E1 ẑ y D
~ 2 = D2 ẑ = ε2 E2 ẑ.
medio, es decir D

---

### Página 168

CAPÍTULO 7. DIELÉCTRICOS
Entonces, aplicando la Ley de Gauss Generalizada al cilindro de la Figura 7.1, se tiene que
¨
~ = Qlibre =⇒ D1 · A − D2 · A = σlibre · A =⇒ ε1 E1 − ε2 E2 = σlibre
~ · dS
D
Adicionalmente,
ˆ0
V0 = V (0) − V (2a) = −

~ = E1 a + E2 a =⇒ E1 + E2 = V0
~ · dl
E
a

2a

De las dos últimas ecuaciones es posible determinar el campo eléctrico presente en el espacio
como




ε2 V0
ε2 V 0
E1 =
+ σlibre
E2 =
− σlibre
ε1 + ε2
a
ε1 + ε2
a
Ahora, también es posible aplicar la Ley de Gauss tradicional al mismo cilindro de la Figura 7.1,
donde se obtiene que
¨
~ = Qtotal =⇒ E1 · A − E2 · A = σtotal · A
~ · dS
E
ε0
ε0
Nótese el hecho que σtotal incluye las tres densidades de carga que existen en z = a, por lo que
finalmente se obtiene
σtotal = 0 =⇒ E1 = E2 =⇒ σlibre =

Solución 7.4

V0 (ε1 − ε2 )
2a

P X

Rodrigo Chi - Marzo 2017

Para iniciar el problema se necesita saber la capacitancia de un condensador cilíndrico que posee
un medio con constante εi en un interior, de radios a y b y de largo H. Para ello se usa la ley de
Gauss para el espacio entre los cilindros (a < r < b).
"
~ = Q =⇒ D(r)2πrH = Q =⇒ E
~
~ =
D(r)
· dS
Ω

Luego

ˆb
∆V = V (a) − V (b) =
a

Q
b
Q
=
ln
2πεi rH
2πεi H
a

Por lo que
C=

Q
r̂
2πεi rH

Q
2πεi H
= b
∆V
ln
a

!

---

### Página 169

CAPÍTULO 7. DIELÉCTRICOS

e1

z

e2

L

z

z

Figura 7.2: Dieléctricos dentro del Condensador Cilíndrico
Para lo que sigue del análisis se debe considerar la Figura 7.2. Se ha puesto el dieléctrico 1 una
distancia z dentro del condensador. La capacitancia de este sistema es equivalente a la de dos
condensadores en paralelo, luego la capacitancia total del sistema es igual a su suma, es decir:
CT = C1 + C2 =

2πε1 z
ln

 +

2πε2 (L − z)

b
a

ln

 
b
a

=

2π
ln

  ((ε1 − ε2 )z + ε2 L)
b
a

Por lo tanto la energía de ese condensador está dada por
1 Q2
2 CT (z)

Luego, considerando que la carga es constante, la fuerza que ejerce el sistema es
∂
F~sist = −∇U = − Q2
2 ∂z

!

1 Q2 ∂CT (z)
ẑ =
ẑ
CT (z)
2 CT (z)2 ∂z

Reduciendo la expresión a
!

1 2
b
ε1 − ε2
F~sist =
Q ln
ẑ
4π
a ((ε1 − ε2 )z + ε2 L)2
Nótese lo siguiente, como ε1 < ε2 la fuerza que efectúa el sistema apunta en el sentido de
negativo de z, por lo que el dieléctrico 2 intenta expulsar al dieléctrico 1 del condensador. En
efecto, este resultado es consecuencia de que el sistema busque su mínima energía, la se obtiene
con el condensador completamente lleno del dieléctrico con constante ε2 . Por lo tanto, para poder
introducir el dieléctrico 1 una distancia z = 21 L dentro del condensador se debe aplicar una fuerza
del mismo valor en el sentido contrario a la que se siente en ese punto, es decir, la fuerza buscada
vale
!
Q
b
ε2 − ε1
F~ext = −F~sist 1 =
ln
ẑ
z= 2 L
πL
a (ε1 + ε2 )2

Problemas Propuestos y Resueltos de Electromagnetismo

U=

---

### Página 170

CAPÍTULO 7. DIELÉCTRICOS
Solución 7.5

P X

a) Se debe encontrar el valor de V (x), sabiendo que el potencial cumple la siguiente condición
d2 V (x)
dV (x)
=0
+k
dx
dx
Con k > 0 y 0 ≤ x ≤ d. Para ello se asume que la solución de la EDO es V (x) = Aeαx + B
con A, B y α constantes no nulas por determinar. En efecto, reemplazando la solución en
la ecuación anterior
d2 V (x)
dV (x)
= Aα2 eαx + kAαeαx = Aαeαx (α + k) = 0
+
k
dx2
dx
De la ecuación anterior se obtiene
α = −k
Luego, la solución se transforma en V (x) = Ae−kx + B y las otras constantes pueden ser
despejadas con las condiciones de borde
V (0) = 0 =⇒ A + B = 0 =⇒ A = −B
V (d) = V0 =⇒ Ae−kd + B = V0
Despejando A y B de las ecuaciones anteriores
V0
e−kd − 1
V0
B = − −kd
e
−1
A=

Finalmente la solución es
V (x) =

V0 (e−kx − 1)
e−kd − 1

b) Dado que se conoce el potencial, es posible conocer el campo eléctrico dentro de las placas

Rodrigo Chi - Marzo 2017

~ = −∇V = − d
E
dx

V0 (e−kx − 1)
V0 ke−kx
x̂
=
x̂
e−kd − 1
e−kd − 1
!

Asumiendo que el material es lineal, isótropo y no homogéneo se tiene que
−kx

~ = ε(x)E
~ = ε(x) · V0 ke
D
x̂
e−kd − 1
Dada la ausencia de carga libre dentro de las placas
~ ·D
~ = 0 =⇒ d (ε(x)e−kx ) = 0 =⇒ ε(x)e−kx = C
∇
dx
Usando la condición de borde ε(x = 0) = ε1 =⇒ C = ε1 por lo tanto
ε(x) = ε1 ekx
~ · n̂
c) La densidad de carga libre en la placa a potencial V0 dada por σl = D
σl = ekx ·

V0 ke−kx
kV0
x̂ · (−x̂) = − −kd
−kd
e
−1
e
−1

x=d

, de modo que

---

### Página 171

CAPÍTULO 7. DIELÉCTRICOS
Solución 7.7

P X

a) La capacitancia de un condensador de placas paralelas es
C=

εA
d

donde ε es la permitividad del medio que lleva dentro el condensador, A es el área de las
placas y d es la separación entre ellas. Si un dieléctrico se pone parcialmente una distancia
x en el condensador, se forman dos condensadores en paralelo, de capacitancia
C1 =

ε0 a(a − x)
εax
, C2 =
b
b

Por lo que la capacitancia total (condensadores en paralelo) es
a
CT = C1 + C2 = (εx + (a − x)ε0 )
d
b) Por otro lado, se tiene que la definición capacitancia es
C=

Q
∆V

Por lo que si el condensador está conectado a una batería de voltaje V0 y tiene una carga
Q∗ se cumple que
Q∗
a
CT = (εx + (a − x)ε0 ) =
=⇒ x =
b
V0
ε − ε0

Q∗ b
− εa
V0 a

!

a
Q(x) = ((ε − ε0 )x − ε0 a)
d
lo cual es una función lineal, y como ε ≥ ε0 se tiene la función Q(x) alcanza su mínimo en
x = 0 y su máximo en x = a. Por lo que
Q(x = 0) =

ε 0 a2
εa2
≤ Q(x) ≤
= Q(x = a)
d
d

Nótese que físicamente esto significa que el condensador alcanza su mínima carga vacío y
su máxima carga lleno de dieléctrico.

Solución 7.8

P X

a) Calcular las densidades de carga de polarización en el espacio. Para resolver este problema
es necesario dividir en dos áreas, un radio menor y mayor al radio de esfera b.

Problemas Propuestos y Resueltos de Electromagnetismo

d) Dada la dependencia Q = Q(x) se tiene que la carga varía en el rango x ∈ [0, a], si se usa
la parte anterior, se obtiene que

---

### Página 172

CAPÍTULO 7. DIELÉCTRICOS
- r > b se tiene que hay vacío por lo tanto no existe el vector polarización.
- r ≤ b, de acuerdo a la ley de Gauss
¨
˚
~
~
D · dS =
ρ0 rdV
Ω

r4
D(r) · 4πr = 4πρ0
ρ
r
~ =
r̂
D

Por lo tanto

~ = ρ0 r r̂
E
4ε

~ − ε0 E
~ se obtiene
Utilizando P~ = D

(ε − ε0 )ρ0 r
P~ =
r̂
4ε
Luego, la densidad de carga de superficial polarización es
σp = P~ · n̂|r=b
(ε − ε0 )ρ0 b2
=
4ε

Rodrigo Chi - Marzo 2017

y la densidad volumétrica polarización es
ρp = −∇ · P~
1 ∂
= − 2 (Pr · r2 )
r ∂r
!
1 ∂ (ε − ε0 )ρ0 r4
=− 2
r ∂r
4ε
1 (ε − ε0 )ρ0 r3
=− 2
r
ε
−(ε − ε0 )ρ0 r
=
ε
~ yE
~
b) Para calcular la energía electrostática del sistema de cargas es necesario encontrar D
para un r > b.
¨

˚
~ =
~ · dS
D

ρ0 rdV

Ω

D(r) · 4πr2 = 4πρ0

b4

~ = ρo b r̂
D
4r2

---

### Página 173

CAPÍTULO 7. DIELÉCTRICOS
Entonces,

~ = ρo b r̂
E
4ε0 r2
Ya con esto es posible encontrar la energía del sistema en todo el espacio
˚
~ · EdV
~
U=
D
Todo el
Espacio

=

ˆ∞ ˆ2π ˆπ
D(r) · E(r)r2 sin θdθdϕdr

=

ˆb ˆ2π ˆπ

D(r) · E(r)r sin θdθdϕdr +

=

0 0
b
ˆ ˆ2π ˆπ

= 2π

ρ0 r2 ρ0 r2 2
r sin θdθdϕdr +
4 4ε

ρ0 r 2
4ε

ε

r2 dr + 2π

ε0

ρ0 b4
4ε0 r2

!2

r2 dr

b



= 2π 


ρ 0 b4 ρ 0 b4 2
r sin θdθdϕdr
4r2 4ε0 r2

b

ˆ∞

!2

D(r) · E(r)r2 sin θdθdϕdr

b 0 0
∞
ˆ ˆ2π ˆπ

ˆb

b
2 ˆ

ερ0
16ε2

=

ˆ∞ ˆ2π ˆπ


πρ20 b7 1



b

+

ε0



P X

a) Para encontrar la carga que se transfiere de un condensador a otro, comenzamos
buscando la carga del sistema completo.
Se considera que la capacitancia de un condensador de placas paralelas está dada por
C=

εA
d

Luego si inicialmente el sistema se encontraba sometido a un voltaje V0 , la carga total
será la suma de la carga de ambos condensadores, pero como estos eran iguales
!

ε0 `w
Qtot = 2CV0 = 2
V0
d
Por otro lado, se calcula las cargas en cada condensador en el tiempo final, tf . Para
esto es necesario notar que en tf una de las capacitancias se habrá modificado de
modo que
ε`w
ε0 `w
C1 =
C2 =
d
d

Problemas Propuestos y Resueltos de Electromagnetismo

Solución 7.13

7ε

ˆ∞ 2
ε0 ρ2 b8
r
r dr +
dr

16ε0
r

---

### Página 174

CAPÍTULO 7. DIELÉCTRICOS
Al estar en paralelo, éstos se encuentran a la misma diferencia de potencial
Vf 1 = Vf 2 =⇒

Q1
Q2
Q2
=
=⇒ Q1 =
C1
C1
C2
C2

Pero como la carga total debe conservarse


Qtot = Q1 + Q2 = Q2

C1
ε
+ 1 = Q2
+1
C2
ε0






Por ende,
Qtot ε
2V0 εε0 `w
=
ε + ε0
d(ε + ε0 )

Q2 =

Con lo anterior es posible concluir que la carga traspasada es
2V0 ε0 `w
Qtot
=
∆Q = Q2 −
d



ε − ε0
ε + ε0



b) La diferencia de potencial estará dada por
Vf =

Q2
2V0 ε0
2V0 εε0 `w d
=
=
C2
d(ε + ε0 ) ε0 `w
ε + ε0

c) Finalmente, para encontrar la corriente cuando dieléctrico se encuentra en la mitad, se
debe calcular la capacidad de sistema para una distancia x cualquiera de penetración
del dieléctrico, en este caso
C1 =

εxw ε0 (` − x)w
+
d
d

Luego


Q2 = Qtot

−1
C1
+1
C2



Rodrigo Chi - Marzo 2017

y como el cuociente
C1
w(εx + ε0 (` − x)) d
εx + ε0 (` − x)
=
=
C2
d
ε0 `w
ε0 `
εx + ε0 (` − x)
+1
ε0 `

2V0 ε0 `w
=⇒ Q2 =
d

!−1

=

2V0 ε20 `2 w
d(2ε0 ` + x(ε − ε0 ))

Finalmente la corriente esta dada por
`
I x=

!

dQ2
dQ2
dx
=
=
=
dt x= `
dx x= ` dt x= `

!

−2V0 ε20 `2 w(ε − ε0 )
v0
d(2ε0 ` + 2` (ε − ε0 ))2

---

### Página 175

CAPÍTULO 7. DIELÉCTRICOS

IV.

Indicaciones Problemas Sin Solución

Indicación 7.6

P X

Debido a las condiciones de borde entre medios materiales, el campo eléctrico debe ser
independiente del radio.
Consecuencia de lo anterior, el campo eléctrico dentro del condensador es el mismo que
hubiese sin el dieléctrico. Con esto se puede determinar fácilmente el vector desplazamiento y la polarización dentro del material. Conocida la polarización es posible conocer las
densidades superficiales y volumétricas de carga.
Determine la diferencia de potencial entre los discos conductores. Con ello ya puede determinar la capacidad.

Indicación 7.9

P X

La componente horizontal de E1 debería ser la misma en todos los medios, ya que E1t = E2t .
La componente que cambia de medio en medio es la vertical.
Para la segunda parte del problema, note que necesariamente en el medio 3 se tendrá la
misma componente horizontal del campo eléctrico que en el medio 1, por ende, si se busca
~1 = E
~ 3 ).
que sean paralelos necesariamente tienen que ser iguales (E

P X

Determine la densidad de carga superficial y volumétrica de la esfera debido a la polarización.
Utilizando las densidades encontradas, use la definición de campo eléctrico para determinar
el campo eléctrico en el centro de la esfera.
Note el momento dipolar de la esfera es |~p| = P V = P · 43 πa3 (demúestrelo), con ello ya
es posible determinar el potencial eléctrico para puntos lejanos a la esfera.

Indicación 7.11

P X

Determine el la capacidad de cada uno de los condensadores por separado.
Note que debido a la tipo de conexión de los condensadores, éstos se encuentran en serie.

Problemas Propuestos y Resueltos de Electromagnetismo

Indicación 7.10

---

### Página 176

CAPÍTULO 7. DIELÉCTRICOS
Indicación 7.12

P X

Encuentre el vector desplazamiento en cada medio para luego determinar la densidad de
~
· n̂
carga libre sobre las placas conductoras. Recuerde sobre un conductor σlibre = D
borde
donde n̂ es la normal del conductor.
Para encontrar el vector desplazamiento puede plantear la ecuación de Laplace en cada
medio o inspirarse en el Problema 7.3.
Para determinar la diferencia de potencial de las placas, determine como cambia la carga
en las placas debido a que la distancia d1 comienza a disminuir. Podría ser útil notar que
d˙1 = −v0 y V = RI = R dQ
dt

Indicación 7.14

P X

Las densidades de carga pueden ser directamente obtenidas a partir del vector polarización.
Use la Ley de Gauss Generalizada para determinar el campo eléctrico dentro y fuera del
cilindro. Note que al ser un dieléctrico no existe carga libre ni dentro ni fuera del cilindro.

Rodrigo Chi - Marzo 2017

Usando la densidades de carga encontradas en la primera parte del problema, determine
las densidades de corriente que existen en el cilindro. Una vez determinadas, determine el
campo magnético mediante Ley de Ampère.

---

### Página 177

CAPÍTULO 7. DIELÉCTRICOS

V.

Respuestas
Problema

Respuestas

~ =
a) E

P







7.1

r < R1

Q
4πεr 2 r̂

R1 < r < R2

Q
4πε0 r 2 r̂

r > R2

Q
Q
Q
0)
0)
, σpol (R2 ) = (ε−ε
, σlibre (R1 ) = 4πR
b) σpol (R1 ) = − (ε−ε
ε
ε
4πR12
4πR22


Q
Q
c) V1 (R1 ) = 4πε
R1 − R2 + 4πε0 R2 , el potencial en la esfera es mayor en ausencia
del dieléctrico.

~ =
a) E

P








7.2




r<R



Q
2πr 2 (ε1 +ε2 ) r̂

r>R

(ε1 −ε0 )Q
(ε2 −ε0 )Q
ε2 Q
1Q
b) σl1 = 2π(ε1ε+ε
2 , σl2 = 2π(ε +ε )R2 , σP 1 = − 2πR2 (ε +ε ) , σP 2 = − 2πR2 (ε +ε )
2 )R

c)

QP
Q

Q
= 39
40 , Qneta = 40

P

7.3

1 −ε2 )
σlibre = V0 (ε2a

P

7.4

Q2
F~ext = πL
2 ln

ε2 −ε1
b
a (ε1 +ε2 )2 ẑ



P

7.5

b) ε(x) = ε1 ekx
kV0
c) σl = − e−kd
−1

a)

P

7.6

rV0
E V0
D
= d ẑ, = ε0 + (ε1 − ε0 ) Rd ẑ
rV0
σP 1 (r) = (ε1 − ε0 ) rV
Rd , σP 2 (r) = −(ε1 − ε0 ) Rd , ρp = 0.

b) C = πR
3d (ε0 + 2ε1 )

Problemas Propuestos y Resueltos de Electromagnetismo

−kx

−1)
a) V (x) = V0e(e−kd −1

---

### Página 178

CAPÍTULO 7. DIELÉCTRICOS
Problema

P

Respuestas
a) CT = ad (εx + (a − x)ε0 )
 ∗

Q b
−
εa
b) x = ε−ε
V0 a

7.7

0 )aV0 2
c) F~ = (ε−ε2d
x̂, donde x crece de derecha a izquierda.

d)

ε0 a2
εa2
d ≤ Q(x) ≤ d

P

7.8

P

7.9

0 )ρ0 b
, ρp (r < b) = − (ε−εε0 )ρ0 r
a) σp (r = b) = (ε−ε4ε


πρ2 b7
b) U = 80
+
7ε
ε0

a) tan θ3 = εε31 tan θ1
b) σl = (ε3 − ε1 )|E1 | cos θ1
a) σp = P0 cos θ, ρl = 0

P

7.10

P0
~
b) E(0)
= − 3ε
ẑ

a cos θ
c) V (r, θ) = P03ε
0r

P

P

7.11

7.12

C = ln(2)
2ε1

πL
+

ln(3)−ln(2)
ln(3)
+ ε +ε
2ε2

2 ε0
0 d1 ε
, σ2 = − d1σε+d
a) σ1 = − d2σε00d+d
1ε
2 ε0
0 σ0 Rv0 t
b) ∆V = (d2 εAεε
0 +(d1 −v0 t)ε)

a) ∆Q = 2V0 εd0 `w

Rodrigo Chi - Marzo 2017

P

7.13

7.14

ε−ε0
ε+ε0



0 ε0
b) Vf = 2V
ε+ε0


−2V ε20 `2 w(ε−ε0 )
v0
c) I = d(2ε 0`+
`
(ε−ε ))2

P



a) ρp = P0 , σp = − P20 a
 Pr
 2ε00 r̂ r < a
~ =
b) E

r>a
~
c) B(z)
=0

---

### Página 179

Parte II

Corriente Eléctrica

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 180

Rodrigo Chi - Marzo 2017

---

### Página 181

Medios Conductores

I.

Resumen Teórico

Corriente y Vector Densidad de Corriente
La corriente o intensidad eléctrica I es simplemente un movimiento de carga. Matemáticamente
se define como la cantidad de carga dQ por unidad de área que atraviesa una sección transversal
de un conductor en un tiempo dt
dQ
(8.1)
I=±
dt
Se define el vector densidad de corriente J~ como flujo por unidad de área
¨
~
I=
J~ · dS
(8.2)

donde n̂ es la normal de la superficie por donde circula la corriente.

Ecuación de Continuidad
La ecuación de continuidad establece un equilibrio entre la carga que se encuentra circulando y
acumulando en un mismo sistema. Formalmente,
~ · J~ + ∂ρ = 0
∇
∂t

(8.4)

En particular, en estado estacionario se cumple que
∂ρ
~ · J~ = 0
= 0 =⇒ ∇
∂t

(8.5)

Problemas Propuestos y Resueltos de Electromagnetismo

También existen densidades superficiales de corriente (ie. corrientes que circulan por superficies),
~ en la cual se relaciona con la intensidad de corriente como
denotadas como K
ˆ
~ × n̂) · d~l
I = (K
(8.3)

---

### Página 182

CAPÍTULO 8. MEDIOS CONDUCTORES

Ley de Ohm
Algunos medios conocidos como “Óhmnicos” poseen una conductividad g asociada que relaciona
~ que circula por el medio.
la densidad de corriente J~ y el campo eléctrico E
~
J~ = g E

(8.6)

Condiciones de Borde para J~
En estado estacionario, se tiene que la componente normal de vector J~ es continua en la interfase
entre dos medios de distinta conductividad g1 y g2 .
J~1n = J~2n

(8.7)

Y que la componente tangencial del campo eléctrico es continua entre dos medios
~ 1t = E
~ 2t
E

(8.8)

Pérdidas por efecto Joule
Las pérdidas por efecto Joule están relacionadas con los modelos óhminicos.
˚
~
P =
J~ · EdV

(8.9)

Rodrigo Chi - Marzo 2017

Resistencia Eléctrica
La resistencia eléctrica es la cualidad de los materiales para impedir el paso de la corriente. La
resistencia R puede ser determinada por la geometría del material, la cual está dada por
R=

ηA
L

Donde η es la resistividad, A es la sección transversal y L el largo del material.

(8.10)

---

### Página 183

CAPÍTULO 8. MEDIOS CONDUCTORES

II.

Problemas Propuestos

#### Problema 8.1

X I

Una densidad de corriente, como función de la posición ~r y tiempo t tiene la forma:

r(~r,t)?

J~ = C~re−αt|~r|

~ r,t)
J(~

Donde C y α son constantes. Mostrar que la ecuación de conservación de la carga se satisface con una
densidad de carga ρ de la forma:
ρ = (f + tg)e−αt|~r|

Donde f y g son funciones por determinar que dependen de la posición.
#### Problema 8.2

X S

#### Problema 8.3

y

~v
x

X I

Considere dos esferas conductoras concéntricas de radios a y 3a. La región entre a < r < 2a es llenada
con un material de conductividad g1 y la región entre 2a < r < 3a tiene material de conductividad g2 .
Asuma que ambos materiales tienen una permitividad
igual a ε0 . La esfera interior se encuentra a un potencial V = V0 y la exterior V = 0. Determine
a) La resistencia del sistema.
b) La densidad superficial de carga en r = 2a.

a
V0
g1
g2

2a
3a

Problemas Propuestos y Resueltos de Electromagnetismo

Considere un plano conductor suficientemente grande,
sobre el cual los portadores se mueven con velocidad
constante ~v = v0 x̂. Si inicialmente la densidad de car2
ga es Gaussiana ρ(x, y, t = 0) = ρ0 e−α(x +y ) donde
ρ0 y α son constantes, encuentre como evoluciona la
densidad de carga en función del tiempo ρ(x, y, t) y
comente como esta densidad de carga cambia con el
tiempo.

---

### Página 184

CAPÍTULO 8. MEDIOS CONDUCTORES
#### Problema 8.4

X S

Considere un condensador cilíndrico de radio interior
a y radio exterior b y largo L. La superficie cilíndrica
interna del condensador se encuentra a potencial V0
mientras que la exterior se encuentra a un potencial
nulo. El condensador tiene dentro de él dos materiales
conductores de conductividad g1 y g2 . El material con
conductividad g1 subtiende un ángulo β en el condensador, mientras que el otro ocupa todo el volumen
restante. Si el sistema ha alcanzado el régimen estacionario, determine

g1
b

a) La corriente eléctrica que circula por ambos medios.

g2

b) Determine la resistencia que opone cada medio
al paso de la corriente. Demuestre que el valor
de la resistencia total está dado por


RT =

+
R1 R2

a
b

−1

donde R1 y R2 es la resistencia del medio 1 y
2, respectivamente.
z

Rodrigo Chi - Marzo 2017

#### Problema 8.5

X S

z = z2

Considere un material de resistividad η el cual tiene
forma de paraboloide de ecuación x2 + y 2 = 4z con
z ∈ [z1 , z2 ]. Si se aplica una diferencia de potencia
V0 entre sus caras planas, determine el valor de la
corriente que circulará por el material.

z = z1
y
x

#### Problema 8.6

d

X I

Un semianillo de sección transversal cuadrada está hecho de un material conductor uniforme de conductividad g. Encuentre la resistencia eléctrica del semianillo
entre sus caras cuadradas. Utilice las dimensiones que
se indican en la figura.

r

---

### Página 185

CAPÍTULO 8. MEDIOS CONDUCTORES
X I

L

Considere un circuito puesto a tierra consistente en
dos esferas perfectamente conductoras, como es mostrado en la Figura. Los radios de las esferas son a1 y a2
y la distancia entre ellas es L, donde L
a1 , a2 . Una
mitad de cada esfera está inmersa en tierra, la cual
posee una conductividad g. Determine la resistencia
total entre las esferas.

#### Problema 8.8

a1

g

a

X I

V0

Entre dos placas conductoras de radio a existe una
barra conductora cilíndrica de radio a y longitud
 L,
z
permitividad ε0 y conductividad g = g0 1 + L . Se
aplica un potencial V0 entre las placas.
a) Calcular la densidad de corriente J~ y el campo
~ dentro del cilindro.
eléctrico E

z

g(z)

b) Calcular la potencia disipada en un disco de espesor e cuyo centro está situado justo en la mitad del conductor.

#### Problema 8.9

a2

Aire
Tierra

+

#### Problema 8.7

X S

a) Considerando que se ha alcanzado el régimen
estacionario, encuentre una ecuación diferencial
de segundo orden que describa el comportamiento del potencial dentro del cubo. Use lo anterior para determinar la diferencial de potencial
entre las caras S y S 0 .
b) Determine la resistencia y la corriente total que
circula entre S y S 0 . Encuentre en valor de la
carga Q que se acumula en el cubo.

z

S

y
a

S0

a

x
a

Problemas Propuestos y Resueltos de Electromagnetismo

Un bloque de material conductor en forma cubo de
lado a tiene una conductividad no uniforme dada por
g(x) = ga0 (x + a) y una permitividad ε0 , donde g0 es
una constante. Asuma que la corriente fluye a lo largo
del eje x desde la cara S hasta la cara opuesta S 0 .
Suponga que potencial eléctrico V dependiente sólo
de x, y que el valor del campo eléctrico en el borde es
~ = 0, y, z) = E0 x̂.
conocido E(x

---

### Página 186

CAPÍTULO 8. MEDIOS CONDUCTORES
#### Problema 8.10

X S

g = k|~E|

Una esfera metálica de radio a está rodeada por un
cascarón conductor esférico de radio interior b, donde b > a. El espacio entre la esfera y el cascarón
está lleno de un material cuya conductividad eléctri~ con la
ca g varía la magnitud del campo eléctrico E,
~
ecuación g = k|E|, donde k es una constante. Una
diferencia de potencial constante V se mantiene entre
la esfera y el cascarón conductor de radio b. Calcule la
corriente eléctrica y la densidad volumétrica de carga
entre la esfera y el cascarón. Exprese el resultado en
función de los datos del problema.

b

+

#### Problema 8.11

a

V

e0 , g

X I

Una esfera de radio a se encuentra inmersa en un
medio de permitividad ε0 y conductividad g. Al tiempo
t = 0 una carga eléctrica Q0 se coloca uniformemente
distribuida sobre la esfera.

r0
a

a) Determine la corriente total en el medio en función del tiempo.

r

Rodrigo Chi - Marzo 2017

b) Calcule la cantidad de energía disipada como
calor durante el proceso de descarga.

#### Problema 8.12

A

X I

Considere un condensador de forma arbitraria, el cual
tiene dentro de él un medio de conductividad g y permitividad ε0 . Sea R y C la resistencia y la capacitancia entre los terminales A y B, respectivamente.
Demuestre que
ε0
RC =
g

e0
Material
g
B

---

### Página 187

CAPÍTULO 8. MEDIOS CONDUCTORES
#### Problema 8.13

X S

Considere dos condensadores de placas cuadradas de
lado 2a separadas una distancia 2d. Dentro de cada condensador existen dos medios con constantes
dieléctricas y conductividades, ε1 , g1 y ε2 , g2 . Los
medios llenan la mitad del volumen de cada condensador, pero de una disposición distinta en cada uno
(ver figura). Despreciando todos los efectos de borde:

b) Para el condensador de la derecha, determine las
densidades de polarización y carga libre donde
correspondan.

+

a) Para cada condensador determine el vector den~ vector campo eléctrico E
~
sidad de corriente J,
~
y vector desplazamiento D dentro de él.

d

e1 , g 1

d

e2 , g2

V0

e1 , g 1

e2 , g2

a

a

2d

c) Determine la capacitancia equivalente que forman ambos condensadores.
d) Determine la corriente que sale por la fuente y
la resistencia equivalente del sistema.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 188

CAPÍTULO 8. MEDIOS CONDUCTORES
X S

Considere el circuito mostrado en la figura. El circuito
consta de una fuente de voltaje V0 , un condensador
cilíndrico, un switch que puede cambiar entre las posiciones 1 y 2 y una resistencia RL desconocida. El
condensador cilíndrico tiene largo L y posee un radio interior a y un radio exterior c (L
a, c). En
el interior del condensador hay dos medios materiales
óhmicos de conductividad constante g1 y g2 y permitividad aproximadamente igual a ε0 . Las posiciones
respectivas de cada material al interior del condensador se muestran en la figura parte (b). Si el switch
inicialmente se encuentra el posición 1 y el sistema ya
ha alcanzado el régimen estacionario, determine
a) El vector densidad de corriente J~ y el campo
~ dentro del condensador.
eléctrico E

L

+

#### Problema 8.14

V0

(a) Vista Exterior

b) La carga total de cada placa cilíndrica del condensador.
c) La corriente que circula por el sistema.

a

d) La resistencia del sistema.

Rodrigo Chi - Marzo 2017

Si el switch se cambia a la posición 2 y el sistema
nuevamente ha alcanzado el régimen estacionario.
e) Determine el valor de RL tal que maximice la
potencia disipada en dicha resistencia. ¿Cuál es
el valor de esa potencia?. (Indicación: Recuerde
la potencia disipada en una resistencia puede ser
calculada como P = V · I)

g1

b

c

g2

(b) Vista Interior

RL

---

### Página 189

CAPÍTULO 8. MEDIOS CONDUCTORES

III.

Soluciones

Solución 8.2

P X

En primera instancia, debe notarse que
J~ = ρ~v = ρ(x, y, t)v0 x̂
Luego usando la ecuación de continuidad se tiene que
~ · J~ + ∂ρ = ∂ (ρv0 ) + ∂ρ = 0 =⇒ ∂ρ + v0 ∂ρ = 0
∇
∂t
∂x
∂t
∂t
∂x
Para resolver la EDP anteriormente encontrada, es necesario usar los cambios de variable w =
x + v0 t y u = x − v0 t. Por regla de la cadena, estos cambios de variable provocan que
∂
∂w ∂
∂u ∂
∂
∂
=
+
=
+
∂x
∂x ∂w ∂x ∂u
∂w ∂u
∂
∂w ∂
∂u ∂
∂
∂
=
+
= v0
−
∂t
∂t ∂w
∂t ∂u
∂w ∂u

!

Aplicando estas derivadas a la EDP original, se obtiene que
2v0

∂ρ
= 0 =⇒ ρ = F (u) = F (x − v0 t)
∂w

La última ecuación muestra que ρ depende netamente de x−v0 t. Finalmente, usando la condición
inicial en t = 0

La densidad de carga se mueve hacia la derecha en la dirección de aumento x manteniendo su
forma de Gaussiana.

Solución 8.4

P X

a) Cuando los problemas involucren más de un medio es necesario decir que cada medio tiene
un campo eléctrico y vector densidad de corriente respectivo. En este caso, el medio g1 tiene
~ 1 (r) y vector densidad de corriente J~1 (r), análogamente el medio g2
un campo eléctrico E
~ 2 (r) y J~2 (r). Por condición de borde, se tiene que el campo eléctrico es tangente
tiene un E
~ 1 (r) = E
~ 2 (r) = E(r).
~
(o paralelo) a la interfase entre los medios, por lo cual se cumple que E
Luego, la corriente eléctrica total que circula desde el cilindro interior al exterior está dada
por
¨
ˆβ ˆL
ˆ2π ˆL
~
I=
J~ · dS =
J1 (r)rdθdz +
J2 (r)rdθdz

β

Problemas Propuestos y Resueltos de Electromagnetismo

ρ(x, y, t = 0) = F (x) = ρ0 e−α(x +y ) =⇒ ρ(x, y, t) = ρ0 e−α((x−v0 t) +y )

---

### Página 190

CAPÍTULO 8. MEDIOS CONDUCTORES
Por Ley de Ohm J1 = g1 E(r) y J2 = g2 E(r), luego
I = g1 E(r)rβL + g2 E(r)r(2π − β) =⇒ E(r) =

I
rL(g1 β + g2 (2π − β))

Falta relacionar este valor de campo eléctrico con la diferencia de potencial entre los casquetes, por lo que debe cumplirse que
ˆb
V0 =
a

b
I
ln
E(r)dr =
L(g1 β + g2 (2π − β))
a

!

=⇒ I =

V0 L(g1 β + g2 (2π − β))
ln

 
b
a

b) A partir de lo anteriormente calculado, se tiene en forma directa que
ln

 
b

V0
a
R=
=
I
L(g1 β + g2 (2π − β))
Por otro lado
ˆβ ˆL
I1 =

ln

a

I2 =
Finalmente

b

βg1 I
βg1 V0 L
a
  =⇒ R1 =
J1 (r)rdθdz =
=
b
(g1 β + g2 (2π − β))
βg1 L
ln

ˆ2π ˆL
β

 

ln

 
b

(2π − β)g2 I
a
=⇒ R2 =
J2 (r)rdθdz =
(g1 β + g2 (2π − β))
(2π − β)g2 L

L(g1 β + g2 (2π − β))
 
=
+
=
R1 R2
R
ln b
a

Rodrigo Chi - Marzo 2017

Solución 8.5

P X

Como la diferencia de potencial entre las caras es conocida, basta encontrar la resistencia que
provoca el material para encontrar la corriente que lo atravesará. Para encontrar en este caso la
resistencia, se divide en trozos infinitesimales el paraboloide, de modo de luego integrar en cada uno
y encontrar la resistencia total. La sección transversal de un paraboloide es una circunferencia,
luego el trozo infinitesimal es un disco de altura dz y radio r, luego usando la definición de
resistencia dada su geometría
ηL
ηdz
dR =
= 2
A
πr
En coordenadas cilíndricas, r = x + y = 4z por lo tanto
ˆz2
R=
z1

ηdz
η
z2
=
ln
4πz
4π
z1




---

### Página 191

CAPÍTULO 8. MEDIOS CONDUCTORES
Solución 8.9

P X

a) De la ecuación de continuidad y considerando que se ha alcanzado el régimen estacionario,
se tiene
~ · J~ = 0
∇
Considerando la ley de Ohm y desarrollando la expresión:
~ · (g(x) · E(x))
~
∇
=0
!

∂V
∂
g(x) · −
=0
∂x
∂x
∂g ∂V
∂ 2V
·
+ g(x) 2 = 0
∂x ∂x
∂x
g0 (x + a) ∂ 2 V
g0 ∂V
+
=0
a ∂x
a
∂x2
1 ∂V
∂ 2V
+
=0
∂x
x + a ∂x
Nótese que se ha encontrado la ecuación diferencial pedida. Para resolverla se toma el
cambio de variable µ = ∂V
:
∂x

Para determinar la diferencia de potencial entre S y S 0 , se encuentra el valor de C1 usando
la condición de borde dada
~ = − ∂V x̂ = − C1 x̂
E
∂x
x+a
~ = 0) = − C1 x̂ = E0 x̂
E(x
a
=⇒ C1 = −E0 a
~ = E0 a x̂
=⇒ E
x+a
Finalmente, al reemplazar C1 , V (x) = −E0 a ln(x + a) + C2
V (S) − V (S 0 ) = −E0 a ln(a) + E0 a ln(2a) = E0 a ln(2)

Problemas Propuestos y Resueltos de Electromagnetismo

dµ
+
µ=0
dx x + a
dx
dµ
=−
=⇒ ln µ = − ln(x + a) + C
µ
x+a
C1
=⇒ µ =
x+a
dV
C1
=⇒
=
dx
x+a
=⇒ V (x) = C1 ln(x + a) + C2

---

### Página 192

CAPÍTULO 8. MEDIOS CONDUCTORES
~ = E0 a x̂ y g(x) = g0 (x+a) , se tiene que
b) Considerando que E
x+a
a
g0 (x + a)
E0 a
J~ =
·
x̂ = g0 E0 x̂
a
(x + a)
Con esto es posible calcular corriente considerando que el flujo atraviesa un área cuadrada
de lado a:
¨
ˆa ˆa
~ =
I=
J~ · dS
g0 E0 dydz = g0 E0 a2

, usando el resultado recién obtenido para I y el de ∆V de la parte
Además como R = ∆V
I
(a), se concluye:
∆V
E0 a ln(2)
ln(2)
R=
=
=
I
g0 E0 a
g0 a
Finalmente, la carga encerrada se calcula usando Ley de Gauss:
¨
¨
¨
Qenc
~
~ = Qenc
~
~
~ · dS
~
=⇒
E · dS +
E
E · dS =
ε0
ε0
S0

S

cubo

E0 2 Qenc
a =
ε0
ε 0 E 0 a2
=⇒ Qenc = −

−E0 a2 +

Rodrigo Chi - Marzo 2017

Solución 8.10

P X

Asumiendo que el sistema está en estado estacionario y dada la simetría radial del problema, se
debe cumplir que
~ · J~ = 1 ∂(r Jr ) = 0 =⇒ J~ = C r̂
∇
r2 ∂r
r2
~
Donde C es una constante por determinar. Usando lo anterior, se procede a relacionar J~ con E,
de modo que
~ = (kE)E
~ = kE 2 r̂
J~ = g E
Por lo tanto
C
kE 2 = 2 =⇒ E =
r
r

s

C
k

Ahora, para encontrar C se utilice el hecho que la diferencia de potencial entre los casquetes
esféricos es conocida, luego
ˆb

s

~ =⇒ V =
~ · dl
E

V =

C
b
ln
k
a

a

!

=⇒ C =

kV 2
ln2 ( ab )

---

### Página 193

CAPÍTULO 8. MEDIOS CONDUCTORES
Donde se deduce que
~ =
E

V
r̂
r ln( ab )

Ya teniendo el campo, es directo que la corriente encontrada se calcula como
¨
I=

ˆ2π ˆπ
~ =
J~ · dS

ˆ2π ˆπ
2 2

kE r sin(θ)dθdϕ ==

kV 2
4πkV 2
r sin(θ)dθdϕ = 2 b
r2 ln2 ( ab )
ln ( a )

Finalmente, la densidad de carga está dada por
~ =
ρ = ε0 ∇ · E

Solución 8.13

V
r2 ln( ab )

P X

a) Como sistema de referencia se tomará z creciente hacia abajo. Para el condensador de la
izquierda:
J1n = J2n =⇒ J~1 = J~2 = J~
(vector densidad de corriente constante en ambos medios). Suponiendo estado estacionario
dentro del condensador
~ · J~ = 0 =⇒ dJ = 0 =⇒ J~ = Aẑ
∇
dz

ˆd
V (z = 2d) − V (z = 0) = −V0 = −

A
dz −
g1

ˆ2d

A
Ad Ad
V0 g1 g2
dz = −
−
=⇒ A =
g2
g1
g2
d(g1 + g2 )

d

Por lo tanto
J~ =

V0 g1 g2
ẑ
d(g1 + g2 )

~1 =
E

V0 g2
V0 g1
~2 =
ẑ , E
ẑ
d(g1 + g2 )
d(g1 + g2 )

~1 =
D

ε1 V0 g2
~ 2 = ε2 V0 g1 ẑ
ẑ , D
d(g1 + g2 )
d(g1 + g2 )

Para el condensador de la derecha:
~1 = E
~2 = E
~
E1t = E2t =⇒ E

Problemas Propuestos y Resueltos de Electromagnetismo

donde A es una constante por determinar. Por lo tanto el campo eléctrico en cada medio
está dado por
~ 2 = A ẑ
~ 1 = A ẑ , E
E
g1
g2
La constante A puede ser determinada como

---

### Página 194

CAPÍTULO 8. MEDIOS CONDUCTORES
(campo eléctrico constante en ambos medios). Luego, dado que no hay densidades volumétricas de carga del condensador
~ ·E
~ = 0 =⇒ dE = 0 =⇒ E
~ = C ẑ
∇
dz
donde C es una constante por determinar. La constante C puede ser determinada como
ˆ2d
V (z = 2d) − V (z = 0) = −V0 = −

Cdz =⇒ C =

V0
2d

Por lo tanto
~ = V0 ẑ
E
2d
g1 V0
g2 V0
J~1 =
ẑ , J~2 =
ẑ
2d
2d
~ 1 = ε1 V0 ẑ , D
~ 2 = ε2 V0 ẑ
D
2d
2d
b) Para el condensador de la derecha, se tienen las siguientes densidades polarización
σP 1 (z = 0) = (ε1 − ε0 )

V0
V0
ẑ · −ẑ = −(ε1 − ε0 )
2d
2d

σP 1 (z = 2d) = (ε1 − ε0 )
σP 2 (z = 0) = (ε2 − ε0 )

Rodrigo Chi - Marzo 2017

σP 2 (z = 2d) = ε2

V0
V0
ẑ · ẑ = (ε1 − ε0 )
2d
2d

V0
V0
ẑ · −ẑ = −(ε2 − ε0 )
2d
2d

V0
V0
ẑ · ẑ = (ε2 − ε0 )
2d
2d

Mientras que las de carga libre son
σL1 (z = 0) = ε1

V0
V0
ẑ · ẑ = ε1
2d
2d

σL1 (z = 2d) = ε1

V0
V0
ẑ · −ẑ = ε1
2d
2d

σL2 (z = 0) = ε2

V0
V0
ẑ · ẑ = ε2
2d
2d

σL2 (z = 2d) = ε2

V0
V0
ẑ · −ẑ = −ε2
2d
2d

No hay densidades volumétricas de ningún tipo dentro del condensador.

---

### Página 195

CAPÍTULO 8. MEDIOS CONDUCTORES
c) En este caso hay que notar que el capacitor de la izquierda puede ser dividido en dos
capactores en serie, mientras que el capacitor de la derecha puede ser dividido en dos en
paralelo. Usando el resultado conocido de la capacitancia de un condensador de placas
paralelas C = εA
, se tiene que:
L
CT =

d
d
+ ε2 4a
ε1 4a2
|

{z

}

+

Capacitancia de la izquierda

ε1 2a2 ε2 2a2
+
| 2d {z 2d }

ε 1 a2 ε 2 a2
4a2 ε1 ε2
+
+
=
d(ε1 + ε2 )
d
d

Capacitancia de la derecha

d) La corriente total que sale de la fuente puede ser determinada integrando los vector densidad
~ y los dos vectores densidad de
de corriente que pasa por el condensador de la izquierda (J)
corriente que pasan por el condensador de la derecha (J~1 y J~2 ). Por lo tanto:
ˆ2a ˆ2a
I=

V0 g1 g2
dxdy +
d(g1 + g2 )

ˆ2a ˆa

V0 a2 g1 g2
I=
d

g1 V0
dxdy +
2d

ˆ2a ˆ2a

+
+
g1 + g2 g2 g1

g2 V0
dxdy
2d

a

!

Por lo tanto la resistencia equivalente es
R=

Solución 8.14

V0

=
I
a2 g1 g2

d
+ g12 + g11
g1 +g2



a) Aplicando la condición de solución estacionaria en la ecuación de conservación de carga, se
tiene que:
~ · J~ = 1 ∂ (rJ(r)) = 0 =⇒ rJ(r) = A =⇒ J(r)
~ = A r̂
∇
r ∂r
r
De esta manera, debido a lo anterior, la geometría cilíndrica y la continuidad de J~ (por
condición de borde), se puede asumir una corriente I = cte circulando por el sistema, con
¨
¨
A
~
~
rdθdz = 2πLA =⇒ I = 2πLA = cte.
I=
J · dS =
r
Por lo tanto, asumiendo una corriente I en el sistema, se tendrá
I
I
J~ =
r̂ =
r̂
2πrL
área

~1 =
E

=⇒

I
r̂;
2πrLg1

~2 =
E

I
r̂
2πrLg2

~1 y E
~ 2 son los campos eléctricos en las zonas con conductividades g1 y g2 respecDonde E
tivamente. A partir de estos campos es posible calcular la diferencia de potencial V0 entre

Problemas Propuestos y Resueltos de Electromagnetismo

P X

---

### Página 196

CAPÍTULO 8. MEDIOS CONDUCTORES
los radios a y c
ˆa

ˆb
~ · d~r = −
E

V0 = −

ˆa
~ 2 · d~r −
E

c

c

~ 1 · d~r = I
E
2πL

ln( cb ) ln( ab )
+
g2
g1

!

b

Y de lo anterior se despeja I
I=

2πLV0
ln( cb )
g2

+

ln( ab )
g1

2πLV0 g1 g2
g1 ln( cb ) + g2 ln( ab )

 =

Finalmente, reemplazando el ahora conocido valor de I en las expresiones anteriores para
~ E
~ 1, y E
~2
J,
V0 g2
~1 =
r̂
E
c
r(g1 ln( b ) + g2 ln( ab ))
~2 =
E

V0 g1
r̂
c
r(g1 ln( b ) + g2 ln( ab ))

J~ =

V0 g1 g2
r̂
r(g1 ln( cb ) + g2 ln( ab ))

~ · n̂, se tiene que en la placa interior, dónde el radio es r = a
b) Usando el hecho que σ = ε0 E
σa = ε0 E1 (a) =⇒ Qa = 2πaLσa =

2πLV0 ε0 g2
(g1 ln( cb ) + g2 ln( ab ))

De manera análoga en r = c
σc = −ε0 E2 (c) =⇒ Qc = 2πcLσc = −

2πLV0 g1 ε0
(g1 ln( cb ) + g2 ln( ab ))

Rodrigo Chi - Marzo 2017

c) De los resultados anteriores
I=

2πLV0
ln( b )
ln( c )
( g2b + g1a )

=

2πLV0 g1 g2
g1 ln( cb ) + g2 ln( ab )

d) La resistencia, se obtiene del cuociente
V0
R=
=
I
2πL

ln( cb ) ln( ab )
+
g2
g1

!

e) Aquí primero se debe observar que las resistencias RL y R están en serie. Luego, sea V1 el
voltaje en la resistencia RL , por LVK y LCK se tiene
V0 = I(R + RL );

V1 = IRL

---

### Página 197

CAPÍTULO 8. MEDIOS CONDUCTORES
Eliminando I de estas dos ecuaciones resulta
V1 =

RL
V0
R + RL

A este resultado genérico, de la caida de potencial en dos resistencias en serie con una
fuente se le conoce como = Divisor de voltaje”. Ahora se puede calcular la potencia disipada
en la resistencia RL
V2
RL V02
P = V1 I = 1 =
RL
(RL + R)2
Ahora, para maximizar la potencia en función de RL
dP
2RL
= V02
−
dRL
(R + RL )
(R + RL )3

!

= 0 =⇒ RL = R =
2πL

ln( cb ) ln( ab )
+
g2
g1

!

Es la resistencia RL que maximiza la potencia disipada en ella. Y dicha potencia máxima
vale
V2
V02 πLg1 g2
P = 0 =
4R
2(g1 ln( cb ) + g2 ln( ab ))

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 198

CAPÍTULO 8. MEDIOS CONDUCTORES

IV.

Indicaciones Problemas Sin Solución

Indicación 8.1

P X

Recuerde que ~r = rr̂ en coordenadas esféricas y use la ecuación de continuidad para despejar
el valor de ρ. Con ello podrá encontrar los valores buscados de f y g.

Indicación 8.3

P X

~ = E(r)r̂. Por condiciones de
Recuerde que por la simetría del problema J~ = J(r)r̂ y E
~
borde, existe un único vector J(r)
entre los cascarones.
Una vez determinado J~ es posible determinar la intensidad de corriente. Dado que la diferencia de potencial es conocida, el valor de la resistencia es directo por ley de Ohm.
En este caso es necesario usar σ = ε0 E2n − ε0 E1n . Nótese que cada medio tiene su propia
función campo eléctrico y que la interfase se ubica en r = 2a.

Indicación 8.6

P X

Divida en trozos infinitesimales el anillo, para ello use anillos muy delgados de ancho dr y
altura d

Rodrigo Chi - Marzo 2017

Note que todos los anillos infinitesimales quedan como un conjunto de resistencias en paralelo.

Indicación 8.7

P X

Asuma una carga Q y −Q en cada esfera (ambas cargas distribuyen uniformemente debido
a que están muy alejadas).
Por simetría y condición de borde, el campo eléctrico es tangencial a la interfase. Luego,
el campo eléctrico es independiente del medio g. Dado esto, determine la diferencia de
potencial entre las esferas.
~ es posible determinar J~ y con ello la corriente que va de una esfera a otra.
Conocido E,
Concluya el problema.

---

### Página 199

CAPÍTULO 8. MEDIOS CONDUCTORES
Indicación 8.8

P X

~ · J~ = 0 =⇒ J~ = J0 ẑ, donde J0 es una
Asumiendo estado estacionario, se tiene que ∇
~ es posible conocer fácilmente el campo
constante desconocida. Luego dado que J~ = g(z)E
eléctrico.
Para conocer la potencia disipada es aplicación directa de la fórmula de pérdidas por efecto
Joule.

Indicación 8.11

P X

La esfera se está descargando en el tiempo, por lo cual la carga sobre ella es Q(t) con la
condición inicial Q(t = 0) = Q0 .
Integre en un volumen a ambos lados de la ecuación de continuidad. Use el teorema de la
divergencia para simplificar un lado. Haciendo esto, debería llegar a una ecuación diferencial
de Q(t).
La energía que se disipa es la misma que se necesita para poner la carga Q0 sobre la esfera
en t = 0.

Indicación 8.12

P X

Ahora, usando la Ley de Ohm relacione el campo eléctrico con la densidad de corriente y
determine la corriente que sale de uno de los conductores.

Problemas Propuestos y Resueltos de Electromagnetismo

Usando la Ley de Gauss encuentre el flujo de campo eléctrico que saldrá de uno de los
conductores.

---

### Página 200

CAPÍTULO 8. MEDIOS CONDUCTORES

V.

Respuestas
Problema

Respuestas

P

8.1

C
f (r) = − αr
2 , g(r) = 2C.

P

8.2

ρ(x, y, t) = ρ0 e−α((x−v0 t) +y )

P

g1 +3g2
a) R = 24πag
1 g2

8.3

0 ε0 (g1 −g2 )
b) σ = 3V2a
(g1 +3g2 )

LV0
a) I = ln(a/b)
(βg1 + (2π − β)g2 )

P

b) R1 = ln(a/b)
Lβg1
8.4

ln(a/b)
R2 = L(2π−β)g

RT = L(βg1ln(a/b)
+(2π−β)g2 )


8.5

η
R = 4π
ln

P

8.6

π
R = gd ln(1+
d
)

P

8.7

R = 2πg
( a11 + a12 − L2 )

P

Rodrigo Chi - Marzo 2017



P

P

z2
z1

r

V0
~ =
ŷ
a) J~ = LV0lng02 ŷ, E
L(1+ y ) ln 2
L

8.8

8.9

b)

V02 g0
P = πa2 L ln
2 2 ln

a)

∂2V
1 ∂V
∂x2 + x+a ∂x

2e
1 + 3L



= 0, V (S) − V (S 0 ) = E0 a ln(2)

ε 0 E0 a
b) R = ln(2)
g0 a , Q = −

---

### Página 201

CAPÍTULO 8. MEDIOS CONDUCTORES
Problema

P

Respuestas

8.10

V
I = 4πkV
, ρ = r2 ln(
b
ln( b )2
)
a

a

g

P

8.11

a) Q(t) = Q0 e− ε0 t
Q0
b) U = 8πε
0a

a) Condensador izquierda:
V0 g1 g2
~1 =
ẑ, E
J~ = d(g
1 +g2 )

V0 g2
~
d(g1 +g2 ) ẑ, E2

V0 g1
~
d(g1 +g2 ) ẑ, D1

=

=

ε1 V0 g2
~
d(g1 +g2 ) ẑ, D2

=

ε2 V 0 g 1
d(g1 +g2 ) ẑ

Condensador derecha:
~ 1 = ε1 V0 ẑ, D
~ 2 = ε2 V0 ẑ
~ = V0 ẑ, J~1 = g1 V0 ẑ, J~2 = g2 V0 ẑ, D
E
2d

P

8.13

2d

2d

d) R =

d
a2 g 1 g 2

g1 +g2 + g2 + g1



a<r<b
b<r<c

2πLV0 g2 ε0
2πLV0 g1 ε0
b) σ(r = a) = (g1 ln(c/b)+g
, σ(r = c) = − (g1 ln(c/b)+g
2 ln(b/a))
2 ln(b/a))
2πLV0 g1 g2
c) I = g1 ln(c/b)+g
2 ln(b/a)


ln(c/b)
ln(b/a)
d) R = 2πL
+
g2
g1


V02 πLg1 g2
ln(c/b)
e) RL = 2πL
+ ln(b/a)
, P = 2(g1 ln(c/b)+g
g2
g1
2 ln(b/a))

Problemas Propuestos y Resueltos de Electromagnetismo

V0 g1 g2
a) J~ = r(g1 ln(c/b)+g
r̂,
2 ln(b/a))

V0 g2

 r(g1 ln(c/b)+g2 ln(b/a)) r̂
~ =
E

V0 g1

r(g1 ln(c/b)+g2 ln(b/a)) r̂

8.14

2d

b) Densidades superficiales de polarización:
σP 1 (z = 0) = −(ε1 − ε0 ) V2d0 , σP 1 (z = 2d) = (ε1 − ε0 ) V2d0 , σP 2 (z = 0) =
−(ε2 − ε0 ) V2d0 , σP 2 (z = 2d) = (ε2 − ε0 ) V2d0
Densidades superficiales de carga libre:
σL1 (z = 0) = ε1 V2d0 , σL1 (z = 2d) = ε1 V2d0 , σL2 (z = 0) = ε2 V2d0 , σL2 (z = 2d) =
−ε2 V2d0
No existen densidades volumétricas de carga de ningún tipo.
4a ε1 ε2
c) CT = d(ε
+ ε1da + ε2da
1 +ε2 )

P

2d

---

### Página 202

Rodrigo Chi - Marzo 2017

CAPÍTULO 8. MEDIOS CONDUCTORES

---

### Página 203

Circuitos Eléctricos

I.

Resumen Teórico

Ley de Ohm, Potencia y Asociación de Resistencias
La ley de Ohm aplicada a un circuito eléctrico es
V = RI

(9.1)

Req =

n
X

Ri

(9.3)

i=1

Mientras que para el caso de asociación en paralelo se tiene que
Req =

n
X

!−1

i=1 Ri

(9.4)

Leyes de Kirchhoff
La primera ley de Kirchhoff señala que: la suma de las corrientes que entran en un nodo es igual
a la suma de las corrientes que salen de él.
n
X

Ii = I1 + I2 + I3 · · · + In = 0

i=1

(9.5)

Problemas Propuestos y Resueltos de Electromagnetismo

Debido a las perdidas de potencia en forma de calor que provocan las resistencias esta puede ser
determinada como
V2
P = V I = RI 2 =
(9.2)
R
Finalmente, las resistencias pueden ser asociadas en serie o paralelo dependiendo de como se
conecten. En el caso de la conexión de n resistencias en serie se tiene que

---

### Página 204

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS
La segundo ley de Kirchhoff señala que: la suma de las diferencias de potencial eléctrico en una
malla cerrada siempre debe ser nula.
n
X

Vi = V1 + V2 + V3 · · · + Vn = 0

(9.6)

i=1

Recomendaciones

Rodrigo Chi - Marzo 2017

En muchos casos no podrá encontrar la resistencia equivalente reduciendo resistencias en
serie y paralelo. En ese caso debe determinar cuanta es la corriente que entra el circuito si
este se conecta a una diferencia de potencial conocida. Finalmente, debe aplicar la ley de
Ohm para despejar el valor de la resistencia.

---

### Página 205

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS

II.

Problemas Propuestos

#### Problema 9.1

R1

X I

En el circuito de la figura, encuentre el valor de R1
de manera que la resistencia equivalente entre las terminales (donde está abierto el circuito) sea igual a
R0 .

R0

R1

X S

15 W

10 W

Una resistencia R se conecta entre los terminales A
y B del circuito de la figura. Calcule el valor de la
resistencia R de manera que:
a) La potencia disipada en el circuito sea máxima.
Determine el valor de esa potencia.

120 V

+

#### Problema 9.2

R1

A

10 W

R

b) La potencia disipada en la resistencia R sea
máxima. Determine el valor de esa potencia.
#### Problema 9.3

B

X I
R

R
R

a

R
R

a) Calcule la resistencia equivalente de este circuito entre los puntos a y b.

R

b

R
R

R

b) Calcule la corriente de cada una de las 9 resistencias.
100 W

X I

En el circuito de la figura, el amperímetro A registra
una corriente I cuandos ambos interruptores están
abiertos o ambos cerrados. Hallar el valor de la resistencia R.

A

R

50 W

300 W
+

#### Problema 9.4

1.5 [V ]

Problemas Propuestos y Resueltos de Electromagnetismo

Nueve resistencias R de 10 Ω están conectadas como
se muestra en la figura y una diferencia de potencial
20 V. se aplica entre los puntos a y b .

---

### Página 206

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS

A

#### Problema 9.5

X I

Considere un cubo el cual posee en cada arista una resistencia R. Determine la resistencia equivalente entre
dos vértices opuestos A y B.
B

#### Problema 9.6

X I

R

Encuentre la pérdida de energía en forma de calor en
el circuito de la figura. Demuestre que éste número
no depende de la resistencia R, teniendo en cuenta
que inicialmente el condensador de capacidad C1 tiene
carga Q0 y que el segundo condensador se encuentra
descargado.

C2

X I

Considere el circuito de la figura. Antes de t = 0,
el switch está en la posición 1 por un tiempo muy
prolongado. En t = 0, el switch S es movido a la
posición 2. Calcule:

R

R

a) La carga en el condensador en t = 0, Q(0).
b) La corriente en t = 0 después de que el switch V
es movido a la posición 2, I(0).
c) La corriente para t > 0, después de que el switch
fue movido a la posición 2.
d) La energía U almacenada en el condensador en
t = 0.

R

+

Rodrigo Chi - Marzo 2017

#### Problema 9.7

C1

C

---

### Página 207

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS
#### Problema 9.8

X I

Un condensador, de capacidad C, formado por placas
circulares de radio b está cargado y con voltaje V0 . La
separación entre las dos placas paralelas es pequeña
comparada con b. En t = 0 se cierra el switch y el condensador comienza a descargarse. Calcule, en función
de V0 , C, b, R, t:

+Q0
R

C
Q0

a) La carga Q(t) en función del tiempo para la
placa cargada positivamente del condensador.
~ en el espacio entre las dos
b) El campo eléctrico E
placas del condensador.

#### Problema 9.9

X S

En una red eléctrica hay n resistencias que cruzan
desde la línea superior a la línea inferior, y hay n − 1
resistencias a lo largo de la línea superior e inferior. El
número total de resistencias es 3n − 2. Todas las resistencias son iguales y de valor R. Determine el valor
de R1 , R2 , R3 y R∞ (Ri es la resistencia equivalente
vista desde los terminales para el caso n = i). En la
Figura se muestra el caso n = 4.

X S

+

E

+

Circuito Serie

E

Ri
+

Batería N

Ri

E
Circuito Paralelo

Ri

R

+

Se tiene N baterías, cada una con la misma fuerza electromotriz E y la misma resistencia interna Ri .
Ellas pueden ser conectadas todas en serie o bien todas en paralelo y, en ambos casos, el circuito es cerrando con una resistencia adicional R. Determine las
potencias Pser y Ppar que se disipan en R en cada uno
de los dos casos. Encuentre el valor Rser de R que
permite obtener el mayor valor para Rser y encuentre
el valor Rpar de R que permite obtener el mayor valor para Ppar . Determine en cuál de los dos casos la
potencia disipada en R es mayor.

Batería 1

#### Problema 9.10

Batería N

Ri

R

Problemas Propuestos y Resueltos de Electromagnetismo

Batería 1

E

---

### Página 208

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS

III.

Soluciones

Solución 9.2

P X

a) Primero se debe calcular el valor de la resistencia R, tal que el valor de la potencia total
disipada en el circuito se maximice. En este caso, se calcula la resistencia equivalente del
circuito considerando un valor desconocido R. Luego
+
Req = 10 +
10 15 + R


−1

=

400 + 20R
25 + R

(en Ω)

Entonces la potencia está dada por
P (R) =

V2
25 + R
= 1202 ·
Req
400 + 20R

(en [W ])

Para maximizar, se deriva la expresión anterior con respecto a R
dP
400 + 20R − 20(25 + R)
1202 · 100
= 1202 ·
=
−
<0
dR
(400 + 20R)2
(400 + 20R)2
Dado que la función potencia tiene derivada negativa, es siempre decreciente para R ≥ 0,
por lo que su máximo lo alcanza en su mínimo valor, o sea R = 0 Ω. Por lo tanto la potencia
disipada vale
P = 900 [W ]
b) Ahora hallar el valor de la resistencia R de modo que se maximice la potencia disipada en
en si misma. En este caso es necesario plantear las leyes de Kirchhoff:

Rodrigo Chi - Marzo 2017

0 = (15 + R)IR − 10(I − IR )
120 = 10I + 10(I − IR )
Donde I es la corriente que sale de la fuente, e IR es la corriente sobre la resistencia
desconocida. Reordenando las ecuaciones:
10I = (25 + R)IR
120 = 20I − 10IR
De estas dos ecuaciones se obtiene que:
=⇒ PR = RIR2 = R
20 + R
20 + R


IR =
Luego:

2

---

### Página 209

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS

dP
2 (20 + R) − 2R(20 + R)
= 60
dR
(20 + R)4

!

= 0 =⇒ R = 20

Por lo tanto, el valor de la resistencia que maximiza la potencia disipada en ella es R = 20 Ω
y dicha potencia vale:
P = 20


Solución 9.9

2

= 45 [W ]

P X

En un principio hay que encontrar la recurrencia de la red de resistencias. Para el caso n = 1,
siguiendo todos los datos del enunciado se tiene

Figura 9.1: Red de Resistencias para n = 1

Figura 9.2: Red de Resistencias para n = 2
En este caso R2 =
+
R R+R+R


Donde R3 =
+
R R + R2 + R
de resistencias está dada por


−1

−1

=

Rn =

= R. Finalmente el caso R3 estará dado por

R. En este punto, es posible verificar que la recurrencia
+
R 2R + Rn−1

!−1

Problemas Propuestos y Resueltos de Electromagnetismo

Donde evidentemente R1 = R. Nuevamente cumpliendo los requisitos del enunciado R2 es

---

### Página 210

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS

Figura 9.3: Red de Resistencias para n = 3
(Nota: Si se desea ser riguroso este resultado debería ser demostrado por inducción, sin embargo
para no escapar de los contenidos del curso no se realizará la demostración) Ahora, se debe
suponer la sucesión de redes de resistencias converge a un valor R∞ , de modo que
lím Rn = n−→∞
lím Rn−1 = R∞

n−→∞

Luego, para n suficientemente grande se cumple que
+
R∞ =
R 2R + R∞


Solución 9.10

−1

√
=⇒ R∞
+ 2RR∞ − 2R2 = 0 =⇒ R∞ = ( 3 − 1)R

P X

En cada caso se puede calcular la potencia disipada por R como
P = RI 2
donde I corresponden a la corriente que pasa por la resistencia R. En el caso serie, la corriente
es la misma que circula en todo el circuito, luego por Kirchhoff se tendrá que
NE
NE
=⇒ Pser = R
N E − N Ri I − RI = 0 =⇒ I =
N Ri + R
N Ri + R
Otro lado, en la conexión en paralelo por las N fuentes debe salir la misma corriente. Entonces,
si por cada batería sale una corriente I/N por la resistencia pasará una corriente I. Por Kirchhoff
nuevamente
2

I
NE
NE
E − Ri − RI = 0 =⇒ I =
=⇒ Ppar = R
N
Ri + N R
Ri + N R
Para hallar los Rser y Rpar que maximizan la potencia hay que derivar e igualar a cero.

Rodrigo Chi - Marzo 2017



dPser
(N E)2 (N Ri + R)(N Ri − R)
=
= 0 =⇒ Rser = N Ri
dR
(N Ri + R)4
dPpar
(N E)2 (Ri + N R)(Ri − N R)
Ri
=
= 0 =⇒ Rpar =
dR
(Ri + N R)
N
Al evaluar las potencias en sus respectivas resistencias, se obtiene que
N E2
4Ri
Por lo que en ambos casos la potencia disipada es la misma.
Pser (Rser ) = Ppar (Rpar ) =



---

### Página 211

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS

IV.

Indicaciones Problemas Sin Solución

Indicación 9.1

P X

Realice asociaciones de serie y paralelo para encontrar la resistencia equivalente del circuito.
Una vez encontrada, imponga que ésta debe ser igual a R0 .

Indicación 9.3

P X

Para encontrar la resistencia equivalente determine la corriente que entra al circuito. Dado
que el voltaje es conocido, la resistencia equivalente puede ser determinada por la ley de
Ohm.
Use la simetría del circuito para aplicar las leyes de Kirchhoff. Note que las corrientes tienen
que ser simétricas, por lo cual sólo hay tres corrientes distintas circulando.

Indicación 9.4

P X

Indicación 9.5

P X

En este caso no puede usar asociaciones en serie/paralelo para determinar la resistencia
equivalente. Suponga que se conectan los terminales A y B a una batería V0 y determine
la corriente que sale de ella.
Use la simetría del circuito para ir viendo de que forma se dividen las corrientes, por ejemplo,
cuando la corriente que sale de la batería llega al primer vértice del cubo necesariamente se
divide en tres corrientes iguales por simetría.
Aplicando las leyes de Kirchhoff determine la corriente, y determine la resistencia equivalente
por ley de Ohm.

Problemas Propuestos y Resueltos de Electromagnetismo

Determine la corriente que circula por el amperímetro en los dos casos, una de ella debería
quedar en función R. Iguale los valores de esas corrientes y determine el valor de R.

---

### Página 212

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS
Indicación 9.6

P X

Usando las leyes de Kirchhoff, encuentre la ecuación diferencial que rige el circuito sobre
la carga Q. Recuerde que la caída/subida de tensión en un condensador está dado por
V = Q/C.
Dado que C1 se está descargando, es una subida de tensión (ie. actúa de forma parecida a
una fuente de voltaje), mientras que R y C2 son caídas de tensión.

Indicación 9.7

P X

Recuerde que la carga no puede variar en forma abrupta en condensador y que pasado un
tiempo muy largo el condensador actúa como un circuito abierto.

Indicación 9.8

P X

Determine la carga inicial del condensador si este se ha cargado a voltaje V0 .
Usando la ley de voltajes de Kirchhoff la ecuación diferencial que rige a la carga en el
circuito.

Rodrigo Chi - Marzo 2017

Conocida la carga en el tiempo que posee las placas, estime el valor del campo eléctrico
entre ellas.

---

### Página 213

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS

V.

Resultados
Problema

Respuestas

P

9.1

R0
R1 = √

P

9.2

a) R = 0 Ω , P = 900 [W ]
b) R = 20 Ω , P = 45 [W ]
a) Req = 53 R
V0
V0
b) Las corrientes son i1 = 2V
5R , i2 = 5R , i3 = 5R

P

9.3

P

9.4

R = 600Ω

P

9.5

RT = 56 R

P

9.6

0 C2
|∆U | = 2C1Q
(C1 +C2 )

(Nota: Las corrientes son simétricas, i1 es la corriente por la resistencia a la izquierda
R, i2 es la corriente que pasa por las tres resistencias en serie e i3 es la corriente
que pasa por la resistencia central de la figura).

a) Q(0) = CV
9.7

V
b) I(0) = 4R
V −t/2RC
c) I(t) = 4R
e

d) U (0) = CV8

−t

a) Q(t) = V0 Ce RC

P

9.8

−t

~ =
b) E

−V0 Ce RC
ẑ donde ẑ apunta desde la placa cargada positiva a la negativa.
πb2 ε0

Problemas Propuestos y Resueltos de Electromagnetismo

P

---

### Página 214

CAPÍTULO 9. CIRCUITOS ELÉCTRICOS
Problema

P

9.10

√
R1 = R, R2 = 34 R, R3 = 11
15 R, R∞ = ( 3 − 1)R.

Pser = R



NE
N Ri +R

2

, Ppar = R



NE
Ri +N R

Ppar (Rpar ) = N4REi

Rodrigo Chi - Marzo 2017

P

9.9

Respuestas

2

, Rser = N Ri , Rpar = RNi y Pser (Rser ) =

---

### Página 215

Parte III

Magnetostática

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 216

Rodrigo Chi - Marzo 2017

---

### Página 217

Ley de Biot-Savart

I.

Resumen Teórico

Ley de Biot-Savart
El campo magnético que genera una corriente I en un circuito puede ser determinado como
~ = µ0
B
4π

ˆ

~ × (~r − ~r 0 )
I dl
|~r − ~r 0 |3

(10.1)

donde ~r es el lugar donde se desea conocer el campo, ~r 0 es el lugar donde se encuentra la corriente
~ es el elemento vectorial que parametriza la dirección de la corriente.
y dl

~ = µ0
B
4π

¨ ~ 0
K(~r ) × (~r − ~r 0 )
dS
|~r − ~r 0 |3

(10.2)

~ = µ0
B
4π

˚ ~ 0
J(~r ) × (~r − ~r 0 )
dV
|~r − ~r 0 |3

(10.3)

~ r 0 ) = σ~v y J(~
~ r 0 ) = ρ~v . También puede ser útil recordar que ~v = ω
donde K(~
~ × ~r 0 , donde ω es
la velocidad con que rota la superficie o el volumen.
~ también cumple el principio de superposición.
Recordar que el campo magnético B

Recomendaciones
En general, se usa la ley de Biot-Savart para determinar el campo magnético en algunos
puntos específicos en el espacio (punto en particular, puntos sobre un eje, etc).

Problemas Propuestos y Resueltos de Electromagnetismo

Para el caso de distribuciones más complejas compuestas por cargas en movimiento con velocidad
~v , la expresión anterior cambia a

---

### Página 218

CAPÍTULO 10. LEY DE BIOT-SAVART
~ el primero hace referencia
A veces puede ser complicado diferenciar los vectores ~r 0 y dl,
al lugar donde se encuentra la la línea, superficie o volumen en el cual se desea integrar,
por otro lado el segundo indica la dirección (no necesariamente el sentido) que sigue la
corriente.
En muchos problemas deberá usar el principio de superposición, es decir, deberá dividir el
camino que sigue la corriente por trozos y determinar el aporte de cada uno en el punto
donde se desea conocer el campo magnético.
~ positivo, a pesar que la corriente pueda ir en el sentido
Se recomienda siempre elegir el dl
contrario a la de ese vector diferencial. El sentido de la corriente se controla más fácilmente
con los límites de la integral.

Rodrigo Chi - Marzo 2017

Siempre corrobore sus resultados usando la regla de la mano derecha para ver si el campo
magnético resultante tiene sentido. Los campos magnéticos siempre rotan entorno a
las corriente según la regla de la mano derecha.

---

### Página 219

CAPÍTULO 10. LEY DE BIOT-SAVART

II.

Problemas Propuestos

#### Problema 10.1

X I

I

Considere el alambre ABCDA que se muestra en la
figura. Por él circula una corriente I en la dirección
indicada. Si BC y DA son arcos de circunferencia
subtendidos por un ángulo α de modo que OA =
OD = R y OB = OC = 2R. Calcule el campo
~ que produce en el centro O.
magnético B

B

C
A

D
a
O
y

#### Problema 10.2

X I

P

Por un conductor rectilíneo semi-infinito circula una
corriente eléctrica de intensidad I en el sentido que se
~
muestra en la figura. Calcule el campo magnético B
en el punto P .

b
I
O

x

a

z

#### Problema 10.3

X I

P

a
a
y
I

x
z

#### Problema 10.4

P

X S

D

Un alambre en forma de L lleva corriente I. El alambre
coincide con el semeje x positivo y con el eje semipositivo y. Calcule el vector campo magnético en un
punto P del eje z, ubicado en z = D.

O

I
x

I

y

Problemas Propuestos y Resueltos de Electromagnetismo

Considere una espira cuadrada de lado a que yace
sobre el plano xy, por la cual circula una corriente I
mostrada en la Figura. Calcule el campo magnético
~ en un punto P , que está a una distancia z sobre el
B
centro del cuadrado.

---

### Página 220

CAPÍTULO 10. LEY DE BIOT-SAVART
#### Problema 10.5

X S

Susana, Rodrigo y Marcel, equipo docente de curso
de electromagnetismo de una cierta universidad, tienen una discusión sobre el campo magnético generado
por un alambre en un mismo punto P . Susana tiene
un alambre infinito por el cual fluye una corriente 2I,
Rodrigo, al ver el alambre lo toma y lo dobla, formando un cuarto de circunferencia de radio R más
otros dos tramos semi-infinitos (ver Figura). Rodrigo
le asegura a Susana que si la corriente disminuye a la
mitad, el campo magnético producido por esta nueva geometría tendrá una mayor magnitud en el punto
P (por lo cual Susana se muestra muy en desacuerdo). Marcel, asombrado por la discusión de su cuerpo
docente, les dice a ambos están equivocados ya que
falta información suficiente para aseverar en cual de
los dos casos el campo magnético es mayor. Ayude al
cuerpo docente de este curso a determinar quién tiene
la razón.

Susana:

2I
R
P

Rodrigo:
R
P

I

y

#### Problema 10.6

X S

Rodrigo Chi - Marzo 2017

Considere un alambre que ha sido doblado de la forma
θ
+1
que se indica la figura, siguiendo la curva r(θ) = 2π
en coordenadas cilíndricas dando n vueltas alrededor
del origen. Si por el alambre se hace circular una corriente I en sentido antihorario, determine el valor del
campo magnético en el origen y analice que sucede
cuando la cantidad de vueltas es muy grande.

x

y

#### Problema 10.7

I

X I

Considere un alambre infinito en el cual circula una
corriente I. El cable ha sido doblado de la forma que se
muestra en la Figura, con un ángulo de 2α. Determine
el campo magnético en cualquier punto del eje x.

a
a

x

---

### Página 221

CAPÍTULO 10. LEY DE BIOT-SAVART

z
#### Problema 10.8

X S

w

Considere un disco de radio R que posee una densidad de carga superficial σ, uniformemente distribuida.
Partiendo del reposo, el disco comienza a girar, hasta
alcanzar una velocidad angular constante ω en torno
a su eje de simetría. Encuentre una expresión para
el campo magnético en z = R. (Propuesto: ¿Cuánto
vale el campo magnético para cualquier punto en el
eje?).

#### Problema 10.9

s

R

X S

Considere un segmento AC recorrido por una corriente de intensidad I como se muestra en la Figura.

O

a) Determine el valor del campo magnético en el
punto O en función αA , αC y r

aC
aA

c) Demuestre que si n −→ ∞, el módulo del campo magnético en el centro del polígono coincide
con el de una espira circular de radio r.

#### Problema 10.10

r

A

P

I

C

I

X I

Encuentre el campo magnético en el punto P sobre
el eje de una bobina cilíndrica de radio a con una
densidad de n vueltas por unidad de largo que lleva
una corriente I. Exprese su respuesta en términos de
θ1 y θ2 (ver Figura).

z

P

a
q1
q2

Problemas Propuestos y Resueltos de Electromagnetismo

b) Use el resultado calculado en a) para determinar
el campo magnético producido por un polígono
regular de n lados en su centro. Considere que
el polígono es de lado a y es recorrido por una
corriente I.

---

### Página 222

CAPÍTULO 10. LEY DE BIOT-SAVART

III.

Soluciones

Solución 10.4

P X

Para el calculo del campo magnético se usará la definición
~ = µ0
B
4π

ˆ

~ × (~r − ~r 0 )
I dl
|~r − ~r 0 |3

Primero se calculará la contribución de campo magnético que genera el cable que está sobre el
~ = dxx̂. Luego
semi-eje positivo x. Nótese que en este caso ~r = z ẑ y ~r 0 = xx̂ y dl
~ 1 = µ0
B
4π
µ0
=
4π

ˆ
ˆ∞

µ0 I
=−
4π

~ × (~r − ~r 0 )
I dl
|~r − ~r 0 |3
Idxx̂ × (z ẑ − xx̂)
|z ẑ − xx̂|3
ˆ∞

zdx

(z 2 + x2 ) 2

ŷ

Usando el cambio de variables x = z tan θ =⇒ dx = z sec2 θdθ, por lo que si x → ∞ se tiene
π
que θ → .
π
ˆ2
z 2 sec2 θdθ
~ 1 = − µ0 I
B
3 ŷ
4π
(z 2 + z 2 tan2 θ) 2

π

=−

µ0 I
ŷ
4πz

ˆ2

cos θdθ

Rodrigo Chi - Marzo 2017

µ0 I
ŷ
=−
4πz
El otro aporte de campo magnético en ese punto está dado por la generación de campo magnético
en el semi-eje y. El campo estará dado por
~ 2 = µ0
B
4π
µ0
=
4π

ˆ
ˆ0
∞

µ0 I
=−
4π

~ × (~r − ~r 0 )
I dl
|~r − ~r 0 |3
Idy ŷ × (z ẑ − y ŷ)
|z ẑ − y ŷ|3
ˆ∞

zdy

(z 2 + y 2 ) 2

x̂

---

### Página 223

CAPÍTULO 10. LEY DE BIOT-SAVART
La última integral es idéntica a la que ya se calculó en la parte anterior (sólo cambia la dirección).
Finalmente el campo total es
~ = D) = B
~ 1 (z = D) + B
~ 2 (z = D) = − µ0 I (x̂ + ŷ)
B(z
4πD

Solución 10.5

P X

En este caso se elige el mismo sistema de referencia para ambos problemas, en este caso tomamos
el origen en el punto P y con eje x creciente a la derecha e y creciente hacia arriba. Para encontrar
los campos magnéticos se usará definición
~ = µ0
B
4π

ˆ

~ × (~r − ~r 0 )
I dl
|~r − ~r 0 |3

~ = 2Idxx̂ con x ∈ (−∞, ∞)
Caso Susana: ~r = 0, ~r 0 = Rŷ + xx̂, I dl
ˆ∞

~ S (P ) = µ0
B
4π

ˆ∞

2Idxx̂ × (−Rŷ − xx̂)
µ0 IRẑ
=−
| − Rŷ − xx̂|
2π

−∞

−∞

(x2 + R2 )

dx = −

µ0 IRẑ 2
µ0 I ẑ
· 2 =−
2π R
πR

(la última integral puede resolverse con el cambio de variables x = R tan θ)
Caso Rodrigo: En este caso hay que separar en tres caminos:

ˆ0

~ 1 (P ) = µ0
B
4π

µ0 IRẑ
Idxx̂ × (−Rŷ − xx̂)
=−
| − Rŷ − xx̂|
4π

−∞

ˆ0

−∞

(x2 + R2 ) 2

dx = −

µ0 I ẑ
µ0 IRẑ 1
· 2 =−
4π
R
4πR

~ = IRdθθ̂ con θ ∈ ( π , 0)
Trozo de cuarto de circunferencia: ~r = 0, ~r 0 = Rr̂, I dl
~ 2 (P ) = µ0
B
4π

ˆ0
π

IRdθθ̂ × (0 − Rr̂)
µ0 I ẑ
=
| − Rr̂|3
4πR

ˆ0
dθ = −
π

µ0 I ẑ
8R

~ = Idy ŷ con y ∈ (0, ∞)
Recta semi-infinita sobre el eje y: ~r = 0, ~r 0 = Rx̂ + y ŷ, I dl
~ 3 (P ) = µ0
B
4π

ˆ∞

Idy ŷ × (−Rx̂ − y ŷ)
µ0 IRẑ
=−
| − Rx̂ − y ŷ|
4π

ˆ0

y

∞

(y 2 + R2 ) 2

dy = −

µ0 IRẑ 1
µ0 I ẑ
· 2 =−
4π
R
4πR

Problemas Propuestos y Resueltos de Electromagnetismo

~ = Idxx̂ con x ∈ (−∞, 0)
Recta semi-infinita sobre el eje x: ~r = 0, ~r 0 = Rŷ + xx̂, I dl

---

### Página 224

CAPÍTULO 10. LEY DE BIOT-SAVART
(Idéntico al primer cálculo)
Por lo tanto el campo total es:
~ R (P ) = B
~1 + B
~2 + B
~ 3 = − µ0 I
B
2R



1 1
+
ẑ
π 4


Finalmente, debe notarse que
µ0 I
~S|
|B
~ S | > |B
~ R|

 =
= µ I πR
> 1 =⇒ |B
~
4+π
|BR |
+
π

2R

Dado que todos los datos de la expresión son conocidos, Susana tiene la razón.

Solución 10.6

P X

~ = drr̂ + rdθθ̂,
En este caso se debe aplicar nuevamente Biot-Savart, con ~r = 0, ~r 0 = rr̂, dl
nótese que independientemente que la geometría de este problema sea más compleja, las parametrizaciones en coordenadas cilíndricas (o polares en este caso) son siempre de la misma forma.
Entonces
µ0
~
B(0)
=
4π

ˆ2πn

µ0 I
I(drr̂ + rdθθ̂) × −rr̂
=
| − rr̂|
4π

ˆ2πn

(drr̂ + rdθθ̂) × −rr̂
| − rr̂|3

Finalmente,

Rodrigo Chi - Marzo 2017

µ0 I ẑ
~
B(0)
=
4π

ˆ2πn

dθ
µ0 I ẑ
=
r
4π

Solución 10.8

ˆ2πn

dθ
µ0 I ẑ
θ
=
· 2π ln
+1
θ
4π
2π
+1
2π

! 2πn

P X

Calculando el campo magnético por definición, se tiene que
~ =
dB

~ × (~r − ~r 0 )
µ0 I dl
4π |~r − ~r 0 |3

aquí
~ =
I dl

~
dq ~
dl
dl = dq = σdS · ~v = σrdrdθ · ~v
dt
dt

=

µ0 I ẑ
ln (n + 1)

---

### Página 225

CAPÍTULO 10. LEY DE BIOT-SAVART
Luego, dado que ~r = Rẑ, ~r 0 = rr̂ y ~v = ω
~ × ~r 0 = ωrθ̂ se tiene que
µ0
~
B(Rẑ)
=
4π

ˆ2π ˆR

σrdrdθ · ωrθ̂ × (Rẑ − rr̂)

ˆ2π ˆR



(R2 + r2 ) 2

=

µ0 

4π

σRωr drdθ

(R2 + r2 ) 2

ˆ2π ˆR

r̂ +



σωr drdθ 
3 ẑ 
(R2 + r2 ) 2

Por asuntos de simetría la primera integral es nula, por lo que el campo magnético es
~ = µ0 σω
B

ˆR

r3 dr

(R2 + r2 ) 2

ẑ

Usando el cambio de variables ρ = R2 + r2 =⇒ dρ = 2rdr, por lo tanto
~ = µ0 σω
B

ˆ2R2

(ρ − R2 )dρ

R2

ρ2



µ0 σω 
ẑ =
ẑ 

ˆ2R2





(ρ − R2 )dρ 

R2

ρ2

µ0 σω 
ẑ 
=

ˆ2R2
ˆ2R2

ρ− 2 dρ − R2
ρ− 2 dρ


R2

R2

Resolviendo las dos integrales anteriores, resulta que
√
~ = µ0 σω (3 2 − 4)Rẑ
B

Solución 10.9

P X

~
~ = µ0 I
~ = µ0 I dl × (~r − ~r ) =⇒ B
dB
4π |~r − ~r |
4π

−rˆ
tan αA

dxx̂ × (rŷ − x x̂)

r tan αC

(r2 + x2 ) 2

µ0 Irẑ
=
4π

−rˆ
tan αA

dx

r tan αC

(r2 + x2 ) 2

De este modo, usando el cambio de variables x = r tan θ =⇒ dx = r sec2 θdθ
~ = µ0 I ẑ
B
4πr

−α
ˆ A

cos θdθ =

µ0 I
µ0 I
(sin (−αA ) − sin αC )ẑ = −
(sin αA + sin αC )ẑ
4πr
4πr

αC

b) En el caso del polígono regular se pueden formar n triángulos isósceles, de forma que
a
αA = αC = πn y además r = 2 tan
π . El aporte de campo magnético en el centro del
n
polígono es realizado por n segmentos como el calculado en la parte a), por lo que el
resultado final es
 
 
µ0 nI
π
π
~
B=−
tan
sin
ẑ
πa
n
n

Problemas Propuestos y Resueltos de Electromagnetismo

a) Se fija un sistema de referencia de centro P para luego usar la definición de campo magnético.

---

### Página 226

CAPÍTULO 10. LEY DE BIOT-SAVART
c) Primero, dado que se necesita parametrizar una espira de radio r para conocer su campo
~ = rdθθ̂. Por lo tanto
en el centro, se tiene que ~r = 0, ~r 0 = rr̂ y dl
~ espira (0) = µ0
B
4π

ˆ2π

Irdθθ̂ × −rr̂
µ0 I
ẑ
=
| − rr̂|
2r

En función del radio r el campo magnético en el centro del polígono vale
π
~ = − µ0 I n sin π ẑ = − µ0 I sin n ẑ
B
2πr
n
2r πn

Como πn −→ 0 cuando n −→ ∞ y aplicando límite conocido de lím sinx x = 1 se tiene que
x→0

~ = − µ0 I ẑ
B
2r

Rodrigo Chi - Marzo 2017

Finalmente se comprueba el hecho de que el campo magnético es el mismo.

---

### Página 227

CAPÍTULO 10. LEY DE BIOT-SAVART

IV.

Indicaciones Problemas Sin Solución

Indicación 10.1

P X

Divida el alambre en cuatro caminos distintos e use Biot-Savart para calcular el campo
magnético que aporta cada uno de los caminos.
Note que hay dos caminos que tienen un aporte nulo de campo magnético en el punto O.

Indicación 10.2

P X

Identifique la parametrización del alambre infinito que va desde x = a hasta el infinito.

Indicación 10.3

P X

En ese problema puede separar el camino en 4 y determinar el campo que genera cada lado
del cuadrado.

Indicación 10.7

P X

Este problema puede algo complicado plateando las integrales de Biot-Savart. En caso que
intente por este método, es útil recordar que para el alambre del primer cuadrante se cumple
~ = dxx̂ + dy ŷ donde dy = tan α.
que dl
dx
Otro método más simple e ingenioso, es usar el resultado obtenido del Problema 10.9 de
forma conveniente.

Indicación 10.10

P X

Determine el campo magnético que genera una sola espira a distancia z del punto P .

Problemas Propuestos y Resueltos de Electromagnetismo

Una solución más rápida es aprovechar la geometría del problema, ya que el resultado final
debe quedar en la dirección de ẑ por simetría. Luego, si se determina el campo magnético
de un solo lado se puede afirmar que el resultado final es cuatro veces la componente en ẑ
de ese resultado.

---

### Página 228

CAPÍTULO 10. LEY DE BIOT-SAVART

Rodrigo Chi - Marzo 2017

~ por
Usando el resultado anterior, integre el campo encontrado en la parte anterior (dB)
cada espira que tiene la bobina cilíndrica (cada espira tiene corriente dI) para encontrar
~ Es sumamente útil notar que dI = nIdz.
finalmente el campo magnético total B.

---

### Página 229

CAPÍTULO 10. LEY DE BIOT-SAVART

V.

Resultados
Problema

Respuestas

P

10.1

~ = − µ0 Iα k̂ donde k̂ está saliendo de la hoja de papel.
B
8πR

P

10.2

h
i
~ = µ0 I 1 − √ a
B
ẑ
4πb
a2 +b2

P

10.3

~ =
B

P

10.4

~ = D) = − µ0 I (x̂ + ŷ)
B(z
4πD

P

10.5

Susana tiene la razón.

P

10.6

~ = µ0 I ẑ ln (n + 1)
B

P

10.7

~ = µI ẑ tan α , si x < 0 B
~ = µI ẑ cot α
Si x > 0: B
2πx
2πx

P

10.8

i
h 2 2
√
2z +R
~ = µ0 σω (3 2 − 4)Rẑ Propuesto: B(z)
~
B
= µ02σω √
−
2|z|
ẑ
R +z

10.9

P

10.10



a2
2 +z

ẑ

~ = − µ0 I (sin αA + sin αC )ẑ (ẑ entrando a la hoja de papel).
a) B
4πr


0 nI
~
tan nπ sin nπ ẑ
b) B = − µπa
~ ) = nI ẑ (cos θ2 − cos θ1 )
B(P

Problemas Propuestos y Resueltos de Electromagnetismo

P

2π

µ0 Iap

a2
4 +z

---

### Página 230

Rodrigo Chi - Marzo 2017

CAPÍTULO 10. LEY DE BIOT-SAVART

---

### Página 231

Fuerza de Lorentz

I.

Resumen Teórico

Fuerza de Lorentz
La fuerza de Lorentz indica que una carga q con una velocidad ~v bajo la influencia de un campo
~ siente una fuerza dada por
magnético B
~
F~ = q~v × B

(11.1)

~ la fuerza cambia a
Adicionalmente, en presencia de un campo eléctrico E
~ + ~v × B)
~
F~ = q(E

(11.2)

~
dF~ = dq~v × B

(11.3)

En el caso particular de un circuito eléctrico con corriente I, el diferencial de fuerza que siente el
circuito es
~ ×B
~
dF~ = I dl
(11.4)
~ es la dirección que sigue la corriente del circuito eléctrico. Recordar que B
~ es el campo
donde dl
externo que afecta al circuito.

Carga Puntual en Campo Magnético Constante
~ tiene
Una carga q de masa m y con una velocidad ~v perpendicular a un campo magnético B
una trayectoria circunferencial de radio
R=

m|~v |
~
q|B|

(11.5)

Problemas Propuestos y Resueltos de Electromagnetismo

Más general, un diferencial de carga dq siente una fuerza dF~ dado por

---

### Página 232

CAPÍTULO 11. FUERZA DE LORENTZ
~ la trayectoria es una espiral, de radio
En caso que de un campo ~v no perpendicular al campo B
mv⊥
~
q|B|

(11.6)

2πvk m
qB

(11.7)

R=
y paso
p=

Donde vk y v⊥ son los módulos de las componente paralela y perpendicular a la velocidad con
respecto al campo magnético, respectivamente.

Recomendaciones
~ son dos vectores que forman un plano. Perpendicular a éste, aparece la
Nótese que ~v y B
fuerza de Lorentz.
Debido a la naturaleza de la fuerza de Lorentz, la energía cinética de la carga es siempre
constante (ie. la fuerza de Lorentz no realiza trabajo sobre la carga). Debido a lo anterior,
el módulo de la velocidad es siempre constante.
Cuando se enfrente a problemas de carga puntales en zonas de campo magnético constante,
siempre tenga en cuenta que esta se moverá en una circunferencia o en una espiral.

Rodrigo Chi - Marzo 2017

En caso de problemas entre fuerza entre circuitos, tenga en cuenta que debe determinar
el campo magnético que provoca un circuito en específico y luego aplicar la Ecuación 11.4
sobre la corriente que circula en el otro circuito.

---

### Página 233

CAPÍTULO 11. FUERZA DE LORENTZ

II.

Problemas Propuestos

#### Problema 11.1

X S

~B

x

Un positrón de carga +e y masa m es disparado desde
el origen de un sistema de carga con un velocidad ~v0
formando un ángulo α entre la velocidad y el eje z.
Si el espacio existen un campo magnético constante
~ = B ẑ
B

~v0

a) La velocidad y la posición de la partícula en el
tiempo.

a

e

z

c) Demuestre que el positrón describe una trayectoria helicoidal. Encuentre su radio y su paso.

#### Problema 11.2

~B = B0 ẑ
-
-
-
-
-
-
-
-
-
-
-
-
-
-

X I

-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-

a

~v0

b

d

+e, m

~B

X I

Una partícula neutra se encuentra sometida a campo
magnético constante B = B0 ẑ. En t = 0 la partícula se rompe (“decae”) en dos cargas +q y −q con
igual masa m, las cuales salen disparadas con velocidades en direcciones contrarias. Determine el tiempo
en ambas partículas vuelven a chocar (exprese su resultado en función de q, m y B e ignore la interacción
coulombiana entre ellas).

⇥⇥⇥⇥⇥⇥⇥⇥
⇥⇥⇥⇥⇥⇥⇥⇥
⇥⇥⇥⇥⇥⇥⇥⇥
⇥⇥⇥⇥⇥⇥⇥⇥
⇥⇥⇥⇥⇥⇥⇥⇥
⇥⇥⇥⇥⇥⇥⇥⇥
⇥⇥⇥⇥⇥⇥⇥⇥
⇥⇥⇥⇥⇥⇥⇥⇥
+q

q

Problemas Propuestos y Resueltos de Electromagnetismo

#### Problema 11.3

-
-
-
-
-
-
-
-
-
-
-
-
-
-

Un protón se dispara a una zona de campo magnético constante tal como se muestra en la figura. Si el
protón de carga +e y masa m incide con un ángulo α
a la zona de campo, determine el valor de la distancia
d que recorre y el ángulo β con el cual sale de la zona
de campo (ver Figura).

---

### Página 234

CAPÍTULO 11. FUERZA DE LORENTZ
#### Problema 11.4

X I

z

Una partícula de masa m y carga q que está sometida
a la influencia simultánea de un campo eléctrico osci~ = E0 cos(Ωt)ẑ y un
latorio en la dirección vertical E
campo magnético constante en la dirección horizontal
~ = B0 x̂ como se ilustra en la figura. Sí la partícula
B
parte en el reposo,

~E

a) Encuentre las componentes x, y y z de la aceleración de la partícula.
b) Encuentre la velocidad en función del tiempo.
c) Encuentre la trayectoria y discuta que ocurre
cuando la frecuencia es Ω = qB
m
#### Problema 11.5

x

~B

X I

Una partícula de masa m, con carga q > 0, ingresa
horizontalmente a una región de ancho L, donde exis~ = B ẑ como se
te un campo magnético uniforme B
indica en la figura.

Zona de Campo

⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥

a) Calcule el valor crítico de la rapidez inicial ~v0 =
v0 x̂ de la partícula que le permite decidir si ella
atraviesa la región, o se devuelve.
b) Determine la trayectoria que realiza la partícu- ~v0
la para los casos en que la rapidez inicial sea
mayor o menor que el valor crítico encontrado m q
anteriormente.

Rodrigo Chi - Marzo 2017

y

q, m

L

c) Suponga ahora que ~v0 = v0 x̂ + vB ẑ, determine la altura con que sale la carga de la zona
de campo (considere distintos casos a partir del
valor encontrado en la parte anterior).
#### Problema 11.6

X I

z

Considere una cinta de ancho 2a por la cual circula
una corriente I homogéneamente distribuida. A una
distancia distancia a de ella, circula un cable con corriente I 0 (ver figura).
a) Encuentre el campo magnético en todo el plano
x > a.
b) Determine la fuerza por unidad de largo que
siente la cinta debido al cable.

I
y

2a
a

I0
x

---

### Página 235

CAPÍTULO 11. FUERZA DE LORENTZ
#### Problema 11.7

X S

Un electrón de carga −e y masa m se acelera a través
de una diferencia de potencial de ∆V = 104 [V] antes
de entrar a una región limitada por dos placas paralelas
que tienen una diferencia de potencial igual a V0 =
100 [V], separadas por una distancia d = 1 [mm] y de
largo L = 1 [m]. El electrón entra a esta región en un
plano equidistante de las placas. Ignorando efectos de
bordes:

d

V0

+

a) ¿Cuál es la velocidad del electrón al llegar a la
región limitada por las dos placas?

d

~ se debe aplicar en
b) ¿Qué campo magnético B
la región limitada por las dos placas para que
el electrón continúe con trayectoria rectilínea?
Indique la dirección de dicho campo en la figura.
c) Suponga que, una vez aplicado el campo calculado anteriormente, suponga que cuando el
electrón ha recorrido una distancia L/2 se quita la fuente de V0 = 100 [V]. ¿Alcanza a salir
el electrón de las placas paralelas?.

DV

q
#### Problema 11.8

X I

`

~v

q
#### Problema 11.9

X S

Suponga que el sistema que se ve en la figura se encuentra en un plano vertical, donde g es la aceleración
de gravedad. A través del alambre rectilíneo infinito
circula una corriente I1 en la dirección indicada. La
espira rectangular, de dimensiones a y b, está ubicada
paralela al alambre, a una distancia d de él y posee
una masa m. Encuentre la corriente I2 que debe circular por la espira (indique el sentido de ella), para
que permanezca en reposo en la posición señalada.

I1
d
g
a

b

Problemas Propuestos y Resueltos de Electromagnetismo

Una barra de largo ` tiene dos cargas puntuales +q
y −q sujetadas fuertemente en sus extremos. ¿Cuál
debe ser el valor de la velocidad ~v (perpendicular a la
barra) que debe avanzar la barra de modo que las dos
cargas no sientan fuerza entre ellas?.

---

### Página 236

CAPÍTULO 11. FUERZA DE LORENTZ
R

#### Problema 11.10

X S

R

~ =
En un espacio de campo magnético constante B
B0 ẑ, un fotón γ experimenta un decaimiento γ →
e− + e+ donde e− representa al electrón y e+ a un
positrón. La carga del electrón es −e < 0 y la del
positrón es +e; ambos tienen igual masa m. Como
resultado del decaimiento, ambas partículas adquieren
trayectorias espirales como se muestra en la figura. El
radio de los mantos cilíndricos por los cuales transita
cada partícula es R, y el paso axial en una vuelta es
s. Determine la rapidez con la que se mueve cada
partícula.

g

~B0

s

e
e+

#### Problema 11.11

X S

~B
~v
a

a) Encuentre el momentum angular del electrón en
función de carga e, el campo magnético B, y la
distancia al eje del cilindro interior r y momentum angular inicial L0 .
b) Asumiendo que los electrones salen con una velocidad inicial v0 ≈ 0, encuentre la velocidad
que tendrá en rmax , es decir en r = b.
c) Mediante conservación de energía, halle otra expresión para la velocidad recién calculada. A
partir de este encuentre el valor que debería
tener B, de modo que a los más el electrón
volviese en r = b.

b

V0

+

Rodrigo Chi - Marzo 2017

Considere dos cables coaxiales de radios a y b como
muestra la figura, cuyo espacio interior se encuentra
vacío. Los cables se encuentran separados a una diferencia de potencial V0 y entre ellos existe un campo
~ = B ẑ. Desde el cilindro inmagnético homogéneo B
terior se libera un electrón de carga −e y masa m.
El objetivo del problema es encontrar el valor máxi~ de modo que el electrón liberado no choque
mo de B
con el cilindro exterior (alcance a dar la vuelta perfectamente). Asuma que la velocidad del electrón tiene
solamente componentes en el plano de la figura.

---

### Página 237

CAPÍTULO 11. FUERZA DE LORENTZ

III.

Soluciones

Solución 11.1

P X

Lo primero que es necesario para abordar este problema es plantear la fuerza que sentirá la carga
por Lorentz
~
F~ = q~v × B
La velocidad inicial sólo tienen componentes en x y z, de hecho según la figura
v0x = v0 sin α

v0z = v0 cos α

Por otro lado, la fuerza inicialmente apunta en
~ = e(v0x x̂ + v0z ẑ) × B ẑ = −eBv0x ŷ
F~ (t = 0) = e~v (0) × B
Este calculo afirma que en t = 0 la carga siente una fuerza en la dirección y, luego esto implicará
que para t > 0 la velocidad tendrá tres componentes. Se plantea entonces las ecuaciones de
movimiento con
~ = e(vx x̂ + vy ŷ + vz ẑ) × B ẑ = eB(−vx ŷ + vy x̂)
F~ = e~v × B
Luego, aplicando Newton F~ = m~a = m~v˙ se obtiene que
m(v̇x x̂ + v̇y ŷ + v̇z ẑ) = eB(−vx ŷ + vy x̂)

v̇z = 0

v̇y = −

eB
vx
m

v̇x =

eB
vy
m

De la primera ecuación se deduce vz (t) = v0z (constante), por otro lado, derivando nuevamente
la segunda ecuación y reemplazando la tercera se puede llegar a una ecuación diferencial para vy
v̈y = −ω 2 vy =⇒ v̈y + ω 2 vy = 0
donde se ha definido ω = eB
. La ecuación anterior es un oscilador armónico, por lo que su solución
m
es de la forma
vy (t) = A1 cos ωt + A2 sin ωt
donde A1 y A2 son constantes por determinar. Aplicando condiciones iniciales
vy (0) = A1 = 0
por otro lado la constante A2 puede ser despejada de
v̇y (0) = −

eB
vx (0) = −ωv0x =⇒ v̇y (0) = A2 ω =⇒ A2 = −v0x
m

Problemas Propuestos y Resueltos de Electromagnetismo

analizando por componentes se tiene

---

### Página 238

CAPÍTULO 11. FUERZA DE LORENTZ
A partir de esto se tiene que las velocidades en el tiempo son
vy (t) = −v0 sin α sin ωt

vz (t) = v0 cos α

vx (t) = v0 sin α cos ωt

Integrando nuevamente para encontrar la posición en el tiempo, se obtiene que
y(t) = −

z(t) = v0 t cos α

v0
sin α(1 − cos ωt)
ω

x(t) =

v0
sin α sin ωt
ω

La ecuación anterior es la forma paramétrica de una trayectoria helicoidal. Manipulando algebraicamente el resultado anterior, se obtiene que
v0
v0
sin α =
sin α cos2 ωt
ω
ω





y+





v0
x =
sin α sin2 ωt
ω





Sumando las expresiones anteriores


x2 + y +

v0
v0
sin α =
sin α
ω
ω







α
El resultado obtenido es el de una helicoide de radio R = v0 sin
= v0 meBsin α (nótese el hecho que
ω
también coincide con el radio de una circunferencia, pero en este caso z aumenta linealmente
en el tiempo). Cabe destacar que la helicoide no está centrada, ésta se encuentra desplazada en
0m
y = − veB
.

Finalmente, para encontrar el paso de la hélice se tiene que
ω=

Rodrigo Chi - Marzo 2017

Solución 11.7

dθ dz
2π
eB
2πv0 cos αm
dθ
=
=
v0 cos α =
=⇒ p =
dt
dz dt
p
m
eB

P X

a) Para determina la velocidad es necesario hacer un balance energético de la siguiente forma
1 2
mvi − eVi = mvf2 − eVf
Dado que vi = 0 y que ∆V = Vf − Vi , se obtiene que
e∆V = mvf2 =⇒ vf =

s

2e∆V
m

b) Para que el electrón continúe una trayectoria rectilínea es necesario que la fuerza aplicada
sobre el electrón sea nula. Para ello, es necesario aplicar la fuerza de Lorentz
~ + ~v × B)
~
F~ = −e(E

---

### Página 239

CAPÍTULO 11. FUERZA DE LORENTZ
Como sistema de referencia se tomara x̂ apuntando de izquierda a derecha, ŷ de abajo hacia
arriba y ẑ saliendo de la hoja de papel. El campo eléctrico puede ser determinado fácilmente
debido a que dentro de un condensador
ˆd
V0 =

~ = V0 x̂
Edx =⇒ E
d

Luego
V0
V0
V0
F~ = −e
x̂ + vf ŷ × B ẑ = 0 =⇒ B = −
=−
d
vf d
d




r

m
2e∆V

Dado que B < 0 esto significa que apunta en el sentido inverso a ẑ, es decir, entra a la
hoja de papel.
c) Una vez apagada la fuente de voltaje, el electrón seguirá una circunferencia de radio
R=

eB
= 0,2m
mvf

dado que el radio es menor que la distancia que le queda por salir, el electrón chocará con
una de las paredes.

Solución 11.9

P X

Para que el sistema esté estático, se debe cumplir que
F~espira = 0

Se comenzará calculando la fuerza magnética que ejerce el hilo sobre la espira. Para ello se usa
la expresión
~ ×B
~
dF~ = I dl
Se asumirá conocido el campo eléctrico que provoca un cable infinito, el cual es
~ = µ0 I1 θ̂
B
2πr
Para usar la expresión anterior, se debe previamente asumir un sentido a la intensidad de corriente
en la espira (I2 ). Se hace el puesto que I2 tiene sentido horario, en el caso que no sea así el
resultado debería entregar un I2 negativo. Como sistema de referencia se tomará que la espira
~ apunta según ẑ (ver Figura 11.1). Considerando lo anterior
yace sobre el plano xy, en el cual B
y la ecuación
~ × µ0 I1 ẑ = µ0 I1 I2 (dl
~ × ~z)
dF~ = I2 dl
2πy
2πy
A continuación se hace el cálculo por segmento de la espira

Problemas Propuestos y Resueltos de Electromagnetismo

X

---

### Página 240

CAPÍTULO 11. FUERZA DE LORENTZ

I1
x

d

(a)

y

I2

(d)

(b)

a

(c)

b
Figura 11.1: Corrientes en la espira y en el cable.
~ = dxx̂
(a) y = d,dl
dF~a =

µ0 I1 I2
µ0 I1 I2
(dxx̂ × ẑ) = −
dxŷ
2πd
2πd

~ = dy ŷ
(b) y ∈ [d, d + a],dl
dF~b =

µ0 I1 I2
µ0 I1 I2
(dy ŷ × ẑ) =
dyx̂
2πy
2πy

~ = dxx̂
(c) y = d + a,dl
dF~c =

µ0 I1 I2
µ0 I1 I2
(dxx̂ × ẑ) = −
dxŷ
2π(d + a)
2π(d + a)

~ = dy ŷ
(d) y ∈ [d, d + a],dl

Rodrigo Chi - Marzo 2017

dF~d =

µ0 I1 I2
µ0 I1 I2
(−dy ŷ × ẑ) = −
dyx̂
2πy
2πy

A continuación cada uno de los valores para los diferenciales de F~ se integran de modo de conocer
la fuerza en cada región:
(a)
µ0 I1 I2
F~a = −
ŷ
2πd

ˆb
dx = −

µ0 I1 I2
bŷ
2πd

(b)
µ0 I1 I2
F~b =
x̂
2π

ˆd+a

dy
µ0 I1 I2
d+a
=
ln(
)x̂
y
2π
d

d

---

### Página 241

CAPÍTULO 11. FUERZA DE LORENTZ
(c)
µ0 I1 I2
F~c = −
ŷ
2π(d + a)

ˆ0
dx =

µ0 I1 I2
bŷ
2πd

b

(d)
µ0 I1 I2
x̂
F~b =
2π

ˆd

µ0 I1 I2
d+a
dy
=−
ln(
)x̂
y
2π
d

d+a

Con lo anterior se calcula la fuerza total
!

!

µ0 I1 I2
µ0 I1 I2
d+a
µ0 I1 I2
µ0 I1 I2
d+a
F~T = F~a +F~b +F~c +F~d = −
bŷ+
ln
x̂+
bŷ−
ln
x̂
2πd
2π
d
2π(d + a)
2π
d
µ0 I1 I2 b
µ0 I1 I2 ab
F~T =
− +
x̂ = −
x̂
2π
d d+a
2πd(a + d)




Dónde
F~b + F~d = 0
lo que anula todas las fuerzas en el eje x̂. Finalmente, además de la fuerza calculada la espira
esta sometida a su peso
X

µ0 I1 I2 ab
=0
F~espira = 0 ⇐⇒ M g −
2πd(a + d)

De dónde es posible despejar el valor de I2 como

Solución 11.10

2πM gd(a + d)
µ0 I1 ab

P X

Las cargas moviéndose dentro de campos magnéticos se mueven siguiendo una circunferencia
(velocidad dentro de un plano) o en una espiral (velocidad en tres dimensiones). Para hallar la
rapidez del electrón, primero se impone la velocidad en coordenadas cilíndricas
~v = ṙr̂ + rθ̇θ̂ + ż ẑ
debido a que r = R =⇒ ṙ = 0, Por otro lado, se tiene que
~
F~ = m~a = −e~v × B
entonces como B = B0 ẑ, se tiene que
m(−Rθ̇2 r̂ + Rθ̈θ̂ + z̈ ẑ) = −eB0 Rθ̇r̂

Problemas Propuestos y Resueltos de Electromagnetismo

I2 =

---

### Página 242

CAPÍTULO 11. FUERZA DE LORENTZ
de lo último se deduce que Rθ̈ = z̈ = 0 y además
θ̇ =

eB0
m

Para terminar el problema está faltando el valor de ż, que puede ser determinado mediante el
paso s que tiene la espiral (cada 2π radianes el electrón baja s metros) de la siguiente forma
ż =

dz dθ
s eB0
=
dθ dt
2π m

Finalmente la rapidez vale
|~v | =

q

s

s
eB0
(Rθ̇)2 + ż 2 =
R2 +
m
2π


2

El resultado es el mismo para el positrón, con la única diferencia que como su carga es +e el giro
será en el sentido inverso al del electrón.

P X

Solución 11.11

a) Previamente se debe notar que la fuerza que afecta al electrón en cualquier punto es F~ =
~ + E),
~ donde B
~ = B ẑ, E
~ = E(r)r̂ y ~v = ṙr̂ + rθ̇θ̂, luego F~ = −e(−ṙB θ̂ +
−e(~v × B
rθ̇Br̂ + E(r)r̂) Para encontrar el momentum angular, se usa el hecho que
~τ =

~
~
dL
dr
dL
= ~r × F~ =⇒
= rr̂ × (eṙB θ̂ − e(rθ̇B + E(r))r̂) = eBr ẑ
dt
dt
dt

Rodrigo Chi - Marzo 2017

Integrando a ambos con respecto al tiempo se obtiene que
L(r)
ˆ
ˆr
r 2 − a2
dL = eB rdr =⇒ L(r) = L0 + eB ·
L0

a

b) Por otro lado
~ = ~r × m~v =⇒ |L|
~ = mr|~v | =⇒ L(r) = mrv
L
sumando al hecho que v0 ≈ 0 =⇒ L0 ≈ 0 se deduce que
mrv = eB ·

r 2 − a2
(b2 − a2 )
=⇒ v(b) = eB
2mb

c) Por análisis energético
Ui + Ki = Uf + Kf =⇒ −eV (a) + mv02 = −eV (b) + mv 2 (b)

---

### Página 243

CAPÍTULO 11. FUERZA DE LORENTZ
Dado que V (b) − V (a) = V0 y v0 ≈ 0 se tiene
eV0 = mv 2 (b) =⇒ v(b) =

s

2eV0
m

Finalmente se deduce que el valor de campo magnético crítico es Bc
(b2 − a2 )
eBc
=
2mb

s

2eV0
2mb
=⇒ Bc =
m
e(b2 − a2 )

s

2eV0
m

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 244

CAPÍTULO 11. FUERZA DE LORENTZ

IV.

Indicaciones Problemas Sin Solución

Indicación 11.2

P X

Intente determinar la ecuación de la trayectoria que sigue la carga.
Recuerde que la trayectoria a la cual debería llegar es una circunferencia.

Indicación 11.3

P X

Suponiendo conocida la trayectoria circunferencial, es posible determinar la velocidad angular de ambas cargas.
Note que ambas cargas vuelven a juntarse cuando han recorrido π radianes.

Indicación 11.4

P X

~ + ~v × B)
~
Plantee la fuerza de Lorentz según F~ = m~a = q(E
Separe la ecuación anterior según cada coordenada y llegue a tres ecuaciones de movimiento
por cada eje. Luego integre cada ecuación para ir obteniendo desde la aceleración la velocidad
y la trayectoria.
Este problema puede ser algebraicamente trabajoso.

Rodrigo Chi - Marzo 2017

Indicación 11.5

P X

Recuerde la trayectoria que realizará la partícula al entrar a la zona de campo (circunferencia).
Relacione el radio R de la trayectoria con el ancho de la zona de campo.
Determinar el tiempo que se encuentra la partícula en la zona de campo puede ser muy útil
para determinar cuanto se eleva la carga.

Indicación 11.6

P X

Es necesario usar Biot-Savart para determinar el campo que genera la cinta y el cable.

---

### Página 245

CAPÍTULO 11. FUERZA DE LORENTZ
Dependiendo de como aborde el problema, puede ser útil el hecho que en la cinta se tiene
~ = I ŷ.
que el vector superficial de corriente es K
2a
~ ×B
~ donde I 0 es la corriente que pasa por el cable y B
~ el campo
Recuerde que dF~ = I 0 dl
que provoca la cinta sobre el alambre.

Indicación 11.8

P X

Tome una carga (positiva o negativa) y analice las fuerzas actuando sobre ellas.
Note que están actuando dos fuerzas sobre la carga: la electrostática y la magnética.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 246

CAPÍTULO 11. FUERZA DE LORENTZ

V.

Respuestas
Problema

Respuestas
a) vz (t) = v0 cos α

vy (t) = −v0 sin α sin ωt

z(t) = v0 t cos α

y(t) = − vω0 sin α(1 − cos ωt)

P

11.1

P

11.2

β = α, d = 2 mv
eB cos θ

P

11.3

t = πm
qB

vx (t) = v0 sin α cos ωt
x(t) = vω0 sin α sin ωt

m cos α
b) R = v0 meBsin α y p = 2πv0eB
.

a) ẍ(t) = 0,
ÿ(t) = qBm0 ż ,
q
z̈(t) = m
(E0 cos (Ωt) − B0 ẏ)

b) ẋ(t) = 0,

P

11.4

ẏ(t) =

q 2 B 0 E0
(cos (Ωt) − cos qB
qB
m t),
m2 ( m0 −Ω2 )

ż(t) =

qE0
( qB0 sin ( qB
qB
m t) − Ω sin(Ωt))
m( m0 −Ω2 ) m

c) x(t) = 0,
y(t) =

q 2 E0 B0
qB
m ( m0 −Ω2 )

z(t) =

q 2 E0
(cos (Ωt) − cos qB
qB
m t)
m( m0 −Ω2 )

m
( sin Ω(Ωt) − qB
sin qB
m t),

Si Ω = qB0 /m la partícula entra en resonancia y la amplitud de su movimiento se
vuelve infinita.

Rodrigo Chi - Marzo 2017

a) |vcritico | = qLB
m

P

11.5

b) Si la velocidad es mayor que ese vcritico , la carga escapa de la zona de campo, sino
la carga se devuelve siguiendo una trayectoria de semicircunferencia.

πm
v0 < vcritico

qB vB
c) h =
 m
qLB
v0 > vcritico
qB vB arcsin v0 m

---

### Página 247

CAPÍTULO 11. FUERZA DE LORENTZ
Problema

P

Respuestas
~ = − µ0 I ln
a) B
4πa

11.6
b)

~
µ0 II
dF
dy = 4πa



x+a
x−a



ẑ

ln(3)x̂

a) v = 6 · 107 [m/s].
[T]. El campo magnético debe apuntar hacia dentro de la hoja.
c) El electrón choca con una de las placas.

P

11.7

P

11.8

La velocidad debe ser igual a v = √ε10 µ0 = c (velocidad de la luz).

P

11.9

I2 = 2mgd(a+d)
µ0 I1 ab , la corriente I2 debe tener sentido horario.

P

11.10

|~v | = eB
m

b) |B| =

q
R2 +


s 2
2π

P

11.11

a) L(r) = L0 + eB · r −a
q
b) v(b) = 2eV
m
q
2eV0
c) Bc = e(b2mb
2 −a2 )
m

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 248

Rodrigo Chi - Marzo 2017

CAPÍTULO 11. FUERZA DE LORENTZ

---

### Página 249

Ley de Ampère

I.

Resumen Teórico

Ley de Ampère (Forma Integral)
La ley circuital de Ampère propone que para cualquier camino cerrado Γ se cumple que
˛
~ = µ0 Ienlazada
~ · dl
B

(12.1)

Γ

Equivalentemente

˛

¨
~ = µ0
~ · dl
B

Γ

~
J~ · dS

(12.2)

Ω

Ley de Ampère (Forma Diferencial)
En su forma diferencial, la ley dice que
~ ×B
~ = µ0 J~
∇

(12.3)

Ley de Gauss Magnética
~ satisface que
El cualquier campo magnético B
~ ·B
~ =0
∇
Lo anterior implica que no existen los monopolos magnéticos.

(12.4)

Problemas Propuestos y Resueltos de Electromagnetismo

Donde Ω es la superficie definida por Γ.

---

### Página 250

CAPÍTULO 12. LEY DE AMPÈRE

Recomendaciones
La ley de Ampère es el análogo a la ley de Gauss en electrostática. La ley de Ampère es
sumamente poderosa, y una de sus aplicaciones (gracias a la simetría de algunos problemas)
es poder determinar campos magnéticos.
¿Cuándo usar Ley de Ampère para determinar campos magnéticos?, al igual que la ley de
Gauss los casos son limitados, no siempre puede usarse. Una lista de posibles casos es
- Cables infinitos con corriente I

- Cilindros macizos infinitos con una densidad de corriente axial constante o de la forma
J~ = J(r)ẑ.
- Cilindros macizos infinitos con una densidad de corriente azimutal constante o de la
forma J~ = J(r)θ̂.
- Superficies cilíndricas infinitas con una densidad superficial de corriente axial o azimutal
constante.
- Planos infinitos con densidad superficial constante.

- Bloque infinito (superposición de planos) con una densidad de corriente dependiente
de la altura del bloque.
- Bobinas/Solenoides infinitos.
- Toroides.

Rodrigo Chi - Marzo 2017

La forma diferencial de la Ley de Ampère suele utilizarse cuando la incógnita es la densidad
de corriente J~ que genera un campo magnético conocido.

---

### Página 251

CAPÍTULO 12. LEY DE AMPÈRE

II.

Problemas Propuestos

#### Problema 12.1

X S

Un cable coaxial muy largo consiste en un cilindro
sólido con un radio interior de radio a, rodeado por
un cascarón cilíndrico conductor concéntrico de radio
interno b y exterior c. El conductor interior tiene una
densidad de corriente no uniforme J~1 = αrẑ donde α
es una constante. El cilindro exterior tiene una densidad de corriente J~2 = −β ẑ donde β es una constante
positiva. Los conductores llevan una igual y opuesta
corriente de magnitud I0 . Entre ambos conductores
existe vacío.
a) Encuentre los valores α y β en términos de a, b, c
y I0

J~2

J~1

a

⇥

b
c

b) Determine el campo magnético en todo el espacio. Exprese sus resultados en términos de a, b, c
~ con respecto a la
y I0 . Realice un gráfico |B|
distancia desde el eje de simetría r.
#### Problema 12.2

X I

a

!

~ = µ0 J0 r 1 − r
B
θ̂
2a2
donde J0 es una constante y r es la distancia del eje
del cilindro. Determine
a) El vector densidad de corriente y la intensidad
de corriente eléctrica dentro de la tubería.
b) El campo magnético fuera de la tubería.
~
c) El valor de la densidad superficial de corriente K
que debe circular por el borde de la tubería para
que el campo magnético en el exterior sea nulo
~ se distribuye uniformemente
(suponga que K
por la superficie).

J~

Problemas Propuestos y Resueltos de Electromagnetismo

Dentro de una tubería metálica cilíndrica de radio a
circula un fluido viscoso con una cierta densidad de
carga. En los puntos al interior de la tubería se ha
determinado que el campo magnético vale

---

### Página 252

CAPÍTULO 12. LEY DE AMPÈRE
#### Problema 12.3

X S

Considere 3 alambres rectos de sección transversal
despreciable, infinitamente largos y separados entre
sí una distancia d. Cada alambre lleva una corriente
I, en la misma dirección (perpendicular al plano de la
hoja y hacia adentro).

⇥

d

a) Encuentre la ubicación de los dos puntos donde
el campo magnético total se anula.

⇥

b) Suponga que el alambre central se desplaza rígidamente una pequeña distancia y (y
d)
en dirección perpendicular a la línea sobre la
que están dispuestos inicialmente los alambres,
mientras los otros dos alambres permanecen fijos. Calcule aproximadamente la fuerza neta por
unidad de largo que actúa sobre el alambre desplazado, al primer orden de y

⇥

2I ⇥

X S

Tres alambres infinitos están ubicados mutuamente
paralelos orientados perpendicularmente al plano de
la hoja y ubicados en los vértices de un cuadrado de
lado d. Uno de ellos lleva corriente 2I que entra al
plano, mientras que los otros llevan corriente I que
emerge del plano de la hoja. Calcule el vector campo
magnético en los puntos P1 y P2 .

x

d

(entra)

#### Problema 12.4

y

d

I

·

d

(sale)

·

P1

·

·

P2

Rodrigo Chi - Marzo 2017

(sale)

#### Problema 12.5

X S

Se tiene un conductor en la forma de una capa cilíndrica recta, infinita, de radio interior a y radio exterior b.
Este conductor tiene una densidad de corriente que,
expresada en coordenadas cilíndricas, es:
~ ≤ r ≤ b) = α θ̂ + β ẑ
J(a
r
Con α y β constantes conocidas. Obtenga el campo
magnético en todas partes.

a
b

I

---

### Página 253

CAPÍTULO 12. LEY DE AMPÈRE
#### Problema 12.6

X S

z

Sobre el plano xy se encuentra una moneda magnetizada muy pequeña de radio R y espesor d. Experimentalmente sólo se conoce la componente axial del
campo magnético dentro de la moneda, dado por

R
d

Bz = B0 (1 + κz 2 )

y

donde κ es una constante. Suponiendo que el campo
magnético posee simetría axial y no posee componente en θ̂, determine la intensidad corriente que circula
dentro de la moneda.
#### Problema 12.7

P1

X S

Considere dos planas metálicas infinitas paralelas Π1
y Π2 , separadas una distancia d. En sus respectivas
placas fluyen corrientes en direcciones arbitrarias, las
cuales tienen una ángulo β entre ellas como se ilustra en la Figura. Encuentre la densidad de fuerza por
unidad de área e indique si la fuerza es repulsiva o
atractiva a partir de los distintos valores de β.
#### Problema 12.8

x

P2

~1
K

~2
K
b

d
z

X I

J~ = J(r)x̂
R
R

P

~ = K x̂
K

J~ = J0 k̂

#### Problema 12.9

X I

Un cable de cilíndrico de radio R lleva una densidad
de corriente J~ = J0 k̂. El cable tiene un hoyo cilíndrico
de radio a paralelo al eje del cilindro a una distancia b
de él. Muestre que el campo magnético dentro de la
cavidad es uniforme, y encuentre su valor.

R
b

a

Problemas Propuestos y Resueltos de Electromagnetismo

Se tiene dos corrientes, ambas con igual sentido. Una
de ellas es una corriente plana e infinita de densidad
lineal K y otra es una corriente cilíndrica
infinitamente


r
larga cuya densidad es J(r) = J0 1 − R . Encuentre
el valor de J0 en función de K que hace que el campo
magnético resultante en el punto P ubicado a una
distancia R2 del centro del cilindro sea nulo.

---

### Página 254

CAPÍTULO 12. LEY DE AMPÈRE
#### Problema 12.10

X I

Considere 3 distribuciones como se muestran en la
figura. Un bloque de ancho w lleva un densidad volumétrica uniforme de corriente J~1 = J1 ẑ. Un cable
infinito de radio R lleva una densidad de corriente no
uniforme J~2 = −αrẑ, donde r es la distancia desde
el eje del cilindro y α una constante. El bloque se encuentra a una distancia d del cilindro. Si se coloca un
alambre con corriente I a una distancia s del centro
del cable (s < d), determine la fuerza por unidad de
largo que siente el cable con corriente I.

Rodrigo Chi - Marzo 2017

#### Problema 12.11

J~1 = J1 ẑ

w
I
d

ŷ

s
x̂
ẑ

R
J~2 =

↵rẑ

X I

Considere dos bobinas muy largas de radios R1 y R2 ,
con N1 y N2 vueltas por unidad de largo, respectivamente. La bobina de radio R2 se encuentra inserta
dentro de la bobina de radio R1 compartiendo su mismo eje. Si por la bobina exterior circula una corriente
I1 , determine:
a) La corriente I2 que circula por la bobina interior,
sabiendo que el campo magnético para r < R2
es nulo.
b) Para la corriente encontrada en la parte anterior, encuentre la fuerza por unidad de área que
siente la bobina interior.

R1
R2

I1 , N1

---

### Página 255

CAPÍTULO 12. LEY DE AMPÈRE

III.

Soluciones

Solución 12.1

P X

a) Usando la definición de corriente eléctrica a partir de la densidad de corriente, se obtiene
que
¨
ˆ2π ˆa
3I0
2παa3
~ =
=⇒ α =
I0 =
J~1 · dS
αrẑ · rdrdθẑ =
2πa3

¨
−I0 =

ˆ2π ˆc
~ =
J~2 · dS

−β ẑ · rdrdθẑ = −βπ(c2 − b2 ) =⇒ β =

I0
π(c − b2 )

b

b) Por otro lado, el campo magnético es por ley de Ampere
- r < a:
˛
ˆ2π ˆr
2π
~ = µ0 Ienl =⇒ B(r)·2πr = µ0
~ dl
~ = µ0 I0 r θ̂
B·
αrẑ·rdrdθẑ = µ0 αr3 =⇒ B
2πa3

- a < r < b:
˛
ˆ2π ˆa
~ = µ0 Ienl =⇒ B(r) · 2πr = µ0
~ · dl
~ = µ0 I0 θ̂
B
αrẑ · rdrdθẑ = I0 =⇒ B
2πr

- r > c:

b

˛
~ = µ0 Ienl =⇒ B(r) · 2πr = I0 − I0 = 0 =⇒ B
~ · dl
~ =0
B

c) Un gráfico aproximado es el que se muestra en la Figura 12.1

Solución 12.3

P X

a) Para iniciar el problema se debe calcular el campo magnético que produce un cable que lleva
corriente. Usando Ley de Ampère sobre un camino Γ (circunferencia de radio r recorrida en
sentido anti-horario).
˛
~ = µ0 I =⇒ −B(r) · 2πr = µo I =⇒ B
~ · dl
~ = µ0 I (−θ̂)
B
2πr
Γ

Problemas Propuestos y Resueltos de Electromagnetismo

- b < r < c:
˛
ˆ2π ˆr
~
~
~ = µ0 I0 c − r θ̂
B · dl = µ0 Ienl =⇒ B(r) · 2πr = I0 −
β ẑ · rdrdθẑ =⇒ B
2πr c2 − b2

---

### Página 256

CAPÍTULO 12. LEY DE AMPÈRE
|B(r)|
µ0 I0
2pa
µ0 I0
2pb
a

c

b

r

Figura 12.1: Gráfico
Se supondrá que el punto donde el campo magnético se anula es sobre el eje X . Sea = x”
el valor medido desde el centro del sistema de referencia. Debido a la superposición de los
campos magnéticos, el campo en ese punto vale:
~
B(x,
0) = B~1 + B~2 + B~3 =

µ0 I
µ0 I
µ0 I
(−ẑ) +
(−ẑ) +
ẑ
2π(x + d)
2πx
2π(d − x)

Es posible verificar que el valor del campo magnético sobre el eje x siempre va en el sentido
ẑ (o −ẑ) y depende sólo de la distancia que separa el cable al punto donde se calcula el
~
campo. Dado que se busca B(x,
0) = 0, se obtiene que
+ −
=0
x+d x d−x
d
donde resultan dos puntos simétricos ubicados en x = ± √
b) Primero se calcula el campo magnético que genera el cable de la izquierda sobre el punto
~ = µ0 I (−θ̂) (precaución: la fórmula anterior está con respecto
(0, y). Recordando que es B
2πr
al origen, aquí la usaremos centrada en el punto (−d, 0)) se obtiene que:

Rodrigo Chi - Marzo 2017

B~1 =

µI
√ 02
(−(− sin αx̂ + cos αŷ))
2π y + d2

De igual forma, para el cable de la derecha se tiene que:
B~2 =

µI
µ0 I
√ 02
(−(− sin (π − α)x̂+cos (π − α)ŷ)) = √ 2
(−(− sin αx̂−cos αŷ))
2π y + d
2π y + d2

y
Sumando las expresiones anteriores, y notando que sin α = √ 2
y + d2
µ0 Iy
~ y) = B~1 + B~2 = µ√0 I sin α x̂ =
B(0,
x̂
π(y 2 + d2 )
π y +d
Por lo que la fuerza estará dada por:
~ × B(0,
~ y) = −Idz ẑ ×
dF~ = I dl

µ0 Iy
µ0 I 2 dz y
x̂
=
−
ŷ
π(y 2 + d2 )
π y 2 + d2

---

### Página 257

CAPÍTULO 12. LEY DE AMPÈRE

⇥

a

d
y
~B1

~B

d

~B2

ŷ

a
x̂

⇥

Figura 12.2: Campos Magnéticos aplicados al cable.

f (λ) =

λ
λ2 + 1

en un punto cercano a λ = 0, por lo tanto
f (λ) ≈ f (0) +

df (λ)
(λ − 0) = λ
dλ λ=0

Finalmente la aproximación es
dF~ = −

Solución 12.4

y
µ0 I 2 dz 1
µ0 I 2 dz y
d
ŷ
≈
−
ŷ
π d ( yd )2 + 1
π d2

P X

Para calcular el campo en los lugares pedidos, primero se debe conocer el resultado genérico para
el campo magnético producido por un alambre infinito con corriente I circulando en el sentido

Problemas Propuestos y Resueltos de Electromagnetismo

Se pide la fuerza anterior linealizada (primer orden), por lo tanto reescribiendo la expresión
como
y
µ0 I 2 dz 1
d
dF~ = −
ŷ
π d ( yd )2 + 1
Como sabemos que y
d tenemos que hacer una aproximación según Taylor de la función

---

### Página 258

CAPÍTULO 12. LEY DE AMPÈRE
positivo de ẑ. Usando la Ley de Ampére en una superficie circular de radio r en el plano xy, y
~ = B(r)θ̂, entonces:
asumiendo por simetría B
˛
~ · d~r = µ0 I = 2πrB =⇒ B
~ = µ0 I θ̂
B
2πr
Ahora volviendo al problema original, primero se calcula el campo en el punto P1 , colocando al
origen de los ejes cartesianos sobre P1 , con x̂ horizontal hacia la derecha, e ŷ vertical hacia arriba:
~ = µ0 I
B
2π √d2

−x̂ + ŷ
√

!

µ0 I
+
2π √d2

x̂ − ŷ
√

!

µ0 I
+ d
π √2

−x̂ − ŷ
√

!

Por lo tanto:

~ 1 ) = − µ0 I (x̂ + ŷ)
B(P
πd
Para el cálculo en el punto P2 , se reubica el origen de los ejes en él, nuevamente con x̂ horizontal
hacia la derecha, e ŷ vertical hacia arriba:
~ = µ0 I x̂ + µ0 I ŷ + µ0√I
B
2πd
2πd
πd 2

Solución 12.5

−x̂ − ŷ
√

!

~ 2) = 0
= 0 =⇒ B(P

P X

En este caso se está en presencia de una superposición de corrientes, una la dirección de θ̂ y otra
en ẑ. Para enfrentar este problema es necesario determinar el campo magnético que genera cada
una de las densidades de corrientes, para luego sumarlos y obtener el campo total por intervalo.
Se define entonces
α
Jz (r) = β
Jθ (r) =
r

Rodrigo Chi - Marzo 2017

Jq (r)q̂
b

Jq (r)q̂

a

b

G1

Jq (r)q̂

a

L

a

G3
L

L

r

r

a<r<b

r<a

r

r>b

b

G2

Figura 12.3: Los caminos Γ1 , Γ2 y Γ3 son los que se usan para determinar el campo magnético
para la densidad de corriente en θ (en naranjo la corriente enlazada por los caminos).
Para la primera corriente Jθ es necesario hacer el supuesto que el campo magnético es de la forma
~ 1 = B1 (r)ẑ debido a la regla de la mano derecha. Para enfrentar es tipo de dirección de corriente
B

---

### Página 259

CAPÍTULO 12. LEY DE AMPÈRE
mediante Ampère es necesario usar un camino rectangular de la forma en que se muestra en la
Figura 12.3. Luego, para r > b se tiene por Ampère
!
¨
˛
b
~ = µ0
~ 1 · dl
B
Jθ θ̂ · drdz θ̂ =⇒ (B1 (0) − B1 (r))L = µ0 Lα ln
a
Γ1

Nótese que dos lados de Γ1 tienen aporte nulo a la integral de linea. Por otro lado, es algo errado
considerar B1 (0) es nulo, de hecho lo correcto es determinar ese valor mediante Biot-Savart
~ 1 (0) = µ0
B
4π

ˆ∞ ˆ2π ˆb α

θ̂rdrdθdz × −(rr̂ + z ẑ)
r

−∞ 0

a

(r2 + z 2 ) 2

!

b
= µ0 α ln
ẑ
a

Lo anterior implica que
~ 1 (r > b) = 0
B
Luego para a < r < b se tiene que
˛
¨
 
r
~
~
B1 · dl = µ0
Jθ θ̂ · drdz θ̂ =⇒ (B1 (0) − B1 (r))L = µ0 Lα ln
a
Γ2

Dado que el valor de B1 (0) ya es conocido, se obtiene que
!

~ 1 (a < r < b) = µ0 α ln b ẑ
B
r

Jz ẑ

Jz ẑ
a

a

r
b

Jz ẑ

b

C2

a

r

C3

r

b

C1
Figura 12.4: Los caminos C1 , C2 y C3 son los que se usan para determinar el campo magnético
para la densidad de corriente en z (en naranjo la corriente enlazada por los caminos).
En el caso de la corriente en z, es necesario tomar caminos circulares como se muestra en la
Figura 12.4. Para el primer caso r > b se tiene que
˛
¨
~ = µ0
~ 2 · dl
~ 2 = µ0 βπ(b − a )
B
Jz ẑ · rdrdθẑ =⇒ B2 (r) · 2πr = µ0 βπ · (b2 − a2 ) =⇒ B
2r
C1

Problemas Propuestos y Resueltos de Electromagnetismo

Finalmente para r < a se tiene que no hay corriente enlazada por lo cual el campo magnético
vale
!
b
~
ẑ
B1 (r < a) = µ0 α ln
a

---

### Página 260

CAPÍTULO 12. LEY DE AMPÈRE
Análogamente para el caso a < r < b se tiene
˛
¨
~
~
~ 2 = µ0 βπ(r − a )
B2 · dl = µ0
Jz ẑ · rdrdθẑ =⇒ B2 (r) · 2πr = µ0 βπ · (r2 − a2 ) =⇒ B
2r
C2

En el último caso r < a no existe corriente en enlazada, por lo cual
˛
¨
~
~
~ 2 (r < a) = 0
B2 · dl = µ0
Jz ẑ · rdrdθẑ = 0 =⇒ B
C3

~ =B
~1 + B
~ 2 es
Finalmente el campo total B
µ0 α ln( ab )ẑ










r<a

µ0 β(r2 −a2 )
~ =
θ̂ + µ0 α ln( rb )ẑ a < r < b
B
2r









µ0 β(b2 −a2 )
θ̂
2r

r>b

P X

Solución 12.6

Como el problema no depende de la componente según θ̂, se puede deducir que el campo magnético
es de la forma
~ z) = Br (r, z)r̂ + Bz (r, z)ẑ
B(r,

Rodrigo Chi - Marzo 2017

~ ·B
~ = 0, esto implica que el
Esto es básicamente debido adicionalmente debe cumplirse que ∇
flujo en cualquier superficie cerrada siempre es nulo. Usando lo anterior, por en enunciado se sabe
que Bz (r, z) = B0 (1 + κz 2 ), por lo que tomando un cilindro pequeño de radio r y altura z dentro
de la moneda se tiene que
ΦCilindro = Φ1 + Φ2 + Φ3
Donde Φ1 y Φ2 son los flujos sobre las tapas superior e inferior respectivamente, y Φ3 el flujo
sobre el manto. Ahora de acuerdo a la Ley de Gauss magnética se debe tener que
¨
~ =0
~
~
~ · dS
∇ · B = 0 =⇒ ΦCilindro =
B
Cilindro

Determinando los flujos por separado se tiene
ˆ2π ˆr

ˆ2π ˆr
~ =
~ 0) · dS
B(r,

Φ1 =

ˆ2π ˆr

ˆ2π ˆr
~ =
~ z) · dS
B(r,

Φ2 =

B0 ẑ · drdθ(−ẑ) = −B0 πr2

B0 (1 + κz 2 )ẑ · drdθẑ = B0 (1 + κz 2 )πr2

---

### Página 261

CAPÍTULO 12. LEY DE AMPÈRE

R

z=d

r
z
z=0
Figura 12.5: Moneda sobre el plano xy
Por lo que Φ1 + Φ2 + Φ3 = 0 =⇒ Φ3 = −(Φ1 + Φ2 ) = −B0 πr2 κz 2 , pero por otro lado
ˆz ˆ2π

ˆz
~ z) · rdθdzr̂ = 2πr
B(r,

Φ3 =

Br (r, z)dz = −B0 πr2 κz 2 =⇒ Br (r, z) = −B0 rκz

entonces el campo magnético vale
~ = −B0 rκzr̂ + B0 (1 + κz 2 )ẑ
B
Finalmente para determinar la corriente
~ ×B
~ = − B0 κr θ̂ =⇒ I =
~ ×B
~ = µ0 J~ =⇒ J~ = 1 ∇
∇
µ0
µ0

ˆd ˆR
−

P X

Se nos pide determinar la fuerza entre las placas que puede ser algo complejo de ver a primera
vista. ¿Por qué siente fuerza una placa?, a priori se podría suponer que la fuerza que siente cada
placa es la misma módulo, ya que es un par acción - reacción. Ahora, si se toma como referencia
~1
la placa Π1 , la placa Π2 sentirá una fuerza por dos motivos: la corriente que circula por K
provoca un campo magnético en todo el espacio y en Π2 existe una corriente circulando. Estos
dos elementos, = campos magnéticos” (por lo general externos) y = corrientes” (o cargas
en movimiento) siempre provocan fuerza sobre las cargas. Ahora para determinar la fuerza
se debe usar la forma diferencial de la fuerza de Lorentz:
~1
dF~2 = dq~v2 × B
Donde F~2 es la fuerza que siente la placa Π2 . En este caso el diferencial de carga dq = σ2 dS,
~ 2 = σ2~v2 . Juntando las igualdades anteriores se puede reescribir la fuerza
pero por otro lado K
como
~
~ 2 dS × B
~ 1 =⇒ dF2 = K
~2 × B
~1
dF~2 = K
dS

Problemas Propuestos y Resueltos de Electromagnetismo

Solución 12.7

B0 κr
B0 κdR2
θ̂ · drdz θ̂ = −
µ0
2µ0

---

### Página 262

CAPÍTULO 12. LEY DE AMPÈRE
~ 1 de una placa puede ser determinado por Ley de Ampère (Figura 12.6).
El campo magnético B

~B1
z
x

z

~1
K

y

z

G
L

Figura 12.6: Corriente en el plano Π1 y camino de Ampère.
La curva Γ es un rectángulo de ancho L y alto 2z como puede verse en la Figura 12.6. Además
~ 1 (z)| = |B
~ 1 (−z)|
debe notarse que por simetría del problema necesariamente se tiene que |B
. Dado que el plano que lleva corriente es infinito, el campo magnético siempre apunta en la
dirección x̂ (esto es debido a que las componentes verticales son siempre anuladas consecuencia
de la simetría del plano). Usando la Ley de Ampère se obtiene que
˛
~ = µ0 I
~ · dl
B
Γ

Por otro lado la integral de camino se puede descomponer de la siguiente forma
˛

ˆL
~ =
~ · dl
B

Rodrigo Chi - Marzo 2017

Γ

ˆz
B1 (z)x̂ · dxx̂ +

ˆ0
B1 (z)x̂ · dz ẑ +

−z

ˆ−z
−B1 (z)x̂ · dxx̂ +

L

B1 (z)x̂ · dz ẑ
z

De la expresión anterior se anulan las dos integrales verticales (el campo es ortogonal al camino).
Por lo tanto
˛
~ = B1 (z) · 2L
~ · dl
B
Γ

Por otra parte, si se tienen densidades de corriente superficiales, la corriente enlazada se puede
determinar como (n̂ normal de la superficie donde fluye corriente)
ˆ
I=

ˆL
~ =
~ 1 × n̂) · dl
(K

(K1 ŷ × ẑ) · dx x̂ = K1 L

Luego la ley de Ampere se transforma en
˛
~ = µ0 I =⇒ B1 (z) · 2L = µ0 K1 L =⇒ B1 (z) = µ0 K1
~ · dl
B
Γ

---

### Página 263

CAPÍTULO 12. LEY DE AMPÈRE
Notar el hecho que el plano Π2 está ubicado en z = d, por lo que el campo magnético que afecta
al plano es
~ 1 (z) = µ0 K1 x̂
B
~ 2 = K2 cos β x̂ + K2 sin β ŷ, se procede a calcular la fuerza por unidad
Ahora, descomponiendo K
de área que siente el plano Π2 como
dF~2
µ0 K 1
µ0 K1 K2 sin β
= K2 (cos β x̂ + sin β ŷ) ×
x̂ = −
ẑ
dS
Finalmente, si β ∈ (0, π), la fuerza es atractiva (corrientes paralelas), si β ∈ (π, 2π) la fuerza es
repulsiva (corrientes antiparalelas), y para los ángulos β = 0, π no existe fuerza al ser las corrientes
ortogonales.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 264

CAPÍTULO 12. LEY DE AMPÈRE

IV.

Indicaciones Problemas Sin Solución

Indicación 12.2

P X

~ para r < a es dato, use la ley de Ampère en su forma diferencial para encontrar
Como B
la densidad de corriente e integre en la sección transversal de la tubería para encontrar la
intensidad de corriente.
Conocida la intensidad de corriente, es posible determinar el campo magnético fuera de la
tubería usando la ley de Ampère en su forma integral.
Usado la ley Ampère en su forma integral, determine cuál debe ser el valor de la intensidad
de corriente (y que sentido debe tener) sobre la superficie de la tubería para que el campo
sea nulo en puntos r > a. Conocida la corriente divídala por el perímetro de la tubería para
~
encontrar la densidad superficial K.

Indicación 12.8

P X

Usando ley de Ampère, determine el campo magnético que provoca J~ dentro del cilindro
(camino circular), en particular determine cuanto vale en P .
Nuevamente por Ampère, determine el campo magnético que general la densidad superficial de corriente para puntos sobre ella (camino rectangular). Recuerde que este valor es
constante.

Rodrigo Chi - Marzo 2017

Use el principio de superposición para concluir este problema y encontrar la relación entre
J0 y K cuando el campo magnético es nulo en P .

Indicación 12.9

P X

Utilice dos sistemas de referencias en coordenadas cilíndricas ~r1 = r1 r̂1 y θ̂1 para el cilindro
de radio R y ~r2 = r2 r̂2 y θ̂2 para el hueco cilíndrico de radio a.
Use el principio de superposición para determinar el campo magnético en un punto dentro
de la cavidad, exprese ese resultado en función de r1 , r2 , θ̂1 , θ̂2 y constantes.
Note que ẑ es el mismo vector unitario para ambos sistemas de referencias, luego ẑ =
r̂1 × θ~1 = r̂2 × θ~2 use esta relación en forma conveniente para dejar el valor del campo
magnético en función de ~r1 , ~r2 , ẑ y constantes.
Concluya el problema utilizando la relación vectorial entre ~r1 y ~r2 .

---

### Página 265

CAPÍTULO 12. LEY DE AMPÈRE
Indicación 12.10

P X

Determine los campos magnéticos que actúan sobre el cable, para ello use el principio de
superposición para el campo que genera en cilindro infinito (camino circular) y el bloque
infinito con corriente (camino rectangular).
~ ×B
~ para
Una vez determinado el campo que actúa sobre el cable, use la relación dF~ = I dl
concluir el problema.

Indicación 12.11

P X

Use la ley de Ampère para determinar el campo magnético que genera una sola bobina
(camino rectangular).
Utilizando el resultado anterior y el principio de superposición, determine el valor del campo
magnético que habría dentro de las dos bobinas. Encuentre el valor de I2 imponiendo que
el valor anterior es nulo.
F ~
~ Intente determinar el
Para encontrar la fuerza por unidad de área, recuerde que d =
K × B.
~ que circula por la bobina interior.
valor de K

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 266

CAPÍTULO 12. LEY DE AMPÈRE

V.

Resultados
Problema

P

12.1

Respuestas
3I0
I0
a) α = 2πa
3 , β = π(c2 −b2 )

µ0 I0 r 2

r<a

2πa3 θ̂


µ0 I0
θ̂
a<r<b
~ =
2πr
b) B
 µ0 I0 c2−r2 θ̂ b < r < c


 2πr c −b
r>c



a) J~ = J0 1 − ar 2 ẑ, I = J0 πa

P

12.2

~ = µ0 J0 a θ̂
b) B
4r

Rodrigo Chi - Marzo 2017

~ = − J0 a ẑ
c) K

P

12.3

P

12.4

a) x ± √d3
b)

~
µ0 I 2 y
dF
dz ≈ − π d2 ŷ

~ 1 ) = − µ0 I (x̂ + ŷ), B(P
~ 2 ) = 0. (x̂ creciendo hacia la derecha e ŷ hacia arriba)
B(P
πd




P

12.5

µ0 α ln( ab )ẑ
µ0 β(r −a2 )
~ =
B
θ̂ + µ0 α ln( rb )ẑ
2r


µ0 β(b2 −a2 )
θ̂
2r

P

12.6

κdR
I = − B02µ

P

12.7

P

12.8

~2
dF
dS

r<a
a<r<b
r>b

= µ0 K1 K2 2 sin β ẑ donde ẑ apunta desde plano Π1 al Π2 . Si β ∈ (0, π), la fuerza
es atractiva, si β ∈ (π, 2π) la fuerza es repulsiva, y para β = 0 o β = π no existe
fuerza.

J = 3K
R

---

### Página 267

CAPÍTULO 12. LEY DE AMPÈRE
Problema

Respuestas

P

12.9

~
B(z)
= µ02J0 k̂ × ~b, el vector ~b es que parte del centro del cilindro hasta el centro de
la circunferencia de radio a.

P

12.10

~
J1 w
dF
αR3
dl = µ0 I( 3s + 2 )ŷ

P

12.11

a) I2 = − N
N2 I1

b)

~
dF
dS = −µ0 (N1 I1 ) r̂

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 268

Rodrigo Chi - Marzo 2017

CAPÍTULO 12. LEY DE AMPÈRE

---

### Página 269

Potencial y Momento Magnético

I.

Resumen Teórico

Potencial Vectorial Magnético
~ existe un vector potencial magnético A
~ tal que
Para todo campo magnético B
~ =∇
~ ×A
~
B

(13.1)

~yB
~
Si se integra en volumen la Ecuación 13.1 se puede encontrar otra relación entre A
˛
¨
~
~
~
~ · dS
A · dl =
B
Γ

(13.5)

Ω

El vector potencial no es único, ya que cualquier solución de la forma
~1 = A
~ 2 + ∇f
A

(13.6)

es también solución de la Ecuación 13.1, ya que para cualquier función escalar f el rotor de su
~ ·A
~ = 0, entonces se cumple que
gradiente es nulo. Si se elige f de modo que ∇
~ = µ0 J~
∇2 A

(13.7)

Problemas Propuestos y Resueltos de Electromagnetismo

Consecuencia de lo anterior, el potencial magnético puede ser determinado por alguna de las
siguientes expresiones
ˆ
~
µ
I dl
~=
(13.2)
A
4π
|~r − ~r 0 |
¨ ~
µ0
KdS
~
A=
(13.3)
4π
|~r − ~r 0 |
˚ ~
µ
JdV
~=
A
(13.4)
4π
|~r − ~r 0 |

---

### Página 270

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO

Torque Magnético
El torque magnético sobre un circuito cerrado Γ está dado por
˛
˛
~ × B)
~
τ = ~r × dF~ = ~r × (I dl

(13.8)

Γ

Γ

Momento Magnético
El momento o dipolo magnético m
~ de un circuito con corriente I está dado por la expresión
˛
~ = IAn̂
m
~ = ~r 0 × I dl
(13.9)
donde A es el área del circuito magnético y n̂ su normal. Para distribuciones de corriente más
complejas, el momento magnético puede ser determinado como
¨
~
~r 0 × KdS
(13.10)
m
~ =
˚
~
m
~ =
~r 0 × JdV
(13.11)

Rodrigo Chi - Marzo 2017

El potencial magnético que genera un momento magnético para puntos muy lejanos a él, está
dado por
~ × (~r − ~r 0 )
~ = µ0 m
A
(13.12)
4π |~r − ~r 0 |3
donde ~r es el lugar donde se quiere determinar el potencial magnético y ~r 0 el lugar donde se
encuentra el momento magnético. Nótese que es posible determinar el campo magnético del
momento mediante
(m
~ · (~r − ~r 0 ))(~r − ~r 0 )
µ0
−m
~
4π|~r − ~r 0 |3
|~r − ~r 0 |2
"

~ =∇
~ ×A
~=
B

#

(13.13)

~ está dado por
El torque de un momento magnético en presencia de un campo magnético B
~
~τ = m
~ ×B

(13.14)

Por otro lado, la energía que tiene un momento es
~
U = −m
~ ·B

(13.15)

---

### Página 271

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO

Recomendaciones
Recuerde que, a diferencia de electrostática, el potencial magnético es un vector y no un
escalar. El potencial magnético vectorial no tiene un significado físico directo.
~
Note que siempre J~ k A.
En general las Ecuaciones 13.2, 13.3 y 13.4 se usan cuando uno quiere conocer el potencial
~ en todo el espacio y se desea conocer
vectorial en algún punto en específico. Si se conoce B
~ puede ser útil la Ecuación 13.5. Note el parecido de esta última con la ley circuital de
A,
Ampère
˛
¨
˛
¨
~
~
~
~
~
~
~
~ · dS
B · dl = µ0
J · dS ←→ A · dl =
B
Γ1

Ω1

Γ2

Ω2

Para calcular el potencial magnético se sigue la analogía de la ley de Ampère.
Los momentos magnéticos están asociados a estudiar el comportamiento de los campos
magnéticos para puntos muy lejanos de donde esta la corriente que lo genera.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 272

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO

II.

Problemas Propuestos
I

#### Problema 13.1

X S

Considere un cilindro hueco infinito de radio R sobre el cual circula sobre su superficie una corriente
homogéneamente distribuida I. Encuentre en todo el
~ Puede usar
espacio el vector potencial magnético A.
el hecho que A(r = 0) = 0.

#### Problema 13.2

R

X S

Considere un circuito en forma de hélice circular con
su eje en z. Por la hélice circula una corriente I, y
está compuesta por 2N vueltas completas y tiene un
paso p. La ecuación paramétrica de la hélice es:

z
z2



x = R cos θ




y = R sin θ
p
θ
2π

I




z =

R

Las vueltas de la hélice están repartidas desde la cota
z1 = −pN hasta la cota z2 = +pN .

p

Rodrigo Chi - Marzo 2017

a) Determine la componente axiales del campo
magnético y del potencial magnético en el origen, Bz (0) y Az (0).
b) Si la longitud del circuito helicoidal es L = 2pN ,
muestre que Bz (0) puede ser escrita de la forma
Bz (0) = B0 f (R, N, p) donde B0 es el campo
magnético creado con solenoide de longitud infinita.
c) Encuentre el valor de f (R, N, p) cuando R

L. ¿Qué relación debe haber entre R y L para
que el Bz (0) sea un 99 % del valor de B0 ?

x

y

z1

---

### Página 273

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO

#### Problema 13.3

y

X I
R

a) Considere un alambre de largo 2L sobre el eje z,
donde fluye una corriente I desde z = −L hasta
z = L como se muestra en la figura. Determine
el potencial magnético vectorial sobre un punto
en el eje y a distancia R del origen. Deduzca el
valor del potencial magnético en el límite L

R.

I
z= L

z=L

O
Parte (a)
z

L

b) Se coloca un nuevo alambre de largo 2L, paralelo al alambre de la parte anterior, por el cual
circula un corriente I en el sentido inverso. El
nuevo alambre se ubica a una distancia d del
primero, perpendicular al plano xy (ver figura).
Determine el potencial magnético vectorial para puntos sobre el plano xy, a una distancias
mucho mayores que L.

I
y

d
x

I

L

Parte (b)

!0
#### Problema 13.4

X S

Considere una esfera de radio R, la cual está cargada
uniformemente con una densidad de carga volumétrica ρ0 constante. La esfera gira entorno a una de sus
diámetros con una velocidad angular constante ω0 ,
como se ilustra en la figura. Encuentre
~ y el potencial magnético
a) El campo magnético B
~ en el centro de la esfera.
vectorial A

R

b) El momento magnético de la esfera.

#### Problema 13.5

A0

A

X I

Un circuito cuadrado rígido de lado L y masa M está
pivoteado en torno a uno de sus ejes (AA0 ) en presen~ uniforme, y el campo
cia de un campo magnético B
gravitatorio. El circuito lleva una corriente I que es
capaz de mantenerlo en equilibrio en el ángulo θ. Encuentre el módulo y el sentido de dicha corriente.

~g

q

q

~B

L

Problemas Propuestos y Resueltos de Electromagnetismo

⇢0

---

### Página 274

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
#### Problema 13.6

X I

Una densidad de corriente determinada por J~ = J0 ẑ,
origina un potencial magnético vectorial

ŷ
ẑ

~ = −ẑ µ0 J0 (x2 + y 2 )
A

x̂

a) Aplique la ecuación vectorial de Poisson para
confirmar el enunciado anterior.

~B?

~A

~ para determinar B.
~
b) Utilice la expresión de A
c) Utilice la expresión para J~ junto a la ley de
~ Compare su respuesta
Ampére y determine B.
con la obtenida en la parte anterior.

#### Problema 13.7

X I

Rodrigo Chi - Marzo 2017

Una esfera no conductora tiene masa m y radio R.
Como se puede apreciar en la figura, una bobina muy
compacta, de cinco vueltas se encuentra enrollada en
la esfera; ésta se encuentra en un plano inclinado que
forma un ángulo θ con la horizontal, de manera tal que
~
la bobina es paralela a éste. Si un campo magnético B
apunta verticalmente en la región, ¿cuál es la corriente
necesaria en la bobina, que permitirá a la esfera permanecer en equilibrio en el plano inclinado?. Muestre
que el resultado es independiente de θ.

~B

q

y
#### Problema 13.8

X S

~B0

Considere una espira de radio R, N vueltas y masa M distribuida homogéneamente por la cual circula
una corriente I0 . Esta espira se coloca en un campo
~ = B0 x̂ inicialmente dismagnético constante de B
puesta con sobre el plano yz con su eje coincidente
con el eje x. Encuentre la frecuencia de pequeñas oscilaciones al perturbar débilmente la espira con respecto
al plano yz.

R

q

x
I0
N

---

### Página 275

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
#### Problema 13.9

X S

Considere un electrón orbitando a un protón, que mantiene una trayectoria circunferencial de radio R debido
a la interacción Coulombiana. Tomando la órbita de
carga como un circuito de corriente eléctrica, calcule
el torque resultante cuando el sistema está inmerso en
~ orientado perpendicularmenun campo magnético B,
te respecto al plano donde vive el protón y el electrón.
La carga del electrón y del protón son conocidas, −e
y e respectivamente , al igual que la masa del electrón
me .

#### Problema 13.10

e, me
R

~B
+e

X I

~m0

Considere tres momentos magnéticos iguales m
~ 0 , ubicados en los vértices
√ de un triángulo rectángulo ABC
de lados a, a y a 2.
a) Determine el trabajo necesario para invertir la
posición del momento magnético ubicado en el
vértice C.
b) ¿Cuál es el torque que sienten los momentos
magnéticos ubicados en A y C?.

C
a

a
~m0

~m0
p
a 2

A

B

#### Problema 13.11

I0

X I

Considere una espira cuadrada conductora de lado a
situada entre dos espiras circulares de radio b (b
a)
también conductoras, ambas espiras circulares están
separadas una distancia 2d (d
b) y colocadas en
forma paralela. La espira cuadrada de encuentra en el
punto medio y su eje de simetría y su eje de simetría,
que es perpendicular al eje de las espiras circulares,
está conectado a un motor que ejerce un torque restaurador ~τ = kθx̂, con k una constante. Si las corrientes son las indicadas en la Figura, determinar la
ecuación que define el ángulo de equilibrio de la espira
cuadrada con la horizontal.

I0

a
I1

Vista Isométrica
Espira Cuadrada

I0
2b

q

a
I1

Espiras Circulares

Vista Frontal

b

I0

y
2b

z

x

Problemas Propuestos y Resueltos de Electromagnetismo

2d

---

### Página 276

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO

III.

Soluciones
P X

Solución 13.1

En este caso se debe usar ley de Ampère para determinar el campo magnético que genera el
cilindro. Para el caso r < R se tiene que
˛
~ = µ0 I = 0 =⇒ B
~ · dl
~ =0
B
Para el caso r ≥ R se obtiene que
˛

~ = µ0 I =⇒ B
~ · dl
~ = µ0 I θ̂
B
2πr

~ ×A
~ = B,
~ integrando a ambos lados y aplicando Teorema de Stokes se obtiene
Ahora dado que ∇
que:
¨
¨
˛
¨
~ =
~ =⇒ A
~ =
~
~ × A)
~ · dS
~ · dS
~ · dl
~ · dS
(∇
B
B
Ω

Ω

Γ

Ω

~ k J~ )
donde Γ es el contorno cerrado de la superficie Ω. Suponiendo que A = A(r)ẑ (siempre A
y que A(r = 0) = 0 se obtiene que en el caso r < R:
˛
¨
~ =
~ =⇒ (A(0) − A(r))L = 0 =⇒ A(r)
~ · dl
~ · dS
~
A
B
=0
Γ1

Ω1

Rodrigo Chi - Marzo 2017

I

W1

r

G1

z=0

z

z=L

Figura 13.1: Superficie y camino de integración para r < R
En la Figura 13.1 se indica Γ1 y Ω1 donde se determinaron la integral de línea y superficie.
Análogamente para el caso r ≥ R, se obtiene que
˛

¨
~ =
~ dl
A·

Γ2

ˆL ˆr
~ =⇒ (A(0)−A(r))L =
~ dS
B·

Ω2

ˆL ˆr
~
B·drdz
θ̂ =

R

µ0 I
µ0 IL
r
θ̂·drdz θ̂ =
ln
2πr
2π
R




---

### Página 277

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
De esto, se determina que
r
µ0 I
~
ln
A(r)
=−
ẑ
2π
R




I

z

W2

r
G2

z=0

z=L

Figura 13.2: Superficie y camino de integración para r ≥ R

Solución 13.2

P X

Dado que sólo interesa la componente axial

µ0 I
Bz (0) =
4π

2πN
ˆ

R2 dθ

−2πN

pθ 2 2
(R2 + ( 2π
))

Problemas Propuestos y Resueltos de Electromagnetismo

pθ
a) La parametrización de la hélice en coordenadas cilíndricas es ~r 0 = Rr̂ + 2π
ẑ con θ ∈
~
[−2πN, 2πN ]. Mientras que el dl = Rdθθ̂ + dz ẑ, dado que se pide el campo magnético en
~r = 0, se llega a
ˆ ~
I dl × (~r − ~r 0 )
µ
~ =
B
4π
|~r − r~0 |3
ˆ
pθ
(Rdθθ̂ + dz ẑ) × (−Rr̂ − 2π
ẑ)
µ0 I
=
pθ 2 2
4π
(R2 + ( 2π
))
ˆ
(R2 dθẑ − Rpθ
dθr̂ − Rdz θ̂)
µ0 I
2π
=
pθ 2 32
4π
))
(R2 + ( 2π

---

### Página 278

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
pθ
p
Usando el cambio de variables u = 2πR
=⇒ du = 2πR
dθ se llega a
pN

Bz (0) =

µ0 I
2p

ˆR

du

(1 + u2 ) 2

− pN
R

pN
R
µ0 I
u
=
2p (1 + u2 ) 2 − pN
R

µ0 I
=
2p
=

pN

(R2 + p2 N 2 ) 2
µ0 IN

+

!

pN

(R2 + p2 N 2 ) 2

(R2 + p2 N 2 ) 2

~ está dado por
Por otro lado, como A
~ r ) = µ0
A(~
4π

ˆ

~
I dl
|~r − ~r 0 |

para calcular Az , habrá que considerar la componente en z de ~r, luego:
µ0
Az (0) =
4π

2πN
ˆ

p
)dθ
I( 2π

=
−2πN

(R2 +



2 1
p
θ )2
2π

pθ
p
Usando el cambio de variables u = 2πR
=⇒ du = 2πR
dθ se llega a
pN

Az (0) =

µ0 I
4π

ˆR

du

− pN
R

(1 + u2 ) 2

Rodrigo Chi - Marzo 2017

pN

R
µ0 I
=
ln |(1 + u2 ) 2 + u| pN
4π
− R





µ0 I  (R2 + (pN )2 ) 2 + pN 
=
ln
4π
(R2 + (pN )2 ) 2 − pN
b) Primero que todo hay que notar que en el exterior de un solenoide el campo magnético
es nulo ya que al darse un camino cualquiera la corriente encerrada siempre será nula,
por lo que Bext = 0. Por otro lado, si se tiene un solenoide infinito, se puede calcular el
campo magnético mediante ley de Ampère considerando un camino cuadrado de largo L
que encierre n espiras por unidad de largo por las cuales circula una corriente I0 , por lo que:
˛
~ = µ0 nIenlaz =⇒ B(z) · L = µ0 nI =⇒ B
~ = nµ0 I ẑ
B · dl

---

### Página 279

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
Este caso
n=

Número de Vueltas
2N
=
=
Largo
2N p
p

Por lo tanto el B0 es
B0 =

µ0 I
p

Si se considera el resultado calculado en (a) y se reordena de manera que pueda colocarse
en función de B0 se tiene:
µ0 IN
Bz (0) =
(R + p2 N 2 ) 2
Np
µ0 I
=
p (R + p2 N 2 ) 21
= B0 
 2  21
1 + NRp
De la expresión anterior es fácil concluir que Bz (0) puede escribirse como Bz = B0 f (R, N, p),
donde f (R, N, p) está dada por:


R
f (R, N, p) = 1 +
Np
c) Finalmente, cuando R
L =⇒
f:



2R
L

2



1 2R
≈1−
2 L




1, y haciendo una aproximación de Taylor para

!2 − 12

2

L
+ O =⇒ f (R, N, p) ≈ 1 − 2
R


2

Luego es posible concluir que para R
L el cuociente entre Bz (0) y B0 esta dado por
Bz (0)
R
=1−2
B0
L


2

Por ende para que el valor de Bz (0) sea dicho cuociente sea un 99 % del valor de B0 , el
cuociente debe tomar el valor de 0,99 con lo que se concluye la relación entre R y L para
que esto se cumpla:
 2
Bz (0)
R
= 0,99 = 1 − 2
B0
L
 2
R
=
L
R
=⇒
= √
L
10 2

Problemas Propuestos y Resueltos de Electromagnetismo

R
f (R, N, p) = 1 +
Np

!2 − 12

---

### Página 280

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
Solución 13.4

P X

a) Primero se determina el campo magnético que genera la esfera, para ello se usa la ley de
Biot-Savart
˚ ~ 0
µ0
J(~r ) × (~r − ~r 0 )dV
B(~r) =
4π
|~r − ~r 0 |3
Esfera

En este caso, ~r = 0, ~r 0 = rr̂ y J~ = ρ0~v = ρ0 ωr sin θϕ̂. Manejando algebraicamente la
expresión anterior
ˆ2π ˆπ ˆR

µ0
~
B(0)
=−
4π

µ0 ρ 0 ω
ρ0 ωr sin θϕ̂ × rr̂ 2
·r
sin
θdrdθdϕ
=
r3
4π

ˆ2π ˆπ ˆR
r sin2 θ·θ̂drdθdϕ

Pero θ̂ = x̂ cos θ cos ϕ + ŷ cos θ sin ϕ − ẑ sin θ, por lo que las integrales en x e y se anulan
debido a la integral en ϕ. Luego el campo sólo tiene componente en z y su valor es
µ0 ρ0 ωẑ
~
B(0)
=
4π

ˆ2π

ˆπ
sin θdθ

dϕ

ˆR

rdr

La única integral compleja es
ˆπ

ˆπ

sin θdθ =

ˆπ

ˆπ
π
sin θdθ− cos2 θ sin θdθ = − cos θ|π0 + cos3 θ =

(1−cos θ) sin θdθ =

Luego el campo vale

Rodrigo Chi - Marzo 2017

~ = µ0 ρ0 ωẑ · 2π · 4 · R = µ0 ρ0 ωR ẑ
B
4π
3 2

Para el caso de potencial magnético se tiene que
˚
~
µ0
JdV
A(~r) =
4π
|~r − ~r 0 |
Esfera

~ ~r y ~r 0 son los mismos que la parte anterior. Entonces
Los vectores J,
µ0
~
A(0)
=
4π

ˆ2π ˆπ ˆR

ρ0 ωr sin θϕ̂ 2
· r sin θdrdθdϕ
r

Pero dado que ϕ̂ = −x̂ sin ϕ + ŷ cos ϕ, la integral en ϕ vuelve anular las dos coordenadas
de modo que
µ0 ρ 0 ω
~
A(0)
=
4π

ˆ2π
ˆπ
ˆR
(−x̂ sin ϕ + ŷ cos ϕ)dϕ sin2 θdθ r2 dr = 0

---

### Página 281

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
b) Para el caso del momento magnético, este esta dado por
˚
~
m
~ =
~r 0 × JdV
~ ya fueron calculados previamente. Reemplanzando
donde ~r 0 y J,
m
~ =

ˆ

ρ0 ω
~
~r 0 × JdV
=−

ˆ2π ˆπ ˆR
r4 sin2 θθ̂drdθdϕ

Nuevamente al descomponer el vector θ̂ se anulan las componentes en x e y. Entonces
ρ0 ωẑ
m
~ =

ˆ2π

ˆR

r4 dr =

sin θdθ

dϕ

Solución 13.8

ˆπ

4πρ0 ωR5
ẑ

P X

Para comenzar este problema es necesario determinar el momento magnético de la espira R, se
supone que la espira ya se ha perturbado un ángulo θ con respecto al eje x, de modo que
m
~ = N I0 πR2 n̂ = N I0 πR2 (cos θx̂ + sin θŷ)
Por otro lado el torque que siente la espira debido al campo magnético presente en el espacio es

Por otro lado debe recordarse que en un sólido rígido
~τ = Iz ω
~˙
La inercia Iz de la ecuación puede ser determinada a partir del teorema eje perpendicular como
Ix = Iy + Iz = 2Iz (debido a la geometría plana de la espira Iy = Iz ) por lo cual
ˆ
M R2
Ix = |~r 0 |2 dm = M R2 =⇒ Iz =
Luego, la ecuación escalar que describe el movimiento de la espira es
M R2
2N I0 B0 π
θ̈ = −N I0 B0 πR2 sin θ =⇒ θ̈ +
sin θ = 0
M
Considerando pequeñas oscilaciones sin θ ≈ θ, por lo cual finalmente se desprende que
2N I0 B0 π
θ = 0 =⇒ ω =
θ̈ +
M

s

2N I0 B0 π
M

Problemas Propuestos y Resueltos de Electromagnetismo

~ = N I0 πR2 (cos θx̂ + sin θŷ) × B0 x̂ = −N I0 B0 πR2 sin θẑ
~τ = m
~ ×B

---

### Página 282

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
Solución 13.9

P X

Se debe comenzar calculando el momento dipolar m
~ = IAn̂, donde I es la corriente y A es el
área. Para este caso la corriente está dada por:
I=

e
dq
=
dt
T

donde e es la carga del electrón, me la masa del electrón y T su periodo. Para encontrar el periodo
se puede relacionar con su frecuencia mediante T = 2π
, con ω = Rv . Luego falta encontrar v,
ω
para ello usamos la interacción coulombiana en el interior de los átomos y la expresión para fuerza
centrípeta:
e2
me v 2
Fe = Fc =⇒
=
4πε0 R2
R
s
e2
=⇒ v =
4πε0 me R
Con la última expresión es posible concluir que el periodo está dado por:
√
2πR
2πR 4πε0 me R
T =
=
v
e
Conocido T , se puede concluir I:
I=

e2
e
√
=
T
2πR 4πε0 me R

Para terminar el cálculo, se considera que el área viene dada por una circunferencia, por lo que
A = πR2 . Con esto se tiene que
e2 R
ẑ
m
~ = √
2 4πε0 me R

Rodrigo Chi - Marzo 2017

Finalmente, el torque está dado por
~ sin 90 = e B
|~τ | = |m
~ × B|
◦

s

R
4πε0 m

---

### Página 283

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO

IV.

Indicaciones Problemas Sin Solución

Indicación 13.3

P X

~ para determinarlo en el punto pedido. Recuerde
Use la definición de potencial magnético A
que ln(1 + ε) ≈ ε cuando ε
1.
Use el principio de superposición para la segunda parte del problema, utilizando el resultado
anterior.

Indicación 13.5

P X

Determine el momento magnético del circuito cuadrado en función θ y el torque que este
siente debido al campo magnético presente.
Determine el torque que provoca el peso sobre la espira. Concluya el problema recordando
que la suma de torques debe ser nula para que la espira se encuentre en equilibrio.

Indicación 13.6

P X

Use la ley de Ampère para encontrar el campo magnético, para ello tome un camino circular
de radio r centrado en el origen sobre el plano xy. Puede ser útil recordar que x2 + y 2 = r2 .

Indicación 13.7

P X

Determine el momento magnético del enrollado de la esfera.
Note que necesariamente debe haber fuerza de roce en el problema para que la esfera se
encuentre en equilibrio. Para determinar el valor de esa fuerza plantee que la sumatoria de
fuerzas sobre la esfera debe ser nulo.
Para concluir el problema imponga que el torque sobre el centro esfera también debe ser
nulo, note los torques involucrados son debidos al momento magnético y al roce.

Problemas Propuestos y Resueltos de Electromagnetismo

~ = µ0 J~
Aplique la ecuación vectorial de Poisson en forma vectorial, recuerde que ∇2 A
significa que ∇ Ax = µ0 Jx , ∇ Ay = µ0 Jy y ∇ Az = µ0 Jz en coordenadas cartesianas.

---

### Página 284

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO
Indicación 13.10

P X

Determine el campo magnético sobre el punto C provocado por los momentos magnéticos
en A y B. Usando ese valor, determine la energía inicial y final del momento magnético,
recuerde que W = ∆U .
Nuevamente determine el campo magnético A y C y aplique la fórmula para determinar el
torque que siente un momento magnético en presencia de un campo magnético.

Indicación 13.11

P X

Dado que las espiras circulares son mucho más grandes que la espera cuadrada, el campo
magnético que afecta a esta última es aproximadamente igual a la superposición del campo
que provocan ambas espiras circulares en el centro de la espira cuadrada.
Use Biot-Savart para determinar el campo magnético que afecta a la espira cuadrada.

Rodrigo Chi - Marzo 2017

Determine el momento magnético de la espira cuadrada y con ello el torque total ella que
siente. Finalmente, deduzca la ecuación que debe cumplirse para que haya equilibrio.

---

### Página 285

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO

V.

Resultados
Problema

P

Respuestas

~
A(r)
=

13.1

a)

P

13.2



0I
− µ2π
ln

r<R
r
R



r≥R

ẑ

µ0 IN

0I
Bz (0) = 2 2 2 1 , Az (0) = µ4π
ln
(R +p N ) 2


b) f (R, N, p) =
c)

P




1+



R
Np



(R2 +(pN )2 ) 2 +pN



(R2 +(pN )2 ) 2 −pN

2 − 12

1√
R
L = 10 2

~ = µ0 I ln
a) A
4π



L
R




q
R2
~ = µ0 I ln
1 + 1 + L2
ẑ si L
R entonces A
4π

2L
R



ẑ

13.3
~ ≈ µ0 I ln
b) A
4π

h 2

x +(d−y)2
x2 +y 2

i

ẑ

~
~
a) B(0)
= µ0 ρ03ωR ẑ A(0)
=0

P

13.4

P

13.5

g tan θ
I = M2LB
y la dirección es horaria según la figura.

P

13.6

~ = µ0 J0 r θ̂
B

P

13.7

Mg
I = 5πBR

P

13.8

ω=

0 ωR
b) m
~ = 4πρ15
ẑ

Problemas Propuestos y Resueltos de Electromagnetismo

q

2N I0 B0 π
M

---

### Página 286

CAPÍTULO 13. POTENCIAL Y MOMENTO MAGNÉTICO

P

Problema

Respuestas

13.9

|~τ | =

e2 B q R
4πε0 m
µ m2

P

13.10

P

13.11

a) W = 2πa
3 ,

b) En A: ~τ =

3µ0 m20
τ = 0. k̂ sale de la hoja de papel.
8πa3 k̂, En C: ~

µ0 I1 I2 a2 b2 cos θeq

= kθeq

Rodrigo Chi - Marzo 2017

(d2 +b2 ) 2

---

### Página 287

Medios Magnéticos

I.

Resumen Teórico

Vector de Magnetización
Dada la composición de momentos magnéticos con lo cual se modelan los materiales, se define
el vector magnetización como
P
m
~i
~
(14.1)
M = lím
∆V →0 ∆V
El cual se define como la densidad de momento magnético por unidad de volumen dentro de un
medio material.

La densidad de corriente de magnetización superficial sobre un medio magnetizado es
~M = M
~ × n̂
K

(14.2)

donde n̂ es la normal de la superficie magnetizada. Por otro lado, la densidad de corriente volumétrica dentro de un material está dada por
~ ×M
~
J~M = ∇

(14.3)

Ley de Ampère Generalizada
Para incluir el efecto del campo magnético que generan las corrientes de magnetización se define
~ como
el vector H
~ = 1B
~ −M
~
H
(14.4)
µ0

Problemas Propuestos y Resueltos de Electromagnetismo

Corrientes de Magnetización

---

### Página 288

CAPÍTULO 14. MEDIOS MAGNÉTICOS
Luego es posible afirmar que

˛
~ = Ilibre
~ · dl
H

(14.5)

donde Ilibre hace referencia a las corrientes reales que circulan por un material magnético y no a
las debidas a la magnetización. En su forma diferencial, puede ser enunciada como
~ ×H
~ = J~libre
∇

(14.6)

Propiedades Magnéticas de los Materiales
~ y H,
~ de modo que
Para gran cantidad de materiales se cumple una relación lineal entre M
~ = χm H
~
M

(14.7)

El valor de χm es conocido como la susceptibilidad magnética y los materiales pueden ser clasificados a partir de ese valor.

Un material paramagnético es aquel que χm > 0.
Un material diamagnético es que χm < 0.
Un material ferromagnético es aquel que χm
1.

Rodrigo Chi - Marzo 2017

Por otro lado, se define el valor de la permeabilidad magnética µ para encontrar la relación lineal
~ yH
~ dada por
entre B
~ = µ0 (H
~ +M
~ ) = µ0 (1 + χm )H
~ = µH
~
B
(14.8)
donde µ = 1+χm . Para los materiales no ferromagnéticos se aproximada que µ ≈ µ0 , sin embargo
los medios ferromagnéticos tienen permeabilidades muy altas y suelen tener un comportamiento
no lineal (curvas de histéresis).

Condiciones de Borde
Las condiciones de borde en magnetostática son las siguientes
B1n = B2n

(14.9)

~2 − H
~ 1) = K
~ libre
n̂ × (H

(14.10)

donde n̂ es la normal a la interfase de los medios.

---

### Página 289

CAPÍTULO 14. MEDIOS MAGNÉTICOS

Recomendaciones
Los medios magnéticos son completamente análogos al caso de los dieléctricos, particularmente con el hecho que en vez de inducirse carga se induce corriente.
En general, las simetrías en las que es posible usar Ley de Ampère no cambian con la
presencia de medios materiales. Tenga precaución en usar de forma correcta las condiciones
de borde para poder determinar el campo magnético en cada medio.
Tenga precaución con identificar bien Ilibre , el cual es una corriente real que circula por el
material. Esta distinción se hace para separar este tipo de corriente con las de magnetización.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 290

CAPÍTULO 14. MEDIOS MAGNÉTICOS

II.

Problemas Propuestos

#### Problema 14.1

X I

Se tiene un dispositivo de simetría cilíndrica que consta de un conductor cilíndrico macizo de radio 3a rodeado por un conductor cilíndrico hueco de radio interior 4a y radio exterior 5a por el cilindro central pasa
una densidad de corriente uniforme J~ = J0 ẑ y por el
cilindro hueco exterior circula una intensidad de corriente de igual magnitud pero de signo opuesto. El
medio entre ambos conductores tiene permeabilidad
µ > µ0 . Calcule el campo magnético en todas partes.
#### Problema 14.2

3a

µ
5a

4a

J0 ẑ

X S

Considere una bobina toroidal de sección rectangular
de N espiras, por cada una de las cuales circula una
corriente I. El radio interior de la bobina es a y el
exterior es b y la altura es h. El núcleo de esta bobina es de un material inhomogéneo en tal forma que
su permeabilidad magnética µ depende tan solo del
ángulo polar θ y satisface

N
q
µ(q )

a

µ0
= 1 + k cos2 θ
µ

h

b

~ en el interior de
Determine la intensidad magnética H
la bobina.

Rodrigo Chi - Marzo 2017

#### Problema 14.3

X S

Un material ferromagnético tiene la forma que se indica en la figura, donde la sección transversal es un
cuadrado de lado de a = 2 cm. El resto de las dimensiones se muestran en la figura con b = 2, 5 cm.
El enrollado tiene N = 500 vueltas, la corriente que
circula es I = 0,3 A y µ = 2500µ0 . Calcule el flujo
neto en la rama central y en la rama del lado derecho.
Desprecie cualquier pérdida de flujo fuera del material
ferromagnético.

6b
I
N

4b

3b

---

### Página 291

CAPÍTULO 14. MEDIOS MAGNÉTICOS
a

#### Problema 14.4

X S

I

Un solenoide infinito de radio a que tiene m espiras
por unidad de largo, lleva corriente I. La permeabilidad magnética del material al interior del solenoide
es
(
µ1 si 0 < θ ≤ π
µ=
µ2 si π < θ ≤ 2π
Encuentre el campo magnético, la intensidad magnética en todo el espacio, la magnetización de los materiales y las densidades de corriente.

µ1
µ1

µ2

µ2

Vista Frontal

#### Problema 14.5

Corte Transversal

X I

Considere un toroide de sección transversal circular A
y de radio medio R como se muestra en la Figura. El
toroide está compuesto por tres medios de permeabilidades µ, µ1 y µ2 (ver Figura). Un cable con corriente I
atraviesa el toroide por su centro por eje perpendicular
al toroide. Para efectos de calculo, puede considerar
que µ → ∞.
~ y B,
~ para cada material si las pera) Calcule H
meabilidades de los materiales son lineales, uniformes e isotrópicas.

µ1
q1
R

q2

µ2

µ !-
I

~ B
~ y las corrientes
c) ¿Cómo cambia (explique) H,
de magnetización si µ1 = αr o µ1 = αθ?.

z
R

X I

Se tiene un cilindro infinitamente largo, de radio R
con su eje coincidente con el eje z y con una magne~ = M0 x̂ perpendicular a su eje.
tización constante M
Determine las corrientes de magnetización (volumétricas y superficiales) y el campo magnético en el eje del
cilindro.

~ = M0 x̂
M

Problemas Propuestos y Resueltos de Electromagnetismo

b) Si las permeabilidades de los materiales son lineales uniformes e isotrópicas ¿existirían densidades de corriente de magnetización?. Si existieran, calcúlelas.

#### Problema 14.6

a

---

### Página 292

CAPÍTULO 14. MEDIOS MAGNÉTICOS
#### Problema 14.7

X I

Por el interior de un cilindro infinito de radio a y permeabilidad magnética µ1 , circula una corriente I0 en
la dirección ẑ. A este cilindro lo rodea un casquete
cilíndrico de radio interno b y radio externo c. El casquete consiste en dos mitades, de permeabilidad µ2 y
µ3 respectivamente (ver figura). Por el casquete circula la misma cantidad de corriente I0 pero en sentido
opuesto al del cilindro interno (es decir, en la dirección
ẑ). Asuma que las densidades de corriente al interior
de estos materiales es homogénea.
a) Encuentre una expresión para la corriente total I(r) que atraviesa una superficie circular de
radio r arbitrario, concéntrica a los cilindros.

µ3

µ1

a
b

c
µ2

~ y el camb) Encuentre la intensidad magnética H
~ en todo el espacio.
po magnético B
c) Determine el valor de las corrientes superficiales
~ M inducidas por la magnetización M
~ de los
K
medios, en cada una de las superficies.

Rodrigo Chi - Marzo 2017

#### Problema 14.8

X I

Considere una línea de transmisión coaxial llena de un
material con permeabilidad magnética no lineal, con
un conductor interno sólido de radio a y un conductor externo muy delgado, de radio interior b según se
muestra en la figura. Se sabe que en el conductor interno circula una corriente I0 hacia afuera de la hoja, y
vuelve en dirección opuesta por el conductor externo.
En ambos conductores la corriente se reparte en forma
homogénea, y ambos se pueden suponer muy largos.
Si la curva de magnetización del material se puede
aproximar como
B=

1,6H
1000 + H

a) Campo magnética en todo el espacio.
b) Vector de magnetización en el medio material.

Material Magnético

a
b

---

### Página 293

CAPÍTULO 14. MEDIOS MAGNÉTICOS
X I

El sistema de la Figura representa un conductor
cilíndrico de resistividad η el cual está sometido a
una diferencia de potencial V0 . Este conductor posee
además características magnéticas,

 con una permeabilidad relativa µ(r) = µ0 1 + Rr , tal como se muestra
en la Figura. Suponiendo que la corriente se distribuye
en forma homogénea al interior del conductor y que
V0
D
L
R, se pide
~ yB
~ en el interior y exterior
a) Estimar campos H
(pero en las cercanías) del conductor.

R

D

+

#### Problema 14.9

µ, rs

L

z

~.
b) Estimar la magnetización M
c) Determinar las densidades de corrientes de magnetización y libre en el conductor.
#### Problema 14.10

X I

z

Un cubo de lado a está hecho de un material ferromagnético el cual está permanentemente magnetizado, con una magnetización igual

a

~ = M0 x ẑ
M
a
x

a

y

X S

Considere N vueltas de un alambre conductor se han
enrollado sobre un toroide de hierro dulce de sección
transversal S y permeabilidad µ. El radio medio del
toroide es R y posee un entrehierro de longitud ` como
se muestra en la Figura. La corriente I que circula por
el alambre es suficientemente grande de manera que
~ adopta su valor de saturación
la magnetización M
~ s = Ms θ̂ en el hierro dulce.
M
~ yB
~ en todo el toa) Encuentre los valores de H
roide.
b) Cuando la corriente I se interrumpe, la magnitud de la magnetización decrece a su valor
~ r = Mr θ̂ en el hierro dulce. Enremanente M
~ yB
~ en esta situación.
cuentre los valores de H

q̂
r̂

R
`
N
µ
I

S

Problemas Propuestos y Resueltos de Electromagnetismo

Encuentre las densidades de corriente de magnetización presentes en el cubo.
#### Problema 14.11

a

~
M

---

### Página 294

CAPÍTULO 14. MEDIOS MAGNÉTICOS

III.

Soluciones
P X

Solución 14.2

~ = B(r, θ)θ̂ y H
~ =
Dada la simetría del problema, el campo magnético debe ser de la forma B
H(r, θ)θ̂. Por otro lado, dado que el medio tiene una permeabilidad dependiente de θ, existe un
cambio progresivo en el material. Lo anterior puede ser aproximado como un cambio de medio,
donde el campo magnético es normal a la interfase de cambio (cada radio vendría siendo una
~ no tiene dependencia de
interfase). Luego, como B1n = B2n se deduce que dentro del toroide B
θ. Luego, por Ampère
˛

ˆ2π
~ = Ilibre =⇒
~ · dl
H

H(r, θ)θ̂ · rdθθ̂ = N I

Como en este caso

~ = µH
~ =⇒ H(r, θ) = B(r) = 1 + k cos θ B(r)
B
µ
µ0
Por lo tanto
ˆ2π

1 + k cos2 θ
rB(r)
B(r)rdθ = N I =⇒
µ0
µ0

ˆ2π
(1 + k cos2 θ)dθ = N I

Resolviendo la integral y despejando B(r) se tiene que

Rodrigo Chi - Marzo 2017

µ0 N I
rB(r)
(2π + kπ) = N I =⇒ B(r) =
µ0
π(2 + k)r
por lo que finalmente
~ =
H

Solución 14.3

µ0 N I
1 + k cos2 θ N I
=
θ̂
π(2 + k)r
2+k
πr

P X

Para resolver este problema se usará la técnica de reluctancias. En primera instancia, es necesario
definir reluctancia como
l
R=
µA
donde l es el largo, µ la permeabilidad y A la sección transversal del medio por donde pasa un
respectivo flujo. La idea de este método es emular un circuito simple con resistencias, en el cual

---

### Página 295

CAPÍTULO 14. MEDIOS MAGNÉTICOS
la fuente de tensión es el equivalente al enrollado con corriente (V −→ N I), las corrientes es
equivalente al los flujos magnéticos (I −→ Φ) y las resistencias a las reluctancias (R −→ R).
Para aplicar este método, es necesario identificar las reluctancias en el circuito magnético, para
ello se verifica en que ramales del circuito pasa el mismo flujo.

6b
I

N

4b

3b
Figura 14.1: Determinación de Reluctancias.

En la Figura 14.1, es posible identificar los caminos por los cuales circula el mismo flujo. Cada
uno de esos caminos Γ1 , Γ2 y Γ3 tienen asociadas los siguientes valores de reluctancias:
R1 =

10b
µA

R2 =

4b
µA

R3 =

10b
µA

Una vez determinado los valores de las reluctancias, se procede a plantear el circuito análogo.
R1

NI

R2

R3

Figura 14.2: Circuito Equivalente.
Las incógnitas en este circuito son los flujos Φ1 , Φ2 y Φ3 como es mostrado en la Figura 14.2.
Planteando la ley de Kirchoff de Nodos se obtiene que
Φ1 = Φ2 + Φ3
Mientras si se plantea la ley de Kirchoff de Voltajes
N I = R1 Φ1 + R2 Φ2
RΦ2 = R3 Φ3

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 296

CAPÍTULO 14. MEDIOS MAGNÉTICOS
Usando las tres ecuaciones anteriores es posible despejar los valores pedidos, de modo que
N I0 µA
18b
N I0 µA
Φ3 =
45b

Φ2 =

Solución 14.4

P X

Dada la geometría del problema, el campo magnético provocado por el solenoide debe ser paralelo
al eje del cilindro. Recuérdese en el solenoide ideal e infinitamente largo se hace el supuesto que
el campo magnético es nulo fuera del mismo.
a
z
I

L

y

~B1

~B2

~1
H

~2
H

µ1

µ2

Rodrigo Chi - Marzo 2017

Figura 14.3: Cálculo de Campo Magnético Usando Ley de Àmpere.

En la Figura 14.3 se muestra el rectángulo con el cual puede ser usada la Ley de Ampère de la
siguente forma
˛
~ = Ilibre =⇒ H1 · L = mLI =⇒ H
~ 1 · dl
~ 1 = mI ẑ
H
~ 2 , por lo que también se puede concluir
Análogamente, es posible hacer el mismo análisis para H
~ 2 = mI ẑ
H
~2 − H
~ 1) = K
~ libre ya que en la
El resultado anterior es coherente con la condición de borde n̂ × (H
~1 = H
~ 2 . Por otro lado, los
interfase de los medios no hay corrientes libres circulando por ende H
campos magnéticos están dados por
~ 1 = µ1 mI ẑ
B

~ 2 = µ2 mI ẑ
B

---

### Página 297

CAPÍTULO 14. MEDIOS MAGNÉTICOS
A partir de lo anterior, se procede a determinar las magnetizaciones de cada medio, las cuales
~ = µ0 ( H
~ +M
~ ), por lo tanto
cumplen B
!

!

µ1
− 1 mI ẑ
µ0

~1 =
M

~2 =
M

µ2
− 1 mI ẑ
µ0

~ × n̂
Ahora, para encontrar las densidades de corrientes presentes se usan las definiciones K~M = M
~ ×M
~ . Hay que tener precaución debido a que los medios tienen más de una normal.
y JˆM = ∇

r̂
µ1
ŷ

y

~1
K

ŷ
µ2

~2
K

x

r̂
Figura 14.4: Cálculo de Corrientes de Magnetización.

Siguiendo la Figura 14.4, se pueden determinar las corrientes superficiales en la división son
µ1
− 1 mI ẑ × (−ŷ) =
µ0

"

µ2
µ2
− 1 mI ẑ × ŷ = −
− 1 mI x̂
µ0
µ0

~2 =
K

!

#

µ1
− 1 mI x̂
µ0

!

!

#

!

Mientras que en los mantos se tiene que
"

µ1
− 1 mI ẑ × r̂ =
µ0

"

µ2
− 1 mI ẑ × r̂ =
µ0

~1 =
K
~2 =
K

!

#

µ1
− 1 mI θ̂
µ0

!

!

#

µ2
− 1 mI θ̂
µ0

!

~ es constante J~ = ∇
~ ×M
~ = 0.
Finalmente, dado que M

Solución 14.11

P X

a) En primera instancia, debido al solenoide enrolado en el toroide, existe un campo magnético
confinado dentro del material magnético y también en el entrehierro. A priori, se supone

Problemas Propuestos y Resueltos de Electromagnetismo

"

~1 =
K

---

### Página 298

CAPÍTULO 14. MEDIOS MAGNÉTICOS
~1 y B
~ 1 en el hierro dulce y los campos H
~0 y B
~ 0 en el entrehierro.
que existen los campos H
Adicionalmente, en este tipo de problema se suele suponer que el campo magnético es más
bien homogéneo dentro del toroide, por lo cual es una buena aproximación es tomar el
~ yB
~ en todos los puntos.
camino medio del mismo para calcular H
Entonces, usando Ley de Ampère al camino medio de radio R y usando el supuesto que
~ 1 = H1 θ̂ y H
~ 0 = H0 θ̂ se obtiene que
H
˛
~ = N I =⇒ H1 · (2πR − `) + H0 · ` = N I
~ · dl
H
Dado que el hierro dulce alcanzó su máxima magnetización, se puede afirmar que
~ 1 = µ0 ( H
~1 + M
~ s)
B
El paso clave del problema, es usar la siguiente condición de borde
~0 − B
~ 1 ) · n̂ = 0 =⇒ B0n − B1n = 0 =⇒ B0n = B1n
(B
Nótese que es posible aplicar esta condición ya que el campo magnético es perpendicular
~ debe ser
a las interfases del problema (hierro-entrehierro y entrehierro-hierro), por ende B
~
~
continuo en esos puntos. Adicionalmente, como H0 = µ0 B0 se obtiene que
~ 1 = N I − Ms ` θ̂
H1 (2πR − `) + H1 ` + Ms ` = N I =⇒ H
2πR
En consecuencia,
~ 0 = N I − Ms ` θ̂ + M
~s
H
2πR

~1 = B
~0 = 1
B
µ0

N I − Ms `
~s
θ̂ + M
2πR

!

Rodrigo Chi - Marzo 2017

~ s −→ M
~ r.
b) Usando el resultado obtenido en la parte anterior, se tiene ahora que I = 0 y M
Por lo que los valores de los campos son
~ 1 = − Mr ` θ̂
H
2πR
~0 = M
~ r − Mr ` θ̂
H
2πR
!
1 ~
Mr `
~
~
B1 = B0 =
Mr −
θ̂
µ0
2πR

---

### Página 299

CAPÍTULO 14. MEDIOS MAGNÉTICOS

IV.

Indicaciones Problemas Sin Solución

Indicación 14.1

P X

Utilice la Ley de Ampère para determinar el campo magnético en todo el espacio. Debe
separar el problema en cuatro casos.
Recuerde que se considera que los conductores tiene una permeabilidad igual a µ0 .

Indicación 14.5

P X

Aplique la Ley de Ampère en un camino circular alrededor del alambre con corriente I. Por
~ es continuo para un mismo radio
condiciones de borde B1n = B2n , el campo magnético B
r (ie. el campo magnético no depende del medio en el cual se encuentre).
~ en cada medio: H
~ 1, H
~2 y H
~ 3 , de modo que la integral de
Note que existen tres vectores H
camino de Ampère debe dividirse en tres.
~ −→ 0 en ese medio.
El hecho de que µ −→ ∞ provoca que el vector H
~ yB
~ en cada medio, determine el vector magnetización
Una vez determinado los vectores H
~
M y con ello las densidades de corrientes de magnetización.

P X

Para determinar las corrientes de magnetización (volumétricas y superficiales) en el cilindro
es útil recordar que x̂ = cos θr̂ − sin θθ̂ en coordenadas cilíndricas.
Una vez determinadas las corrientes de magnetización, use Biot-Savart para determinar el
campo en el eje z. Note que debido a que el cilindro es infinito el campo magnético debe
ser igual en todo el eje del cilindro, por lo que se recomienda determinarlo en el centro del
cilindro.

Indicación 14.7

P X

Para determinar la corriente I(r) recuerde que esta se distribuye en forma homogénea, por
I0
I0
~
lo cual J~interior = πa
2 ẑ y Jexterior = − π(c2 −b2 ) ẑ

Problemas Propuestos y Resueltos de Electromagnetismo

Indicación 14.6

---

### Página 300

CAPÍTULO 14. MEDIOS MAGNÉTICOS
Use la Ley de Ampère para determinar el campo magnético en todas las zonas. Note que
en el caso b < r < c se tiene que aplicar la condición de borde B1n = B2n .
~ yB
~ determine M
~ y con ello las cinco densidades de corriente superficiales que
Conocido H
existen en el problema.

Indicación 14.8

P X

~
Use la Ley de Ampère dentro del material magnético para determinar el valor de H.
~ y junto a la relación que da el enunciado del problema es posible determinar
Determinado H
~ Finalmente, es directo determinar M
~ a partir de lo anterior.
el valor de B.

Indicación 14.9

P X

~ y H.
~
Como L
R es posible aplicar la Ley de Ampère para determinar B
~ y las corrientes de magnetización.
Con lo anterior, determine M

Indicación 14.10

P X

Rodrigo Chi - Marzo 2017

Identifique las seis normales del cubo y haga los productos cruces correspondientes para
determinar las densidades superficiales. La densidad volumétrica es directa de aplicar el
rotor al vector magnetización.

---

### Página 301

CAPÍTULO 14. MEDIOS MAGNÉTICOS

V.

Resultados
Problema

P

14.1

Respuestas

~ =
B










µ0 rJ0
2 θ̂

r < 3a

9µa2 J0
2r θ̂

3a < r < 4a





µ 0 J0


 2r (25a − r )θ̂

4a < r < 5a
r > 5a

P

14.2

~ = 1+k2 cos2 θ N I θ̂
H
2+k
πr

P

14.3

I0 µA
I0 µA
Φcentral = N 18b
y Φderecho = N 45b

~ = mI ẑ, B
~ =
H

P

14.4

14.5

P

14.6

µ1 mI ẑ
µ2 mI ẑ

 

 µ1 − 1 mI ẑ
µ
~ =


M
 µ2 − 1 mI ẑ
µ0

si 0 < θ ≤ π
si π < θ ≤ 2π

si 0 < θ ≤ π
si π < θ ≤ 2π

µ1 µ2 I
µ2 I
µ1 I
~ =
~
~
~
a) B
R(θ1 µ2 +θ2 µ1 ) θ̂ H1 = R(θ1 µ2 +θ2 µ1 ) θ̂ H2 = R(θ1 µ2 +θ2 µ1 ) θ̂ H3 = 0
µ2 −µ0
µ2 I
µ1 I
~
~
~ 1 | = µ1 −µ0
b) |K
µ0 R(θ1 µ2 +θ2 µ1 |K2 | =
µ0 R(θ1 µ2 +θ2 µ1 J = 0

~ = M0 ẑ sin θ, B
~ = µ0 M0 x̂
J~ = 0, K
2R

Problemas Propuestos y Resueltos de Electromagnetismo

P



---

### Página 302

CAPÍTULO 14. MEDIOS MAGNÉTICOS
Problema

Respuestas

a) I(r) =

Rodrigo Chi - Marzo 2017

P

14.7

P

14.8

P

14.10

P

14.11











I0 r 2
a2

r<a

I0

a<r<b






r 2 −b2


I
−
b<r<c

c −b


r>c

I0 r
r<a

2πa2 θ̂






I0


a<r<b

2πr θ̂
~
b) H(r)
=

µ2
I0 c2 −r 2

b<r<c 0<θ<π
 µ2 +µ
2 θ̂

3 πr c −b


µ
I
c
−r

b < r < c pi < θ < 2π

2 θ̂

 µ2 +µ3 πr c −b
r>c

I0 r

r<a

2πa2 θ̂






I0
a<r<b
2πr θ̂
~
B(r)
=



µ2 µ3 I0 c2 −r 2



µ
c2 −b2 θ̂ b < r < c

 2 +µ3 πr
r>c
~ = 1,6I0 θ̂, H
~ = I0 θ̂
a) B
2000πr+I0
2πr


1,6I0
I0
~ =
−
b) M
µ0 (2000πr+I0 )
2πr θ̂
~ 1 = M0 x x̂, K
~ 2 = − M0 x x̂, K
~ 3 = M0 x̂. En las otras caras no hay densidades
K
a
a
M
superficiales. J~ = − a ŷ


~ 1 = N I−Ms ` θ̂, H
~ 0 = N I−Ms ` θ̂ + M
~ s, B
~1 = B
~ 0 = 1 N I−Ms ` θ̂ + M
~s .
a) H
2πR
2πR
µ0
2πR


~0 = M
~ r − Mr ` θ̂, B
~1 = B
~0 = 1 M
~ r − Mr ` θ̂ .
~ 1 = − Mr ` θ̂, H
b) H
2πR
2πR
µ0
2πR

---

### Página 303

Parte IV
Campos Electromagnéticos Variantes en
el Tiempo

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 304

Rodrigo Chi - Marzo 2017

---

### Página 305

Ley de Faraday-Lenz

I.

Resumen Teórico

Ley de Faraday
La ley de Faraday indica que la fem (fuerza electromotriz inducida) en un circuito cerrado está
dado por
dΦ
(15.1)
ε=−
dt
donde Φ es el flujo de campo magnético por el área respectiva.

La corriente inducida en un circuito debido a la variación temporal del flujo del campo magnético
siempre es opuesta al crecimiento/decrecimiento del mismo.

Ley de Faraday (Forma Diferencial)
En presencia de campo magnéticos que dependen del tiempo, se cumple que
~
~ ×E
~ = − ∂B
∇
∂t

(15.2)

Nótese el hecho que el campo eléctrico deja de ser conservativo cuando existen campos dependientes del tiempo.

Problemas Propuestos y Resueltos de Electromagnetismo

Ley de Lenz

---

### Página 306

CAPÍTULO 15. LEY DE FARADAY-LENZ

Ley de Faraday (Forma Diferencial)
Integrando en una superficie la Ecuación 15.2, se obtiene que
˛
¨
∂
~
~
~ · dS
B · dl = −
B
∂t
Γ

(15.3)

Ω

donde Ω es la superficie delimitada por Γ.

Inducción por Fuerza de Lorentz
Las conductores también pueden sufrir diferencias de potencial en algunos de sus puntos si estos se
~ El campo eléctrico
encuentran moviéndose con velocidad ~v en campos magnéticos constantes B.
inducido está dada por
~ = −~v × B
~
E
(15.4)
Por lo cual el módulo de la fem estará dada por
ˆ
~
~ · dl
|ε| = (~v × B)

(15.5)

Recomendaciones

Rodrigo Chi - Marzo 2017

La ley de Faraday viene a cambiar lo visto en los capítulos anteriores, donde el único
generador de campo eléctrico eran las cargas. Como fue mostrado, la variación del flujo
magnético en el tiempo también inducen campos eléctricos en el tiempo.
A la naturaleza no le gustan los cambios, siempre intentará oponerse al cambio de flujo
magnético con la generación de la corriente inducida. Si el flujo aumenta, aparecerá una
corriente inducida que intentará hacer que ese flujo disminuya. Por otro lado, si el flujo
magnético está disminuyendo aparecerá una corriente oponiéndose a eso.
Para determinar el sentido de la corriente inducida basta hacer el análisis anterior del punto
anterior, sin la necesidad de otros cálculos.

---

### Página 307

CAPÍTULO 15. LEY DE FARADAY-LENZ

II.

Problemas Propuestos

#### Problema 15.1

X S

b

Una bobina muy larga de radio b tiene m vueltas por
unidad de largo y lleva una corriente I(t) = I0 sin ωt.

I(t)

a) Encuentre el campo magnético dentro de la bobina.
b) Encuentre el campo eléctrico dentro de la bobina.
c) Encuentre el campo eléctrico fuera de la bobina.
#### Problema 15.2

X I

y

Un carrito de masa m que se desplaza con velocidad
v0 x̂, hasta llegar a una región en que existe un campo
magnético uniforme en x = 0.
a) Si el carrito posee solamente una resistencia R
(Figura a), encuentre la velocidad del carrito
como función del tiempo.

~v = v0 x̂
R

a

x

(a) Circuito Simple

y

~B = B0 ẑ

~v = v0 x̂

a

C

R

x

(b) Circuito RC

Problemas Propuestos y Resueltos de Electromagnetismo

b) Si el carrito posee una resistencia R y un condensador C inicialmente descargado (Figura b),
encuentre la velocidad del carrito como función
del tiempo y la carga del condensador en el tiempo.
En ninguno de los dos casos, considere el campo
magnético producido por la corriente en el circuito
por ser mucho menor al campo externo constante y
suponga que el carrito es muy largo por lo que no
debe preocuparse de lo que ocurre una vez que entra
entero al campo.

~B = B0 ẑ

---

### Página 308

CAPÍTULO 15. LEY DE FARADAY-LENZ
#### Problema 15.3

X S

Un generador de corriente G produce una corriente
I(t) en un circuito formado por un riel conductor sin
roce, en forma de U y una barra conductora de masa
m que atraviesa los rieles en dirección perpendicular~
mente. Un campo magnético constante y uniforme B
que apunta perpendicular al plano del circuito existe
en todo el espacio. La corriente I(t) que circula en el
circuito varía en el tiempo de acuerdo con
I(t) =



 0

t<0
bt 0 < t < T


0 T <t

I(t)

G

⇥⇥ ⇥ ⇥ ⇥ ⇥
⇥⇥ ⇥ ⇥ ⇥ ⇥
⇥⇥ ⇥ ⇥ ⇥ ⇥
⇥⇥ ⇥ ⇥ ⇥ ⇥
⇥⇥ ⇥ ⇥ ⇥ ⇥
⇥⇥ ⇥ ⇥ ⇥ ⇥
⇥⇥ ⇥ ⇥ ⇥ ⇥

⇥
⇥
⇥
⇥
⇥
⇥
⇥

L

Para t ≤ T , determine la fuerza electromotriz inducida en el circuito y la velocidad de la barra en función
del tiempo.
#### Problema 15.4

X I

Un disco de material aislante de radio R tiene en su
borde una carga uniformemente distribuida λ [C/m] y
está suspendido horizontalmente de un hilo que coincide con su eje. Dentro de un círculo más pequeño de
~ uniforme
radio a < R existe un campo magnético B
paralelo al eje. El disco está inicialmente en reposo.
En t = 0 se desconecta la fuente del campo magnético, el que cae a cero después de un corto intervalo
de tiempo. Si I es el momento de inercia del disco,
encuentre:

z

R

a

l

Rodrigo Chi - Marzo 2017

a) La velocidad angular final del disco
b) ¿Depende ésta de la forma en que cae a cero el
campo B?
#### Problema 15.5

X I

D

Una bobina circular plana de N vueltas tiene diámetro D y resistencia R. La bobina se orienta con su
eje paralelo a un campo magnético B uniforme y los
extremos de la bobina se conectan a un dispositivo
capaz de medir la carga que pasa a través de él. Si
la bobina se gira en 180◦ sobre un eje perpendicular
al campo magnético el dispositivo mide una carga Q.
Encuentre el valor de B en términos de N , D, R y
Q.

N
Dispositivo
Medidor de Carga

---

### Página 309

CAPÍTULO 15. LEY DE FARADAY-LENZ
#### Problema 15.6

X S

Una barra conductora de masa m desliza sin roce sobre dos rieles conductores paralelos separados una distancia b. El circuito posee un switch que puede cambiar entre dos posiciones. Si el switch se encuentra en
la posición 1, los rieles quedan conectados únicamente
mediante una resistencia R, mientras que si se mueve
a la posición 2, los rieles quedan conectados por la
misma resistencia R y una batería que provee un diferencia de potencial V0 (ver Figura). Hay un campo
~ = B0 ẑ uniforme perpendicular R
magnético uniforme B
al plano de la Figura.
a) Considere que inicialmente el switch se encuentra en la posición 1 y se le imparte una velocidad
v0 a la barra en t = 0. Determine la velocidad
en función del tiempo de la barra y el desplazamiento máximo que alcanza la misma.

-
-
-
-
-
-
-
-

~B = B0 ẑ
-
-
-
-
-
-
-
-

-
-
-
-
-
-
-
-

+

-
-
-
-
-
-
-
-

-

-

-

-
-
-
-
-
-
-

-
-
-
-
-
-
-
-

b

-

V0

b) Suponiendo que la barra alcanzó su máximo
desplazamiento, el switch se cambia la posición
2 y se reinicia el tiempo. Determine nuevamente
la velocidad de la barra en el tiempo.

X S

Los hornos de inducción se usan para fundir metales.
Ellos consisten en grandes contenedores donde caben
hasta 30 toneladas, aislados térmicamente y rodeados
de una gran bobina donde circula corriente. A modo
de ejemplo, considere el siguiente modelo simplificado.
Una barra conductora de radio a, largo h y conductividad g se coloca en la interior de una bobina que
tiene n vueltas por unidad de longitud y que lleva una
corriente alterna I = I0 sin ωt con ω la frecuencia
angular. Calcule la potencia disipada en el cilindro.
Desprecie efectos de borde. (Propuesto: ¿Cuál es el
valor de la corriente que circula dentro del cilindro?).

a
h

Problemas Propuestos y Resueltos de Electromagnetismo

#### Problema 15.7

---

### Página 310

CAPÍTULO 15. LEY DE FARADAY-LENZ
#### Problema 15.8

X I

Una espira circular de radio a, masa M y resistencia R
se deja caer desde z = 0 con su eje de simetría vertical
en una zona donde el campo magnético es axialmente
simétrico alrededor del eje z y cuya componente vertical es Bz = Cz. El eje de la espira coincide con el
eje de simetría del campo.
a) ¿En qué dirección fluye la corriente en la espira mientras cae bajo la acción de la fuerza de
gravedad?.

z

~B

a
~g
M, R

b) Encuentre la corriente en la espira en función
de la velocidad. Desprecie las contribuciones al
flujo provenientes de la corriente inducida.
c) Determine las fuerzas que actúan sobre la espira
provenientes axial y radial del campo magnético.
d) Encuentre la velocidad de la espira después que
ha caído un largo tiempo.
X I

a

Rodrigo Chi - Marzo 2017

Una espira rectangular de resistencia R, ancho a, largo L (muy grande) y de masa m cae bajo efecto de la
~ perpendicular
gravedad bajo un campo magnético B
al plano de la espira y no nulo solo en la parte superior
del plano. Asuma que una parte de la espira siempre
está afuera de la región de campo magnético, determine la velocidad terminal y el sentido de la corriente
inducida en la espira.
#### Problema 15.10

g

⇥ ⇥ ⇥
⇥ ⇥ ⇥
~B ⇥ ⇥ ⇥
⇥ ⇥ ⇥
⇥ ⇥ ⇥
⇥ ⇥ ⇥

⇥ ⇥ ⇥ ⇥ ⇥⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥ ⇥⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥ ⇥⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥ ⇥⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥ ⇥⇥ ⇥ ⇥
⇥ ⇥ ⇥ ⇥ ⇥⇥ ⇥ ⇥

⇥ ⇥ ⇥
⇥ ⇥ ⇥
⇥ ⇥ ⇥
⇥ ⇥ ⇥
⇥ ⇥ ⇥
⇥ ⇥ ⇥

X S

La parte final de un riel de resistencia nula está conectada a un condensador de capacidad C, el cual
está inicialmente cargado a un voltaje V0 (ver figura). El sistema se encuentra además en presencia de
~ homogéneo y perpendicular
una campo magnético B
al plano de la figura. Una barra de masa m y resis- V0
tencia R es dispuesta perpendicularmente a los dos
rieles separados una distancia L, de modo que puede
deslizarse sobre ellos sin roce. En t = 0, se cambia
la configuración del interruptor de modo que la barra
comienza a moverse desde el reposo hacia la derecha.
Encuentre la velocidad de la barra cuando t → ∞ .

~B

+

#### Problema 15.9

⇥ ⇥
⇥ ⇥
⇥ ⇥
C ⇥ ⇥
⇥ ⇥
⇥ ⇥
⇥ ⇥

m

⇥
⇥
⇥
⇥
⇥
⇥
⇥

L

---

### Página 311

CAPÍTULO 15. LEY DE FARADAY-LENZ

I

#### Problema 15.11

X I

Una barra metálica de largo d y espesor despreciable
se mueve con rapidez v constante, de forma paralela a
una corriente eléctrica de intensidad I. Si el extremo
izquierdo de la barra está a una distaba a del cable
con corriente, determine la diferencia de potencial entre los extremos de la barra. ¿Cuál es el valor de esa
diferencia cuando a
d? .

~v
a

d

z

#### Problema 15.12

~B = B0 k̂

X S

W

El disco de Faraday consiste en un disco conductor de
radio R que gira con velocidad angular Ωk̂ bajo la ac~ = B0 k̂ (ver
ción de un campo magnético constante B
Figura). Calcule el módulo de la fuerza electromotriz
(fem) inducida entre el centro y el borde del disco.

e

R

#### Problema 15.13

X I

~B0

Considere un cable infinito de sección transversal cuadrada de largo `, sobre el cual cruza una corriente I
con una densidad de portadores n homogénea (ie. cantidad de portadores por unidad de volumen) y carga e.
Si todo el sistema esta bajo la influencia de un campo
~ 0 perpendicular a la dirección
magnético uniforme B
de la corriente. Encuentre el voltaje (voltaje de Hall)
que se genera entre las placas transversales.

`

e

V

I

Problemas Propuestos y Resueltos de Electromagnetismo

`

---

### Página 312

CAPÍTULO 15. LEY DE FARADAY-LENZ

III.

Soluciones

Solución 15.1

P X

~ = B(z)ẑ y se
a) En primera instancia se debe usar el hecho que dentro de una bobina se tiene B
está trabajando en un régimen cuasiestacionario (se desprecia la corriente desplazamiento).
Luego, usando Ley de Ampère para el camino Γ recorrido en sentido antihorario y suponiendo
que la bobina tiene una largo L, se obtiene que
˛
~ = µ0 Ienlaz =⇒ B(z, t) · L = µ0 mLI(t)
~ · dl
B
Γ1

Lo que finalmente implica que
~ = µ0 mI0 sen(ωt)ẑ
B
b) Usando un camino circular de radio r < b, se tiene que por ley de Faraday-Lenz
˛
¨
∂
~ =⇒ E(r, t)·2πr = −πr2 ∂ B(t) =⇒ E(r,
~
~ dS
~ t) = − rµ0 mI0 ω cos(ωt) θ̂
~
B·
E·dl = −
∂t
∂t
Γ2

Ω

c) Usando el mismo procedimiento anterior para un r ≥ b
¨
˛
∂
~ =⇒ E(r, t)·2πr = −πb2 ∂ B(t) =⇒ E(r,
~
~ dS
~ t) = − b µ0 mI0 ω cos(ωt) θ̂
~
B·
E·dl = −
∂t
∂t
2r
Ω

b

Rodrigo Chi - Marzo 2017

Γ2

~B

G2

~E

G1

Figura 15.1: Senoloide

---

### Página 313

CAPÍTULO 15. LEY DE FARADAY-LENZ
Solución 15.3

P X

La fuerza electromotriz inducida es
dΦ
d
ε=−
=−
dt
dt

ˆL ˆx(t)
−B ẑ · dxdyẑ

de este modo se obtiene que
ε = BLẋ
Por otro lado, considerando que la fuente de corriente es capaz de mantener la corriente constante
(en el sentido de la figura) y sin alteraciones durante cada período de tiempo (ie. se ignora la
corriente adicional inducida en el circuito), se tiene que la velocidad de la barra está dada por
~ = −I(t)dy ŷ × −B ẑ = −BI(t)dyx̂ =⇒ F~ = BI(t)Lx̂
dF
Entonces
dv
m = BLI(t) =⇒
dt

ˆv(t)
ˆt
BL
dv =
I(t)dt
m

Si t < 0
v(t) = 0
Si 0 < t ≤ T

ˆt
btdt =

BLbt2
2m

Por lo tanto se tiene que la fem inducida en el circuito es

ε(t) =








B 2 L2 bt2




2m

Solución 15.6

t<0
0<t≤T

P X

~ = B0 ẑ (saliendo
a) La fuerza que mueve a la barra está determinada por el campo magnético B
de la hoja) y la corriente que circula por el circuito. La corriente dependerá de la fem inducida
de la siguiente forma:
ε
1 dΦ
B0 bẋ
I=
=−
=−
R
R dt
R

Problemas Propuestos y Resueltos de Electromagnetismo

BL
v(t) =
m

---

### Página 314

CAPÍTULO 15. LEY DE FARADAY-LENZ
Luego la fuerza que siente la barra es
ˆ
F~ =

ˆb
~ ×B
~ =−
I dl

B0 bẋ
(B0 b)2 ẋ
dy ŷ × B0 ẑ = −
x̂
R
R

Planteando la ecuación de movimiento de la barra se tiene que
mẍ = −

(B0 b)2 ẋ
dv
(B0 b)2 v
=⇒ m = −
R
dt
R

Resolviendo la ecuación diferencial
mR
−
(B0 b)2

ˆv(t)

dv
=
v

v0

ˆt

!

(B0 b)2
t
dt =⇒ v(t) = v0 exp −
mR

La posición que se detiene la barra está determinada por (asumiendo que comienza en el
origen)
!

dx
(B0 b)2
= v0 exp −
t =⇒
v(t) =
dt
mR

!
ˆt
ˆx(t)
(B0 b)2
dx = v0 exp −
t dt
mR

de modo que
!!

(B0 b)2
v0 mR
−
exp
−
t
x(t) =
(B0 b)2
mR
Por lo que finalmente la barra en t → ∞ se quedará en

Rodrigo Chi - Marzo 2017

xf inal =

v0 mR
(B0 b)2

b) En primera instancia, dado que hay una fuente de voltaje fija de valor V0 , existe una corriente
permanente
V0
I0 =
R
Donde se ha considerado positivo el sentido de la corriente antihoraria. La corriente I0
circula en la dirección positiva debido a la forma de como está conectada la fuente de
~ = B0 ẑ
voltaje. La fuerza que mueve a la barra está determinada por el campo magnético B
(saliendo de la hoja) y las corrientes que circulan por el circuito (corriente inducida y fija).
La corriente inducida dependerá de la fem inducida de la siguiente forma:
Iind =

ε
1 dΦ
B0 bẋ
=−
=−
R
R dt
R

Luego la fuerza que siente la barra es
ˆ
F~ =

ˆb
~ ×B
~ =
(Iind + I0 )dl

!

!

B0 bẋ ε0
(Bb)2 ẋ V0 Bb
−
+
dy ŷ × B0 ẑ = −
+
x̂
R
R
R
r

---

### Página 315

CAPÍTULO 15. LEY DE FARADAY-LENZ
Planteando la ecuación de movimiento de la barra se tiene que
(B0 b)2 ẋ V0 B0 b
dv (B0 b)2 v
V0 B0 b
mẍ = −
+
=⇒
+
=
R
R
dt
mR
mR
Resolviendo la ecuación diferencial con factor integrante
(B0 b)2 t
dv (B0 b)2 t (B0 b)2 v (B0 b)2 t
V0 B0 b (B0 b)2 t
d
e mR +
e mR =
e mR =⇒
v(t)e mR
dt
mR
mR
dt





=

V0 B0 b (B0 b)2 t
e mR
mR

Finalmente integrando a ambos lados (e imponiendo que la barra parte del reposo)

v(t)e

(B0 b)2 t
mR

ˆt
=

(B0 b)2
V0
V0 B0 b (B0 b)2 t
e mR dt =⇒ v(t) =
1 − e− mR t
mR
B0 b





P X

Solución 15.7

Al igual que el Problema 15.1, se tiene que el campo magnético dentro la bobina es
~
B(t)
= µ0 nI0 sin ωtẑ
¨ ~
¨
~
∂B
∂B ~
~
~
~
~
~
En este caso se aplica la ley de Maxwell ∇ × E = −
(∇ × E)dS = −
dS,
=⇒
∂t
∂t
Ω

Ω

Γ

Ω

~ = E(r, t)θ̂ (el campo eléctrico rota en torno a los campos magnéticos variables
Asumiendo que E
en el tiempo) y que Ω es un circulo de radio r con normal ẑ, se tiene que
¨
˛
∂
~
~ =⇒ E(r, t)·2πr = − ∂ (µ0 nI0 sin ωt·πr2 ) =⇒ E
~ dS
~ = − r µ0 nI0 ω cos ωtθ̂
~
E·dl = −
B·
∂t
∂t
Ω

Γ

~ , luego
Considerando que se trata de un material ohmnico, J~ = g E
gr
J~ = − µ0 nI0 ω cos ωtθ̂
Finalmente, la potencia que disipa el cilindro es
˚
P =
Cilindro

ˆh ˆ2π ˆa 
2
r
gπh(a2 µ0 I0 ω cos ωt)2
~
~
E · JdV =
g
µ0 nI0 ω cos ωt rdrdθdz =

Problemas Propuestos y Resueltos de Electromagnetismo

usando el teorema de Stokes con la última expresión
˛
¨
∂
~
~
~
~ · dS
E · dl = −
B
∂t

---

### Página 316

CAPÍTULO 15. LEY DE FARADAY-LENZ
Solución 15.10

P X

Para iniciar el problema hay que determinar el valor de la corriente inducida, la cual debe ir sentido
antihorario ya que se opone al aumento del flujo magnético. Esta corriente provoca una fuerza
magnética sobre la barra, la cual puede ser determinada como
ˆL
~ ×B
~ = −IBLx̂
I dl

F~m =

Luego, la derivada temporal del flujo que atraviesa por el circuito cerrado es
d
dΦ
=
dt
dt

ˆL ˆx
B(−ẑ) · dxdyẑ = −BLv

Usando la Ley de Voltajes de Kirchhoff, se tiene un circuito RC alimentado por un fem debida a
la inducción. De la parte anterior se sabe que
ε(t) = −

dΦ
= BLv
dt

Luego debe cumplirse que
ε = IR +

Q
= BLv
C

Derivando la ecuación anterior, se obtiene
BL

dv
d2 Q
1 dQ
=R 2 +
dt
dt
C dt

Usando el hecho que

Rodrigo Chi - Marzo 2017

IBL
BL dQ
dv
=−
=−
F~m = mv̇x̂ = −IBLx̂ =⇒
dt
m
m dt
Reemplazando y reordenando se obtiene que
!

d2 Q
(BL)2 dQ
+
+
=0
dt2
RC
mR
dt
|
{z
}
α
La solución de esa EDO es
Q(t) =

C1 −αt
e
+ C2 =⇒ I(t) = −C1 e−αt
α

Aplicando las condiciones iniciales Q(0) = CV0 e I(0) = VR0 se obtiene que C1 = − VR0 y C2 =
V0 (C + αR
). Finalmente, a partir de la ecuación obtenida en la parte anterior
Q(∞)
Q(∞)
V0
BLv(∞) = I(∞)R +
=⇒ v(∞) =
=
C+
C
BLC
BLC
αR




---

### Página 317

CAPÍTULO 15. LEY DE FARADAY-LENZ
Solución 15.12

P X

Dado que el disco esta girando con velocidad angular constante, todas sus cargas en su superficie
sienten una fuerza magnética (carga libre con velocidad bajo un campo magnético). El material
crea un campo eléctrico al interior de él, debido a que desea que todas sus cargas se queden en
el mismo lugar y anule la fuerza magnética que se está produciendo. Por lo tanto
~
~ = − Fm
E
q
~
= −~v × B
~
= −(~ω × ~r) × B
= −(Ωk̂ × rr̂) × B0 k̂
= −B0 Ωrr̂
Finalmente

ˆ
|ε| =

ˆR
~ =
~ · dl
E

B0 Ωrdr =

B0 ΩR2

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 318

CAPÍTULO 15. LEY DE FARADAY-LENZ

IV.

Indicaciones Problemas Sin Solución

Indicación 15.2

P X

Asuma que el carrito ha entrado una distancia x a la zona de campo. Determine la fuerza
que siente el carrito en función de la corriente inducida y luego plantee su ecuación de
movimiento. Con lo anterior, llegará a una EDO con respecto a la velocidad y con ello al
resultado final.
Con la presencia del condensador ahora ε 6= IR ya que hay que agregar el efecto del
condensador. Haciendo un Kirchhoff de voltaje, se cumple que ε = IR + Q
.
C
Usando la fuerza de Lorentz, determine la ecuación diferencial que cumple la velocidad y
con ello el valor pedido.
El Problema 15.10 puede ser muy útil para referencia de como enfrentar este problema.

Indicación 15.4

P X

Determine el campo eléctrico inducido en la zona donde se encuentra el anillo.
Utilizando ese valor, determine el torque ~τ = ~r × F~ que siente el anillo completo.
Utilizando el hecho que ~τ = I ω
~˙ , donde I es la inercia del disco, encuentre una ecuación
≈ ∆B
diferencial que describa la velocidad angular del disco. Puede ser útil recordar que dB
dt
∆t
∆ω
y que dω
≈
.
dt
∆t

Rodrigo Chi - Marzo 2017

Indicación 15.5

P X

~ uniforme, determine el cambio de su flujo entre el
Asumiendo un campo magnético B
instante inicial y final (ie. antes y después del giro).
Recordando que I = dQ
≈ ∆Q
y que por otro lado la corriente inducida vale I = − R1 dΦ
=
dt
∆t
dt
1 ∆Φ
− R ∆t es fácil concluir el problema.

Indicación 15.8

P X

Note que para resolver este problema es necesario determinar las otras componentes del
~ ·B
~ = 0, puede ser muy útil revisar el Problema
campo magnético. Para ello recuerde que ∇

---

### Página 319

CAPÍTULO 15. LEY DE FARADAY-LENZ
12.5.
Determine el flujo de campo magnético sobre la bobina y con ellos la corriente inducida. A
partir de ello, use la Fuerza de Lorentz para determinar el valor de la fuerza total que actúa
sobre la espira.
La velocidad terminal puede ser obtenida a partir de encontrar la ecuación de movimiento
de la espira o de un análisis energético. En el último caso, la energía total de la espira en
un instante t es la suma de su energía cinética más potencial gravitatoria. La derivada de
la energía en el tiempo es igual a P = −I 2 R que es la potencia que disipa la resistencia.
Concluya el problema imponiendo que en el infinito la aceleración es nula.

Indicación 15.9

P X

Tome un sistema de referencia adecuado para el problema, por ejemplo x creciendo hacia
abajo.
Determine la corriente inducida en el circuito, para ello determine el flujo sobre la parte de
la espira que ha caído en la zona de campo magnético y con ello la fem inducida.
Una vez determinada la corriente inducida, calcule la fuerza de Lorentz sobre el lado inferior
de la espira. Los lados verticales anulan su fuerza entre ellos.
Usando la ecuación de movimiento y la segunda ley de Newton, determine la ecuación
diferencial que cumple la espira. Puede ser útil recordar que en la velocidad terminal la
aceleración es nula ya es nula.
P X

Usando Ley de Ampère, determine el campo magnético que sentirá la barra.
Conocido el campo magnético y la velocidad de barra (dato), determine el campo eléctrico
en los puntos sobre la barra. Integre el resultado anterior y concluya.
Puede ser útil la aproximación ln(1 + x) ≈ x cuando x
1.

Indicación 15.13

P X

Determine la velocidad de los portadores, para ello recuerde que I es dato y que J~ = ρ0~v .
Conocida la velocidad de los portadores, determine el campo eléctrico que aparece dentro
del cable e intégrelo entre las caras transversales para hallar la diferencia de potencial.

Problemas Propuestos y Resueltos de Electromagnetismo

Indicación 15.11

---

### Página 320

CAPÍTULO 15. LEY DE FARADAY-LENZ

V.

Resultados
Problema

Respuestas
~ = µ0 mI0 sin(ωt)ẑ
a) B

P

15.1

~ t) = − rµ0 mI0 ω cos(ωt) θ̂
b) E(r,

~ t) = − b µ0 mI0 ω cos(ωt) θ̂
c) E(r,
2r

P

15.2



a) v(t) = v0 exp − (aB)
mR t
h
i

2 2
a τ
0τ
, Q(t) = Bav
b) v(t) = v0 1 − BmR
1 − exp − τt
1 − exp − τt , donde τ1 =
R
B 2 a2
RC + mR

P

15.3

B L bt
v(t) = BLbt
2m ε(t) =
2m

Rodrigo Chi - Marzo 2017

P

15.4

P

15.5

B
a) ωf = λRπa
I

b) Es independiente de B(t), solamente importa el valor inicial y final.

P

15.6

P

15.7

2QR
B = πN
D2



v0 mR
0 b)
a) v(t) = v0 exp − (BmR
t xmax = (B
0 b)


(B0 b)2
b) v(t) = BV00b 1 − e− mR t

P = gπh(a µ0 I80 ω cos ωt) , Prop. I = − gha
4 µ0 nI0 ω cos ωt
a) Antihorario (considerando normal positiva +ẑ)

P

15.8

b) I = − Cπa
R ż
c) F~r = 0, F~z = πa2 CI ẑ
mgR
d) vT = (Cπa
2 )2

---

### Página 321

CAPÍTULO 15. LEY DE FARADAY-LENZ
Problema

Respuestas

P

15.9

mRg
vT = B
2 a2 , el sentido de la corriente en la figura es antihorario.

P

15.10


V0
v(∞) = BLC
C + αR
con α = RC
+ (BL)
mR

P

15.11


0 vI
0 vId
|∆V | = µ2π
ln 1 + ad , si a
d entonces |∆V | ≈ µ2πa

P

15.12

|ε| = B0 ΩR

P

15.13

IB
∆V = ne`

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 322

Rodrigo Chi - Marzo 2017

CAPÍTULO 15. LEY DE FARADAY-LENZ

---

### Página 323

Inductancia y Energía Magnética

I.

Resumen Teórico

Inductancia Mutua
Sean dos circuitos Γ1 y Γ2 , los cuales circula una corriente I1 e I2 , respectivamente. Sea Φ1→2 el
flujo magnético que genera el circuito Γ1 sobre Γ2 y Φ2→1 el flujo que genera el circuito Γ2 sobre
Γ1 . Luego, se define la inducción mutua M como
M=

Φ2→1
Φ1→2
=
I1
I1

(16.1)

Nótese el hecho que la inducción mutua es simétrica. A partir de lo anterior, si I1 = I1 (t) existirá
una fem inducida en el circuito Γ2 dada por
dΦ1→2
dI1
= −M
dt
dt

(16.2)

Inductancia Propia
Sea un circuito Γ1 por el cual circula una corriente I1 y sea Φ2→1 el flujo de campo magnético que
genera el circuito sobre si mismo. Se define la inductancia propia de ese circuito o autoinductancia
L como
Φ1→1
L=
(16.3)
I1
La fem autoinducida en un circuito debido a su corriente está dada por
ε1 = −

dΦ1→1
dI1
= −L
dt
dt

(16.4)

En presencia de otro otro circuito Γ2 con una corriente I2 , la fem total inducida en el circuito es
ε1 = −M

dI2
dI1
−L
dt
dt

(16.5)

Problemas Propuestos y Resueltos de Electromagnetismo

ε2 = −

---

### Página 324

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA

Energía Magnética
La energía magnética de un circuito está dada por
˚
~ · HdV
~
U=
B

(16.6)

Todo el
Espacio

Por otro lado, también puede ser determinada en forma equivalente en función de la inductancia
L, el flujo Φ y la corriente I como
Φ2
U = LI 2 = ΦI =
2L

(16.7)

Recomendaciones
Tanto la inductancia propia como mutua dependen netamente de la geometría del problema.

Rodrigo Chi - Marzo 2017

Es interesante notar que la inductancia es análoga a la capacitancia. Mientras que en una
capacitancia la carga no puede variar abruptamente, la corriente no puede hacerlo en una
inductancia.

---

### Página 325

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA

II.

Problemas Propuestos

#### Problema 16.1

X I

Encuentre el coeficiente de inductancia mutua entre
un alambre infinitamente largo y un triángulo isósceles
de altura h dispuestos como se muestra en la Figura.

a

h

z

#### Problema 16.2

b

X S

Considere dos espiras de radios a y b (a
b) dispuesta de forma que sus centros se ubican en el eje z
separadas por una distancia d, como se muestra en la
Figura. Encuentre el coeficiente de inducción mutua
del sistema.

#### Problema 16.3

X S

d

a

I

#### Problema 16.4

a

2a

I

X S

Considere una bobina muy larga de radio a y n vueltas
por unidad de largo. Al interior de la bobina, existe un
espira de radio b que forma un ángulo α con respecto
al eje de la bobina.
a) Determine la inductancia mutua entre la bobina
y la espira.
b) Si por la espira empieza a circular un corriente
I(t) = I0 sin(ωt), ¿cuál es la máxima diferencia
de potencial en los terminales de la bobina?.

b

a

a

Problemas Propuestos y Resueltos de Electromagnetismo

Dos cables infinitos llevan una corriente I y están separados una distancia 2a como se muestra en la Figura. Un anillo circular conductor de radio a yace en
el mismo plano entre entre los dos cables totalmente
aislados de ellos. Encontrar el coeficiente de inductancia mutua entre los cables y el anillo circular. Puede
x
= √1−x
ser útil d arcsin
2.
dx

---

### Página 326

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
#### Problema 16.5

X S

Dos alambres infinitos están separados una distancia d
y llevan una corriente eléctrica I en direcciones opuestas (ver Figura). La corriente I incrementa a una tasa
dI/dt suficientemente baja de tal manera que la ley
de Ampere se cumple. Una espira cuadrada de lado
d se encuentra dispuesta en el mismo plano de los
alambres, tal como se muestra en la Figura.

d
d

a) Calcule la inductancia mutua entre la espira y
los alambres.

d

b) Indique la dirección de la corriente inducida en
la espira cuando dI/dt es positivo. Justifique su
respuesta.

d

I

I

c) Sabiendo que la resistencia de la espira es r, calcule la fuerza que actúa sobre la espira (magnitud y dirección).
#### Problema 16.6

X S

a

Un cable coaxial está formado por dos superficies
cilíndricas infinitamente largas, por las cuales circula una misma corriente en sentidos contrarios. Si las
densidades superficiales de corriente que circulan por
las superficies cilíndricas de radios a y b son, respectivamente:
~ a = I0 ẑ
K
2πa

~ b = − I0 ẑ
K
2πb

b

z

~b
K

~a
K

Rodrigo Chi - Marzo 2017

. Determine:
a) La energía por unidad de largo.
b) La autoinductancia por unidad de largo del cable
coaxial.
#### Problema 16.7

~ (t)
w

X S

Un cilindro de radio R y largo H
R, posee una
densidad de carga σ0 con su eje coincidente al eje
z. En t = 0 el cilindro comienza a rotar lentamente
con velocidad angular ω
~ (t) = αtẑ, donde α es una
constante. Determine la energía eléctrica y magnética
dentro del cilindro

s0

R

H

---

### Página 327

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
#### Problema 16.8

X I

Considere toroide de sección transversal rectangular
de N vueltas, de radio interior a y exterior b, y altura
h.

N

a) Determine la autoinductancia de este toroide.

h

b) Demuestre que si b − a
a entonces la autoinductancia del toroide puede ser aproximada
como
µ0 N 2 h(b − a)
L=
2πa

#### Problema 16.9

a

X I

z

Considere inicialmente una espira circular de radio a
que yace sobre el plano xz. En t = 0 la espira comienza a girar con una velocidad angular ω
~ = ω0 ẑ. Si en
el espacio existe un campo homogéneo y constante de
~ = B0 ŷ determine:
valor B

b

~
w
~B

a

a) La fem inducida en el circuito.

y

b) La corriente en función del tiempo que circula
por la espira, si la espira posee una resistencia
R y una autoinducción L.

x

#### Problema 16.10

X I

Un carrito de masa m que se desplaza con velocidad
v0 x̂, hasta llegar a una región en que existe un campo
magnético uniforme en x = 0. El carrito es perfectamente conductor (ie. resistencia nula) y posee una
autoinductancia L. Determine la velocidad del carrito en el tiempo y la corriente que circula por éste.
¿Cuál debe ser la condición sobre el largo del carrito
para que éste logre entrar completamente a la zona
de campo?.

y

~B = B0 ẑ

~v = v0 x̂
L
a

x

Problemas Propuestos y Resueltos de Electromagnetismo

c) El torque que siente la espira, suponiendo que
ésta ha estado rotando un tiempo muy largo.

---

### Página 328

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
#### Problema 16.11

X I

a) Instantáneamente una vez que el interruptor es
cerrado.

R1
I1

I2

I3

R2

L

+

Considere que interruptor S del circuito mostrado en
la Figura, ha estado abierto un tiempo muy largo.
Determine las corrientes I1 , I2 e I3 que se muestran
en la figura, cuando:

V0
S

b) Un largo tiempo después que el interruptor es
cerrado.

#### Problema 16.12

X S

I(t)

+

En el circuito de la Figura se ha tenido conectada la
batería por mucho tiempo (desde t = −∞) con el
interruptor S abierto. Luego en t = 0 el interruptor se
cierra. Considere que V0 = 120 V, R1 = R2 = 30Ω y
L = 50 mH.

R1

V0

a) Determine por inspección la corriente I en t = 0
(“justo” antes de cerrar S) y en t = ∞ (“mucho” después de haber cerrado S) .
b) Obtenga una expresión analítica para I(t), entre
0 ≤ t < ∞ . Grafique su resultado.

Rodrigo Chi - Marzo 2017

#### Problema 16.13

R2
S

L

X I

Se debe determinar los valores de L y C en un circuito
RLC en serie cuando se conoce R. Para ello se carga
el condensador con una carga Q0 y se cierra el circuito
observándose que la corriente partiendo de cero, oscila
con una frecuencia angular ω0 y amplitud decreciente.
Si al circuito se le reemplaza la resistencia R por otra
de magnitud 2R, éste queda justo en el límite cuando
ya no oscila.
a) Determine los valores de L y C.
b) Escriba la función Q(t) en función de t.
En ambos casos sus resultados deben quedar expresados a lo más en función de los datos R, Q0 y ω0 .

L

R

C

---

### Página 329

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
Disco Conductor

µ0 , g

`

a

#### Problema 16.14

b

X I

µ

Un toroide de material magnéticamente lineal de permeabilidad µ, de sección circular de radio R, tiene un
radio interior a y exterior b. El toroide tiene un entrehierro de longitud e, que está ocupado por un disco
conductor de radio R y conductividad g. Si al enrollado de N vueltas se le da una corriente I(t). ¿Cuánta
potencia disipará el disco?.

N
I(t)

`
R
g
Disco Conductor

X I

Considere un toroide de permeabilidad µ de sección
cuadrada a2 y de largo 8a. El toroide cuenta con dos
entrehierros de una longitud muy pequeña g tal como
y se muestra en la Figura. En uno de sus extremos el
toroide posee un enrollado de N vueltas, el cual está
conectado una fuente de corriente I0 . Determine

g

I0

µ

a

N

6a

a) El flujo magnético y la autoinductancia del sistema.
b) Si el lado izquierdo con forma es U es fijo, la
fuerza que siente el material de la derecha.

a
a

6a

a

Problemas Propuestos y Resueltos de Electromagnetismo

#### Problema 16.15

---

### Página 330

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA

III.

Soluciones

Solución 16.2

P X

Dado que una espira es mucho más pequeña otra, se supondrá que el campo magnético que pasa
~ = d), donde B
~ es el campo
a través de la espira de radio b es aproximadamente igual a B(z
magnético que genera la espira de radio a. Usando la definición de campo magnético

~ = d) = µ0
B(z
4π
µ0
=
4π

ˆ
ˆ2π

~ × (~r − ~r 0 )
I dl
|~r − ~r 0 |3
I1 · adθθ̂ × (dẑ − ar̂)
|~r − ~r 0 |3

µ0 I1 a
=
4π

ˆ2π

dθθ̂ × (dẑ − ar̂)
|dẑ − ar̂|3

ˆ2π

ˆ2π



=

=

µ0 I1 a2
4π

Rodrigo Chi - Marzo 2017

(d2 + a2 )

ˆ2π

+

a · dθẑ 
3 
(d2 + a2 ) 2

dθẑ

=

d · dθr̂

µ0 I1 a 

4π



(d2 + a2 ) 2

µ0 I1 a

3 ẑ
2(d2 + a2 ) 2
Por lo tanto el el flujo en la espira de radio b está dado por
¨
~ = πb2 · µ0 I1 a 3
~ · dS
Φ2 =
B
2(d2 + a2 ) 2

Por lo que la inductancia mutua está dada por
M=

Solución 16.3

Φ2
µ0 π(ab)2
=
I1
2(d2 + a2 ) 2

P X

~ = µ0 I θ̂, entonces
Sabiendo que el campo producido por un alambre infinito con corriente I vale B
2πr
a una distancia r de uno de los dos cables se tiene que el campo magnético total es:
~ = µ0 I ẑ
B
2π



+
r 2a − r



---

### Página 331

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
Donde ẑ es el vector unitario que entra a la hoja, perpendicular a ella. De esta manera, se calcula
el flujo magnético, teniendo en cuenta que r = a + x donde x es la coordenada vertical en la
figura, e y es la coordenada horizontal, con el origen ubicado al centro del anillo.
ˆ
Φ=

ˆ ˆ
~ · dS
~=
B

Luego:
µ0 I
Φ=
2π

ˆa 

µ0 I
2π



µ0 I
+
dydx =
r 2a − r
2π


ˆa

√

a2 −x2 
ˆ

√
−a − a2 −x2

√
2a
2µ0 Ia
a2 − x2 )dx =
(2a
a −x
π


−a

ˆa
√
−a

+
dydx
a+x a−x

dx
a2 − x 2



= 2µ0 Ia

Y recordando la relación de inducción mutua Φ = M I, finalmente resulta:
M = 2µ0 a

Solución 16.4

P X

a) Para determinar la inducción mutua, se supone en primera instancia una corriente I1 que
pasa por la bobina y una corriente nula en la espira. Luego, es necesario determinar el flujo
Φ1→2 que genera el campo magnético de la bobina sobre la espira. El campo magnético que
genera la bobina dentro de ella es
~ = µ0 nI1 ẑ
B
y la normal de la espira (dado que está rotada con respecto al eje de la bobina) es

Por lo tanto el flujo es
¨
Φ1→2 =

ˆ2π ˆb
~ =
~ · dS
B

µ0 nI1 ẑ · rdrdθ(cos αŷ + sin αẑ) = µ0 nI1 πb2 sin α

Luego la inducción mutua es
M=

Φ1→2
= µ0 nπb2 sin α
I1

2→1
b) La fem inducida en la bobina estará dado por ε = − dΦdt
. Donde Φ2→1 es el flujo de la
espira sobre la bobina. A priori, parece complicado determinar el valor del flujo Φ2→1 , sin
embargo es posible utilizar el calculo anterior, ya que por simetría de la inductancia mutua

M=

Φ1→2
Φ2→1
=
=⇒ Φ2→1 = M I2
I1
I2

Problemas Propuestos y Resueltos de Electromagnetismo

n̂ = cos αŷ + sin αẑ

---

### Página 332

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
y

n̂
a
z

~B

Figura 16.1: Representación normal espira y campo magnético.
Utilizando el hecho que I2 (t) = I0 sin ωt, se obtiene que
dI2
dΦ2→1
= −M
= −µ0 nπb2 sin α · I0 ω cos ωt
dt
dt
Finalmente, el máximo valor que alcanza la fem en la bobina (o equivalentemente, la diferencia de potencial en sus terminales) es en t = ωπ
ε=−

∆Vmax = µ0 nI0 ωπb2 sin α

Solución 16.5

P X

a) El campo magnético que genera cualquier alambre con corriente I es
˛
~ = µ0 I
~ · dl
B

Rodrigo Chi - Marzo 2017

B(r) · 2πr = µ0 I
µ0 I
~
B(r)
=
θ̂
2πr
Extrapolando ese resultado al problema, y considerando que el sistema de referencia está
ubicado con el alambre inferior y = 0
µ0 I
~ tot = B
~ cable1 + B
~ cable2 = µ0 I ẑ +
B
(−ẑ)
2πy
2π(y − d)
Luego

¨

ˆd ˆ3d
~ =
~ tot · dS
B

!

µ0 I
ẑ
−
· dxdyẑ
2π
y y−d

0 2d

µ0 I
=
d ln
− ln(2)
2π
 
µ0 I
=
d ln
2π


Finalmente como

 



|Φ|
µ0 d
M=
=
ln
I
2π

 

---

### Página 333

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
0I
b) Usando la Ley de Lenz y los resultados de la parte anterior Φ = µ2π
d ln
Luego
  
dI
µ0 I
dΦ
=−
d ln
>0
ε=−
dt
dt
{z 4 } |{z}
|2π

 

< 0.

>0

<0

Como ε > 0, la corriente va en el sentido positivo de la normal ẑ (antihorario).
c) Como la resistencia de espira es r, la corriente que ciercula por ella es
ε
µ0 d
3 dI
=−
ln
r
2πr
4 dt
 

I1 =

La fuerza puede calcularse en los cuatro lados de la espira.
Para los lados verticales la fuerza es simétrica, igual en módulo pero en sentidos contrarios,
por ende se anulan.
Por otro lado
~ ×B
~ tot (y = 2d) = I1 dxx̂ × µ0 I
dF1 = I1 dl
2π

−
y y−d

!

ẑ =
y=2d

µ0 II1
2π



−
dx(−ŷ)
2d d


Integrando en x entre 0 y d,
µ0 II1
ŷ
4π
Análogamente para la sección horizontal del cable superior, usando y = 3d
=⇒ F~1 =

~ ×B
~ tot (y = 3d) = µ0 II1
dF3 = I1 dl
2π



−
dx(−ŷ)
3d 2d


µ0 II1
µ0 I µ0 d
3 dI
ŷ = −
ln
ŷ
F~tot =
6π
6π 2πr
4 dt
 

Solución 16.6

P X

Existen dos maneras de resolverlo, mediante la energía magnética o mediante el flujo magnético:
i) Energía magnética: Primero que todo, se calcula el campo magnético en el espacio mediante
Ley de Ampére en una superficie circular de radio r, perpendicular a los dos cascarones
cilíndricos. De esta manera, para a < r < b:
ˆ
~
~ · d~l = 2πrB = µ0 I
B = B(r)θ̂ =⇒ B

Problemas Propuestos y Resueltos de Electromagnetismo

µ0 II1
ŷ
12π
Finalmente la fuerza está dada por la suma de F~1 + F~3
=⇒ F~3 = −

---

### Página 334

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
Luego, la corriente que atraviesa dicho camino es:
ˆ
~ a × n̂) · d~l
I = (K
Donde n̂ = r̂ es el vector normal a la superficie cilíndrica de radio a (superficie a través de
la cuál circula la corriente enlazada), y d~l = rdθθ̂. Por lo tanto:
ˆ2π
I=

I0
~ < r < b) = µ0 I0 θ̂
adθ = I0 =⇒ B(a
2πa
2πr

~ < a) = 0 debido a que no hay corrientes enlazadas
Además, se debe tener claro que B(r
~ > b) = 0 debido a que la suma de corrientes enlazadas es nula para
para r < a; y B(r
r > b.
Ahora, se calcula la energía magnética asociada a una altura h arbitraria en los cilindros:
Um =
2µ0

˚

ˆh ˆ2π ˆb
~ 2

|B| dV =

µ20 I02
µ0 I02 h
b
rdθdrdz
=
ln
4π 2 r2
4π
a

!

a

Así, se obtiene la energía por unidad de largo:
Um
µ0 I02
b
um =
=
ln
h
4π
a

!

Para calcular la autoinductancia por unidad de largo, se debe recordar que la energía
magnética asociada a una autoinductancia es (recordar que en este caso I = I0 ):
µ0 I02 h
LI 2
b
ln
Um = 0 =
4π
a

!

µ0 h
b
=⇒ L =
ln
2π
a

!

Rodrigo Chi - Marzo 2017

Por lo tanto, la autoinductancia por unidad de largo vale:
L
µ0
b
l= =
ln
h
2π
a

!

ii) Flujo magnético: Usando los resultados anteriores del campo magnético, se calcula el flujo
~ de lado (b − a)
magnético a través de una superficie rectangular, perpendicular al campo B,
y altura h:
!
ˆ
ˆb ˆh
µ
I
µ
I
b
~ · dS
~=
Φ= B
drdz =
ln
2πr
2π
a
a

Recordando que:
µ0 h
b
Φ = LI0 =⇒ L =
ln
2π
a

!

µ0
b
=⇒ l =
ln
2π
a

!

---

### Página 335

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
Solución 16.7

P X

~
Dado que la carga comienza a rotar, se genera una densidad superficial de corriente K(t)
=
σ0 ω(t)Rθ̂. Este problema es análogo al de una bobina con una corriente circulando por ella, por
ende el campo magnético fuera del cilindro es nulo. A partir de eso se obtiene por ley de Ampère:
˛
~ = µ0 I =⇒ B · H = µ0 KH =⇒ B
~ · dl
~ = µ0 σ0 αtRẑ
B
El camino elegido es el mismo que se usa en bobina, un rectángulo de altura H. Luego, usando
la ley de Faraday para un disco de radio r < R
¨
˛
µ0 σ0 αRr
d
~ =⇒ E(r, t) · 2πr = − d (πr2 · µ0 σ0 αtR) =⇒ E(r)
~
~
~ · dS
~
=
θ̂
B
E · dl = −
dt
dt
El campo eléctrico cambia debido a la inducción que provoca el campo magnético en el tiempo.
Finalmente, la energía magnética es
Um =
2µ0

˚

~ 2 dV = 1
|B|
2µ0

ˆH ˆ2π ˆR
(µ0 σ0 αtR)2 rdrdθdz =

µ0 (σ0 αtR)2 · πR2 H

y la energía eléctrica es
ε0
Ue =

˚

ε0
|E| dV =
~ 2

ˆH ˆ2π ˆR 

2

rdrdθdz =

ε0 (µ0 σ0 αR)2
R4
· πH ·

P X

a) Para t = 0, el interruptor S ha estado abierto mucho tiempo, por cual la corriente que
circula en el circuito se vuelve constante (la inductancia en un tiempo muy extenso actúa
como un cortocircuto, es decir, como un simple cable). Por ende la corriente está dada por
I(t = 0) =

V0
= 4 [A].
R2

Para el caso que t → ∞, el interruptor se cierra y quedan las dos resistencias en paralelo.
Al igual que el caso anterior se tiene la corriente es
I(t → ∞) = V0



+
R1 R2



= 8 [A].

b) Usando un Kirchoff de Voltajes, se obtiene
V0 = IR + L

dI
dI R
V0
=⇒
+ I=
dt
dt
L
L

Problemas Propuestos y Resueltos de Electromagnetismo

Solución 16.12

µ0 σ0 αRr

---

### Página 336

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
Donde R = (R1−1 + R2−1 )−1 = 15 Ω. Usando factor integrante (ie. multiplicar a ambos
R
lados e L t )

R
R
dI R t R R t V0 R t
d
V0 R
V0 R
e L + Ie L = e L =⇒ (I(t)e L t ) = e L t =⇒ I(t)e L t − I(0) = (e L t − 1)
dt
L
L
dt
L
R

Reemplazando los valores de R e I(0), se obtiene que
I(t) =

R
V0 − R t V0
e L + (1 − e L t ) = 8 − 4e−300t
R2
R

I(t)

t

Rodrigo Chi - Marzo 2017

Figura 16.2: Gráfico de I(t)

---

### Página 337

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA

IV.

Indicaciones Problemas Sin Solución

Indicación 16.1

P X

Divida el flujo en dos triángulos rectángulos más pequeños, los cuales quedan definidos a
partir de la altura del triángulo isósceles. Por simetría ambos flujos son iguales.
Note que al integrar el triángulo rectángulo definido por la altura se cumple que z(r) =
r tan α.

Indicación 16.8

P X

Determine el campo magnético que existe dentro del toroide suponiendo que por este circula
una corriente I, para ello use la ley de Ampère tomando un camino circunferencial de radio
r entre a y b.
Una vez determinado el campo magnético, determine el flujo sobre todo el toroide. Recuerde
que el flujo total sobre el toroide es N veces el que cruza una sección transversal. La
autoinductancia es directa a partir de lo anterior.
Para la segunda parte puede ser útil la relación la aproximación ln(1 + x) ≈ x cuando
x
1.

P X

Para determinar la fem inducida en el circuito determine el valor de la normal de la espira
circular. Note que la espira rota con respecto al eje z , por lo cual su normal vale n̂(t) =
−x̂ sin ω0 t + ŷ cos ωt (demuéstrelo).
~ = dS n̂ = rdrdθ(−x̂ sin ω0 t + ŷ cos ωt)
Determine el flujo recordando que dS
Para determinar la corriente en el tiempo es necesario considerar el efecto de la inductancia
L y la resistencia R. Haga un Kirchhoff del voltajes para encontrar una ecuación diferencial
˙ Resuélvala.
con respecto a al corriente, la cual debería ser de la forma ε(t) = RI + LI.
Si la espira ha estado rotando entonces los términos de la forma e−αt =⇒ 0. Considerando
eso, estime el valor de la corriente la cual circula por la espira y determine el torque a partir
del momento magnético de la espira.

Problemas Propuestos y Resueltos de Electromagnetismo

Indicación 16.9

---

### Página 338

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
Indicación 16.10

P X

Determine la fem inducida en el carrito suponiendo que este a penetrado una distancia x
˙
en la zona de campo magnético. Por Kirchhoff debe cumplirse que ε(t) = LI.
Por otro lado, determine la fuerza que siente el carrito debido a la corriente I que circula
por ella y encuentre la ecuación de movimiento del carrito en función de la velocidad.
Las dos ecuaciones anteriores forman un sistema de ecuaciones diferenciales, donde las dos
incógnitas a resolver son la velocidad y la corriente. Encuentre las condiciones iniciales y
resuélvalo.
Una vez encontrada la velocidad, determine la posición en el tiempo del carrito. El movimiento debería ser oscilatorio ya que no existen perdidas de energía en el carrito. Determine
cual es la máxima penetración que puede tener el carrito antes que se devuelva y deduzca
la condición pedida.

Indicación 16.11

P X

Para este problema no es necesario hacer ningún cálculo. Recuerde que la corriente no puede
ser discontinua en una inductancia (ie. no pueden existir variaciones abruptas de ella).

Indicación 16.13

P X

Rodrigo Chi - Marzo 2017

Mediante la aplicación de la ley Kirchhoff de voltaje, establezca las ecuación que sigue
el circuito RLC con respecto a su carga Q. Ésta debería ser una ecuación diferencial de
segundo orden.
El circuito se encuentra subamortiguado inicialmente debido a que se encuentra oscilando
con una amplitud decreciente. Si el circuito ya no oscila al cambiar la resistencia, significa
que su régimen ahora es de críticamente amortiguado.
Establezca las soluciones de cada caso y relacione los valores de L y C con los de R y ω0 .

Indicación 16.14

P X

Determine el campo magnético dentro del disco conductor. Para ello debe usar la ley de
Ampère previamente en el toroide.
~ tiene una dependencia temporal, éste inducirá un campo eléctrico.
Como B

---

### Página 339

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
Dada la conductividad asociada del disco, se provocará una densidad corriente en el cilindro.
~ y J~ es suficiente para determinar la potencia.
Conocido E

Indicación 16.15

P X

Plantee el toroide como un circuito magnético con reluctancias. Utilizando eso, determine
el flujo que circula por el toroide y luego la autoinductancia.
Conocido el flujo y la autoinductancia determine la energía del sistema. Recuerde que la
fuerza es posible de determinar mediante F~ = −∇U donde U es la energía.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 340

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA

V.

Resultados
Problema

Respuestas

P

16.1

M = µ0 h πtan α

P

16.2

M=

P

16.3

M = 2µ0 a

P

16.4

µ0 π(ab)2

2(d2 +a2 ) 2

a) M = µ0 nπb2 sin α
b) ∆Vmax = µ0 nπb2 ωI0 sin α
µ0 d ln(4/3)
a) M = |Φ|
I =
2π

P

16.5

P

16.6

P

16.7

P

16.8

b) Antihorario en la figura.

3 dI
0 I µ0 d
c) F~tot = − µ6π
2πr ln 4 dt ŷ

a) um =

µ0 I02
4π ln

µ0
b) l = 2π
ln

b
a

b
a





N h
ln
a) L = µ02π

b
a

Um = µ0 (σ0 αt)2 R πH Ue = ε0 (µ0 α)16 R Hπ



Rodrigo Chi - Marzo 2017

a) ε = −πa2 B0 ω0 sin(ω0 t)

P

16.9

R

B0
−Lt
b) I(t) = Rωπa
))
2 +ω 2 L2 (R sin ω0 t − ω0 L(cos ω0 t − e

ωπ 2 a4 B 2

c) τ (t) = R2 +ω2 L02 (R sin ω0 t − ω0 L cos ω0 t) sin ω0 t

---

### Página 341

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA
Problema

P

16.10

P

16.11

P

16.12

Respuestas
t, i(t) = − √mv
sin √aB
t. El largo del carrito debe ser menor a
v(t) = v0 cos √aB
mL
mL
mL

v0

√

mL
para que logre entrar.
aB

a) I3 = 0 (la corriente no puede aumentar en forma abrupta en una inductancia),
I1 = I2 = R1V+R
V0
b) I1 = I3 = R
, I2 = 0 (la inductancia actúa como un cortocircuito en un tiempo
muy largo).

a) I(0) = 4 A. e I(∞) = 8 A.
b) I(t) = 8 − 4e−300t A.
√

a) L = 2ω3R
, C = 2ω√03R

P

16.13

P

16.14

R
b) Q(t) = Ae−γt cos(ω 0 t + φ) con γ = 2L
, ω0 =
γ
tan φ = − ω0

P

16.15

q

Q0
R 2
1 2
−( 2L
) + ( LC
) , A = cos
φ y

N I0 µµ0 a
N µµ0 a
a) Φ = 32aµ
, L = 32aµ
0 +2gµ
0 +2gµ
2 2

N I µ µ0 a
b) |F~ | = (32aµ00 +2gµ)
2 la fuerza es atractiva.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 342

Rodrigo Chi - Marzo 2017

CAPÍTULO 16. INDUCTANCIA Y ENERGÍA MAGNÉTICA

---

### Página 343

Corriente Alterna

I.

Resumen Teórico

Corriente Alterna
Los circuitos de corriente alterna son circuitos alimentados por una fuente de voltaje de la forma
V (t) = V0 cos(ωt − φ)

(17.1)

donde V0 es amplitud de la señal, ω su frecuencia angular y φ su fase. En general, para enfrentar
problemas de este tipo se utiliza la técnica de fasores, es decir
V (t) = Re{V0 ejωt }

V (t) = V0 ejωt

(17.3)

Impedancias
La impedancia es la resistencia aparente (compleja) que tiene un circuito alimentando por una
fuente de voltaje alterna. Se define entonces
ZR = R
jωC
ZL = jωL

ZC =

(17.4)
(17.5)
(17.6)

Donde ZR , ZC y ZL son las impedancias de una resistencia, un condensador y un inductor,
respectivamente.

En Ingeniería Eléctrica no se suele la notación i =
se denotará j como la unidad compleja.

√

−1 para evitar confusión con la corriente i. En este libro

Problemas Propuestos y Resueltos de Electromagnetismo

(17.2)
√ 1
donde se expresa la tensión de la fuente como una exponencial compleja donde j = −1 .
Adicionalmente, se suele tomar como referencia la fuente de voltaje de modo que φ = 0. Como
notación, se suele obviar el hecho que se trabaja sólo con la parte real, por lo cual

---

### Página 344

CAPÍTULO 17. CORRIENTE ALTERNA

Potencia
La potencia instantánea de un circuito con una fuente de voltaje V (t) que entrega una corriente
I(t) está dada por
P (t) = V (t)I(t)
(17.7)
Por interés práctico, es útil conocer el valor de la potencia promedio que emite
hP (t)i =
T

ˆT
P (t)dt

(17.8)

donde T = 2π
. En caso de usar fasores, con V (t) = V0 ejωt y I(t) = I0 ej(ωt−φ) la potencia
ω
promedio puede ser determinada en forma equivalente como
hP (t)i =

Re{V (t)I ∗ } = V0 I0 cos φ

(17.9)

Donde I ∗ es el conjugado de I. A partir de lo anterior, se define el valor rms (“Root Mean
Square”) o efectivo de una señal como
V0
Vrms (t) = √

(17.10)

hP (t)i = Vrms Irms cos φ

(17.11)

de modo que

Rodrigo Chi - Marzo 2017

Frecuencia de Resonancia
La frecuencia de resonancia ω0 de un circuito eléctrico es aquella frecuencia la cual anula la parte
imaginaria de la impendancia equivalente de un circuito eléctrico. En esta frecuencia ocurre
La máxima corriente que circula por el circuito.
La máxima potencia promedio.

Recomendaciones
El uso de fasores en la notación de circuitos de corriente alterna facilita su desarrollo. Los
condensadores y inductores pueden ser vistos como = resistencias complejas” iguales a su
impedancia.

---

### Página 345

CAPÍTULO 17. CORRIENTE ALTERNA
Recuerde que a pesar de trabajar con números complejos, el resultado que tiene sentido
físico es la parte real del resultado complejo.
Distinga entre la tensión peak-to-peak y la rms. En general, los artefactos eléctricos hacen
referencia a su
√ consumo promedio y tensión en rms. En Chile la tensión máxima no son 220
V , sino 220 2 V.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 346

CAPÍTULO 17. CORRIENTE ALTERNA

II.

Problemas Propuestos

#### Problema 17.1

X I

Considere el circuito de corriente alterna mostrado en
la Figura. El circuito es alimentado con un generador
de voltaje V (t) = V0 cos ωt.

C

a) Demuestre que el módulo de la diferencia de potencial entre los puntos A y B es independiente V0
de la frecuencia ω del generador.

A

R
B

R

C

b) Calcule la fase de esta diferencia de potencial
con respecto al generador.
c) Explique cualitativamente como cambiarían sus
resultados si el generador tuviese una resistencia
interna Rint = R/10.

#### Problema 17.2

X I

Un circuito RLC serie tiene R = 100 Ω, L = 10 mH
y una frecuencia de resonancia de ω0 = 3 kHz.

R

a) ¿Cuál es el valor de C?
b) ¿Cuál es valor de la impedancia total cuando la
frecuencia es de ω 0 = 5 kHz?

V (t)

L

Rodrigo Chi - Marzo 2017

c) ¿Cuál es la corriente de respuesta a un voltaje
V (t) = 200 cos(104 πt)?
d) ¿Cuál es la potencia promedio consumida?
e) ¿Cuál es el máximo voltaje en cada uno de
los tres elementos de circuito? ¿Por qué estos
números no suman 200 [V]?

C

---

### Página 347

CAPÍTULO 17. CORRIENTE ALTERNA
#### Problema 17.3

X S

Considere el circuito eléctrico de la figura, que es alimentado por una fuente de voltaje alterno V (t) =
V0 cos ωt. Determine:

R

a) La impedancia equivalente de la configuración,
especificando claramente su parte real e imaginaria.

L

b) La frecuencia de resonancia ω0 del circuito, tal V0
que haga máxima la corriente que sale de la
fuente.

C2
C1

c) La corriente que circula por la resistencia R en
función del tiempo (ie. escriba la corriente de
la forma I(t) = I0 cos (ωt − φ), especificando
claramente los valores de I0 y φ).
d) La potencia promedio entregada por la fuente.
#### Problema 17.4

X I

#### Problema 17.5

[220 V]
[110 W]

[220 V]
[1100 W]

E

X S

Un circuito tiene dos resistencias R1 y R2 , un condensador C y una inductancia L dispuestas de la forma
que se indica en la Figura. El circuito es alimentado
mediante una fuente de voltaje alterno de ecuación
V (t) = V0 sin ωt. Determine
a) La impedancia equivalente del circuito y el V0
módulo de la corriente en función del tiempo
por cada rama del circuito.
b) La frecuencia de resonancia del circuito, ¿Cuál
es el valor de la corriente máxima que sale de la
fuente? (exprese su resultado en función de la
frecuencia de resonancia).

R1

R2

L

C

Problemas Propuestos y Resueltos de Electromagnetismo

En la figura se esquematiza la conexión de un computador personal, una lampara de escritorio y una estufa
eléctrica a un enchufe múltiple (“alargador”) el cual
es conectado al enchufe de 220 V en la muralla. Las
especificaciones de cada artículo aparecen en la figura.
El enchufe E conectado a la muralla tolera una corriente máxima de 7 A. Examine cuantitativamente la
conexión y determine si el enchufe E es el adecuado.

[220 V]
[1,5 A]

---

### Página 348

CAPÍTULO 17. CORRIENTE ALTERNA
#### Problema 17.6

X I

Los enchufes eléctricos chilenos proveen una fuente
de voltaje alterno con 220 [V] y una frecuencia 50
[Hz], por otro lado, los enchufes en Estados Unidos
usan 120 [V] y una frecuencia 60 [Hz]. Si se trae una
ampolleta de 60 [W] y 120 [V] de Estados Unidos a
Chile, ¿Cuán grande debe ser una inductancia L, en
henrys, que debe ser conectada en serie tal que la
ampolleta opere normalmente, produciendo la misma
cantidad de luz como si fuese conectada en Estados
Unidos?. Explique brevemente por qué es ventajoso
corregir la iluminación con una inductancia en vez de
una resistencia.
#### Problema 17.7

X S

R2

C

Para el circuito en la figura, muestre si

V0

L
R1 R2 =
C

A

B

R1

L

entonces VA = VB sin importar la frecuencia ω. Ambos potenciales están medidos de la tierra del circuito.

Rodrigo Chi - Marzo 2017

#### Problema 17.8

X I

El circuito de la figura tiene una fuente de voltaje
alterno V (t) = V0 cos ωt , conectada en serie con una
resistencia R = 1 Ω y una = caja negra”, que puede
contiene un condensador, un inductor, o ambos. Se
mide la corriente que circula en el circuito con una
frecuencia angular ω1 = 1 rad/s y se observa que la
corriente adelanta al voltaje de la fuente en una fase
de π/4 radianes. Si se repite el experimento con una
frecuencia a ω2 = 2 rad/s se encuentra la corriente
se atrasa exactamente π/4 radianes con respecto a la
fuente.
a) ¿Qué hay dentro de la caja negra?.
b) ¿Cuál/es es/son los valor/es de inductancia o/y
capacitancia?.
c) ¿Puede ser el circuito resonante?, en caso de
serlo, ¿cuál es la frecuencia de resonancia?.

R
V0

?

---

### Página 349

CAPÍTULO 17. CORRIENTE ALTERNA
#### Problema 17.9

X I

a) Un circuito RLC serie contiene una inductancia
de 0.1 H. y una resistencia y capacitancia de
valor desconocido. Cuando el circuito es conectado a una fuente AC V (t) = 230 sin 100πt,
la corriente que fluye por el circuito es I(t) =
2,3 sin 100πt. Encuentre: los valores de la resistencia y la capacitancia, la diferencia de potencial en la inductancia y la potencia promedio
total consumida.
b) Un circuito resonante en paralelo consiste en un
condensador C = 32 pF en paralelo con una inductancia F = 18 µH y una resistencia R = 60
Ω, respectivamente. Determine la frecuencia de
resonancia del circuito y el módulo de la impedancia equivalente en función de la frecuencia
ω del generador.

#### Problema 17.10

X I

Suponga usted que cuenta con dos herramientas que
operan 110 V. Una de ellas es un taladro eléctrico
cuyas especificaciones son (110 V - 2,6 A). La otra
herramienta en una sierra eléctrica de especificaciones (110 V - 3 A). Para utilizar estas herramientas
requiere un transformador que reduzca el voltaje de
220 V a 110 V. Estos aparatos se encuentran en el
comercio y los hay de 50 W, 100 W, 800 W, 1000
W, 1500 W. Mientras mayor es la potencia tolerable
por el transformador mayor es su precio. Determine el
transformador más económico que permita la operación simultánea de ambas herramientas.

V0

L

C

(a) RLC Serie

V0

R

L

C

(b) RLC Paralelo
Problemas Propuestos y Resueltos de Electromagnetismo

c) Un generador entrega un voltaje constante con
frecuencia variable de Vrms = 100 [V] (rms) a un
circuito RLC serie que contiene R = 5Ω, L = 4
mH, y C = 0.1 µF . La frecuencia del generador
se varía hasta que se obtiene el máximo valor de
la corriente. Determine el valor de la corriente
máxima, la frecuencia en la cual ocurre, y el
voltaje entre la inductancia y el condensador.

R

---

### Página 350

CAPÍTULO 17. CORRIENTE ALTERNA

III.

Soluciones

Solución 17.3

P X

a) La impedancia equivalente está dada por
+
Z =R+
jXL − jXC1 −jXC2

!−1

!−1

−jXC2 + jXL − jXC1
=R+
(XL − XC1 )XC2
(XL − XC1 )XC2
=R+j
XC2 + XC1 − XL
ω 2 LC1 − 1
=R+j
ω(C1 + C2 − ω 2 LC1 C2 )

b) La frecuencia de resonancia es tal que la parte imaginaria de la impedancia se vuelve nula,
es decir
=⇒ ω0 = √
XL = XC1 =⇒ ω0 L =
ω0 C1
LC1
Nótese el hecho que al elegir esta frecuencia, el módulo de la impedancia se vuelve mínimo,
y en consecuencia, se maxima el módulo de la corriente que sale de la fuente.
c) La corriente que circula por la resistencia es
V0 ejωt
I(t) = Re
Z
(

)

V0 ejωt
= Re
|Z|ejφ
(

)

=

V0
cos(ωt − φ)
|Z|

Rodrigo Chi - Marzo 2017

donde de la parte anterior se tiene que los valores de |Z| y φ son
v
u
u
|Z| = tR2 +

ω 2 LC1 − 1
ω(C1 + C2 − ω 2 LC1 C2 )

!2

ω 2 LC1 − 1
φ = arctan
Rω(C1 + C2 − ω 2 LC1 C2 )

!

d) Finalmente, la potencia media que entrega la fuente es
V02
cos φ
2|Z|
V2
= 0 2 Re{Z}
2|Z|
V02 R
=

2
ω 2 LC1 −1
2R2 + 2 ω(C1 +C
2 −ω LC1 C2 )

hP i =

---

### Página 351

CAPÍTULO 17. CORRIENTE ALTERNA
Solución 17.5

P X

a) La impedancia equivalente está dada por


Zeq =

+
R1 + ZL R2 + ZC

−1

donde ZL = jXL y ZC = −jXC , con XL = ωL y XC = ωC
. Luego

!−1

+
Zeq =
R1 + jXL R2 − jXC
(R1 + jXL )(R2 − jXC )
=
(R1 + R2 ) + j(XL − XC )
(R1 R2 + XL XC ) + j(XL R2 − XC R1 )
=
(R1 + R2 ) + j(XL − XC )
[(R1 R2 + XL XC ) + j(XL R2 − XC R1 )][(R1 + R2 ) + j(XL − XC )]
=
(R1 + R2 )2 + (XL − XC )2
(R1 R2 + XL XC )(R1 + R2 ) − (XL R2 − XC R1 )(XL − XC )
=
(R1 + R2 )2 + (XL − XC )2
(R1 R2 + XL XC )(XL − XC ) + (XL R2 − XC R1 )(R1 + R2 )
+j
(R1 + R2 )2 + (XL − XC )2
Los módulos de cada una de las corrientes vale
V0
V0 ejωt
V0 ejωt
=q
|I1 (t)| =
|I2 (t)| =
R1 + jωL
R1 − j ωC
R12 + ω 2 L2

V0
=q
1 2
R22 + ( ωC
)

b) La frecuencia de resonancia puede ser calculada al hacer nula la parte imaginaria de la
impedancia, de modo que
(R1 R2 + XL XC )(XL − XC ) + (XL R2 − XC R1 )(R1 + R2 ) = 0
Reemplazando los valores de XL y XC





R1
L
R1 R2 +
− ω0 L = ω0 LR2 −
(R1 + R2 )
C
ω0 C
ω0 C
donde puede despejarse el valor de ω0 como
v
u

u R2 C − L
ω0 = √
· t 12
R2 C − L
LC

El valor de la corriente para esa frecuencia vale
(R1 + R2 )2 + (ω0 L − ω01C )2
V
|V0 |
I=
=⇒ |I| =
= V0 ·
Zeq
|Zeq |
(R1 R2 + CL )2 + (ω0 LR2 − ω01C R1 )2

Problemas Propuestos y Resueltos de Electromagnetismo

Nótese que los módulos de las corrientes son constantes en el tiempo y sólo dependen
de los parámetros fijos del circuito. El aporte temporal está dado netamente por la parte
exponencial compleja de la corriente.

---

### Página 352

CAPÍTULO 17. CORRIENTE ALTERNA
Solución 17.7

P X

Previamente, antes de resolver el problema, es bueno conocer el concepto de = Divisor de
Voltaje” que es sumamente útil en problemas de corriente alterna.
Z1

Vout
Z2

Vin

Figura 17.1: Divisor de Voltaje con Impedancias
En la Figura 17.1 es posible apreciar una malla de un circuito CA que posee dos impedancias
en serie Z1 y Z2 . El divisor de voltaje permite obtener el voltaje el punto Vout , que es
justo antes de donde comienza la impedancia Z2 . Nótese que Vout representa la caída de
tensión al pasar la corriente por Z1 . Para determinar el valor de Vout se debe considerar que
Vin = I · (Z1 + Z2 ) y Vout = I · Z2 , juntando ambas ecuaciones se llega a
Vout = Vin ·

Z2
Z1 + Z2

Volviendo al problema, usando notación fasorial para la fuente V (t) = V0 ejωt , se tiene que
usando la fórmula del divisor de voltaje para la rama que contiene a C y R1 :
VA = V0 ejωt ·

R1
ZR1
jωt
= V0 ejωt ·
·
j = V0 e
Zc + ZR1
R1 − ωC
1 − R1jωC

Rodrigo Chi - Marzo 2017

De la misma manera, para la rama que contiene a R2 y L:
VB = V0 ejωt ·

jωL
= V0 ejωt ·
R2 + jωL
1 − jR
ωL

Luego, usando el dato que R1 R2 = CL o equivalentemente R1 C = RL2 , se llega a que
VA = V0 ejωt ·

1 − ωRj1 C

que era lo que se quería demostrar.

= V0 ejωt ·

= VB
1 − jR
ωL

---

### Página 353

CAPÍTULO 17. CORRIENTE ALTERNA

IV.

Indicaciones Problemas Sin Solución

Indicación 17.1

P X

Use las Leyes de Kirchhoff aplicadas al circuito y encuentre el la diferencia de potencial
entre A y B.
Recuerde que las impedancias pueden ser tratadas como resistencias. Se recomienda llamar
Zc a la impedancia del condensador y no reemplazar su valor hasta obtener el resultado
final.

Indicación 17.2

P X

Determine el valor de la frecuencia de resonancia de un circuito RLC, a partir de ello puede
encontrar C.
Las demás partes del problema son aplicaciones directas de fórmulas expresadas en el resumen.

Indicación 17.4

P X

Indicación 17.6

P X

Determine la resistencia de la ampolleta con los datos entregados sobre Estados Unidos.
Recuerde que los valores entregados de voltaje son rms.
Ajuste el valor de la inductancia que debe ser colocada en serie para que la potencia emitida
por la ampolleta en Chile sea la misma que en Estados Unidos.

Indicación 17.8

P X

Haga inicialmente el análisis de que pasaría si hubiese sólo un condensador o sólo un inductor
en la caja negra. ¿Podría darse la condición del enunciado al cambiar la frecuencia?.

Problemas Propuestos y Resueltos de Electromagnetismo

Recuerde que la potencia entregada por los fabricantes es promedio y que la corriente y el
voltaje son rms (y no máximos).

---

### Página 354

CAPÍTULO 17. CORRIENTE ALTERNA
Una vez impuesto el circuito RLC, imponga las condiciones del enunciado y despeje los
valores de R y C.
De lo anterior es directo poder determinar la frecuencia de resonancia del circuito.

Indicación 17.9

P X

Para el primer problema, note que cuando se alimenta el circuito con una fuente de voltaje
con esa frecuencia la corriente está totalmente en fase. Lo anterior ocurre cuando el circuito
está en resonancia.
En el segundo problema, determine la impedancia equivalente del sistema (todas las impedancias se encuentran en paralelo). Lo pedido es directo de esa expresión.
Para el tercer problema, recuerde que la máxima corriente ocurre en la frecuencia de resonancia.

Indicación 17.10

P X

Rodrigo Chi - Marzo 2017

Encuentre la potencia consumida por las herramientas, recuerde que el voltaje y la corriente
entregada es en rms.

---

### Página 355

CAPÍTULO 17. CORRIENTE ALTERNA

V.

Resultados
Problema

P

Respuestas
b) φ = 2 arctan ωRC

17.1

c) Cambian los dos resultados anteriores, ya que ocurre una división de voltaje previa
que cambia el módulo y el desfase de la diferencia de potencial.
a) C = 281n[F ]
b) R = (225)ej1,11 Ω

P

17.2

c) I(t) = 0,89 cos(10000πt − 1,11) [A]
d) hP i = 39,6 [W]
C
L
R
= 100,7 [V]
= 89π [V], Vmax
= 89 [V], Vmax
e) Imax = 0,89 [A] , Vmax

ω LC1 −1
a) Z = R + j ω(C1 +C
2 −ω LC1 C2 )
b) ω0 = √LC

r

P

17.3

c)

V0
I(t) = |Z|
cos(ωt − φ) donde |Z| =

φ = arctan
d) hP i =

17.4

ω 2 LC1 −1
Rω(C1 +C2 −ω 2 LC1 C2 )
V02 R

2R2 +2

ω 2 LC1 −1
ω(C1 +C2 −ω 2 LC1 C2 )



ω 2 LC1 −1
ω(C1 +C2 −ω 2 LC1 C2 )

2



2

√
Imax = 7 2 > 7 [A] . El enchufe no es capaz de trabajar con esa corriente.
a) Zeq = ( R1 +jX
+ R2 −jX
)−1 , donde XL = ωL y XC = ωC
, |I1 (t)| = √ 2V0 2 2
L
C
R1 +ω L

P

17.5

|I2 (t)| = √ 2 V0 1

R2 +( ωC )2

b) ω0 = √LC
·

q

(R1 +R2 )2 +(ω0 L− 1 )2
R12 C−L
y |I| = V0 · (R R + L )2 +(ω LR −ω0 C1 R )2
R22 C−L
1 2
C
ω C

Problemas Propuestos y Resueltos de Electromagnetismo

P



R2 +

---

### Página 356

CAPÍTULO 17. CORRIENTE ALTERNA
Problema

Respuestas
r

P

17.6

Rampolleta = 240Ω, L =

Vrms-chile
Rampolleta −P ·Rampolleta
P ·(2πfchile )2

= 1,2[H] (una inductancia muy

grande!). Es mejor un inductor ya que no consume potencia.
a) Contiene un inductor y un condensador.

P

17.8

b) C = 0,5 F y L = 1H.
c) Sí, y la frecuencia es ω0 =

√

2 rad/s .

a) R = 100Ω, C ≈ 10−5 F, ∆V (t) = 23π sin(100πt + π2 ), P = 72,25 W.

P

17.9

b) ω0 = √LC
, |Z| = p L 2

L
R· C

( C ) +R2 (ω 2 L2 − ω21C 2 )

√

c) Imax = VrmsR 2 , esto ocurre en resonancia con ω = ω0 = √LC
y ∆VLC (ω = ω0 ) = 0.

17.10

La potencia consumida es de 616 W, por lo que bastaría un transformador de 800 W.

Rodrigo Chi - Marzo 2017

P

---

### Página 357

Leyes de Maxwell

I.

Resumen Teórico

Ley de Ampère-Maxwell
Debido a la incompatibilidad de lo propuesto por Ampère con la Ecuación de Continuidad en el
caso no estático, es necesario corregirla de la siguiente forma
~
~ ×H
~ = J~ + ∂ D
∇
∂t

(18.1)

En su forma integral, la ecuación se transforma en
¨
˛
¨
∂
~
~
~
~ · dS
~
~
D
H · dl =
J · dS +
∂t
Ω

Ω

donde Γ es el borde de superficie Ω. En particular, se define la corriente desplazamiento como
¨
∂
~
~ · dS
Id =
D
(18.3)
∂t
Ω

debido a que es provocada por el cambio el tiempo de ese vector.

Teorema de Poynting
El vector de Poynting se define como
~= 1E
~ ×B
~ =E
~ ×H
~
S
µ0

(18.4)

Por otro lado, la energía electromagnética por unidad de volumen estada dada por
1 ~ ~
~ · H)
~
uem = (D
·E+B

(18.5)

Problemas Propuestos y Resueltos de Electromagnetismo

Γ

(18.2)

---

### Página 358

CAPÍTULO 18. LEYES DE MAXWELL
El teorema de Poynting indica que
∂uem ~ ~
~
+ ∇ · S = −J~ · E
∂t

(18.6)

En su versión integral
∂
∂t

˚

¨
uem dV +

˚
~ =−
~ · dA
S

~
J~ · EdV

(18.7)

equivalentemente
∂Uem
+ ΦS = −P
(18.8)
∂t
Esta ecuación constituye un balance de energía electromagnética Uem , ya que relaciona la variación
de la energía electromagnética con el flujo de vector de Poynting ΦS y con las fuentes que provocan
~
esta energía (término J~ · E).

Ecuaciones de Maxwell en el vacío
Las ecuaciones de Maxwell en el vacío son
~ ·E
~ = ρ
∇
ε0
~
~ ×E
~ = − ∂B
∇
∂t
~
~
∇·B =0

(18.9)

~
~ ×B
~ = µ0 J~ + µ0 ε0 ∂ E
∇
∂t
Mientras que las ecuaciones de Maxwell en medios materiales está dado por

Rodrigo Chi - Marzo 2017

~ ·D
~ =ρ
∇
~
~ ×E
~ = − ∂B
∇
∂t
~ ·B
~ =0
∇

(18.10)

~
~ ×H
~ = J~ + ∂ D
∇
∂t

Ecuación de Onda
Se dice que una función u(x, y, z, t) satisface la ecuación de onda cuando
∇2 u −

1 ∂ 2u
=0
v 2 ∂t2

(18.11)

---

### Página 359

CAPÍTULO 18. LEYES DE MAXWELL
Donde se denomina v es la velocidad de la onda.
Suponiendo que las ondas viajan en vacío, de modo que ρ = 0 y J~ = 0 y a partir de las Ecuaciones
en 18.9, es posible afirmar que
2~
~ − µ 0 ε0 ∂ E = 0
∇2 E
(18.12)
∂t2
2~
~ − µ 0 ε0 ∂ B = 0
∇2 B
(18.13)
∂t2
Esto quiere decir que los campos eléctrico y magnético satisface la ecuación de onda. En el caso
~
particular de un campo eléctrico tenga dependencia de una única variable, ie. E(x,
y, z, t) =
~
E(x,
t) la Ecuación 18.12 se reduce a
~
~
∂ 2E
∂ 2E
−
µ
ε
=0
∂x2
∂t2

(18.14)

La Ecuación 18.14 es la ecuación de onda para una función de una sola variable, la cual tiene por
~
solución E(x,
t) = F (x − vt) + G(x + vt), donde F y G son funciones reales. La velocidad de
está onda es
=c
(18.15)
=
µ
ε
=⇒
v
=
√
v2
µ 0 ε0
Las ondas electromagnéticas viajan a la velocidad de la luz. Por lo que se deduce que hay una
infinidad de formas posibles tanto para el campo eléctrico como magnético mientras satisfaga las
Ecuaciones en 18.9.

Ondas Planas Monocromáticas

~ =E
~ 0 cos(~k · ~r − ωt) = E0 n̂ cos(~k · ~r − ωt)
E

(18.16)

donde ~k es conocido como el vector de onda el cual indica la dirección de propagación de la onda,
n̂ es vector que indica la dirección del campo eléctrico (también llamado vector de polarización
de la onda) y ω su frecuencia. En su forma compleja, también se denota como
~ =E
~ 0 ej(~k·~r−ωt)
E

(18.17)

El argumento de la exponencial compleja se puede reescribir como
~k · ~r − ωt = k k̂ · ~r − ω t
k




(18.18)

A partir de esto se deduce que
El vector de onda ~k = k k̂ es inversamente proporcional a la longitud de onda λ = 2π
. El
k
vector unitario k̂ señala la dirección de propagación de la onda.

Problemas Propuestos y Resueltos de Electromagnetismo

El caso particular de estudio son las ondas planas y monocromáticas. El campo eléctrico perteneciente a este tipo de onda es de la forma

---

### Página 360

CAPÍTULO 18. LEYES DE MAXWELL
La velocidad de fase de la onda es v = ωk , donde en el caso particular del vacío se tiene que
ω
= c.
k
= 2πf donde T es el periodo de la onda y f
La frecuencia angular de la onda es ω = 2π
T
su frecuencia.
En el caso de la polarización lineal n̂ es fijo en el tiempo. En otras polarizaciones como
circulares y elípticas, el vector n̂ = n̂(~r, t) depende de la posición y el tiempo.
Dada las Ecuaciones de Maxwell es posible afirmar que
~ ⊥B
~ ⊥ ~k
E

(18.19)

~ =0
~ = ~k · E
~ ·B
~ = ~k · B
E

(18.20)

Por lo anterior
Adicionalmente, también debe cumplirse que
~ ~
~ = k×E
B
ω

(18.21)

Intensidad de una Onda
La intensidad de la onda se determina a partir del vector de Poynting promedio de una onda el
cual puede ser determinado como
ˆT
~
~ =
S(t)dt
(18.22)
hSi
T

Rodrigo Chi - Marzo 2017

donde T = 2π
. Si la onda es tratada en su forma compleja, el vector de Poynting promedio puede
ω
ser determinado en forma equivalente como
~ =
hSi

~ ×H
~ ∗}
Re{E

(18.23)

~ ∗ es el vector conjugado a H.
~
donde H

Recomendaciones
Las ondas electromagnéticas son un resultado notable dentro de un curso de electromagnetismo.
En la mayoría de los casos es más sencillo trabajar la expresión de onda como un complejo
más que con senos y cosenos.

---

### Página 361

CAPÍTULO 18. LEYES DE MAXWELL

II.

Problemas Propuestos

#### Problema 18.1

d

X S

Se tiene dos discos conductores paralelos de radio c
y separados una distancia d
c entre los cuales se
ha colocado una sustancia homogénea de conductividad g y permitividad ε0 . Los discos se someten a una
diferencia de potencial V (t) conocida.

c

e

b

a) Calcule la fem inducida en un rectángulo de lados a y b como se muestra en la Figura.
Evalúe
− εg t
en particular esa fem si V (t) = V0 e
.

µ0 e g

~ dentro del
b) Determine el vector de Poynting S
condensador y compruebe el teorema de Poynting.
#### Problema 18.2

V (t)

X I

Para calcular de una forma más exacta el campo
eléctrico dentro de un condensador de placas paralelas
circulares (ver Figura), en el que se aplica una fuente
de voltaje alterna se plantea el siguiente método:
~ 0 (t) como valor del campo en un
a) Determine E
régimen cuasiestático.

~ 1 (t), determine E
~ 2 (t) inducido.
c) Con B
d) Finalmente, determine el valor más exacto como
~
~ 0 (t) + E
~ 2 (t).
E(t)
≈E
X S

a) Explique qué es una onda plana monocromática
e identifique explícitamente la dirección de propagación, la velocidad de propagación, la frecuencia, y la longitud de onda.
b) En el caso que la onda plana sea electromagnéti~ yB
~ son perca, demuestre que los campos E
pendiculares entre si y (ambos) perpendiculares
a la dirección de propagación. Indicación: use
las ecuaciones de Maxwell.

a

d
V (t) = V0 cos wt

Problemas Propuestos y Resueltos de Electromagnetismo

~ 0 (t), determine B
~ 1 (t) inducido.
b) Conocido E

#### Problema 18.3

a

---

### Página 362

CAPÍTULO 18. LEYES DE MAXWELL
#### Problema 18.4

X S

Se plantea estimar en forma idealizada la incorporación de energía solar para suplir necesidades de potencia eléctrica del área metropolitana. Se sabe que la
potencia electromagnética del Sol es PS = 3,8 · 1026
W. Además, la distancia entre la Tierra y el Sol es
R = 1,5 · 1011 m.
a) Calcule la magnitud del vector de Poynting (valor medio) en la Tierra
b) Suponiendo que: no hay pérdidas de energía por
la atmósfera; que el Sol sale a las 8h00 y se pone
a las 18h00; y que el Sol pasa por el zenit a las
13h30 (simplificación), calcule la energía solar
directa recibida por un panel horizontal de 1 m2
de superficie durante un día.
c) Si el consumo anual promedio por habitante es
de 700 kWh, y suponiendo eficiencia de 100 %
en el proceso de generación de energía eléctrica a partir de la solar, dimensione los paneles
solares necesarios para cubrir el consumo de un
habitante. ¿Que área es la que se necesitaría
para seis millones de habitantes? Comente.

Rodrigo Chi - Marzo 2017

#### Problema 18.5

X I

Considere una onda electromagnética que posee el siguiente campo eléctrico
~ = E0 cos[(10 m−1 ) · x + (3 · 109 s−1 ) · t]ẑ
E
Encuentre:
a) La longitud de onda λ y el periodo T .
b) La dirección y el sentido de propagación.
~ asociado a esta onda.
c) El campo magnético B
~
d) El vector de Poynting S.

---

### Página 363

CAPÍTULO 18. LEYES DE MAXWELL
#### Problema 18.6

X S

a) Escriba una expresión para el campo eléctrico y
magnético de una onda electromagnética plana,
cuyo campo eléctrico está contenido en el plano
xy y se propaga desde el origen hasta el punto
(0, 3, 3). La frecuencia angular de la onda es
ω = 100π [rad/s] y la velocidad de la luz es c.
La magnitud del campo eléctrico es E0 .
b) Encuentre la potencia promedio que transporta
esta onda.
#### Problema 18.7

X I

Una onda plana linealmente polarizada se propaga a
lo largo de la dirección √12 (x̂ + ŷ) en el vacío. La
polarización de la onda yace sobre el plano XY (ie,
el campo eléctrico vive en el plano XY ).Si el módulo
de campo eléctrico es E0 y la frecuencia de la onda
es ω, encuentre
~ y B.
~
a) Las funciones reales que representan E
b) El promedio temporal del vector de Poynting.
#### Problema 18.8

Considere una onda electromagnética que viaja en la
dirección z en el vacío, el cual posee un campo eléctrico dado por
~ = E1 ej(kz−ωt) x̂ + E2 ej(kz−ωt−φ) ŷ
E
donde E1 y E2 son números reales.
a) Determine el campo magnético asociado a esta
onda electromagnética y el promedio temporal
de Poynting.
b) Considere el caso φ = π2 y E1 = E2 = E0 .
Encuentre las funciones reales que describen el
campo eléctrico y magnético de la onda.
~ vs tiempo (en z = 0) y E
~
c) Realice un gráfico E
vs posición z (en t = 0) ¿Qué comportamiento
tiene la onda electromagnética?.

Problemas Propuestos y Resueltos de Electromagnetismo

X I

---

### Página 364

CAPÍTULO 18. LEYES DE MAXWELL
X I

#### Problema 18.9

Al interior de una guía de ondas se transmite una
onda electromagnética (solución de las ecuaciones de
Maxwell en ausencia de cargas y corrientes ρ = 0
y J~ = 0) tal que las únicas componentes del campo
~ son Bx y Bz . Su expresión en función
magnético son B
de las coordenadas x, z y del tiempo t es:
πx
aB0 k
sin
sin(kz − ωt)
π
a


Bx =

y



πx
cos(kz − ωt)
a
en donde a, B0 , k y ω son constantes. La relación
entre k y ω es




Bz = B0 cos

s

k=

x
z

ω2 π2
− 2
c2
a

~ sólo tiene compoSe sabe que el campo eléctrico E
nente Ey que es función solamente de las coordenadas
x, z, t. Encuentre la expresión para este Ey .

#### Problema 18.10

X S

Dos ondas electromagnéticas son emitidas desde dos
diferentes fuentes, de modo que
~ 1 (x, t) = E10 cos(kx − ωt)ŷ
E

Rodrigo Chi - Marzo 2017

~ 2 (x, t) = E20 cos(kx − ωt + φ)ŷ
E

y

c

c

a) Encuentre el vector de Poynting asociado a la
onda electromagnética resultante.
x

b) Encuentre la intensidad de la onda.
c) Repita el calculo si la dirección de propagación
de la segunda onda electromagnética viaja en la
dirección contraria a la primera
~ 1 (x, t) = E10 cos(kx − ωt)ŷ
E
~ 2 (x, t) = E20 cos(kx + ωt + φ)ŷ
E

---

### Página 365

CAPÍTULO 18. LEYES DE MAXWELL
#### Problema 18.11

X S

En un buen conductor, cuando la frecuencia no es demasiado grande, una buena aproximación consiste en
despreciar el término de la corriente desplazamiento.
~ es
En tal caso la ecuación para E
~ − µ0 g
∇2 E

~
∂E
=0
∂t

Considere el caso de una onda plana que ha penetrado
a un medio (interfaz: plano XY ) con conductividad
g.
a) Tomando ~k = (0, 0, k) demuestre de lo anterior
q

que k = (1 + j) ωµ0 g/2. En lo que sigue se
usará la notación k0 =

q

ωµ0 g/2

b) Para el campo eléctrico de una onda plana en el
medio conductor, luego de una incidencia nor~ = E0 ej(kz−ωt) x̂, (convencionalmente
mal, es E
~
escoja E0 real). Determine el valor de B.
c) D
Calcule
el flujo temporal del vector de Poynting
E
~
S

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 366

CAPÍTULO 18. LEYES DE MAXWELL

III.

Soluciones

Solución 18.1

P X

a) Dado que el potencial depende del tiempo V (t), el campo eléctrico también estará variando
en el tiempo y éste provocará un campo magnético que inducirá una fem en la espira
rectangular. En una primera aproximación, el campo dentro de un condensador puede ser
estimado como
ˆ
~ =⇒ V (t) = E(t)d =⇒ E
~ · dl
~ = V (t) ẑ
V = E
d
Luego, para puntos dentro del condensador r < c debe cumplirse que
˛
¨
¨
d
~
~
~
~
~
~ · dS
H · dl =
J · dS +
D
dt
Γ

Ω

Ω

~ D
~ = ε0 E
~ yH
~ = H(r, t)θ̂
Donde Ω es un circulo de radio r y Γ su borde. Como J~ = g E,
la expresión anterior se transforma en
˛
¨
¨
d
~
~
~
~
~
~ · dS
H · dl = g
E · dS + ε0
E
dt
Γ

Ω

Ω

g
ε0
H(r) · 2πr = V (t)πr2 + V̇ (t)πr2
d
d
~ = µ0 H
~ el campo magnético dentro del condensador vale
Luego como B
µ0 r
~
(gV (t) + ε0 V̇ (t))θ̂
B(r)
=
2d
Rodrigo Chi - Marzo 2017

Luego, el flujo sobre la espira es
ˆe+aˆb
Φ=
e

µ0 r
µ0 ab2
(gV (t) + ε0 V̇ (t))drdz =
(gV (t) + ε0 V̇ (t))
2d
4d

Por lo tanto

dΦ
µ0 ab2
=−
(g V̇ (t) + ε0 V̈ (t))
dt
4d
En el caso particular de potencial entregado, se tiene
ε=−

− εg t

V (t) = V0 e

V0 g − εg t
V0 g 2 − εg t
=⇒ V̇ (t) = −
e
=⇒ V̈ (t) = 2 e 0
ε0
ε0

Al evaluar los valores anteriores se obtiene ε = 0.

---

### Página 367

CAPÍTULO 18. LEYES DE MAXWELL
b) El vector de Poynting dentro del condensador vale
~=E
~ ×H
~ = − rV (t) (gV (t) + ε0 V̇ (t))r̂
S
2d2
Por lo que el flujo sobre la superficie del condensador (manto cilíndrico) es
ˆ2π ˆd
−

ΦS =

2πc2 V (t)
cV (t)
(gV (t) + ε0 V̇ (t))
(gV
(t)
+
ε
V̇
(t))r̂
·
cdθdzr̂
=
−
2d2
2d

Por otro lado, la energía electromagnética vale
˚
ε0
ε0 πc2 V 2
Uem =
|E|2 dV =
2d
Cilindro

No se ha considerado la energía magnética, ya que al ser inducida por el campo eléctrico
es de mucho menor magnitud. Falta por determinar el valor de la potencia disipada en el
cilindro la cual está dada por
˚
gπc2 V 2
~
P =
J~ · EdV
=
d
Cilindro

Finalmente

Lo que comprueba el Teorema de Poynting.

Solución 18.3

P X

a) Una onda plana es una onda tal que se propaga en una sola dirección en el espacio, o
equivalentemente, su frentes de ondas son infinitos planos perpendiculares a la dirección de
propagación. Un onda plana es monocromática debido a que posee una única frecuencia de
propagación. La forma matemática para expresarla (solución de la ecuación de ondas) es
~

A(~r, t) = Aej(k·~r−ωt)
donde:
- La dirección de propagación está dada por el vector ~k,

Problemas Propuestos y Resueltos de Electromagnetismo

Uem
ε0 πc2 V V̇
πc2 V
+ ΦS =
−
(gV + ε0 V̇ )
∂t
d
d
gπc2 V 2
=−
d
= −P

---

### Página 368

CAPÍTULO 18. LEYES DE MAXWELL
- La velocidad de onda puede ser obtenida al reemplazar la expresión anterior en la
ecuación de ondas, resultando v = |ω~k| .
- La frecuencia angular está dada por ω = 2πf , donde f es la frecuencia.
- La longitud de onda λ está dada a partir del módulo del número onda como |k| = 2π
.
λ
b) Se debe considerar un campo eléctrico arbitrario como
~ =E
~ 0 ej(~k·~r−ωt) = (E0x x̂ + E0y ŷ + E0z ẑ)ej(~k·~r−ωt)
E
~ = (E0x x̂+E0y ŷ+E0z ẑ)ej(kx x+ky y+kz z−ωt) .
Reescribiendo ~k = kx x̂+ky ŷ+kz ẑ se tiene que E
Tomando la divergencia de este campo
~ ·E
~ = ∂Ex + ∂Ey + ∂Ez = j (kx E0x + ky E0y + kz E0z )ej(kx x+ky y+kz z−ωt)
∇
|
{z
}
∂x
∂y
∂z
~k·E
~

~ ⊥ ~k, de igual
~ ·E
~ = 0 =⇒ E
~ · ~k = 0 =⇒ E
Por la primera ley de Maxwell, se sabe que ∇
~ ·B
~ = 0 =⇒ B
~ ⊥ ~k. Por otro lado
forma como ∇
!
!
!
∂Ez ∂Ey
∂Ex ∂Ez
∂Ey ∂Ex
~
~
∇×E =
x̂ +
ŷ +
ẑ
−
−
−
∂y
∂z
∂z
∂x
∂x
∂y
|

{z

}

j(ky E0z −kz E0y )ej(~k·~r−ωt)

|

{z

}

j(kz E0x −kx E0z )ej(~k·~r−ωt)

|

{z

}

j(kx E0y −ky E0x )ej(~k·~r−ωt)

Por lo tanto
~
~ E
~ = j [(ky E0z − kz E0y )x̂ + (kz E0x − kx E0z )ŷ + (kx E0y − ky E0x )ẑ] ej(~k·~r−ωt) = j~k×E
∇×
|

{z

~k×E
~0

}
~

Rodrigo Chi - Marzo 2017

~ =B
~ 0 ej(k·~r−ωt) y aplicando
Suponiendo que el campo magnético también es de la forma B
la Ley de Faraday
~ ~
~
~ = jω B
~ =⇒ B
~ = k×E
~ ×E
~ = − ∂ B =⇒ j~k × E
∇
∂t
ω
~ a ambos lados
Aplicando producto punto con E
~ ~
~
~
~ ·B
~ =E
~ · k × E = ~k · E × E = 0
E
ω
ω
~ ⊥B
~ ⊥ ~k.
Por lo que se deduce finalmente que E

Solución 18.4

P X

a) La radiación del Sol tiene la misma intensidad en todas las direcciones, por lo que la tasa
a la que llega a la Tierra es la misma tasa la que pasa a través de una esfera centrada en
el Sol con un radio igual al radio de la órbita de la Tierra. Luego tiene que cumplirse
P = |S| · A =⇒ |S| =

P
3,80 · 1026
W
=
≈ 1350 2
A
4π(1,5 × 10 )
m

donde A se considero el área de la Tierra.

---

### Página 369

CAPÍTULO 18. LEYES DE MAXWELL
b) Dado los horarios del enunciado, se explicita que el sol se mueve con una velocidad angular
constante sobre el panel.
13:30 hrs
Sol

Panel Solar

q

18:00 hrs

~S

08:00 hrs

Figura 18.1: Movimiento del Sol.
~ sin θ =
La componente de vector de Poynting que apunta directamente al panel es |S|
~ sin ωt, donde ω = π y ∆T = 10 horas. Luego, si se desea encontrar la energía solar
|S|
∆T
directa sobre el panel hay que integrar esa componente de la siguiente forma
ˆ∆T
|S| sin ωtdt = APanel

U = APanel

|S|∆T
|S|
(− cos π + cos 0) = 2APanel
ω
π

Evaluando numéricamente el resultado U ≈ 8,6 kWh .

At =

700 kWh
año
kWh = 0,22m
3139 m2 año

Para 6 millones de personas el área total vendría siendo 1,32 km2 esto es del orden de
casi 2000 canchas de fútbol una al lado de la otra o casi el doble del tamaño del Parque
O’Higgins en Santiago de Chile.

Solución 18.6

P X

a) Se debe recordar que la forma general del campo eléctrico de una onda electromagnética
es en este caso:
~ = E0 n̂ej(~k·~r−ωt)
E
Donde ~r = (x, y, z) y ~k = k k̂ indica la dirección de propagación de la onda y n̂, la
polarización del campo eléctrico. En este caso la dirección de propagación de la onda es k̂

Problemas Propuestos y Resueltos de Electromagnetismo

c) Del resultado anterior se tiene que la generación de energía por unidad de área es de
kWh
8,6 mkWh
2 día = 3139 m2 año . Luego, para alcanzar los 700 kWh anual, debe tenerse un área de

---

### Página 370

CAPÍTULO 18. LEYES DE MAXWELL
(unitario) y está determinado por
ŷ + ẑ
(0, 3, 3) = √ (0, 1, 1) = √
k̂ = √ 2
3 +3
Por otro lado se sabe que el campo eléctrico está polarizado en el plano xy por lo que
n̂ = √ 2
(α, β, 0)
α + β2
Ahora usando el hecho que la dirección de propagación es siempre perpendicular a la polarización de la onda se cumple que
k̂ · n̂ = 0 =⇒ (0, 1, 1) · (α, β, 0) = 0 =⇒ β = 0
Por ende

n̂ = √ (α, 0, 0) = (1, 0, 0) = x̂
α2
El campo eléctrico es entonces
k

~ = E0 x̂ej( √2 (y+z)−ωt)
E
El valor de k se determina volviendo a la ecuación de onda
2~
2~
2~
2~
~ − 1 ∂ E = ∂ E + ∂ E − 1 ∂ E = 0 =⇒ − k − k + ω = 0 =⇒ k = ω
∇2 E
c2 ∂t2
∂y 2
∂z 2
c2 ∂t2
c2
c
~ puede ser determinado como
Finalmente el campo magnético B
k

j( √ (y+z)−ωt)
~
k̂ × E
E0
(ŷ + ẑ) × E0 x̂e 2
j( √k (y+z)−ωt)
~
√
B=
= √ (ŷ − ẑ)e 2
=
c
c 2
c 2

En resumen como ω = 100πrad/s :
√
~ = E
√0 (ŷ − ẑ)ej100π( c 2 −t)
B
c 2

y+z

y+z

~ = E0 x̂ej100π( c√2 −t)
E

Rodrigo Chi - Marzo 2017

b) El vector de Poynting Promedio está dado por
~ =
h|S|i

1 ~ ~∗
E0
E02
E2
√ −t)
√ −t)
jω( y+z
−jω( y+z
c 2
√ |(ŷ+ẑ)| = 0
|E×B | =
E0 x̂e c 2 × √ (ŷ − ẑ)e
=
2µ0
2µ0
µ0 c
c 2
µ0 c 2

Solución 18.10

P X

a) Para determinar el vector de Poynting es necesario determinar el valor del campo magnético
~ Luego para el campo E~1 se tiene que
B.
x̂

ŷ

ẑ

~ ×E
~1 = ∂
∇
∂x

∂
∂y

∂
∂z

E10 cos(kx − ωt)

= E10 k sin(kx − ωt)ẑ

---

### Página 371

CAPÍTULO 18. LEYES DE MAXWELL
y dado que por Maxwell
~1
∂B
~ 1 (x, t) = E10 k cos(kx − ωt)ẑ = E10 cos(kx − ωt)ẑ
= −k sin(kx − ωt)ẑ =⇒ B
∂t
ω
c
~ 2 , por lo tanto por principio de superposición se
El cálculo es análogo para determinar B
tiene que
~ = [E10 cos(kx − ωt) + E20 cos(kx − ωt + φ)]ŷ
E
~ = 1 [E10 cos(kx − ωt) + E20 cos(kx − ωt + φ)]ẑ
B
c
Donde finalmente el vector de Poynting vale
~
~
~ = E × B = 1 [E10 cos(kx − ωt) + E20 cos(kx − ωt + φ)]2 x̂
S
µ0
cµ0
b) La intensidad de la onda está dada por
I = hSi =
T

ˆT

[E10 cos(kx − ωt) + E20 cos(kx − ωt + φ)]2 dt
cµ0

Antes de comenzar a trabajar la expresión debe usarse el hecho que
ˆT
cos2 (kx − ωt + φ) =

Por lo tanto


1  2
I=
E10
cµ0 T

ˆT

ˆT

cos

(kx − ωt + φ)dt + E20

cos2 (kx − ωt)dt

ˆT



cos (kx − ωt + φ) cos (kx − ωt)dt

+2E10 E20









1 
E2
E2
2E10 E20
 10 + 20 +
=

cµ0  2
T


ˆT




cos (kx − ωt + φ) cos (kx − ωt)dt



|
{z
}
J

Problemas Propuestos y Resueltos de Electromagnetismo

T

---

### Página 372

CAPÍTULO 18. LEYES DE MAXWELL
Para la última integral se tiene que
J=
T

ˆT
cos (kx − ωt + φ) cos (kx − ωt)dt

=
T

ˆT
[cos (kx − ωt) cos φ − sin (kx − ωt) sin φ] cos (kx − ωt)dt

cos φ
=
T

ˆT

sin φ
cos (kx − ωt)dt +
T

=

ˆT

cos (kx − ωt) sin (kx − ωt)dt

cos φ sin φ
+
2T

ˆT
sin (2(kx − ωt))dt

cos φ
Finalmente la intensidad vale
=

"

#

1 E10
E2
I=
+ 20 + E10 E20 cos φ
cµ0 2

c) Repitiendo nuevamente los cálculos de parte anterior se tiene que el campo magnético
~ 1 se mantiene, mientras tanto el campo asociado a E
~ 2 vale
asociado a E
x̂

ŷ

ẑ

~ ×E
~2 = ∂
∇
∂x

∂
∂y

∂
∂z

E20 cos(kx + ωt + φ)

= E20 k sin(kx + ωt)ẑ

Rodrigo Chi - Marzo 2017

Nuevamente por Maxwell,
~2
∂B
~ 2 (x, t) = − E20 cos(kx + ωt + φ)ẑ
= −E20 k sin(kx + ωt + φ)ẑ =⇒ B
∂t
c
donde se tiene que
~ = [E10 cos(kx − ωt) + E20 cos(kx + ωt + φ)]ŷ
E
~ = 1 [E10 cos(kx − ωt) − E20 cos(kx + ωt + φ)]ẑ
B
c
lo que implica que en este caso
~ = 1 [E10
S
cos2 (kx − ωt) − E20
cos2 (kx + ωt + φ)]x̂
cµ0
Por lo que la intensidad de la onda vale
I=
T

ˆT

"

1 E10
E2
[E10
cos2 (kx − ωt) − E20
cos2 (kx + ωt + φ)]dt =
− 20
cµ0
cµ0 2

#

---

### Página 373

CAPÍTULO 18. LEYES DE MAXWELL
Solución 18.11

P X

~ =E
~ 0 ej(~k·~r−ωt) , luego como ~k · ~r = (0, 0, k) ·
a) Como el campo eléctrico es de la forma E
(x, y, z) = kz lo que entrega que
~ − µ0 g
∇2 E

~
∂E
~ 0 ej(kz−ωt) + µ0 gjω E
~ 0 ej(kz−ωt) = 0
= −k 2 E
∂t

Esto implica que
k 2 = µ0 gjω =⇒ k =

q

µ0 gjω

Pero por otro lado se tiene que
q

π

π
(1 + j)
π
+ j sin = √

π

j = (ej 2 ) 2 = ej 4 = cos

Por lo que se demuestra que
r

k = (1 + j)

µ0 gω

~ se usa el hecho que
b) Para encontrar el valor de B

Nótese que el conductor agrego un desfase del campo magnético con respecto al eléctrico
y adicionalmente una exponencial real decreciente (ie. la onda va perdiendo energía dentro
del material debido a las corrientes que provoca el campo eléctrico).
c) Finalmente, el vector de Poynting promedio está dado por
~ ×H
~ ∗}
Re{E
√
(
)
k0 E0 2 −k0 z −j(k0 z−ωt+ π )
−k0 z j(k0 z−ωt)
4 ŷ
= Re E0 e
e
x̂ ×
e
e
ωµ0
√
π
k0 E02 2 −2k0 z
=
e
ẑ Re{e−j 4 }
2µ0 ω
k0 E02 −2k0 z
=
e
ẑ
2µ0 ω

~ =
hSi

Problemas Propuestos y Resueltos de Electromagnetismo

j(kz−ωt)
~ ~
x̂
(1 + j)k0 E0 j(kz−ωt)
~ = k × E = (1 + j)k0 ẑ × E0 e
B
=
e
ŷ
ω
ω
ω
√ π
Como 1 + j = 2ej 4 y k = (1 + j)k0 el campo magnético puede ser reescrito como
√
k
E
2 −k0 z j(k0 z−ωt+ π )
~ =
4 ŷ
B
e
e
ω

---

### Página 374

CAPÍTULO 18. LEYES DE MAXWELL

IV.

Indicaciones Problemas Sin Solución

Indicación 18.2

P X

~ 0 suponiendo que la dependencia del tiempo no existiese.
Determine el valor de E
~ 1 (t). Recuerde que el campo magnético rota
Usando la Ley de Ampère-Maxwell determine B
~ 1 = B1 (r, t)θ̂.
en alrededor del campo eléctrico, en este caso B
~ 2 (t) inducido a partir de B
~ 1.
Usando la ley de Faraday, determine el campo eléctrico E
Recuerde que este campo eléctrico apunta en la dirección ẑ.

Indicación 18.5

P X

A partir de la forma general de onda onda electromagnética identifique en primera instancia
los valores de k y ω. A partir de ello, es directo identificar λ y T .
Recuerde el dirección y sentido de la propagación está dada por ~k.
~ yS
~ es directo a partir del campo eléctrico.
Tanto la determinación de B

Indicación 18.7

P X

Rodrigo Chi - Marzo 2017

√
Note que el enunciado está diciendo que k̂ = x̂+ŷ
y que n̂ = x̂. Con esto debería ser
~
~
~
suficiente para encontrar E, B y S.

Recuerde que en una onda que viaja en el vacío siempre se cumple que |~k| = ωc donde c es
la velocidad de la luz.

Indicación 18.8

P X

Identifique la dirección de la onda electromagnética y determine en forma directa cuanto es
~
el valor de B.
Evalúe φ pedido junto con las condiciones de los módulos. Recuerde que la funciones reales
de las ondas electromagnéticas están dadas por su parte real.
Note que la polarización del campo eléctrico y magnético cambia con la posición y el tiempo.
¿Qué tipo de polarización sigue la onda?¿Lineal, Circular o Elípica?

---

### Página 375

CAPÍTULO 18. LEYES DE MAXWELL
Indicación 18.9

P X

Evalué magnético dado en la Ley de Faraday (forma diferencial) y determine el campo
eléctrico pedido.

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 376

CAPÍTULO 18. LEYES DE MAXWELL

V.

Respuestas
Problema

Respuestas

P

18.1

ab
a) ε = − µ04d
(g V̇ (t) + ε0 V̈ (t)), caso particular ε = 0

~ = − rV (t)
b) S
2d2 (gV (t) + ε0 V̇ (t))r̂
~ 0 = − V0 cos ωt ẑ (z crece de la placa inferior a la superior)
a) E
d

P

~ 1 = µ0 ε0 V0 ω sin ωtθ̂
b) B
2d
18.2



~ 2 = µ0 V0 ε0 ω2 cos ωt r2 − a2 ẑ
c) E
4d
h

i
~ = − V0 cos ωt 1 + ω2 µ0 ε0 a2 − r2 ẑ
d) E
d
a) |S| ≈ 1350 mW2

P

18.4

b) U ≈ 8,6 kWh .
c) 0,22 m2 , para 6 millones 1,32 km2 .

P

18.5

−9
a) λ = π5 m y T = 2π
s.
3 · 10

b) La onda se propaga en −x̂.
y+z

~ = E0 x̂ej100π( c√2 −t)
a) E

P

y+z

18.6

~ = E√0 (ŷ − ẑ)ej100π( c√2 −t)
B
c 2
~ = E02
b) h|S|i
µ0 c

Rodrigo Chi - Marzo 2017

ω
~ = E0 x̂−ŷ
√ cos( √
a) E
(x + y) − ωt)
c 2

P

18.7

ω
~ = − E0 ẑ cos( √
B
(x + y) − ωt)
c
c 2
E2

~ = 0
b) h|S|i
2µ0 c

---

### Página 377

CAPÍTULO 18. LEYES DE MAXWELL
Problema

Respuestas
~ = E1 ej(kz−ωt) ŷ − E2 ej(kz−ωt−φ) x̂, hSi = 1 (E 2 + E 2 )ẑ
a) B
c
c
cµ0

P

18.8

~ = E0 (cos(kz − ωt)x̂ + sin(kz − ωt)ŷ) y B
~ = E0 (cos(kz − ωt)ŷ − sin(kz − ωt)x̂)
b) E
c
c) La onda esta polarizada circularmente.

P

P

P

18.9

18.10

~ = − aB0 ω sin
E
π



sin (kz − ωt) ŷ

~ = 1 [E10 cos(kx − ωt) + E20 cos(kx − ωt + φ)]2 x̂
a) S
cµ0
h 2
i
E
E2
b) I = cµ10 210 + 220 + E10 E20 cos φ
h 2
i
E
E2
c) I = cµ10 210 − 220
~ = E0 k0
b) B
ω

18.11

πx
a

√

π

2e−k0 z ej(k0 z−ωt+ 4 )

~ = E02 k0 e−2k0 z
c) h|S|i
2µ0 ω

Problemas Propuestos y Resueltos de Electromagnetismo

---

### Página 378

Rodrigo Chi - Marzo 2017

CAPÍTULO 18. LEYES DE MAXWELL

---

### Página 379

Apéndice

Herramientas Matemáticas
~yB
~ campo vectoriales y f un campo escalar.
Sean A

Triple Producto

~ × (B
~ × C)
~ = B(
~ A
~ · C)
~ − C(
~ A
~ · B)
~
A
~ · (B
~ × C)
~ =B
~ · (C
~ × A)
~ =C
~ · (A
~ × B)
~
A

~ A
~ · B)
~ = (A
~ · ∇)
~ B
~ + (B
~ · ∇)
~ A
~+A
~ × (∇
~ × B)
~ +B
~ × (∇
~ × A)
~
∇(
~ · (f A)
~ = f∇
~ ·A
~+A
~ · ∇f
~
∇
~ · (A
~ × B)
~ =B
~ · (∇
~ × A)
~ +A
~ · (∇
~ × B)
~
∇
~ × (A
~ × B)
~ =A
~∇
~ ·B
~ −B
~∇
~ ·A
~ + (B
~ · ∇)
~ A
~ − (A
~ · ∇)
~ B
~
∇

Segundas Derivadas

~ × (∇
~ × A)
~ = ∇(
~ ∇
~ · A)
~ − ∇2 A
~
∇
~ · (∇
~ × A)
~ =0
∇

Problemas Propuestos y Resueltos de Electromagnetismo

Reglas del Producto

---

### Página 380

CAPÍTULO 18. LEYES DE MAXWELL

Coordenadas Esféricas

z

r

θ
P

y
φ

x
Figura 18.2: Coordenadas esféricas

1 ∂f
1 ∂f
∂f
r̂ +
θ̂ +
ϕ̂
∂r
r ∂θ
r sin θ ∂ϕ


~ ·A
~ = 1 ∂ r2 Ar + 1 ∂ (sin θAθ ) + 1 ∂Aϕ
∇
r2 ∂r
r sin θ ∂θ
r sin θ ∂ϕ
!
∂
∂Aθ
~ ×A
~= 1
(sin θAϕ ) −
r̂
∇
r sin θ ∂θ
∂ϕ
!
1 ∂Ar
∂
+
−
(rAϕ ) θ̂
r sin θ ∂ϕ
∂r
!
1 ∂
∂Ar
+
(rAθ ) −
ϕ̂
r ∂r
∂θ
!
!
1 ∂
∂
∂f
2 ∂f
∇f= 2
r
+ 2
sin θ
r ∂r
∂r
r sin θ ∂θ
∂θ
∂ 2f
+ 2 2
r sin θ ∂ϕ2

Rodrigo Chi - Marzo 2017

∇f =

Diferenciales:
~ = drr̂ + rdθθ̂ + r sin θdϕϕ̂
dl
~ = r2 sin θdθdϕr̂ + r sin θdrdϕθ̂ + rdrdθϕ̂
dS
dV = r2 sin θdrdθdϕ

---

### Página 381

CAPÍTULO 18. LEYES DE MAXWELL

Coordenadas Cilíndricas

z

P

r
x

z

y

θ

Figura 18.3: Coordenadas cilíndricas

1 ∂f
∂f
∂f
r̂ +
θ̂ +
ẑ
∂r
r ∂θ
∂z
~ ·A
~ = 1 ∂ (rAr ) + 1 ∂Aθ + ∂Az
∇
r ∂r
r !∂θ
∂z
~ ×A
~ = 1 ∂Az − ∂Aθ r̂
∇
r ∂θ
∂z
!
∂Ar ∂Az
θ̂
+
−
∂z
∂r
!
1 ∂
∂Ar
+
(rAθ ) −
ẑ
r ∂r
∂θ
!
1 ∂
∂f
1 ∂ 2f
∂ 2f
∇f=
r
+ 2 2 + 2
r ∂r
∂r
r ∂θ
∂z
∇f =

~ = drr̂ + rdθθ̂ + z ẑ
dl
~ = rdθdzr̂ + drdz θ̂ + rdrdθẑ
dS
dV = rdrdθdz

Problemas Propuestos y Resueltos de Electromagnetismo

Diferenciales:

---

### Página 382

CAPÍTULO 18. LEYES DE MAXWELL

Notación usualmente usada
Magnitud Física

Símbolo

Unidades SI

Dimensiones

Capacidad
Carga

C
q

faradays (F)
coulomb (C)

s2 ·C 2
kg·m2

Conductividad
Intensidad de Corriente

g
I
~
D

siemens/metro (S/m)
ampére (A)
ampere/m

Densidad Volumétrica de Corriente

~
K
J~

ampere/m2

Campo Eléctrico

~
E

volt/metro

Fuerza Electromotriz (fem)

ε

volt (V)

Trabajo

W
F~

joule (J)

s·C 2
kg·m3
C
s
C
m2
C
s·m
C
s·m2
kg·m
s2 ·C
kg·m2
s2 ·C
kg·m2
s2
kg·m
s2
−1

Desplazamiento Eléctrico
Densidad Superficial de Corriente

Fuerza
Frecuencia

f

newton (N)
hertz (Hz)

Impedancia

Z

ohm (Ω)

Inductancia

L
~
H

henry (H)

Intensidad de Campo Magnético
Largo

`

ampere/metro
metro (m)

Φ
~
B

weber (Wb)
ampere-m2

Magnetización

m
~
~
M

ampere-vuelta/m

Permeabilidad

µ

henry/metro

Permitividad

faraday/metro

Polarización

ε
P~

Potencial Eléctrico

V

volt (V)

Potencia

watt (W)

Vector de Poynting

P
~
S

Resistencia

R

ohm (Ω)

Resistividad
Tiempo
Velocidad

η
t
~v

ohm-metros
segundos
metro/segundos

Flujo Magnético
Campo Magnético
Momento Magnético

Rodrigo Chi - Marzo 2017

coulomb/m2

tesla (T)

coulomb/m2

W/m2

C

s

kg·m2
s·C 2
kg·m2
C2
C
s·m

m
kg·m2
s·C
kg
s·C
m2 ·C
s
C
s·m
kg·m
C2
s ·C 2
kg·m3
C
m2
kg·m2
s2 ·C
kg·m2
s3
kg
s3
kg·m2
s·C 2
kg·m3
s·C 2

s
m
s

---

### Página 383

Bibliografía
[1] Barger, V., and Olsson, M. G. Classical electricity and magnetism: a contemporary
perspective. Allyn & Bacon, 1987.
[2] Cordero, P. Electromagnetismo. Editorial Universitaria, 2015.
[3] Dourmashkin, P., Liao, S.-B., and Winston Belcher, J. Introduction to electricity and magnetism. Pearson, 2013.
[4] Griffiths, D. J., and College, R. Introduction to electrodynamics, vol. 3. Prentice
Hall Upper Saddle River, NJ, 1999.
[5] Lim, Y.-K. Problems and solutions on quantum mechanics, vol. 6. World Scientific, 1998.
[6] Nayfeh, M. H., and Brussel, M. K. Electricity and magnetism. Courier Dover
Publications, 2015.

[8] Pollack, G. L., and Stump, D. R. Electromagnetism. Addison-Wesley, 2002.
[9] Purcell, E. M. Electricidad y magnetismo, vol. 2. Reverté, 1988.
[10] Rodríguez, V. L. Problemas resueltos de Electromagnetismo. Editorial Universitaria
Ramon Areces, 2003.
[11] Serway, R. A., Jewett, J. W., Pedroza, M. d. C. R., and López, E. F. Física
para ciencias e ingeniería, 7 ed., vol. 2. Cengage Learning Editores, 2015.

Problemas Propuestos y Resueltos de Electromagnetismo

[7] Núñez Cubero, F., López Pérez, E., et al. 100 problemas de electromagnetismo.
Alianza Editorial, 1997.
