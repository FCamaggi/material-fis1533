---
title: "Resumen FIS1533 (2)"
source_pdf: "Electro/2025-2/Material_Extra/Resumen_FIS1533 (2).pdf"
pages: 21
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Resumen FIS1533 (2)

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Resumen - FIS1533
2° Semestre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Contenidos
1 Electrostática
1.1 Ley de Coulomb - Generalidades . . . . . . . . . . . . . . . . . . . . . . . . . .
1.2 Ley de Coulomb - Cómo Utilizarlo Correctamente . . . . . . . . . . . . . . . .
1.3 Campo Eléctrico - Distribución Discreta de Carga . . . . . . . . . . . . . . . .
1.4 Campo Eléctrico - Cómo Utilizarlo Correctamente I . . . . . . . . . . . . . . .
1.5 Campo Eléctrico - Distribución Continua de Carga . . . . . . . . . . . . . . . .
1.6 Campo Eléctrico - Cómo Utilizarlo Correctamente II . . . . . . . . . . . . . . .

2 Ley de Gauss
2.1 Ley de Gauss - Generalidades . . . . . . . . . . . . . . . . . . . . . . . . . . . .
2.2 Ley de Gauss - Cómo Utilizarlo Correctamente . . . . . . . . . . . . . . . . . .

3 Potencial Electrostático
3.1 Potencial Electrostático - Distribución Discreta de Carga . . . . . . . . . . . .
3.2 Potencial Electrostático - Distribución Continua de Carga . . . . . . . . . . . .
3.3 Potencial Electrostático - Cómo Utilizarlo Correctamente I . . . . . . . . . . .
3.4 Potencial Electrostático - Otras Expresiones . . . . . . . . . . . . . . . . . . . .
3.5 Potencial Electrostático - Cómo Utilizarlo Correctamente II . . . . . . . . . . .

4 Trabajo y Energía en Electrostática
4.1 Trabajo y Energía en Electrostática - Generalidades . . . . . . . . . . . . . . .

5 Conductores
5.1 Conductores - Generalidades . . . . . . . . . . . . . . . . . . . . . . . . . . . .
5.2 Conductores - Cómo Utilizarlo Correctamente . . . . . . . . . . . . . . . . . . .

6 Condensadores
6.1 Condensadores - Generalidades . . . . . . . . . . . . . . . . . . . . . . . . . . .
6.2 Condensadores - Cómo Utilizarlo Correctamente . . . . . . . . . . . . . . . . .

7 Medios Dieléctricos
7.1 Dieléctricos - Polarización, Susceptibilidad y Constante Dieléctrica . . . . . . .
7.2 Dieléctricos - Campo Eléctrico y Ley de Gauss Generalizada . . . . . . . . . . .
7.3 Dieléctricos - Cómo Utilizarlo Correctamente I . . . . . . . . . . . . . . . . . .
7.4 Dieléctricos - Cómo Utilizarlo Correctamente II . . . . . . . . . . . . . . . . . .
7.5 Dieléctricos - Cómo Utilizarlo Correctamente III . . . . . . . . . . . . . . . . .

---

### Página 2

8 Anexos
8.1 Series de Taylor . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
8.2 Transformación de Unidades . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
8.3 Prefijos del Sistema Internacional . . . . . . . . . . . . . . . . . . . . . . . . . .
8.4 Ecuación de la Recta . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
8.5 Coordenadas y Diferenciales . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
8.6 Aplicación Ley de Gauss . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
8.7 Coordenadas y Operador ∇ . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

---

### Página 3

Electrostática

1.1

Ley de Coulomb - Generalidades

En primer lugar, la carga eléctrica será siempre un número entero del valor de la carga de un
electrón:
e = 1.6 × 10−19 C

(1)

Donde = C” es Coulomb, la unidad de medida para la carga.

Ahora, y para una distribución discreta de cargas, la fuerza sobre una carga = q2 ” debido a una
carga = q1 ” ubicada a una distancia = r” se puede escribir como:
Fe = ke

q1 q2
1 q1 q2
r̂12 =
r̂12
r
4πε0 r2

(2)

Donde = ε0 ” y = ke ” son la constante de permitividad del
vacío y la constante de Coulomb, respectivamente:

C2
(3)
N · m2
N · m2
ke =
≈ 9 × 109
(4)
4πε0
C2
Finalmente, y gracias al principio de superposición, para un sistema de = N ” cargas puntuales
la fuerza total sobre la carga = Q” está dada por la suma de las fuerzas ejercidas por cada una
de estas cargas:
ε0 = 8.85 × 10−12

N

Fe (x) =

Q X (x − xj ′ )
qj
4πε0
|x − xj ′ |3

(5)

j=1

Figura 1. Diagrama de vectores para fuerza eléctrica entre dos cargas.

1.2

Ley de Coulomb - Cómo Utilizarlo Correctamente

Los pasos a seguir recomendados para aplicar la Ley de Coulomb son:
1. Considerar los signos de las cargas para determinar el sentido y dirección de la fuerza
eléctrica, recordando que signos opuestos se atraen y que signos iguales se repelen.
2. Calcular el módulo de la fuerza asociada a cada par de cargas y ponderarlo de acuerdo
a su descomposición vectorial en las coordenadas respectivas. Se recomienda representar
gráficamente los vectores para comprenderlo de mejor manera.

