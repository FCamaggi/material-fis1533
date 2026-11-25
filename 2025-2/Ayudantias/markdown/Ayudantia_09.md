---
title: "Ayudantia 09"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_09_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_09_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 09

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Ayudantía 9
09 de Septiembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Medios Dieléctricos

1.1

Dieléctricos - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Conocer las propiedades y los efectos de medios dieléctricos.
□
✓ Determinar el desplazamiento eléctrico en presencia de medios dieléctricos mediante la
□
Ley de Gauss Generalizada.
✓ Determinar el campo eléctrico en presencia de medios dieléctricos a partir de la expresión
□
que lo relaciona con el desplazamiento eléctrico.
✓ Determinar la capacitancia de diversas configuraciones en presencia de medios dieléctricos.
□
✓ Calcular el vector polarización en medios dieléctricos.
□
✓ Identificar el vector normal en las superficies de medios dieléctricos.
□
✓ Determinar la densidad de carga de polarización superficial en medios dieléctricos.
□
✓ Determinar la densidad de carga de polarización volumétrica en medios dieléctricos.
□
✓ Aplicar la condición de borde para el campo eléctrico en la interfaz de medios dieléctricos
□
según corresponda.
✓ Aplicar la condición de borde para el desplazamiento eléctrico en la interfaz de medios
□
dieléctricos según corresponda.
□ Determinar la densidad de carga libre superficial en medios dieléctricos.
□ Utilizar la constante dieléctrica de un medio en términos de su permitividad eléctrica.

✓ Calcular la divergencia de una función para distintos sistemas de coordenadas.
□

---

### Página 2

1.2

Dieléctricos - Polarización, Susceptibilidad y Constante Dieléctrica

El átomo posee un pequeño momento dipolar que apunta en la misma dirección que el campo
eléctrico tal que:
p = αE
Donde = α” es la polarizabilidad atómica.
Además, se puede definir el momento dipolar eléctrico por unidad de volumen como:

P=

∆p
∆v

Donde = P” es la polarización del material.

La polarización de un medio dieléctrico es el resultado de la aplicación de un campo eléctrico
externo:
P(x) = ε0 χe E(x)

(1)

Donde = E” es el campo eléctrico total y = χe ” la susceptibilidad eléctrica del medio.
Así, el vector desplazamiento para un dieléctrico lineal está dado por:

D(x) = ε0 (1 + χe )E(x) = εE(x)

(2)

Donde = ε” es la permitividad del material y = ε0 ” la permitividad del vacío.
Luego, se puede definir la permitividad relativa o constante dieléctrica como:

κ = εr =

ε
= 1 + χe
ε0

(3)

Notar que = κ” es siempre mayor que 1, excepto en el vacío, donde es igual a 1.

1.3

Dieléctricos - Campo Eléctrico y Ley de Gauss Generalizada

La densidad de carga total dentro de un material dieléctrico se puede modelar como:
ρ = ρb + ρf

(4)

Donde = ρf ” y = ρb ” es la densidad de carga libre y ligada, respectivamente. Además, se tiene que:

σP (x) = P(x) · n̂(x)

(5)
r=a

⃗ · P(x)
ρP (x) = −∇

(6)

Donde = σP ” y = ρP ” son las densidades de carga de polarización
superficial y volumétrica, respectivamente. Se recuerda que = n̂”
es el vector normal a la superficie en cuestión, en este caso = a” .

Ahora, se puede definir el desplazamiento eléctrico como:
D(x) = ε0 E(x) + P(x)
De esta manera, la Ley de Gauss generalizada se puede enunciar como:

I
D · ds = Qf → ∇ · D = ρf
S

(7)

---

### Página 3

Donde = Qf ” es la carga libre total del cuerpo que está encerrada por la superficie gaussiana.

Sumado a lo anterior, y al atravesar una interfaz entre dos medios dieléctricos, los campos
deben satisfacer que:
E1t = E2t

(8)
r=a

D2n − D1n = σf

(9)
r=a

