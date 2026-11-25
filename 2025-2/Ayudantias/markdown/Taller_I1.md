---
title: "Taller I1"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Enunciado_Taller_I1.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Solución_Taller_I1.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Taller I1

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Taller I1
23 de Septiembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

0.0.1

“I1 2021-2”, Problema 2, Facultad de Física

El alambre de la figura es infinito y tiene una densidad de carga lineal constante λ.
Encuentre el campo eléctrico en el punto O.

Figura 1. Esquema sobre el alambre.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en el punto O, el cual puede ser expresado como la suma
de los campos generados por los 3 segmentos mediante principio de superposición. Como la
figura no posee ninguna simetría apta para la Ley de Gauss, se aplicará la definición de campo
eléctrico:
Z
(x − x ′ )
E(x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |3
Se nota que se usa la integral simple en virtud de la naturaleza del problema,
puesto que el alambre se puede describir con solo una componente variable en coordenadas cilíndricas.

---

### Página 2

0.0.2

“Ejercicios Teoría Electromagnética ”, 5.6.9, Fabián Cádiz

Un alambre cuya densidad lineal de carga es λ se extiende en el eje z desde z = −d
hasta z = d. Despreciando efectos gravitacionales:
a) Calcule el potencial en un punto z > d sobre el eje del alambre.
b) ¿Cuál es el cambio de energía potencial de un electrón si se mueve de z = 4d hasta
z = 3d?
c) Si el electrón parte del reposo desde z = 4d, ¿cuál es la velocidad en z = 3d?

Figura 2. Esquema sobre el alambre.

Solución a)
Se pide determinar el potencial eléctrico en un punto z > d sobre el eje del alambre. Como
la figura no posen ninguna simetría apta para la Ley de Gauss, se aplicará la definición de
potencial eléctrico para distribuciones continuas de carga:
Z
V (x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Se nota que se usa la integral simple en virtud de la naturaleza del problema, puesto que el
alambre se puede describir con solo una componente variable en coordenadas cartesianas.

---

### Página 3

Solución b)
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

---

### Página 4

0.0.3

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

### Página 5

Solución b) y c)
Se pide determinar las cargas en las superficies interior y exterior del cascarón (i.e r = R1 y
r = R2 ). Como se está hablando de un cilindro, se deberá aplicar estratégicamente Ley de
Gauss utilizando una cilindro coaxial de altura = L” y radio = r” arbitrario:
I
⃗ · d⃗s = Qenc
E
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
E
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
E
R1

Solución g)
Paso Único: Capacitancia - C
Se pide determinar la capacitancia de la configuración propuesta. Para ello, es necesario solo
conocer el campo y potencial eléctrico que se encuentra en medio de los lugares que contienen
cargas de igual magnitud, pero opuestas (i.e R0 < r < R1 ). Finalmente, se ocupa la expresión
que relaciona carga almacenada con capacitancia:
Q = C∆V

---

### Página 6

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

Solución Taller I1
23 de Septiembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

0.0.1

“I1 2021-2”, Problema 2, Facultad de Física

El alambre de la figura es infinito y tiene una densidad de carga lineal constante λ.
Encuentre el campo eléctrico en el punto O.

