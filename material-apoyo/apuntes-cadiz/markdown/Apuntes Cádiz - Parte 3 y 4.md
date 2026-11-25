---
title: "Parte 3 y 4"
source_pdf: "Electro/material-apoyo/apuntes-cadiz/Apuntes Cádiz - Parte 3 y 4.pdf"
pages: 109
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Parte 3 y 4

### Página 1

Parte III
El campo en medios materiales

---

### Página 2

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 3

#### Capítulo 10
Dieléctricos
10.1.

El campo en medios Dieléctricos

Aquí comenzamos a discutir otra de las propiedades interesantes de la materia bajo la
influencia de un campo eléctrico. Anteriormente consideramos el comportamiento de los conductores, en donde hay cargas libres para moverse en respuesta a un campo eléctrico de forma de
cancelar el campo en el interior del conductor. Ahora discutiremos qué sucede con los aislantes,
materiales que no conducen electricidad. Uno podría creer primeramente que no debería haber
efecto alguno, sin embargo, usando un condensador de placas paralelas, Faraday descubrió que
ésto no es así. Sus experimentos mostraron que la capacidad aumenta en un factor κ que depende únicamente de la naturaleza del material asilante. Éstos materiales también son llamados
dieléctricos, el factor κ es una propiedad del dieléctrico (y se llama constante dieléctrica). La
constante dieléctrica del vacío es, por supuesto, 1. A continuación se derivará el comportamiento de un dieléctrico en un campo externo y se aplicará al cálculo de capacidades con dieléctricos.
Todos los medios materiales se componen de moléculas, las que a su vez se componen de
entes cargados (núcleos atómicos y electrones), y las moléculas de los dieléctricos son, de hecho, afectadas por la prescencia de un campo eléctrico externo. El campo eléctrico produce
una fuerza que se ejerce sobre cada partícula cargada, empujando las partículas positivas en
la dirección del campo, y las negativas en sentido opuesto, de modo que las partes positivas
y negativas de cada molécula se desplazan de sus posiciones de equilibrio, sin embargo estas
cargas moleculares no están libres para moverse muy lejos o ser extraídas del material (lo que
sí ocurre en conductores).
El efecto total, desde el punto de vista macroscópico, se visualiza como un desplazamiento
de toda la carga positiva en el dieléctrico en relación a la carga negativa (Se produce una
colección de dipolos!). A esto se le llama polarización. Existen 2 tipos de dieléctricos, unos
son los dieléctricos polares, que tienen momentos dipolares permanentes. Un ejemplo de este
tipo de dieléctrico es el agua.

---

### Página 4

La orientación de las moléculas polares ante la ausencia de un campo es totalmente aleatoria.
~ 0 es aplicado, un torque causa que las moléculas se alinien en la dirección
Cuando un campo E
~ 0 . (ver último problema de ayudantía 9)
de E
El otro tipo de dieléctrico son los no polares, que no poseen momentos dipolares permanentes, pero que de igual forma se polarizan ante un campo eléctrico externo. Las moleculas
polarizadas son como dipolos y se alinean en la dirección del campo.

~ 0 . En
La figura ilustra la orientacion de las moléculas no polares con y sin campo externo E
ambos tipos de dieléctricos, ante la prescencia de un campo eléctrico externo, se produce una
polarización. Un dieléctrico polarizado, aun cuando sea eléctricamente neutro en promedio,
produce un campo eléctrico en los puntos exteriores e interiores al dieléctrico.

10.1.1.

Polarización

Vimos que si un medio se polariza, se efectúa una separación de cargas positivas y negativas,
y un elemento de volumen se caracterizará entonces por un momento dipolar eléctrico, ∆~p. Se
define P~ , el momento dipolar eléctrico por unidad de volumen
∆~p
P~ =
∆v
Estrictamente, P~ debe definirse como el límite de esta cantidad a medida que ∆v se hace muy
pequeño desde el punto de vista macroscópico. De esta forma, P~ se convierte en una función
puntual P~ (x, y, z), llamada Polarización del medio (Es, de hecho, un campo vectorial). Sus
dimensiones son carga por unidad de área.

10.1.2.

Campo de un Medio Dieléctrico

Consideremos un pedazo finito de dieléctrico polarizado, es decir, que se caracterize en
cada punto ~x0 por su polarización P~ (~x‘). La polarización da origen a un campo eléctrico. Para
encontrarlo, encontremos primero el potencial en un punto P .

---

### Página 5

Cada elemento de volumen d3 x0 se comporta como un dipolo microscópico, y entonces se caracteriza por un momento dipolar ∆~p(~x0 ) = P~ (~x0 )d3 x0 , y como la distancia entre ~x y d3 x0 es
grande comparada con las dimensiones de d3 x0 , el potencial en ~x será
∆~p(~x0 ) · (~x − ~x0 )
P (~x0 ) · (~x − ~x0 )d3 x0
=
dφ(~x) =
4π0 |~x − ~x0 |3
4π0 |~x − ~x0 |3
(Recordar el potencial de un dipolo!). El potencial en el punto ~x se obtiene sumando las contribuciones de todas las partes del dieléctrico, luego
φ(~x) =
4π0

d3 x0 P~ (~x0 ) · (~x − ~x0 )
|~x − ~x0 |3
V

˚

Esta integral puede evaluarse directamente si se conoce la forma funcional de P~ (~x0 ). En la
práctica eso no se hace, resulta ventajoso desarrollar aún más esta expresión. Usando la ya
conocida identidad
~0
∇

~x − ~x0
=
|~x − ~x0 |
|~x − ~x0 |3

El potencial queda
φ(~x) =
4π0

˚

~0
d3 x0 P~ (~x0 ) · ∇

V

|~x − ~x0 |

El siguiente paso consiste en utilizar la siguiente identidad
~ 0 · F~ + F~ · ∇
~ 0f
~ 0 · (f F~ ) = f ∇
∇
Donde f es cualquier función escalar y F~ un campo vectorial. Con esto, si utilizamos f =

y F~ = P~ (~x0 )
|~
x−~
x0 |

~0
P~ (~x0 ) · ∇

~ 0
~ 0 · P~ (~x0 )
~ 0 · P (~x ) −
∇
=
∇
|~x − ~x |
|~x − ~x | |~x − ~x |

Con esto
φ(~x) =
4π0

˚
P~ (~x0 )
~ 0 · P~ (~x0 )
d x∇ ·
d3 x0
−
∇
0|
|~
x
−
~
x
|
4π
|~
x
−
~
x
V
V

˚

3 0~ 0

La primera integral puede transformarse en una integral sobre una superficie cerrada mediante el teorema de la divergencia, obteniendo

---

### Página 6

ˆˆ
˚
1  ~ 0
P~ (~x0 )
3 0
~ 0 · P~ (~x0 )
φ(~x) =
x)·
d
x
−
∇
 dS(~
0|
4π0 S
|~x − ~x0 | 4π0
|~
x
−
~
x
V
O, equivalentemente
ˆˆ
˚
~ 0 ~ x0 )
~ x0 ) · n̂(~x0 )
1 
0 P (~
3 0 −∇ · P (~
+
φ(~x) =
x)
d
x
 dS(~
4π0 S
|~x − ~x0 |
4π0
|~x − ~x0 |
V
~ · P~ (~x) son dos funciones escalares obtenidas a partir de la
Las cantidades P~ (~x) · n̂(~x) y −∇
polarización P~ (~x). Es conveniente asignar a estas cantidades símbolos especiales, y como tienen
dimensiones de carga por unidad de área y carga por unidad de volumen, respectivamente,
escribiremos
σ(~x) = P~ (~x) · n̂(~x)
~ · P~ (~x)
ρ(~x) = −∇
Y llamaremos a σ y ρ densidades de carga de polarización. La densidad superficial
de carga de polarización está dada por la componente de polarización normal a la superficie,
y la densidad volumétrica de carga de polarización es una medida de la no uniformidad de la
polarización dentro del material.
En resumen, el potencial debido al material dieléctrico es, finalmente
ˆˆ
˚
1 
σ(~x0 )
x0 )
3 0 ρ(~
φ(~x) =
x)
d
x
+
 dS(~
4π0 S
|~x − ~x0 | 4π0
|~x − ~x0 |
V
De esta expresión es evidente que proviene de una distribución de carga. En otras palabras,
el material dieléctrico se ha sustituido por una distribución adecuada de carga de polarización.
~ x) = −∇φ(~
~ x)
El campo eléctrico se obtiene usando el hecho E(~
ˆˆ
˚
1 
x0 )(~x − ~x0 )
x0 )(~x − ~x0 )
0 σ(~
3 0 ρ(~
~
E(~x) =
x)
+
d
x
 dS(~
4π0 S
|~x − ~x0 |3
4π0
|~x − ~x0 |3
V
Notemos que la carga de polarización total de un cuerpo dieléctrico es
˚
ˆˆ

3 0
0 ~
~
Qp =
d x (−∇ · P (~x )) +   dS(~x0 )P~ (~x0 ) · n̂(~x0 )
V

S(V )

Utilizando el teorema de la divergencia, es evidente que Qp = 0, (como debe ser!) Esto
concuerda con que un dieléctrico, como un todo, es eléctricamente neutro.

10.2.

Ley de Gauss en un Dieléctrico, Desplazamiento
Eléctrico

Es sabido que una de las leyes fundamentales de la electrostática es la ley de Gauss. Esta
ley dice que el flujo eléctrico a través de cualquier superficie cerrada es proporcional a la carga
total encerrada por la superficie. Al aplicar la ley de Gauss a una región que contiene cargas

---

### Página 7

libres dentro de un dieléctrico, hay que tener cuidado en incluír todas las cargas dentro de la
superficie gaussiana, tanto la carga de polarización como la carga libre

Consideremos una superficie S cerrada imaginaria colocada dentro de un medio dieléctrico.
Consideremos cierta cantidad de carga libre Q, contenida en el volumen limitado por S 0 . La ley
de Gauss entrega
ˆˆ
˚
ˆˆ
Q


 ~ 0
~ x)= +
d3 x0 ρ(~x0 )
x )σ(~x ) +
x ) · E(~
  dS(~
 dS(~



S
S
ˆˆ
˚
ˆˆ
Q
1  ~ 0 ~ 0
 ~ 0
~
~ 0 P~ (~x0 )
x ) · E(~x ) = +
d3 x0 ∇
x ) · P (~x ) −
  dS(~
 dS(~



S
S
ˆˆ
ˆˆ
1  ~ 0 ~ 0
1 
Q
~ x0 ) · P~ (~x0 )
= +
x ) · P (~x ) −
  dS(~
  dS(~
0 0 S 0
0 S+S 0
Así

 ~ 0
 ~ 0
~ x0 ) = Q − 1 
x ) · E(~
x ) · P~ (~x0 )
 dS(~
 dS(~

ˆˆ

0

S

0

ˆˆ

S

Equivalentemente
ˆˆ

ˆˆ

 ~ 0
 ~ 0
~ x0 ) = Q − 
x ) · E(~
x ) · P~ (~x0 )
0  dS(~
 dS(~
S

S

ˆˆ

 ~ 0
x)·
 dS(~
S




~ x0 ) + P~ (~x0 ) = Q
0 E(~

Se define el Desplazamiento eléctrico como
~ x) + P~ (~x)
~ x) = 0 E(~
D(~
~ queda
La ley de Gauss, en términos de D
˚
ˆˆ
 ~ 0
~
x ) · D(~x ) = Q =
 dS(~
S

d3 x0 ρlibre (~x0 )

S(V )

Esta es la Ley de Gauss generalizada a un dieléctrico, notar que Q representa únicamente la carga libre, es decir, toda la información sobre la polarización del medio se encuen~ x0 ). Notar que si no hay dieléctrico (espacio vacío), se tiene P~ (~x)= 0,
tra contenida en D(~
~ x) = 0 E(~
~ x) y
D(~
ˆˆ
 ~ 0
~ x0 ) = Q
0  dS(~
x ) · E(~
S

que es la ley de Gauss usual para el vacío.

---

### Página 8

10.3.

Forma diferencial de la Ley de Gauss General

A partir de la ley de Gauss
ˆˆ

 ~ 0
~ x0 ) =
x ) · D(~
 dS(~
S

˚

d3 x0 ρ(~x0 )

V (S)

Aquí, ρ(~x0 ) representa la densidad volumétrica de carga libre. Utilizando el teorema de la
divergencia
˚
¨
3 0~
~ x)=
d x ∇ · D(~
d3 x0 ρ(~x0 )
V (S)

V (S)

De donde se obtiene la forma diferencial de la ley de Gauss general
~ · D(~
~ x0 ) = ρ(~x0 )
∇
Esta es la primera ecuación de Maxwell reescrita para un medio material. Notar que la
~ tiene la ventaja de conservar como fuentes únicamente las cargas lidefinición del vector D
~
bres. El efecto de las cargas de polarización están contenidas en D.

10.4.

Susceptibilidad Eléctrica y constante Dieléctrica

~ x) se anula. Como éste es
Para la mayoría de los materiales, P~ (~x) se anula cuando E(~
el comportamiento más común, nos limitaremos a los materiales de este tipo. Además, si el
material es isotrópico, la polarización deberá tener el mismo sentido que el campo eléctrico que
la provoca. Esto se resume en
~ x)
P~ (~x) = χ(E)E(~
Donde la cantidad escalar χ(E) se llama susceptibilidad eléctrica del material. Así, una
~ x) en medios isotrópicos sería
expresión para D(~
~ x) = (E)E(~
~ x)
~ x) = (0 + χ(E))E(~
D(~
Donde (E) = 0 + χ(E) es la permitividad del material. Experimentalmente χ y  son
independientes del campo eléctrico para campos no muy intensos. En otras palabras, χ y  pasan
a ser constantes características del material. Materiales de este tipo se llaman dieléctricos
lineales, y se tiene
~ x)
P~ (~x) = χE(~
~ x) = E(~
~ x)
D(~
Es más conveniente trabajar con una cantidad adimensional, κ, definida por
κ=


= r
0

Esta constante se llama constante dieléctrica, de manera que
~ x) = E(~
~ x) = 0 κE(~
~ x)
D(~

---

### Página 9

Notar que κ es siempre mayor que 1, excepto en el vacío, donde κ = 1. La primera ecuación
de Maxwell en este tipo de medios queda
~ · E(~x) = ρ(~x) = ρ(~x)
∇

κ0
Eso significa que en un medio dieléctrico, el campo eléctrico es debilitado por un
factor κ.

10.5.

Condiciones de borde en la frontera

Las condiciones que deben satisfacer el campo eléctrico en una zona interfacial que separa
dos madios dieléctricos se deducen a partir de las leyes diferenciales
~ · D(~
~ x) = ρ(~x)
∇
~ × E(~
~ x) = 0
∇
En cualquier zona interfacial entre dos medios se puede construír una superficie cilíndrica
como se muestra en la figura

Integrando la ley de Gauss general sobre el volumen limitado por el cilindro se obtiene
˚
˚
3 ~
~
d x∇ · D(~x) =
d3 xρ(~x)
V

V




¨

ˆˆ

~ x) · D(~
~ x) =
dS(~

V (S)

d3 xρ(~x)

V

si h → 0, entonces
(D1n − D2n ) A = σA
donde A es la superficie de las tapas, y σ es la densidad superficial de carga en la frontera que
~ x) es discontinua al atravesar
divide a los dos medios. Así, la componente normal del campo D(~
una superficie cargada
D1n − D2n = σ

---

### Página 10

o, equivalentemente para medios lineales
1 E1n − 2 E2n = σ

Ahora veremos que la componente tangencial del campo eléctrico es continua. A partir de
la ecuación
~ × E(~
~ x) = 0
∇
Integremos esta ecuación sobre una superficie plana rectangular como la de la figura

El contorno de S es el camino Γ indicado en la figura. Utilizando el teorema de Stokes
ˆˆ

 ˛
 ~
~ x) = 0
~ × E(~
~ x) = d~x · E(~
 dS(x̂) · ∇
S

Γ

En el caso en que h1 → 0, h2 → 0

lE1t − lE2t = 0
~ x) debe ser continua al atravesar
De aquí se deduce que la componente tangencial de E(~
una interfaz entre dos medios
lE1t = lE2t

~ x) y D(~
~ x)
En resumen, al atravesar una interfaz entre dos medios (1 y 2), los campos E(~
satisfacen
E1t = E2t
D1n − D2n = σ

---

### Página 11

10.5.1.

Condensadores con Dieléctricos

Un material no conductor, ancho t, área A y constante dieléctrica κ se inserta en el espacio
entre placas de un condensador con distancia d entre placas, carga Q y área A. No es necesario
que el dieléctrico esté en la mitad del espacio entre placas

Para encontrar la capacitancia, calculemos primero la diferencia de potencial entre placas.
Ya se vió que en auscencia de dieléctrico, el campo eléctrico entre las placas está dado por
E0 = σ0 = 0QA , y entonces ED = Ek0 . El potencial se puede encontrar integrando el campo
eléctrico sobre una curva vertical desde la placa superior a la inferior
ˆ −
Q
Q
dxE = −phi0 + phiD = −E0 (d − t) − ED t = −
(d − t) −
∆φ = −
t
A0
A0 κ
+
∆φ = −
Con esto se obtiene
C=

Q
(d − t(1 − ))
A0
κ

Q
0 A
=
|∆V |
d − t(1 − κ1 )

Notemos algunos límites, por ejemplo cuando t → 0, es decir, cuando el ancho del dieléctrico tiende a cero, se obtiene C = 0 Ad = C0 , que es la capacidad esperada para cuando no hay
dieléctrico.
Cuando κ = 1, nuevamente se obtiene C = 0dA = C0 , ya que al ser κ = 1, el dieléctrico es
simplemente vacío.
En el límite cuando t → d, el espacio está totalmente lleno de dieléctrico, y se tiene
κ0 A
= κC0
d
Es decir, un condensador lleno de dieléctrico aumenta su capacidad en el factor κ!
C=

---

### Página 12

Problema
Calcular la capacidad del condensador de la figura

#### Solución
El problema se puede tratar como 2 condensadores en paralelo, uno formado por los dieléctricos
de constante κ1 y κ2 , y el otro formado por dieléctrico de constante κ3 y vacío.
El primer condensador (C1 ), se puede ver como 2 condensadores en serie, llenos de los dieléctricos 1 y 2, así
= 0 + 00
C1
C1 C1
Con
κ1 0 S1
C10 =
d1
C100 =

κ2 0 S1
d2

d1
d2
=
+
C1
κ1 0 S1 κ2 0 S1
De donde se obtiene
κ1 κ2 0 S1
d1 κ2 + d2 κ1
Para el condensador C2 , se procede de manera similar, esto es
C1 =

= 0 + 00
C2
C2 C2
Donde
C20 =
C200 =

 0 S2
d1

κ3 0 S2
d2

Donde se obtiene
κ3 0 S2
d1 κ3 + d2
Finalmente, como C1 y C2 están en paralelo, la capacidad total será
C2 =

C = C1 + C2 =

κ1 κ2 0 S1
κ3 0 S2
+
d1 κ2 + d2 κ1 d1 κ3 + d2

---

### Página 13

Problema
Se tiene un condensador plano de área A en el vacío, y se carga con una batería. El condensador
obtiene una carga Q. Luego, se desconecta de la batería y se llena la mitad del espacio entre
placas con un dieléctrico de permitividad 2 . Calcular
a) la nueva diferencia de potencial entre las placas
b) las densidades superficiales de carga en cada placa
c) las densidades de carga de polarización del dieléctrico