---

### Página 4

1.3

Campo Eléctrico - Distribución Discreta de Carga

El campo eléctrico generado por una carga puntual = q” puede ser expresado como:
E(r) =

1 q
r̂
4πε0 r2

(6)

Donde = r” es la distancia al punto deseado.
Luego, se puede reescribir la fuerza eléctrica como:

Fe = qE

(7)

También, es posible utilizar esta última expresión en su forma diferencial.

Ahora, y gracias al principio de superposición, para un sistema de = N ” cargas puntuales el
campo eléctrico total sobre un punto en el espacio está dado por la suma de los campos
eléctricos generados por cada una de estas cargas:
N

1 X (x − xj ′ )
E(x) =
qj
4πε0
|x − xj ′ |3

(8)

j=1

Figura 2. Líneas de campo eléctrico correspondientes a cargas positivas y negativas.
Por último, y como se puede observar, las líneas de campo eléctrico se originan
en cargas positivas (hacia afuera) y terminan en cargas negativas (hacia dentro).
Pueden seguir experimentando con estos conceptos en Cargas y Campos Eléctricos.

1.4

Campo Eléctrico - Cómo Utilizarlo Correctamente I

Los pasos a seguir recomendados para aplicar el campo eléctrico por definición en distribuciones
discretas de carga son:
1. Considerar los signos de las cargas para determinar el sentido y dirección de las líneas
de campo eléctrico en el punto requerido.
2. Calcular el módulo del campo asociado a cada carga y ponderarlo de acuerdo a su descomposición vectorial en las coordenadas respectivas. Se recomienda representar gráficamente
los vectores para comprenderlo de mejor manera.

---

### Página 5

1.5

Campo Eléctrico - Distribución Continua de Carga

Para una distribución continua de carga, el campo eléctrico está dado por:
Z
(x − x ′ )
E(x) =
dq(x ′ )
4πε0
|x − x ′ |3

(9)

Donde = dq(x ′ )” se refiere a la densidad de carga que posee el cuerpo, la cual puede ser:

Densidad

Relación Diferencial

Integral Campo Eléctrico

Lineal

dq(x ′ ) = λ(x ′ ) dl′

E(x) = 4πε

Superficial

dq(x ′ ) = σ(x ′ ) ds′

E(x) = 4πε

RR

Volumétrica

dq(x ′ ) = ρ(x ′ ) dv ′

E(x) = 4πε

RRR

R

(x−x ′ )
′
′
L |x−x ′ |3 λ(x ) dl
(x−x ′ )
′
′
S |x−x ′ |3 σ(x ) ds
(x−x ′ )
′
′
V |x−x ′ |3 ρ(x ) dv

Asimismo, se puede extender la definición de fuerza eléctrica a distribuciones continuas de
carga:
Z
Fe (x) = E dq(x)
(10)
Donde = E” es el campo eléctrico experimentado por el objeto
en estudio y = dq(x)” la densidad de carga del mismo.

1.6

Campo Eléctrico - Cómo Utilizarlo Correctamente II

Los pasos a seguir para aplicar el campo eléctrico por definición en distribuciones continuas de
carga son:
1. Reconocer el tipo de densidad de carga asociado al cuerpo en estudio, según la dimensión
en la que vive. Por ejemplo, un disco es bidimensional y, por lo tanto, su densidad sería
superficial.
2. Luego, cambiar el diferencial de carga = dq(x ′ )” según el tipo de densidad y calcular el
valor de la densidad de carga si es que no la entregan de manera explícita. En este paso
se deberá utilizar el tipo de coordenada pertinente al problema y las relaciones entre los
diferenciales, las cuales se pueden encontrar en la tabla del Anexo ??.
3. Después, y respetando el tipo de coordenadas en uso, se tendrá que construir = x”, el cual
es un vector que se extiende desde el origen hasta el punto deseado. Siempre recuerden
agregar el sentido y dirección de un vector.
4. Por último, y respetando el tipo de coordenadas en uso, se tendrá que construir = x ′ ”, el
cual es un vector que recorre desde el origen todo el cuerpo cargado. Siempre recuerden
agregar el sentido y dirección de un vector.
5. No hay que olvidar los límites de integración, los cuales dependerán netamente del ejercicio en cuestión. Será más fácil guiarse por la figura que generalmente se encontrará a
disposición.
6. Por último, solo quedaría integrar la expresión cuidadosamente. Recuerden que el campo
eléctrico es un vector (por lo que también posee sentido y dirección) y que no es posible
mezclar términos que pertenezcan a distintas coordenadas a la hora de integrar.

---

### Página 6

Ley de Gauss

2.1

Ley de Gauss - Generalidades

El flujo de un campo eléctrico = E” a través de una superficie = S” está dado por:
Z
E · ds
Φe =

(11)

S

Se debe considerar que solo la componente ortogonal a la superficie contribuye al flujo.

Luego, la Ley de Gauss se puede enunciar como:
I
Qenc
E · ds =
ε0
S

(12)

Donde = Qenc ” es la carga encerrada y = ds” la diferencial de superficie.

Finalmente, y aplicando el teorema de la divergencia al flujo del campo eléctrico, es posible
obtener la primera ecuación de Maxwell en el vacío:
ρ
(13)
∇·E=
ε0

