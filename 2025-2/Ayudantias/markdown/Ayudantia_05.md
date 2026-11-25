---
title: "Ayudantia 05"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_05_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_05_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 05

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 5
26 de Agosto 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Potencial Electrostático

1.1

Potencial Electrostático - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Determinar el potencial eléctrico generado por una distribución discreta de carga medi□
ante su definición.
□ Determinar el potencial eléctrico generado por una distribución continua de carga mediante su definición en coordenadas cartesianas.

✓ Determinar el potencial eléctrico generado por una distribución continua de carga medi□
ante su definición en coordenadas cilíndricas.
□ Determinar el potencial eléctrico generado por una distribución continua de carga mediante su definición en coordenadas esféricas.
□ Determinar el potencial eléctrico generado por un cuerpo que cumple las condiciones de
simetría de Ley de Gauss mediante la integral de línea.

✓ Aplicar el principio de superposición para potenciales eléctricos en un sistema compuesto
□
por dos o más cuerpos.
□ Evaluar el potencial eléctrico en un punto del espacio.
□ Graficar la magnitud del potencial eléctrico en función del radio para alambres, cilindros
y esferas.

✓ Conocer la unidad de medida para el potencial eléctrico.
□
□ Aplicar la segunda ecuación de Maxwell y la ecuación de Poisson en diversos contextos.

---

### Página 2

1.2

Potencial Electrostático - Distribución Discreta de Carga

El potencial eléctrico generado por una carga puntual = q” puede ser expresado como:
1 q
4πε0 r

V (r) =

(1)

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

(2)

j=1

1.3

Potencial Electrostático - Distribución Continua de Carga

Para una distribución continua de carga, el potencial eléctrico está dado por:
dq(x ′ )
V (x) =
4πε0
|x − x ′ |

(3)

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

1.4

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
Sección ?? y ??.

1.5

Potencial Electrostático - Otras Expresiones

Gracias al teorema de Stokes, se puede obtener la segunda ecuación de Maxwell:
I
E · d⃗l = 0 → ∇ × E = 0

(4)

Ahora, y como la integral de línea es independiente del camino de integración, el potencial
eléctrico se puede escribir como:
Z rb
E = −∇V → V (rb ) − V (ra ) = −
E · d⃗l
(5)
ra

---

### Página 3

Esta última expresión es más fácil de resolver que la dada por definición, por lo que hay
que tenerla siempre en mente a la hora de enfrentar un ejercicio. En caso de presentarse
más de un valor de campo eléctrico, se deberá separar la integral en varias partes y con
sus respectivos límites. Asimismo, el = Volt” es la unidad de medida para el potencial:

J
(6)
C
Finalmente, y mediante la primera ecuación de Maxwell y la relación de potencial, se puede
obtener la ecuación de Poisson:
ρ
∇2 V = −
(7)
ε0
1V=1

En ausencia de cargas, esta expresión se transforma en la ecuación de Laplace:

∇2 V = 0

1.6

(8)

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

Se debe considerar que el usar V (∞) es algo nada más estratégico, pues
generalmente este poseerá un valor nulo. La idea es que el segundo término sea algo
fácil de manipular, por lo que conviene que sea una constante o 0. Además, se deberá
separar la integral si es que observamos distintos campos en los intervalos respectivos.

5. Por último, si un cuerpo se conecta a = tierra” su potencial será nulo. Asimismo, el que
dos cuerpos estén unidos mediante un cable significará que su potencial será idéntico y
que se repartirán las cargas entre ellos según el principio de conservación de carga.

---

### Página 4

1.6.1

“Problemas Resueltos de Electromagnetismo”, 2.4, Rodrigo Chi

Una densidad de carga lineal λ está repartida de forma homogénea a lo largo de un
semicircunferencia BD centrada en C y de radio R. Una carga puntual q está ubicada
−→
en punto A como se indica en la Figura (|CA| = R).
a) Calcule el potencial eléctrico en el punto C.
b) Por argumentos de simetría, determine la dirección del campo eléctrico en el punto
C.
c) Calcule el campo eléctrico en el punto C.
d) Determine la relación entre λ y q tal que el campo eléctrico en el punto C sea igual
a 0.