#### Solución
Sea el origen en un punto sobre la placa inferior. Se define el eje z como vertical y positivo
hacia arriba. Si escogemos un camino de integración Γ como una línea recta vertical desde la
placa superior hasta la inferior

podemos obtener la diferencia de potencial entre las placas como
ˆ
ˆ 0
~ x) =
~ x)
d~xE(~
φd − φo = V = d~x · E(~
d

Γ

Despreciando efectos de borde, el campo debe ser uniforme en la región interior, y además
apunta según −k̂. Ojo con la parametrización! se tiene l = d − t, con t = 0...d. De esta forma
dl = −dt y d~l = dtk̂ ,luego
ˆ 0
ˆ 0
~
d~x · E(~x) = −E
dt = Ed
V =
d

d

Luego E = Vd

La curva Γ fue escogida de manera arbitraria,y se podría haber escogido en la mitad donde
se encuentra el dieléctrico, sin embargo la diferencia de potencial entre las placas debe ser la
misma para ambos caminos de integración. Lo que esto significa es que el campo eléctrico debe
ser igual tanto en el vacío como en la región con dieléctrico. La única forma de que esto sea
posible es que se distribuyan densidades de carga superficial en los conductores, digamos σ1 y
σ2 no necesariamente iguales entre sí.

---

### Página 14

ahora, sabemos que en la región 1
D1 =  1 E =  0

V
d

y para la región 2

V
d
Además, utilizando la ley de Gauss con las superficies S1 y S2 de la figura:
ˆˆ
 ~ ~
 dS · D1 = D1 S = σ1 S
D2 =  2 E = 

S

luego

V
d
Equivalente, para la región 2 se obtiene de forma análoga
D1 = σ1 = 0

D2 = σ2 = 

V
d

Además, como la carga Q en la placa superior sólo se distribuye, la ley de continuidad
establece
A
V A
= Q = ( + 0 )
=Q
d 2
de aquí obtenemos la diferencia de potencial entre las placas del condensador
(σ1 + σ2 )

V =

2Qd
A( + 0 )

Notar que si  = 0 (y entonces el material dieléctrico es el vacío) el potencial es simplemente
el potencial inicial
Q
Qd
=
= Vo
V =
A0
C
b) Las densidades de carga superficial están dadas por
σ1 = 0
σ2 = 
Notar que
σ1

0 2Q
V
=
d
A( + 0 )

2Q
V
=
d
A( + 0 )

A
A
+ σ2 = Q

---

### Página 15

c) Calculemos ahora las densidades de polarización. Necesitamos encontrar σP y ρP en el
material dieléctrico. Tenemos que
~ · P~ = −χ∇
~ ·E
~
ρP = −∇
Ahora, en todos los puntos en el dieléctrico no hay densidad de carga libre, luego, de la
primera ecuación de Maxwell
~ ·D
~ =ρ=0
∇
~ = E
~ →∇
~ ·E
~ =0
y como D
Esto es válido en todos los puntos interiores al dieléctrico. Con esto
ρP = 0
Ahora, para obtener la densidad de carga superficial, se tiene
σP = P~ · n̂
donde n̂ es la normal a la superficie del dieléctrico.
Recordar que
D = E = 0 E + P
Luego
( − 0 )E = P
Ahora, en la superficie superior del dieléctrico se tiene n̂ = k̂ y
~ =−
E
Luego
σP = −

2Q
k̂
A( + 0 )

2Q
( − 0 )
A( + 0 )

Y la densidad en la placa inferior será, simplemente
−σP =

2Q
( − 0 )
A( + 0 )

se verifica que la carga total de polarización es cero

---

### Página 16

Problema
Una esfera de radio R con carga libre q está sumergida en un medio dieléctrico homogéneo de
constante κ y de extensión teóricamente infinita. Calcular
a) Los vectores campo eléctrico y polarización a distancia r de la carga puntual
b) La densidad de carga de polarización
#### Solución
~ D
~ y P~ son todos paralelos entre sí en cada punto, y por la simetría esférica,
a) Debido a que E,
la naturaleza radial del campo no cambia por la prescencia del medio dieléctrico. Además, estos
vectores pueden depender sólo de la distancia al centro de la esfera y no de alguna coordenada
angular.
Usando la ley de gauss general, con una superficie esférica de radio r (r > R) concéntrica a la
esfera de carga q
ˆˆ

 ~ 0
~ x0 ) = q
x ) · D(~
 dS(~
S

ˆˆ

ˆˆ



x0 ) = q
 dSD(r) = q → D(r)  dS(~
S

S

Con lo que
4πr2 D(r) = q
~
D(r)
=

q
r̂
4πr2

~
El campo eléctrico y la polarización pueden evaluarse con bastante facilidad al conocer D
~
~
~
D(r)
= κ0 E(r)
→ E(r)
=
además

q
r̂
4πκ0 r2

~ x) + P~ (~x)
~ x) = 0 E(~
D(~
~
P~ (r) = ( − 0 ) E(r)
=

q
q
q
r̂ − 0
r̂ =
4πr
4πκ0 r
4πr2



1−
κ



r̂ =

q(κ − 1)
P~ (r) =
r̂
4πκr2
b) Claramente el dieléctrico ha debilitado la magnitud del campo eléctrico (en comparación
al espacio vacío). El campo eléctrico es originado por toda la carga, la de polarización y la
carga libre. La carga libre es sólo la carga de la esfera q. Sin embargo, la carga de polarización
~ · P~ (~x) y una densidad
se forma de dos contribuciones, una densidad volumétrica ρP (~x) = −∇
superficial σP (~x) = P~ (~x)·n̂(~x) sobre la superficie del dieléctrico en contacto con la carga puntual.
Es claro que en todos los puntos del dieléctrico
~ · E(~
~ x) = 0
∇
y entonces

~ · P~ (~x) = 0
ρP (~x) = −∇

---

### Página 17

Usando que
q(κ − 1)
P~ (r) =
r̂
4πκr2
La densidad superficial será
σ = P~ · n̂ = P~ (R) · −r̂ = −

(κ − 1)q
4πκR2

y la carga superficial es
ˆˆ



QS =  dS(~x0 )σ(~x0 ) = −4πR2
S

QS = −

(κ − 1)q
4πκR2

(κ − 1)q
κ

Notar que la carga total será
(κ − 1)q
q
=
κ
κ
Otra forma de ver como campo eléctrico es menor en un factor κ, la carga se ve debilitada
por este factor de lo que sería si no hubiera un medio dieléctrico.
Q = Qlibre + QS = q −

---

### Página 18

Problema
Considere una cáscara esférica dieléctrica de radio interior a, radio exterior b y permitividad .
Se coloca una carga puntual q en su centro. Calcule el campo eléctrico en todo el espacio y las
densidades de carga de polarización

#### Solución
Tomando una superficie gaussiana esférica arbitraria de radio r > 0 concentríca con la carga
libre q, se tiene
ˆˆ
 ~ 0
~ x0 ) = 4πr2 D(r) = qin = q
x ) · D(~
 dS(~
S

Con esto

q
r̂
4πr2
para todo r > 0. Ahora, podemos obtener el campo eléctrico como sigue. En la región r < a,
se tiene
~
D(r)
=

~ I (r) =
E

q
r̂
4πo r2

~ II (r) =
E

q
r̂
4πr2

para a < r < b
y para r > b

q
r̂
4πo r2
Notar que el campo se debilita en la región interior del cascarón dieléctrico. Ahora,
~ III (r) =
E

~ · P~ (~x) = −∇
~ · ( − o ) E
~r = 0
ρP = −∇

---

### Página 19

Ahora, sea σin la densidad superficial de polarización en la cáscara interior y σext la densidad
superficial de polarización en la cáscara exterior

~ II (a) · (−r̂) = −
σin = ( − 0 )E

q( − 0 )
4πa2

~ II (b) · (r̂) = q( − 0 )
σext = ( − 0 )E
4πb2
se verifica que la carga total de polarización es cero

---

### Página 20

Problema
Se tiene un condensador esférico de radio interno a y externo b, el cual está lleno de un dieléctrico que tiene una constante dieléctrica κ.¿Cuál es la capacitancia de este condensador? Si el
condensador está cargado con una carga Q, encuentre la energía almacenada en él

#### Solución
Supongamos que el condensador tiene almacenada una carga Q, es decir, la pared r = a
está cargada con carga Q, mientras que la pared r = b se encuentra cargada con carga −Q. Se
puede determinar la capacitancia al determinar la diferencia de potencial entre estas superficies.
Utilizando la ley de Gauss general, con una superficie esférica de radio r, con a ≤ r ≤ b

ˆˆ

 ~
~ x) = Q
x) · D(~
 dS(~
S

~ x) = D(r)r̂ y entonces
dada la simetría radial, D(~
ˆˆ
 ~
~ x) = 4πD(r)r2 = Q
x) · D(~
 dS(~
S

de esta forma
~ x) = Q r̂, a ≤ r ≤ b
D(~
4πr2
Si el dieléctrico es lineal, homogéneo e isotrópico, entonces
~ x)
~ x) = 0 κE(~
D(~
donde κ es la constante dieléctrica del material. Luego
~ x) =
E(~

Q
r̂, a ≤ r ≤ b
4π0 κr2

---

### Página 21

Ahora, la diferencia de potencial entre los extremos del condensador es
ˆ b
~ x)
∆V = φ(a) − φ(b) =
d~x · E(~
a

tomando un camino radial de la forma ~x = rr̂, ≤ ar ≤ b, entonces d~x = drr̂


ˆ b
drQ
Q
1 1
∆V =
=
−
4π0 κ a b
a 4π0 κr

Finalmente

4π0 κ(b − a)
Q
=
∆V
ab
Es decir, es κ veces la capacidad de un condensador esférico en vacío
C=

C = κC0 > C0

---

### Página 22

Problema
Considere una espera conductora de radio interior a y radio exterior c. El espacio entre las 2
superficies es llenado con 2 dieléctricos distintos, de manera que la constante dieléctrica es κ1
entre a y b, y κ2 entre b y c. Determine la capacitancia del sistema

#### Solución
Para encontrar la capacitancia, podemos suponer que el condensador se encuentra cargado con
una carga Q, en este estado, habrá una cierta diferencia de potencial entre r = a y r = c. La
relación entre esta diferencial de potencial y la carga almacenada nos permitirá encontrar la
capacidad

Para encontrar ∆V = φ(a) − φ(c) necesitamos determinar el campo eléctrico en la región
Ω : a ≤ r ≤ c. Para ello, utilizamos la ley de Gauss general, para una superficie esférica de
radio r contenida en Ω
ˆˆ
 ~
~ x) = 4πr2 D(r)
x) · D(~
 dS(~
S

esto último dada la clara simetría esférica del problema. Por la ley de Gauss
ˆˆ
 ~
~ x) = Q
x) · D(~
 dS(~
S

De aquí es posible obtener el campo de desplazamiento eléctrico en Ω
Q
~
r̂, a ≤ r ≤ c
D(r)
=
4πr2
Suponiendo que los dieléctricos involucrados son lineales, homogéneos e isotrópicos, se tendrá
~ x)
~ x) = 0 κE(~
D(~

donde κ es la constante dieléctrica.

---

### Página 23

Así, para la región I (a ≤ r ≤ b)
~ x) = Q r̂, a ≤ r ≤ b
0 κ1 E(~
4πr2
Despejando
~ x) =
E(~

Q
r̂, a ≤ r ≤ b
4π0 κ1 r2

Análogamente, para la región II (b ≤ r ≤ c)
~ x) =
E(~

Q
r̂, b ≤ r ≤ c
4π0 κ2 r2

Con esto
∆V = φ(a) − φ(c) =

ˆ c

~ x)
d~x · E(~

a

tomando un camino radial de la forma ~x = rr̂ (para algun valor del ángulo ϑ), entonces
d~x = drr̂
ˆ c
ˆ b
drQ
drQ
+
∆V =
a 4π0 κ1 r
b 4π0 κ2 r
Luego
Q
= 4π0
C=
∆V



ab
κ2 bc
+
κ1 (b − a) c − b



Otra forma de resolver el sistema es notando que el condensador equivale a dos condensadores esféricos en serie. Recordando que la capacidad equivalente para un condensador esférico de radio interior r1 y radio exterior r2 , lleno de un dieléctrico lineal de constante κ está dado
por


r1 r 2
C = 4π0 k
r2 − r 1
Con lo que la capacidad equivalente del sistema está dada por

(b − a)
(c − b)
κ2 c(b − a) + κ1 a(c − b)
=
+
=
C
4π0 κ1 ab 4π0 κ2 bc
4π0 κ1 κ2 abc
Así
C=

4π0 k1 k2 abc
k2 c(b − a) + k1 a(c − b)

que es el mismo resultado obtenido anteriormente

---

### Página 24

Problema
Se tiene un condensador plano con placas cuadradas de largo a, distancia d entre placas, y una
carga total Q. Calcular la fuerza que se ejerce sobre un material dieléctrico cuando se encuentra
a una distancia x del punto O

#### Solución
La energía potencial asociada a esta configuración es
1 Q2
2 C(x)
Notar que es función de x, puesto que la capacitad total del condensador es función de x.
El sistema se puede ver como dos condensadores en paralelo
U (x) =

Ceq = C1 + C2 =
Ceq =

0 ax κ0 a(a − x)
+
d
d

0 a(x + κ(a − x))
d

Con esto, la energía potencial eléctrica almacenada es
dQ2
U (x) =
2 0 a(x + κ(a − x))
Y la fuerza que se ejerce sobre el dieléctrico será
Fx î = −

dU
î
dx

(1 − k)
Q2 d
F~x =
î
20 a (x + k(a − x)2 )
Notar que (1 − k) < 0, es decir, la fuerza apunta según - . Esto significa que la placa
dieléctrica es atraída hacia el interior del condensador.

---

### Página 25

Problema
Un condensador cilíndrico de altura l y cuyos conductores tienen radios a y b (b > a), está cargado con una carga Q, es decir, una armadura tiene carga +Q y la otra −Q. Entre ellas existe
vacío. La armadura es un cilíndro metálico macizo.
Este dispositivo se sumerge en un líquido dieléctrico de densidad constante ρ y permitividad ,
a una profundidad h.
Determinar la altura x que sube el nivel del líquido que queda dentro del condensador, en
relación al líquido externo (basta llegar a la ecuación correspondiente).

#### Solución
La diferencia de nivel ∆h estará dada por el equilibrio entre la fuerza eléctrica sobre el líquido
y su peso. Como la carga es constante, entonces
U=

1 Q2
2 C(x)

La fuerza electrostática es
∂U
î
∂x
Con C(x) la capacidad del condensador cuando el agua está a una altura x.
De esta forma,el problema se traduce en determinar la capacidad del condensador en función
de la altura x.
Fx î = −

La figura muestra que el condensador puede considerarse como dos condensadores conectados
en paralelo, uno de altura l − x y otro de altura x. La capacidad total será la suma de las
capacidades C1 , C2 .
Podemos hacer esta suposición (equivalente con 2 condensadores en paralelo) si despreciamos
los efectos de borde y la deformación del campo eléctrico cerca de la superficie del líquido.
Para calcular la capacidad del condensador de altura x, supongamos que hay una carga
q2 distribuida en el conductor interno. Así, utilizando un cilindro como superficie de gauss de
radio r, concéntrico al conductor interno y contenido en la región con dieléctrico, se tiene

---

### Página 26

ˆˆ

 ~ 0
~ x0 ) = q2
x ) · D(~
 dS(~

~
Si D(r)
= D(r)r̂, se tiene
~
D(r)
=

q2
r̂
2πrx

~
E(r)
=

q2
r̂
2πrx

De donde

Ahora podemos obtener el potencial entre los conductores como
 
ˆ b
q
b
~ · d~r =
∆V =
E
ln
2πx
a
a
Con lo que la capacidad para este condensador será
C2 =

2πx

ln ab

Análogamente se obtiene la capacidad para el condensador superior, que estará dada por
C1 =

2π0 (l − x)

ln ab

La capacidad total del sistema será la suma de ambas
C = C1 + C2 =
Y la energía eléctrica será
U (x) =

2π
 (x + 0 (l − x))
ln ab

1 Q2 ln(b/a)
4π x( − 0 ) + 0 l

Derivando se obtiene la fuerza que tiende a subir el agua
Fx î = −

dU
1 Q2 ln(b/a)( − o )
î
î =
dx
4π (x( − 0 ) + 0 l)2

Y el peso del líquido que es elevado una altura ∆h es
W = (x − h)π(b2 − a2 )ρ
Finalmente la ecuación para determinar x es
(x − h)π(b2 − a2 )ρ =

1 Q2 ln(b/a)(0 − )
4π (x( − 0 ) + 0 l)2

---

### Página 27

Problema
Dos esferas concéntricas conductoras de radio interior a y exterior b, respectivamente, poseen
cargas ±Q (como se muestra en la figura). La mitad del espacio entre ellas se llena con un
dieléctrico ( de constante dieléctrica /0 )

a) Encuentre el campo eléctrico entre las esferas
b) Calcule la densidad de carga libre superficial en la esfera interior
c) Calcule la densidad de carga de polarización inducida en la superficie del dieléctrico en r = a
#### Solución
a) Sea S una esfera de radio r concéntrica a ambas esferas conductoras, con a < r < b. De la
ley de Gauss general
ˆˆ
 ~
