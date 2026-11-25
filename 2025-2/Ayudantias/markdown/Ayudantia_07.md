---
title: "Ayudantia 07"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_07_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_07_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 07

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Ayudantía 7
02 de Septiembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Conductores y Condensadores

1.1

Conductores - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Conocer las propiedades y efectos de medios conductores sobre el campo eléctrico.
□
✓ Determinar el campo eléctrico en configuraciones con medios conductores.
□
✓ Determinar el potencial eléctrico en configuraciones con medios conductores.
□
✓ Calcular la carga y densidad de carga superficial inducida en superficies de medios con□
ductores.
✓ Aplicar el principio de conservación de carga para cuerpos neutros y cargados.
□
1.2

Condensadores - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Conocer el concepto, funcionamiento y aplicaciones de un condensador.
□
✓ Determinar la capacitancia de diversas configuraciones en presencia de conductores.
□
✓ Determinar la fuerza generada entre medios conductores cargados.
□
✓ Calcular la energía almacenada en un capacitor según el contexto.
□
✓ Aplicar la expresión de capacitancia para placas paralelas en diversas configuraciones.
□
✓ Calcular el gradiente de una función para distintos sistemas de coordenadas.
□
✓ Comparar el valor de la capacitancia en presencia de medios conductores.
□
✓ Conocer la unidad de medida para la capacitancia.
□

---

### Página 2

1.3

Conductores - Generalidades

Los materiales conductores (tales como los metales) presentan ciertas propiedades que les son
inherentes por naturaleza. Así, los electrones se podrán mover libremente en su interior y
seguirán en movimiento mientras experimenten un campo eléctrico; sin embargo, estos se detendrán si no están provistos continuamente de una fuente de energía externa.
De esta manera:
a) El campo eléctrico dentro de un conductor es nulo.
b) Luego, por Ley de Gauss y el principio de conservación de carga, la carga en un conductor
necesariamente debe distribuirse equipotencialmente y solo en su superficie:
I
⃗ · d⃗s = 0 → Qenc = 0
(1)
S

Al mismo tiempo, esto significa que al interior
de un conductor el potencial eléctrico es constante:

⃗ =0
−∇V

(2)

c) La componente tangencial del campo eléctrico en la superficie de un conductor es cero,
por lo que solo sobrevivirá la componente normal a esta.

1.4

Conductores - Cómo Utilizarlo Correctamente

En variados ejercicios les pedirán determinar la carga superficial inducida en las superficies del
conductor. Los pasos a seguir son:
1. = Calcular” estratégicamente el campo en un lugar que contenga conductor y que esté
justo afuera de la superficie relacionada con la carga pedida. Por propiedades, este
campo debe ser nulo e implica necesariamente que la carga encerrada es 0:
I
⃗ · d⃗s = 0 → Qenc = 0
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

### Página 3

1.5

Condensadores - Generalidades

Un condensador es un dispositivo capaz de acumular carga eléctrica, que generalmente consiste
en dos conductores cargados con cargas opuestas de igual magnitud. De esta forma, la carga
almacenada en un condensador está dada por:
Q = C∆V

(3)

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

(4)

(5)

Resolviendo, y reemplazando por la expresión que
relaciona carga almacenada con capacitancia, se obtiene que:

U=

1 Q2
= CV 2 = QV
2 C

(6)

Asimismo, la fuerza entre conductores cargados se puede escribir como:

⃗ )
F⃗ = (∇U

⃗ )
= − (∇U
V =cte

(7)
Q=cte

Finalmente, podría ser de utilidad saber la capacitancia de un condensador de placas paralelas:
C=

εA
d

(8)

Donde = ε” es la constante de permitividad del medio que se encuentra
rellenando totalmente el espacio entre ambas placas, = A” el área = efectiva” de
las placas (proyección de una sobre la otra) y = d” la distancia entre las mismas.

1.6

Condensadores - Cómo Utilizarlo Correctamente

El fuerte en esta sección será determinar la capacitancia de cierta configuración:
1. ¿Dónde se ubican las cargas opuestas? Esto será fundamental, pues solo se deberá calcular
la diferencia de potencial entre estos límites de acuerdo a la siguiente fórmula:
Z a
⃗ a<r<b · d⃗l
∆V = V (a) − V (b) = −
b

Donde = a” y = b” indican la ubicación de la carga positiva y negativa.
De esta manera, se tendrá que calcular el campo eléctrico necesario para el potencial.

2. Luego, se utilizará la fórmula que relaciona carga almacenada con capacitancia:
Q = C∆V → C =

Q
∆V

La capacitancia es propia de la geometría del cuerpo y es siempre un valor positivo.

---

### Página 4

1.6.1

“Ejercicios Teoría Electromagnética ”, 7.2.8, Fabián Cádiz

Considere una esfera maciza conductora de radio a dentro de un cascarón esférico de
radio b. En el espacio entre ambos conductores se introduce un cascarón esférico conductor neutro de radios interno y externo c y d, respectivamente. Si la esfera de radio
a tiene carga Q y el cascarón de radio b tiene −Q, discuta que ocurre con la capacidad
al introducir el cascarón.

Figura 1. Esquema sobre los conductores en estudio.
a) Determine las cargas en las superficies interior y exterior del cascarón intermedio
(radios c y d).
b) Determine las densidades de carga en las superficies interior y exterior del cascarón
intermedio (radios c y d).
c) ¿En qué regiones el campo eléctrico es nulo?
d) Calcule la diferencia de potencial entre la superficie de la esfera maciza y el cascarón esférico de radio b.
e) Determine el valor de capacitancia para la configuración.
f) ¿Qué sucede con el valor de la capacitancia si se extrae el cascarón intermedio de
la configuración? Eqplíquelo de manera cualitativa y cuantitativa.

