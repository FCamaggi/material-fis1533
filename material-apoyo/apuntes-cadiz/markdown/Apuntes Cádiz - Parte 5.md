---
title: "Parte 5"
source_pdf: "Electro/material-apoyo/apuntes-cadiz/Apuntes Cádiz - Parte 5.pdf"
pages: 115
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Parte 5

### Página 1

Parte V
Magnetostática. Campos variantes en
el tiempo

---

### Página 2

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 3

#### Capítulo 12
Magnetostática
El campo Magnético
Hemos visto que las cargas estáticas son fuentes de campo eléctrico. Además conocemos una ley
que nos permite saber cómo es la fuerza que un campo eléctrico ejerce sobre una carga puntual
(Ley de Coulomb). Ahora, sucede que si dos cargas se están moviendo, existe una fuerza adicional entre ellas debido a éste movimiento. Ésta fuerza se conoce como Fuerza Magnética.
Sin embargo, la fuerza magnética entre 2 cargas puntuales en movimiento relativo es muchísimo
menos intensa que la fuerza de Coulomb, por lo que se hace prácticamente imposible medir la
fuerza magnética entre 2 cargas puntuales. De todas formas, efectos magnéticos se pueden
medir al utilizar corrientes eléctricas en conductores (donde existe un número muy grande de
electrones en movimiento!)
En resumen, cargas en movimiento generan campos magnéticos (y entonces una corriente
eléctrica también), y a su vez, campos magnéticos actúan sobre cargas en movimiento (en
consecuencia, un campo magnético ejerce una fuerza sobre un conductor con corriente).

Comenzaremos por el estudio de la Magnetostática, es decir, el estudio de campos magnéticos
producidos por corrientes estacionarias. Con esto queremos decir
I=

dq
=C
dt

Recordando la ecuación de continuidad de la carga
~ · J(~
~ x, t) + ∂ρ(~x, t) = 0
∇
∂t
La condición de que las corrientes sean estacionarias entrega
∂ρ(~x, t)
~ · J(~
~ x) = 0
=0→∇
∂t
Más adelante veremos como se relacionan los campos eléctrico y magnético, y encontraremos
las leyes fundamentales de la electrodinámica.

---

### Página 4

~ Esto se puede verificar
Un imán permanente es una fuente natural de campo magnético B.
al mover un compás cerca de un imán, la aguja del compás se alineará en la dirección del campo
magnético producido por el imán, como se ve en la figura

Es decir, el efecto del imán sobre la aguja es el de un torque (Torque de Ampère). Una
barra magnética consiste de dos polos, que se designan como norte (N) y sur (S). Esto significa
que las líneas de campo emergen desde un polo (norte) y terminan en el opuesto (sur). Veremos
que los campos magnéticos siempre tienen esta característica, es decir, las líneas de campo
magnético siempre emergen y terminan en la misma fuente del campo. (No se han encontrado
monopolos magnéticos). Cuando se acercan 2 barras magnéticas, 2 polos iguales se repelen,
mientras que polos contrarios se atraerán

Al contrario de las cargas eléctricas, las cuales pueden estar aisladas, los 2 polos magnéticos
siempre vienen en pares. Cuando se quiebra un imán, se obtienen 2 nuevos imanes, cada uno
con polo norte y sur. En otras palabras, no existen monopolos magnéticos aislados

Se verá más adelante que éste resultado se resume en la tercera ecuación de Maxwell
~ · B(~
~ x) = 0
∇
Podría resultar, en principio, misterioso que un material genere campos magnéticos. Lo
único que hemos dicho es que cargas en movimiento generan campos magnéticos. Es sabido que
una de las fuerzas fundamentales que dan forma a los átomos es la fuerza eléctrica (que atrae
al electrón con el protón). El movimiento de electrones en un material genera entonces campos
magnéticos. En realidad, tener la visión de un electrón como una partícula que gira en torno al
núcleo no es muy correcto, lo que se debe usar a niveles atómicos es la Mecánica Cuántica. El
magnetismo en la materia es en general un fenómeno puramente cuántico y que tiene relación
con el espín del electron. Al igual que en electrostática vimos que las moléculas de un material
dieléctrico son levemente polarizadas ante la presencia de un campo eléctrico, y que entonces un
material se caracteriza por una suma de infinitos momentos dipolares, también se puede definir
un análogo magnético, el momento magnético. De todas formas, es algo que está presente en
todos los átomos. ¿Por qué entonces, no toda la materia presenta esta cualidad de generar un
campo magnético medible, como los objetos que hemos llamado imanes permanentes?. La respuesta es que, si bien cada átomo en un material contribuye generando un campo magnético, la

---

### Página 5

disposición de los momentos magnéticos puede ser tan aleatoria, que el efecto neto al sumarlos
es una cancelación de un campo magnético total. Los imanes son materiales cuyos momentos
magnéticos están todos alineados, y por esto es que cada uno contribuye del mismo modo a un
campo magnético total que es el que medimos en la cercanía de un imán.

12.1.

Fuerza magnética sobre una carga puntual