2.2

Ley de Gauss - Cómo Utilizarlo Correctamente

Es importante aclarar que esta ley solo se podrá utilizar cuando el problema presente simetría
plana, cilíndrica o esférica. De aquí en adelante, y siempre cuando lo amerite, se deberá tratar
de usar la Ley de Gauss por sobre la definición de campo eléctrico para resolver de una manera
más sencilla los ejercicios. Así, la aplicación consta de dos partes:
H
a) = S E · ds ”: en esta se calculará el flujo que aporta el campo eléctrico al pasar por la
superficie gaussiana. De esta manera:
1. Se deberá elegir la superficie gaussiana según la simetría del cuerpo.
2. Calcular el flujo eléctrico, considerando que solo la componente perpendicular a la
superficie gaussiana contribuye a su valor.
3. Generalmente, este cálculo resultará en el producto entre el área de la superficie
gaussiana = importante” y la componente ortogonal del campo. Todos los aspectos
revelantes se resumen en la tabla del Anexo 8.6.
b) = Qεenc
”: en esta parte se deberá calcular la carga del cuerpo que está encerrada por la
superficie gaussiana.
1. Luego, se deberá despejar el campo eléctrico de la igualdad.
2. En caso de requerir la forma vectorial del campo, se añade el componente vectorial
que aporta al flujo, el cual será siempre hacia fuera del cuerpo (vector normal = n̂”).
3. Todo este procedimiento se debe realizar para cada intervalo existente, los cuales se
pueden reconocer fácilmente mediante los = cortes” visuales del cuerpo.
4. Además, una superficie cargada provocará una discontinuidad en el campo eléctrico.
Gráficamente esto podría verse como una = punta”, lo cual matemáticamente equivaldría a una inexistencia del límite en el punto respectivo (en otras palabras, los
límites por la derecha e izquierda del punto no coinciden en su valor).

---

### Página 7

Potencial Electrostático

3.1

Potencial Electrostático - Distribución Discreta de Carga

El potencial eléctrico generado por una carga puntual = q” puede ser expresado como:
1 q
4πε0 r

V (r) =

(14)

Donde = r” es la distancia al punto deseado.

De esta manera,, y gracias al principio de superposición, para un sistema de = N ” cargas
puntuales el potencial eléctrico total sobre un punto en el espacio está dado por la suma de los
potenciales eléctricos generados por cada una de estas cargas:
N

qj
1 X
V (x) =
4πε0
|x − xj ′ |

(15)

j=1

3.2

Potencial Electrostático - Distribución Continua de Carga

Para una distribución continua de carga, el potencial eléctrico está dado por:
Z
V (x) =
dq(x ′ )
4πε0
|x − x ′ |

(16)

Donde = dq(x ′ )” se refiere a la densidad de carga que posee el cuerpo, la cual puede ser:

Densidad

Relación Diferencial

Lineal

dq(x ′ ) = λ(x ′ ) dl′

V (x) = 4πε

Superficial

dq(x ′ ) = σ(x ′ ) ds′

V (x) = 4πε

RR

Volumétrica

dq(x ′ ) = ρ(x ′ ) dv ′

V (x) = 4πε

RRR

3.3

Integral Potencial Eléctrico
′
′
L |x−x ′ | λ(x ) dl

R

′
′
S |x−x ′ | σ(x ) ds
′
′
V |x−x ′ | ρ(x ) dv

Potencial Electrostático - Cómo Utilizarlo Correctamente I

Los pasos a seguir para aplicar el potencial eléctrico por definición en distribuciones continuas
y discretas de carga son idénticos al de campo eléctrico. Por ello, se recomienda repasar la
#### Sección 1.4 y 1.6.

---

### Página 8

3.4

Potencial Electrostático - Otras Expresiones

Gracias al teorema de Stokes, se puede obtener la segunda ecuación de Maxwell:
I
E · d⃗l = 0 → ∇ × E = 0

(17)

Ahora, y como la integral de línea es independiente del camino de integración, el potencial
eléctrico se puede escribir como:
Z rb
E · d⃗l
(18)
E = −∇V → V (rb ) − V (ra ) = −
ra

Esta última expresión es más fácil de resolver que la dada por definición, por lo que hay
que tenerla siempre en mente a la hora de enfrentar un ejercicio. En caso de presentarse
más de un valor de campo eléctrico, se deberá separar la integral en varias partes y con
sus respectivos límites. Asimismo, el = Volt” es la unidad de medida para el potencial:

J
(19)
C
Finalmente, y mediante la primera ecuación de Maxwell y la relación de potencial, se puede
obtener la ecuación de Poisson:
ρ
(20)
∇2 V = −
ε0
1V=1

En ausencia de cargas, esta expresión se transforma en la ecuación de Laplace:

∇2 V = 0

3.5

(21)

Potencial Electrostático - Cómo Utilizarlo Correctamente II

En primer lugar, estas expresiones se usarán generalmente en conjunto con la Ley de Gauss.
De esta manera, los pasos serán los siguientes para determinar el potencial eléctrico:
1. Calcular el campo eléctrico generado por el cuerpo mediante Ley de Gauss, siempre y
cuando se cumplan las condiciones de simetría.
2. Luego, utilizar la forma integral de la relación campo - potencial:
Z rb
V (rb ) − V (ra ) = −
E · d⃗l
ra