Solución a), b) y c)
Se pide determinar las cargas en las superficies interior y exterior del cascarón intermedio (i.e
r = c y r = d). Como se está hablando de una esfera, se deberá aplicar estratégicamente Ley
de Gauss utilizando una esfera concéntrica de radio = r” arbitrario:
I
⃗ · d⃗s = Qenc
ε0
S
El conductor intermedio es neutro y experimentará un efecto
de polarización debido a la esfera conductora cargada de radio a.
Luego, la carga en la superficie estará determinada por una integral doble en esféricas:

---

### Página 5

ZZ
σ dS

Q=
S

Solución d) y e)
Se pide determinar la capacitancia de la configuración. Para ello, es necesario solo conocer el
campo y potencial eléctrico que se encuentra en medio de los lugares que contienen carga (i.e
a < r < b). Como se está hablando de una esfera, es posible aplicar Ley de Gauss utilizando
una esfera concéntrica de radio = r” arbitrario:
I
⃗ · d⃗s = Qenc
ε0
S
Luego, se puede utilizar la forma integral de la relación campo - potencial eléctrico:
Z ⃗rb
⃗ · d⃗l
V (⃗rb ) − V (⃗ra ) = −
⃗
ra

Además, y como se presentan = cortes visuales” relacionados con un cambio en la densidad
de carga, se debe trabajar por intervalos: r < a, a < r < c, c < r < d, d < r < b y r > b.

Finalmente, se ocupa la expresión que relaciona carga almacenada con capacitancia:
Q = C∆V

Solución f )
Se pide determinar la capacitancia de la nueva configuración, luego de la extracción del conductor intermedio. Para ello, es necesario solo conocer el campo y potencial eléctrico que se
encuentra en medio de los lugares que contienen carga (i.e a < r < b). Como se está hablando
de una esfera, es posible aplicar Ley de Gauss utilizando una esfera concéntrica de radio = r”
arbitrario:
I
⃗ · d⃗s = Qenc
ε0
S
Luego, se puede utilizar la forma integral de la relación campo - potencial eléctrico:
Z ⃗rb
⃗ · d⃗l
V (⃗rb ) − V (⃗ra ) = −
⃗
ra

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: r < a, a < r < b y r > b.

Finalmente, se ocupa la expresión que relaciona carga almacenada con capacitancia:
Q = C∆V

---

### Página 6

1.6.2

“Ejercicios Teoría Electromagnética ”, 7.5.6, Fabián Cádiz

Dos placas conductoras cuadradas de lado a se disponen con sus caras paralelas y muy
próximas entre sí. La distancia entre las placas es x, como se indica en la figura. Calcule
la fuerza sobre la placa B en las direcciones x y z cuando la diferencia de potencial entre
las placas es V0 .

Figura 2. Esquema sobre las placas conductoras.

#### Solución
Se pide determinar la fuerza sobre la placa B cuando la diferencia de potencial entre las placas
es V0 . Como la diferencia de potencial es constante, la fuerza entre conductores cargados estará
dada por:
⃗ )
F⃗ = (∇U
V =cte

La energía almacenada en un condensador se puede expresar de distintas maneras:

U=

1 Q2
= CV 2 = QV
2 C

Por último, la capacitancia de un condensador de placas paralelas se puede escribir como:

C=

εA
d

---

### Página 7

1.6.3

“Problemas Resueltos de Electromagnetismo”, 4.13, Rodrigo Chi

Una carga +Q se encuentra inserta en un alambre conductor de largo L y radio R0
muy pequeño. Un cascarón cilíndrico conductor neutro de radios internos R1 y externo
R2 y largo L es ubicado simétricamente alrededor del alambre. Tener en cuenta que
R0 ≪ R1 , R2 ≪ L.

Figura 3. Esquema sobre la configuración en estudio.
Ahora, deposite una carga −Q en el cascarón cilíndrico. Calcule:
a) La densidad lineal de carga λ del alambre.
b) La densidad superficial de carga en la capa interna y externa del cascarón.
c) El campo eléctrico en todo el espacio.
d) La diferencia de potencial entre el alambre y el cilindro.
e) La capacitancia del sistema.
f) La capacidad C ′ si ahora el alambre tiene carga 2Q y el cascarón tiene carga −2Q.
Explique su resultado basado en la definición de capacitancia.