Figura 1. Esquema sobre la carga lineal y la semicircunferencia.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el potencial eléctrico en el punto C, el cual puede ser expresado como la
suma de los potenciales generados por la carga puntual y la semicircunferencia. Como las
figuras no poseen ninguna simetría apta para la Ley de Gauss, se aplicará la definición de
potencial eléctrico para distribuciones discretas y continuas de carga:
1 q
V (r) =
4πε0 r
V (x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Se nota que se usa la integral simple en virtud de la naturaleza del problema, puesto que la
semicircunferencia se puede describir con solo una componente variable en coordenadas cilíndricas.

---

### Página 5

Solución b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en el punto C, el cual puede ser expresado como la suma
de los campos generados por la carga puntual y la semicircunferencia. Como la figura no posee
ninguna simetría apta para la Ley de Gauss, se aplicará la definición de campo eléctrico para
distribuciones discretas y continuas de carga:
1 q
E(r) =
r̂
4πε0 r2
(x − x ′ )
E(x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |3
Se nota que se usa la integral simple en virtud de la naturaleza del problema, puesto que la
semicircunferencia se puede describir con solo una componente variable en coordenadas cilíndricas.

Solución d)
Paso Único: Condición y Relación
Por último, se impone la condición propuesta para que el campo eléctrico en el punto C sea
cero:
E(C) = 0

---

### Página 6

Trabajo y Energía en Electrostática

2.1

Trabajo y Energía en Electrostática - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Determinar el trabajo necesario para mover una carga en presencia de un campo eléctrico.
□
□ Determinar la energía potencial almacenada por una distribución discreta de carga.

✓ Determinar la energía potencial almacenada por una distribución continua de carga.
□
✓ Aplicar el principio de conservación de energía según el contexto.
□
2.2

Trabajo y Energía en Electrostática - Generalidades

En primer lugar, el trabajo necesario para mover una carga = q” desde el punto = x1 ” hasta el
punto = x2 ” en contra de un campo eléctrico = E(x)” estará dado por:
Z x2
W =−
qE(x) · dx = q(V2 − V1 )
(9)
x1

Suponiendo que el potencial en el infinito es cero, el trabajo necesario
para traer una carga desde el infinito hasta un punto = x” es entonces:

W = qV (x)
(10)
De esta manera, la energía potencial almacenada en un sistema compuesto por = N ” cargas
puntuales se puede escribir como:
N

N

i=1

i=1 j>i

1X
1 X X qi qj
U=
qi V (xi ) =
4πε0
rij
Donde = V (xi )” es el potencial en la posición de la carga = i” debido a las demás cargas.
Análogamente, para una distribución continua de carga se tiene que:

(11)

---

### Página 7

2.2.1

“Ejercicios Teoría Electromagnética ”, 5.6.9, Fabián Cádiz

Un alambre cuya densidad lineal de carga es λ se extiende en el eje z desde z = −d
hasta z = d. Despreciando efectos gravitacionales:
a) Calcule el potencial en un punto z > d sobre el eje del alambre.
b) ¿Cuál es el cambio de energía potencial de un electrón si se mueve de z = 4d hasta
z = 3d?
c) Si el electrón parte del reposo desde z = 4d, ¿cuál es la velocidad en z = 3d?

Figura 2. Esquema sobre el alambre.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el potencial eléctrico en un punto z > d sobre el eje del alambre. Como
la figura no posen ninguna simetría apta para la Ley de Gauss, se aplicará la definición de
potencial eléctrico para distribuciones continuas de carga:
V (x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Se nota que se usa la integral simple en virtud de la naturaleza del problema, puesto que el
alambre se puede describir con solo una componente variable en coordenadas cartesianas.

---

### Página 8

Solución b)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el cambio de energía potencial ∆U de un electrón que se mueve desde
z = 4d hasta z = 3d. La energía potencial que posee una carga puntual se puede escribir como:
U = qV (x)
Se conoce el potencial que afecta a la carga,
por lo que solo queda reemplazar por los valores requeridos.

Solución c)
Paso Único: Velocidad Electrón - v(z = 3d)
Se pide determinar la velocidad del electrón en z = 3d si parte del reposo en z = 4d. Mediante
el principio de conservación de energía se tiene que:
E(z = 3d) = E( z = 4d)
2.2.2