Donde = t” y = n” son las componentes tangencial y normal, respectivamente.
Se debe considerar que los subíndices = 1” y = 2” hacen referencia a lo que se
encuentra dentro y fuera con respecto a la superficie en cuestión, en este caso = a”.
De lo anterior, se deduce que = Et ” debe ser continua, mientras que = Dn ” discontinua.

1.4

Dieléctricos - Cómo Utilizarlo Correctamente I

Generalmente, se querrá determinar el vector polarización y, con ello, las densidades de carga
de polarización superficial y volumétrica. Los pasos a seguir son:
a) = D = ε0 E + P ”: el vector polarización se puede calcular fácilmente a partir de la
relación con el campo y desplazamiento eléctrico. De esta manera:
1. Si es que el dieléctrico es lineal, es posible despejar el vector polarización fácilmente:
P = D − ε0 E = εE − ε0 E = (ε − ε0 )E

(10)

De ahora en adelante, se podrá utilizar esta fórmula libremente.

2. Solo quedaría reemplazar por el = ε” y = E” respectivos, los cuales dependerán únicamente
del lugar en donde se requiera calcular. Se hace énfasis en que = E” será el campo
en donde se localice el dieléctrico y, además, se desprende que el vector polarización
poseerá la misma componente que el campo eléctrico.
b) = σP (x) = P(x) · n̂(x) r=a ”: en esta parte se deberá calcular la densidad de carga de
polarización superficial en una superficie arbitraria = a”. Para ello:
1. Se debe distinguir el lugar en donde se requiere calcular la densidad superficial.
2. Luego, se debe identificar el campo eléctrico próximo a tal superficie y el cual
contiene al dieléctrico. Se calcula el vector polarización y simplemente se reemplaza.
3. ¿Cómo se determina el vector normal? Este será un vector ortogonal a la superficie
en cuestión y apuntará hacia afuera del dieléctrico.
4. Por último, se reemplaza todo en la expresión y se evalúa en el = punto” en donde se
ubica la superficie. Recuerden también que el producto punto de dos coordenadas
idénticas es igual a 1.
⃗ · P(x) ”: en esta parte se deberá calcular la densidad de carga de polarc) = ρP (x) = −∇
ización volumétrica en el lugar en donde se encuentra el dieléctrico. Para ello:
1. Se debe distinguir el lugar en donde se requiere calcular la densidad volumétrica.
2. Luego, se debe identificar el campo eléctrico que existe en esa zona y el cual contiene
al dieléctrico.
3. Se calcula el vector polarización, se reemplaza y se aplica la divergencia. En este
punto tengan cuidado, pues la divergencia dependerá de las coordenadas que se
estén utilizando.

---

### Página 4

1.5

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

1.6

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
aspectos revelantes se resumen en la tabla del Anexo ??.
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

### Página 5

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

### Página 6

1.6.1

“Problemas Resueltos de Electromagnetismo”, 7.11, Rodrigo Chi

Dos condensadores cilíndricos de radio interior a y exterior 3a, y largo L (muy largo),
han sido llenados con dos materiales dieléctricos ε1 y ε2 de distinta forma. Si los condensadores son conectados de la forma que se indica en la figura, determine la capacidad
equivalente entre los puntos A y B.

Figura 1. Esquema sobre los condensadores cilíndricos.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la capacitancia de la configuración, la cual puede ser vista como dos capacitores conectados en serie (i.e por ambos circula la misma corriente):
N

X 1
=
Ceq
Ci
i

Para ello, es necesario solo conocer el campo y potencial eléctrico que se encuentra en medio de
los lugares que contienen cargas opuestas pero de igual magnitud (i.e a < r < 3a para ambos
casos). Como se está hablando de un cilindro infinito y de materiales dieléctricos, es posible
aplicar Ley de Gauss Generalizada utilizando un cilindro coaxial de altura = L” y radio = r”
arbitrario:
I
D · ds = Qf

---

### Página 7

Ahora, el vector desplazamiento para un dieléctrico está dado por:

D = εE = ε0 κE
Como la permitividad no es constante en la misma sección transversal,
se debe cumplir la siguiente condición de borde para el capacitor inferior:

E1t = E2t
Luego, se puede utilizar la forma integral de la relación campo - potencial eléctrico:
Z rb
V (rb ) − V (ra ) = −
E · dl
ra

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: a < r < 2a y 2a < r < 3a.

Finalmente, se ocupa la fórmula que relaciona carga almacenada con capacitancia:
Q = C∆V
Se asignará de forma arbitraria una carga Q y −Q a las superficies r = a y r = 3a, respectivamente.
Se recuerda que esto no afectará al valor de la capacitancia, pues esta
depende únicamente de su geometría y no de la carga almacenada.

---

### Página 8

1.6.2

“Problemas Resueltos de Electromagnetismo”, 17.7, Rodrigo Chi

Una esfera dieléctrica de radio b y permitividad de carga ε contienen en un interior una
densidad de carga libre:

ρ(r) =

ρ0 r si 0 < r < b
si r > b

a) ¿En qué casos el vector polarización es nulo? Justifique su respuesta.
b) Determine el vector polarización en todo el espacio.
c) Calcule la carga de polarización en la superficie r = b.
d) Calcule la carga de polarización volumétrica en todo el espacio.

Solución a), b), c) y d)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el valor de la densidad de carga de polarización volumétrica y superficial
en las zonas donde existan. El dieléctrico solo toca la superficie r = b, por lo que se debe
observar esa interfaz a la hora de calcular σP , mientras que ρP solo se encontrará en donde el
dieléctrico esté presente (i.e r < b). Luego, se debe utilizar que:
σP (x) = P(x) · n̂(x)
r=b

⃗ · P(x)
ρP (x) = −∇
De aquí se nota que se necesita el vector polarización, el cual está dado por:

P(x) = (ε − ε0 )E(x)
Como se está hablando de una esfera y de materiales dieléctricos, es posible aplicar Ley de
Gauss Generalizada utilizando una esfera concéntrica de radio = r” arbitrario:
I
D · ds = Qf
Ahora, el vector desplazamiento para un dieléctrico está dado por:

D = εE = ε0 κE
La densidad de carga del cilindro no es uniforme,
por lo que se tendrá que utilizar la definición de carga:

ZZZ
Q=

ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: 0 < r < b, y r > b.

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 9
09 de Septiembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Medios Dieléctricos

1.1

Dieléctricos - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Conocer las propiedades y los efectos de medios dieléctricos.
□
✓ Determinar el desplazamiento eléctrico en presencia de medios dieléctricos mediante la
□
Ley de Gauss Generalizada.
✓ Determinar el campo eléctrico en presencia de medios dieléctricos a partir de la expresión
□
que lo relaciona con el desplazamiento eléctrico.
✓ Determinar la capacitancia de diversas configuraciones en presencia de medios dieléctricos.
□
✓ Calcular el vector polarización en medios dieléctricos.
□
✓ Identificar el vector normal en las superficies de medios dieléctricos.
□
✓ Determinar la densidad de carga de polarización superficial en medios dieléctricos.
□
✓ Determinar la densidad de carga de polarización volumétrica en medios dieléctricos.
□
✓ Aplicar la condición de borde para el campo eléctrico en la interfaz de medios dieléctricos
□
según corresponda.
✓ Aplicar la condición de borde para el desplazamiento eléctrico en la interfaz de medios
□
dieléctricos según corresponda.
□ Determinar la densidad de carga libre superficial en medios dieléctricos.
□ Utilizar la constante dieléctrica de un medio en términos de su permitividad eléctrica.

✓ Calcular la divergencia de una función para distintos sistemas de coordenadas.
□

---

### Página 2

1.2

Dieléctricos - Polarización, Susceptibilidad y Constante Dieléctrica

El átomo posee un pequeño momento dipolar que apunta en la misma dirección que el campo
eléctrico tal que:
p = αE
Donde = α” es la polarizabilidad atómica.
Además, se puede definir el momento dipolar eléctrico por unidad de volumen como:

P=

∆p
∆v