Solución a)
Paso Único: Densidad de Carga - λ
La carga total del alambre estará determinada por una integral simple en cartesianas:
Z
Q=
λ dl
L

---

### Página 8

Solución b) y c)
Se pide determinar las cargas en las superficies interior y exterior del cascarón (i.e r = R1 y
r = R2 ). Como se está hablando de un cilindro, se deberá aplicar estratégicamente Ley de
Gauss utilizando una cilindro coaxial de altura = L” y radio = r” arbitrario:
I
⃗ · d⃗s = Qenc
ε0
S
El cascarón está cargado y experimentará un efecto
de polarización debido al alambre con carga Q.
Luego, la carga en la superficie estará determinada por una integral doble en cilíndricas:

ZZ
σ dS

Q=
S

Solución e)
Se pide determinar el campo eléctrico en todo el espacio. Como se está hablando de un alambre
y cilindro, es posible aplicar Ley de Gauss utilizando un cilindro coaxial de altura = L” y de
radio = r” arbitrario:
I
⃗ · d⃗s = Qenc
ϵ0
S
Además, y como se presentan = cortes visuales” relacionados con un cambio en la
densidad de carga, se debe trabajar por intervalos: r < R1 , R1 < r < R2 y r > R2 .

Solución f )
Paso Único: Potencial Eléctrico - ∆V
Se pide determinar la diferencia de potencial que se encuentra entre el alambre y el cilindro
(i.e R0 < r < R1 ), por lo que se utilizará la forma integral de la relación campo - potencial
électrico:
Z R0
⃗ R <r<R · d⃗l
∆V = V (R0 ) − V (R1 ) = −
R1

Solución g)
Paso Único: Capacitancia - C
Se pide determinar la capacitancia de la configuración propuesta. Para ello, es necesario solo
conocer el campo y potencial eléctrico que se encuentra en medio de los lugares que contienen
cargas de igual magnitud, pero opuestas (i.e R0 < r < R1 ). Finalmente, se ocupa la expresión
que relaciona carga almacenada con capacitancia:
Q = C∆V

---

### Página 9

Solución i)
Se pide determinar la capacitancia de la nueva configuración. Para ello, es necesario solo
conocer el campo y potencial eléctrico que se encuentra en medio de los lugares que contienen
cargas de igual magnitud, pero opuestas (i.e R0 < r < R1 ). Finalmente, se ocupa la fórmula
que relaciona carga almacenada con capacitancia:
Q = C∆V

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 7
02 de Septiembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Conductores y Condensadores

1.1

Conductores - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Conocer las propiedades y efectos de medios conductores sobre el campo eléctrico.
□
✓ Determinar el campo eléctrico en configuraciones con medios conductores.
□
✓ Determinar el potencial eléctrico en configuraciones con medios conductores.
□
✓ Calcular la carga y densidad de carga superficial inducida en superficies de medios con□
ductores.
✓ Aplicar el principio de conservación de carga para cuerpos neutros y cargados.
□
1.2

Condensadores - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Conocer el concepto, funcionamiento y aplicaciones de un condensador.
□
✓ Determinar la capacitancia de diversas configuraciones en presencia de conductores.
□
✓ Determinar la fuerza generada entre medios conductores cargados.
□
✓ Calcular la energía almacenada en un capacitor según el contexto.
□
✓ Aplicar la expresión de capacitancia para placas paralelas en diversas configuraciones.
□
✓ Calcular el gradiente de una función para distintos sistemas de coordenadas.
□
✓ Comparar el valor de la capacitancia en presencia de medios conductores.
□
✓ Conocer la unidad de medida para la capacitancia.
□

---

### Página 2

1.3

Conductores - Generalidades

Los materiales conductores (tales como los metales) presentan ciertas propiedades que les son
inherentes por naturaleza. Así, los electrones se podrán mover libremente en su interior y
seguirán en movimiento mientras experimenten un campo eléctrico; sin embargo, estos se detendrán si no están provistos continuamente de una fuente de energía externa.
De esta manera:
a) El campo eléctrico dentro de un conductor es nulo.
b) Luego, por Ley de Gauss y el principio de conservación de carga, la carga en un conductor
necesariamente debe distribuirse equipotencialmente y solo en su superficie:
⃗ · d⃗s = 0 → Qenc = 0
(1)
S

Al mismo tiempo, esto significa que al interior
de un conductor el potencial eléctrico es constante:

⃗ =0
−∇V

(2)