“Problemas de Electromagnetismo”, 1.4.5, Sebastián Urrutia

Una esfera de radio R posee una densidad de carga radial ρ(r) = kr, con k una constante.
Encuentra la energía potencial de esta configuración.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la energía potencial almacenada de una distribución continua de carga:
ε0
U=
|E|2 dτ
2 R3
Como se está hablando de una esfera, es posible aplicar Ley de Gauss utilizando una esfera
concéntrica de radio = r” arbitrario:
I
Qenc
E · d⃗s =
ϵ0
S
La densidad de carga de la esfera no es uniforme,
por lo que se tendrá que utilizar la definición de carga:

ZZZ
Q=

ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: r < R, y r > R.

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 5
26 de Agosto 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Potencial Electrostático

1.1

Potencial Electrostático - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Determinar el potencial eléctrico generado por una distribución discreta de carga medi□
ante su definición.
□ Determinar el potencial eléctrico generado por una distribución continua de carga mediante su definición en coordenadas cartesianas.

✓ Determinar el potencial eléctrico generado por una distribución continua de carga medi□
ante su definición en coordenadas cilíndricas.
□ Determinar el potencial eléctrico generado por una distribución continua de carga mediante su definición en coordenadas esféricas.
□ Determinar el potencial eléctrico generado por un cuerpo que cumple las condiciones de
simetría de Ley de Gauss mediante la integral de línea.

✓ Aplicar el principio de superposición para potenciales eléctricos en un sistema compuesto
□
por dos o más cuerpos.
□ Evaluar el potencial eléctrico en un punto del espacio.
□ Graficar la magnitud del potencial eléctrico en función del radio para alambres, cilindros
y esferas.

✓ Conocer la unidad de medida para el potencial eléctrico.
□
□ Aplicar la segunda ecuación de Maxwell y la ecuación de Poisson en diversos contextos.

---

### Página 2

1.2

Potencial Electrostático - Distribución Discreta de Carga

El potencial eléctrico generado por una carga puntual = q” puede ser expresado como:
1 q
4πε0 r

V (r) =

(1)

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

(2)

j=1

1.3

Potencial Electrostático - Distribución Continua de Carga

Para una distribución continua de carga, el potencial eléctrico está dado por:
dq(x ′ )
V (x) =
4πε0
|x − x ′ |

(3)

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

1.4

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
Sección ?? y ??.

1.5

Potencial Electrostático - Otras Expresiones

Gracias al teorema de Stokes, se puede obtener la segunda ecuación de Maxwell:
I
E · d⃗l = 0 → ∇ × E = 0

(4)

Ahora, y como la integral de línea es independiente del camino de integración, el potencial
eléctrico se puede escribir como:
Z rb
E = −∇V → V (rb ) − V (ra ) = −
E · d⃗l
(5)
ra

---

### Página 3

Esta última expresión es más fácil de resolver que la dada por definición, por lo que hay
que tenerla siempre en mente a la hora de enfrentar un ejercicio. En caso de presentarse
más de un valor de campo eléctrico, se deberá separar la integral en varias partes y con
sus respectivos límites. Asimismo, el = Volt” es la unidad de medida para el potencial:

J
(6)
C
Finalmente, y mediante la primera ecuación de Maxwell y la relación de potencial, se puede
obtener la ecuación de Poisson:
ρ
∇2 V = −
(7)
ε0
1V=1

En ausencia de cargas, esta expresión se transforma en la ecuación de Laplace:

∇2 V = 0

1.6

(8)

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

Se debe considerar que el usar V (∞) es algo nada más estratégico, pues
generalmente este poseerá un valor nulo. La idea es que el segundo término sea algo
fácil de manipular, por lo que conviene que sea una constante o 0. Además, se deberá
separar la integral si es que observamos distintos campos en los intervalos respectivos.

5. Por último, si un cuerpo se conecta a = tierra” su potencial será nulo. Asimismo, el que
dos cuerpos estén unidos mediante un cable significará que su potencial será idéntico y
que se repartirán las cargas entre ellos según el principio de conservación de carga.

---

### Página 4

1.6.1

“Problemas Resueltos de Electromagnetismo”, 2.4, Rodrigo Chi