Donde = P” es la polarización del material.

La polarización de un medio dieléctrico es el resultado de la aplicación de un campo eléctrico
externo:
P(x) = ε0 χe E(x)

(1)

Donde = E” es el campo eléctrico total y = χe ” la susceptibilidad eléctrica del medio.
Así, el vector desplazamiento para un dieléctrico lineal está dado por:

D(x) = ε0 (1 + χe )E(x) = εE(x)

(2)

Donde = ε” es la permitividad del material y = ε0 ” la permitividad del vacío.
Luego, se puede definir la permitividad relativa o constante dieléctrica como:

κ = εr =

ε
= 1 + χe
ε0

(3)

Notar que = κ” es siempre mayor que 1, excepto en el vacío, donde es igual a 1.

1.3

Dieléctricos - Campo Eléctrico y Ley de Gauss Generalizada

La densidad de carga total dentro de un material dieléctrico se puede modelar como:
ρ = ρb + ρf

(4)

Donde = ρf ” y = ρb ” es la densidad de carga libre y ligada, respectivamente. Además, se tiene que:

σP (x) = P(x) · n̂(x)

(5)
r=a

⃗ · P(x)
ρP (x) = −∇

(6)

Donde = σP ” y = ρP ” son las densidades de carga de polarización
superficial y volumétrica, respectivamente. Se recuerda que = n̂”
es el vector normal a la superficie en cuestión, en este caso = a” .

Ahora, se puede definir el desplazamiento eléctrico como:
D(x) = ε0 E(x) + P(x)
De esta manera, la Ley de Gauss generalizada se puede enunciar como:

I
D · ds = Qf → ∇ · D = ρf
S

(7)

---

### Página 3

Donde = Qf ” es la carga libre total del cuerpo que está encerrada por la superficie gaussiana.

Sumado a lo anterior, y al atravesar una interfaz entre dos medios dieléctricos, los campos
deben satisfacer que:
E1t = E2t

(8)
r=a

D2n − D1n = σf

(9)
r=a

Donde = t” y = n” son las componentes tangencial y normal, respectivamente.
Se debe considerar que los subíndices = 1” y = 2” hacen referencia a lo que se
encuentra dentro y fuera con respecto a la superficie en cuestión, en este caso = a”.
De lo anterior, se deduce que = Et ” debe ser continua, mientras que = Dn ” discontinua.

1.4

Dieléctricos - Cómo Utilizarlo Correctamente I

Generalmente, se querrá determinar el vector polarización y, con ello, las densidades de carga
de polarización superficial y volumétrica. Los pasos a seguir son:
a) = D = ε0 E + P ”: el vector polarización se puede calcular fácilmente a partir de la
relación con el campo y desplazamiento eléctrico. De esta manera:
1. Si es que el dieléctrico es lineal, es posible despejar el vector polarización fácilmente:
P = D − ε0 E = εE − ε0 E = (ε − ε0 )E

(10)

De ahora en adelante, se podrá utilizar esta fórmula libremente.

2. Solo quedaría reemplazar por el = ε” y = E” respectivos, los cuales dependerán únicamente
del lugar en donde se requiera calcular. Se hace énfasis en que = E” será el campo
en donde se localice el dieléctrico y, además, se desprende que el vector polarización
poseerá la misma componente que el campo eléctrico.
b) = σP (x) = P(x) · n̂(x) r=a ”: en esta parte se deberá calcular la densidad de carga de
polarización superficial en una superficie arbitraria = a”. Para ello:
1. Se debe distinguir el lugar en donde se requiere calcular la densidad superficial.
2. Luego, se debe identificar el campo eléctrico próximo a tal superficie y el cual
contiene al dieléctrico. Se calcula el vector polarización y simplemente se reemplaza.
3. ¿Cómo se determina el vector normal? Este será un vector ortogonal a la superficie
en cuestión y apuntará hacia afuera del dieléctrico.
4. Por último, se reemplaza todo en la expresión y se evalúa en el = punto” en donde se
ubica la superficie. Recuerden también que el producto punto de dos coordenadas
idénticas es igual a 1.
⃗ · P(x) ”: en esta parte se deberá calcular la densidad de carga de polarc) = ρP (x) = −∇
ización volumétrica en el lugar en donde se encuentra el dieléctrico. Para ello:
1. Se debe distinguir el lugar en donde se requiere calcular la densidad volumétrica.
2. Luego, se debe identificar el campo eléctrico que existe en esa zona y el cual contiene
al dieléctrico.
3. Se calcula el vector polarización, se reemplaza y se aplica la divergencia. En este
punto tengan cuidado, pues la divergencia dependerá de las coordenadas que se
estén utilizando.