~ x) = Q
x) · D(~
 dS(~
S

De la simetria del problema, se deduce una dependencia y dirección radial para el campo
de desplazamiento eléctrico (y también para el campo eléctrico)
~ x) = D(r)r̂
D(~
Sean además S1 y S2 los hemisferios dados por
S1 = {~x ∈ S/0 ≤ ϕ ≤ π}
S2 = {~x ∈ S/π ≤ ϕ ≤ 2π}
S

Notar que S1 S2 = S
¨
ˆˆ
¨
 ~
~ x) · D(~
~ x) +
~ x) · D(~
~ x) = Q
~ x) =
dS(~
dS(~
x) · D(~
 dS(~
S

ˆˆ

 ~
~ x) =
x) · D(~
 dS(~
S

S1

¨

S2

~ x) +
~ x) · 0 κE(~
dS(~

S1

¨

~ x) = 2πrE(r)0 (1 + κ)
~ x) · 0 E(~
dS(~

S2

donde κ es la constante dieléctrica de la región asociada al hemisferio S1 , es decir
κ=


0

Así
~ x) =
E(~

2Q
4π0 r2 (1 + /0 )

r̂, a ≤ r ≤ b

---

### Página 28

b) Para encontrar la densidad de carga libre en la esfera r = a, utilizamos que
~ x) = σ(~x) , ∀~x ∈ Sa : {r = a}
D(~
(~x)

Así
σ1 = 0 E(a) =

Q0
2πa ( + 0 )

σ2 = E(a) =

Q
2πa2 ( + 0 )

c) Para encontrar la densidad de carga inducida en la superficie de dieléctrico con r = a,
utilizamos la relación
~ x) + P~ (~x) = E(~
~ x)
~ x) = 0 E(~
D(~
Así, el vector polarización está dado por
~ x)
P~ (~x) = ( − 0 ) E(~
La densidad de carga inducida de polarización en la superficie del dieléctrico con r = a es
σP = P~ · n̂

~
x∈Sa

donde n̂ es la normal a la superficie Sa que limita al dieléctrico, es decir n̂ = −r̂
σP = − ( − 0 ) E(r)
σP =



0 − 
0 + 



r=a

Q
2πa2

---

### Página 29

Problema
Un cascarón esférico macizo (radio interno a y externo b) está hecho de un material tal que la
polarización en su interior está dada por P~ (r) = kr r̂, donde k es una constante arbitraria y r la
distancia al centro. Note que no hay carga libre en este problema. Encuentre de dos maneras
distintas el campo eléctrico en todo el espacio
#### Solución
Una forma natural de resolver este problema consiste en encontrar las densidades de carga de
polarización, es decir , ρpol y σpol

La divergencia en coordenadas esféricas para una función radial de la forma f~ = f (r)r̂ es

En este caso


~ · f~ = 1 ∂ r2 f (r)
∇
r ∂r


∂
k
~ · P~ = −
r
ρP = −∇
r2 ∂r
r

k
ρP = − 2 , r ∈ (a, b)
r
Falta obtener además las densidades superficiales de polarización en r = a y r = b. Para
ello utilizamos que
σP = P~ · n̂
donde n̂ apunta hacia el exterior de la región de dieléctrico. Para la superficie r = a se tiene

en este caso, n̂ = −r̂, y entonces
σP

r=a

=

k
k
r̂ · (−r̂) = −
a
a

---

### Página 30

En r = b, la normal exterior a la región de dieléctrico coincide con n̂ = r̂, de forma que
k
k
r̂ · r̂ =
b
b
r=b
Dividimos el espacio en dos regiones, dadas por {I : a < r < b}, {II : b < r}. Tomando una
superficie esférica S de radio r tal que r > b, e integrando el flujo del campo eléctrico a través
de ella, se tendrá por ley de Gauss
ˆˆ
 ~
~ x) = Qin = 4πr2 E(r)
x) · E(~
 dS(~
0
S
σP

=

donde se ha utilizado la clara simetría radial del problema. La carga encerrada por S está dada por
˚
Qin = σa 4πa + σb 4πb +
d3 xρP (~x)
V (S)

La integral de la densidad volumétrica de carga de polarización es como sigue


˚
ˆ 2π
ˆ π
ˆ b
−k
d xρP (~x) =
dϕ
dϑ sin ϑ
drr
= −4πk (b − a)
r2
V (S)
a
Entonces
k
k
Qin = − 4πa2 + 4πb2 − 4πb (b − a) = 0
a
b
(Resultado totalmente conocido a estas alturas, pues un dieléctrico es eléctricamente neutro). De esta forma, el campo eléctrico en la región II es nulo
~ x) = ~0, ∀~x ∈ II
E(~
Para la región I, nuevamente utilizando la ley de Gauss con una superficie esférica de radio
r, ahora con a < r < b
ˆˆ
 ~
~ x) = 4πr2 E(r) = Qin
x) · E(~
 dS(~
0
S
donde ahora la carga encerrada por S es


ˆ 2π
ˆ π
ˆ b
−k
Qin = σa 4πa +
dϕ
dϑ sin ϑ
drr
r2
a
Qin = −4πka + 4πk (a − r) = −4πkr
Luego
4πr2 E(r) = −

4πkr
0

~ x) = − k r̂, a < r < b
E(~
0 r
~ x) = ~0 si r < a
Es claro, por ley de Gauss, que E(~

---

### Página 31

Otra forma de resolver este problema, es utilizando la ley de Gauss para el vector desplazamiento eléctrico. Utilizando una superficie S (cualquiera) contenida en la región II, se tiene
ˆˆ
 ~
~ x) = Qlibre
x) · D(~
 dS(~
S

donde Qlibre representa la carga libre encerrada por S. En este caso, Qlibre = 0 y entonces,
por continuidad
~ x) = ~0, ∀x ∈ II
D(~
Además, en la región II (vacío), la polarización es nula, P~ (~x) = ~0, ∀x ∈ II. Utilizando
además
~ x) = 0 E(~
~ x) + P~ (~x) = ~0 → E(~
~ x) = ~0, ∀x ∈ II
D(~

~ es nulo
Para la región I, se obtiene nuevamente que el campo D
ˆˆ
 ~
~ x) = ~0, ∀S ∈ I
x) · D(~
 dS(~
S

~ x) = ~0, ∀~x ∈ I
D(~
entonces

~ x) + P~ (~x) = ~0
0 E(~
~ x) = − 1 P~ (~x) = − k r̂
E(~
0
0 r

~ x) = ~0 para r < a por la misma razón ( D(~
~ x) = P~ (~x) = ~0 en r < a)
y, por supuesto, E(~

---

### Página 32

Problema
Un cilindro conductor hueco sin espesor, de radio r1 , y largo l, lleva una carga q uniformemente
distribuída. Alrededor de él, otro cilindro conductor hueco sin espesor, coaxial con el anterior,
de radio r2 y mismo largo l, tal como indicado en la figura, lleva una carga -q, también uniformemente distribuída. Se llena la región entre los dos cilindros con un material cuya constante
dieléctrica es función de la distancia al eje de los cilindros, κ = κ(r). Considere l mucho mayor
que r1 y r2

a) Encuentre una expresión para κ(r) que lleva un campo electrostático radial independiente
de la distancia al eje
b) Calcule la capacidad del condensador cilíndrico correspondiente
c) Calcule la densidad superficial de cargas de polarización en la superficie del material dieléctrico a r = r1 y r = r2 , para el κ(r) calculado en el ítem a)
~ ·A
~ = 1 ∂ (rAr ), calcular la densidad
d) Considerando que, en coordenadas cilíndricas , ∇
r ∂r
volumétrica de cargas de polarización en el dieléctrico
e) Calcular la cantidad total de cargas de polarización, incluyéndose cargas en la superficie y
en el volumen del dieléctrico
f) Calcule la energía potencial electrostática almacenada en el condensador
g) Suponiendo que uno puede sacar el material dieléctrico de entre r1 y r2 deslizándolo fácilmente sin roce, a lo largo del eje del sistema, calcule el trabajo necesario para remover el
dieléctrico de entre las placas del condesador
#### Solución
Para obtener el campo electrostático en el interior, utilizamos la ley de Gauss general, con una
superficie cilíndrica de radio r, con r1 < r < r2 y largo l

~ es de la forma D
~ = D(r)r̂, con esto
Por simetría, es evidente que D
ˆˆ
ˆˆ

 ~ 0
~
x ) · D(~x ) =  dS(~x0 )r̂ · D(r)r̂ = q
 dS(~
S

S

D(r)2πrlD = q
Así
~ =
D

q
r̂
2πrl

---

### Página 33

~ se relaciona con E
~ según
además D
~ x) = E(~
~ x) = κ(r)0 E(~
~ x)
D(~
luego
~
E(r)
=

q
r̂
2πlrκ(r)0

~ no dependa de r, κ(r) debe ser de la forma
para que E
κ(r) =

α
r

Así
~
E(r)
=

q
r̂
2πlα0

b) Calculemos la diferencia de potencial entre las cáscaras cilíndricas

ˆ B

~ x) = φ(A) − φ(B) = ∆V
d~x · E(~

A

ˆ r2

q
q
drr̂ ·
r̂ =
2πlα0
2πlα0
r1

ˆ r2

dr =

r1

q(r2 − r1 )
2πlα0

y la capacidad de este condensador es
C=

2πlα0
q
=
∆V
r 2 − r1

c) La densidad superficial de cargas de polarización está dada por
σP (~x) = P~ (~x) · n̂(~x), ~x ∈ S
y
sobre la superficie interior