Aún no hemos establecido una expresión matemática para determinar el campo magnético
generado por una distribución de cargas en movimiento. Sin embargo, por el momento po~ x), en cierta región del espacio.
dremos asumir que simplemente existe un campo magnético, B(~
Estudiaremos primero cual es el efecto de un campo magnético sobre una carga puntual q en
movimiento, más adelante veremos cómo son creados los campos magnéticos. Consideremos una
partícula de carga q, que se mueve con cierta velocidad ~v (~x). Experimentalmente, se obtienen
las siguientes observaciones
1. La magnitud de la fuerza magnética F~B (~x) ejercida sobre la partícula cargada es proporcional a | ~v (~x) | y a q
~ x)
2. La magnitud y dirección de F~B (~x) depende de ~v (~x) y de B(~
~ x). Sin embargo, cuando
3. La fuerza magnética F~B (~x) desaparece cuando ~v (~x) es paralela a B(~
~ x), la dirección de F~B (~x) es perpendicular al plano formado por
~v (~x) forma un ángulo ϑ con B(~
~
~v (~x) y B(~x), y la magnitud de F~B (~x) es proporcional a sin ϑ
4. Cuando la carga cambia de signo, la dirección de la fuerza magnética se invierte

Todas las observaciones anteriores se pueden resumir en la siguiente expresión
~ x)
F~B (~x) = q~v (~x) × B(~

La magnitud de F~B (~x) está dada por

FB = |q|vB sin θ

~ x) es el tesla T = 1 N/Am. Notar que F~B (~x) es siempre perpenLa unidad en SI para B(~
~ x), de forma que una fuerza magnética no puede alterar la rapidez de la
dicular a ~v (~x) y B(~
particula. (No realiza trabajo sobre ella). En efecto


~ x)) · ~v (~x)dt = q(~v (~x) × ~v (~x)) · B(~
~ x) dt = 0
dW (~x) = F~B (~x) · d~x = q(~v (~x) × B(~

Si sobre la partícula sólo actúa una fuerza magnética, entonces el trabajo sobre ella es nulo,
y entonces su energía cinética es constante. (Luego el módulo de la velocidad es constante). Sin

---

### Página 6

embargo,la dirección de ~v (~x), sí puede ser alterada por la fuerza magnética. (De lo contrario, el
movimiento de una carga en un campo magnético sería extremadamente aburrido, simplemente
se movería en una línea recta)

12.2.

Movimiento de una carga en un campo eléctrico y
magnético uniforme

Una partícula de carga q se podría encontrar en una región del espacio en donde existen un
~ y un campo eléctrico E.
~ Así, sobre ella actuará una fuerza neta igual a
campo magnético B


~ + ~v × B
~
F~ = q E

esta es llamada fuerza de Lorentz . Ésto permite acoplar el electromagnetismo clásico con
la mecánica, en efecto, la trayectoria de la partícula es la solución de la segunda ley de Newton


d~p
~ + ~v × B
~
=q E
dt
Resolvamos el movimiento de una partícula sometida a la fuerza de Lorentz, en un caso
muy particular y sencillo, como se muestra en la siguiente figura

~ = E î, B
~ = B k̂. Se debe resolver
Es decir, se tienen dos campos uniformes y perpendiculares E


d~v
~ + ~v × B
~
=q E
dt

q 
d~v
E î + ~v × B k̂
=
dt
m
m

La velocidad de la partícula es, simplemente
~v = ẋî + ẏ ĵ + ż k̂
de forma que

q 
d
E î − ẋB ĵ + ẏB î
~v =
dt
m

---

### Página 7

De aquí se obtienen las siguientes ecuaciones diferenciales que describen el movimiento de
la partícula
z̈ = 0
qB
ÿ = − ẋ
m


qE
+ ẏB
ẍ =
m
Definiendo qB
= w0 y qE
= w1
m
m

z̈ = 0
ÿ = −w0 ẋ
ẍ = w1 + w0 ẏ

La solución de la primera de ellas es evidente, y está dada por
z(t) = z0 + voz t
es decir, la partícula describe un movimiento uniforme en la dirección z . Las ecuaciones
para la velocidad en x y en y están acopladas, y pueden ser escritas de forma matricial como
  
   
d ẏ
0 −w0
ẏ
=
+
ẋ
w
ẋ
w
dt
Es decir, se tiene un sistema de ecuaciones diferenciales no homogéneo de la forma
~x˙ = A~x + f~
Puede ser resuelto fácilmente de la siguiente manera
~x˙ − A~x = f~
e−At~x˙ − e−At A~x = e−At f~ =
entonces
−At

e

~x = ~x0 +

ˆ t

d −At 
e ~x
dt

dτ e−Aτ f~(τ )

Finalmente
At

~x = e ~x0 +

ˆ t

dτ eA(t−τ ) f~(τ )

La solución homogénea es, simplemente
~xh = eAt~x0
donde x0 corresponde a ~x(t = 0). Para calcular eAt obtenemos los valores propios de A
| A − λI |=

−λ −w0
= λ2 + w02 = 0
w0 −λ

---

### Página 8

Están dados por
λ1 = iw0 , λ2 = −iw0

Para encontrar eAt se puede utilizar el teorema de Caley-Hamilton ( o simplemente diagonalizar A)
eAt = a0 I + a1 A
donde a0 y a1 están dados por
eiw0 t = a0 + iw0 a1
e−iw0 t = a0 − iw0 a1
Resolviendo
a0 = cos w0 t
a1 =
sin w0 t
w0
Con esto
At

e

=



 

− sin w0 t
cos w0 t
+
cos w0 t
sin w0 t


cos w0 t − sin w0 t
eAt =
sin w0 t cos w0 t

y la solución homogénea queda
  

v0y cos w0 t − v0x sin w0 t
ẏ
=
~xh (t) =
ẋ
v0y sin w0 t + v0x cos w0 t

Además, la solución particular toma la forma
 
ˆ t 
cos w0 (t − τ ) − sin w0 (t − τ )
dτ
~xp (t) =
sin
w
(t
−
τ
)
cos
w
(t
−
τ
)
w



ˆ t 
t
w1 cos w0 (t − τ )
w1 sin w0 (t − τ )
=
dτ
~xp (t) =
w1 cos w0 (t − τ )
w0 − sin w0 (t − τ ) 0


w1 1 − cos w0 t
~xp (t) =
sin w0 t
w0

Finalmente, se tiene

ẋ = v0y sin w0 t + v0x cos w0 t +
ẏ = v0y cos w0 t − v0x sin w0 t +

w1
sin w0 t
w0

w1
(1 − cos w0 t)
w0

---

### Página 9

Integrando, se obtiene la cinemática general para la partícula
v0y
v0y w1
v0x
w1
x(t) = −
cos w0 t +
sin w0 t − 2 cos w0 t +
+ 2 + x0
w0
w0
w0
w0
w0


v0y
v0x
w1
v0x
t−
y(t) =
sin w0 t +
cos w0 t +
sin w0 t −
+ y0
w0
w0
w0
w0
w0
z(t) = z0 + v0z t

12.2.1.

Trayectorias en casos particulares

Resuelta la ecuación de movimiento para la carga sometida a la fuerza de Lorentz, es posible
graficar y obtener su trayectoria para distintas condiciones iniciales y magnitudes de los campos.
La siguiente figura muestra una solución con q = 10 C, B = 110 T, E = 200 N/C, y x0 = y0 =
z0 = 0 (partícula que parte del origen)

Solución con velocidad inicial en z distinta de cero
El movimiento en la dirección vertical (eje z) es uniforme. Notar que la partícula tiene una
cierta velocidad de traslación en la dirección y, y no en la dirección x (dirección del campo
eléctrico), como se podría pensar. La razón se debe a que si bien el campo eléctrico ejerce una
fuerza según x con un incremento en la velocidad, ambos efectos se traducen en una fuerza
~ intensa en la dirección y. El efecto neto es una traslación general en dicha
magnética q~v × B
dirección

Misma solución anterior, ahora con velocidad inicial en x de 1 m/s

Trayectoria con velocidad inicial en y de 1 m/s

---

### Página 10

Ahora, ¿qué ocurre si el campo eléctrico es nulo?. Las soluciones quedan de la forma
x(t) = −
y(t) =

v0y
v0x
v0y
cos w0 t +
sin w0 t +
+ x0
w0
w0
w0

v0y
v0x
v0x
sin w0 t +
cos w0 t −
+ y0
w0
w0
w0
z(t) = z0 + v0z t

La partícula describe un movimiento circular en el plano x − y (¿cuál sería el centro?),
como se muestra en la figura

Este movimiento tiene una frecuencia angular de oscilación (constante) dada por
qB
m
En particular, si la velocidad inicial en la dirección z es nula, la trayectoria es definitivamente
una circunferencia en el espacio
w0 =

Así, una partícula en un campo magnético uniforme describe una trayectoria circular en el
plano perpendicular al campo magnético. Este movimiento circular es uniforme (frecuencia
angular constante). Esto último es evidente pues el campo magnético nunca realiza trabajo sobre
la partícula (y no modifica su energía cinética). Si v es el módulo de la velocidad, entonces se
tiene
v = w0 R
y el radio de la circunferencia descrita está dado por
R=

mv
v
=
qB
w0

El período de este movimiento circular estará dado por
T =

2π
2πm
=
w0
qB

---

### Página 11

Trayectoria general de una partícula en un campo magnético uniforme
Hay que notar que estas trayectorias han sido obtenidas a partir de campos extremadamente sencillos (uniformes). Muchísimos efectos interesantes se pueden lograr con campos que
varían en el espacio. Uno de ellos consiste en un campo magnético con curvatura en que bajo
ciertas condiciones se puede confinar a la partícula en determinadas regiones del espacio (espejos magnéticos). El confinamiento magnético parece ser la solución con más posibilidades
de permitir en el futuro la construcción de un reactor de fusión nuclear de potencia con fines
comerciales, la idea consiste en confinar un plasma a altas temperaturas lejos de las paredes
del reactor, de forma de poder replicar procesos de fusión nuclear (por ejemplo, la fusión de
Deuterio-Tritio)

Diseño de confinamiento de plasma utilizado en el International Thermonuclear Experimental
Reactor (ITER), en Francia

---

### Página 12

12.2.2.

El descubrimiento del electrón

Notar que existe una solución muy particular al movimiento de una partícula bajo la acción
de la fuerza de Lorentz cuando los campos son uniformes y perpendiculares. Resulta muy
interesante que para un determinado valor de la velocidad ~v una partícula cargada no siente
fuerza alguna. En efecto, supongamos una partícula cargada que ingresa a una región con
~ y un campo magnético B,
~ si la velocidad inicial de tal
prescencia de un campo eléctrico E,
partícula es
1 ~
~
~v = 2 E
×B
B
entonces su trayectoria será una línea recta, con velocidad constante y en la dirección de ~v .
Esto es fácil de demostrar, pues la fuerza de Lorentz que actúa sobre la carga es




~ + ~v × B
~ =q E
~+
~ × B)
~ ×B
~
F~ = q E
(E
B2




1 2~
1 ~
~
~
~
~
~
F = q E − 2 B × (E × B) = q E − 2 B E = ~0
B
B
Este fue el principio utilizado por JJ Thompson para medir la razón entre la carga y la
masa del electrón

Aparato de Thompson para estudiar la deflexión de partículas cargadas
La palabra átomo (que significa indivisible en Griego) fue propuesta por Demócrito, quien
vivió en Atenas (460-370 ac). El consideraba inconcebible que los objetos materiales pudiesen
ser divididos en partes cada vez más pequeñas, sin límite, y postuló la existencia de partículas
elementales, tan pequeñas que no son posibles dividirlas en partes más pequeñas. El distinguió cuatro tipos de átomos, y propuso que toda la materia está conformada por estos objetos
indivisibles. Hoy en día, la idea de Demócrito es transferida a partículas más pequeñas aún,
que constituyen la estructura interna de los átomos, y se espera que los electrones, protones, y
las demás partículas elementales sean realmente indivisibles.
Hacia el siglo 19, la atención de muchos físicos fue puesta en el paso de la electricidad a
través de los gases. Se sabía que los gases, siendo muy buenos aislantes eléctricos, a veces podían
conducir electricidad al ser sometidos a tensiones muy altas. Sin embargo, Sir Williams Crookes
mostró que el paso de la electricidad en gases tomaba una forma muy clara (en efecto, se ven
haces de luz) cuando la presión del gas es reducida a una pequeña fracción de una atmósfera

---

### Página 13

Los tubos de Crookes emitían luz de determinado color dependiendo de la naturaleza del
gas, y ellos aún brillan en las calles y ciudades de todo el mundo

Tubo de Crooke. Éste consiste de un ánodo y un cátodo entre los cuales se establece una
diferencia de potencial, al interior se tiene gas a baja presión
Al colocar un imán cerca del tubo, Crookes observó la deflección de estos rayos catódicos, tal
cual sucede con las partículas cargadas. Al mismo tiempo, Jean Perrin en Francia descubrió que
al colocar una placa metálica en el camino del haz, ésta adquiría una carga eléctrica negativa.
Todo esto parecía indicar que estos rayos se trataban de partículas cargadas negativamente
moviéndose a través del gas. Sin embargo, esta idea eran opuestas a las observaciones del físico
Philipp Lenard, quien habría encontrado que los rayos catódicos eran capaces de traspasar
varias pantallas puestas en su camino sin dejar agujeros en ellas. Lenard pensaba que sólo
ondas, y no un haz de partículas, podría hacer esto. La tarea de resolver estas contradicciones
experimentales, y probar que los rayos catódicos son en efecto un haz de partículas, y encontrar
las características físicas de éstas particulas, le fue dada a Joseph John Thompson por el Consejo
Supremo del progreso de la ciencia. Thompson fue un físico nacido en Manchester, que a los 40
años era director del famoso laboratorio de Cavendish en Cambridge. Asumiendo que los rayos
catódicos son partículas moviendose a alta velocidad, Thompson decidió medir su masa y su
carga, y una parte de esta investigación consistió en observar la deflexión de rayos catódicos en
un campo magnético

Los electrones con carga −e y masa m son emitidos del cátodo C y acelerados hacia A. Sea
la diferencia de potencial entre C y A ∆V = φa − φc . El cambio en la energía potencial del
electrón es igual al trabajo externo realizado para acelerarlo, por conservación de energía, la
energía cinética adquirida está dada por
1 2
mv = e∆V
y entonces la velocidad que adquieren los electrones al pasar por A es
v=

r

2e∆V
m

---

### Página 14

A continuación los electrones entran en una región donde existe un campo eléctrico (hacia
abajo en la figura), y un campo magnético perpendicular (hacia adentro de la hoja). Si las
partículas ingresan con velocidad
1 ~
~ = E î
E×B
B
B
se moverán en una línea recta, y pasarán por un agujero (en rojo) al final del selector de
velocidades. Así, se ajusta el valor de ∆V , E y B de forma que las partículas sean detectadas
al final del selector de velocidades. Cuando esto sucede, se obtiene
~v =

e
E2
=
m
2∆V B 2
Al medir E, B y ∆V , se obtiene la razón entre la carga y la masa del electrón. Esta es
aproximadamente
e
= 1,7588 × 1011 C/kg
m

Sir J.J. Thompson y sus aparatos
En esa fecha el valor de e habría sido obtenido experimentalmente gracias a los experimentos de electrólisis de líquidos de Faraday. De todas formas Thompson realizó un experimento
especial para medir la carga con gases ionizados. Este método se basó en el descubrimiento de
otro físico del laboratorio Cavendish, C.T.R Wilson. Gracias a esto Thompson logró medir el
valor de m, usando sus resultados para e/m, obteniendo
m = 9, 11 × 10−31 kg
y esta resultó ser 1840 veces más pequeña que la masa del átomo de Hidrógeno. Ésto fue un
gran descubrimiento, una partícula aproximadamente 2 mil veces más liviana que el átomo más
liviano! Thompson concluyó que las partículas que conforman los rayos catódicos eran cargas
eléctricas, y les llamó electrones. El visualizó el átomo como una esfera de un material masivo
cargado positivamente, con pequeños electrones esparcidos estáticamente a través del núcleo

---

### Página 15

Placa conmemorativa en Cambridge acerca del descubrimiento del electrón. Cortesía de mi
amigo Germán Vogel

Fig. 12.1: Joseph John Thompson
Joseph John Thompson(1856-1940) Físico Inglés. En 1870 estudió Ingeniería en la
Universidad de Manchester, y se trasladó a Trinity College de Cambridge en 1876. En 1884 se
convirtió en profesor de Física en Cavendish. Uno de sus alumnos fue Ernest Rutherford, quién
más tarde sería su sucesor en el puesto. Obtuvo el Premio Nobel en 1906, en reconocimiento
de los grandes méritos de sus investigaciones teóricas y experimentales en la conducción de la
electricidad generada por los gases. Fue nombrado caballero en 1908 y nombrado en la Orden
del Mérito en 1912. En 1918 fue nombrado Rector del Trinity College de Cambridge, donde
permaneció hasta su muerte.

---

### Página 16

12.3.

Ley de Biot-Savart

Hemos descrito rápidamente la fuerza que se ejerce sobre una partícula cargada en un campo
magnético. Experimentalmente, resulta mucho más accesible estudiar que ocurre cuando se
acercan dos conductores rígidos (es decir, son mantenidos en su posición) con corriente (dado
que en ellos hay muchísimos electrones en movimiento, los efectos magnéticos ser amplifican).
Consideremos una curva Γ en el espacio, que representa un conductor lineal que lleva una
corriente I. Vamos a recorrer esta curva en el sentido de la corriente. En el punto ~x ∈ Γ,
definimos un elemento de corriente infinitesimal dado por
~ x) = Id~x
dI(~
donde I es la magnitud de la corriente (es una constante) y d~x es el elemento de línea sobre la
curva Γ (Insisto en que su dirección apunta en el sentido de la corriente) .
Sean dos circuitos lineales, Γ1 y Γ2 , con corrientes I1 e I2 , respectivamente. Ambas curvas
serán parametrizadas de forma de ser recorridas en el sentido de sus respectivas corrientes

Tomamos un elemento de corriente en ~x0 sobre el circuito 1, y un elemento de corriente en ~x
sobre el circuito 2. La fuerza que ejerce el elemento de corriente 1 sobre el elemento de corriente
2 está dada por


µ0 I1 d~x0 × (~x − ~x0 )
~
dF2 (~x) = I2 d~x ×
4π
| ~x − ~x0 |3

donde µo = 4π10−7 (H/m) es la permeabilidad del vacío. Notar que esta impresionante
expresión es mucho más compleja que la ley de Coulomb, primero que nada, implica 2 productos
vectoriales. Es importante notar además que la fuerza resultante ya no apunta necesariamente
en la dirección que une ambos elementos de línea (No es una fuerza Central). Lo que sí se sigue
cumpliendo es que la magnitud de la fuerza decae según el cuadrado de la distancia. Ahora bien,
podemos obtener la fuerza que ejerce todo el circuito 1 sobre el elemento de línea 2, utilizando
el principio de superposición, e integrando como sigue
˛
µ0 I1 d~x0 × (~x − ~x0 )
~
F2 = I2 d~x × (
)
| ~x − ~x0 |3
Γ1 4π
Finalmente, la fuerza total sobre el circuito 2 está dada por

˛
˛
I
µ
d~
x
×
(~
x
−
~
x
)
I2 d~x ×
F~2 =
| ~x − ~x0 |3
Γ2
Γ1 4π
µ0 I1 I2
F~2 =
4π

d~x × [d~x0 × (~x − ~x0 )]
| ~x − ~x0 |3
Γ1

˛ ˛
Γ2

---

### Página 17

Aparentemente esta fórmula presenta una asimetría y podría pensarse que no se satisface
la tercera ley de Newton. Sin embargo, se puede demostrar que esta ley es absolutamente
simétrica, de forma que
F~2 = −F~1
La demostración es la siguiente

[d~x · (~x − ~x0 )]d~x0 (d~x · d~x0 ) (~x − ~x0 )
d~x × [d~x0 × (~x − ~x0 )]
=
−
| ~x − ~x0 |3
| ~x − ~x0 |3
| ~x − ~x0 |3


d~x0 × [d~x × (~x − ~x0 )]
x − ~x0
0 ~
~
d~
x
·
∇
−
d~
x
·
d~
x
=
−d~
x
| ~x − ~x0 |3
| ~x − ~x0 |
| ~x − ~x0 |3
El término de la izquierda es una diferencial exacta, de forma que
˛
˛
˛ ˛
µ0 I1 I2
µ0 I1 I2
x − ~x0
0 ~
~
~
−
d~x
d~x · ∇
d~
x
·
d~
x
F2 = −
4π
| ~x − ~x0 |
4π
| ~x − ~x0 |3
Γ1
Γ2
Γ2 Γ1
˛ ˛
µ0 I1 I2
~x − ~x0
~
F2 =
d~x · d~x0
4π
| ~x − ~x0 |3
Γ2 Γ1
Hemos obtenido una identidad para la fuerza que ejerce el circuito 1 sobre el circuito 2 que
es totalmente simétrica. De aquí es evidente que
F1 = −F2

12.3.1.

Campo de un circuito rígido, Biot-Savart

Hemos concluído que la fuerza sobre el circuito 2 es
˛

˛
µ0 I1 d~x0 × (~x − ~x0 )
~
I2 d~x ×
F2 =
| ~x − ~x0 |3
Γ2
Γ1 4π

es fácil ver que la expresión entre paréntesis no depende en absoluto del circuito 2, es de
~ x),
hecho, un campo vectorial B(~
˛
~ x)
~
I2 d~x × B(~
F2 =
Γ2

~ ~x es el Campo Magnético en ~x debido a la corriente I1
B

Es decir

˛
I1 d~x0 × (~x − ~x0 )
µ0
~
B(~x) =
4π Γ1
| ~x − ~x0 |3
De esto podemos leer que el campo magnético en cualquier punto ~x debido a ésta corriente
~ x), de pequeños segmentos de
se puede calcular al sumar las contribuciones infinitesimales dB(~
conductor d~x

---

### Página 18

Esta es la ley de Biot-Savart, y da una expresión para la contribución al campo magnético
de un elemento de corriente Id~x
~ x) =
dB(~

µ0 I d~x0 × (~x − ~x0 )
4π
|~x − ~x0 |3

Fig. 12.2: Jean Baptiste Biot
Jean Baptiste Biot (1774-1862) Físico y matemático Francés. Estudió la polarización
de la luz cuando pasaba a través de soluciones químicas, y las relaciones entre la corriente
eléctrica y el magnetismo. La Ley de Biot-Savart describe como se genera el campo magnético
mediante una corriente estacionaria y se proporcionó el nombre gracias a su colaboración con
Félix Savart. Un cráter en la luna lleva su nombre en honor a sus contribuciones

12.4.

Fuerza sobre conductores de corriente

Habíamos obtenido que la fuerza sobre un circuito con corriente I2 es
F~2 =

˛

Γ2

~ x)
I2 d~x × B(~

~ x) es cualquier campo magnético externo
Donde B(~
Esto nos dice que para un conductor de forma arbitraria, la fuerza magnética se puede
obtener al sumar sobre las fuerzas actuando sobre pequeños segmentos que constituyen al
conductor. Sea un segmento diferencial denotado por d~x

---

### Página 19

Fig. 12.3: La figura ilustra el efecto de la fuerza magnética sobre conductores

Entonces la fuerza sobre un elemento infinitesimal de un conductor de carga es
~ x)
dF~B (~x) = Id~x × B(~
Anteriormente calculamos la fuerza sobre un conductor definido por una curva cerrada. Si
se desea encontrar la fuerza sobre un segmento de conductor entonces
ˆ b
~ x)
~
d~x × B(~
FB = I
a

donde a y b representan los extremos del conductor. Como ejemplo, consideremos un conductor
~ como se muestra
curvo que lleva corriente I y sumergido en un campo magnético uniforme B,
en la figura

Tenemos entonces que la fuerza sobre este conductor está dada por
ˆ b
~ x) = I (~xb − ~xa ) × B(~
~ x)
d~x) × B(~
F~B = I(
a

Notar que esto se debe a que el campo magnético es uniforme (sólo en este caso!). Sea ~l = ~xb −~xa
el vector dirigido desde a hacia b. Con esta notación
~
F~B = Id~l × B

---

### Página 20

Ahora veamos que sucede si el conductor constituye un circuito cerrado de forma arbitraria,
entonces la fuerza será
˛

~
~
FB = I
d~x × B
Γ

Pero

˛

d~x = ~0

Γ

La fuerza magnética neta sobre un circuito cerrado en un campo magnético uniforme es
~
FB = ~0

12.5.

Torque sobre una espira

Veamos qué sucede cuando colocamos una espira rectangular que lleva corriente estacionaria
~ x) = B î paralelo al
I en el plano XY , ante la prescencia de un campo magnético uniforme B(~
plano de la espira

Vemos que las fuerzas magnéticas actuando en los segmentos 1 y 3 son nulas debido a que los
~ . Por otro lado, las fuerzas
vectores ~l1 = −bî y ~l3 = bî son paralelos al campo magnético B
magnéticas actuando en los segmentos 2 y 4 son


F~2 = I −aĵ × B î = IaB k̂
 
~
F4 = I aĵ × B î = −IaB k̂

De aquí es claro que la fuerza neta es 0, algo que era de esperar por lo visto anteriormente.
Sin embargo, aun cuando la fuerza neta sobre la espira es nula, las fuerzas F~2 y F~4 producirán
un torque que genera una rotación de la espira con respecto al eje y. El torque con respecto al
centro de la espira es








~τc = −b/2î × F~2 + b/2î × F~4 = (−b/2)î × IaB k̂ + (b/2î) × −IaB k̂

---

### Página 21




IabB IabB
~τc =
+
ĵ = IabB ĵ = IAB ĵ
Donde A = ab representa el área de la espira. Es conveniente introducir el vector de área,
en este caso constante sobre la superficie limitada por la espira
~ = An̂
S
con n̂ el vector unitario en la dirección normal al plano de la espira. En este caso, tenemos
n̂ = k̂. La expresión para el torque se puede reescribir entonces como
~×B
~
~τ = I A

~ forma un
Consideremos ahora el caso más general donde la espira (o el vector de area S)
ángulo ϑ con respecto al campo magnético

De la figura

y el torque neto es


b
− sin ϑî + cos ϑk̂ = −~r4
~r2 =


b
τ̂c = ~r2 × F~2 + ~r4 × F~4 = 2~r2 × F~2 = 2 − sin ϑî + cos ϑk̂ × (IaB k̂)
~×B
~
τ̂c = IabB sin ϑĵ = I A

Se obtiene la misma expresión obtenida anteriormente. Notar que la magnitud del torque es
máxima cuando el vector normal a la espira es perpendicular al campo magnético. El torque es
nulo cuando la normal a la espira está orientada en la dirección paralela al campo magnético.
~ es, por definición, el momento magnético de la espira
El vector I A
~
~µ = I A

---

### Página 22

~ (perpendicular al plano de la espira).
La dirección de ~µ es la misma que el vector de área S
Con esto, el torque sobre una espira de corriente es
~
~τc = ~µ × B
Una espira en un campo magnético uniforme experimenta un torque hasta que su momento magnético esté completamente alineado con el campo magnético. Notar la analogía con el
torque que ejerce un campo eléctrico sobre un dipolo. En efecto, es posible definir un momento
magnético para una distribución general de corriente en el espacio. Así, cada átomo en un material estará caracterizado por un momento magnético, y el efecto de un campo magnético sobre
el material será el de alinear los momentos magnéticos de forma paralela al campo. Estos momentos magnéticos alineados (como sucede en un imán) también generarán un campo magnético

---

### Página 23

Problema
Considere el circuito cerrado de la figura que lleva una corriente I en el sentido contrario al
reloj. Un campo magnético uniforme apuntando en la dirección ĵ es aplicado. Encuentre la
fuerza magnética que actúa sobre el elemento rígido y el arco semicircular.

#### Solución
~ = B ĵ , llamemos F~1 y F~2 a las fuerzas actuando sobre
Tenemos un campo uniforme dado por B
el segmento rígido y la parte semicircular, respectivamente. La fuerza sobre el segmento rígido
es
ˆ R 
ˆ R 
~ × B ĵ = I
dx
F~1 = I
dx î × B ĵ = I2Rî × B ĵ = 2IRB k̂
−R

−R

Ahora, para calcular F~2 , notamos que elemento infinitesimal d~x en el semicírculo se puede
escribir como
d~x = dxêϕ = Rdϕ(− sin ϕî + cos ϕĵ)

~ es
La fuerza que actúa sobre un elemento dx


~ = IRdϕ − sin ϕî + cos ϕĵ × (B ĵ) = −IBRdϕ sin ϕk̂
dF~2 = Id~x × B

Integrando sobre el arco semicircular, tenemos
ˆ π
dϕ sin ϕ = −2IBRk̂
F~2 = −IBRk̂

Así, la fuerza neta que actúa sobre el circuito completo es

---

### Página 24

F~net = F~1 + F~2 = ~0
Consistente con el hecho de que la fuerza sobre un circuito cerrado en un campo magnético
uniforme es siempre nula

---

### Página 25

Problema
Un alambre delgado y rígido que lleva una corriente I es colocado a lo largo del eje x. Calcular
el campo magnético en el punto P . Analice el caso particular en que el alambre es simétrico
con respecto al eje y
¿Qué sucede cuando L → ∞?

#### Solución
Consideremos un elemento diferencial d~x0 = dxî que lleva una corriente I en la dirección x

Para calcular el campo magnético en el punto P utilizamos la ley de Biot-Savart. Según nuestra
elección del origen, se tiene ~x = a~j y ~x0 = xî. Así
~ x) =
dB(~

µ0 d~x0 × (~x − ~x0 )
I
4π
|~x − ~x0 |3

~x − ~x0 = aĵ − xî
y su magnitud es
|~x − ~x0 | =

√

a2 + x 2

Con esto, la contribución al campo queda
~ x) =
dB(~

µ0
I
4π

~ x) =
dB(~



dxî × aĵ − xî
(a2 + x2 )3/2

µ0
adxk̂
I 2
4π (a + x2 )3/2

Y el campo total en P será
~ ) = µ0 I
B(P
4π

ˆ L2

adxk̂
2 3/2
−L1 (a + x )

---

### Página 26

Notar además que
tan ϑ1 =

a
a
→ tan(−ϑ1 ) = −
→ −L1 = acot(−ϑ1 )
L1
L1

a
→ L2 = aϑ2
L2
Para resolver esta integral, utilizamos el siguiente gambito
tan ϑ2 =

x = actgϑ → dx = −a csc2 ϑdϑ
y la integral queda
~ = µ0 I
B
4π

ˆ ϑ2

dϑa(−a csc2 ϑ)k̂
2 3/2
−ϑ1 (a + a ctg ϑ)

Ahora nos comemos a la reina
ˆ ϑ2
ˆ ϑ2
µ0
−dϑ csc2 ϑk̂
µ0
~
B=
I
I
dϑ sin ϑk̂
=−
4πa −ϑ1 (1 + ctg 2 ϑ)3/2
4πa −ϑ1
~ = µ0 I (cos ϑ1 + cos ϑ2 ) k̂
B
4πa
En el caso simétrico en que ϑ2 = ϑ1 , y digamos que el largo total es 2L, entonces
cosϑ1 = √

L
L 2 + a2

y el campo es
~ = µ0 I √ L
k̂
B
2πa L2 + a2
De aquí es claro que si L → ∞, o , equivalentemente, θ1 → 0, θ2 → 0, el campo magnético
a una distancia a del conductor es
~ = µ0 I k̂
B
2πa
Notemos que en este límite, el sistema posee simetría cilíndrica, y las líneas de campo
magnético son circulares. Este resultado se comprobará más adelante con la ley de Ampère

---

### Página 27

Problema
Se lanza un electrón (carga -e) con velocidad inicial ~v en el medio de dos placas entre las cuales
~ constante (entrando a la hoja). Ignore todo efecto gravitacional
existe un campo mangético B
a) ¿Hacia dónde se deflecta la trayectoria?
b) ¿Cuál es la magnitud de la velocidad si la partícula choca exactamente con el fin de la placa?