3. Ahora, nos podemos enfrentar a dos casos. El primero es que nos pidan un potencial con
un límite bien = definido” o que no dependa de algo variable. Así, solo necesitaríamos el
campo entre esos límites:
Z a
V (a) − V (b) = −
Ea<r<b · d⃗l
b

4. El otro caso es que nos pidan un potencial con un límite que dependa de alguna variable,
generalmente del radio = r”. Luego, necesitaríamos el campo que va desde = r” hasta el
infinito para formar la integral del potencial:
Z r
V (r) − V (∞) = −
E · d⃗l
∞

---

### Página 9

Se debe considerar que el usar V (∞) es algo nada más estratégico, pues
generalmente este poseerá un valor nulo. La idea es que el segundo término sea algo
fácil de manipular, por lo que conviene que sea una constante o 0. Además, se deberá
separar la integral si es que observamos distintos campos en los intervalos respectivos.

5. Por último, si un cuerpo se conecta a = tierra” su potencial será nulo. Asimismo, el que
dos cuerpos estén unidos mediante un cable significará que su potencial será idéntico y
que se repartirán las cargas entre ellos según el principio de conservación de carga.

Trabajo y Energía en Electrostática

4.1

Trabajo y Energía en Electrostática - Generalidades

En primer lugar, el trabajo necesario para mover una carga = q” desde el punto = x1 ” hasta el
punto = x2 ” en contra de un campo eléctrico = E(x)” estará dado por:
Z x2
qE(x) · dx = q(V2 − V1 )
(22)
W =−
x1

Suponiendo que el potencial en el infinito es cero, el trabajo necesario
para traer una carga desde el infinito hasta un punto = x” es entonces:

W = qV (x)
(23)
De esta manera, la energía potencial almacenada en un sistema compuesto por = N ” cargas
puntuales se puede escribir como:
U=

N

N

i=1

i=1 j>i

1X
1 X X qi qj
qi V (xi ) =
4πε0
rij

(24)

Donde = V (xi )” es el potencial en la posición de la carga = i” debido a las demás cargas.
Análogamente, para una distribución continua de carga se tiene que:

U=

Z
V (x) dq(x) =

ε0

Z

|E|2 dτ

R3

Ambas expresiones son equivalentes, por lo que el
uso de una u otra dependerá de los datos entregados.

(25)

---

### Página 10

Conductores

5.1

Conductores - Generalidades

Los materiales conductores (tales como los metales) presentan ciertas propiedades que les son
inherentes por naturaleza. Así, los electrones se podrán mover libremente en su interior y
seguirán en movimiento mientras experimenten un campo eléctrico; sin embargo, estos se detendrán si no están provistos continuamente de una fuente de energía externa.
De esta manera:
a) El campo eléctrico dentro de un conductor es nulo.
b) Luego, por Ley de Gauss y el principio de conservación de carga, la carga en un conductor
necesariamente debe distribuirse equipotencialmente y solo en su superficie:
I
E · ds = 0 → Qenc = 0
(26)
S

Al mismo tiempo, esto significa que al interior
de un conductor el potencial eléctrico es constante:

⃗ =0
−∇V

(27)

c) La componente tangencial del campo eléctrico en la superficie de un conductor es cero,
por lo que solo sobrevivirá la componente normal a esta.

5.2

Conductores - Cómo Utilizarlo Correctamente

En variados ejercicios les pedirán determinar la carga superficial inducida en las superficies del
conductor. Los pasos a seguir son:
1. = Calcular” estratégicamente el campo en un lugar que contenga conductor y que esté
justo afuera de la superficie relacionada con la carga pedida. Por propiedades, este
campo debe ser nulo e implica necesariamente que la carga encerrada es 0:
I
E · ds = 0 → Qenc = 0
S

2. Ahora, se debe centrar en la sumatoria de carga encerrada. Además de la carga = normal”,
se debe considerar la carga inducida que se encuentra en la superficie del conductor, por
lo que:
Qenc = Qa + Qb = 0
Este ejemplo sería el de una carga encerrada normal = Qa ”,
junto con una carga inducida = Qb ” en la superficie de un conductor r = b.

3. ¿Cómo se calcula la carga en la otra superficie del conductor? Mediante el principio de
conservación de carga, las cargas inducidas sumadas deben ser igual a la carga original
del conductor:
Q1 = Qb + Qc
Donde = Q1 ” es la carga original del conductor, = Qb ” la carga inducida en una superficie
interior r = b y = Qc ” la carga inducida en una superficie exterior r = c, por ejemplo.

---

### Página 11

Condensadores

6.1

Condensadores - Generalidades

Un condensador es un dispositivo capaz de acumular carga eléctrica, que generalmente consiste
en dos conductores cargados con cargas opuestas de igual magnitud. De esta forma, la carga
almacenada en un condensador está dada por:
Q = C∆V

(28)

Donde = C” es una constante de proporcionalidad llamada capacitancia. Esta se mide en = Farad”:

C
V
Por otra parte, la energía almacenada por un capacitor se puede expresar como:
Z Q
q
U=
dq
0 C
1F=1

(29)

(30)

Resolviendo, y reemplazando por la expresión que
relaciona carga almacenada con capacitancia, se obtiene que:

U=