~ = α − 1 0 E
~
P~ = ( − 0 E
r

---

### Página 34

n̂ = −r̂


α
~
P~ =
− 1 0 E
r1


α
q
r̂
P~ (~x) =
−1
r1
2πlα

y entonces

σ1 = P~ · n̂

=
r=r1

−




q
α
−1
r1
2πlα

para la superficie exterior

P~ =
luego
σ2 = P~ · n̂



n̂ = r̂

α
~
− 1 0 E
r2

r=r2

=




q
α
−1
r2
2πlα

d) La densidad volumétrica de carga de polarización es
~ · P~
ρP = −∇
como

P~ = P (r)r̂



~ · P~ = − 1 ∂ rP (r) = − 1 ∂ r α − 1 0 E
~
ρP = −∇
r ∂r
r ∂r
r
 


1 ∂
α−r
q
ρP = −
r
0
r ∂r
r
2πlα0




1 ∂ (α − r) q
1 −q
ρP = −
=−
r ∂r
2πlα
r 2πlα
ρP =

q
r2πlα

e) La carga total de polarización es
˚
ˆˆ
ˆˆ


3 0
Qp =
d x ρP (~x ) +   dS(~x )σ1 (~x ) +   dS(~x0 )σ2 (~x0 )
V

S1

S2

---

### Página 35



ˆˆ


x0 )σ1 (~x0 ) = −
  dS(~
S1




ˆˆ
α
q 
α
q2πr1 l
x)=−
−1
−1
  dS(~
r1
2πlα S1
r1
2πlα

q

x0 )σ1 (~x0 ) = − (α − r1 )
  dS(~

ˆˆ

α

S1

del mismo modo
q


x0 )σ2 (~x0 ) = σ2   dS(~x0 ) = (α − r2 )
  dS(~

ˆˆ

ˆˆ

S2

α

S1

por último, recordando que el elemento de volumen en coordenadas cilíndricas es d3 x0 =
rdrdϕdz
ˆ
˚
ˆ 2π
ˆ l ˆ r2
2πlq r2
q
3 0
=
drr
dr
d x ρP (~x ) =
dϕ
dz
2πlαr
2πlα r1
V
r1
˚
q
d3 x0 ρP (~x0 ) = (r2 − r1 )
α
V
Así

q
q
q
(r2 − r1 ) − (α − r1 ) + (α − r2 ) = 0
α
α
α
Esto siempre se cumple, pues un dieléctrico siempre es eléctricamente neutro, en efecto
˚
ˆˆ

3 0
~
~
~ x0 ) · P~ (~x0 ) = 0
QP =
d x − ∇ · P (~x ) +   dS(~
QP =

V

S(V )

f) La energía almacenada por el condensador es
U=
donde
C=

1 q2
2C

2πlα0
(r2 − r1 )

así
U=

1 q 2 (r2 − r1 )
2 2πlα0

g) Tenemos que la energía inicial es
Ui =

1 q 2 (r2 − r1 )
2 2πlα0

y la final
Uf =

1 q2
2 Cf

donde Cf es la capacidad final (en vacío).

---

### Página 36

Por ley de Gauss
 ~ 0
~ x0 ) = q = E2πrl
x ) · E(~
 dS(~

ˆˆ

0

S

~ =
E
y
∆V =

ˆ r2

~ =
d~x · E

r1

Así
Cf =

q
r̂
2πrl0

q
2πl0

ˆ r2
r1

q
dr
=
ln
r
2πl0



r2
r1

2πl0
q
=  
∆V
ln r2
r1

y la energía final

 
r2

1 q2
1 q ln r1
=
Uf =
2 Cf
2 2πl0

Finalmente, el trabajo necesario para remover el dieléctrico es

 
r 1 − r1
r2
1 q2
W = Uf − Ui =
− ln
2 2πl0
α
r1



---

### Página 37

Problema
Un condensador de placas paralelas de separación d entre las placas mucho menor que su largo
L y ancho w tiene la región entre las placas llenada por un material de constante dieléctrica κ,
el que puede deslizar libremente a lo largo de la dirección dada por L, como indicado en la figura. Inicialmente, el dieléctrico llena completamente la región entre las placas, y el condensador
está cargado con una carga total Q. Se pide determinar hasta qué distancia x uno tiene que
sacar el dieléctrico para que la energía almacenada en él aumente por un factor 2 con respecto
a su valor original, si la carga almacenada en el condensador se mantiene constante en el proceso

#### Solución
Antes de mover el dieléctrico, la capacidad es
Ci =

κ0 wL
d

y la energía inicial es
1 Q2
1 Q2 d
Ui =
=
2 Ci
2 κ0 wL
Supongamos que ahora se mueve el dieléctrico hasta una distancia x. Ahora el condensador
se puede pensar como dos condensadores en paralelo

---

### Página 38

la capacidad equivalente es
Ceq = C1 + C2 =

0 w
(x + κ(L − x))
d

y la energía final queda
1 Q2
Q2 d
U (x) =
=
2 Ceq x
2 0 w (x + κ(L − x))
se pide que
U (x) = 2Ui =

Q2 d
κ0 wL

Así, x debe cumplir
Q2 d
Q2 d
=
2 0 w (x + κ(L − x))
κ0 wL
2 (x + κ(L − x)) = κL
2x − 2κx + 2κL = κL → 2x (1 − κ) = −κL
x=

κL
2 (κ − 1)

---

### Página 39

Problema
Se tienen tres esferas conductoras concéntricas de radios a, b, y c. El espacio entre las dos
primeras está lleno con un dieléctrico de constante κ. Inicialmente la esfera de radio a está descargada y las esferas de radios b y c tienen carga q1 y q2 , respectivamente. La esfera interior de
radio a se conecta con la esfera de radio c con un cable aislado delgado

a) Calcular la carga libre en cada esfera
b) Calcular la carga de polarización en la superficie externa y en la superficie interna del
dieléctrico
#### Solución
a) Definimos las siguientes regiones

Al conectar las esferas de radio a y c, se distribuirá la carga en ambas de modo que quedan
al mismo potencial, luego
q2 = qA + q C
Además, para la región I

~ x) = ~0
r < a → E(~

pues corresponde al interior de una esfera conductora. Para a < r < b se utiliza la ley de Gauss
con una superficie esférica de radio r
ˆˆ

~ x0 ) · D(~
~ x0 ) = 4πr2 D(r) = qA
  dS(~
S(r)

~ = qA r̂
D
4πr2

---

### Página 40

y luego
~
E(r)
=

qA
r̂
4πκ0 r2

Para la región b < r < c
ˆˆ

~ x0 ) · E(~
~ x0 ) = 4πr2 E(r) = (qA + q1 )
dS(~
0
S(r)




q A + q1
~
E(r)
=
r̂
4π0 r2
Por último, para r > c
ˆˆ

~ x0 ) · E(~
~ x0 ) = 4πr2 E(r) = q1 + qA + qC
dS(~
0
S(r)




En resumen





~0

qA
r̂
4πκ0 r 2
~ x) =
E(~
qA +q1

2 r̂

0r
 qA4π
+q1 +qC
r̂
4π0 r 2

si 0 < r < a
si a < r < b
si b < r < c
si c < r

El potencial en una esfera de radio a es
ˆ ∞
ˆ b
ˆ c
ˆ ∞
~ =
~
~
~
φ(a) =
d~r · E
d~r · E(r)
+
d~r · E(r)
+
d~r · E(r)
a

a

b

c

donde la última integral corresponde a
ˆ ∞
~
d~r · E(r)
= φ(c) = φ(a)
c

qA
φ(a) =
4πκ0

ˆ b

dr qA + q1
+
4π0
a r

ˆ c
b

dr
+ φ(a)
r2

luego




qA + q1 1 1
1 1
qA
+
=0
−
−
4πκ0 a b
4π0
b c




c−b
b−a
qA
+ (qA + q1 )
=0
ab
bc
b−a
c−b
+ (qA + q1 )
=0
ab
cb


b
q1 (b − c)
b
b(c − a)
b−c
qA
=
−1+1−
→ qA
= q1
a
c
c
ac
c
qA

Finalmente

qA =

q1 (b − c)a
b(c − a)

---

### Página 41

qC = q2 − qA = q2 −

q1 (b − c)a
b(c − a)

b) Sobre la superficie interna del dieléctrico

σP = P~ · n̂
~
P~ = ( − 0 ) E
sobre la superficie
~ =
E

qA
r̂
4πκ0 a2

y n̂ = −r̂
σa = −

( − 0 ) qA
(κ − 1) qA
=
−
4πκ0 a2
4πκa2

y sobre la superficie externa

~ =
E

qA
r̂
4πκ0 b2
n̂ = r̂

luego
σb = P~ · n̂ = ( − 0 )
σb =

qA
4πκ0 b2

(κ − 1) qA
4πκb2

---

### Página 42

Problema
Una esfera dieléctrica de radio a y permitividad  se coloca en un campo eléctrico inicialmente
uniforme, como se muestra en la figura

Encuentre el potencial φ y el campo eléctrico en todo el espacio
#### Solución
Dada la simetría esférica del problema, resolveremos el problema en coordenadas esféricas, como
se muestra en la figura

Como no hay cargas libres, el potencial electrostático satisface la ecuación de Laplace
~ 2φ = 0
∇
Dada la simetría azimutal (el potencial no depende del ángulo polar ϕ), la solución general
para r < a y r > a toma la forma
φint =

∞
X

Al rl Pl (cos ϑ)

l=0

φext =

∞
X
l=0


Bl rl Pl + Cl r−(l+1) Pl (cos ϑ)