#### Solución
La fuerza de Lorentz es la unión entre el electromagnetismo y la mecánica, y en general una
~ yB
~ está sometida a una fuerza
partícula de carga q en prescencia de campos E


~ + ~v × B
~
F~ = q E
donde ~v es la velocidad de la partícula. En este caso, q = −e, y el campo eléctrico es nulo.
De esta forma
~
F~ = −e~v × B
Dado que la velocidad inicial con que incide el electrón es perpendicular al campo magnético,
la trayectoria será una circunferencia en el plano x − y (siempre y cuando la partícula esté contenida en la región donde existe campo magnético)

Para analizar hacia donde se deflectará la partícula, basta con analizar que ocurre en el
instante inicial t = 0
~ = v î × −B k̂ = vB ĵ
~v (0) × B
Luego en t = 0 la fuerza es

F~ (0) = −evB ĵ

Es decir, la partícula se deflecta hacia abajo

---

### Página 28

b) Dado que el electrón impacta con el extremo derecho de la placa inferior, la trayectoria
de la partícula es la siguiente

La magnitud de la fuerza magnética sobre el electrón es constante y dada por
| F~ |= evB
y su dirección es radial (apuntando hacia el centro de curvatura). Por dinámica circular, se
tendrá
evB =

mv 2
R

R=

mv
eB

luego

por otro lado, se tiene


d
l + R−

2

l2 + R2 − Rd +
R=

= R2

d2
= R2

l2 d
+
d

entonces
l2 d
mv
= +
eB
d
y el módulo de la velocidad del electrón resulta ser


eB l2 d
v=
+
m d

---

### Página 29

Problema
En la figura se muestran los componentes escenciales de un espectrómetro de masas. Éste es
utilizado para medir la masa de partículas cargadas. En una fuente se produce un ión de masa m
y carga q, el cual parte del reposo y es acelerado por una diferencia de potencial ∆V , entrando
~ uniforme (entrando a la hoja), y
a un proceso de selección, donde hay un campo magnético B
~ Sólo partículas con velocidad ~v constante abandonan el selector
un campo eléctrico deflector E.
(es un selector de velocidades). Las partículas emergentes entran a una segunda región donde
~ 0 (entrando a la hoja), la partícula sigue una trayectoria circular
existe otro campo magnético B
y se estrella en un detector a distancia 2r del punto de entrada

a) Encuentre la velocidad ~v
~
b) Encuentre el campo B
c) Finalmente, encuentre la masa m de la partícula
#### Solución
a) La velocidad v con que el ión entra al selector se obtiene por conservación de energía
1 2
mv = q∆V
donde el cambio en energía potencial se traduce en un aumento en la energía cinética
r
2q∆V
~v =
ĵ
m
b) Para que la velocidad de la partícula permaneza constante y salga a través del selector,
se requiere que la fuerza de Lorentz actuando sobre ella sea nula. Se tiene


~
~
~
F = q E + ~v × B
~ = E î, B
~ = −B k̂, ~v = v ĵ
donde E

qE î − qv ĵ × B k̂ = 0
qE î − qvB î = 0 → qE = qvB

---

### Página 30

y entonces
E
B=
=E
v

r

m
2q∆V

~ 0 , la partícula describe una circunc) Luego de ingresar a la región de campo magnético B
ferencia de radio r. La magnitud de la fuerza magnética es qvB0 . Por dinámica circular
qvB0 = m
m
qB0 =
r
Finalmente

r

v2
r

2q∆V
m

qB02 r2
m=
2∆V

---

### Página 31

Problema
Considere una espira circular que lleva corriente I en el sentido indicado por la figura. Calcule
el campo magnético a una distancia z en el eje de simetría de la espira