c) La componente tangencial del campo eléctrico en la superficie de un conductor es cero,
por lo que solo sobrevivirá la componente normal a esta.

1.4

Conductores - Cómo Utilizarlo Correctamente

En variados ejercicios les pedirán determinar la carga superficial inducida en las superficies del
conductor. Los pasos a seguir son:
1. = Calcular” estratégicamente el campo en un lugar que contenga conductor y que esté
justo afuera de la superficie relacionada con la carga pedida. Por propiedades, este
campo debe ser nulo e implica necesariamente que la carga encerrada es 0:
⃗ · d⃗s = 0 → Qenc = 0
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

### Página 3

1.5

Condensadores - Generalidades

Un condensador es un dispositivo capaz de acumular carga eléctrica, que generalmente consiste
en dos conductores cargados con cargas opuestas de igual magnitud. De esta forma, la carga
almacenada en un condensador está dada por:
Q = C∆V

(3)

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

(4)

(5)

Resolviendo, y reemplazando por la expresión que
relaciona carga almacenada con capacitancia, se obtiene que:

U=

1 Q2
= CV 2 = QV
2 C

(6)

Asimismo, la fuerza entre conductores cargados se puede escribir como:

⃗ )
F⃗ = (∇U

⃗ )
= − (∇U
V =cte

(7)
Q=cte

Finalmente, podría ser de utilidad saber la capacitancia de un condensador de placas paralelas:
C=

εA
d

(8)

Donde = ε” es la constante de permitividad del medio que se encuentra
rellenando totalmente el espacio entre ambas placas, = A” el área = efectiva” de
las placas (proyección de una sobre la otra) y = d” la distancia entre las mismas.

1.6

Condensadores - Cómo Utilizarlo Correctamente

El fuerte en esta sección será determinar la capacitancia de cierta configuración:
1. ¿Dónde se ubican las cargas opuestas? Esto será fundamental, pues solo se deberá calcular
la diferencia de potencial entre estos límites de acuerdo a la siguiente fórmula:
Z a
⃗ a<r<b · d⃗l
∆V = V (a) − V (b) = −
b

Donde = a” y = b” indican la ubicación de la carga positiva y negativa.
De esta manera, se tendrá que calcular el campo eléctrico necesario para el potencial.

2. Luego, se utilizará la fórmula que relaciona carga almacenada con capacitancia:
Q = C∆V → C =

∆V

La capacitancia es propia de la geometría del cuerpo y es siempre un valor positivo.

---

### Página 4

1.6.1

“Ejercicios Teoría Electromagnética ”, 7.2.8, Fabián Cádiz

Considere una esfera maciza conductora de radio a dentro de un cascarón esférico de
radio b. En el espacio entre ambos conductores se introduce un cascarón esférico conductor neutro de radios interno y externo c y d, respectivamente. Si la esfera de radio
a tiene carga Q y el cascarón de radio b tiene −Q, discuta que ocurre con la capacidad
al introducir el cascarón.

Figura 1. Esquema sobre los conductores en estudio.
a) Determine las cargas en las superficies interior y exterior del cascarón intermedio
(radios c y d).
b) Determine las densidades de carga en las superficies interior y exterior del cascarón
intermedio (radios c y d).
c) ¿En qué regiones el campo eléctrico es nulo?
d) Calcule la diferencia de potencial entre la superficie de la esfera maciza y el cascarón esférico de radio b.
e) Determine el valor de capacitancia para la configuración.
f) ¿Qué sucede con el valor de la capacitancia si se extrae el cascarón intermedio de
la configuración? Eqplíquelo de manera cualitativa y cuantitativa.

Solución a), b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar las cargas en las superficies interior y exterior del cascarón intermedio (i.e
r = c y r = d). Como se está hablando de una esfera, se deberá aplicar estratégicamente Ley
de Gauss utilizando una esfera concéntrica de radio = r” arbitrario:
⃗ · d⃗s = Qenc
ε0
S
El conductor intermedio es neutro y experimentará un efecto
de polarización debido a la esfera conductora cargada de radio a.
Luego, la carga en la superficie estará determinada por una integral doble en esféricas:

---

### Página 5

ZZ
σ dS

Q=
S

Paso 1: Carga Superficial - Qa
La esfera de radio a es conductora, por lo que el campo eléctrico en su interior será nulo y su
carga solo se ubicará en su superficie:
Qa = Q

(9)

Paso 2: Carga Superficial - Qc
Luego, se calculará estratégicamente el campo eléctrico mediante la Ley de Gauss en la región
c < r < d:
⃗ c<r<d · dS
⃗ = Qenc
ε0
El cascarón esférico es conductor, por lo que el campo eléctrico
en su interior será nulo y su carga solo se ubicará en sus superficies:

⃗ c<r<d = 0

(10)

Con lo anterior, la carga encerrada (en r < d) también debe ser igual a 0:

Qenc = 0
Qa + Qc = 0
Reemplazando se obtiene que:

Q + Qc = 0
Qc = −Q

(11)

Paso 3: Densidad Carga Superficial - σc
Así, la carga en la superficie r = c estará determinada por una integral doble en esféricas:
ZZ
Qc =
σ dS
S

Como la densidad de carga del cascarón es uniforme,
se puede tratar como una constante y sale de la integral:

Z 2π Z π
−Q = σc

c2 sin θ dθdϕ

−Q = σc · 2π · 2 · c2
σc = −
4πc2

(12)

---

### Página 6

Paso 4: Carga Superficial - Qd
El cascarón esférico ubicado entre c y d no posee carga y es conductor, es decir, es neutro y su
carga solo se ubicará en sus superficies. Aplicando el principio de conservación de carga sobre
el cascarón se obtiene que:
Qc + Qd = 0
−Q + Qd = 0
Qd = Q

(13)

Paso 5: Densidad Carga Superficial - σd
Así, la carga en la superficie r = d estará determinada por una integral doble en esféricas:
ZZ
Qd =
σ dS
S

Como la densidad de carga del cascarón es uniforme,
se puede tratar como una constante y sale de la integral.

Z 2π Z π
Q = σd

d2 sin θ dθdϕ

(14)

Q = σd · 2π · 2 · d2
σd =
4πd2

Nota: No es estrictamente necesario realizar la integral de superficie para determinar
la densidad de carga. Como la densidad de carga es uniforme, basta con saber que se
refería al área de una esfera de radio ri , con i = c, d.

Solución d) y e)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la capacitancia de la configuración. Para ello, es necesario solo conocer el
campo y potencial eléctrico que se encuentra en medio de los lugares que contienen carga (i.e
a < r < b). Como se está hablando de una esfera, es posible aplicar Ley de Gauss utilizando
una esfera concéntrica de radio = r” arbitrario:
⃗ · d⃗s = Qenc
ε0
S
Luego, se puede utilizar la forma integral de la relación campo - potencial eléctrico:
Z ⃗rb
⃗ · d⃗l
V (⃗rb ) − V (⃗ra ) = −
⃗
ra

Además, y como se presentan = cortes visuales” relacionados con un cambio en la densidad
de carga, se debe trabajar por intervalos: r < a, a < r < c, c < r < d, d < r < b y r > b.

Finalmente, se ocupa la expresión que relaciona carga almacenada con capacitancia:
Q = C∆V

---

### Página 7

⃗ a<r<c
Paso 1: Ley de Gauss - E
En primer lugar, se calculará el campo eléctrico mediante la Ley de Gauss en la región a <
r < c:
⃗ a<r<c · dS
⃗ = Qenc
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada será la carga total de la esfera de radio a:

Ea<r<c ·

dS =

ε0

Ahora, la integral cerrada es en verdad la superficie de la esfera gaussiana.
pues el flujo es ortogonal a este en todo momento:

Ea<r<c · 4πr2 =
Ea<r<c =

ε0
4πr2 ε0

(15)

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

⃗ a<r<c =

r̂
4πr2 ε0

(16)

⃗ d<r<b
Paso 3: Ley de Gauss - E
Finalmente, se calculará el campo eléctrico mediante la Ley de Gauss en la región d < r < b:
⃗ d<r<b · dS
⃗ = Qenc
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada será la carga total de la esfera de radio a.
Recordemos que el cascarón es neutro, pese a que existan cargas polarizadas:

Ed<r<b ·

dS =

ε0

Ahora, la integral cerrada es en verdad la superficie de la esfera gaussiana,
pues el flujo es ortogonal a este en todo momento:

Ed<r<b · 4πr2 =

ε0

Ed<r<b =
4πr2 ε0

(17)

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

⃗ d<r<b =

r̂
4πr2 ε0

(18)

---

### Página 8

Paso 4: Potencial Eléctrico - ∆V
Ahora, se calculará la diferencia de potencial eléctrico en la región a < r < b:
Z a
⃗ a<r<b · d⃗l
∆V = V (a) − V (b) = −
b

Por propiedades de integrales se pueden invertir los límites, el campo varía a lo
largo de la trayectoria y la única componente en juego es la radial, por lo que:

Z c

dr +
∆V =
2ε
4πr
a

Z b

Z d
0 dr +
c

dr
2ε
4πr
d

c

1 b
=
(− ) +
(− )
4πε0
r a 4πε0
r d
Q 1 1
Q 1 1
( − )−
( − )
=−
4πε0 c a
4πε0 b d
Q 1 1 1 1
( − + − )
=
4πε0 a c d b

(19)

Paso 5: Capacitancia - C
Por último, se ocupa la expresión que relaciona carga almacenada con capacitancia:
C=
=

∆V
4πε0 ( a − c + d − b )

(20)