1 Q2
= CV 2 = QV
2 C

(31)

Asimismo, la fuerza entre conductores cargados se puede escribir como:

⃗ )
F⃗ = (∇U

⃗ )
= − (∇U
V =cte

(32)
Q=cte

Finalmente, podría ser de utilidad saber la capacitancia de un condensador de placas paralelas:
C=

εA
d

(33)

Donde = ε” es la constante de permitividad del medio que se encuentra
rellenando totalmente el espacio entre ambas placas, = A” el área = efectiva” de
las placas (proyección de una sobre la otra) y = d” la distancia entre las mismas.

6.2

Condensadores - Cómo Utilizarlo Correctamente

El fuerte en esta sección será determinar la capacitancia de cierta configuración:
1. ¿Dónde se ubican las cargas opuestas? Esto será fundamental, pues solo se deberá calcular
la diferencia de potencial entre estos límites de acuerdo a la siguiente expresión:
Z a
∆V = V (a) − V (b) = −
Ea<r<b · dl
b

Donde = a” y = b” indican la ubicación de la carga positiva y negativa.
De esta manera, se tendrá que calcular el campo eléctrico necesario para el potencial.

2. Luego, se utilizará la expresión que relaciona carga almacenada con capacitancia:
Q = C∆V → C =

Q
∆V

La capacitancia es propia de la geometría del cuerpo y es siempre un valor positivo.

---

### Página 12

Medios Dieléctricos

7.1

Dieléctricos - Polarización, Susceptibilidad y Constante Dieléctrica

El átomo posee un pequeño momento dipolar que apunta en la misma dirección que el campo
eléctrico tal que:
p = αE
Donde = α” es la polarizabilidad atómica.
Además, se puede definir el momento dipolar eléctrico por unidad de volumen como:

p=

∆p
∆v

Donde = p” es la polarización del material.

La polarización de un medio dieléctrico es el resultado de la aplicación de un campo eléctrico
externo:
p(x) = ε0 χe E(x)

(34)

Donde = E” es el campo eléctrico total y = χe ” la susceptibilidad eléctrica del medio.
Así, el vector desplazamiento para un dieléctrico lineal está dado por:

D(x) = ε0 (1 + χe )E(x) = εE(x)

(35)

Donde = ε” es la permitividad del material y = ε0 ” la permitividad del vacío.
Luego, se puede definir la permitividad relativa o constante dieléctrica como:

κ = εr =

ε
= 1 + χe
ε0

(36)

Notar que = κ” es siempre mayor que 1, excepto en el vacío, donde es igual a 1.

7.2

Dieléctricos - Campo Eléctrico y Ley de Gauss Generalizada

La densidad de carga total dentro de un material dieléctrico se puede modelar como:
ρ = ρb + ρf

(37)

Donde = ρf ” y = ρb ” es la densidad de carga libre y ligada, respectivamente. Además, se tiene que:

σP (x) = p(x) · n̂(x)

(38)
r=a

⃗ · p(x)
ρP (x) = −∇

(39)

Donde = σP ” y = ρP ” son las densidades de carga de polarización
superficial y volumétrica, respectivamente. Se recuerda que = n̂”
es el vector normal a la superficie en cuestión, en este caso = a” .

Ahora, se puede definir el desplazamiento eléctrico como:
D(x) = ε0 E(x) + p(x)
De esta manera, la Ley de Gauss generalizada se puede enunciar como:

I
D · ds = Qf → ∇ · D = ρf
S

(40)

---

### Página 13

Donde = Qf ” es la carga libre total del cuerpo que está encerrada por la superficie gaussiana.

Sumado a lo anterior, y al atravesar una interfaz entre dos medios dieléctricos, los campos
deben satisfacer que:
E1t = E2t

(41)
r=a

D2n − D1n = σf

(42)
r=a

Donde = t” y = n” son las componentes tangencial y normal, respectivamente.
Se debe considerar que los subíndices = 1” y = 2” hacen referencia a lo que se
encuentra dentro y fuera con respecto a la superficie en cuestión, en este caso = a”.
De lo anterior, se deduce que = Et ” debe ser continua, mientras que = Dn ” discontinua.

7.3

Dieléctricos - Cómo Utilizarlo Correctamente I

Generalmente, se querrá determinar el vector polarización y, con ello, las densidades de carga
de polarización superficial y volumétrica. Los pasos a seguir son:
a) = D = ε0 E+p ”: el vector polarización se puede calcular fácilmente a partir de la relación
con el campo y desplazamiento eléctrico. De esta manera:
1. Si es que el dieléctrico es lineal, es posible despejar el vector polarización fácilmente:
p = D − ε0 E = εE − ε0 E = (ε − ε0 )E

(43)

De ahora en adelante, se podrá utilizar esta fórmula libremente.