#### Solución
Utilizando la ley de Biot-Savart para un elemento infinitesimal de la espira
~ x) =
dB(~
en este caso, tenemos

µ0 I d~x0 × (~x − ~x0 )
4π
|~x − ~x0 |3



~x0 = R cos φî + sin φĵ = Rr̂(φ)


d~x0 = Rdφ −î sen φ + ĵ cos φ = Rdφφ̂

y



~x − ~x0 = z k̂ − R cos φî + R sin φĵ = −îR cos φ − ĵR sin φ + k̂z
|~x − ~x0 | = (R2 + z 2 )1/2

Así
~ x) =
dB(~


 

Rdφ
−
î
sin
φ
+
ĵ
cos
φ
×
−
îR
cos
φ
−
ĵR
sin
φ
+
k̂z
µI

(R2 + z 2 )3/2

4π

~ x) = dφ
dB(~

µ0 I (R2 sin φ2 k̂ + Rz sin φĵ + R2 cos φ2 k̂ + Rz cos φî)
4π
(R2 + z 2 )3/2

~ x) = dφ
dB(~

µ0 I (R2 k̂ + Rz sin φĵ + Rz cos φî)
4π
(R2 + z 2 )3/2

---

### Página 32

Con esto
~ x) = µ0 I
B(~
4π

ˆ 2π

dφ

(R2 k̂ + Rz sin φĵ + Rz cos φî)
(R2 + z 2 )3/2

Las integrales según î y ĵ son cero, como era de esperarse por argumentos de simetría.
Finalmente el campo magnético a una distancia z del anillo es
~ x) = µ0 I
B(~
4π

ˆ 2π

dφ

µ0 I
R2
R2
k̂
=
k̂
(R2 + z 2 )3/2
2 (R2 + z 2 )3/2

---

### Página 33

Problema
Considere un disco muy delgado que tiene una densidad de carga superficial σ uniformemente
distribuída. El disco se pone a girar a velocidad angular w en torno a su eje. Encuentre el campo
magnético en el eje del disco

#### Solución
Se tiene una distribución de carga en movimiento (en efecto es una distribución de corriente), de
forma que ésta generará sin duda un campo magnético. Anteriormente se determinó el campo
magnético en el eje de un anillo de radio r con corriente I, esto es
~
B(z)
=

µ0 Ir2
2(z 2 + r2 )3/2

Podemos ver el disco como una superposición de anillos con corriente de ancho infinitesimal
dr, de esta forma por el principio de superposición el campo magnético total será la suma de
las contribuciones de estos anillos. Veamos que ocurre en la porción de disco comprendida entre
r y r + dr, con r ∈ (0, R)

La carga contenida en este anillo es
dq = σ2πrdr
la rotación le asocia a este anillo una corriente.

---

### Página 34

La carga dq da una vuelta completa en un tiempo
∆t =

2π
w

luego la corriente asociada es
dI =

dq
wσ2πrdr
=
= σwrdr
∆t
2π

el campo magnético a una distancia z sobre el eje del disco generado por este anillo es
~
dB(z)
=

drµ0 wσr3
µ0 dIr2
k̂ =
k̂
2(z 2 + r2 )3/2
2(z 2 + r2 )3/2

Entonces el campo total es
ˆ R
ˆ
µ0 wσ R
drµ0 wr3 σ
drr3
~
B(z) =
k̂
=
k̂
2 3/2
2 3/2
0 2(z + r )
0 (z + r )
Realizando el cambio de variable
u2 = z 2 + r2 , 2udu = 2rdr
ˆ

De esta forma



ˆ
ˆ
drr3
duu(u2 − z 2 )
z2
=
= du 1 − 2
(z 2 + r2 )3/2
u3
u
ˆ
drr3
z2 √ 2
z2
2+ √
=
=
u
+
z
+
r
(z 2 + r2 )3/2
u
z 2 + r2



R
z2
µ0 wσ √ 2
~
z +r + √
k̂
B(z) =
z 2 + r2 0


√
z2
z2
µ0 wσ √ 2
~
z +R + √
− z −√
k̂
B(z) =
z 2 + R2
z2

µ0 wσ
~
B(z)
=



√

z 2 + R2 + √

µ0 wσ
~
B(z)
=




z2
− 2 | z | k̂
z 2 + R2


2z 2 + R2
√
− 2 | z | k̂
z 2 + R2

---

### Página 35

Problema
Considere dos bobinas de N vueltas de radio R, cada una perpendicular al eje de simetría, con
sus centros localizados en z = l/2 y z = −l/2. Existe una corriente constante I en el mismo
sentido en cada bobina, como se muestra en la figura. Encuentre el campo magnético en el eje
a una distancia z del centro de una de las bobinas. Verifique que la primera derivada del campo
en el punto medio es nula.

#### Solución
Del problema anterior, tenemos que para una espira circular con corriente I, radio R y a una
distancia z de su centro, el campo en el eje de simetría es
R2
µ0 I
~
k̂
B(~x) =
2 (R2 + z 2 )3/2
Como una bobina consta de N espiras circulares separadas por una distancia despreciable
con respecto a z, podemos utilizar el principio de superposición y obtener el campo provocado
por una bobina de N vueltas
R2
~ x) = µ0 N I
B(~
k̂
2 (R2 + z 2 )3/2
Ahora, sea un punto en el eje, a una distancia z del origen, el campo provocado por la
bobina de abajo es
R2
~ 1 (z k̂) = µ0 N I
k̂
B
2 (R2 + (z + l/2)2 )3/2
y el campo generado por la bobina de arriba
R2
~ 2 (z k̂) = µ0 N I
B
k̂
2 (R2 + (z − l/2)2 )3/2
Y el campo magnético total, por el principio de superposición


µ0 N IR2
~
k̂
B(z k̂) =
+
(R2 + (z − l/2)2 )3/2 (R2 + (z + l/2)2 )3/2

---

### Página 36

Notemos que la primera derivada con respecto a z está dada por


µ0 N IR2
dB
3(z − l/2)
3(z + l/2)
=
−
−
dz
((z − l/2)2 + R2 )5/2 ((z + l/2)2 + R2 )5/2
Se puede notar de inmediato que en el punto medio z = 0 se tiene
dB
=0
dz z=0
También se puede demostrar que si la distancia l entre ambas bobinas es R (radio de las
espiras), se obtiene que
d2 B
=0
dz 2 z=0
Esta configuración se conoce como Helmhotz coils (bobinas de Helmhotz). La gracia es que
el campo es aproximadamente uniforme en una pequeña región cercana a z = 0. Si se expande
en torno a este punto
1 00
B (0)z 2 + B 000 (0)z 3 + ...
2!
3!
B(z) = B(0) + B 000 (0)z 3 + ...
3!
Incluso se puede demostrar que la tercera derivada también es cero en z = 0, es decir, el
cambio en el campo en el punto medio para pequeñas variaciones de z es del orden de z 4 !!
B(z) = B(0) + B 0 (0)z +

---

### Página 37

Problema
Calcule el campo magnético en el centro de la circunferencia de la figura

#### Solución
Este problema se soluciona fácilmente utilizando el principio de superposición.
En el problema 2 ya se vió que la magnitud del campo eléctrico debido a un alambre rectilíneo
muy largo a una distancia a de él es
B1 =

µ0 I
2πa

En este caso, según el sentido de la corriente
~ 1 = µ0 I ĵ
B
2πR
Es decir, apunta hacia el fondo de la hoja. Ahora, del problema 3 obtuvimos el campo magnético
de un anillo a una distancia z del centro en el eje de simetría está dado por
R2 k̂
~ 2 = µ0 I
k̂
B
2 (R2 + z 2 )3/2
Como interesa el campo en el centro del anillo, z=0
~ 2 = µ0 I k̂
B
2R
Finalmente, por el principio de superposición, el campo resultante en el centro del anillo es
~ =B
~1 + B
~ 2 = µ0 I ĵ + µ0 I k̂
B
2πR
2R


µ0 I
~
B=
ĵ + k̂
2R
π

---

### Página 38

Problema
Una partícula de carga q y masa m entra con velocidad v en un campo magnético uniforme B
como se muestra en la figura. ¿Cuánto tiempo transcurre entre que la carga ingresa al campo
magnético y sale?

#### Solución
Es sabido que la fuerza magnética sobre una carga en movimiento q está dada por la fuerza de
Lorentz
~
F~ = q~v × B

Ésta fuerza es siempre perpendicular a ~v , luego, se sigue que ésta fuerza no ejerce trabajo.
Con esto, la energía cinética de la partícula es constante y entonces su rapidez también. La
trayectoria que sigue la partícula bajo este campo magnético uniforme es una hélice

Si se observa el movimiento proyectado en un plano perpendicular al campo magnético, la
trayectoria describe una semicircunferencia, hasta volver a salir de la región donde se encuentra
el campo magnético. Sea R el radio de ésta semicircunferencia, luego podemos determinar el
tiempo que demora en salir como
πR
2πR
=
T =
2v 0
v0
donde v es la componente de la velocidad que es perpendicular al campo magnético. Ahora
debemos determinar R. De la segunda ley de Newton

---

### Página 39

mv 02
=F
R
donde F es la magnitud de la fuerza magnética que se ejerce sobre la partícula.
F = qvB sin(π/4) = qv 0 B
de esta forma

mv 02
= qv 0 B
R
R=

Finalmente
T =

mv 0
qB

πm
π mv 0
=
v 0 qB
qB

---

### Página 40

Problema
Considere dos alambres paralelos separados por una dstancia a y que llevan corrientes I1 e I2
en la dirección x. Calcule la fuerza entre ambos conductores.

#### Solución
La fuerza magnética F~1 , que ejerce el alambre 2 sobre el alambre 1, se puede obtener como
F~1 = I1

ˆ

~
d~l1 × B

~ es el campo magnético creado por el conductor 2. Usando el resultado del problema
donde B
2, para alambres suficientemente largos, las líneas del campo magnético debido a I2 son círculos
~ 2 apuntando en la dirección tangencial. Así, en
concéntricos con el alambre 2, con el campo B
un punto arbitrario P sobre el alambre 1, tenemos
~ 2 = µ0 k̂
B
2πa
que apunta en dirección perpendicular al alambre 1, como se ve en la figura

Al ser este campo uniforme a lo largo del conductor 1, y siendo éste un alambre rectilíneo, la
fuerza que experimenta está dada por
~ 2 = I1 lĵ ×
F~1 = I1~l × B



µ0 I2
2πa



k̂ =

µ0 I1 I2 l
î
2πa

Claramente esta fuerza apunta hacia el conductor 2. Resulta evidente que F~2 = −F~1 . De
esta forma, 2 cables paralelos que llevan corriente en la misma dirección se atraerán. Por otro
lado, si las corrientes fluyen en direcciones opuestas, la fuerza resultante será repulsiva.

---

### Página 41

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 42

Problema
Calcular la fuerza resultante sobre la espira con corriente I2

#### Solución
Para obtener la fuerza total sobre la espira, sumamos las fuerzas sobre las secciones 1,2,3 y 4.

Tenemos
F~1 = I2

ˆ c

~1
d~l1 × B

el campo en la sección 1 es uniforme y está dado por
~ 1 = − µ0 I1 k̂
B
2πa
Así
F~1 = I2

ˆ c

dy ĵ × −

µ0 I1
k̂
2πa

µ0 cI1 I2
ĵ × k̂
F~1 = −
2πa
µ0 cI1 I2
î
F~1 = −
2πa

---

### Página 43

Ahora, para la sección 3
F~3 = I2

ˆ c

~3
d~l3 × B

con
~3 = −
B

µ0 I1
k̂
2π(a + b)

y entonces
F~3 = I2

ˆ 0
c

dy ĵ × −

µ0 I1
k̂
2π(a + b)

y obtenemos
µ0 cI1 I2
î
F~3 =
2π(a + b)
La fuerza sobre la sección 2 será
F~2 = I2

ˆ b

F~2 = −I2
Notemos que
F~4 = I2

ˆ 0
b

ˆ b

~2
d~l2 × B

dxî ×

−dxî ×

µ0 I1
k̂
2π(a + x)

−µ0 I1
k̂ = −F~2
2π(a + x)

F2 y F4 se cancelan, luego, la fuerza total sobre la espira es


µ0 cI1 I2
µ0 cI1 I2
î
−
2π(a + b)
2πa

Notar que en signo es negativo, es decir, la fuerza es atractiva.

---

### Página 44

Problema
Un circuito cuadrado rígido de lado L y masa M está pivoteado en torno a uno de sus ejes en
~ uniforme, y el campo gravitatorio. El circuito lleva una
prescencia de un campo magnético B
corriente I que es capaz de mantenerlo en equilibrio en un ángulo ϑ. Encuentre el sentido y
magnitud de dicha corriente

#### Solución
Para el equilibrio, se requiere que el torque neto sobre la espira con respecto a algún punto de
aceleración nula sea cero. Se escoge como origen el punto O ubicado en una de las esquinas de
la espira, como se muestra en la figura

Para el torque que ejerce el peso, usamos que la fuerza de gravedad se puede concentrar en
el centro de masa


l
~
~τ = ~r × F =
sin ϑî − cos ϑĵ × −M g ĵ
~τ = −

M gl
sin ϑk̂

---

### Página 45

Por otro lado, el torque que ejerce la fuerza magnética es
~
~τ = m
~ ×B
donde m
~ es el momento magnético de la espira
m
~ = IAn̂ = Il2 n̂
Requerimos en primer lugar que este torque tenga dirección k̂. Luego n̂ debe tener la dirección de m
~ en el dibujo

~ = Il2 B cos ϑk̂
~τ = m
~ ×B
El equilibrio exige entonces
l
M g sin ϑk̂ − Il2 B cos ϑk̂ = 0
Luego, la corriente I debe ser
M g tan ϑ
2lB
La dirección debe ser acorde con la dirección del momento magnético, la cual se muestra en
la siguiente figura
I=

---

### Página 46

Problema
Un circuito cuadrado de lado a está suspendido en el centro de un enorme anillo fijo de radio
R, con R >> a por un hilo que ejerce un torque restaurador de magnitud τ = kϑ, con ϑ el
ángulo de torsión que forman los planos de ambos circuitos. Si por el circuito pequeño circula
una corriente i y por el grande I, encuentre en forma aproximada el valor de la constante k de
modo que ϑ = π/2 sea posición de equilibrio

#### Solución
~ que la corriente I produce en el centro del anillo (coinciEncontramos el campo magnético B
dente con el centro de la espira cuadrada). Como a << R, podemos considerar que el campo
es aproximadamente uniforme en una región que contenga a la espira cuadrada. El campo en
el centro es fácil de obtener con la ley de Biot-Savart
ˆ
µ0 I
~x − ~x0
~
B(~x) =
d~x0 ×
4π Γ
| ~x − ~x0 |
donde Γ es la curva que parametriza al anillo. Se tiene

~x = ~0, ~x0 = Rr̂(ϕ), d~x0 = Rdϕϕ̂, | ~x − ~x0 |= R
~ ~0) = µ0 I
B(
4π

ˆ 2π

dϕRϕ̂ ×

−Rr̂(ϕ)
R3

~ ~0) = µ0 I 2π k̂ = µ0 I k̂
B(
4πR
2R
El torque del campo magnético sobre la espira está dado por
~
~ ×B
~τ1 = m

El cual dependerá del ángulo que formen los planos de ambos circuitos

---

### Página 47

De acuerdo a la figura, en tal posición se tendrá un torque magnético dado por
~ = ia2 µ0 I sin ϑĵ
~τ1 = m
~ ×B
2R
En ϑ = π/2
~τ1 =

iIa2 µ0
ĵ
2R

Por otro lado, se tendrá un torque restaurador
~τ2 = −kϑĵ
en ϑ = π/2

π
~τ2 = −k ĵ

Para que ϑ = π/2 sea una posición de equilibrio
π
iIa2 µ0
−k =0
2R
Luego
k=

µ0 Iia2
πR

---

### Página 48

Problema
Considere la espira de corriente formada por segmentos radiales y arcos de circunferencia como
~ en el punto P.
se muestra en la figura. Obtenga el campo magnético B

#### Solución
Para obtener el campo magnético en P, utilizaremos el principio de superposición, notando que
el campo total en P será la suma de las contribuciones de las secciones 1,2,3,4 y 5

Si fijamos el origen en P , notamos inmediatamente que las contribuciones de los segmentos 1
y 5 son nulas, ya que en ambos casos el vector d~x0 es paralelo al vector ~x − ~x0 , con ~x = ~0
Para el sector 2

Tenemos
~2 =
dB
Utilizando coordenadas polares

µ0 d~x0 × (~x − ~x0 )
I
4π
|~x − ~x0 |3

---

### Página 49



d~x = bdφ − sin φî + cos φĵ



ya que P es el origen, ~x = 0, y por último el vector que va desde el origen al elemento diferencial
de corriente tiene magnitud b y la dirección del vector unitario radial en polares


~x = b cos φî + sin φĵ
Notar que

|~x − ~x0 |3 = | − ~x0 |3 = b3
con esto




µ0 dφ − sin φî + cos φĵ × −b(cos φî + sin φĵ)
Ib
4π
b3


dφ sin φk̂ + cos φ
µ0
~ 2 = µ0 I
dB
Idφk̂
k̂ =
4π
b
4πb

~2 =
dB

Así, el campo total en P debido al arco exterior es
ˆ φ
µ0
µ0 φ
~
dφk̂ =
I
k̂
B2 =
4πb 0
4πb
Ahora, para el arco interior (sección 4) el procedimiento es totalmente análogo, con la
diferencia de que la distancia ahora es a, y que la corriente va en el sentido opuesto al del arco
exterior
~ 4 = − µ0 φ k̂
B
4πa
Por último, para la sección 3, es fácil notar que su contribución es nula, ya que en este caso,
el vector d~x0 apunta en la dirección contraria al vector unitario radial en coordenadas polares,
y a su vez ~x0 apunta en la dirección radial, de esta forma, el producto vectorial d~x0 × (~x − ~x0 )
es 0 en todo el segmento 3. Resumiendo, solo los segmentos 2 y 4 contribuyen al campo en P,
y el campo total será la suma de ambas contribuciones


µ0 φ 1 1
~
~
~
B = B2 + B4 =
k̂
−
4π b a

---

### Página 50

Problema
Un conductor rectilíneo con corriente I baja por el eje y hasta el origen, y luego continua en
dirección horizontal. Muestre que el campo magnético en algún punto (x, y) con x > 0, y > 0
está dado por
!
µ
x
I
y
~
B(x,
y) =
k̂
+ + p
+ p
4π x y y x2 + y 2 x x2 + y 2

#### Solución
Sea P un punto sobre el plano (x,y) con x > 0, y > 0. El campo magnético en P será la
superposición del campo creado por la sección vertical y el de la sección horizontal. Sea Γ1 la
curva descrita por
Γ1 : ~x0 = ~x0 (t) = (0, −t) , t ∈ (−∞, 0)

Así d~x0 (t) = dt(0, −1) .Es fácil ver que esta curva representa el segmento vertical de conductor,
y es recorrido en el sentido de la corriente. El campo magnético en P se obtiene a partir de la
ley de Biot-Savart
ˆ
µ0
~x − ~x0
~
B1 (x, y) =
d~x0 I ×
4π Γ1
| ~x − ~x0 |3
~ 1 (x, y) = µ0 I
B
4π

ˆ 0

(x, y) − (0, −t)
µ0 I
−dtĵ ×
=
| (x, y) − (0, −t) |3
4π
−∞

~ 1 (x, y) = µ0 I
B
4π

ˆ 0

ˆ 0

−dtĵ ×

ˆ 0

dt

−∞

µ0 Ix
dt
=
k̂

3/2
4π
−∞
x2 + (y − t)2
xk̂

−∞

La función a integrar es par, luego

~ 1 (x, y) = µ0 I k̂
B
4πx2

ˆ ∞

dt 

xî + (y − t) ĵ
3/2
x2 + (y − t)2



x3 1 + (y−t)
x2

3/2

1 + (y−t)
x

3/2

Ahora se utiliza la sustitución tan ϑ = (y−t)
, sec2 ϑdϑ = − dt
, y entonces
x
x
ˆ

dt 

1 + (y−t)
x2

3/2 = −x

ˆ

sec2 ϑdϑ
3/2

(1 + tan2 ϑ)

= −x

ˆ

sec2 ϑdϑ
= −x
sec3 ϑ

ˆ

dϑ cos ϑ = −x sin ϑ

---

### Página 51

Ahora, como tan ϑ = (y−t)
, es fácil ver que (es cosa de construír un triángulo rectángulo,
x
con un lado igual a (y − t), y otro igual a x)
(y − t)
sin ϑ = q
x2 + (y − t)2

de forma que




∞
y
µ0 I
~ 1 (x, y) = − µ0 I k̂  q (y − t)

k̂ −1 − p
=−
B
4πx
4πx
x2 + y 2
x2 + (y − t)2
!
µ
y
I
~ 1 (x, y) = 0
k̂
+ p
B
4π x x x2 + y 2

!

Ahora, el segmento horizontal está caracterizado por la curva
Γ2 : ~x0 (t) = (t, 0)
d~x0 = (1, 0)dt, t ∈ (0, ∞)
De la ley de Biot-Savart, obtenemos el campo magnético generado por esta sección
˛
ˆ
µ0 I
~x − ~x0
µ0 I ∞
(x − t, y)
~
d~x ×
B2 (x, y) =
=
dtî ×
4π Γ2
| ~x − ~x |
4π 0
((x − t)2 + y 2 )3/2
ˆ ∞
I
µ
y
~ 2 (x, y) =
dt
B
k̂
4π
((x − t)2 + y 2 )3/2
Esta integral es idéntica a la calculada anteriormente, sólo que intercambiando el rol de x e
y
~ 2 (x, y) = µ0 I
B
4π
Finalmente
µ0 I
~
B(x,
y) =
4π

x
+ p
y y x2 + y 2

!

k̂

y
1 1
x
+ p
+ + p
x y y x2 + y 2 x x2 + y 2

!

k̂

---

### Página 52

Problema
Un cilindro de radio a y largo h tiene una corriente superficial I uniformemente distribuída en
el manto. Calcule el campo magnético producido sobre su eje

#### Solución
El sistema se puede ver como un conjunto de espiras por las cuales circula una corriente infinitesimal dada por
Idz 0
h
puestas una al lado de la otra. Determinemos inicialmente el campo asociado a una espira
ubicada a una distancia z 0 del origen por la cual circula una corriente I. Por la ley de Biot Savart, el campo magnético originado por un elemento de corriente I es
~ z0 =
dB

µ0 dz 0 Id~l × (~r − ~r0 )
4πh | ~r − ~r0 |3

En este caso ~r = z k̂, ~r0 = ar̂ + z 0 k̂, d~l = adϑϑ̂
~ z0 =
dB

µ0 dz 0 Iadϑϑ̂ × (−ar̂ + (z − z 0 )k̂)
4πh
(a2 + (z − z 0 )2 )3/2

Integrando la componente según k̂ tiene que
~ z0 = µ0 dz
B
4πh

ˆ 2π
o

dϑIa2 k̂
(a2 + (z − z 0 )2 )3/2

Notar que existe una componente según r̂, sin embargo su integral es cero, como se podría
esperar por simetría.
Ia2 k̂
µ0 dz 0
~
Bz =
2h (a2 + (z − z 0 )2 )3/2

Este es el aporte de una sola espira, y por lo tanto, puede considerarse como un elemento
diferencial de campo magnético. El campo magnético total es
ˆ h
µ
Ia2
~ =
B
dz 0 2
k̂
2h o
(a + (z − z 0 )2 )3/2
Usando el cambio z − z 0 = atanx, −dz 0 = asec2 x
ˆ
ˆ
µ o I x2
µ0 x2 −dxIa2 asec2 x
~
dxcosxk̂
k̂ = −
B=
2h x1 (a2 + a2 tan2 x)3/2
2 x1

---

### Página 53

~ = − µ0 I (sinx2 − sinx1 )k̂
B
2h
donde
sinx2 = p

z−h

a2 + (z − h)2
z
sinx1 = √
z + a2

Finalmente
µo I
z
~ = − µo I p z − h
√
B
k̂ +
k̂
2h a + (z − h)
z + a2

---

### Página 54

12.6.

Corrientes estacionarias extensas localizadas

Vamos a generalizar la ley de Biot-Savart para una distribución de corrientes localizadas en
un volumen V , como se muestra en la figura

Para calcular el campo magnético en ~x, se utiliza un modelo de anillos Biot-Savart. Sea
~x0 ∈ V , y Γ(~x0 ) una curva cerrada de corriente estacionaria, luego
˛
~x − ~x00
µ
~ x) =
d~x00 ×
dI(~x )
dB(~
4π
| ~x − ~x00 |3
Γ(~
x0 )
Además

~ x0 ) = dI(~x ) ˆl(~x0 )
J(~
dS(~x0 )

luego
~ x)=
J(~



dI
dS



~
x0

t̂(~x0 )

~ x0 )
dI(~x0 ) = dS(~x0 )t̂(~x0 ) · J(~
con t̂(~x0 ) el vector unitario tangente a la curva Γ(~x0 ). Así
~x0 ∈ Γ(~x0 ) : dI(~x0 ) = dS(~x0 )J(~x0 )
Pero
~x00 ∈ Γ(~x0 ) → dI(~x00 ) = dI(~x0 ) = C
ya que es un elemento de corriente estacionaria. Luego
˛
~x − ~x00
µ
~ x) =
dB(~
d~x00 ×
dI(~x00 )
4π Γ(~x0 )
| ~x − ~x00 |3
˛
~x − ~x00
µ0
ds00 t̂(~x00 ) ×
dS(~x00 )J(~x00 )
=
4π Γ(~x0 )
| ~x − ~x00 |3
˛
µ0
~ x00 ) × ~x − ~x dS(~x00 )
ds00 J(~
=
4π Γ(~x0 )
| ~x − ~x00 |3
El campo magnético total en ~x será
¨
˛
~x − ~x00
µ0
00 ~ 00
~
dS(~x ) ds J(~x ) ×
B(~x) =
4π
| ~x − ~x00 |3

---

### Página 55

~ x) = µ0
B(~
4π

˚

~ x) = µ0
B(~
4π

˚

~ x00 ) ×
d3 x00 J(~

V

~x − ~x00
| ~x − ~x00 |3

~x − ~x0
d x J(~x ) ×
| ~x − ~x0 |3
V
3 0

Este es el campo magnético generado por una distribución de corriente localizada dentro de un
volumen V

12.7.

Las dos leyes fundamentales de la magnetostática

Hemos obtenido, a partir de la ley de Biot-Savart y el principio de superposición la forma
general del campo magnético generado por una distribución de corriente localizada dentro de
un volumen V
˚
µ0
~
~ x0 ) × ~x − ~x
B(~x) =
d3 x0 J(~
4π
| ~x − ~x0 |3
V
Ahora utilizamos el lema

~
∇
entonces

~x − ~x0
=
−
| ~x − ~x0 |
| ~x − ~x0 |3

~ x) = − µ0
B(~
4π

˚

V

~
~ x0 ) × ∇
d3 x0 J(~

~ x) = µ0 ∇
~ ×
B(~
4π

˚

d3 x0

V

| ~x − ~x0 |

~ x0 )
J(~
| ~x − ~x0 |

de forma que el campo magnetostático es el rotor de un campo vectorial, que llamaremos
potencial magnético vectorial
~ x) =
A(~

˚

d3 x0

V

y

~ x0 )
J(~
| ~x − ~x0 |

~ x) = ∇
~ × A(~
~ x)
B(~

De esta forma, la divergencia del campo magnético es siempre nula
~ · B(~
~ x) = 0
∇
Además, se tiene
˚
~ x0 )
J(~
µ0 ~
~
~
~
d3 x0
∇ × B(~x ) =
∇×∇×
4π
| ~x − ~x0 |
V
˚
˚
~ x0 )
~ x0 )
µ0 ~ 2
µ0 ~ ~
3 0 J(~
3 0 J(~
~
~
−
∇∇ ·
∇
dx
d
x
∇ × B(~x ) =
4π
| ~x − ~x0 | 4π
| ~x − ~x0 |
V
V
˚
˚
µ0 ~
3 0~ 0
~ x0 )δ(~x − ~x0 )
~
=
+ µ0
d x J(~x ) · ∇
d3 x0 J(~
∇
4π
| ~x − ~x |
V
V

---

### Página 56

Si ~x ∈ V
˚
µ0 ~
~
~
~0
~ x0 ) · ∇
∇ × B(~x ) = − ∇
+ µ0 J(~x)
d3 x0 J(~
4π
| ~x − ~x0 |
V
˚
˚
~ 0 ~ x0 )
~ x0 )
J(~
µ0 ~
µ0
3 0~ 0
3 0 ∇ · J(~
~ x)
d x∇ ·
d
x
=− ∇
+
+ µ0 J(~
4π
| ~x − ~x0 | 4π
| ~x − ~x0 |
V
V
˚
~ x0 ) · J(~
~ x0 )
~ 0 ~ x0 ) µ0 ˆˆ  dS(~
µ0
3 0 ∇ · J(~
~
~ 
dx
= µ0 J(~x) +
∇
−
4π
| ~x − ~x0 |
4π
| ~x − ~x0 |
V
δV

Pero, si la distribución corriente está localizada dentro de V , no hay flujo de corriente a
través de δV , es decir
~ x) = 0, ~x ∈ δV
n̂(~x) · J(~
Además, la condición de corriente estacionaria significa
~ · J(~
~ x) = 0, ~x ∈ V
∇
De forma que
~ × B(~
~ x) = µ0 J(~
~ x)
∇

12.8.

Leyes fundamentales, forma diferencial

Hemos obtenido las siguientes ecuaciones diferenciales para el campo magnetostático
~ · B(~
~ x) = 0
∇
~ x)
~ × B(~
~ x) = µ0 J(~
∇
Recordar el teorema de Helmholtz! La teoría magnetostática es completa. La primera de
ellas contiene la información de que nunca han sido observados monopolos magnéticos. Se puede
obtener una forma integral, integrando sobre un volumen V
˚
~ · B(~
~ x) = 0
d3 x∇
V

utilizando el teorema de la divergencia
ˆˆ
 ~
~ x) = 0
x) · B(~
 dS(~
S

Es decir, el flujo magnético sobre cualquier superficie cerrada es siempre nulo. La segunda
ecuación para el rotor
~ x)
~ × B(~
~ x) = µ0 J(~
∇
es la ley de Ampère, cuya forma integral y aplicaciones serán estudiadas en detalle en el
siguiente capítulo

---

### Página 57

#### Capítulo 13
Ley de Ampére
Se vió que cargas en movimiento son fuentes de campo magnético. En particular, corrientes
estacionarias en un conductor son fuentes de campos magnéticos estáticos (no varían en el
tiempo). Tal cual la ley de Gauss en electrostática puede ser muy util en problemas de geometría
simple, para campos magnéticos existe un equivalente, que es la ley integral de Ampère.
~ x)
Ésta se obtiene a partir de la ecuación para el rotor de B(~
~ × B(~
~ x) = µ0 J(~
~ x)
∇
Podemos integrar esta ecuación sobre una superficie S arbitraria
¨
¨


~ × B(~
~ x) = µ0
~ x) · ∇
~ x) · J(~
~ x)
dS(~
dS(~
S

S

Y utilizando el teorema de Stokes
˛
¨
~ x) = µ0
~ x) · J(~
~ x)
d~x · B(~
dS(~
Γ(S)

S

La integral de línea del campo magnético sobre una curva cerrada Γ (circulación), es proporcional al flujo de corriente sobre cualquier superficie cuyo contorno sea (Γ). Definiendo IΓ
como la corriente que cruza a S, entonces
˛
~ x) = µ0 IΓ
d~x · B(~
Γ

Ejemplo conocido es el campo magnético exterior de una distribución cilíndrica de corriente
(muy larga), como se ve en la figura. Debido a la simetría, la magnitud del campo magnético
debe ser constante a una distancia r del centro del conductor, y su dirección siempre tangente
a curvas circulares concéntricas con el conductor. De esta forma

---

### Página 58

˛

Γ

~ x) = 2πrB(r) = µ0 I
d~x · B(~

de donde

µ0 I
2πr
Problemas con simetría cilíndrica son muy sencillos de resolver con la ley de Ampère. El
campo interior al conductor se obtiene de la misma forma, pero teniendo en cuenta que en ese
caso la corriente encerrada por una trayectoria circular no es I, sino una fracción de ésta
B=

---

### Página 59

Problema
Considere un conductor cilíndrico de radio R y de extensión infinita, que lleva una corriente I
con una densidad de corriente no uniforme
J = αr
donde α es una constante (desconocida), y r es la distancia de un punto interior al conductor
al eje de simetría. Encuentre el campo magnético en todo el espacio

#### Solución
Dada la clara simetría cilíndrica, utilizamos la ley de Ampère para resolverlo. Sea Γ una curva
circular de radio r, con 0 < r < R concéntrica al eje de simetría del conductor. Es claro que
la magnitud del campo magnético sólo puede ser función de r, y su dirección tangente en todo
punto a la curva Γ. Así, veamos que ocurre con la circulación del campo
˛
~ x)
d~x · B(~
Γ





con ~x = r cos ϑî, sin ϑĵ , d~x = rdϑϑ̂, ϑ ∈ [0, 2π]
˛

Γ

~ x) =
d~x · B(~

ˆ 2π

~
dϑrϑ̂ · B(r)
= 2πrB(r)

Por la ley de Ampère, la circulación sobre Γ es igual a µ0 I(Γ) donde I(Γ) es la corriente que
atraviesa la superficie limitada por Γ.(Escogemos la superficie plana encerrada por Γ). Sea k̂ la
dirección del eje de simetría del cilindo (coindidente con el sentido de la corriente). Entonces
I(Γ) =

¨

Γ

~ x) · J(~
~ x) =
dS(~

ˆ 2π

ˆ r

dϑ

ˆ r

~ k̂
drrk̂ · J(r)

2παr3
drr =
I(Γ) = 2πα

De esta forma
2πrB(r) = µ0

2παr3

µ0 αr
~
ϑ̂
B(r)
=
Para encontrar el campo magnético exterior, se utilizan los mismos argumentos de simetría,
y se utiliza una nueva curva Γ circular de radio r > R. La ley de Ampère en este caso entrega
˛
~ x) = 2πr = µ0 I(Γ)
d~x · B(~
Γ

---

### Página 60

donde I(Γ) es la corriente que atraviesa cualquier superficie de contorno Γ. Por supuesto,
escogemos la superficie plana limitada por Γ
¨
ˆ 2π ˆ r
~
~
I(Γ) =
dS(~x) · J(~x) =
dϑ
drrk̂ · J(r)k̂
S

drr2 =

2παR3

pero J(r) = 0, r > R, luego
I(Γ) = 2πα

ˆ R

pero es claro que I(Γ) = I, luego
α=

3I
2πR3

y se tiene
2πrB(r) = µ0 I
µ0 I
~
B(r)
=
ϑ̂, r > R
2πr
µ0 Ir2
~
B(r)
=
ϑ̂, r < R
2πR3

---

### Página 61

Problema
Considere un conductor plano de ancho w e infinitamente largo, en el plano xy. Éste lleva una
corriente I en el sentido de eje x, como se muestra en la figura. Encuentre el campo magnético
en un punto P en el plano del conductor, a una distancia s de él

#### Solución
Considere una sección de conductor de ancho dr, paralela a la dirección de la corriente y a una
distancia r de P , como se ilustra en la siguiente figura

La cantidad de corriente contenida en este elemento diferencial está dada por
 
dr
dI = I
w
Utilizando la ley de Ampère para este elemento de conductor (similar al de un conductor
lineal) se obtiene el ya conocido resultado
~ )=
dB(P

µ0 dI
k̂
2πr

µ0 Idr
k̂
2πrw
Por el principio de superposición, el campo magnético total se obtiene al integrar sobre el
conductor
~ )=
dB(P

ˆ s+w
µ0 I
µ0 I
dr
dr
k̂ =
k̂
2πrw
2πw s
r
s


s+w
µ0 I
~
ln
k̂
B(P ) =
2πw
s

~ )=
B(P

ˆ s+w

Notar que en el límite cuando w << s
ln


s+w
w 1
≈ w
= ln 1 +
s
s
s

---

### Página 62

y entonces

~ ) ≈ µ0 I k̂
B(P
2πs
que es el campo a distancia s de un conductor rectilíneo de ancho despreciable, con corriente

I

---

### Página 63

Problema
Calcule el campo magnético dentro de un solenoide ideal de largo l, N vueltas y que lleva una
corriente estacionaria I.
#### Solución
Un solenoide es una bobina enrollada en forma helicoidal. La figura muestra las lineas de campo
magnético de un solenoide con corriente constante I

Vemos que si las vueltas están muy cercanas espacialmente, el campo magnético resultante
dentro del solenoide es parcialmente uniforme, siempre que la longitud del solenoide sea mucho
mas grande que su diámetro. Para un solenoide ideal, que es infinitamente largo con vueltas
infinitamente cercanas, el campo magnético dentro es uniforme y paralelo al eje x, y es nulo
fuera del solenoide. Podemos utlizar la ley de Ampère para calcular el campo magnético dentro
de un solenoide ideal. Una vista transversal de un solenoide ideal se muestra en la figura

Consideremos el camino rectangular de largo l y ancho w y en sentido contrareloj. La integral
~ x) a través de este camino es
de línea de B(~
ˆ
ˆ
ˆ
ˆ
˛
~
~
~
~
~ x)
d~x · B(~x) = d~x · B(~x) + d~x · B(~x) + d~x · B(~x) + d~x · B(~

Ahora, la integral sobre 1 es 0, ya que el campo es nulo en el exterior del solenoide. Las
integrales sobre 2 y 4 también son nulas, ya que el campo a lo largo de estas trayectorias es
perpendicular a d~x. Con esto, podemos estirar el camino cerrado de manera que encierre todo el
solenoide,notando que la corriente total que atraviesa la superficie encerrada por la trayectoria
es N I, con N el número de vueltas del solenoide
˛
~ x) = Bl = µ0 N I
d~x · B(~

Finalmente
B=

µ0 N I
l

---

### Página 64

Problema
Considere dos planos infinitos paralelos separados por una distancia b en el plano xy. En la
región interior existe una densidad de corriente uniforme J~ = J0~i. Encuentre el campo magnético
en todo el espacio

#### Solución
Podemos pensar la región de corriente como una superposición de conductores paralelos que
llevan corrientes en la direccion +x. De la figura, y por un argumento de simetría vemos que el
campo magnético en un punto P sobre la región apunta en la direccion −y

La componente z desaparece después de sumar todas las contribuciones debidas a todos los
conductores. Similarmente, se puede mostrar que el campo magnético en un punto dentro de la
región apunta en la dirección +y, y en un punto inferior a la región también según la dirección
+y.

---

### Página 65

Ahora podemos utilizar la ley de Ampère para encontrar el campo magnético debido a esta
distribución de corriente. Tomaremos las curvas cerradas que aparecen en la figura. Para el
campo exterior, integramos sobre la curva Γ1 . La corriente que atraviesa la superficie limitada
por Γ1 es
¨
~ x) = J0 (bl)
I(Γ1 ) =
.S(~x) · J(~
Notando que en la integral de línea los segmentos verticales no contribuyen (d~x perpendicular
~ x))
al campo B(~
˛
~ x) = B2l = µ0 I(Γ1 ) = µ0 J0 bl
d~x · B(~
Γ1

de donde
B = µ0 J0 b/2
Notamos que el campo magnético fuera es uniforme, independiente de la distancia a la
región entre ambos planos. Ahora encontremos el campo magnético interior. La corriente total
encerrada por el camino cerrado Γ2 es
¨
~ x) · J(~
~ x) = J0 2zl
I(Γ2 ) =
dS(~
Usando la ley de Ampère,
˛
~ x) · B(~
~ x) = B2l = µ0 I(Γ2 ) = µ0 J0 2zl
dS(~
Γ2

de donde
B = µ0 J 0 z
Notemos que en z=0 el campo magnético es nulo, como se requiere por simetría. Resumiendo
~ = − µ0 J0 b ĵ, z > b/2
B
~ = −µ0 J0 z ĵ, −b/2 < z < b/2
B
~ = µ0 J0 b ĵ, z < −b/2
B

---

### Página 66

Problema
Se tiene dos corrientes, ambas con igual sentido (en el dibujo, saliendo de la hoja). Una de
ellas es una corriente plana e infinita de densidad lineal
Js , y la otra es una corriente cilíndrica

r
infinitamente larga cuya densidad es J = J0 1 − R . Encuentre el valor de J0 en función de Js ,
que hace que el campo magnético resultante en el punto P ubicado a distancia R/2 del centro
del cilindro sea nulo

#### Solución
El campo de la distribución plana de corriente fue obtenido en el problema anterior. De la
simetría es claro que su dirección es como se muestra en la figura

y entonces para encontrar su magnitud se utiliza la ley de Ampère, con una curva plana de
ancho l

˛

Γ

~ 1 (~x) = 2lB1 = µ0 Js lb
d~x · B

---

### Página 67

Luego, en la región superior a la distribución plana
~ 1 (~x) = − µ0 Js b ĵ
B
Para el cilindro, utilizamos nuevamente la ley de Ampère. Dada su extensión infinita, por
simetría el campo magnético en su interior debe ser función únicamente de la coordenada radial
r, y su dirección es tal que es tangente en todo punto a una curva circular concéntrica al cilindro

˛

Γ

~ 2 (~x) = µ0 Ienc
d~x · B

luego

ˆ 2π

ˆ r


r
drrJ0 1 −
R

 2
r3
r
2πrB2 (r) = µ0 J0 2π
−
3R


r2
r
~
B2 (~x) = µ0 J0
−
ϕ̂
2 3R

2πrB2 (r) = µ0

dϕ

En el punto P , se tendrá la superposición de ambos campos. Notar que en dicho punto, ϕ̂
coincide con la dirección ĵ, y entonces




R2
R
µ0 bJs
~
B(P ) = µ0 J0
−
ĵ
−
12R
para tener un campo magnético nulo, debe tenerse entonces
J0

bJs
R
=

Finalmente
J0 =

3bJs
R

---

### Página 68

Problema
Un cable de radio R lleva una densidad de corriente J~ = J0 k̂. El cable tiene un hoyo cilíndrico
de radio α paralelo al eje del cable, a distancia b de él. Muestre que el campo magnético dentro
de la cavidad es uniforme

#### Solución
Resolvemos el problema por superposición de dos corrientes, una del cilindro completo con
densidad de corriente J0 k̂, y otra en la cavidad con densidad −J0 k̂. El campo magnético al
interior de un cable con densidad de corriente J~ = J0 k̂ se puede obtener fácilmente con la ley
de Ampère

Tomando la curva circular de radio r, y dada la simetría cilíndrica de la distribución de corriente,
el campo magnético es constante y tangente sobre la curva. Así
˛
¨
~
d~x · B(~x) = B(r)2πr = µ0
dS(~x)k̂ · J0 k̂
Γ

S(Γ)

B(r)2πr = µ0 J0 πr2
µ0 J 0 r
~
ϑ̂(r)
B(r)
=

---

### Página 69

Sea entonces un punto arbitrario al interior de la cavidad, como muestra la figura

La superposición de los campos magnéticos es la siguiente

~ = µ0 J0 r1 ϑ̂1 − µ0 J0 r2 ϑ̂2
B
pero
ϑ1 = k̂ × r̂1
ϑ2 = k̂ × r̂2
luego


~ = µ0 J0 r1 k̂ × r̂1 − r2 k̂ × r̂2
B


~ = µ0 J0 k̂ × ~r1 − k̂ × ~r2 = µ0 J0 k̂ × (~r1 − ~r2 )
B
~ = µ0 J0 k̂ × ~b
B
el cual es un campo uniforme

---

### Página 70

Problema
Se tiene un conductor cilíndrico de radio R, muy largo, con corriente I, y un conductor plano
también muy largo con corriente superficial I 0 . Se supone que ambos conductores son paralelos
y que el conductor plano y el eje de la corriente cilíndrica son coplanares. Si el plano conductor
tiene ancho a, y el eje del cilindro se encuentra a distancia b del origen, encuentre
a) El campo magnético sobre el eje x, para x > a
b) La fuerza de interacción entre ambos conductores por unidad de largo