1 1 1 1
= 4πε0 ( − + − )−1
a c d b
Se debe notar que b > d > c > a, por lo que se cumple que C > 0.

Solución f )
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la capacitancia de la nueva configuración, luego de la extracción del conductor intermedio. Para ello, es necesario solo conocer el campo y potencial eléctrico que se
encuentra en medio de los lugares que contienen carga (i.e a < r < b). Como se está hablando
de una esfera, es posible aplicar Ley de Gauss utilizando una esfera concéntrica de radio = r”
arbitrario:
⃗ · d⃗s = Qenc
ε0
S
Luego, se puede utilizar la forma integral de la relación campo - potencial eléctrico:
Z ⃗rb
⃗ · d⃗l
V (⃗rb ) − V (⃗ra ) = −
⃗
ra

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: r < a, a < r < b y r > b.

---

### Página 9

Finalmente, se ocupa la expresión que relaciona carga almacenada con capacitancia:
Q = C∆V
⃗ a<r<b
Paso 1: Ley de Gauss - E
En primer lugar, se calculará el campo eléctrico en la región a < r < b:
⃗ a<r<b · dS
⃗ = Qenc
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada será la carga total de la esfera de radio a:

Ea<r<b ·

dS =

ε0

Ahora, la integral cerrada es en verdad la superficie de la esfera.
pues el flujo es ortogonal a esta en todo momento:

Ea<r<b · 4πr2 =
Ea<r<b =

ε0
4πr2 ε0

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

⃗ a<r<b =

r̂
4πr2 ε0

Paso 2: Potencial Eléctrico - ∆V
Luego, se calculará la diferencia de potencial eléctrico en la región a < r < b:
Z a
⃗ a<r<b · d⃗l
∆V = V (a) − V (b) = −
b

Por propiedades de integrales se pueden invertir los límites
y la única componente en juego es la radial, por lo que:

Z b
∆V =

dr
a 4πr ε0

1 b
(− )
4πε0
r a
Q 1 1
=−
( − )
4πε0 b a
Q 1 1
=
( − )
4πε0 a b
=

(21)

---

### Página 10

Paso 3: Capacitancia - C
Finalmente, se ocupa la expresión que relaciona carga almacenada con capacitancia:
C=
=

∆V
4πε0 ( a − b )

(22)

1 1
= 4πε0 ( − )−1
a b
Se debe notar que b > a, por lo que se cumple que C > 0.

Paso 4: Análisis Capacitancia - C
Por último, se debe comparar el valor de la capacitancia en ambos casos. Se nota que el único
término diferente es = − 1c + d1 ”, por lo que se analiza su posible valor. Como el radio = d” es
mayor que el radio = c”:
d>c
” y considerando ambos radios como positivos:
Multiplicando la expresión por = cd

<
d
c
1 1
− <0
d c

(23)

De esta manera, el término adicional posee un valor negativo.

Así, el potencial de la configuración en presencia de un material conductor será menor y, por
lo tanto, su capacitancia será mayor con respecto a la de un condensador esférico común.
Finalmente, y al extraer el conductor intermedio, la nueva capacitancia es menor.
Nota: Se realizó nuevamente el cálculo de potencial para ilustrar de mejor manera el
efecto provocado por la extracción del conductor, pero no era estrictamente necesario
determinarlo. Bastaría con notar que el campo eléctrico que aporta un conductor es
nulo y, por ello, la diferencia de potencial experimentará un aumento luego de extraer
el cascarón intermedio.

---

### Página 11

1.6.2

“Ejercicios Teoría Electromagnética ”, 7.5.6, Fabián Cádiz

Dos placas conductoras cuadradas de lado a se disponen con sus caras paralelas y muy
próximas entre sí. La distancia entre las placas es x, como se indica en la figura. Calcule
la fuerza sobre la placa B en las direcciones x y z cuando la diferencia de potencial entre
las placas es V0 .