~ x) = E0 z, o, equivalentemente
Lejos de la esfera dieléctrica, E(~
φ∞ = −E0 z
en coordenadas esféricas
φ∞ = −E0 r cos ϑ
Es decir
lím φ(r, ϑ) = φ∞ = −E0 r cos ϑ

r→∞

---

### Página 43

lím φext =

r→∞

∞
X

Bl rl Pl (cos ϑ) = −E0 r cos ϑ

l=0

De aquí, es claro que

Bl = 0, l = 0, 2, 3, 4...
y
B1 r cos ϑ = −E0 r cos ϑ
B1 = −E0
con esto, el potencial exterior toma la forma
φext = −E0 r cos ϑ +

∞
X

Cl r−(l+1) Pl (cos ϑ)

l=0

Ahora utilizaremos las condiciones de contorno en la superficie r = a. En primer lugar, la
componente tangencial del campo eléctrico en r = a debe ser continua
~ int · ϑ̂
E
~ int · ϑ̂
−∇φ

r=a

r=a

~ ext · ϑ̂
=E

r=a

~ ext · ϑ̂
= −∇φ

r=a

1 ∂φint
1 ∂φext
=−
a ∂ϑ r=a
a ∂ϑ r=a
de forma equivalente, se puede imponer
−

φint
∞
X

r=a

= φext

l

Al a Pl (cos ϑ) = −E0 a cos ϑ +

l=0

∞
X

Cl a−(l+1) Pl (cos ϑ)

l=0

∞
X
l=0

De aquí, se obtiene

r=a


Al al − Cl a−(l+1) Pl (cos ϑ) = −E0 a cos ϑ
A1 a −

C1
= −E0 a
a2

y para l 6= 1
Al al − Cl a−(l+1) = 0, l 6= 1

Además, si no hay densidad de carga libre en la superficie dieléctrica, la componente normal
~ x) es continua
del campo D(~
~ int · r̂
~ ext · r̂
D
=D
r=a

r=a

---

### Página 44

~ int · r̂
−∇φ
−



∞
X

r=a

~ ext · r̂
= −0 ∇φ

r=a

∂φext
∂φint
= −0
∂r r=a
∂r r=a

Al lal−1 Pl (cos ϑ) = 0

−E0 cos ϑ − (l + 1)

l=0

∞
X

!

Cl a−(l+2) Pl (cos ϑ)

l=0

 X
∞
∞
X

l−1
Al la Pl (cos ϑ) = −E0 cos ϑ −
(l + 1)Cl a−(l+2) Pl (cos ϑ)
0 l=0
l=0
∞  
X

l=0

0

l−1

Al la

+ (l + 1)Cl a

−(l+2)



Pl (cos ϑ) = −E0 cos ϑ

de aquí se obtiene

 

A1 + 2C1 a−3 = −E0
0
 

Al lal−1 + (l + 1)Cl a−(l+2) = 0, l 6= 1
0
En resumen
A1 a −

C1
= −E0 a
a2

Al al − Cl a−(l+1) = 0, l 6= 1
 

A1 + 2C1 a−3 = −E0
0
 

Al lal−1 + (l + 1)Cl a−(l+2) = 0, l 6= 1
0
de la segunda ecuación

Al = Cl 2l+1 , l 6= 1
a

reemplazando en la cuarta
 

Cl 2l+1 lal−1 + (l + 1)Cl a−(l+2) = 0, l 6= 1
0
a
  


l+1
l
+ l+2 = 0, l 6= 1
Cl
0
al+2
a

Luego

Cl = Al = 0, l 6= 1

---

### Página 45

Para l = 1, de la primera ecuación
A1 =

C1
− E0
a3

reemplazando en la tercera
 


C1
− E0 + 2C1 a−3 = −E0
0
a3
C1
a3
Finalmente








+ 2 = E0
−1
0
0

−1
0

+2
0

C1 = a E0


−1
0

+2
0

A1 = E0

A1 = E0

!

!

− E0


− 1 − 0 − 2
0

+2
0


+2
0

A1 = −E0

!

!

Con esto, se tiene
φint = −E0


+2
0

!

r cos ϑ = −E0

φext = −E0 r cos ϑ +

a
cos ϑE0
r2


+2
0

−1
0

+2
0

!

!

Notar que el potencial interior define un campo eléctrico uniforme
!
~ int = E0
E
ẑ

+2
0

z

---

### Página 46

La figura muestra las equipotenciales para E0 = 100 (V /m), /0 = r = 5, a = 10 (m)

Notar que un dieléctrico con permitividad muy grande se compora de forma similar a un
conductor, en efecto, si  → 0
~ · E(~
~ x) = ρ → 0
∇

~
~
∇ × E(~x) = 0
y entonces el campo está forzado a ser nulo en el interior del dieléctrico / conductor. La
siguiente figura muestra la solución para r = 5000

En este caso, el potencial es prácticamente constante e igual a cero dentro de la esfera

---

### Página 47

Parte IV
Corrientes Eléctricas

---

### Página 48

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 49

#### Capítulo 11
Corrientes Eléctricas
Las corrientes eléctricas son flujos de cargas eléctricas. Para ilustrar esto supongamos un
conjunto de cargas que se mueven perpendicularmente a una superficie de área A, como se
muestra en la figura

La corriente eléctrica se define como la tasa a la cual las cargas atraviesan un área transversal.
Si una cantidad de carga ∆Q pasa a través una superficie en un intervalo de tiempo ∆t, entonces la corriente promedio Iavg está dada por:
∆Q
∆t
. El rango común
La unidad en S.I. de la corriente es el ampere (A), con 1A = 1 Coulomb
seg
de corrientes va desde mega-amperes en rayos hasta nano-amperes en células nerviosas. En el
límite cuando ∆t → 0, la corriente instantánea se define como
Iavg =

dQ
dt
Ya que el flujo tiene una dirección, hemos introducido implícitamente la convención de que
la dirección de la corriente corresponde a la dirección en la cual las cargas positivas se mueven.
Las cargas que se mueven dentro de un cable son electrones cargados negativamente que se
mueven en dirección opuesta a la corriente. Corrientes eléctricas fluyen en conductores, sólidos
(metales, semiconductores), fluídos (electrolitos, ionizados) y gases (ionizados), pero el flujo no
es permitido en no conductores o aislantes.
I=

---

### Página 50

11.1.

Densidad de Corriente

Intentaremos ahora relacionar la corriente (una cantidad macroscópica) con el movimiento
microscópico de las cargas. Para ello supongamos un conductor de área transversal A, como se
muestra en la figura

Sea la corriente total a través de una superficie escrita como
¨
~ x0 ) · J(~
~ x0 )
I=
dS(~
S

~ x) es la densidad de corriente ( tiene unidades de A/m2 ). Si q es la carga de cada
donde J(~
portador, y n es el número de portadores de carga por unidad de volumen, la cantidad de carga
total en esta sección es ∆Q = q(nA∆x). Supongamos que las cargas se mueven con velocidad
vd , así, el desplazamiento en un intervalo ∆t será ∆x = vd ∆t, lo que implica
∆Q
= nqvd A
∆t
La velocidad vd a la cual el portador de carga se mueve se conoce como velocidad de deriva.
Físicamente, vd es la velocidad promedio de un portador de carga dentro de un conductor
cuando un campo eléctrico externo es aplicado. De hecho, un electrón dentro de un conductor
no viaja en línea recta, si no que su movimiento es errático, como se ve en la figura
Iavg =

Se tiene entonces que la densidad de carga se puede escribir como
J~ = nq~vd
Vemos entonces que J~ y ~vd tienen la misma dirección para portadores de carga positiva, y
tienen direcciones opuestas para los portadores de carga negativa

---

### Página 51

11.2.

Continuidad de la carga Eléctrica

Consideremos un volumen V determinado por una superficie cerrada S. La carga que entra
en el dominio V en 1 segundo será ( o equivalentemente, la corriente que ingresa a V )
ˆˆ
 ~ 0
~ x0 )
x ) · J(~
I = −  dS(~
S

Notar que el signo menos es consistente con la definición de flujo (Flujo es positivo cuando
las líneas de campo salen a través de la superficie ). Por otro lado, la carga total encerrada por
este volumen para cierto instante estará dada por
˚
d3 x0 ρ(~x0 , t)
Q(t) =
V

Con lo que la corriente será la razón de cambio de esta carga en el tiempo
˚
dQ
∂ρ(~x0 )
I=
d3 x0
=
dt
∂t
V
Igualando debe tenerse entonces
˚
ˆˆ
∂ρ(~x0 )
 ~ 0
~
d3 x0
−  dS(~x ) · J(~x ) =
∂t
S
V
Utilizando el teorema de la divergencia
˚
˚
∂ρ(~x0 )
3 0~ 0 ~ 0
−
d x ∇ · J(~x ) =
d3 x0
∂t
V
V


˚
∂ρ(~x0 )
3 0
0 ~
~
=0
d x ∇ · J(~x) +
∂t
V
Esta ley de conservación de la carga simplemente indica que la variación de la carga contenida en un volumen arbitrario V se debe a un flujo de carga a través de su superficie. Como
se cumple para todo V , se obtiene la ecuación de continuidad para la carga eléctrica, en su
forma diferencial
~ · J(~
~ x, t) + ∂ρ(~x) = 0
∇
∂t
Supongamos que en determinada región del espacio existe una corriente en estado estacionario, es decir, no hay dependencia temporal. Entonces se cumple
~ · J(~
~ x) = 0
∇

---

### Página 52

Cuando existen corrientes estacionarias, la densidad de carga en cada punto es una constante. Es decir, sobre cualquier volumen V , el flujo neto de carga a través de su superficie es
cero, lo que es consistente con
ˆˆ
˚

~ x) · J(~
~ x) =
~ · J(~
~ x) = 0
d3 x∇
  dS(~
S(V )

11.3.

V

Ley de Ohm

Las corrientes en medios materiales surgen como una respuesta a un campo eléctrico. En
algunos materiales, la densidad de corriente depende linealmente del campo eléctrico externo
~ Esta relación usualmente se expresa como
E.
~ x) = σ E(~
~ x)
J(~
Donde σ es la conductividad del material. Este podría ser una matriz de coeficientes
no constantes (lo que representa a un medio no homogéneo y anisotrópico). Sin embargo,
trabajaremos con medios simples, en donde σ es una constante positiva. Esta ecuación se
conoce como la ley de Ohm diferencial. Un material que obedece esta relación se dice Ohmico.
Veamos un caso particular y muy usual de la ley de Ohm, consideremos un segmento de alambre
recto de largo l ,área A, y conductividad σ, como se muestra en la figura

Supongamos que una diferencia de potencial ∆V = φb − φa es aplicada entre los extremos del
~ , y como consecuencia, una corriente I. Asumiendo
alambre, generando un campo eléctrico E
~ uniforme en el conductor, y apuntando en la dirección longitudinal se tiene
E
∆V = φb − φa = −

ˆ b

~ x) = El
d~x · E(~

a

Si el medio es Ohmico, el módulo de la densidad de corriente se puede escribir como


∆V
J = σE = σ
l
Por otro lado, J = I/A, luego
l
∆V = J =
σ
Donde



l
σA



I = RI

l
∆V
=
I
σA
es la resistencia del conductor. La famosa ecuación
R=

---

### Página 53

∆V = IR
Es la version macroscópica de la ley de Ohm. La unidad de R es el Ohm (Ω), donde
1V
1A
También se suele definir la de un material como una propiedad intensiva de éste, que es
simplemente el recíproco de la conductividad
1Ω =

σ
con esto la resistencia de un conductor cilíndrico queda
ρ=

ρl
A
La mayoría de los metales, con buena conductividad y baja resistividad, son ohmicos.
R=

11.3.1.

Conexión entre conductores

Imaginemos que se tienen 2 conductores perfectos, inicialmente cargados (se encuentran
entonces a determinado potencial). La forma de estos dos conductores es absolutamente irrelevante, pero por simpleza y elegancia, en la siguiente figura se ilustran dos conductores esféricos,
cargados con carga q1 y q2 , respectivamente

Si estos conductores están en el vacío, existirá un campo electrostático. Suponiendo que el
conductor con carga q1 se encuentra a mayor potencial, las líneas de campo se verán (para el
caso de los conductores esféricos) así

Si existiera alguna carga libre, ciertamente ésta se movería debido al campo eléctrico que
generan los conductores. Sin embargo, en el vacío (ausencia de cargas), simplemente nada
ocurre. Ahora, imaginemos que ambos conductores se conectan por algún medio parcialmente
conductor (de conductividad finita). La forma puede ser cualquiera, incluso podríamos imaginar
en llenar todo el espacio de un material conductor, pero podemos imaginar como caso particular
(y simple) un alambre muy delgado

---

### Página 54

¿Qué ocurre entonces?. Ahora existe un medio entre los conductores que posee cargas libres !
Sin duda éstas se moveran siempre que exista un campo eléctrico, y entonces cargas se moverán
desde el conductor a mayor potencial hacia el conductor que está a menor potencial. Como
consecuencia de esto, el campo eléctrico en la región entre los conductores se irá debilitando,
pues este movimiento de cargas de uno al otro provocará una disminución en la diferencia de
potencial entre ambos conductores. En conclusión, la conexión entre 2 conductores mediante
un medio de conductividad finita dará origen a una corriente. Esta corriente se hará cada vez
mas débil, hasta que se alcanze un equilibrio en el cual los dos conductores quedan al mismo
potencial.
Ahora, pensemos que tenemos un solo conductor, inicialmente cargado con carga Q. Imaginemos que lo conectamos con el infinito mediante algun camino de conductividad finita, por
ejemplo un alambre infinito, esto equivale a conectarlo a otro conductor a potencial cero. Lo
que sucederá es que toda la carga contenida en el conductor se irá por este camino hacia el
infinito, de esta forma, nuestro conductor queda a potencial cero y absolutamente descargado.

---

### Página 55

11.4.

Circuitos Eléctricos

Un circuito es una malla de resistencias, fuentes, condensadores, etc, unidas por medio de
conductores perfectos. Un nodo es un punto donde convergen 2 o más conductores. Así, en un
nodo se cuple que la suma de las corrientes es cero, esta es la 1 Ley de Kirchhoff, o Ley de
Corrientes de Kirchhoff (LCK)
X
Ik = 0
k

Notar que esta ecuación es equivalente a la ecuación de continuidad de la carga eléctrica
para corrientes continuas (estacionarias)
~ · J(~
~ x) = 0
∇

.
La segunda Ley de Kirchhoff o Ley de Voltajes de Kirchhoff (LVK) dice que la suma de las
caídas de potencial en cada camino cerrado suma 0. Notar que esta ley proviene de
~ × E(~
~ x) = 0
∇
~ sobre una curva cerrada (circuito cerrado) es 0.
Debido a esto la integral de línea del campo E
Energía eléctrica y potencia
Considere un circuito consistente en una batería y una resistencia (R). Sea la diferencia de
potencial entre los puntos a y b ∆V = φb − φa > 0. Si una carga ∆q se mueve a través de
la batería, su energía potencial eléctrica aumenta ∆U = ∆q∆V . Por otro lado, si la carga se
mueve a través de la resistencia, la energía potencial decrece debido a las colisiones con los
átomos de la resistencia. Si despreciamos la resistencia interna de la batería y la de los cables
conductores, al volver al punto a, la energía de ∆q permanece invariante.

Así, la tasa a la que se disipa energía a través de la resistencia está dada por
∆q
∆U
= ( )∆V = I∆V
∆t
∆t
Esta es precisamente la potencia suministrada por la batería. Usando que ∆V = IR, se
puede reescribir como
P =

(∆V )2
R
Los circuitos eléctricos conectan fuentes de poder a cargas como resistencias, motores,
lámparas, etc. La conexión entre la fuente y la carga se hace soldando con cables conductores, tambien llamados nodos. Las distintas partes de un circuito pueden estar en serie o en
P = I 2R =

---

### Página 56

paralelo, como ya se vió en el caso de los capacitores.
Dos elementos se dicen estar en paralelo cuando son conectados a la misma diferencia de potencial.

Por otro lado,cuando los elementos son conectados uno seguido de otro, tal que la corriente
pasa a través de cada elemento sin otros caminos de por medio, los elementos están en serie.
Se pueden tener circuitos cerrados, a través de los cuales fluye corriente, o bien circuitos
abiertos en donde no existen corrientes. Usualmente por accidente, los cables pueden entrar en
contacto, causando un corto circuito, esto es, gran parte de la corriente fluirá a través del corto
circuito, mientras que una fracción muy pequeña fluirá a través de la carga.
Esto podría quemar un equipo eléctrico como un transformador. Para prevenir el daño, un
fusible se conecta en serie. Cuando hay un corto circuito, el fusible aisla la carga del resto del
circuito.
En los circuitos eléctricos, un punto (o un nodo en común) se escoge como tierra. A este punto
se le asigna arbitrariamente un voltaje, usualmente cero, y el voltaje V en cualquier otro punto
del circuito está definido como la diferencia de potencial entre el punto y la tierra.
Fuerza Electromotriz
Vimos que energía eléctrica debe ser suministrada para mantener una corriente constante en
un circuito cerrado. La fuente de energía es llamada comúnmente como la fuerza electromotriz,
o f.e.m (ε). Las baterías son ejemplos de fuentes de f.e.m. Se pueden pensar como bombas que
mueven cargas desde potenciales bajos a potenciales más altos. Matemáticamente la f.e.m se
define como
dW
ε=
(11.1)
dq
Que corresponde al trabajo hecho para mover una unidad de carga en la dirección del potencial
más alto. La unidad SI para ε es el volt (V). Considere un circuito simple que consiste en una
batería como fuente de f.e.m y una resistencia R, como se muestra en la figura

Asumiendo que la batería no posee resistencia interna, la diferencia de potencial ∆V entre los
terminales positivo y negativo de la batería es igual a la fem ε. Para establecer una corriente

---

### Página 57

alrededor del circuito, la batería efectúa un proceso de descarga que convierte energía química
en una f.e.m. La corriente I se puede encontrar notando que no hay un trabajo neto al mover
una carga q a través de un camino cerrado debido a la naturaleza conservativa de la fuerza
electrostática.

W = −q

˛

~ · dS
~=0
E

Sea a el punto de partida

Cuando se atraviesa desde el terminal negativo al positivo, el potencial aumenta en ε. Por otro
lado, cuando atravesamos la resistencia, el potencial decrece una cantidad IR, y la energía
potencial se convierte en energía térmica en la resistencia. Asumiendo que los cables conectores
no poseen resistencias, a través de un camino cerrado, la diferencia de potencial neta es cero
ε − IR = 0
Lo que implica
I=

ε
R

De todas formas, una batería real siempre posee una resistencia interna r

Ahora la diferencia de potencial a través de la batería es
∆V = ε − Ir
Ya que no hay una diferencia de potencial neta a través de un camino cerrado, tenemos
ε − Ir − IR = 0
O bien
ε
R+r
De la figura de la derecha vemos el cambio de potencial mientras atravesamos el circuito en el
sentido del reloj. Notar que la mayor diferencia de potencial está inmediatamente despues de la
I=

---

### Página 58

batería. El voltaje cae a medida que se atraviesa cada resistencia. Notar también que el voltaje
es constante en los cables. Esto se debe a que los cables poseen resistencias extremadamente
pequeñas comparadas con las resistencias del circuito.
Para una fuente de f.e.m ε, la potencia a la cual la energía se entrega es
P = Iε = I(IR + Ir) = I 2 R + I 2 r
Es decir, la potencia de la fuente es igual a la suma de la potencia disipada en ambas resistencias, la interna y la de carga. Esto es necesario debido a la conservación de la energía.

---

### Página 59

Problema
El espacio entre dos circuitos conductores de largo L y radios a y b (b > a), está lleno de
material de conductividad σ. Calcule la intensidad de la corriente por unidad de longitud y la
resistencia, cuando la diferencia de potencial entre los conductores es V0 .

#### Solución
La diferencia de potencial será responsable de un movimiento de cargas a través del material
conductor que se encuentra entre los conductores externos. La conservación de la carga implica
∂ρ(~x) ~ ~
+ ∇ · J(~x) = 0
∂t
Para corrientes estacionarias
∂ρ(~x)
~ · J(~
~ x) = 0
=0→∇
∂t
~ x) = σ E(~
~ x)
Si el medio es Ohmico, J(~
~ ·
∇
Si el medio además es homogéneo




1~
E(~x) = 0
σ

1~ ~
~ · E(~
~ x) = 0
∇ · E(~x) = 0 → ∇
σ
Finalmente

~ 2φ = 0
∇

Y entonces el potencial satisface la ecuación de Laplace en la región a < r < b. La solución
en coordenadas cilíndricas (suponiendo que ése depende únicamente de la coordenada radial r)
es
φ(r) = A ln r + B
Imponiendo la condición φ(a) − φ(b) = V0
A = V0 ln

b
a

Así, se obtiene el campo eléctrico
~ x) = −∇φ(~
~ x)
E(~
~ x) = V0 ln b 1 r̂
E(~
ar

---

### Página 60

Utilizando la ley de Ohm, se obtiene la densidad de corriente
~ x) = σ E(~
~ x) = σV0 ln b r̂
J(~
ar
La corriente por unidad de largo que fluye a través de los conductores se puede obtener
como la integral de flujo de la densidad de corriente sobre una superficie cilíndrica de radio r
(y largo unitario). Esta integral resulta simple pues la densidad de corriente tiene magnitud
constante a lo largo de esta superficie, y su dirección coincide en todo punto con la normal. El
diferencial de área sobre el cilindro es da = drdϕdz
ˆ 1 ˆ 2π
¨
σV0 b
~
~
dS(~x) · J(~x) =
dz
dϕr
I=
ln
r
a
S
b
I = 2πσV0 ln [A/m]
a
Así, la resistencia por unidad de longitud es
r=

V0
ln(b/a)
=
I
2πσ

y la resistencia total es
R = rL =

L ln(b/a)
2πσ

---

### Página 61

Problema
Dos esferas metálicas concéntricas, de radios a y b están separadas por un material conductor
de conductividad σ constante
a) Si estas esferas son mantenidas a una diferencia de potencial V constante, encuentre la
corriente que va de una a la otra
b) Encuentre la resistencia entre las esferas
c) Observe que en este caso se cumple R = 0 /, donde C es la capacidad. Demuestre esta
fórmula para dos conductores cualquiera, separados por un material conductor de conductividad
σ constante