#### Solución
Resolvemos el problema por superposición. El plano de corriente puede ser visto como una
superposición de corrientes lineales muy delgadas, de ancho diferencial dx0 , como se muestra en
la figura

Nos concentramos entonces en la porción de plano contenida entre x y x + dx. Este alambre
lleva una corriente
dx
dI = I 0
a

---

### Página 71

El campo magnético sobre el eje a distancia x del origen (con x > a) se puede obtener mediante
la ley de Ampère, integrando sobre la curva circular Γ centrada en x0 y de radio x − x0 . La
magnitud del campo magnético alrededor de la curva es constante e igual a la magnitud del
campo en x
˛
~ x) = B(x)2π(x − x0 ) = µ0 I 0 dx
d~x · B(~
a
Γ
~
B(x)
=−

µ0 I 0 dx0
k̂
2πa(x − x0 )

Entonces el campo magnético en x debido a la distribución plana es
ˆ
a
µ0 I 0 a dx0
µ0 I 0
~
B(x)1 = −
k̂
=
−
ln(x − x0 ) k̂
2πa 0 x − x
2πa
Así, para x > a

~ 1 = − µ0 I ln
B(x)
2πa



x
x−a



k̂

Para el cilindro de radio R, distinguimos dos regiones: dentro y fuera del cilindro. El campo
magnético exterior se obtiene de una aplicación inmediata de la ley de Ampère

~ consistente con la dirección de la corriente, se indica en la figura
El sentido de B,
˛
~ x) = µ0 I
d~x · B(~
Γ

2πrB(r) = µ0 I
µ0 I
2πr
donde r es la distancia radial con respecto al centro del cilindro. De esta forma, en el punto
x, con a < x < b − R
B(r) =

~ 2 (x) =
B

µ0 I
k̂
2π(b − x)

---

### Página 72

Para x > b + R
~ 2 (x) = −
B

µ0 I
k̂
2π(x − b)

Ahora, para el campo al interior del conductor cilíndrico, nuevamente se utiliza la ley de
Ampère

˛

Γ

~ x) = B(r)2πr = µ0
d~x · B(~

B(r)2πr = µ0

¨

S(Γ)

¨

S(Γ)

~ x)
dS(~x)n̂(~x) · J(~

dS(~x)ĵ · J ĵ = µ0 Jπr2

donde
JπR2 = I → J =
B(r)2πr = µ0
B(r) = µ0

I
πR2

Ir2
R2

Ir
2πR2

---

### Página 73

Finalmente, tenemos lo siguiente. Para a < x < b − R


µ
I
I
µ
x
~
B(x)
=
−
ln
k̂
2π(b − x) 2πa x − a
Para b − R < x < b

~
B(x)
=
Para b < x < b + R

~
B(x)
=−
Para b + R < x

x
µ0 I(b − x) µ0 I 0
−
ln
2πR
2πa x − a





µ0 I(x − b) µ0 I 0
x
+
ln
2πR
2πa x − a





k̂



~
B(x)
=−

µ0 I
µ0 I 0
x
+
ln
2π(x − b) 2πa x − a

k̂



k̂

b) Para calcular la fuerza por unidad de largo que ejerce el cilindro sobre la distribución
plana de corriente, calculemos la fuerza que se ejerce sobre el segmento lineal de largo 1, y
ancho dx0 en la posición x0