Figura 1. Esquema sobre el alambre.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en el punto O, el cual puede ser expresado como la suma
de los campos generados por los 3 segmentos mediante principio de superposición. Como la
figura no posee ninguna simetría apta para la Ley de Gauss, se aplicará la definición de campo
eléctrico:
Z
(x − x ′ )
E(x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |3
Se nota que se usa la integral simple en virtud de la naturaleza del problema,
puesto que el alambre se puede describir con solo una componente variable en coordenadas cilíndricas.

Paso 1: Campo Eléctrico Segmento Superior - E1
Desde ahora en adelante, nuestro sistema de referencia será el punto O y se utilizarán coordenadas cartesianas por la geometría del ejercicio. Se recuerda que el vector r parte en el origen
y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

---

### Página 2

Luego, el vector r ′ parte en el origen y recorre todo el cuerpo con carga:
r ′ = xx̂ + Rŷ,

x ∈ [−∞, 0]

Donde = R” es el radio de la semicircunferencia.

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = −(xx̂ + Rŷ)
Calculando el módulo del vector anterior:

p
|r − r ′ | = x2 + R2
Considerando que la densidad de carga es lineal y que la única componente variable para el
alambre es x:
dq(x ′ ) = λ(x ′ ) dl′ = λ dx
Para llegar a lo anterior se utilizó el diferencial de línea para cartesianas,
omitiendo las componentes constantes y el sentido vectorial.

Finalmente, se utiliza la definición de campo eléctrico considerando los límites de integración
propuestos con anterioridad:
Z
(x − x ′ )
λ(x ′ ) dl′
E1 =
4πε0 L |x − x ′ |3
Z 0
−(xx̂ + Rŷ)
=
λ dx
4πε0 −∞ (x2 + R2 )3/2
Paso 2: Campo Eléctrico Segmento Central - E2
Desde ahora en adelante, nuestro sistema de referencia será el punto O y se utilizarán coordenadas cilíndricas por la geometría del ejercicio. Se recuerda que el vector r parte en el origen
y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ parte en el origen y recorre todo el cuerpo con carga:
π π
r ′ = Rr̂, θ ∈ [− , [
2 2
Donde = R” es el radio de la semicircunferencia y = r̂” la componente radial en coordenadas cilíndricas.

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = −Rr̂
Calculando el módulo del vector anterior:

|r − r ′ | = R
Considerando que la densidad de carga es lineal y que la única componente variable para el
alambre es θ:
dq(x ′ ) = λ(x ′ ) dl′ = λ · R dθ

---

### Página 3

Para llegar a lo anterior se utilizó el diferencial de línea para cilíndricas,
omitiendo las componentes constantes y el sentido vectorial.

Finalmente, se utiliza la definición de campo eléctrico considerando los límites de integración
propuestos con anterioridad:
Z
(x − x ′ )
E2 =
λ(x ′ ) dl′
4πε0 L |x − x ′ |3
Z π
2 −Rr̂
=
λ · R dθ
4πε0 − π R3
Z π
2 −λr̂
dθ
=
4πε0 − π R
Z π
−λ
=
r̂ dθ
4πε0 R − π

Utilizando que r̂ = cos θ x̂ + sin θ ŷ:

E2 =

−λ
4πε0 R

Z π

cos θ x̂ + sin θ ŷ dθ

− π2

Z π
Z π
−λ
·(
=
cos θ x̂ dθ +
sin θ ŷ dθ)
4πε0 R
−π
−π

π

π

−λ
· ( (sin θ x̂)
+ (− cos θ ŷ)
)
=
4πε0 R
−π
−π

−λ
π
π
π
π
=
· ((sin − sin (− )) x̂ − (cos − cos (− )) ŷ)
4πε0 R
−λ
=
· 2 x̂
4πε0 R
−λ
=
x̂
2πε0 R
Paso 3: Campo Eléctrico Segmento Inferior - E3
Desde ahora en adelante, nuestro sistema de referencia será el punto O y se utilizarán coordenadas cartesianas por la geometría del ejercicio. Se recuerda que el vector r parte en el origen
y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ parte en el origen y recorre todo el cuerpo con carga:
r ′ = xx̂ − Rŷ,

x ∈ [−∞, 0]

Donde = R” es el radio de la semicircunferencia.

Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = −(xx̂ − Rŷ)

---

### Página 4

Calculando el módulo del vector anterior:

p
|r − r ′ | = x2 + R2
Considerando que la densidad de carga es lineal y que la única componente variable para el
alambre es x:
dq(x ′ ) = λ(x ′ ) dl′ = λ dx
Para llegar a lo anterior se utilizó el diferencial de línea para cartesianas,
omitiendo las componentes constantes y el sentido vectorial.

Finalmente, se utiliza la definición de campo eléctrico considerando los límites de integración
propuestos con anterioridad:
Z
(x − x ′ )
λ(x ′ ) dl′
E3 =
4πε0 L |x − x ′ |3
Z 0
−(xx̂ − Rŷ)
=
λ dx
4πε0 −∞ (x2 + R2 )3/2
Paso 4: Campo Eléctrico - Principio de Superposición E
Finalmente, y mediante el principio de superposición, el campo eléctrico en el punto O será la
suma de los campos generados por los distintos segmentos:
E = E1 + E2 + E3
Z 0
Z 0
−(xx̂ + Rŷ)
−(xx̂ − Rŷ)
−λ
=
x̂ +
λ dx +
λ dx
3/2
4πε0 −∞ (x + R )
2πε0 R
4πε0 −∞ (x2 + R2 )3/2
Z 0
−2xx̂
−λ
=
λ dx +
x̂
3/2
4πε0 −∞ (x + R )
2πε0 R
Z
x
−2λ 0
−λ
x̂
=
dx x̂ +
4πε0 −∞ (x2 + R2 )3/2
2πε0 R
Z 2
−2λ R
−λ
=
dβ x̂ +
x̂
3/2
4πε0 ∞ 2β
2πε0 R

−2 R
−λ
−λ
· (√ )
x̂
=
x̂ +
4πε0
2πε0 R
β ∞
−λ
−2
−2
−λ
=
· (√
− √ ) x̂ +
x̂
4πε0
2πε0 R
∞
R
−λ
−2
−λ
=
·√
x̂ +
x̂
4πε0
2πε0 R
R
λ
−λ
=
x̂ +
x̂
2πε0 R
2πε0 R
=0
Notar que se realizó un cambio de variable β = x2 + R
√ → dβ = 2x dx.
También, y como R > 0, se puede considerar que R2 = |R| = R.

---

### Página 5

Nota: El tratamiento de las integrales también se puede realizar observando la simetría
de la figura, con el objetivo de obviar la componente ŷ.

---

### Página 6

0.0.2

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
Z
V (x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Se nota que se usa la integral simple en virtud de la naturaleza del problema, puesto que el
alambre se puede describir con solo una componente variable en coordenadas cartesianas.

---

### Página 7

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

|r − r ′ | = z + z ′
Considerando que la densidad de carga es lineal y que la única componente variable para el
alambre es z:
dq = λ dz ′
Para llegar a lo anterior se utilizó el diferencial de línea para cartesianas,
omitiendo las componentes constantes y el sentido vectorial.

Paso 3: Potencial Eléctrico - Alambre
Finalmente, se utiliza la definición de potencial eléctrico para el alambre considerando los
límites de integración propuestos con anterioridad:
Z
V =
λ(x ′ ) dl′
4πε0 L |x − x ′ |
Z d
=
· λ dz ′
4πε0 −d (z + z ′ )
Z z+d
λ
=
dβ
4πε0 z−d β
(1)
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
Notar que se realizó un cambio de variable β = z + z ′ → dβ = dz ′ .

---

### Página 8

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

(2)

---

### Página 9

0.0.3

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

### Página 10

se puede tratar como una constante y sale de la integral.
Su largo es L y su carga total es Q:

Z L
dz

Q=λ

Q=λ·L
Q
λ=
L

(3)

Solución b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar las cargas en las superficies interior y exterior del cascarón (i.e r = R1 y
r = R2 ). Como se está hablando de un cilindro, se deberá aplicar estratégicamente Ley de
Gauss utilizando una cilindro coaxial de altura = L” y radio = r” arbitrario:
I
⃗ · d⃗s = Qenc
E
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
I
⃗ R <r<R · dS
⃗ = Qenc
E
ε0
El cascarón cilíndrico es conductor, por lo que el campo eléctrico
en su interior será nulo y su carga solo se ubicará en su superficie:

⃗ R <r<R = 0
E

(4)

Con lo anterior, la carga encerrada (en r < R2 ) debe ser igual a 0:

Qenc = 0
Q + Q R1 = 0
QR1 = −Q

(5)

Paso 2: Densidad Carga Superficial - σR1
Así, la carga en la superficie r = R1 estará determinada por una integral doble en cilíndricas:
ZZ
QR1 =
σ dS
S

---

### Página 11

Como la densidad de carga del cascarón es uniforme,
se puede tratar como una constante y sale de la integral:

Z L Z 2π
−Q = σR1

R1 dθdz

−Q = σR1 · 2πR1 L
Q
σ R1 = −
2πR1 L

(6)

Paso 4: Carga Superficial - QR2
El cascarón cilíndrico ubicado entre R1 y R2 está cargado con carga −Q y es conductor, es
decir, su carga solo se ubicará en sus superficies. Mediante el principio de conservación de
carga se obtiene que:
QR1 + QR2 = −Q
−Q + QR2 = −Q
QR2 = 0

(7)

Paso 5: Densidad Carga Superficial - σR2
Así, la carga en la superficie r = R2 estará determinada por una integral doble en cilíndricas:
ZZ
Q=
σ dS
S

Como su carga total es 0, su densidad de carga es nula:

σR2 = 0

(8)

Nota: No es estrictamente necesario realizar la integral de superficie para determinar
la densidad de carga. Como la densidad de carga es uniforme, basta con saber que se
refería al área del manto de un cilindro de altura L y radio Ri , con i = 1, 2.

Solución e)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en todo el espacio. Como se está hablando de un alambre
y cilindro, es posible aplicar Ley de Gauss utilizando un cilindro coaxial de altura = L” y de
radio = r” arbitrario:
I
⃗ · d⃗s = Qenc
E
ϵ0
S
Además, y como se presentan = cortes visuales” relacionados con un cambio en la
densidad de carga, se debe trabajar por intervalos: r < R1 , R1 < r < R2 y r > R2 .

---

### Página 12

⃗ r<R
Paso 1: Ley de Gauss - E
En primer lugar, se calculará el campo eléctrico mediante la Ley de Gauss en la región r < R0 :
I
⃗ = Qenc
⃗ r<R · dS
E
ε0
El alambre es conductor, por lo que el campo eléctrico en su
interior será nulo y su carga solo se ubicará en su superficie:

⃗ r<R = 0
E

(9)

⃗ R <r<R
Paso 2: Ley de Gauss - E
Ahora, se calculará el campo eléctrico mediante la Ley de Gauss en la región R0 < r < R1 :
I
⃗ R <r<R · dS
⃗ = Qenc
E
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada será la carga total del alambre:

I
ER0 <r<R1 ·

dS =

Q
ε0

Ahora, la integral cerrada es en verdad la superficie del manto del cilindro gaussiano,
pues el flujo es ortogonal a esta en todo momento:

ER0 <r<R1 · 2πrL =

Q
ε0

Q
ER0 <r<R1 =
2πrLε0

(10)

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

⃗ R <r<R =
E

Q
r̂
2πrLε0

(11)

⃗ r>R
Paso 4: Ley de Gauss - E
Por último, se calculará el campo eléctrico mediante la Ley de Gauss en la región r > R2 :
I
⃗ r>R · dS
⃗ = Qenc
E
ε0
Se conoce que el campo solo posee componente radial.
Además, la carga encerrada será la carga total de la configuración:

I
Er>R2 ·

dS =

Q−Q
=0
ε0

Como la configuración es eléctricamente neutra se obtiene que:

⃗ r>R = 0
E

(12)

---

### Página 13

Solución f )
Paso Único: Potencial Eléctrico - ∆V
Se pide determinar la diferencia de potencial que se encuentra entre el alambre y el cilindro
(i.e R0 < r < R1 ), por lo que se utilizará la forma integral de la relación campo - potencial
électrico:
Z R0
⃗ R <r<R · d⃗l
∆V = V (R0 ) − V (R1 ) = −
E
R1

Luego, por propiedades de integrales se pueden invertir los límites
y la única componente en juego es la radial, por lo que:

Z R1
∆V =
R0

Q
dr
2πrLε0

R1
Q
(ln r)
2πLε0
R0
Q
(ln R1 − ln R0 )
=
2πLε0
 
Q
R1
=
ln
2πLε0
R0

=

(13)

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

Q
∆V
Q


Q
R1
2πLε0 ln R0



(14)

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

### Página 14

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
E

(15)
(16)

Finalmente, se ocupa la fórmula que relaciona carga almacenada con capacitancia:

C′ =
=

=

Q
∆V
2Q
 
2Q
R1
ln
2πLε0
R0

(17)

2πLε0
 
ln R
R0

Se debe notar que R1 > R0 , por lo que se cumple que C > 0.
Luego, se concluye que la nueva capacitancia es igual a la anterior (i.e C = C ′ ).

Nota: Se puedo haber realizado todo el ejercicio nuevamente con el cambio propuesto,
pero supone algo demoroso. Luego, basta con saber que la capacitancia nace a partir
de la geometría de la figura y no depende de la carga almacenada.