#### Solución
a) Al establecer una diferencia de potencial sobre los conductores
V = φ(a) − φ(b)
se inducirán cargas Q y −Q sobre las superficies r = a y r = b, respectivamente. El campo
eléctrico en la región interior se puede determinar a partir de la ley de Gauss debido a la simetría
esférica que éste debe tener
ˆˆ
 ~
~ x) = Q
x) · E(~
 dS(~
0
S
Si S se escoge como una superficie esférica de radio r, se tiene
E(r)4πr2 =
~
E(r)
=

Q
0

Q
r̂, a < r < b
4π0 r2

Por otro lado
V =

ˆ b

~ x) =
d~x · E(~

a

ˆ b

drQ
a 4π0 r

donde se ha utilizado un camino radial para evaluar la integral de línea


1 1
Q
V =
−
4π0 a b
Entonces

V 4π0
Q= 1 1
−b
a

---

### Página 62

luego, para a < r < b
~ x) =
E(~

V ab
r̂
(b − a)r2

Debido a que la zona a < r < b está llena con un material conductor, el campo eléctrico
dará origen a un movimiento de cargas (corriente), en donde la densidad está relacionada con
~ mediante la ley de Ohm
el campo E
~ x) = σ E(~
~ x) =
J(~

V σab
r̂
(b − a)r2

La corriente que fluye entre los conductores se puede obtener integrando sobre una superficie
esférica S de radio r, a < r < b
ˆˆ
 ~
~ x) = 4πr2 J(r)
x) · J(~
I =  dS(~
S

Luego
I=

4πσV ab
(b − a)

b) La resistencia está dada por
V
I


1 1
−
R=
4πσ a b
R=

c) La capacidad de un condensador esférico es
C=

4π0 ab
Q
=
V
b−a

Evaluando
0 a1 − 1b
0
=
=
σC
σ 4π0
y entonces se tiene

0
=R
σC

− 1b
a

4πσ



---

### Página 63

Veamos que esto se cumple en el caso general. Sean 1 y 2 dos conductores cualquiera ,
separados por un material de conductividad σ

Se tendrá un flujo de corriente dado por
ˆˆ
 ~
~ x)
I =  dS(~
x) · J(~
S

por ley de Ohm

~ x) = σ E(~
~ x)
J(~
ˆˆ

 ~
~ x)
x) · E(~
I = σ  dS(~
S

por ley de Gauss
Q
0
Por otro lado, si C es la capacidad del sistema, se cumple
I=σ

Q = CV
entonces
I=

σCV
0

V =

0
I
σC

Finalmente se demuestra la relación general
R=

0
σC

---

### Página 64

Problema
Considere un conductor perfecto, inicialmente con carga Q0 , y completamente rodeado por un
medio uniforme de conductividad σ y constante dieléctrica 
a) Si el conductor es una esfera de radio a, muestre que su carga como función del tiempo es
Q(t) = Q0 e−σt/
b) Muestre que el resultado anterior es válido independientemente de la forma del conductor
#### Solución
a) Sea Q(t) la carga sobre la superficie esférica al instante t. Ésta generará un campo eléctrico
esféricamente simétrico

~ x, t) = Q(t) r̂
E(~
4πr2
al ser el medio circundante un conductor de conductividad σ, se tendrá una densidad de
corriente como respuesta a este campo
~ x, t) = σ E(~
~ x) = σQ(t) r̂
J(~
4πr2
Esta es una corriente que fluye isotrópicamente de forma radial. La corriente se obtiene de
~ x) sobre una superficie cerrada que contenga a la esfera conductora, en particular se
integrar J(~
puede evaluar tomando una esfera concéntrica de radio r > a
¨
~ x) · J(~
~ x, t) = σQ(t)
I(t) =
dS(~

S
Por otro lado, la carga total contenida en el volumen encerrado por S es
˚
Q(t) =
d3 xρ(~x, t)
V

Por la continuidad de la carga
dQ(t)
= I(t)
dt
σQ(t)
dQ(t)
=
dt


---

### Página 65

cuya solución es
Q(t) = Q0 e−tσ/

b) El resultado anterior es independiente de la forma de los conductores. En efecto, sea S
una superficie cerrada que contenga completamente al conductor. La corriente que se genera
está dada por
ˆˆ
 ~
~ x)
I =  dS(~
x) · J(~
S

Si el medio es ohmico
ˆˆ

 ~
~ x)
x) · E(~
I = σ  dS(~
S

y utilizando la ley de Gauss
I=σ

dQ(t)
Q(t)
=

dt

y se obtiene la misma ecuación diferencial para la carga contenida en el conductor

---

### Página 66

Problema
Dos cilindros coaxiales (radios a y b) de largo L están separados por un material de conducividad
σ(r) = kr donde k es una constane arbitraria y r la distancia al eje (común) de los cilindros.
Encuentre la resistencia entre los cilindros. Observe que al ser la conductividad función de la
posición, la densidad de carga en el material conductor no es cero y el campo E no varía como
1/r. Recuerde que una corriente estacionaria I tiene el mismo valor para cualquier superficie
cilíndrica

#### Solución
Supongamos que se establece una diferencia de potencial ∆V > 0 entre los conductores r = a
y r = b. Usaremos el hecho de que la corriente que fluye entre los cilindros está dada por la
integral
¨
~ x)
I=
dS(~x)n̂(~x) · J(~
S

Donde S es un cilindro concéntrico a los conductores, de radio r y largo L. Además, por
simetría cilíndrica, J~ = J(r)r̂
I = 2πrLJ(r)
luego la densidad de corriente es
~ x) =
J(~

I
r̂
2πrL

~ = E(r)r̂ (por simetría), se tiene por ley de Ohm
Si E
~ x) = σ(r)E(r)
~
J(~
luego
E(r) =

r I
k 2πrL

con esto, la diferencia de potencial entre los conductores es
ˆ b
~ x) = I (b − a)
∆V =
d~x · E(~
2πLk
a
Entonces
R=

∆V
b−a
=
I
2πkL

---

### Página 67

Problema
Se sabe que la atmósfera tiene una conductividad (causada principalmente por los rayos cósmicos) que depende de la altura de la siguiente manera


z2
σ(z) = 3 +
10−14 [Ω]−1
donde z es la distancia vertical sobre el suelo. Se ha encontrado además, un campo eléctrico
vertical, dirigido hacia el suelo, que en la superficie de la tierra vale
~ = −100k̂
E
Suponga el siguiente modelo de la atmósfera: imagine una capa conductora paralela a la superficie; situada a una distancia de 15 km sobre el nivel del suelo. Entre esta capa y la tierra se
encuentra la atmósfera, con la conductividad y el campo eléctrico indicados arriba. El radio de
la tierra es RT = 6400 km.
a) Calcule el campo eléctrico y el potencial en función de la altura z
b) Calcule la corriente total que fluye entre la capa superior conductora y la tierra
#### Solución
a) Sabemos que en corriente continua (o estacionaria) se cumple que
~ · J(~
~ x) = 0
∇
Además, se sabe que la dirección del campo eléctrico es según z y, por razones de simetría
no debe depender de las coordenadas x e y. Eso se traduce en
~ · (σ(z)E(z)) = d (σ(z)E(z)) = 0
∇
dz
σ(z)E(z) = A
El valor de esta constante se puede obtener evaluando en z=0
A = σ(0)E(0) = −3 × 10−12

De esta forma, el campo eléctrico en la atmósfera es
~ x) = −3 × 10−12
E(~

(3 + z3 )10−14

k̂ =

−300
2 k̂
3 + z3

Fijando el valor del potencial en la tierra como 0, entonces
φ(z) =

ˆ ~x2

~ x)
d~x · E(~

~
x1

donde ~x2 es cualquier punto a altura z, y ~x1 es un punto sobre la superifice. Escogiendo una
curva vertical, se tiene

ˆ z 
ˆ z
z 
φ(z) =
=
900Arctg
dz
=
dz
3 + z2
3 + z3

---

### Página 68

b) La densidad de corriente se obtiene usando la ley de Ohm, esto es


z
~ x) = σ(z)E(~
~ x) = − 3 +
J(~
k̂ = −3 × 10−12 [A/m2 ]k̂
10−14
z2
3+ 3
La corriente será
I=

¨

S

~ x0 ) · J(~
~ x0 ) = −3 × 10−12 S = −3 ∗ 10−12 4πRT2
dS(~
I = 122,88[A]

---

### Página 69

Problema
Una batería descargada se carga conectándola a la batería cargada de otro automóvil mediante
cables para corriente. Determine la corriente del motor de arranque y en la batería descargada

#### Solución
Se utiliza la Ley de Voltajes de Kirchhoff (LVK) para cada malla, esto es

Para la malla 1
−12 + 0,01I1 + 1 (I1 − I2 ) + 10 = 0
y en la malla 2
−10 + 1(I2 − I1 ) + 0,06I2 = 0

De la primera ecuación se obtiene
I2 = 1,01I1 − 2
Reemplazando
0,0706I1 − 2,02 = 10 → I1 = 170,25A
Con esto
I2 = 1,01 ∗ I1 − 2 = 169, 95A

---

### Página 70

I2 es la corriente a través del motor de arranque, mientras que la corriente a través de la
batería descargada será, según nuestra convención

I3 = I1 − I2 = 170,25 − 169,95 = 0,2975A

---

### Página 71

Problema
En el circuito de la figura la batería tiene una FEM de valor V . Encuentre la resistencia R que
debe colocarse entre los terminales A y B para que en ella se disipe la máxima potencia

#### Solución
Resolviendo el problema con mallas

Para la malla 1
−V + I1 R0 + R0 (I1 − I2 ) = 0
Para la malla 2
R0 (I2 − I1 ) + R0 I2 + RI2

De la primera ecuación se obtiene
I1 =

V + I2 R0
2R0

Reemplazando en la ecuación de la malla 2
V + I2 R0
2R0
V
(3R0 + 2R)I2 = V → I2 =
3R0 + 2R
(2R0 + R)I2 = R0 I1 = R0

Teniendo la corriente que pasa por la resistencia R, la potencia que ésta consume se puede
obtener como
P = VR IR = (IR R)IR = IR2 R

---

### Página 72

Así
P =

V2
R
(3R0 + 2R)2

Para encontrar el valor de R que maximize esta potencia consumida, bastará con resolver
dP (R)
=0
dR
Esto es
dP
4RV 2
3V 2 R0 + 2V 2 R − 4RV 2
V2
−
=
=
dR
(3R0 + 2R)2 (3R0 + 2R)3
(3R0 + 2R)3

3V 2 R0 − 2V 2 R
= 0 → 3V 2 R0 − 2V 2 R = 0
(3R0 + 2R)
Así, la resistencia R que maximiza la potencia consumida es
R = R0

---

### Página 73

Problema
La fuente V1 = 240 (V) está conectada a tres resistencias iguales según la figura

a) Determine R si la fuente de voltaje entrega 1920(W) al conjunto de resistencias
b) Si al circuito en paralelo, se le agregan más resistencias en paralelo, siguiendo una secuencia
de 3R en serie, 4R en serie, hasta llegar a N R en serie, calcule la potencia suministrada por la
fuente de voltaje cuando N tiende a Infinito

#### Solución
a) El circuito se puede reducir considerando que hay 2 resistencias en serie, cuya resistencia
equivalente será la suma de ambas, así, el circuito queda

Estas 2 resistencias ahora se encuentran en paralelo, por lo que se puede obtener un Req de
todo el circuito
= +
=
Req
R 2R
2R
Con lo que

Req = R

---

### Página 74

Con esto, el circuito equivale a

La potencia generada por este circuito será la misma que consume Req , esto es


V
= 1920W
P = VReq IReq = V IReq = V
Req
De aquí se obtiene
Req =

V2
=
= 30Ω
P

Finalmente se obtiene R usando que
Req = R → R = Req = 45Ω
b)

En este caso, se puede obtener una resistencia equivalente según
= +
+ ... +
Req
R 2R
NR
Así, se puede obtener la potencia que debe entregar la fuente para un cierto valor de N
N
X
V2
PN =
=V
Req
kR
k=1

Así, para obtener la potencia cuando N tiende a infinito, bastará con obtener el siguiente
límite (si existe)
PN →∞ = lím PN = V 2
N →∞

∞
X
k=1

kR

Pero esta serie diverge, es decir, la potencia necesaría sería infinita. Esto es lógico ya que la
fuente tendría que alimentar un número infinito de resistencias.

---

### Página 75

Problema
Una batería tiene una f.e.m ε y una resistencia interna R. Una resistencia de carga R2 se conecta
a los terminales de la batería.
a) Determine el valor de R2 tal que la diferencia de potencial aplicada a los terminales sea
máxima.
b) Determine el valor de R2 para obtener una corriente máxima en el circuito.
c) Determine el valor de R2 para que la potencia consumida por ésta sea la máxima posible

#### Solución
a) Primero determinamos la corriente a través del circuito
ε
R + R2
Así, la diferencia de potencial entre los extremos de la batería es
−ε + IR + IR2 = 0 → I =

V = IR2 =

R2 ε
ε
=
R + R2
1 + RR2

La diferencia de potencial entre los terminales será máxima cuando R2 → ∞ y valdrá ε,
que es el valor de la fem.
b) Teníamos que

ε
R + R2
Luego, la corriente será máxima si R2 = 0, y equivale a cortocircuitar los terminales de la
batería
I=

c) La potencia consumida por R2 está dada por
P =VI =

R 2 ε2
R2 ε
ε
=
R + R2 R + R2
(R + R2 )2

Para encontrar el valor de R2 que maximiza esta potencia resolvemos
ε2 (R + R2 )2 − 2(R + R2 )R2 ε2
dP
=
=0
dR2
(R + R2 )4

---

### Página 76

Así
(R + R2 )2 − 2(R + R2 )R2 = 0 → R2 + R − 2R2 = 0
Luego, la potencia será máxima si
R2 = R
es decir, se debe colocar una resistencia igual a la resistencia interna de la batería

---

### Página 77

Problema
Calcule la potencia entregada a cada resistencia en el circuito de la figura

#### Solución
Se resuelve el circuito mediante LVK

Para la malla 1
−18 + 2I1 + 3(I1 − I2 ) + 4I1 = 0 → 9I1 − 3I2 = 18
en la malla 2
3(I2 − I1 ) + 1I2 = 0 → 4I2 = 3I1

Resolviendo
9I1 − I1 = 18 → I1 = 2, 6A
I2 = I1 = 2A
Teniendo las corrientes que circulan por el circuito, podemos obtener la potencia que consume cada resistencia, usando que P = V I = I 2 R
P2Ω = 2I12 = 13, 52W
P4Ω = 4I12 = 27, 04W
P3Ω = 3(I1 − I2 )2 = 1, 08W
P1Ω = 1I22 = 4W

---

### Página 78