La fuerza que actúa sobre este segmento es
dF~ (x0 ) =

µ0 I
I 0 dx0
I 0 dx0
ĵ × B2 (x0 )k̂ =
ĵ × k̂
a
a 2π(b − x)
dF~ (x0 ) =

I 0 µ0 Idx0
î
2πa(b − x)

Por superposición, la fuerza neta por unidad de largo que se ejerce sobre el plano es
ˆ a
µ0 II 0
î
dx0
F~ =
2πa(b − x)


II
µ
b
F~ =
î
ln
2πa
b−a

---

### Página 74

Problema
Suponga que tiene dos cables infinitamente largos con densidad lineal de carga λ, separados
por una distancia d, moviéndose a velocidad v constante. Encuentre el valor de v para que la
atracción magnética se compense con la repulsión eléctrica. ¿Es razonable este resultado?

#### Solución
El campo eléctrico generado por el cable izquierdo sobre el cable derecho está dado por
λ
ĵ
2π0 d
De esta forma, la fuerza eléctrica por unidad de largo será
~ =
E

F~Le = λ

λ
λ2
ĵ =
ĵ
2π0 d
2π0 d

Por otro lado, los alambres en movimiento equivalen a una corriente
λdx
dq
=
= λv
dt
dt
El campo magnético generado por el cable izquierdo sobre el derecho es
I=

~ = − µ0 I k̂ = − µ0 λv k̂
B
2πd
2πd
En este caso, la fuerza magnética por unidad de largo sobre el cable derecho será


λv
µ
m
k̂
F~L = −I î × −
2πd
2 2

µ0 λ v
ĵ
F~Lm = −
2πd
Para que éstas fuerzas se anulen

F~Le + F~Lm = 0
λ2
µ0 λ 2 v 2
=
2π0 d
2πd
= µ0 v 2
0

---

### Página 75

La velocidad debe ser
v=√

µ0  0

Evaluando
v=p
= 3 × 108
−12
8,85 × 10
× 4π10−7
Esta es la velocidad de la luz en el vacío!. Claramente este curioso resultado no es razonable,
ya que para tratar problemas con velocidades altas se debe usar la electrodinámica relativista

---

### Página 76

13.1.

Potencial Vectorial

A partir de la ley de Biot-Savart se demostró que el campo magnético satisface la siguiente
relación integro-diferencial
~ x) = µ0 ∇
~ ×
B(~
4π

˚

d3 x0

V

~ x0 )
J(~
| ~x − ~x0 |

Es decir, el campo magnético es el rotor de un campo vectorial, cuya forma más general es
~ x) = µ0
A(~
4π

˚

V

d3 x0

~ x0 )
J(~
~ x)
+ ∇ψ(~
| ~x − ~x0 |

donde ψ es un campo escalar arbitrario(función de Gauge). Sea cual sea el campo ψ, el
~ x) = ∇
~ × A(~
~ x) es siempre el mismo. Veamos que
campo magnético obtenido a partir de B(~
ocurre con
~ · A(~
~ x) = µ0
∇
4π

˚

V

~
d x J(~x ) · ∇
3 0~

~ · A(~
~ x) = − µ0
∇
4π

~ 2 ψ = − µ0
+∇
| ~x − ~x |
4π

˚

V

~0
~ x0 ) · ∇
d3 x0 J(~

~ 2ψ
+∇
| ~x − ~x0 |

˚
~ x0 )
~ 0 ~ x0 )
J(~
µ0
3 0 ∇ · J(~
~ 2ψ
d x∇
d
x
+
+∇
0 |
0 |
|
~
x
−
~
x
4π
|
~
x
−
~
x
V
V

˚

3 0~ 0

la condición de corriente estacionaria entrega
˚
~ 0
µ
~ 0 J(~x ) + ∇
~ · A(~
~ x) = −
~ 2ψ
d3 x0 ∇
∇
0 |
4π
|
~
x
−
~
x
V
y del teorema de la divergencia
ˆˆ
~ x0 )
µ
J(~
 ~ 0
~ · A(~
~ x) = −
~ 2ψ
∇
d
S(~
x
+∇
)
·

4π
| ~x − ~x0 |
La condición de corriente localizada da
~ · A(~
~ x) = ∇
~ 2ψ
∇

Para todo ψ. De esta forma, podemos perfectamente escoger un Gauge tal que
~ · A(~
~ x) = 0
∇

Este es llamado Gauge de Coulomb.

13.2.

Ecuación de Poisson y Laplace

~ x) tal que
Como el campo magnético es de divergencia nula, existe un campo vectorial A(~
~ x) = ∇
~ × A(~
~ x)
B(~
Luego

~ × B(~
~ x) = ∇
~∇
~ × A(~
~ x) − ∇
~ 2 A(~
~ x)
∇

El potencial puede ser escogido como un campo de divergencia nula (Gauge de Coulomb),
luego

---

### Página 77

~ × B(~
~ x) = −∇
~ 2 A(~
~ x)
∇
Además, de la forma diferencial de la ley de Ampère
~ × B(~
~ x) = µ0 J(~
~ x)
∇
De esta forma, el potencial vectorial bajo el gauge de Coulomb satisface la ecuación de
Poisson
~ x) = −µ0 J(~
~ x)
~ 2 A(~
∇
en regiones del espacio libre de corrientes, se obtiene la ecuación de Laplace
~ x) = 0
~ 2 A(~
∇

---

### Página 78

13.3.

Expansión Multipolar del campo magnético

Sea una distribución localizada de corriente dentro de un volumen V . El potencial vectorial
está dado por
~ x) = µ0
A(~
4π

˚

d3 x0

V

~ x0 )
J(~
| ~x − ~x0 |

Veamos que ocurre muy lejos de las fuentes, es decir, analizaremos el caso | ~x0 |<<| ~x |

0 −1


0 −1/2

0 2

| ~x − ~x | = | ~x | + | ~x | −2~x · ~x

La expansión en taylor a primer orden entrega

=
| ~x |



| ~x0 |2 2~x · ~x0
−
1+
| ~x |2
| ~x |2

−1/2

~x · ~x0 1 | ~x0 |2
≈
+
−
+ ...
| ~x − ~x0 |
| ~x | | ~x |3 2 | ~x |3

Luego, el potencial vectorial lejos de las fuentes tiene la forma
˚
˚
µ0
µ0
3 0~ 0
~ x0 )~x0 · ~x + ...
~
d x J(~x ) +
d3 x0 J(~
A(~x) =
4π | ~x |
4π
|
~
x
|
V
V

Ahora, la primera integral es nula, para ello demostraremos el siguiente lema: ∀f, g
˚
~ x) · [f (~x)∇g(~
~ x) + g(~x)∇f
~ (~x)] = 0
d3 xJ(~
V

la demostración es la siguiente
˚
 ˚
 ˚


~ x) · ∇f
~ g =
~ g −
~ · Jf
~ · J(~
~ x)
d x J(~
d x∇
d3 xf g ∇
V

V

V

Usando la condición de corriente estacionaria y el teorema de la divergencia
˚

 ˆˆ
 ~
~ x)f g = 0
~ x) · ∇f
~ g = 
d x J(~
x) · J(~
  dS(~
V

δV

Tomando f (~x) = 1, g(~x) = x
˚
V

~ x) · ∇x
~ =
d xJ(~

˚

d3 xJx (~x) = 0

V

Del mismo modo se puede demostrar que la integral de las componentes en y e z es nula.
Así
˚
~ x) = ~0
d3 xJ(~
V

En otras palabras, corrientes estacionarias localizadas no generan monopolos magnéticos!.
Mas aún, utilizando el mismo teorema , podemos encontrar una nueva expresión para la segunda
integral de la expansión. Tenemos
˚
~ x) · [f (~x)∇g(~
~ x) + g(~x)∇f
~ (~x)] = 0, ∀f, g
d3 xJ(~
V

tomando la componente a-ésima
˚

V

~ a (f g) = 0
d3 xJ~a (~x)∇

---

### Página 79

tomando f g = xb xc
˚

V

~
d xJ~a ∇a(x
b xc ) =

=

˚

˚

d3 xJ~a (xb δac + xcab )

V

d3 x (Jc xb + Jb~xc ) = 0

V

luego
˚

d3 x[xa Jb (~x) + xb Ja (~x)] = 0

V

De esta forma, tomando la componente a-ésima de la siguente integral

˚
˚
˚
3 0~ 0 0
3 0 0 0
d x J(~x )~x · ~x =
d x Ja x b x b =
d3 x0 (Ja0 x0b − Jb0 x0a ) xb
V
V
V
a
y es fácil verificar que
˚

 ˚


3 0~ 0 0
3 0
~
d x J(~x )~x · ~x =
d x [~x × J(~x ) × ~x ]
V
V
a
a
Así, se obtiene

~ x) ≈ µ0 ~x ×
A(~
4π | ~x |3

˚

V

~ x0 ) × ~x0
d3 x0 J(~

Se define el momento magnético de una distribución de corriente localizada en V como
˚
~ x0 )
d3 x0~x0 × J(~
µ=
V

~ x) = µ0 ~µ × ~x
A(~
4π | ~x |3

Es decir, el potencial vectorial (y por lo tanto el campo magnético) muy lejos de la fuente
está completamente determinado (a primer orden) por el momeno magnético de la distribución
de carga.

---

### Página 80

13.4.

Magnetismo en la materia

13.4.1.

Magnetización

La materia consiste en de una colección de momentos magnéticos. En los materiales no
magnéticos, estos momentos están alineados de forma arbitraria, así se cancelan unos a otros y
no hay un efecto neto de campo magnético debido a este material. Sin embargo, como hemos
visto, ante la prescencia de un campo magnético externo, los momentos magnéticos en el interior
del material se alinearán en la dirección paralela al campo

Fig. 13.1: Momentos magnéticos en un material se alinearán en la dirección paralela al campo
externo
Estos momentos magnéticos crearán a su vez un campo magnético. Para obtener el efecto
de esta magnetización, consideremos un elemento de volumen ∆V (~x0 ) ubicado en algún punto interior de material ~x0 . Este elemento de volumen estará caracterizado por un momento
magnético

∆~µ(~x) =

X

m
~a

a∈∆V (~
x0 )

donde la suma se realiza sobre cada átomo contenido en ∆V (~x0 ). Definimos la magnetización del material como la densidad de momento magnético por unidad de volumen, esto
es


∆µ
~
M (~x ) =
∆V
~
x0

Veamos que ocurre con el campo magnético en un punto ~x fuera del material. El potencial
estará dado por
~ x) = A
~ L (~x) + A
~ M (~x)
A(~

~ M (~x) el potencial debido a la
~ L (~x) es el potencial magnético del campo externo y A
donde A
magnetización del medio.

---

### Página 81

En ~x0 ∈ V hay un momento magnético dado por
~ (~x0 )∆V (~x0 )
µ(~x0 ) = M

El potencial en ~x debido a este momento magnético puntual está dado por
~ M (~x) =
∆A

µ0 ∆µ(~x0 ) × (~x − ~x0 )
4π
| ~x − ~x0 |3

El potencial total en ~x debido al material se obtiene al integrar sobre V
~ M (~x) = µ0
A
4π

˚

d3 x0

V

Ahora, se tiene

~ (~x0 ) × (~x − ~x0 )
M
| ~x − ~x0 |3

~ 0
~0×M
~ (~x0 ) × (~x − ~x0 )
~ (~x0 )
∇
M
~ (~x0 ) × ∇
~0
~ 0 × M (~x )
=
M
=
−
∇
| ~x − ~x0 |3
| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |

de forma que

~ M (~x) = µ0
A
4π

~ x0 ) µ0 ˚
~0
3 0 ∇ × M (~
~0×
−
dx
d3 x0 ∇
| ~x − ~x |
4π
V
V

¨

~ (~x0 )
M
| ~x − ~x0 |

!

Finalmente
~ M (~x) = µ0
A
4π

~0
~ x0 ) µ0 ˆˆ  dS(~
~ x0 ) × M
~ (~x0 )
3 0 ∇ × M (~
dx
−


| ~x − ~x0 |
4π δV
| ~x − ~x0 |
V

˚

Recordando que el potencial magnético de una distribución de corriente libre en un volumen
V está dado por
˚
~ x0 )
J(~
~
d3 x0
A(~x) =
| ~x − ~x0 |
V
es inmediato notar que todo sucede como si dentro del material existiera una densidad de
corriente estacionaria
~ ×M
~ (~x)
J~M (~x) = ∇

y como si en el contorno del material hubiera una densidad de corriente superficial
~ (~x)
~σM (~x) = −n̂(~x) × M
Notar que

~ × J~M (~x) = 0
∇

---

### Página 82

(como debe ser para una corriente estacionaria), y
n̂(~x) · σM (~x) = 0
(como debe ocurrir para una corriente localizada). Luego, el efecto de un campo magnético
externo sobre un medio material se puede resumir en una distribución de corriente estacionaria y
localizada dentro del medio, el potencial en ~x debido a esta corriente de magnetización está dado
por
~ M (~x) = µ0
A
4π

13.5.

ˆˆ
J~M (~x0 )
µ0  
x0 )
0 σM (~
dx
x)
+
  dS(~
| ~x − ~x0 | 4π δV
| ~x − ~x0 |
V

˚

3 0

Leyes fundamentales en un medio magnetizado

Queremos ver como se pueden reescribir las leyes fundamentales del campo magnético en el
interior de un medio material. En todo punto dentro del material, se tendrán una densidad de
corriente de carga libre, J~L (~x), y una densidad de corriente de magnetización J~M (~x). Es decir
~ x) = J~L (~x) + J~M (~x)
J(~
Escribiendo la ecuación rotacional para el campo magnético, se debe incluír por supuesto
la densidad de corriente total


~ ×M
~ (~x)
~ x) = µ0 J~L (~x) + ∇
~ × B(~
~ x) = µ0 J(~
∇
Equivalentemente

~ ×
∇

!
~ x)
B(~
~ (~x) = J~L (~x)
−M
µ0

~ x)
~ x) = B(~
~ (~x), y entonces
Definimos el campo H(~
−M
µ0

~ × H(~
~ x) = J~L (~x)
∇
La gracia es que al lado derecho aparece únicamente la densidad de corriente libre. To~ x) a través de la densidad
do el efecto del medio magnetizado se encuentra contenido en H(~
~ (~x). Las ecuaciones fundamentales en un medio magnetizado son,
de momento magnético M
entonces
~ · B(~
~ x) = 0
∇
~ × H(~
~ x) = J~L (~x)
∇
Notar la total analogía con las leyes fundamentales de la electrostática en un medio
~ · D(~x) = ρL (~x)
∇
~ × E(~
~ x) = 0
∇

donde ρL (~x) es la densidad de carga libre. Recordar además que en ciertos materiales lineales,
homogéneos e isotrópicos

---

### Página 83

~ x) = E(~
~ x),  > 0
D(~
Esto se obtuvo de suponer que los momentos dipolares se alineaban en la dirección del campo
eléctrico y que la respuesta era lineal en el campo eléctrico. De esta forma las dos ecuaciones
fundamentales de la electrostática podían ser escritas como
~ · E(~x) = ρL (~x)
∇

~ × E(~
~ x) = 0
∇
donde la única diferencia con las leyes en el vacío es la permitividad , no necesariamente
igual a 0 . (de hecho, siempre es mayor o igual). Notar que esto implica que el efecto de un
medio dieléctrico es el de disminuír la magnitud del campo eléctrico en su interior. En cambio,
con el campo magnético, podría suceder que el material aumentara la magnitud del campo
magnético total, lo que veremos a continuación

13.6.

Relaciones constitutivas del material

Se tiene

~
~ (~x)
~ x) = B(~x) − M
H(~
µ0

~ (~x) es, por supuesto, una función del campo magnético
La magnetización M
~ (~x) = G(
~ B(~
~ x))
M
En consecuencia
o equivalentemente

~ x) = B(~
~ x) − G(
~ B(~
~ x))
H(~
~ x) = F (H(~
~ x))
B(~

~ y cada componente de H
~ es
Si el medio es lineal, la relación entre cada componente de B
lineal
~ b (~x)
~ a (~x) = Fab (~x)H
B
~ x) y H(~
~ x) es la misma en cada
Si el medio es homogéneo, entonces la relación entre B(~
punto
~ a (~x) = Fab H(~
~ x)b
B
Por último, si el medio es isotrópico, Fab = µδab , o simplemente
~ x) = µH(~
~ x)
B(~
donde µ es una constante llamada permeabilidad magnética del material.
Con esto las leyes fundamentales quedan de la siguiente manera
~ · B(~
~ x) = 0
∇
~ × B(~
~ x) = µJ~L (~x)
∇

---

### Página 84

Es decir, la ley de Ampère es exactamente la misma, exceptuando que ahora la permeabilidad no es necesariamente igual a la del vacío. Lo interesante es que para ciertos medios,
llamados paramagnéticos, µ > µ0 , y el material magnetizado tiende a aumentar la magnitud
del campo magnético. Por el contrario, para medios llamados diamagnéticos µ < µ0 , y la
magnitud del campo magnético es debilitada

13.7.

Ferromagnetismo

Existe otro tipo de materiales, llamados ferromagnéticos. En ellos existe una interacción
fuerte entre momentos magnéticos cercanos. Este tipo de materiales está constituído por dominios, como se ilustra en la figura . Un campo magnético externo tiende a alinear los momentos magnéticos en la dirección paralela al campo externo. La interacción entre los momentos
magnéticos vecinos causa un alineamiento mucho más fuerte

El aumento en la magnitud del campo magnético puede ser considerable, de hecho la magnitud el campo magnético en el interior de un material ferromagnético puede ser 103 o 104
veces mas grande que la del campo externo aplicado. El comportamiento de un material ferromagnético es no lineal, de forma que no podemos caracterizarlo por una permeabilidad
~ = F (H)
~ no es monovalente, o dicho de otra formagnética constante. De hecho, la relación B
ma, depende de la historia previa del material. Este fenómeno es conocido como histéresis. En
la figura se muestra la variación de la magnetización ante la prescencia de un campo magnético
externo, partiendo desde a

Fig. 13.2: Curva de histéresis
Notar que cuando el campo magnético externo vuelve a ser nulo (c), una magnetización sigue
presente. Es decir, la fuerte interacción entre momentos magnéticos cercanos puede mantenerlos alineados, incluso cuando un campo magnético externo se reduce a cero. Estos momentos

---

### Página 85

alineados puede producir campos magnéticos fuertes, sin la necesidad de un campo magnético
externo, este es el origen de los imagnes permanentes.

---

### Página 86

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 87

#### Capítulo 14
Ley de Inducción de Faraday
Los campos eléctricos y magnéticos que hemos considerado hasta ahora han sido producidos por cargas y corrientes estacionarias. A principios del siglo XIX ya era bien sabido que
imponiendo una diferencia de potencial entre dos conductores, el campo eléctrico en el interior
originaba una corriente de electrones, que a su vez crea un campo magnético a su alrededor.
Era válido entonces preguntarse si un campo eléctrico podía o no ser producido por un campo
magnético. Diversos intentos se realizaron, hasta que en 1831, Michael Faraday descubrió que
una corriente eléctrica se genera en un conductor cuando éste se mueve en la cercanía de
un imán. Pero, en su época, tal fenómeno, conocido ahora como inducción magnética, no
parecía ser más que una simple curiosidad.
El notable físico Richard Feynman contaba en sus cursos de Física en Caltech, que cuando Faraday presentó su descubrimiento a la comunidad científica, alguien le preguntó para
qué servía, a lo cual Faraday respondió con otra pregunta: ¿para qué sirve un recién nacido?
Medio siglo después, Tomás Edison tuvo la idea de utilizar el descubrimiento de Faraday para
generar corriente eléctrica y distribuirla a través de cables por la ciudad de Nueva York. La
primera planta eléctrica de la historia fue inaugurada en 1881, y consistía en unas enormes
turbinas de vapor que hacían girar unas grandes bobinas de alambre conductor alrededor de
imanes. Debido al efecto Faraday se generaba una corriente eléctrica que se podía transmitir
por toda la ciudad. La energía térmica se convertía, así, en energía eléctrica. Pocos meses
después se inauguró la primera planta hidroeléctrica, en la que el agua de un río hacía girar las
bobinas.
Toda la electricidad que consumimos hoy en día se genera gracias al efecto Faraday. Lo único que
varía es el mecanismo utilizado para hacer girar una bobina alrededor de un imán: este mecanismo puede ser el flujo del agua en una presa, el funcionamiento de un motor de combustión de
petróleo, la presión del vapor de agua calentada por el uranio en una planta nuclear, en otras
palabras, Faraday descubrió el principio fundamental de la conversión electromecánica de
la energía (el recién nacido creció espectacularmente, como diría Feynman).

---

### Página 88

El experimento de Faraday consiste en una espira conductora y un imán.

Faraday mostró que el galvanómetro no mide ninguna corriente cuando el imán está estacionario
con respecto a la espira. Sin embargo, se induce una corriente cuando existe un movimiento
relativo entre el imán y la espira, en particular, el galvanómetro marca en una dirección cuando
el imán se acerca, y en la dirección opuesta cuando el imán se aleja.

14.1.

Ley de Inducción

La descripción formal es la siguiente, sea Γ una curva que describe la forma del conductor,
entonces
˛
~ x, t)
εΓ (t) =
d~x · E(~
Γ[t]

Es la fuerza electromotriz inducida en Γ. Notar que es una cantidad dinámica que puede
evolucionar en el tiempo, ya que ahora aceptaremos que los campos eléctricos y magnéticos
puedan variar con el tiempo. Del mismo modo
¨
~ x) · B(~
~ x, t)
ΦB (t) =
dS(~
SΓ (t)

es el flujo magnético a través de SΓ
El experimento de Faraday muestra que una corriente eléctrica es inducida en la espira al
cambiar el flujo magnético que la atraviesa. Se comporta entonces como si estuviera conectada
a una fuente de f.e.m. Experimentalmente se encuentra que esta f.e.m inducida depende de la
tasa a la que varía el flujo magnético a través de la espira, esto es
εΓ = −

dΦB
dt

---

### Página 89

La unidad SI del flujo magnético es el Weber (W b) = 1 T m2
La ley de Faraday se puede enunciar como sigue: La f.e.m inducida en un circuito cerrado es
igual a la tasa negativa de cambio del flujo magnético a través del área encerrada por la espira
El signo menos indica que la corriente inducida en la espira tiende a oponerse a este cambio
de flujo. Existen muchas formas de inducir una fem en una espira. Por ejemplo si consideramos
un caso particular en donde el campo magnético es uniforme (espacialmente), la espira es plana
y su normal forma un ángulo ϑ con el campo magnético, se tiene

 
 

d(BS cos ϑ)
dS
dϑ
dB
ε=−
S cos ϑ − B
cos ϑ + BS sin ϑ
=−
dt
dt
dt
dt
A partir de esto, vemos que una f.e.m inducida se puede producir de las siguientes formas
~ en el tiempo (por ejemplo ocurre cuando en un circuito
1. Al variar la magnitud de B
cercano la corriente varía)

~ es decir, el área encerrada por la espira en el tiempo
2. Al variar la magnitud de S,

~ y el vector de superficie S
~ en el tiempo
3. Al variar el ángulo entre B

Este último es el principio más utilizado en centrales de generación
Es fácil obtener el sentido de la corriente inducida, ya que ésta produce un campo magnético
que tiene a oponerse al cambio del flujo magnético que induce dicha corriente. Ésta se conoce
como Ley de Lenz. (aunque se deduce completamente de la ley de Inducción!)

---

### Página 90

~ x, t) y B(~
~ x, t), variables en
Esta ley, que introduce una relación dinámica distante entre E(~
~ yB
~ son objetos físicos reales. No son intermediarios puramente
el tiempo, sugiere que E
matemáticos introducidos para facilitar los cálculos 1

14.2.

Forma diferencial de la ley de Inducción

Consideremos un circuito de prueba Γ fijo, es decir Γ(t) = Γ
˛
¨
d
~ x, t) = −
~ x) · B(x,
~
dS(~
t)
εΓ(t) = dx · E(~
dt S(Γ)
Γ
˛

Γ

~ x, t) = −
dx · E(~

¨

S(Γ)

~ x) ·
dS(~

Por el teorema de Stokes
¨
¨


~ × E(~
~ x, t) = −
dS(~x) · ∇
S(Γ)

S(Γ)

∂ ~
B(x, t)
∂t

~ x) ·
dS(~

∂ ~
B(x, t)
∂t

válido para todo S(fijo), luego se obtiene la ley diferencial de Faraday
~ × E(~
~ x, t) + ∂ B(~
~ x, t) = 0
∇
∂t

Esta es una de las ecuaciones de Maxwell para campos que varían en el tiempo, y es una
~ x), en donde sólo para casos estáticos (la primera parte
generalización para el rotor de E(~
del curso)
~ x) = 0
~ × E(~
∇
~ es conservativo.
Notar, que sólo en ése caso el campo E

Hypothesis non fingo de Newton se viene abajo en Electromagnetismo

---

### Página 91

Problema
La espira rectangular de la figura se encuentra sumergida en un campo magnético uniforme
~ = B x̂. Si la espira gira con velocidad angular w utilizando el eje z como eje de rotación, y
B
asumiendo que en t = 0 la espira se encuentra en el plano y-z, determine la fuerza electromotriz
inducida y la corriente inducida en la espira

#### Solución
Definiendo la normal a la espira rectangular como en la figura

Según ésta definición, la normal es en todo instante igual a −êφ , es decir
n̂ = −(− sin φx̂ + cos φŷ) = sin φx̂ − cos φŷ

De esta forma, y dado que el campo magnético es uniforme, el flujo a través de la espira es
¨
~ x) · B(~
~ x) = B
~ ·S
~=B
~ · S n̂ = BS sin φ
dS(~
ΦB =
S

Es decir
ΦB = Bab sin φ
Tenemos una expresión del flujo magnético a través de la espira en función del ángulo polar
φ. La idea es obtener el flujo en función del tiempo, para ello observamos que
dφ
= w → φ(t) = wt + C
dt
La constante C es fácil de determinar, considerando que en t = 0, la espira se ubica en el
eje y-z, es decir, φ0 = π/2. Así
ΦB = Bab sin(wt + π/2)

---

### Página 92

A partir de la ley de inducción de Faraday, podemos obtener la magnitud de la fem inducida
en la espira
dΦB
= −Babw cos(wt + π/2)
dt
Vemos que la fem es alterna y varía de forma sinusoidal, como se aprecia en la figura
ε=−

Esta es la forma típica de generación alterna. La tensión que llega a nuestras casas también
varía de forma sinusoidal, a una frecuencia de 50 Hz y valor efectivo de 220 Volts.
La magnitud de la corriente es, simplemente
I=

|ε|
Babw
=
cos(wt + π/2)
R
R

---

### Página 93

Problema
Considere la disposición que se muestra en la figura. Suponga que R = 6Ω, l = 1, 2 m y un
campo magnético uniforme de 2, 5 T está dirigido hacia el interior de la página.
a) ¿A qué rapidez deberá moverse la barra para producir una corriente de 0,5 A en la resistencia?
b) Calcule la fuerza que se debe ejercer sobre la barra en este caso