---

### Página 4

1.5

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

1.6

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
aspectos revelantes se resumen en la tabla del Anexo ??.
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

### Página 5

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

### Página 6

1.6.1

“Problemas Resueltos de Electromagnetismo”, 7.11, Rodrigo Chi

Dos condensadores cilíndricos de radio interior a y exterior 3a, y largo L (muy largo),
han sido llenados con dos materiales dieléctricos ε1 y ε2 de distinta forma. Si los condensadores son conectados de la forma que se indica en la figura, determine la capacidad
equivalente entre los puntos A y B.

Figura 1. Esquema sobre los condensadores cilíndricos.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la capacitancia de la configuración, la cual puede ser vista como dos capacitores conectados en serie (i.e por ambos circula la misma corriente):
N

X 1
=
Ceq
Ci
i

Para ello, es necesario solo conocer el campo y potencial eléctrico que se encuentra en medio de
los lugares que contienen cargas opuestas pero de igual magnitud (i.e a < r < 3a para ambos
casos). Como se está hablando de un cilindro infinito y de materiales dieléctricos, es posible
aplicar Ley de Gauss Generalizada utilizando un cilindro coaxial de altura = L” y radio = r”
arbitrario:
I
D · ds = Qf

---

### Página 7

Ahora, el vector desplazamiento para un dieléctrico está dado por:

D = εE = ε0 κE
Como la permitividad no es constante en la misma sección transversal,
se debe cumplir la siguiente condición de borde para el capacitor inferior:

E1t = E2t
Luego, se puede utilizar la forma integral de la relación campo - potencial eléctrico:
Z rb
E · dl
V (rb ) − V (ra ) = −
ra

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: a < r < 2a y 2a < r < 3a.

Finalmente, se ocupa la fórmula que relaciona carga almacenada con capacitancia:
Q = C∆V
Se asignará de forma arbitraria una carga Q y −Q a las superficies r = a y r = 3a, respectivamente.
Se recuerda que esto no afectará al valor de la capacitancia, pues esta
depende únicamente de su geometría y no de la carga almacenada.

Paso 1: Ley de Gauss Generalizada (Superior) - Da<r<2a
En primer lugar, se calculará el desplazamiento eléctrico mediante la Ley de Gauss Generalizada
en la región a < r < 2a:
I
Da<r<2a · ds = Qf
Se conoce que el desplazamiento solo posee componente radial.
Además, la carga encerrada libre será la carga total del cilindro de radio a:

I
Da<r<2a ·

dS = Q

Ahora, la integral cerrada es en verdad la superficie del manto del cilindro gaussiano,
pues el flujo es ortogonal a este en todo momento:

Da<r<2a · 2πrL = Q
Da<r<2a =

Q
2πrL

(11)

Finalmente, y como el desplazamiento eléctrico es un vector, se aplica la componente radial:

Da<r<2a =

Q
r̂
2πrL

(12)

Paso 2: Campo Eléctrico Dieléctrico (Superior) - Ea<r<2a
Luego, el vector desplazamiento está dado por:
D = εE = ε0 κE
Es importante notar que se puede ocupar cualquiera de las dos expresiones anteriores.
Por conveniencia se utilizará la primera, pues por enunciado se entrega = ε”:

Da<r<2a = ε1 Ea<r<2a
Q
Ea<r<2a =
r̂
2πrLε1

(13)

Se usó = ε1 ” debido a que es la permitividad del dieléctrico que se encuentra en la región a < r < 2a.