Una densidad de carga lineal λ está repartida de forma homogénea a lo largo de un
semicircunferencia BD centrada en C y de radio R. Una carga puntual q está ubicada
−→
en punto A como se indica en la Figura (|CA| = R).
a) Calcule el potencial eléctrico en el punto C.
b) Por argumentos de simetría, determine la dirección del campo eléctrico en el punto
C.
c) Calcule el campo eléctrico en el punto C.
d) Determine la relación entre λ y q tal que el campo eléctrico en el punto C sea igual
a 0.

Figura 1. Esquema sobre la carga lineal y la semicircunferencia.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el potencial eléctrico en el punto C, el cual puede ser expresado como la
suma de los potenciales generados por la carga puntual y la semicircunferencia. Como las
figuras no poseen ninguna simetría apta para la Ley de Gauss, se aplicará la definición de
potencial eléctrico para distribuciones discretas y continuas de carga:
1 q
V (r) =
4πε0 r
V (x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Se nota que se usa la integral simple en virtud de la naturaleza del problema, puesto que la
semicircunferencia se puede describir con solo una componente variable en coordenadas cilíndricas.

---

### Página 5

Paso 1: Potencial Eléctrico - Carga Puntual
El potencial eléctrico de una carga puntual se puede escribir como:
V (r) =

1 q
4πε0 r

Como la distancia de la carga q al punto C es R:

Vc =

1 q
4πε0 R

(9)

Paso 2: Potencial Eléctrico Semicircunferencia - Componentes Integral
Desde ahora en adelante, nuestro sistema de referencia será el punto C y se utilizarán coordenadas cilíndricas por la geometría del ejercicio. Se recuerda que el vector r inicia en el origen
y se extiende hasta el punto en donde se quiere calcular el potencial:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con carga:
r ′ = Rr̂,

θ ∈ [0, π[

Donde = R” es el radio de la semicircunferencia
y = r̂” la componente radial en coordenadas cilíndricas.

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = −Rr̂
Luego, el módulo del vector anterior será:

|r − r ′ | = R
Considerando que la densidad de carga es lineal y que la única componente variable para la
semicircunferencia es θ:
dq(x ′ ) = λ(x ′ ) dl′ = λ · R dθ
Para llegar a lo anterior se utilizó el diferencial de línea para cilíndricas,
omitiendo las componentes constantes y el sentido vectorial.

Paso 3: Potencial Eléctrico - Semicircunferencia
Finalmente, se utiliza la definición de potencial eléctrico para la semicircunferencia considerando
los límites de integración propuestos con anterioridad:
Vs =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Z π
=
λ · R dθ
4πε0 0 R
Z π
λ
(10)
=
dθ
4πε0 0
λ
=
·π
4πε0
λ
=
4ε0

---

### Página 6

Paso 4: Principio de Superposición - V
Finalmente, y mediante el principio de superposición, el potencial eléctrico en el punto C será
la suma de los potenciales eléctricos generados por la carga puntual y la semicircunferencia:
V (C) = Vc + Vs
1 q
λ
=
+
4πε0 R 4ε0

(11)

Solución b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en el punto C, el cual puede ser expresado como la suma
de los campos generados por la carga puntual y la semicircunferencia. Como la figura no posee
ninguna simetría apta para la Ley de Gauss, se aplicará la definición de campo eléctrico para
distribuciones discretas y continuas de carga:
1 q
E(r) =
r̂
4πε0 r2
(x − x ′ )
E(x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |3
Se nota que se usa la integral simple en virtud de la naturaleza del problema, puesto que la
semicircunferencia se puede describir con solo una componente variable en coordenadas cilíndricas.

Paso 1: Campo Carga - Ec
El campo eléctrico de una carga puntual se puede escribir como:
E(r) =

1 q
r̂
4πε0 r2

Se recuerda que el vector r se extiende hasta el punto en donde se quiere calcular el campo,
respetando el sentido de las líneas de campo asociadas a la carga. Como las líneas de campo eléctrico
se originan en cargas positivas y la distancia de la carga q al punto C es R (i.e r = Rŷ), se tiene que:

Ec =

1 q
ŷ
4πε0 R2

(12)

Paso 2: Campo Eléctrico Semicircunferencia - Componentes Integral
Desde ahora en adelante, nuestro sistema de referencia será el punto C y se utilizarán coordenadas cilíndricas por la geometría del ejercicio. Se recuerda que el vector r inicia en el origen
y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con carga:
r ′ = Rr̂,

θ ∈ [0, π[

Donde = R” es el radio de la semicircunferencia
y = r̂” la componente radial en coordenadas cilíndricas.

---

### Página 7

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = −Rr̂
Calculando el módulo del vector anterior:

|r − r ′ | = R
Considerando que la densidad de carga es lineal y que la única componente variable para la
semicircunferencia es θ:
dq(x ′ ) = λ(x ′ ) dl′ = λ · R dθ
Para llegar a lo anterior se utilizó el diferencial de línea para cilíndricas,
omitiendo las componentes constantes y el sentido vectorial.

Paso 3: Campo Eléctrico - Semicircunferencia
Finalmente, se utiliza la definición de campo eléctrico para la semicircunferencia considerando
los límites de integración propuestos con anterioridad:
(x − x ′ )
Es =
λ(x ′ ) dl′
4πε0 L |x − x ′ |3
Z π
−Rr̂
=
λ · R dθ
4πε0 0 R3
Z π
−λr̂
=
dθ
4πε0 0 R
Z π
−λ
=
r̂ dθ
4πε0 R 0
Utilizando que r̂ = cos θ x̂ + sin θ ŷ:

Z π
−λ
Es =
cos θ x̂ + sin θ ŷ dθ
4πε0 R 0
Z π
Z π
−λ
=
·(
cos θ x̂ dθ +
sin θ ŷ dθ)
4πε0 R
π
π
−λ
=
· ( (sin θ x̂) + (− cos θ ŷ) )
4πε0 R
−λ
=
· ((sin π − sin 0) x̂ − (cos π − cos 0) ŷ)
4πε0 R
−λ
=
· 2 ŷ
4πε0 R
−λ
=
ŷ
2πε0 R

(13)

Nota: La integral asociada también puede simplificarse por temas de simetría de la
semicircunferencia, ya que se puede obviar la parte asociada a la componente x̂.

---

### Página 8

Paso 4: Principio de Superposición - E
Finalmente, y mediante el principio de superposición, el campo eléctrico en el punto C será la
suma de los campos eléctricos generados por la carga puntual y la semicircunferencia:
E(C) = Ec + Es
1 q
−λ
=
ŷ
ŷ +
4πε0 R
2πε0 R

(14)

Solución d)
Paso Único: Condición y Relación
Por último, se impone la condición propuesta para que el campo eléctrico en el punto C sea
cero:
E(C) = 0
1 q
−λ
ŷ +
ŷ = 0
4πε0 R
2πε0 R
Como la componente vectorial es única y equivalente
en la ecuación vectorial, se puede obviar en el análisis:

1 q
λ
=
4πε0 R
2πε0 R
q = 2λR

(15)

---

### Página 9

Trabajo y Energía en Electrostática

2.1

Trabajo y Energía en Electrostática - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Determinar el trabajo necesario para mover una carga en presencia de un campo eléctrico.
□
□ Determinar la energía potencial almacenada por una distribución discreta de carga.

✓ Determinar la energía potencial almacenada por una distribución continua de carga.
□
✓ Aplicar el principio de conservación de energía según el contexto.
□
2.2

Trabajo y Energía en Electrostática - Generalidades

En primer lugar, el trabajo necesario para mover una carga = q” desde el punto = x1 ” hasta el
punto = x2 ” en contra de un campo eléctrico = E(x)” estará dado por:
Z x2
W =−
qE(x) · dx = q(V2 − V1 )
(16)
x1

Suponiendo que el potencial en el infinito es cero, el trabajo necesario
para traer una carga desde el infinito hasta un punto = x” es entonces:

W = qV (x)
(17)
De esta manera, la energía potencial almacenada en un sistema compuesto por = N ” cargas
puntuales se puede escribir como:
N

N

i=1

i=1 j>i

1X
1 X X qi qj
U=
qi V (xi ) =
4πε0
rij
Donde = V (xi )” es el potencial en la posición de la carga = i” debido a las demás cargas.
Análogamente, para una distribución continua de carga se tiene que:

(18)

---

### Página 10

2.2.1

“Ejercicios Teoría Electromagnética ”, 5.6.9, Fabián Cádiz

Un alambre cuya densidad lineal de carga es λ se extiende en el eje z desde z = −d
hasta z = d. Despreciando efectos gravitacionales:
a) Calcule el potencial en un punto z > d sobre el eje del alambre.
b) ¿Cuál es el cambio de energía potencial de un electrón si se mueve de z = 4d hasta
z = 3d?
c) Si el electrón parte del reposo desde z = 4d, ¿cuál es la velocidad en z = 3d?

Figura 2. Esquema sobre el alambre.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el potencial eléctrico en un punto z > d sobre el eje del alambre. Como
la figura no posen ninguna simetría apta para la Ley de Gauss, se aplicará la definición de
potencial eléctrico para distribuciones continuas de carga:
V (x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Se nota que se usa la integral simple en virtud de la naturaleza del problema, puesto que el
alambre se puede describir con solo una componente variable en coordenadas cartesianas.

---

### Página 11

Paso 2: Potencial Eléctrico Alambre - Componentes Integral
Desde ahora en adelante, nuestro sistema de referencia será el centro del alambre y se utilizarán
coordenadas cartesianas por la geometría del ejercicio. Se recuerda que el vector r inicia en el
origen y se extiende hasta el punto en donde se quiere calcular el potencial:
r = zẑ,

z ∈ [d, ∞[

Luego, el vector r ′ inicia en el origen y recorre todo el cuerpo con carga:
r ′ = z ′ ẑ, z ′ ∈ [−d, d]
Se siguen determinando componentes de la integral:
r − r ′ = zẑ − z ′ ẑ
Calculando el módulo del vector anterior:

|r − r ′ | = z − z ′
Considerando que la densidad de carga es lineal y que la única componente variable para el
alambre es z:
dq = λ dz ′
Para llegar a lo anterior se utilizó el diferencial de línea para cartesianas,
omitiendo las componentes constantes y el sentido vectorial.

Paso 3: Potencial Eléctrico - Alambre
Finalmente, se utiliza la definición de potencial eléctrico para el alambre considerando los
límites de integración propuestos con anterioridad:
V =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Z d
=
· λ dz ′
4πε0 −d (z − z ′ )
Z z−d
λ
=
− dβ
4πε0 z+d
β
(19)
z+d
λ
=
(ln β)
4πε0
z−d
λ
=
(ln (z + d) − ln (z − d))
4πε0
λ
z+d
=
ln (
)
4πε0
z−d
Notar que se realizó un cambio de variable β = z − z ′ → dβ = −dz ′ .

---

### Página 12

Solución b)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el cambio de energía potencial ∆U de un electrón que se mueve desde
z = 4d hasta z = 3d. La energía potencial que posee una carga puntual se puede escribir como:
U = qV (x)
Se conoce el potencial que afecta a la carga,
por lo que solo queda reemplazar por los valores requeridos.

Paso 1: Cambio Energía Potencial - ∆U
El cambio en la energía potencial de un electrón (i.e q = −e) que se mueve desde z = 4d hasta
z = 3d vendrá dado por:
∆U = U (z = 3d) − U (z = 4d)
= qV (z = 3d) − qV (z = 4d)
3d + d
λ
4d + d
λ
ln (
)−
ln (
))
= −e(
4πε0
3d − d
4πε0
4d − d
−eλ
=
· (ln 2 − ln )
4πε0
−eλ
=
ln ( )
4πε0

(20)

Solución c)
Paso Único: Velocidad Electrón - v(z = 3d)
Se pide determinar la velocidad del electrón en z = 3d si parte del reposo en z = 4d. Mediante
el principio de conservación de energía se tiene que:
E(z = 3d) = E( z = 4d)
U (z = 3d) + K(z = 3d) = U (z = 4d) + K(z = 4d)
Donde U y K son la energía potencial y cinética del electrón, respectivamente.
Como este parte del reposo (i.e K(z = 4d) = 0):

U (z = 3d) + K(z = 3d) = U (z = 4d)
K(z = 3d) = U (z = 4d) − U (z = 3d)
K(z = 3d) = −∆U
Reescribiendo la energía cinética como K = 21 mv 2 :

me v 2 (z = 3d) = −∆U
v 2 (z = 3d) =
· −∆U
m
re
λe
v(z = 3d) =
ln ( )
2πε0 me

(21)

---

### Página 13

2.2.2

“Problemas de Electromagnetismo”, 1.4.5, Sebastián Urrutia

Una esfera de radio R posee una densidad de carga radial ρ(r) = kr, con k una constante.
Encuentra la energía potencial de esta configuración.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la energía potencial almacenada de una distribución continua de carga:
ε0
U=
|E|2 dτ
2 R3
Como se está hablando de una esfera, es posible aplicar Ley de Gauss utilizando una esfera
concéntrica de radio = r” arbitrario:
I
Qenc
E · d⃗s =
ϵ0
S
La densidad de carga de la esfera no es uniforme,
por lo que se tendrá que utilizar la definición de carga:

ZZZ
Q=

ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: r < R, y r > R.

Paso 1: Ley de Gauss - Er<R
En primer lugar, se calculará el campo eléctrico mediante la Ley de Gauss en la región r < R:
I
⃗ = Qenc
Er<R · dS
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada estará determinada por una integral triple en esféricas:

RRR

I
Er<R ·

V ρ dV

dS =

ε0

Como la densidad de carga de la esfera no es uniforme,
no se puede tratar como una constante y se debe integrar.
Ahora, la integral cerrada es en verdad la superficie de la esfera,
pues el flujo es ortogonal a esta en todo momento:

RRR

Er<R · 4πr =

V ρ dV

ε0

La integral de volumen se refiere al volumen encerrado
por la esfera gaussiana de altura = h” y radio = r”.
En este caso, sería parte del volumen de la esfera con carga:

---

### Página 14

R 2π R π R r
Er<R · 4πr2 =
Er<R · 4πr2 =

0 kr · r

2 sin θ drdθdϕ

ε0
2π · 2 · k r4

ε0

kr2
Er<R =
4ε0
Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

kr2
r̂
4ε0

Er<R =

(22)

Paso 2: Ley de Gauss - Er>R
Luego, se calculará el campo eléctrico mediante la Ley de Gauss en la región r > R:
I
⃗ = Qenc
Er>R · dS
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada estará determinada por una integral triple en esféricas:

RRR

I
Er<R ·

V ρ dV

dS =

ε0

Como la densidad de carga de la esfera no es uniforme,
no se puede tratar como una constante y se debe integrar.
Ahora, la integral cerrada es en verdad la superficie de la esfera,
pues el flujo es ortogonal a esta en todo momento:

RRR

V ρ dV

Er>R · 4πr =

ε0

La integral de volumen se refiere al volumen encerrado
por la esfera gaussiana de altura = h” y radio = r”.
En este caso, sería todo el volumen de la esfera con carga:

R 2π R π R R

Er>R · 4πr =

kr · r2 sin θ drdθdϕ
ε0

2π · 2 · k R4
Er>R · 4πr =
ε0
kR
Er>R =
4ε0 r2

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

Er>R =

kR4
r̂
4ε0 r2

(23)

---

### Página 15

Paso 3: Energía Potencial - U
La energía potencial almacenada en una distribución continua de carga está dada por:
ε0
|E|2 dτ
2 R3
Z 2π Z π Z R
Z 2π Z π Z ∞
ε0
= (
|Er<R | · r sin θ drdθdϕ +
|Er>R |2 · r2 sin θ drdθdϕ)
2 0
R
Z 2π Z π Z R
Z 2π Z π Z ∞
kr2 2 2
kR4
ε0
(
) · r sin θ drdθdϕ +
(
) · r2 sin θ drdθdϕ)
= (
2 0
4ε0
4ε0 r2
R
Z ∞ 2 8
Z R 2 6
k R
ε0
k r
dr +
=
· 2 · 2π · (
2 2 dr)
R 16ε0 r
0 16ε0

U=

R

∞

k2 r7
k 2 R8 −1
= 2πε0 · (
+
)
·
·
r R
16ε20 7 0
16ε20
k 2 R7 k 2 R8 1
+
·
· )
16ε20 7
16ε20 R
k 2 R7
k 2 R7
= 2πε0 · (
+
)
112ε20
16ε20
πk 2 R7
=
7ε0

= 2πε0 · (

(24)