Problema
El circuito de la figura es llamado Puente de Wheastone y se usa para calibrar resistencias. El
dispositivo está formado por 3 resistencias, de las cuales 2 son ajustables, y un galvanómetro
(dispositivo que sirve para medir corrientes). Para realizar la medida, se ajustan las resistencias
variables R1 y R2 hasta que el galvanómetro marque cero. Exprese el valor de Rx en función
de las otras 3 resistencias. Modele el galvanómetro como una resistencia RG .

#### Solución
Definamos las corrientes que circulan por el circuito

Se obtienen las relaciones inmediatas
I = I1 + I2
I1 = I3 + Ig
I = I4 + I3
I4 = I2 + Ig
Cuando la corriente que pasa por el galvanómetro es nula, se tiene
I1 = I3
I2 = I4
Además, utilizando la ley de voltajes de Kirchhoff
−V + I2 R2 + I4 Rx = 0
−V + I1 R1 + I3 R3 = 0

---

### Página 79

I1 R1 − I2 R2 = 0
De esta última ecuación, se obtiene
I2 = I1

R1
R2

Además, igualando el valor de V
I2 R2 + I4 Rx = I1 R1 + I3 R3
I2 R2 + I2 Rx = I1 R1 + I1 R3
I1

R1
(R2 + Rx ) = I1 (R1 + R3 )
R2

Rx =

R2
R2 R3
(R1 + R3 ) − R2 =
R1
R1

Finalmente
Rx =

R2 R3
R1

---

### Página 80

Problema
En el circuito de la figura, la batería de más arriba y la de más abajo tienen la misma f.e.m
igual a ε. La del medio tiene 2ε. Las resistencias interiores de las baterías son iguales a r. Existe
una sola resistencia exterior R (ubicada como se ve en el dibujo). Designe las corrientes por I1 ,
I2 , I3 , como se ve en el dibujo

a) Calcule las tres corrientes en valor y signo.
b) Suponga que el punto a del circuito está conectado a tierra y calcule en tal caso el potencial
que tiene el punto b
#### Solución
Definimos un sentido arbitrario para las corrientes I1 ,I2 e I3 , como se ve en la figura

Resolvemos el circuito con la ley de voltajes de Kirchhoff (LVK). La ecuación para la malla
2 es
ε + rI2 − 2ε + (I2 + I1 )r = 0
−ε + 2rI2 + rI1 = 0
Para la malla 1
−2ε + (I1 + I2 )r + I1 R + ε + I1 r = 0
−ε + I2 r + I1 (R + 2r) = 0

De la primera ecuación obtenemos
I2 =

ε − rI1
2r

---

### Página 81

Así
−ε +

ε − rI1
+ I1 (R + 2r) = 0

−2ε + ε − rI1 + 2I1 (R + 2r) = 0
Finalmente
I1 =

ε
3r + 2R

y
I2 =

ε
rε
3rε + 2Rε − rε
ε(r + R)
−
=
=
2r 2r(3r + 2R)
2r(3r + 2R)
r(3r + 2R)

Por ultimo, I3 = I1 + I2
I3 =

ε
ε(2r + R)
ε(r + R)
+
=
r(3r + 2R) 3r + 2R
r(3r + 2R)

Como los valores obtenidos son todos positivos, los sentidos de las corrientes supuestos inicialmente son todos correctos.
b)

De la figura es claro que
VB − VA = I1 R + ε + I1 r = I1 (R + r) + ε

Como A está conectado a tierra, VA = 0
VB = ε + (R + r)

ε(R + 2r)
ε
=ε+
3r + 2R
2R + 3r

---

### Página 82

Problema
Considere la línea telegráfica de L metros de longitud, y de resistencia por unidad de largo
r[Ω/m]. Esta línea tiene una falla de resistencia R en un punto. Demuestre que la corriente
que lee un amperímetro ideal (de resistencia interna 0) conectado a un extremo de la línea es
mínima cuando la falla se encuentra en el medio de la distancia entre el transmisor y el receptor.
#### Solución
Supongamos que la falla está a una distancia x de uno de los extremos. El sistema queda
modelado por el siguiente circuito

Sea I1 la corriente por R1 , I2 la corriente por R2 e I la corriente por R. Es claro que
I = I1 − I2
Ahora, las ecuaciones de malla son las siguientes
−V + R1 I1 + R(I1 − I2 ) = −V + rxI1 + R(I1 − I2 ) = 0
R2 I2 + R(I2 − I1 ) = r(l − x)I2 + R(I2 − I1 ) = 0

De la primera ecuación
I1 =

V + RI2
R + rx

Reemplazando esto último
r(l − x)I2 + RI2 − R

V + RI2
=0
R + rx

RrlI2 − RxrI2 + r2 lxI2 − x2 r2 I2 + R2 I2 + RrxI2 − RV − R2 I2 = 0
I2 =

RV
Rrl + r2 lx − x2 r2

I2 =

RV
Rrl + r2 x(l − x)

---

### Página 83

Ahora veamos cuando esta corriente es mínima. Esto equivale a encontrar el x tal que el
denominador sea máximo

d
Rrl + r2 xl − lr2 x2 = r2 l − 2lr2 x = 0
dx
r2 x = 2r2 l → x =

l

Es decir, la corriente medida es mínima cuando la falla se encuentra en la mitad de la línea

---

### Página 84

Problema
Obtener la resistencia equivalente entre A y B aplicando las leyes de Kirchhoff

#### Solución
La resistencia equivalente entre a y b se puede obtener al ver la relación entre el voltaje aplicado
y la corriente que circula por el circuito. Se tiene
VA − VB = IReq

LCK para el nodo A
I=

(VA − VD ) (VA − VC )
+
→ IR = 2VA − VC − VD
R
R

LCK para el nodo C
VC − VD VC − VB
VA − VC
=
+
→ VA = 3VC − VB − VD
R
R
R

Para el nodo D
VC − VD VA − VD
VD − VB
+
=
→ 3VD − VA − VC = VB
R
R
R

Y para el nodo B
VD − VB VC − VB
+
= I → IR = VC + VD − 2VB
R
R

---

### Página 85

Resolviendo
VB − VA = 3VD − VA − VC − 3VC + VB + VD
VB − VA = 4VD − VA − 4VC + VB → VD = VC
Es decir, la corriente entre D y C es cero. Así, el sistema queda
IR = 2VA − 2VC
VA = 2VC − VB
IR = 2VC − 2VB
Luego

VA + VB
= VC

Así
IR = VA − VB = IReq

Con lo que la resistencia equivalente es R

---

### Página 86

Problema
Calcular la diferencia de potencial entre los puntos a y b. Todas las fem tienen una resistencia
interna de 1 Ω

#### Solución
Para resolver este problema basta con notar que solo fluye corriente por la malla exterior, ya
que a y b forman un circuito abierto. Aplicando LVK alrededor del circuito se obtiene

2I + 2I + 12 + I + I + 2I − 8 + I = 0 → 9I = −4
I = −4/9A
Redefinamos I con su sentido correcto, es decir, el contrario al que habíamos supuesto. Así,
I = 4/9 en el sentido contrareloj.
Para obtener los potenciales en a y b, nos damos como referencia el punto c. Con esto
Va = 2I + Vc = 8/9 + Vc
Mientras que
Vc − 8 − I − 2I + 10 = Vb
+ 10 = Vc + 0, 667
Notar que no existe una caída de potencial a través de la resistencia de 3Ω ya que por ella
no pasa corriente. Finalmente
Vb = Vc − 8 −

Vb − Va = 0, 667 − 0, 888 = −0, 221V

---

### Página 87

11.5.

Circuitos RC

11.5.1.

Carga de un condensador

Considere el circuito de la figura. El condensador está conectado a una fuente de voltaje
DC (corriente continua) de fem ε. En t = 0 el interruptor S se cierra. Supongamos además que
el condensador inicialmente está descargado, q(t = 0) = 0

En particular, para t < 0, no hay voltaje entre los terminales del condensador, asi que éste
actúa como un corto circuito. Cuando t = 0, el interruptor se cierra y la corriente comienza a
fluir acorde con
ε
R
En este instante, la diferencia de potencial entre los terminales de la batería es la misma
que la diferencia de potencial a través de la resistencia. Esto inicia la carga del condensador.
Mientras éste comienza a cargarse, el voltaje a través de él aumenta en el tiempo
I0 =

q(t)
C
Para la malla utilizamos la ley de voltajes para un circuito cerrado, obteniendo
VC (t) =

−ε + VC (t) + I(t)R = 0
−ε +

q
dq
+ R=0
C
dt

Debido a que I debe ser la misma en todas las partes del circuito, la corriente a través de la
resistencia R es igual a la tasa de incremento de carga en las placas del condensador. El flujo de
corriente en el circuito irá decreciendo debido a que la carga presente en el capacitor haga cada
vez más difícil poner más carga en él. Una vez que la carga del condensador alcanza su maximo
valor Q, la corriente en el circuito caerá a cero. Esto es evidente al reescribir la ecuación de
malla como
I(t)R = ε − VC (t)

Así, el capacitor cargado satisface una ecuación diferencial de primer orden que relaciona la
tasa de cambio de carga con la carga en el condensador
dq
q
1
ε−
=
dt
R
C

---

### Página 88

Esta ecuación la podemos resolver con el método de separación de variables
dq
dq
dt →
=−
dt
q =
ε− C
R
q − Cε
RC
Ahora podemos integrar para obtener
ˆ q

dq
q = −
ε− C
RC

ln



ˆ t

dt

Lo que nos lleva a
q − Cε
−Cε



=−

t
RC

Finalmente, se obtiene


q(t) = Cε 1 − e−t/RC = Q 1 − e−t/RC
Donde Q = Cε es la cantidad máxima de carga almacenada por las placas. La independencia
temporal de q(t) se grafica en la figura

Teniendo la carga en el condensador, podemos determinar el voltaje a través de éste

q(t)
= ε 1 − e−t/RC
C
El gráfico del voltaje como función del tiempo tiene la misma forma que la carga a través
del condensador. De la figura, vemos que después de un tiempo suficientemente largo la carga
acumulada en el condensador tiende a
VC (t) =

lím q(t) = Cε = Q

t→∞

En el límite, el voltaje a través del condensador es igual al voltaje de la fuente y el proceso
de carga efectivamente termina
Q
q(t)
=
=ε
t→∞ C
C

lím VC (t) = lím

t→∞

La corriente en el circuito es igual a la razón de cambio de la carga en el condensador
I(t) =

dq
ε
= e−t/RC = I0 e−t/RC
dt
R

---

### Página 89

El coeficiente que acompaña a la exponencial es igual a la corriente inicial que fluye a través
del circuito cuando el interruptor fue cerrado en t = 0. El gráfico de la corriente en función del
tiempo es

La corriente en el circuito decrece exponencialmente en el tiempo. Se suele escribir de la
siguiente manera
I(t) = I0 e−t/τ
Donde τ = RC se llama constante de tiempo. En efecto, la unidad de τ en SI es el
segundo. La constante de tiempo τ es una medida del decaimiento temporal para la función
exponencial. Este decaimiento satisface la siguiente propiedad
I(t + τ ) = I(t)/e
Lo que muestra que despues de un tiempo τ la corriente cae por un factor de e−1 = 0,368,
como se ve en el gráfico. Similarmente, el voltaje a través del condensador también se puede
expresar en términos de esta constante
VC (t) = ε 1 − e−t/τ



Notar que inicialmente en t = 0, VC (t = 0) = 0. Después de un tiempo τ , la diferencia de
potencial a través del condensador ha aumentado un factor (1 − e−1 ) = 0,632 de su valor final.

VC (τ ) = ε 1 − e−1 = 0,632ε

---

### Página 90

11.5.2.

Descarga de un Condensador

Suponga ahora que el condensador ha sido cargado hasta un valor Q. Para t < 0, el interruptor está abierto y la diferencia de potencial a través del condensador está dada por VC = Q/C.
Por otro lado, la diferencia de potencial a través de la resistencia es cero por que no hay un
flujo de cargas, esto es I = 0. Ahora supongamos que en t = 0 el interruptor se cierra. El
condensador comenzará a descargarse

El condensador cargado ahora actúa como una fuente de voltaje para conducir corriente alrededor del circuito. Cuando el condensador se descarga (el flujo de electrones va desde la placa
negativa hasta la placa positiva), el voltaje entre sus extremos disminuye. Usando la ley de
Kirchhoff para un circuito cerrado
q(t)
− I(t)R = 0
C
Además se cumple
dq(t)
dt
El signo se debe al hecho de que un flujo de corriente implica una disminución en la diferencia
de polaridad de las placas del condensador. Así, la carga satisface la ecuación diferencial de
primer orden
I(t) = −

dq(t)
q(t)
+R
=0
C
dt
que también se puede resolver mediante el método de separación de variables
dq
=−
dt
q
RC
 
ˆ t
ˆ q
q
t
dq
dt → ln
=−
=−
RC 0
Q
RC
Q q
Así
q(t) = Qe−t/RC
Y el voltaje a través del condensador es
VC (t) =

q(t)
Q
= ( )e−t/RC
C
C

---

### Página 91

El gráfico del voltaje a través del capacitor en función del tiempo

La corriente también decae exponencialmente en el circuito
I=−

Q −t/RC
dq
=
e
dt
RC

---

### Página 92

Problema
En el circuito de la figura, suponga que el interruptor ha estado abierto por un tiempo muy
largo. En t = 0 se cierra

a) Cual es la constante de tiempo antes de que se cerrara el interruptor?
b) Cual es la constante de tiempo después de que se cierra el interruptor?
c) Encuentre la corriente a través del interruptor como función del tiempo una vez que el interruptor se ha cerrado.
#### Solución
a) Antes que el interruptor se cerrara, las dos resistencias R1 y R2 están en serie con el condensador. Debido a que la resistencia equivalente es Req = R1 + R2 , la constante de tiempo
está dada por
τ = Req C = (R1 + R2 )C

Y la carga almacenada en el condensador es
q(t) = Cε 1 − e−t/τ



b) Una vez que el interruptor se cierra, el circuito cerrado a la derecha se vuelve un circuito
RC que decae con constante de tiempo τ 0 = R2 C. La carga comienza a decaer acorde a
q 0 (t) = Cεe−t/τ

c) La corriente a través del interruptor consiste en 2 fuentes, la corriente constante I1 del
circuito izquierdo, y la corriente que decae I2 del circuito RC. Las corrientes están dadas por
I1 =
I 0 (t) =

ε
R1

dq 0
ε
Cε
= − 0 e−t/τ = − e−t/R2 C
dt
τ
R2

Así, ya que I1 e I 0 van en la dirección hacia abajo a través del interruptor, la corriente total
será
I(t) = I1 + I 0 (t) =

ε
ε −t/R2 C
+
e
R1 R2

---

### Página 93

Problema
Considere el circuito de la figura. Sea ε = 40V , R1 = 8Ω, R2 = 6Ω, R3 = 4Ω y C = 4µF . El
condensador inicialmente está descargado

En t = 0 el interruptor se cierra.
a) Encuentre la corriente a través de cada resistencia inmediatamente después de que el interruptor es cerrado.
b) Encuentre la carga final del capacitor.
#### Solución
a) Inmediatamente después de que el interruptor se cierra, el condensador equivale a un corto
circuito, ya que el voltaje en t = 0 a través de éste es nulo. Es decir, en el instante justo en que
se cierra el interruptor el circuito equivale a

Para la malla 1
−ε + I1 R1 + R2 (I1 − I2 ) = 0
Para la malla 2
R2 (I2 − I1 ) + I2 R3 = 0

Reemplazando los valores numéricos, se tiene
−40 + 8I1 + 6(I1 − I2 ) = 0 → I1 =

40 + 6I2