#### Solución
a) Consideremos el circuito cerrado formado por la barra y los rieles.

~ = −S k̂. (Hacia dentro del papel) Supongamos que la
Definamos al vector de superficie como S
barra se encuentra a una distancia x del riel izquierdo, según esto, el flujo magnético sobre la
superficie plana encerrada por este circuito es
ΦB = BA = Blx
Ahora, utilizando la ley de Faraday obtenemos que la fem inducida en el circuito
ε=−

dΦ
d
dx
= − (Blx) = −Bl
dt
dt
dt

Pero dx/dt es simplemente la velocidad de la barra, así
ε = −Blv

---

### Página 94

La correspondiente corriente inducida es
|ε|
Blv
=
R
R
Y el sentido de ésta se deduce de la ley de Lenz. Notemos que mientras la velocidad de la barra
sea positiva (y entonces se mueve hacia la derecha) el flujo magnético aumenta. Le ley de Lenz
dice que la corriente inducida intentará siempre oponerse al cambio de flujo magnético que la
origina. Es decir, el sentido de la corriente será tal que intentará frenar a la barra.
I=

Notar que en la figura anterior se ha supuesto un sentido para la corriente. Éste podría
ser correcto o no. Según el sentido de la corriente que aparece en la figura, habrá una fuerza
magnética sobre la barra en la direccion −î, que justamente intentará frenar a la barra, por lo
tanto ese será el verdadero sentido de la corriente. Despejando
v=

RI
Bl

reemplazando los valores numéricos
v=

6 × 0,5
= = 1m/s
2,5 × 1,2

b) Vemos que sobre la barra actúan dos fuerzas

La fuerza externa es la fuerza que se debe ejercer sobre la barra para que se mueva a velocidad
v. La fuerza magnética tiene relación con la corriente inducida que circula por el circuito, cuyo
equivalente es

La fuerza magnética que experimenta la barra es simplemente
~ ×B
~ = I(lĵ) × (−B k̂)
F~B = I L
2 2

B l v
F~B = −IlB î = −
î
R
que apunta en la dirección opuesta a ~v . Para que la barra se mueva a velocidad constante, la
fuerza neta actuando sobre ella debe ser igual a cero. Así
2 2

B l v
î
F~ext = −F~B =
R

---

### Página 95

Notar que la potencia entregada por F~ext es igual a la potencia disipada en la resistencia
(consecuencia de la conservación de la energía)
2 2 2

B l v
P = F~ext · ~v = Fext v =
R
P =

ε2
(Blv)2
=
= I 2R
R
R

---

### Página 96

Problema
Una barra conductora de masa m y resistencia R desliza entre 2 rieles conductores sin fricción que forman un ángulo ϑ con la horizontal. y están separados una distancia l. Un campo
~ es aplicado verticalmente. La barra se suelta del reposo y desliza habia
magnético uniforme B
abajo.

a) La corriente inducida en la barra. ¿En qué dirección fluye, de a hacia b o de b hacia a ?
b) La velocidad terminal de la barra
Una vez alcanzada la velocidad terminal
c) Cual es la corriente inducida?
d) A qué tasa se disipa energía en la resistencia?
e) Cual es la tasa de trabajo ejercido por la gravedad?
#### Solución
a) Supongamos que en un instante dado la barra se encuentra a una distancia x del extremo,
como se ve en la figura

El circuito formado por los rieles y la barra que desliza encierra una superficie plana cuya
normal es
n̂ = sinϑx̂ + cosϑŷ
Y el flujo a través de esta superficie es
¨
~ x) · B(~
~ x) = B
~ · S n̂ = BS cos ϑ = Bxl cos ϑ
ΦB =
dS(~
S

Con esto, la fem inducida en los extremos de la barra es
ε=−

dx
dΦB
= −Bl cos ϑ
dt
dt

---

### Página 97

Así, la corriente inducida está dada por
I=

Bl
dx
|ε|
=
cos ϑ
R
R
dt

La magnitud de la corriente es tal que se opone al cambio de flujo, es decir, debe ser tal que
sobre la barra actúa una fuerza magnética en la dirección -x̂.
~ ×B
~ = IL
~ × B ĵ
F~B = I L
De aquí es claro que la corriente debe ir en la dirección k̂ (es decir de b hacia a), de forma que
F~B = IlB k̂ × ĵ = −IlB x̂
b)

Se tiene además que

d2 x
mg sin ϑ − FB cosϑ = m 2
dt
d2 x
mg sin ϑ − IlBcosϑ = m 2
dt

Recordando que
I=

Bl
dx
cos ϑ
R
dt

se tiene
d2 x
l2 B 2 2 dx
cos ϑ
=m 2
R
dt
dt
2 2
dx
l B
dx
cos2 ϑ
= 2
g sin ϑ −
mR
dt
dt

mg sin ϑ −

A − Bv =
dt =

dv
dt

dv
(A − Bv)

t − t0 = −

ln(A − Bv)
B

−B(t − t0 ) = ln(A − Bv)
Finalmente
e−B(t−t0 ) = A − Bv

---

### Página 98

A
− e−B(t−t0 ) = v
B B
Si t0 = 0

l2 B 2
mR
mRg sin ϑ
v(t) = 2 2 2 − 2 2 2 e− mR cos ϑt
l B cos ϑ l B cos ϑ
Para encontrar la velocidad terminal, simplemente vemos que ocurre en el límite cuando
t→∞

vt =

mgRtgϑsecϑ
l2 B 2

c) La corriente terminal está dada por
Bl
mgtgϑ
cos ϑvt =
R
lB
d) El módulo de la fem inducida en esta situación es
I=

| ε |=

mgRtgϑ
lB

la tasa a la cual se disipa energía en la resistencia es la potencia que consume, esta es
P =| ε | I =

m2 g 2 Rtg 2 ϑ
l2 B 2

e) La tasa de trabajo ejercida por la gravedad es
Pg = Fg vt
donde Fg es la componente de la fuerza gravitacional en la dirección del desplazamiento
m2 g 2 Rtg 2 ϑ
l2 B 2
que es lo mismo que la potencia que disipa la resistencia. Esto debe tenerse por el principio
de conservación de la energía
Pg = mg sin ϑvt =

---

### Página 99

Problema
Una espira de alambre en forma de rectángulo de largo l y ancho w, y un alambre recto paralelo
al lado l y que lleva una corriente I, yacen sobre una mesa.
La distancia entre el alambre largo y el lado izquiero de la espira es h.
a) Determine el flujo magnético que atraviesa la espira.
b) Suponga que la corriente es una función del tiempo con I(t) = a + bt, con a y b constantes
positivas. ¿Cuál es la f.e.m inducida en la espira y la dirección de la corriente inducida?
#### Solución

Usando la ley de Ampère para el alambre recto se obtiene que el campo a una distancia r
de éste está dado por
~ = − µ0 I k̂
B
2πr
~ = −S k̂ de modo
Es decir, apunta hacia dentro del papel. Definimos el vector de área como S
que ΦB > 0. Para obtener el flujo total, simplemente debemos sumar los flujos sobre todos los
pequeños elementos de área de largo l y ancho dr encerrados por la espira
¨
¨
~ · dS
~
ΦB =
dΦB =
B
S

ΦB =

µ0 Il
2π

Finalmente

ˆ h+w
h

S