---

### Página 8

Paso 3: Ley de Gauss Generalizada (Superior) - D2a<r<3a
En primer lugar, se calculará el desplazamiento eléctrico mediante la Ley de Gauss Generalizada
en la región 2a < r < 3a:
I
D2a<r<3a · ds = Qf
Se conoce que el desplazamiento solo posee componente radial.
Además, la carga encerrada libre será la carga total del cilindro de radio a:

I
D2a<r<3a ·

dS = Q

Ahora, la integral cerrada es en verdad la superficie del manto del cilindro gaussiano,
pues el flujo es ortogonal a este en todo momento:

D2a<r<3a · 2πrL = Q
Q
2πrL

D2a<r<3a =

(14)

Finalmente, y como el desplazamiento eléctrico es un vector, se aplica la componente radial:

D2a<r<3a =

Q
r̂
2πrL

(15)

Paso 4: Campo Eléctrico Dieléctricos Superior - E2a<r<3a
Luego, el vector desplazamiento está dado por:
D = εE = ε0 κE
Es importante notar que se puede ocupar cualquiera de las dos expresiones anteriores.
Por conveniencia se utilizará la primera, pues por enunciado se entrega = ε”:

D2a<r<3a = ε1 E2a<r<3a
Q
E2a<r<3a =
r̂
2πrLε2

(16)

Se usó = ε2 ” debido a que es la permitividad del dieléctrico que se encuentra en la región 2a < r < 3a.

Paso 5: Potencial Eléctrico (Superior) - ∆V
Ahora, se calculará la diferencia de potencial eléctrico en la región a < r < 3a:
Z 3a
∆V = V (a) − V (3a) = −
Ea<r<3a · dl
a

Por propiedades de integrales se pueden invertir los límites, el campo varía a lo
largo de la trayectoria y la única componente en juego es la radial, por lo que:

Z 2a
∆V =
a

Q
dr +
2πrLε1
2a

Z 3a
2a
3a

Q
dr
2πrLε2

Q ln r
ln r
(
+
)
2πL ε1 a
ε2 2a
Q ln (2a) − ln (a) ln (3a) − ln (2a)
=
(
+
)
2πL
ε1
ε2
Q ln (2) ln (3/2)
=
(
+
)
2πL ε1
ε2
=

(17)

---

### Página 9

Paso 6: Capacitancia (Superior) - Csup
Por último, se ocupa la expresión que relaciona carga almacenada con capacitancia:
Csup =
=

Q
∆V
Q
ln (3/2)
Q ln (2)
2πL ( ε1 +
ε2 )

= ln (2)
ε1

(18)

2πL
+ ln (3/2)
ε2

Se debe notar que 2 > 1 ∧ 3/2 > 1, por lo que se cumple que Csup > 0.

Paso 7: Ley de Gauss Generalizada (Inferior) - Da<r<3a
En primer lugar, se calculará el desplazamiento eléctrico mediante la Ley de Gauss Generalizada
en la región a < r < 3a:
I
Da<r<3a · ds = Qf
Ahora, se deberá dividir la integral en dos partes, puesto que la
permitividad no es idéntica en la misma sección transversal
(pero sí el campo eléctrico por condición de borde):

I

I
Dizq · dsizq +

Dder · dsder = Qf

Se conoce que el desplazamiento solo posee componente radial.
Además, la carga encerrada libre será la carga total de la esfera de radio a:

I
Dizq ·

I
dSizq + Dder ·

dSder = Q

Ahora, cada una de las integrales cerradas son en verdad la mitad de la superficie
del manto del cilindro gaussiano, pues el flujo es ortogonal a este en todo momento:

Dizq · πrL + Dder · πrL = Q
Q
Dizq + Dder =
πrL
Paso 8: Campo Eléctrico Dieléctrico (Inferior) - Ea<r<3a
Luego, el vector desplazamiento está dado por:
D = εE = ε0 κE
Es importante notar que se puede ocupar cualquiera de las dos expresiones anteriores.
Por conveniencia se utilizará la primera, pues por enunciado se entrega = ε”.
Además, y por condición de borde, el campo eléctrico debe ser idéntico para ambos casos:

(19)

---

### Página 10

Q
πrL
Q
εizq Eizq + εder Eder =
πrL
Q
ε1 E + ε 2 E =
πrL
Q
E(ε1 + ε2 ) =
πrL
Dizq + Dder =

E=

Q
πrL(ε1 + ε2 )

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

Ea<r<3a =

Q
r̂
πrL(ε1 + ε2 )

(20)

Se usó = ε1 ” debido a que es la permitividad que se encuentra en la región a < r < 3a (izquierda),
mientras que = ε2 ” debido a que es la permitividad que se encuentra en la región a < r < 3a (derecha).

Paso 9: Potencial Eléctrico (Inferior) - ∆V
Ahora, se calculará la diferencia de potencial eléctrico en la región a < r < 3a:
Z 3a
∆V = V (a) − V (3a) = −
Ea<r<3a · dl
a

Por propiedades de integrales se pueden invertir los límites, el campo varía a lo
largo de la trayectoria y la única componente en juego es la radial, por lo que:

Z 3a
∆V =
a

Q
dr
πrL(ε1 + ε2 )

3a
Q
(ln r)
πL(ε1 + ε2 )
a
Q
(ln (3a) − ln (a))
=
πL(ε1 + ε2 )
Q
=
ln (3)
πL(ε1 + ε2 )

=

(21)

Paso 10: Capacitancia (Inferior) - Cinf
Finalmente, se ocupa la expresión que relaciona carga almacenada con la capacitancia:
Cinf =
=
=

Q
∆V
Q
Q
πL(ε1 +ε2 ) ln (3)

πL(ε1 + ε2 )
ln (3)

Se debe notar que 3 > 1, por lo que se cumple que Cinf > 0.

(22)

---

### Página 11

Paso 11: Capacitancia Equivalente - Ceq
Por último, la configuración puede ser vista como dos capacitores conectados en serie:
=
+
Ceq
Cinf
Csup
1 −1
Ceq = (
)
+
Cinf
Csup
ln (3)
1 ln (2) ln (3/2) −1
=(
+
))
+
(
πL(ε1 + ε2 ) 2πL ε1
ε2
2πL
= 2 ln (3) ln (2) ln (3/2)
ε1 +ε2 + ε1 +
ε2

(23)

---

### Página 12

1.6.2

“Problemas Resueltos de Electromagnetismo”, 17.7, Rodrigo Chi

Una esfera dieléctrica de radio b y permitividad de carga ε contienen en un interior una
densidad de carga libre:

ρ(r) =

ρ0 r si 0 < r < b
si r > b

a) ¿En qué casos el vector polarización es nulo? Justifique su respuesta.
b) Determine el vector polarización en todo el espacio.
c) Calcule la carga de polarización en la superficie r = b.
d) Calcule la carga de polarización volumétrica en todo el espacio.

Solución a), b), c) y d)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el valor de la densidad de carga de polarización volumétrica y superficial
en las zonas donde existan. El dieléctrico solo toca la superficie r = b, por lo que se debe
observar esa interfaz a la hora de calcular σP , mientras que ρP solo se encontrará en donde el
dieléctrico esté presente (i.e r < b). Luego, se debe utilizar que:
σP (x) = P(x) · n̂(x)
r=b

⃗ · P(x)
ρP (x) = −∇
De aquí se nota que se necesita el vector polarización, el cual está dado por:

P(x) = (ε − ε0 )E(x)
Como se está hablando de una esfera y de materiales dieléctricos, es posible aplicar Ley de
Gauss Generalizada utilizando una esfera concéntrica de radio = r” arbitrario:
I
D · ds = Qf
Ahora, el vector desplazamiento para un dieléctrico está dado por:

D = εE = ε0 κE
La densidad de carga del cilindro no es uniforme,
por lo que se tendrá que utilizar la definición de carga:

ZZZ
Q=

ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: 0 < r < b, y r > b.