Figura 2. Esquema sobre las placas conductoras.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la fuerza sobre la placa B cuando la diferencia de potencial entre las placas
es V0 . Como la diferencia de potencial es constante, la fuerza entre conductores cargados estará
dada por:
⃗ )
F⃗ = (∇U
V =cte

La energía almacenada en un condensador se puede expresar de distintas maneras:

U=

1 Q2
= CV 2 = QV
2 C

Por último, la capacitancia de un condensador de placas paralelas se puede escribir como:

C=

εA
d

Paso 1: Capacitancia Placas Paralelas - C
La capacitancia de un condensador de placas paralelas se puede escribir como:
C=

εA
d

En este caso = ε = ε0 ”, pues entre ambas placas solo existe vacío.
Además, = d = x” será la distancia y = A = a(a − z)” el área efectiva entre las placas:

---

### Página 12

C(x, z) =

ε0 a(a − z)
x

(24)

Paso 2: Energía Almacenada - U
La energía almacenada en un condensador se puede expresar de distintas maneras:
U=

1 Q2
= CV 2 = QV
2 C

Es importante notar que todas son equivalentes e igual de válidas.
Por conveniencia, se utilizará la que relaciona = C” y = V ”, pues son datos conocidos:

1 ε0 a(a − z) 2
U = CV 2 =
V0
x
Por enunciado, la diferencia de potencial entre ambas placas es = V0 ”.

Paso 3: Fuerza y Gradiente de la Energía - F⃗
Como la diferencia de potencial es constante por enunciado, la fuerza entre conductores cargados estará dada por:
⃗ )
F⃗ = (∇U
V =cte

Luego, y como se está trabajando en coordenadas cartesianas, el vector gradiente será:

dU
dU
dU
F⃗ =
x̂ +
ŷ +
ẑ
dx
dy
dz
d a−z
d a−z
d a−z
= ε0 aV02 ( (
)x̂ + (
)ŷ + (
)ẑ)
dx x
dy x
dz x
a−z
= ε0 aV02 (−( 2 )x̂ + 0 + − ẑ)
x
x
1 ε0 aV02 (a − z)
=−
(
x̂ + ẑ)
2 x
x

(25)

---

### Página 13

1.6.3

“Problemas Resueltos de Electromagnetismo”, 4.13, Rodrigo Chi

Una carga +Q se encuentra inserta en un alambre conductor de largo L y radio R0
muy pequeño. Un cascarón cilíndrico conductor neutro de radios internos R1 y externo
R2 y largo L es ubicado simétricamente alrededor del alambre. Tener en cuenta que
R0 ≪ R1 , R2 ≪ L.

Figura 3. Esquema sobre la configuración en estudio.
Ahora, deposite una carga −Q en el cascarón cilíndrico. Calcule:
a) La densidad lineal de carga λ del alambre.
b) La densidad superficial de carga en la capa interna y externa del cascarón.
c) El campo eléctrico en todo el espacio.
d) La diferencia de potencial entre el alambre y el cilindro.
e) La capacitancia del sistema.
f) La capacidad C ′ si ahora el alambre tiene carga 2Q y el cascarón tiene carga −2Q.
Explique su resultado basado en la definición de capacitancia.

Solución a)
Paso Único: Densidad de Carga - λ
La carga total del alambre estará determinada por una integral simple en cartesianas:
Z
Q=
λ dl
L

Como la densidad de carga del alambre es uniforme,

---

### Página 14

se puede tratar como una constante y sale de la integral.
Su largo es L y su carga total es Q:

Z L
dz

Q=λ

Q=λ·L
λ=
L

(26)

Solución b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar las cargas en las superficies interior y exterior del cascarón (i.e r = R1 y
r = R2 ). Como se está hablando de un cilindro, se deberá aplicar estratégicamente Ley de
Gauss utilizando una cilindro coaxial de altura = L” y radio = r” arbitrario:
⃗ · d⃗s = Qenc
ε0
S
El cascarón está cargado y experimentará un efecto
de polarización debido al alambre con carga Q.
Luego, la carga en la superficie estará determinada por una integral doble en cilíndricas:

ZZ
Q=

σ dS
S

Paso 1: Carga Superficial - QR1
En primer lugar, se calculará estratégicamente el campo eléctrico mediante la Ley de Gauss
en la región R1 < r < R2 :
⃗ R <r<R · dS
⃗ = Qenc
ε0
El cascarón cilíndrico es conductor, por lo que el campo eléctrico
en su interior será nulo y su carga solo se ubicará en su superficie:

⃗ R <r<R = 0

(27)

Con lo anterior, la carga encerrada (en r < R2 ) debe ser igual a 0:

Qenc = 0
Q + QR1 = 0
QR1 = −Q

(28)

Paso 2: Densidad Carga Superficial - σR1
Así, la carga en la superficie r = R1 estará determinada por una integral doble en cilíndricas:
ZZ
QR1 =
σ dS
S

---

### Página 15

Como la densidad de carga del cascarón es uniforme,
se puede tratar como una constante y sale de la integral:

Z L Z 2π
−Q = σR1

R1 dθdz

−Q = σR1 · 2πR1 L
σ R1 = −
2πR1 L

(29)

Paso 4: Carga Superficial - QR2
El cascarón cilíndrico ubicado entre R1 y R2 está cargado con carga −Q y es conductor, es
decir, su carga solo se ubicará en sus superficies. Mediante el principio de conservación de
carga se obtiene que:
QR1 + QR2 = −Q
−Q + QR2 = −Q
QR2 = 0

(30)

Paso 5: Densidad Carga Superficial - σR2
Así, la carga en la superficie r = R2 estará determinada por una integral doble en cilíndricas:
ZZ
Q=
σ dS
S

Como su carga total es 0, su densidad de carga es nula:

σR2 = 0

(31)