µ0 Il
dr
=
(ln(h + w) − ln(h))
r
2π

µ0 Il 
w
ΦB =
ln 1 +
2π
h

b)Utilizando la ley de Faraday
d
dΦB
=−
ε=−
dt
dt



µ0 Il 
w
ln 1 +
2π
h



Como las dimensiones de la espira permanecen constantes, lo único que varía en el tiempo
es la corriente, y entonces
w  dI
µ0 l 
ε = − ln 1 +
2π
h dt
y sabemos que dI/dt = b, así
µ0 lb 
w
ε=−
ln 1 +
2π
h
Ahora, notemos que el alambre recto de corriente I produce un flujo magnético a través de la
espira entrando a la pagina. Por la ley de Lenz, la corriente inducida en la espira debe fluír
en el sentido contrareloj para así producir un campo magnético saliendo a través de la página
para contrarrestar el incremento del flujo hacia adentro.

---

### Página 100

Problema
Una espira rectangular de dimensiones l y w se mueve con velocidad constante ~v alejándose de
un alambre recto infinitamente largo que lleva corriente I en el mismo plano de la espira. Sea
la resistencia total de la espira R. ¿Cuál es la corriente en la espira en el instante en que el lado
más cercano está a una distancia r del alambre?
#### Solución

Sabemos que el campo magnético a una distancia x del alambre recto está dado por
~ = − µ0 I k̂
B
2πx
Apuntando hacia dentro del papel debido a la dirección de la corriente. Ahora, el flujo magnético
sobre un elemento diferencial de área de largo l y ancho dx en la espira es
~ · dS
~ = µ0 I ldx
dΦB = B
2πx
donde hemos escogido el vector de superficie apuntando hacia dentro de la página, para que
ΦB > 0. Integrando sobre toda la espira
ˆ
µ0 Il r+w dx
ΦB =
2π r
x
µ0 Il 
w
ΦB =
ln 1 +
2π
r
el mismo resultado del problema anterior. Derivando con respecto a t, obtenemos la fem inducida




dΦB
µ0 Il
µ0 Il d
1 dr
r+w
ε=−
=−
=−
ln
−
dt
2π dt
r
2π
r + w r dt
donde dr/dt es simplemente el módulo de la velocidad de la espira




µ0 Ilv r − r − w
µ0 Ilv
=−
−
ε=−
2π
r+w r
2π
r(r + w)
w
µ0 Ilv
2π r(r + w)
Y la corriente inducida será simplemente
ε=

I=

w
µ0 Ilv
|ε|
=
R
2πR r(r + w)

---

### Página 101

Problema
Una barra conductora de masa m y resistencia R es empujada en la dirección horizontal a través
de dos rieles sin fricción apartados una distancia l, mediante un hilo de masa despreciable que
pasa a través de una polea ideal y que está conectada a un bloque de masa M . Un campo
magnético uniforme es aplicado verticalmente hacia arriba. La barra parte del reposo.

a) Sea la velocidad de la barra en algún instante igual a v. Encuentre una expresión para la
corriente inducida. En qué dirección fluye, de a hacia b o de b hacia a?
b) Resuelva la ecuación diferencial para la velocidad de la barra en función del tiempo.
#### Solución
a) Sea nuestro origen de coordenadas la esquina inferior del sistema como se aprecia en la figura

~ = S k̂,
Es una situación muy similar a la del problema 2, si escogemos el vector de superficie S
entonces el flujo a través del circuito será positivo.
Supongamos que cuando la velocidad es v, la barra está a una distancia horizontal x del origen,
así
ΦB = Bxl
y la fem inducida es
ε=−

dΦB
dx
= −Bl
= −Blv
dt
dt

La corriente inducida será

Blv
|ε|
=
R
R
b) Sea x la coordenada x del centro de masa de la barra en el instante t. El equilibrio de
fuerzas para la barra es
I=

X

~ = T î − Il~j × B k̂ = (T − IlB)î = m dx î
F~ = T î − I~l × B
dt2

---

### Página 102

Para la masa M

dy
F~ = M g − T = M 2
dt
Debemos notar que dx /dt = dy /dt , así
X

Mg − M

dx2
dy 2
=
M
g
−
M
=T
dt2
dt2

Así, el equilibrio de fuerzas para la barra queda
(M g − M

dx2
dx2
−
IlB)
=
m
dt2
dt2

dx2
l2 B 2
v = (m + M ) 2
Mg −
R
dt
Por último, hay que notar que v = dx/dt, y obtenemos una ecuación diferencial para v
l2 B 2
Mg
dv
+
v−
=0
dt R(M + m)
M +m
la solución es de la forma
B 2 l2

v(t) = Ce− R(M +m) t +

M gR
l2 B 2

y la condición inicial es que v(0) = 0, así
C+
Finalmente

M gR
M gR
=0→C=− 2 2
l B
l B

M gR
v(t) = 2 2
l B



2 2

B l
− R(M
t
+m)

1−e



---

### Página 103

Problema
Un disco en cuyo borde se encuentra una carga uniformemente distribuída q, pende de un hilo
vertical. En la región r < a existe un campo magnético uniforme B k̂.
Se desconecta la fuente de campo magnético, disminuyendo éste uniformemente a 0 en un intervalo corto de tiempo. Si el momento de inercia del disco es I, calcule la velocidad angular
final de éste.

#### Solución
Inicialmente, se tiene un flujo constante a través de la región r < a dado por
ΦBi = Bπa2
donde hemos elegido la normal a la superficie según la dirección k̂, de manera que ΦB > 0.
Ahora, tomemos la curva C que coincide con el borde del disco, y utilizando la ley de Faraday
˛
~ · d~l = − dΦB
E
dt
E2πb = −

dΦB
dt

lo que se puede reescribir como
E2πbdt = −dΦB
E=−

1 dΦB
2πb dt

Este campo eléctrico genera una fuerza sobre cada elemento de carga en el borde del disco

---

### Página 104

~ = Eλbdϑϑ̂
dF
En consecuencia, se produce un diferencial de torque dado por
~ = Eλb2 dϑk̂
d~τ = br̂ × dF
d~τ = −

1 dΦB 2
λb dϑk̂
2πb dt

λb dΦB
dϑk̂
2π dt
El torque total a un tiempo t estará dado por
ˆ 2π
λb dΦB (t)
dϑ
~τ = −
2π dt
d~τ = −

~τ = −λR

dΦ(t)
dt

~ es el momento angular del disco con respecto al centro, entonces
Si L
~τ =

~
dL
dτ

dΦB (t)
dL
=
dt
dt
ˆ tf
ˆ tf
dΦB (t)
dL
dtλb
dt
−
=
dt
dt
−λb

−λb (ΦB (tf ) − ΦB (0)) = Lf − Li
si el disco parte del reposo, Li = 0, y además ΦB (tf ) = 0
λbπa2 B = Iwf
wf =

λRπa2 B
I

---

### Página 105

Problema
Se considera una bobina con N espiras cuadradas de lado a sin un medio material en el interior.
Cada espira está a distancia b de un alambre recto y muy largo que lleva una corriente I =
I0 sin wt, con w constante. Además, todas las espiras cuadradas son coplanares con el alambre
recto. Calcule, en función de los datos I0 , w, a, b, la fem inducida entre los terminales de la
bobina

#### Solución
El campo magnético del alambre recto se obtiene fácilmente por la ley de Ampère, pues por
la extensión infinita del alambre el campo debe tener una simetría cilíndrica radial, y debe ser
tangente a trayectorias que son circunferencias concéntricas al alambre. De esta forma
˛
~ x) = 2πrB(r) = µo I(t)
d~x · B(~
Γ

donde Γ es una circunferencia concéntrica al alambre, de radio r

Calculemos ahora el flujo por una sola espira, como se muestra en la figura

Se tiene
Φ=

¨

S

~ x) · B(~
~ x)
dS(~

---

### Página 106

donde S es la superficie plana encerrada por la espira cuadrada. El campo magnético en el
plano de la espira está dado por
~ x) = − µ0 I(t) k̂
B(~
2πx
Escogiendo la normal unitaria en el sentido −k̂, el flujo magnético queda


ˆ a ˆ a
µ0 I(t)a
a+b
µ0 I(t)
=
ln
Φ(t) =
dy
dx
2πx
2π
b
El flujo será el mismo sobre cada una de las N espiras, de forma que el flujo total sobre la
bobina es


a+b
N µ0 I(t)a
ΦT (t) = N Φ(t) =
ln
2π
b
por la ley de Faraday, se inducirá una fem sobre la bobina dada por
dΦT (t)
dt


a+b
N µ0 wa
cos wt
ln
ε(t) = −
2π
b
ε(t) = −

---

### Página 107

Problema
Una bobina circular plana de N vueltas tiene diámetro D y resistencia R. La bobina se orienta
~ = B k̂ uniforme, y los extremos de la bobina se
con su eje paralelo a un campo magnético B
conectan a un dispositivo capaz de medir la carga que pasa a través de él. Si la bobina se gira
en 180 grados sobre un eje perpendicular al campo magnético, el dispositivo mide una carga
Q. Encuentre el valor de B en términos de N, D, R y Q

#### Solución
En la situación inicial, el flujo magnético a través de la bobina es constante y está dado por
¨
~ x)
Φ=N
dS(~x)n̂(~x) · B(~
S

orientando la normal a la espira según n̂ = k̂, se tiene
¨
¨
dS(~x)k̂ · B k̂ = N B
dS(~x) = N Bπ (D/2)2
Φ=N
S

S

La espira se gira en 180 grados, de forma que la situación final es la siguiente

Mientras la espira gira, se induce una fem ε entre sus extremos, ya que el flujo magnético
Φ varía. Si se induce una fem, se induce una corriente
I(t) =

ε(t)
R

ε(t) = −

dΦ(t)
dt

y

---

### Página 108

Supongamos que la espira demora un tiempo T en girar en 180 grados, luego la carga que
pasará por el detector es
ˆ T
ˆ T
ε(t)
Q=
dtI(t) =
dt
R
ˆ
1 T dΦ(t)
= − (Φ(T ) − Φ(0))
Q=−
dt
R 0
dt
R
donde

Φ(0) = N Bπ (D/2)2

mientras que
Φ(T ) = −N Bπ (D/2)2
luego

N BπD2
Q=
2R

Finalmente
B=

2QR
πN D2

---

### Página 109

Problema
Un tren de masa m se desplaza inicialmente con velocidad v0 î. Ingresa a una región de frenado
electromagnético para disminuír la velocidad del tren, en donde existe un campo magnético
uniforme, en el sentido que se muestra en la figura. Encuentre la velocidad del tren en función
del tiempo. El largo del tren es L

#### Solución
Analizamos un instante cualquiera cuando el tren ha entrado x(t) < L a la región de campo B

Sea Γ la curva que encierra al área que ha ingresado a la zona de campo magnético, en el
sentido indicado por la figura. Así, la normal exterior está dirigida según k, y el flujo a través
de la espira es
¨
¨
~
~
Φ(t) =
dS(~x) · B(~x) =
dS(~x)B = aBx(t)
S(Γ)

S(Γ

por la ley de inducción, habrá una fem inducida en el circuito Γ
dΦ(t)
= −aB ẋ(t)
dt
El signo menos da el sentido de la corriente inducida, como muestra la figura
ε(t) = −

Por ley de mallas, la corriente del circuito en el sentido de la figura está dada por
IR = aB ẋ(t)
aB
ẋ(t)
R
Por otro lado, en cada segmento del circuito hay una fuerza por unidad de largo dada por
~
~ De la figura es claro que las fuerzas sobre las secciones horizontales se cancelan
I × B.
I=

---

### Página 110

F~ = −Iaĵ × B k̂ = −IaB î
De esta forma, la segunda ley de Newton para el tren entrega
−IaB = m

d2 x
dt2

pero
I(t) =

aB ẋ(t)
R

−(aB)2 ẋ(t)
= mẍ(t), x(t) < L
R
−(aB)2 dx(t)
d2 x(t)
, x(t) < L
=m
R
dt
dt2
Resolviendo para v(t)
−(aB)2
dv(t)
v(t) =
mR
dt
La solución es
(aB)2

v(t) = v0 e− mR t , t < t∗
con x(t∗) < L. Este tiempo puede ser obtenido mediante x(t)


(aB)2
v0 mR
− mR t
1−e
x(t) =
(aB)2
la solución es válida para todo t tal que x(t) < L . Una vez que el tren ha ingresado
completamente a la región de campo magnético, el flujo se mantiene constante, luego no hay
fuerzas sobre el tren y se mantendrá con velocidad constante igual a v(t∗ )

---

### Página 111

Problema
Considere un generador que consta de un electroimán que genera un campo magnético constante. Una espira de área A gira con velocidad angular constante w como se ve en la figura. Si
los terminales de la espira se conectan a una resistencia R, calcule la potencia consumida por
ésta. Calcule además la potencia necesaria para producir el movimiento rotatorio de la espira.

#### Solución
El flujo magnético que atraviesa la espira es, dado que el campo magnético es uniforme
~ · dS
~ = BAcos(ϑ)
ΦB = B
ΦB = BAcos(wt)
Así, la tasa a la que varía el flujo magnético es
dΦB
= −BAwsin(wt)
dt
Utilizando la ley de Faraday, obtenemos la f.e.m inducida en el circuito
ε=−

dΦB
= BAwsinwt
dt

Si el circuito se conecta a una resistencia R, la corriente a través de ésta será
I=

BAw
|ε|
=
sinwt
R
R

Notemos que es una corriente alterna, cuya amplitud máxima es
I0 =

BAw
R

Ahora, la potencia suministrada al circuito eléctrico es
P = |ε|I =

(BAw)2
sin2 wt
R

Por otro lado, el torque necesario para producir el movimiento rotatorio de la espira es
τ = µBsinθ = µBsinwt
donde µ es la magnitud del momento magnético de la espira
µ = IA → τ = IABsinwt

---

### Página 112

B 2 A2 w
sin2 wt
R
Por último, la potencia mecánica necesaria está dada por
τ=

Pm = τ w =

B 2 A2 w2
sin2 wt
R

Como era de esperarse, la potencia mecánica entregada es igual a la potencia consumida
por el circuito.

---

### Página 113

Problema
Considere una espira rectangular de lado a y masa m, en el plano y-z, sumergida en un campo
~ = (B0 − αz)x̂, con α > 0. La espira cae en la dirección vertical debido a la
magnético B
gravedad. Encontrar la fem y corriente inducida en función de la velocidad ~v de la espira. ¿Cuál
es la velocidad terminal?

#### Solución
Definiendo la normal a la espira rectangular según n̂ = x̂, y suponiendo que el extremo inferior
se encuentra a una altura z, el flujo mangético a través de la espira está dado por
¨
¨
ˆ a ˆ z+a
~
~
ΦB =
dS · B =
dydzB(z) =
dy
dz(B0 − αz)
S

S

z

α 2 z+a
aα 2
z )z = a2 Bo −
(z + 2az + a2 − z 2 )
α
αa3
ΦB = a2 Bo − (2za2 + a3 ) = a2 (B0 − αz) −
Con esto, y utilizando la ley de inducción de Faraday, podemos determinar la fem inducida
en la espira
dΦB dz
dΦB
=−
= −ż(−αa2 )
ε=−
dt
dz dt
ΦB = a(B0 z −

ε = vαa2
Donde v es la rapidez con que cae la espira. Podemos distinguir dos casos, si la espira sube,
entonces v > 0 y ε > 0, lo que nos dice que la corriente inducida irá en el sentido contrareloj,
como se aprecia en la figura

Otra forma de verlo, es notando que el campo magnético se hace más débil en la medida
que aumenta la altura z, de forma que si la espira sube, el flujo disminuye. Así, la corriente
inducida debe ir en una dirección tal que el flujo que ésta genere se sume al flujo magnético

---

### Página 114

externo e intente evitar que el flujo total disminuya
Ahora, el caso de interés (la espira cae por gravedad), implica v < 0, de forma que ε < 0 y
esto significa que la corriente va en el sentido indicado por la siguiente figura. Otra forma de
verlo es notando que si la espira cae, el flujo magnético aumenta, luego la corriente inducida
debe generar un flujo magnético opuesto de manera de oponerse a este aumento.

La magnitud de la corriente está dada por
I=

αa2 | v |
|ε|
=
R
R

Ahora, para encontrar la velocidad terminal de la espira, necesitamos encontrar la ecuación
de movimiento. Calculemos la fuerza magnética que actúa sobre la espira. Podemos descomponer la fuerza total como la suma de las fuerzas sobre 4 segmentos

Es fácil notar que sobre los segmentos verticales 2 y 4, las fuerzas se anulan (el campo no
depende de la coordenada y y la corriente tiene sentido inverso en ambos segmentos). Ahora,
la fuerza sobre el segmento 1 es
F~1 = IaB(z + a)(−ŷ × x̂) = IaB(z + a)k̂
Y para el segmento 2

F~2 = IaB(z)(ŷ × x̂) = −IaB(z)k̂

La fuerza total es
F~ = Ia(Bo − α(z + a) − B0 + αz)k̂ = −Ia2 αk̂
2 4

α av
F~ = −
k̂
R

---

### Página 115

Notar nuevamente que si v > 0 (sube), entonces la fuerza intenta hacer caer a la espira. Si
por otro lado, la espira cae v < 0 y entonces la fuerza magnética es hacia arriba. Finalmente,
la ecuación de movimiento es
dv
α 2 a4 v
=−
− mg
dt
R
=0
Para encontrar la velocidad terminal, imponemos dv
dt
m

mg
α2 a4
El signo menos indica que finalmente la espira cae con velocidad constante dada por | vt |
vt = −R