2. Solo quedaría reemplazar por el = ε” y = E” respectivos, los cuales dependerán únicamente
del lugar en donde se requiera calcular. Se hace énfasis en que = E” será el campo
en donde se localice el dieléctrico y, además, se desprende que el vector polarización
poseerá la misma componente que el campo eléctrico.
b) = σP (x) = p(x) · n̂(x) r=a ”: en esta parte se deberá calcular la densidad de carga de
polarización superficial en una superficie arbitraria = a”. Para ello:
1. Se debe distinguir el lugar en donde se requiere calcular la densidad superficial.
2. Luego, se debe identificar el campo eléctrico próximo a tal superficie y el cual
contiene al dieléctrico. Se calcula el vector polarización y simplemente se reemplaza.
3. ¿Cómo se determina el vector normal? Este será un vector ortogonal a la superficie
en cuestión y apuntará hacia afuera del dieléctrico.
4. Por último, se reemplaza todo en la expresión y se evalúa en el = punto” en donde se
ubica la superficie. Recuerden también que el producto punto de dos coordenadas
idénticas es igual a 1.
⃗ · p(x) ”: en esta parte se deberá calcular la densidad de carga de polarc) = ρP (x) = −∇
ización volumétrica en el lugar en donde se encuentra el dieléctrico. Para ello:
1. Se debe distinguir el lugar en donde se requiere calcular la densidad volumétrica.
2. Luego, se debe identificar el campo eléctrico que existe en esa zona y el cual contiene
al dieléctrico.
3. Se calcula el vector polarización, se reemplaza y se aplica la divergencia. En este
punto tengan cuidado, pues la divergencia dependerá de las coordenadas que se
estén utilizando.

---

### Página 14

7.4

Dieléctricos - Cómo Utilizarlo Correctamente II

En muy pocos ejercicios se tendrá que calcular la densidad de carga libre superficial, pero no
por ello es menos importante. Los pasos a seguir son:
1. Se debe identificar en que lugar se requiere calcular la densidad superficial, para luego
utilizar la siguiente expresión:
D2n − D1n = σf
r=a

2. Luego, se debe identificar y calcular los desplazamientos eléctricos normales colindantes a
la superficie arbitraria = a” en cuestión. Generalmente, la componente del desplazamiento
será completamente normal (i.e radial en una esfera y/o cilindro), por lo que no se tienen
que complicar de más.
3. Finalmente, se reemplaza en la fórmula y se evalúa en el = punto” en donde se ubica la
superficie.
4. Si es que se cumplen las condiciones necesarias y les resulta más sencillo, podrían usar
que = D = εE ”. No obstante, deben tener en cuenta que hay que cambiar σf por σ, que
es la densidad de carga superficial total:
ε2 E2n − ε1 E1n = σ
r=a

7.5

Dieléctricos - Cómo Utilizarlo Correctamente III

Para la mayoría de los problemas (sino todos) será necesario determinar el campo eléctrico junto
con el desplazamiento eléctrico. El método se realizará mediante la Ley de Gauss Generalizada
y, al igual que con la Ley de Gauss Común, solo se podrá utilizar cuando el problema presente
simetría plana, cilíndrica o esférica. Así, la aplicación consta de 3 partes:
H
a) = S D · ds ”: en esta se calculará el flujo que aporta el desplazamiento eléctrico al pasar
por la superficie gaussiana. De esta manera:
1. Se deberá elegir la superficie gaussiana según la simetría del cuerpo.
2. Calcular el flujo eléctrico, considerando que solo la componente perpendicular a la
superficie gaussiana contribuye a su valor.
3. Generalmente, este cálculo resultará en el producto entre el área de la superficie
gaussiana = importante” y la componente ortogonal del desplazamiento. Todos los
aspectos revelantes se resumen en la tabla del Anexo 8.6.
4. En caso de que en la misma sección transversal hayan 2 o más permitividades
distintas y/o un corte, se tendrán que utilizar las siguientes condiciones de borde
en la superficie = a”:
E1t = E2t
r=a

D2n − D1n = σf
r=a

b) = Qf ”: en esta parte se deberá calcular la carga libre del cuerpo que está encerrada por
la superficie gaussiana.

---

### Página 15

1. Por practicidad, se considerará a la carga libre como aquella carga que se ve en la
figura y/o explicitan por enunciado. En algunos problemas también podrían decir
que simplemente no existe carga libre, lo que facilita aún más los cálculos.
2. Luego, se deberá despejar el desplazamiento eléctrico de la igualdad.
3. En caso de requerir la forma vectorial del desplazamiento, se añade el componente
vectorial que aporta al flujo, el cual será siempre hacia fuera del cuerpo (vector
normal = n̂”).
c) = D = εE ”: finalmente, se calcula el campo eléctrico.
1. En la mayoría de los ejercicios (sino todos) el dieléctrico será lineal, por lo que
simplemente quedaría despejar E de la fórmula.
2. Notar que el sentido o componente vectorial del campo será idéntico al del desplazamiento.
3. También, = ε” será la permitividad del medio en el que se encuentra. En caso de
haber vacío, se reemplaza = ε” por = ε0 ”, quedando así la Ley de Gauss Común.
d) Algunos detalles a considerar son:
1. Todo este procedimiento se debe realizar para cada intervalo existente, los cuales
se pueden reconocer fácilmente mediante los = cortes” visuales del cuerpo. Tengan
cuidado al cambiar de intervalo, pues es probable que cambie el medio y, con ello,
la permitividad = ε”.
2. El cálculo de diferencia de potencial en dieléctricos no sufre ningún cambio. Se
calcula tranquilamente el campo mediante Gauss Generalizado y se reemplaza en la
integral de línea.
3. La Ley de Gauss Generalizada es para ”ajustar” las distintas permitividades que
pueden existir aparte del vacío. Por ello, y en caso de encontrarse en presencia
de vacío, podría usarse perfectamente la Ley de Gauss Común. No obstante, se
recomienda utilizar de ahora en adelante solo Ley de Gauss Generalizada.