---

### Página 13

Paso 1: Ley de Gauss Generalizada - D0<r<b
En primer lugar, se calculará el desplazamiento eléctrico mediante la Ley de Gauss Generalizada
en la región 0 < r < b:
I
D0<r<b · ds = Qf
Como es una esfera, el campo solo poseerá componente radial.
Además, la carga encerrada libre estará determinada por una integral triple en esféricas:

RRR

V ρ dV

I
D0<r<b ·

dS =

ε0

Como la densidad de carga volumétrica de la esfera no es uniforme,
no se puede tratar como una constante y es necesario integrar.
Ahora, la integral cerrada es en verdad la superficie de la esfera
gaussiana, pues el flujo es ortogonal a este en todo momento:

RRR

V ρ dV

D0<r<b · 4πr =

ε0

La integral de volumen se refiere al volumen
encerrado por la esfera gaussiana de radio = r”.
En este caso, sería parte del volumen de la esfera con carga:

Z 2π Z π Z r

D0<r<b · 4πr =

ρ0 r · r2 sin θdrdθdϕ

ρ0 r4
D0<r<b · 4πr2 = 2 · 2π ·
ρ0 r2
D0<r<b =
Finalmente, y como el desplazamiento eléctrico es un vector, se aplica la componente radial:

D0<r<b =

ρ0 r2
r̂

(24)

Paso 2: Campo Eléctrico Dieléctrico - E0<r<b
Luego, el vector desplazamiento en la región 0 < r < b está dado por:
D = εE = ε0 κE
Es importante notar que se puede ocupar cualquiera de las dos expresiones anteriores.
Por conveniencia se utilizará la primera, pues por enunciado se entrega = ε”:

D0<r<b = εE0<r<b
ρ0 r2
E0<r<b =
r̂
4ε

(25)

Se usó = ε” debido a que es la permitividad del dieléctrico que se encuentra en la región 0 < r < b.

---

### Página 14

Paso 3: Vector Polarización - P0<r<b
Ahora, se calculará el vector polarización en la región 0 < r < b:
P0<r<b = (ε − ε0 )E0<r<b
(ε − ε0 )ρ0 r2
=
r̂
4ε

(26)

Se usó = ε” debido a que es la permitividad del dieléctrico que se encuentra en la región 0 < r < b.

Paso 4: Densidad Carga Polarización Superficial - σPb
Posteriormente, se utiliza la expresión de densidad de carga de polarización superficial evaluada
en el límite r = b:
σPb = P0<r<b · n̂
r=b

En este caso n̂ apunta hacia afuera de forma radial (i.e n̂ = r̂), puesto que se dirige
hacia el exterior del dieléctrico. Reemplazando el vector polarización se obtiene que:

σ Pb =

(ε − ε0 )ρ0 r2
r̂ · r̂
4ε
r=b

(ε − ε0 )ρ0 b2
=
4ε

(27)

Paso 5: Densidad Carga Polarización Volumétrica - ρP0<r<b
Finalmente, se utiliza la expresión de densidad de carga de polarización volumétrica en la
región 0 < r < b, considerando que se está trabajando en coordenadas esféricas y que el vector
polarización solo posee componente radial:
⃗ · P0<r<b
ρP0<r<b = −∇
1 δ
1 δ
1 δPϕ̂
= −( 2 (r2 Pr̂ ) +
(sin θPθ̂ ) +
)
r δr
r sin θ δθ
r sin θ δϕ
1 δ
(ε − ε0 )ρ0 r2
1 δ
1 δ0
= −( 2 (r2 ·
)+
(sin θ · 0) +
)
r δr
4ε
r sin θ δθ
r sin θ δϕ
(ε − ε0 )ρ0 δ 4
=−
(r )
4εr2 δr
(ε − ε0 )ρ0
=−
· 4r3
4εr2
(ε − ε0 )ρ0 r
=−
ε

(28)

Nota: El vector polarización solo tiene sentido cuando se habla de algún material
dieléctrico, por lo que la región propicia para calcularlo es en donde este se ubica.