6(I2 − I1 ) + 4I2 = 0 → I2 = I1
Resolviendo este sistema
70I1 = 200 + 18I1 → I1 = 3, 84A

---

### Página 94

con esto
I2 = 2, 3A
Finalmente la corriente por R2 será
I3 = I1 − I2 = 3, 84 − 2, 3 = 1, 54
Simulando el circuito, obtenemos las corrientes como función del tiempo

Notar que en t = 0 los valores coinciden con los obtenidos recién. Ver también como el
circuito llega a un estado estacionario en un margen de tiempo de los 120 µ s.
Por último, es claro como la corriente I3 decae rápidamente a cero a medida que el condensador
se va cargando.

b) Después de un tiempo, el condensador se carga totalmente y este pasa a comportarse
como un circuito abierto, es decir, a través del condensador no pasa corriente.(y tampoco por
R3 )

Así, es fácil notar que el voltaje final a través del condensador será igual al voltaje a través
de la resistencia R2 .
−ε + I(R1 + R2 ) = 0 → I =

=

Y el voltaje a través de R2 será
= 17, 14(V ) = VC (t = ∞)
Así, la carga final del condensador se puede obtener como
VR2 = IR2 = 6

Q(t = ∞) = CVC = 4µF ∗ 17, 14 = 6, 85 ∗ 10−5 C

---

### Página 95

El voltaje en el condensador en función del tiempo es

---

### Página 96

Problema
En el circuito de la figura, el interruptor se encuentra cerrado durante un tiempo muy largo.
a) ¿Cuál es la corriente en cada resistencia?
b) ¿Cuál es la carga en el condensador C?
c) En t=0 se abre el interruptor S. Encuentre la corriente que pasa por la resistencia R2 en
función de t.
d) ¿Cuánto tiempo debe pasar para que la carga en C disminuya hasta 4/5 del valor en t=0?

#### Solución
a) El interruptor ha estado cerrado durante un tiempo muy largo, esto significa que el condensador se ha cargado completamente. Cuando esto sucede, el condensador equivale a un circuito
abierto, es decir, no pasa corriente a través de él. Bajo estas circunstancias, sólo habrá corriente
por la malla 1, así

LVK en malla 1
−ε + I1 R2 + I1 R1 = 0 → I1 =

V
R1 + R 2

Que es la corriente por R1 y por R2 , por lo dicho anteriormente, la corriente por R3 es cero.

---

### Página 97

b) Para obtener la carga en el condensador, primero debemos obtener el voltaje a través de
él, y luego utilizar la relación que relaciona el voltaje con la carga acumulada
VC (t) = Cq(t)
Nos interesa la carga final del condensador, esto es
VC (t → ∞)
C
Como ya vimos, después de un tiempo suficientemente largo no hay corriente por la malla
derecha, así, no hay una diferencia de potencial a través de R3 . Por lo tanto el voltaje en el
condensador será igual al voltaje a través de R2
lím q(t) =

t→∞

lím VC (t) = VR2 = I1 R2

t→∞

VC (∞) =

V R2
R1 + R 2

q = CV =

V CR2
R1 + R2

y así

c) Notemos que al abrir el interruptor, no pasa corriente por la malla 1 y se inicia un proceso
de descarga en el condensador.

Si esto no parece evidente, veamos la ecuación de la malla 2
I2 R3 − VC (t) + R2 I2 = 0
q(t)
C
Notemos que I2 es positiva, es decir, el sentido que le asignamos es el correcto. Esto significa
que cargas positivas están dejando la placa positiva y están llegando a la placa negativa. Es
decir, la carga entre las placas va disminuyendo en la medida en que I2 sea positiva. Esto se
traduce en
I2 (R2 + R3 ) = VC (t) =

dq
dt
Así, obtenemos una ecuación diferencial de primer orden para q(t)
I2 = −

---

### Página 98

−

dq
q(t)
(R2 + R3 ) =
dt
C

dq
q(t)
(R2 + R3 ) +
=0
dt
C
Ecuación homogénea cuya solución es de la forma
q(t) = q0 e−t/(C(R2 +R3 ))
con q0 la carga inicial del condensador, calculada anteriormente como
q0 =

R2 V C
(R1 + R2 )

Finalmente,
I(t) = −

dq
q0
=
e−t/C(R2 +R3 )
dt
C(R2 + R3 )

d) Para determinar el tiempo que debe pasar para obtener 4/5 de la carga inicial, resolvemos
la ecuación
q0 = q0 e−t/(C(R2 +R3 ))
ln(4/5) = −

t
C(R2 + R3 )

con lo que
t = ln(5/4)(R2 + R3 )C

---

### Página 99

Problema
Dos baterías de FEM ε1 y ε2 y resistencias R1 y R2 se conectan en paralelo con una resistencia
R

a) Calcule la potencia entregada por cada batería
b) Ahora se reemplaza la resistencia R por un interruptor S y un condensador C en serie.

El interruptor se cierra en t=0
i) Calcule la carga q en el condensador como función del tiempo
ii) Calcule la corriente en cada resistencia como función del tiempo
#### Solución
a)Para obtener la potencia entregada por cada batería, debemos conocer la corriente que pasa
por cada una, y lo hacemos usando la LVK para las mallas 1 y 2, como se muestra en la figura

Para la malla 1
−ε1 + I1 R1 + R2 (I1 − I2 ) + ε2 = 0
En la malla 2
−ε2 + R2 (I2 − I1 ) + I2 R = 0

---

### Página 100

De la primera ecuación se obtiene

I1 =

R2 I2 + ε1 − ε2
R1 + R2

Reemplazando en la segunda
−ε2 + I2 (R2 + R) = I1 R2 =

R22 I2 + R2 (ε1 − ε2 )
R1 + R2

Así
−ε2 (R1 + R2 ) + I2 (R2 + R)(R1 + R2 ) = R22 I2 + R2 (ε1 − ε2 )
−ε2 (R1 + R2 ) + I2 (R2 R1 + R22 + RR1 + RR2 ) = R22 I2 + R2 (ε1 − ε2 )
I2 (R2 R1 + RR1 + RR2 ) = R2 (ε1 − ε2 ) + ε2 (R1 + R2 )
I2 =

ε1 R2 + ε2 R1
R(R1 + R2 ) + R1 R2

Y entonces, I1 está dada por
I1 =
I1 =

R2 I2 + ε1 − ε2
ε1 R22 + ε2 R1 R2 + (ε1 − ε2 )(R(R1 + R2 ) + R1 R2 )
=
R1 + R 2
(R(R1 + R2 ) + R1 R2 )(R1 + R2)

ε1 R22 + ε2 R1 R2 + ε1 RR1 + ε1 R1 R2 + ε1 RR2 − ε2 RR1 − ε2 RR2 − ε2 R1 R2
(R(R1 + R2 ) + R1 R2 )(R1 + R2)
I1 =

R(ε1 − ε2 )(R1 + R2 ) + R2 ε1 (R1 + R2 )
(R(R1 + R2 ) + R1 R2 )(R1 + R2)

Finalmente,
I1 =

R(ε1 − ε2 ) + R2 ε1
R(R1 + R2 ) + R1 R2

Y la corriente por la fem ε2 es
I3 = I1 − I2 =

R(ε1 − ε2 ) + R2 ε1 − ε1 R2 − ε2 R1
R(ε1 − ε2 ) − ε2 R1
=
R(R1 + R2 ) + R1 R2
R(R1 + R2 ) + R1 R2

Con esto, la potencia entregada por ε1 es
P1 = I1 ε1 = ε1

R(ε1 − ε2 ) + R2 ε1
R(R1 + R2 ) + R1 R2

Y la potencia entregada por ε2
P2 = −I3 ε2 = ε2

R(ε2 − ε1 ) + ε2 R1
R(R1 + R2 ) + R1 R2

---

### Página 101

b)

Aquí, la ecuación de la malla 1 es equivalente al caso anterior, donde se obtuvo
I1 =

R2 I2 + ε1 − ε2
R1 + R2

Para la malla 2
−ε2 + R2 (I2 − I1 ) + VC = 0 → −ε2 + R2 I2 − R2 I1 +

q
=0
C

Reemplazando I1

−ε2 + R2 I2 − R2 (
−ε2 +

R2 I2 + ε1 − ε2
q
)+ =0
R1 + R2
C

R22 I2 + R1 R2 I2 − R22 I2 − R2 (ε1 − ε2 )
q
+ =0
R1 + R2
C
I2

R1 R2
q
ε1 R2 + ε2 R1
+ =
R1 + R2 C
R1 + R2

Pero I2 = dq/dt
q
ε1 R2 + ε2 R1
dq R1 R2
+ =
dt R1 + R2 C
R1 + R2
ε1 R2 + ε2 R1
dq CR1 R2
+q =C
dt R1 + R2
R1 + R2
Sean
τ=

CR1 R2
ε1 R2 + ε2 R1
,A = C
R1 + R 2
R1 + R2

Entonces
dq
τ +q =A
dt
Cuya solución es
q(t) = A(1 − e−t/τ )
Con esto,
I2 (t) =
I1 (t) = (

dq(t)
A
= e−t/τ
dt
τ

R2
A
ε1 − ε2
) e−t/τ +
R1 + R2 τ
R1 + R2

---

### Página 102

Y la corriente por R2
I3 (t) = I1 (t) − I2 (t) = (

R2
A
ε1 − ε2
A
) e−t/τ +
− e−t/τ
R1 + R2 τ
R1 + R2
τ

---

### Página 103

Problema
Considere el circuito de la figura. Inicialmente el circuito ha estado abierto largo tiempo
a) Calcule la carga del condensador, con el interruptor abierto
b) Si el interruptor se cierra y transcurre mucho tiempo, encuentre la nueva carga del condensador

#### Solución
a) Antes que se cierre el interruptor, sólo se debe considerar el circuito de la derecha

Si ha pasado mucho tiempo, ha dejado de circular corriente y el condensador está cargado
completamente
Q = CV

b) Si se cierra el interruptor, el circuito es el siguiente

Como ha pasado mucho tiempo, el condensador está cargado y no hay corriente hacia él.

---

### Página 104

De esta forma, la corriente circula según

Se tiene
V1 + I(R1 + R2 ) − V2 = 0
Luego
I=

V2 − V1
R1 + R2

Con esto podemos determinar la diferencia de potencial entre los terminales del condensador

Sea
∆V = Vb − Va
−∆V + V1 + IR1 = 0
Luego
R1 V2 + R2 V1
R1 + R2
con esto, la carga almacenada en el condensador es
∆V =

Q = C∆V
Q=C

R1 V2 + R2 V1
R1 + R2

---

### Página 105

Problema
Inicialmente el condensador de capacidad C1 tiene carga Q0 , y el segundo condensador está descargado. Encuentre la pérdida de energía por calor de Joule al conectar ambos condensadores
mediante un conductor de resistencia R, como muestra la figura

#### Solución
Definimos la corriente por el circuito según se muestra en la figura

La ecuación de la malla entrega
−V1 + IR + V2 = 0
donde los voltajes entre los extremos de cada condensador se relacionan con las cargas
V1 =

Q1
C1

V2 =

Q2
C2

La ecuación a resolver es
−

Q1
Q2
+ IR +
=0
C1
C2

Pero Q1 , Q2 e I no son independientes. En efecto
I(t) =

dQ2
dQ1
=−
dt
dt

Notar que esto es consistente con
d
(Q1 + Q2 ) = 0
dt
pues por conservación de la carga
Q1 (t) + Q2 (t) = Q0

---

### Página 106

Luego, derivando una vez con respecto al tiempo
−

1 dQ1 dI(t)
1 dQ2
+
R+
=0
C1 dt
dt
C2 dt

dI(t)
I(t) +
I(t) = 0
R+
C1
dt
C2


dI(t)
+
=−
dt
R C1 C2

Finalmente

dI(t)
=−
dt
R



C1 + C2
C1 C2



I(t)

La solución de esta ecuación es
−R

I(t) = Ke



C1 +C2
C1 C2



t

donde K es una constante a determinar. Considerando que el condensador 2 está inicialmente
descargado
Q2 (0) = 0
Se tiene
Q2 (t) =

ˆ t

dτ I(τ ) = K

ˆ t

−R

dτ e



C1 +C2
C1 C2



t

KRC1 C2
Q2 (t) =
C1 + C2



−R

1−e



C1 +C2
C1 C2

 
t

La constante K se puede determinar imponiendo que para todo t ∈ R+
−

Q1 (t)
Q2 (t)
+ I(t)R +
=0
C1
C2

Como Q1 (t) = Q0 − Q2 (t)
Q0 Q2 (t)
Q2 (t)
+
+ I(t)R +
=0
C1
C1
C2


C1 + C2
Q0
Q2 (t) + I(t)R = 0
+
−
C1
C1 C2
−

Reemplazando




 


1 C1 +C2
1 C1 +C2
Q0
C1 + C2
C1 C2
−R
−R
t
t
C1 C2
C1 C2
−
+
=0
KR
1−e
+ RKe
C1
C1 C2
C1 + C2
−

Q0
+ KR = 0
C1

Luego

---

### Página 107

Q0
RC1
Equivalentemente uno podría haber notado que en t = 0, el condensador 2 se comporta
como un cortocircuito, y el voltaje inicial en el condensador 1 es
K=

V1 (0) =

Q0
C1

de forma que
I(0) =

V1 (0)
Q0
=
R
C1 R

La potencia disipada en la resistencia está dada por
P (t) = RI 2 (t) = R

Q20 −2 (CRC1 +CC2 ) t
1 2
e
R2 C12

y la energía perdida será
−∆E =

ˆ ∞

dt

1 +C2 ) t
Q20 − 2(C
Q20 C2
RC1 C2
e
=
RC12
2C1 (C1 + C2 )

Notar que es independiente de R! Esta pérdida de energía coincide exactamente con la diferencia de energía almacenada por el sistema antes y después de conectar ambos condensadores

---

### Página 108

Problema
Encuentre en el circuito de la figura la intensidad de corriente eléctrica por cada rama y la carga
en cada condensador al tiempo t. Asuma que inicialmente los condensadores están descargados

#### Solución
Definimos las corrientes que se indican en la figura, asi como las cargas en cada condensador

Por supuesto que debe tenerse
I(t) = I1 (t) + I2 (t)
Tomando el circuito cerrado que involucra a la fuente, la resistencia R1 y el condensador C1
se tiene
−V + I1 (t)R1 +

Q1
=0
C1

Por otro lado, considerando el circuito cerrado que contiene a V , R2 y C2
−V + I2 R2 +

Q2
=0
C2

Además se tiene
I1 (t) =

dQ1 (t)
dt

dQ2
dt
De esta forma, y derivando las ecuaciones obtenidas anteriormente
I2 (t) =

1 dQ1 (t)
dI1 (t)
+ R1
=0
C1 dt
dt
dI1 (t)
I1 (t) + R1
=0
C1
dt

---

### Página 109

luego
dI1 (t)
=−
I1 (t)
dt
R1 C1
del mismo modo

dI2 (t)
I2 (t)
=−
dt
R2 C2

Resolviendo
−

t

−

t

I1 (t) = K1 e R1 C1
I2 (t) = K2 e R2 C2
Las constantes K1 y K2 se determinan de forma inmediata al considerar que en t = 0 ambos
condensadores se comportan como un cortocircuito y entonces
V
R1
V
I2 (0) =
R2

I1 (0) =

con esto
V − R tC
e 1 1
R1


t
−
Q1 (t) = V C1 1 − e R1 C−1
I1 (t) =

V − R tC
e 2 2
R2


− R tC
Q2 (t) = V C2 1 − e
I2 (t) =