---

### Página 16

Anexos

8.1

Series de Taylor

Decimos que una función = f (x)” puede expandirse como una serie de potencias en torno a = a”:
f (x) =

∞
X

cn (x − a)n

para todo |x − a| < R con R > 0

n=0

Ahora, y si la función = f (x)” puede derivarse infinitamente alrededor de = a”, podemos expresarla como una serie de Taylor:
T (x) =

∞
X
f (n) (a)

n!

n=0

(x − a)n = f (a) +

f ′ (a)
f ′′ (a)
f (3) (a)
(x − a) +
(x − a)2 +
(x − a)3 + . . .
1!
2!
3!

Más aún, y si a = 0, esta serie pasa a llamarse la serie de McLaurin de la función = f (x)”:

M (x) =

∞
X
f (n) (0)

n!

n=0

xn = f (0) +

f ′ (0)
f ′′ (0) 2 f (3) (0) 3
x+
x +
x + ...
1!
2!
3!

Ejemplo: Series más Utilizadas
Algunas de las series más comunes se muestran a continuación:
∞

X
=
xn = 1 + x + x2 + x3 + . . . ,
1−x

R=1

n=0

sin x =

∞
X

(−1)n

n=0
∞
X

cos x =

x2n+1
x3 x5 x7
=x−
+
−
+ ...,
(2n + 1)!
3!
5!
7!

(−1)n

n=0
k

(1 + x) =

∞  
X
k
n=0

n

x2n
x2 x4 x6
=1−
+
−
+ ...,
(2n)!
2!
4!
6!

xn = 1 + kx +

R=∞

R=∞

k(k − 1) 2 k(k − 1)(k − 2) 3
x +
x + ...,
2!
3!

R=1

Ejemplo: Aproximación por Grados
Sería muy poco conveniente usar toda la expresión asociada a la serie de potencia, por
lo que se acostumbra utilizarlas hasta cierto = grado”, el cual será igual al exponente más
alto que acompañe a cualquiera de las = x”. Por ejemplo, podríamos querer aproximar
la expansión de = ex ” a primer orden (aún así, se incluyen todos los términos de orden
inferior a este), tal como se muestra a continuación:
x

e =

∞
X
xn
n=0

n!

=1+

x
x2 x3
x
+
+
+ ··· ≈ 1 +
1!
2!
3!
1!

Si es que aún te cuesta, puedes seguir consultando estos conceptos en Series de Taylor y de McLaurin.

---

### Página 17

8.2

Transformación de Unidades

En general, y para evitar confusiones a la hora de realizar un ejercicio, se tendrá que trabajar
con unidades de medida que pertenezcan a un mismo sistema. Para ello, será importante
conocer sobre prefijos dimensionales y desarrollar una correcta transformación de unidades.
Sin ánimos de presentar más contenidos de los que ya se han visto, se tomará como ejemplo una transformación que se utiliza bastante en el ámbito de la mecánica.
Ejemplo: Transformación de km/h a m/s
m
Nos podrían dar por enunciado una rapidez v = 72 km
h que queremos expresar en s por
temas de simplicidad. Primero, debemos pensar cuáles son las equivalencias y relaciones
que guardan estas unidades de medida:

1 km = 1000 m
1 h = 60 min = 3600 s
Luego, podemos multiplicar estratégicamente estas igualdades con lo pedido,
de manera de = simplificar” las unidades de medida originales y expresarlas
en función de lo que deseamos, tal como se muestra a continuación:

v = 72

km
h

h
1000 m
1h
= 72 · (1 km ·
)·(
·
)
1 km
1 h 3600 s
1000 m
= 72 ·
3600 s
m
= 20
s
= 72 · 1 km ·

Ejemplo: Transformación de Unidades Elevadas
También está el caso de las unidades elevadas, como m2 o m3 . Supongamos que queremos
expresar una distancia d = 10 cm2 en m2 . Primero, debemos pensar cuáles son las
equivalencias y relaciones que guardan estas unidades de medida:
1 m = 100 cm
Luego, podemos multiplicar estratégicamente estas igualdades con lo pedido, de manera de
“simplificar” las unidades de medida originales y expresarlas en función de lo que deseamos.
Se debe tener cuidado con el elevado, pero el método es el mismo:

d = 10 cm2
= 10 · 1 cm · 1 cm
1m
1m
) · (1 cm ·
)
= 10 · (1 cm ·
100 cm
100 cm
= 10−3 m2

---

### Página 18

8.3

Prefijos del Sistema Internacional

Los prefijos se anteponen a una unidad de medida para indicar múltiplos o submúltiplos de la
misma. Algunos de los prefijos más comunes se pueden observar en la siguiente tabla:

8.4

Factor

Prefijo

Símbolo

giga

G

mega

M

kilo

k

10−2

centi

c

10−3

mili

m

10−6

micro

µ

10−9

nano

n

Ecuación de la Recta

Podría ser de ayuda conocer la expresión de la ecuación de la recta, en especial para interpolar
datos de las tablas termodinámicas o interrelacionar dos variables:
y − y1 =

y2 − y 1
(x − x1 )
x2 − x 1

(44)

Donde (xi , yi ) son las coordenadas del punto Pi . Se debe recordar que x e y
son las variables dependiente e independiente y que se mantienen como incógnitas,
puesto que se reemplazan con los valores que uno quiere determinar.
Además, la pendiente de una gráfica se puede expresar como:

m=

y2 − y 1
x2 − x 1

(45)

---

### Página 19

r = xx̂ + yŷ + zẑ

Forma
Vectorial

dV = dx dy dz

Diferencial
Volumen

Se debe notar que pueden haber distintas notaciones para el vector unitario (î = x̂, ĵ = ŷ, k̂ = ẑ)
y que la diferencial de volumen también se puede obtener mediante el cálculo de la matriz jacobiana.
Finalmente, en las coordenadas esféricas se considera al ángulo = θ” como el que barre verticalmente
desde arriba (0 < θ < π), mientras que al ángulo = ϕ” como el que barre el = suelo” (0 < ϕ < 2π).

dV = r2 sin θ dr dθ dϕ

dSr=cte = r2 sin θ dθ dϕ r̂
dSθ=cte = r sin θ dr dϕ θ̂
dSϕ=cte = r dr dθ ϕ̂
dSρ=cte = ρ dθ dz ρ̂
dSθ=cte = dρ dz θ̂
dSz=cte = ρ dρ dθ ẑ

dSx=cte = dy dz x̂
dSy=cte = dx dz ŷ
dSz=cte = dx dy ẑ

Diferencial
Superficie

dV = ρ dρ dθ dz

dr = drr̂ + r dθθ̂ + r sin θ dϕϕ̂

dr = dρρ̂ + ρ dθθ̂ + dzẑ

r̂ = sin θ cos ϕ x̂+sin θ sin ϕ ŷ+cos θ ẑ

ρ̂ = cos θ x̂ + sin θ ŷ
θ̂ = − sin θ x̂ + cos θ ŷ

dr = dxx̂ + dyŷ + dzẑ

r = rr̂

C. Esféricas

r = ρρ̂ + zẑ

C. Cilíndricas

Coordenadas y Diferenciales

Diferencial
Línea

Componente

C. Cartesianas

Conceptos

8.5

---

### Página 20

Cilindro Ortogonal

Perpendicular (ẑ)

Superficie
Gaussiana

Componente
Ortogonal

Resultado
Integral
S.G.I

Integral
S.G.I

S = πR2

S = 2πrL

0 r dz dθ

R 2π R L

Manto Cilindro

Radial (ρ̂)

Cilindro Coaxial

Alambres - Cilindros Infinitos

Simetría Cilíndrica

Aplicación Ley de Gauss

2 sin θ dθ dϕ

S = 4πr2

0 r

R 2π R π

Superficie Esfera

Radial (r̂)

Esfera Concéntrica

Esferas

Simetría Esférica

En algunos casos será necesario integrar, por lo que no se recomienda solo saber los resultados.
Para armar las integrales puede ser de utilidad conocer las relaciones de los diferenciales del Anexo 8.5.
R 2π R π R R
Podría ser conveniente tener en mente que Vesfera, R = 0 0 0 r2 sin θ dr dθ dϕ = 34 πR3

0 r dr dθ

R 2π R R

Bases Cilindro

Planos - Bloques Infinitos

Ejemplos
Cuerpos

Superficie
Gaussiana
Importante

Simetría Plana

Conceptos

8.6

---

### Página 21

δFẑ
ŷ
x̂
∇ · F = δF
δx + δy + δz

Divergencia

δF

Fx̂ Fŷ Fẑ

∇×F=

Rotacional

δF

Fρ̂ ρFθ̂ Fẑ

δ
δz

ẑ

δ
ẑ
∇ · F = ρ1 δρ
(ρFρ̂ ) + ρ1 δθθ̂ + δF
δz

∇×F=

δ
δθ

ρθ̂

δ
δz

δ
δρ

ρ̂

ẑ

δ
δy

ŷ

δ
δx

x̂

δ f
1 δ f
∇2 f = δδρf2 + ρ1 δf
δρ + ρ2 δθ2 + δz 2

∇2 f = δδxf2 + δδyf2 + δδzf2

δf
1 δf
∇f = δf
δρ ρ̂ + ρ δθ θ̂ + δz ẑ

δf
δf
∇f = δf
δx x̂ + δy ŷ + δz ẑ

Gradiente

Laplaciano

C. Cilíndricas

C. Cartesianas

Coordenadas y Operador ∇

Conceptos

8.7

δ
δϕ

δ
δθ
δ
δr

Fr̂ rFθ̂ r sin θFϕ̂

r sin θϕ̂

rθ̂

r̂

δ
1 δFϕ̂
r sin θ δθ (sin θFθ̂ ) + r sin θ δϕ

δ
∇ · F = r12 δr
(r2 Fr̂ )+

r2 sin θ

δ
(r2 δf
∇2 f = r12 δr
δr )+
δf
δ2 f
δ
(sin θ δθ ) + r2 sin
2 θ δϕ2
r2 sin θ δθ

1 δf
1 δf
∇f = δf
δr r̂ + r δθ θ̂ + r sin θ δϕ ϕ̂

C. Esféricas