Nota: No es estrictamente necesario realizar la integral de superficie para determinar
la densidad de carga. Como la densidad de carga es uniforme, basta con saber que se
refería al área del manto de un cilindro de altura L y radio Ri , con i = 1, 2.

Solución e)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en todo el espacio. Como se está hablando de un alambre
y cilindro, es posible aplicar Ley de Gauss utilizando un cilindro coaxial de altura = L” y de
radio = r” arbitrario:
⃗ · d⃗s = Qenc
ϵ0
S
Además, y como se presentan = cortes visuales” relacionados con un cambio en la
densidad de carga, se debe trabajar por intervalos: r < R1 , R1 < r < R2 y r > R2 .

---

### Página 16

⃗ r<R
Paso 1: Ley de Gauss - E
En primer lugar, se calculará el campo eléctrico mediante la Ley de Gauss en la región r < R0 :
⃗ = Qenc
⃗ r<R · dS
ε0
El alambre es conductor, por lo que el campo eléctrico en su
interior será nulo y su carga solo se ubicará en su superficie:

⃗ r<R = 0

(32)

⃗ R <r<R
Paso 2: Ley de Gauss - E
Ahora, se calculará el campo eléctrico mediante la Ley de Gauss en la región R0 < r < R1 :
⃗ R <r<R · dS
⃗ = Qenc
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada será la carga total del alambre:

ER0 <r<R1 ·

dS =

ε0

Ahora, la integral cerrada es en verdad la superficie del manto del cilindro gaussiano,
pues el flujo es ortogonal a esta en todo momento:

ER0 <r<R1 · 2πrL =

ε0

ER0 <r<R1 =
2πrLε0

(33)

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

⃗ R <r<R =

r̂
2πrLε0

(34)

⃗ r>R
Paso 4: Ley de Gauss - E
Por último, se calculará el campo eléctrico mediante la Ley de Gauss en la región r > R2 :
⃗ r>R · dS
⃗ = Qenc
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada será la carga total de la configuración:

Er>R2 ·

dS =

Q−Q
=0
ε0

Como la configuración es eléctricamente neutra se obtiene que:

⃗ r>R = 0

(35)

---

### Página 17

Solución f )
Paso Único: Potencial Eléctrico - ∆V
Se pide determinar la diferencia de potencial que se encuentra entre el alambre y el cilindro
(i.e R0 < r < R1 ), por lo que se utilizará la forma integral de la relación campo - potencial
électrico:
Z R0
⃗ R <r<R · d⃗l
∆V = V (R0 ) − V (R1 ) = −
R1

Luego, por propiedades de integrales se pueden invertir los límites
y la única componente en juego es la radial, por lo que:

Z R1
∆V =
R0

dr
2πrLε0

R1
(ln r)
2πLε0
R0
(ln R1 − ln R0 )
=
2πLε0
 
R1
=
ln
2πLε0
R0

=

(36)

Solución g)
Paso Único: Capacitancia - C
Se pide determinar la capacitancia de la configuración propuesta. Para ello, es necesario solo
conocer el campo y potencial eléctrico que se encuentra en medio de los lugares que contienen
cargas de igual magnitud, pero opuestas (i.e R0 < r < R1 ). Finalmente, se ocupa la expresión
que relaciona carga almacenada con capacitancia:
Q = C∆V
Reemplazando valores se obtiene que:

C=
=

=

∆V


R1
2πLε0 ln R0



(37)

2πLε0
 
R1
ln R

Se debe notar que R1 > R0 , por lo que se cumple que C > 0.

Solución i)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la capacitancia de la nueva configuración. Para ello, es necesario solo
conocer el campo y potencial eléctrico que se encuentra en medio de los lugares que contienen

---

### Página 18

cargas de igual magnitud, pero opuestas (i.e R0 < r < R1 ). Finalmente, se ocupa la fórmula
que relaciona carga almacenada con capacitancia:
Q = C∆V
Paso 1: Análisis Nueva Capacitancia - C ′
Como se modifican las cargas contenidas de igual manera para el alambre y el cascarón, solo
bastaría con cambiar Q por 2Q en los resultados anteriores:
2Q
r̂
2πrLε0
 
2Q
R1
∆V =
ln
2πLε0
R0

⃗ R <r<R =

(38)
(39)

Finalmente, se ocupa la fórmula que relaciona carga almacenada con capacitancia:

C′ =
=

=

∆V
2Q
 
2Q
R1
ln
2πLε0
R0

(40)

2πLε0
 
ln R
R0

Se debe notar que R1 > R0 , por lo que se cumple que C > 0.
Luego, se concluye que la nueva capacitancia es igual a la anterior (i.e C = C ′ ).

Nota: Se puedo haber realizado todo el ejercicio nuevamente con el cambio propuesto,
pero supone algo demoroso. Luego, basta con saber que la capacitancia nace a partir
de la geometría de la figura y no depende de la carga almacenada.
