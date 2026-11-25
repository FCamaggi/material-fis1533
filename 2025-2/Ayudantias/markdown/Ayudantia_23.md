---
title: "Ayudantia 23"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_23_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_23_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 23

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Ayudantía 23
04 de Noviembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

0.0.1

“Control 2 2015-1”, Problema 2, Departamento de Física

Se tiene un condensador con tres placas paralelas de área A como se indica en la figura.
Las primeras están separadas una distancia L entre ellas y las últimas lo están una
distancia d. Además, entre las placas se disponen dos materiales, el primero tiene una
conductividad g1 , mientras que el segundo tiene una conductividad g2 . El sistema se
encuentra en estado estacionario, conectado a un generador que establece una diferencia
de potencial V0 entre las placas.
a) Determine el(los) campo(s) eléctrico(s) entre las placas. ¿Es el mismo en ambos
medios?
b) Determine la(s) densidad(es) de corriente volumétricas que circula(n) entre las
placas. ¿Es la misma en ambos medios?
c) Calcule la intensidad de corriente total que circula entre las placas.
d) Determine la resistencia del sistema.
e) ¿Qué pasaría si el generador se desconecta? Explique cualitativamente.

Figura 1. Esquema sobre el condensador.

---

### Página 2

Solución a), b), c) y d)
Se pide determinar la resistencia del sistema (i.e 0 < z < L + d). En primer lugar, la intensidad
de corriente estará dada por:
ZZ
I=
J(x) · dS(x)
S

Como la conductividad no es constante en distintas secciones
transversales, se debe cumplir la siguiente condición de borde:

J1n = J2n
Ahora, la densidad de corriente se puede calcular como:

J(x) = σE(x)
Luego, se puede utilizar la forma integral de la relación campo - potencial:
Z rb
V (rb ) − V (ra ) = −
E · dl
ra

Finalmente, la resistencia se puede calcular utilizando la Ley de Ohm Macroscópica:
V = IR

---

### Página 3

0.0.2

“Ejercicios Teoría Electromagnética ”, 11.5.1, Fabián Cádiz

En el circuito de la figura, suponga que el interruptor ha estado abierto por un tiempo
muy largo y en t = 0 se cierra.
a) ¿Cuál es la constante de tiempo antes de que se cerrara el interruptor?
b) ¿Cuál es la constante de tiempo después de que se cerrara el interruptor?
c) Encuentre la corriente a través del interruptor como función del tiempo una vez
que el interruptor se ha cerrado.

Figura 2. Esquema sobre el circuito RC.

Solución a) y b)
Se pide determinar la constante de tiempo antes de que se cierre el interruptor, por lo que será
necesario calcular el voltaje/intensidad del capacitor en función del tiempo. Los pasos a seguir
para llegar y resolver la EDO se detallan en el resumen.

Solución c)
Se pide determinar la intensidad la corriente a través del interruptor cerrado como función del
tiempo. A simple vista, se puede observar que por este circulará la suma de las corrientes I1
e I2 (según nuestra definición). Luego, se debe determinar I1 e I2 mediante la expresión de la
intensidad en el capacitor a partir de la diferencia de potencial presente en él:
Ic = C

dVC
dt

---

### Página 4

0.0.3

“I2 2021-2”, Problema 3, Facultad de Física

Determine el campo magnético en el punto O debido a la corriente constante I que
circula por un circuito formado por dos segmentos verticales semi-infinitos y un segmento
horizontal de largo 2a, tal como muestra la figura.

Figura 3. Circuito en estudio.

#### Solución
Se pide determinar el campo magnético en el punto O, el cual puede ser expresado como la
suma de los campos generados por los 3 segmentos . Como las figuras no poseen ninguna
simetría apta para la Ley de Ampére, solo queda aplicar campo por definición:
Z
µ0
Idl × (x − x ′ )
B(x) =
4π L
|x − x ′ |3
Se nota que se usa la integral simple debido a la naturaleza del problema,
puesto que el alambre vive en una dimensión.

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 23
04 de Noviembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

0.0.1

“Control 2 2015-1”, Problema 2, Departamento de Física

Se tiene un condensador con tres placas paralelas de área A como se indica en la figura.
Las primeras están separadas una distancia L entre ellas y las últimas lo están una
distancia d. Además, entre las placas se disponen dos materiales, el primero tiene una
conductividad g1 , mientras que el segundo tiene una conductividad g2 . El sistema se
encuentra en estado estacionario, conectado a un generador que establece una diferencia
de potencial V0 entre las placas.
a) Determine el(los) campo(s) eléctrico(s) entre las placas. ¿Es el mismo en ambos
medios?
b) Determine la(s) densidad(es) de corriente volumétricas que circula(n) entre las
placas. ¿Es la misma en ambos medios?
c) Calcule la intensidad de corriente total que circula entre las placas.
d) Determine la resistencia del sistema.
e) ¿Qué pasaría si el generador se desconecta? Explique cualitativamente.

Figura 1. Esquema sobre el condensador.

---

### Página 2

Solución a), b), c) y d)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la resistencia del sistema (i.e 0 < z < L + d). En primer lugar, la intensidad
de corriente estará dada por:
ZZ
I=
J(x) · dS(x)
S

Como la conductividad no es constante en distintas secciones
transversales, se debe cumplir la siguiente condición de borde:

J1n = J2n
Ahora, la densidad de corriente se puede calcular como:

J(x) = σE(x)
Luego, se puede utilizar la forma integral de la relación campo - potencial:
Z rb
V (rb ) − V (ra ) = −
E · dl
ra

Finalmente, la resistencia se puede calcular utilizando la Ley de Ohm Macroscópica:
V = IR → R =

V
I

Paso 1: Condición de Borde - J1n = J2n
En primer lugar, el sistema se encuentra en estado estacionario, es decir:
∇·J=0
Luego, y por la geometría del problema, se llega a que:

J = J ẑ
Gracias a la ecuación de continuidad, se concluye que la densidad de corriente es constante.
Imponiendo la condición de borde (i.e J1n = J2n ) en la región 0 < z < L + d:

J = J0<z<L = JL<z<L+d
Paso 2: Ley de Ohm Microscópica - E0<z<L
Ahora, y ocupando la Ley de Ohm Microscópica en la región 0 < z < L, se obtiene que:
J0<z<L
σ0<z<L
J
ẑ
g1

E0<z<L =

---

### Página 3

Paso 3: Ley de Ohm Microscópica - EL<z<L+d
Análogamente, y ocupando la Ley de Ohm Microscópica en la región L < z < L + d, se obtiene
que:
JL<z<L+d
σL<z<L+d
J
ẑ
g2

EL<z<L+d =

Paso 4: Potencial Eléctrico - ∆V
Como V0 = ∆V , se calculará la diferencia de potencial eléctrico entre z = 0 y z = d:
Z 0
E0<z<L+d · dl
V0 = V (0) − V (L + d) = −
L+d

Por propiedades de integrales se pueden invertir los límites
y la única componente en juego es la normal, por lo que dl = d⃗z:

Z L

Z L+d

V0 =

E0<z<L dz +
EL<z<L+d dz
L
Z L
Z L+d
J
J
V0 =
dz +
dz
g2
0 g1
L
J
J
V0 =
·L+
·d
g1
g2
J(dg1 + Lg2 )
V0 =
g1 + g2
V0 g1 g2
J=
dg1 + Lg2

Agregando la componente normal:

J=

V0 g1 g2
ẑ
dg1 + Lg2

(1)

Reemplazando en lo anterior, obtenemos que:

V0 g1 g2
ẑ
g1 (dg1 + Lg2 )
V0 g1 g2
EL<z<L+d =
ẑ
g2 (dg1 + Lg2 )
E0<z<L =

(2)
(3)

Paso 5: Intensidad de Corriente - Ieq
Notando que los medios se encuentran conectados en serie (i.e misma intensidad de corriente)
y utilizando la definición de intensidad de corriente en la región 0 < z < L + d:
ZZ
Ieq =
J(x) · dS(x)
S

---

### Página 4

Se conoce que J = J ẑ → E = E ẑ, por lo que se utilizará
el diferencial de superficie que contiene a “ẑ” en coordenadas cartesianas:

ZZ
J ẑ · dxdy ẑ
ZZ
V0 g1 g2
dxdy
·
dg1 + Lg2
S
V0 g1 g2
·A
dg1 + Lg2

Ieq =

S

Luego, se cumple que:

I1 = I2 =

V0 Ag1 g2
dg1 + Lg2

(4)

Paso 6: Ley de Ohm Macroscópica - Req
Finalmente, utilizando la Ley de Ohm Macroscópica en la región 0 < z < L + d se obtiene que:
Req =

Veq
Ieq
V0

= AV0 g1 g2

(5)

dg1 +Lg2

dg1 + Lg2
Ag1 g2

Solución e)
Paso Único: Efectos Desconexión Generador
En un comienzo, el generador estaba conectado y permitía la aparición de campos eléctricos
en la región 0 < z < L + d. Al desconectar el generador, la diferencia de potencial entre las
placas se vuelve nula, lo que implica necesariamente la descarga de las placas y, con ello, la
desaparición de los campos en tal región.

---

### Página 5

0.0.2

“Ejercicios Teoría Electromagnética ”, 11.5.1, Fabián Cádiz

En el circuito de la figura, suponga que el interruptor ha estado abierto por un tiempo
muy largo y en t = 0 se cierra.
a) ¿Cuál es la constante de tiempo antes de que se cerrara el interruptor?
b) ¿Cuál es la constante de tiempo después de que se cerrara el interruptor?
c) Encuentre la corriente a través del interruptor como función del tiempo una vez
que el interruptor se ha cerrado.

Figura 2. Esquema sobre el circuito RC.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio? - τ
Se pide determinar la constante de tiempo antes de que se cierre el interruptor, por lo que será
necesario calcular el voltaje/intensidad del capacitor en función del tiempo. Los pasos a seguir
para llegar y resolver la EDO se detallan en el resumen.
Paso 1: Condición Abierto y Ecuación Mallas - M1
Primero, se nombra de forma arbitraria la intensidad de la malla. Como es solo una, es bastante
simple:

---

### Página 6

Figura 3. Esquema sobre el circuito RC (antes del cierre).
Para armar las ecuaciones debemos observar una malla y recorrerla en el sentido otorgado.
Se sumará solo si se entra a fuentes de + a − y/o en aquellos voltajes de resistores (en caso
contrario se resta):
−ε + VR1 + VC + VR2 = 0
Luego, se debe realizar el reemplazo del voltaje en los resistores por Ley de Ohm, dejando positiva la
corriente que pasa por la malla observada y negativa la malla opuesta (en caso de haber):

−ε + IR1 + VC + IR2 = 0
Ahora, se observa que I también pasa por el capacitor y que este
C
se encuentra en proceso de carga, por lo que se aplica la expresión I = IC = C dV
dt :

−ε + CR1

dVC
dVC
+ VC + CR2
=0
dt
dt

(6)

Paso 2: Solución EDO - VC
La EDO se puede tratar mediante el método de separación de variables, por lo que a un lado
se dejarán las variables dependientes de VC y al otro las variables dependientes del tiempo y/o
constantes:
dVC
(R1 + R2 )
dt
dt
dVC
C(R1 + R2 )
ε − VC

−ε + VC = −C

Integrando a cada lado:

Z t

dt
t0 C(R1 + R2 )

Z VC
V0

dVC
ε − VC

Como es antes de que se cierre el circuito t ∈ ] − ∞, 0].
Además, el condensador inicialmente se encuentra descargado, por lo que V0 = 0:

Z t

dt
C(R
1 + R2 )

Z VC

dVC
ε − VC

Aplicando un cambio de variable al lado derecho α = ε − VC → dα = −dVC :

---

### Página 7

Z t

Z ε−VC
dt
dα
−
α
0 C(R1 + R2 )
ε
t
ε − VC
= − ln (
)
C(R1 + R2 )
ε

Aplicando exponencial a cada lado con el objetivo de despejar VC :

e

− C(R t+R )

ε − VC
ε

− C(R t+R )

VC (t) = ε(1 − e

)

(7)

Paso 3: Constante de Tiempo - τ
Al analizar la solución podremos notar que:
−

t
t
=−
→ τ = C(R1 + R2 )
τ
C(R1 + R2 )

(8)

Solución b)
Paso 0: ¿Cómo plantear el ejercicio? - τ
Se pide determinar la constante de tiempo después de que se cierre el interruptor, por lo que
será necesario calcular el voltaje/intensidad del capacitor en función del tiempo. Los pasos a
seguir para llegar y resolver la EDO se detallan en el resumen.
Paso 1: Condición Cerrado y Ecuación Mallas - M1 − M2
Primero, se nombran de forma arbitraria las intensidades de las mallas. Por simplicidad, se
tiene que:

Figura 4. Esquema sobre el circuito (después del cierre)
Para armar las ecuaciones debemos observar una malla y recorrerla en el sentido otorgado.
Se sumará solo si se entra a fuentes de + a − y/o en aquellos voltajes de resistores (en caso
contrario se resta):
M1 → −ε + VR1 = 0
M2 → −VC + VR2 = 0

---

### Página 8

Luego, se debe realizar el reemplazo del voltaje en los resistores por Ley de Ohm, dejando positiva la
corriente que pasa por la malla observada y negativa la malla opuesta (en caso de haber):

M1 → −ε + I1 R1 = 0
M2 → −VC + I2 R2 = 0
Ahora, se observa que I2 también pasa por el capacitor y que este
C
se encuentra en proceso de descarga, por lo que se aplica la expresión I2 = IC = −C dV
dt :

M1 → −ε + I1 R1 = 0
dVC
M2 → −VC − CR2
=0
dt

(9)
(10)

Paso 2: Solución EDO - VC
La EDO asociada a la segunda expresión se puede tratar mediante el método de separación
de variables, por lo que a un lado se dejarán las variables dependientes de VC y al otro las
variables dependientes del tiempo y/o constantes:
dVC
dt
dt
dVC
−
CR2
VC

VC = −CR2

Integrando a cada lado:

Z t

dt
−
CR2
t0

Z VC
V0

dVC
VC

Como es antes de que se cierre el circuito t ∈ [0, ∞[. Además, el condensador se encontrará a cierto
voltaje inicial V (0) = V0 = ε dado por el límite de la expresión calculada en a):

Z t

Z VC
dVC
dt
−
CR2
VC
ε
t
VC
−
= ln ( )
CR2
ε

Aplicando exponencial a cada lado con el objetivo de despejar VC :

VC (t) = εe

t
− CR

(11)

Paso 3: Constante de Tiempo - τ
Al analizar la solución podremos notar que:
−

t
t
=−
→ τ = CR2
τ
CR2

(12)

---

### Página 9

Solución c)
Paso 0: ¿Cómo plantear el ejercicio? - I
Se pide determinar la intensidad la corriente a través del interruptor cerrado como función del
tiempo. A simple vista, se puede observar que por este circulará la suma de las corrientes I1
e I2 (según nuestra definición). Luego, se debe determinar I1 e I2 mediante la expresión de la
intensidad en el capacitor a partir de la diferencia de potencial presente en él:
Ic = C

dVC
dt

(13)

ε
R1

(14)

Paso 1: Intensidad de Corriente - I1
Despejando I1 de la primera ecuación de malla:
∴ I1 =
Paso 2: Intensidad de Corriente - I2
Utilizando la expresión para corriente en capacitores en proceso de descarga:
I2 = −C

dVC
− t
= −C · εe CR2 · −
dt
CR2
ε − CRt
∴ I2 =
e
R2

(15)

Paso 3: Suma de Corrientes - I
Finalmente, la corriente total que pasa por el interruptor sería la suma de ambas:
ε
ε − CRt
∴ I(t) = I1 + I2 =
+
e
R1 R2

(16)

---

### Página 10

0.0.3

“I2 2021-2”, Problema 3, Facultad de Física

Determine el campo magnético en el punto O debido a la corriente constante I que
circula por un circuito formado por dos segmentos verticales semi-infinitos y un segmento
horizontal de largo 2a, tal como muestra la figura.

Figura 5. Circuito en estudio.

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo magnético en el punto O, el cual puede ser expresado como la
suma de los campos generados por los 3 segmentos . Como las figuras no poseen ninguna
simetría apta para la Ley de Ampére, solo queda aplicar campo por definición:
Z
µ0
Idl × (x − x ′ )
B(x) =
4π L
|x − x ′ |3
Se nota que se usa la integral simple debido a la naturaleza del problema,
puesto que el alambre vive en una dimensión.

Paso 1: Campo Segmento 1 - B1
Desde ahora en adelante, nuestro sistema de referencia será el punto = O” y se utilizarán
coordenadas cartesianas por la geometría del ejercicio. Se recuerda que el vector r parte en el
origen y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ parte en el origen y recorre todo el cuerpo con corriente:
r ′ = −ax̂ + y ŷ,

y ∈ [∞, b]

---

### Página 11

Se debe hacer énfasis en cómo es el sentido de la corriente.

Se siguen determinando componentes de la integral:
r − r ′ = −(−ax̂ + y ŷ)
Calculando el módulo del vector anterior:

|r − r ′ | =

p
a2 + y 2

Usando los resultados anteriores:
Idl × (r − r ′ ) = I dy ŷ × −(−ax̂ + y ŷ)
= −Ia dy ẑ
Para realizar este producto cruz de manera sencilla se recuerda que estamos en la base “(x, y, z)”
en coordenadas cartesianas, por lo que ŷ × x̂ = −ẑ. Al avanzar hacia atrás el signo es negativo.
Para determinar = dl” se debe observar cómo es el movimiento de la corriente (en este caso
es en el eje y), las coordenadas en uso (cartesianas) y el tipo de diferencial (lineal).

Finalmente, se arma la integral del campo para el segmento 1, considerando los límites de
integración propuestos con anterioridad:
Z
µ0
Idl × (x − x ′ )
B1 =
4π L
|x − x ′ |3
Z b
−Ia dy ẑ
µ0
4π ∞ (a2 + y 2 )3/2
b
Z
µ0 arctan( a ) −Ia · a sec2 θ dθ ẑ
4π π
(a2 + (a tan θ)2 )3/2
b
Z
sec2 θ
−Iµ0 arctan( a )
dθ ẑ
2 )3/2
4πa π
(1
+
tan
θ
b
Z
−Iµ0 arctan( a ) 1
dθ ẑ
4πa π
sec θ
Z arctan( b )
a
−Iµ0
cos θ dθ ẑ
4πa π

b

arctan( a )
−Iµ0
· (sin θ)
ẑ
4πa
π

 
−Iµ0
b
π
· (sin arctan
− sin ) ẑ
4πa
a

 
−Iµ0
b
· (sin arctan
− 1) ẑ
4πa
a

Notar que se realizó un cambio de variable y = a tan θ → dy = a sec2 θ dθ
y que se utilizó la propiedad trigonométrica sec2 θ = 1 + tan2 θ.

---

### Página 12

Paso 2: Campo Segmento 2 - B2
Desde ahora en adelante, nuestro sistema de referencia será el punto = O” y se utilizarán
coordenadas cartesianas por la geometría del ejercicio. Se recuerda que el vector r parte en el
origen y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ parte en el origen y recorre todo el cuerpo con corriente:
r ′ = xx̂ + bŷ,

x ∈ [−a, a]

Se debe hacer énfasis en cómo es el sentido de la corriente.

Se siguen determinando componentes de la integral:
r − r ′ = −(xx̂ + bŷ)
Calculando el módulo del vector anterior:

|r − r ′ | =

p
x2 + b 2

Usando los resultados anteriores:
Idl × (r − r ′ ) = I dxx̂ × −(xx̂ + bŷ)
= −Ib dx ẑ
Para realizar este producto cruz de manera sencilla se recuerda que estamos en la base “(x, y, z)”
en coordenadas cartesianas, por lo que x̂ × ŷ = ẑ. Al avanzar hacia adelante el signo es positivo.
Para determinar = dl” se debe observar cómo es el movimiento de la corriente (en este caso
es en el eje x), las coordenadas en uso (cartesianas) y el tipo de diferencial (lineal).

Finalmente, se arma la integral del campo para el segmento 2, considerando los límites de
integración propuestos con anterioridad:
Z
µ0
Idl × (x − x ′ )
B2 =
4π L
|x − x ′ |3
Z a
µ0
−Ib dx ẑ
4π −a (x2 + b2 )3/2
a
Z
µ0 arctan( b ) −Ib · b sec2 θ dθ ẑ
4π arctan( −a ) (b2 + (b tan θ)2 )3/2
b
Z arctan( a )
b
−Iµ0
sec2 θ
dθ ẑ
4πb arctan( −a ) (1 + tan θ2 )3/2
b
a
Z
−Iµ0 arctan( b ) 1
dθ ẑ
4πb arctan( −a ) sec θ
b
a
Z
−Iµ0 arctan( b )
cos θ dθ ẑ
4πb arctan( −a )
b
arctan( ab )
−Iµ0
· (sin θ)
ẑ
4πb
arctan( −a
b )




 a 
−Iµ0
−a
· (sin arctan
− sin arctan
) ẑ
4πb
b
b

---

### Página 13

Notar que se realizó un cambio de variable x = b tan θ → dx = b sec2 θ dθ
y que se utilizó la propiedad trigonométrica sec2 θ = 1 + tan2 θ.

Paso 3: Campo Segmento 3 - B3
Desde ahora en adelante, nuestro sistema de referencia será el punto = O” y se utilizarán
coordenadas cartesianas por la geometría del ejercicio. Se recuerda que el vector r parte en el
origen y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el centro de referencia coincide con el punto a calcular el vector es nulo.

Luego, el vector r ′ parte en el origen y recorre todo el cuerpo con corriente:
r ′ = ax̂ + y ŷ,

y ∈ [b, ∞]

Se debe hacer énfasis en cómo es el sentido de la corriente.

Se siguen determinando componentes de la integral:
r − r ′ = −(ax̂ + y ŷ)
Calculando el módulo del vector anterior:

|r − r ′ | =

p
a2 + y 2

Usando los resultados anteriores:
Idl × (r − r ′ ) = I dy ŷ × −(ax̂ + y ŷ)
= Ia dy ẑ
Para realizar este producto cruz de manera sencilla se recuerda que estamos en la base “(x, y, z)”
en coordenadas cartesianas, por lo que ŷ × x̂ = −ẑ. Al avanzar hacia atrás el signo es negativo.
Para determinar = dl” se debe observar cómo es el movimiento de la corriente (en este caso
es en el eje y), las coordenadas en uso (cartesianas) y el tipo de diferencial (lineal).

Finalmente, se arma la integral del campo para el segmento 3, considerando los límites de
integración propuestos con anterioridad:

---

### Página 14

Z
µ0
Idl × (x − x ′ )
B3 =
4π L
|x − x ′ |3
Z ∞
µ0
Ia dy ẑ
4π b (a + y 2 )3/2
Z π
µ0
Ia · a sec2 θ dθ ẑ
4π arctan( b ) (a2 + (a tan θ)2 )3/2
a
Z π
Iµ0
sec2 θ
dθ ẑ
4πa arctan( b ) (1 + tan θ2 )3/2
a
Z π
Iµ0
dθ ẑ
b
4πa arctan( ) sec θ
a
Z π
Iµ0
cos θ dθ ẑ
4πa arctan( b )
a
π

Iµ0
· (sin θ)
ẑ
4πa
arctan( ab )

 
b
Iµ0
π
· (sin − sin arctan
) ẑ
4πa
a

 
b
Iµ0
· (1 − sin arctan
) ẑ
4πa
a

Notar que se realizó un cambio de variable y = a tan θ → dy = a sec2 θ dθ
y que se utilizó la propiedad trigonométrica sec2 θ = 1 + tan2 θ.

Paso 4: Principio de Superposición - B
Finalmente, el campo magnético en el punto O será la suma de los campos generados por los
3 segmentos:
B = B 1 + B 2 + B3

 




 a 
−Iµ0
b
−Iµ0
−a
· (sin arctan
− 1) ẑ +
· (sin arctan
− sin arctan
) ẑ
4πa
a
4πb
b
b

 
Iµ0
b
· (1 − sin arctan
) ẑ
+
4πa
a
Iµ0
b
−Iµ0
a
−a
· (1 − √
· (√
)+
−√
) ẑ
2πa
4πb
a +b
a +b
a2 + b 2
b
−Iµ0
a
Iµ0
· (1 − √
)+
·√
ẑ
2πa
2πb
a +b
a + b2
x
Notar que se utilizó la propiedad trigonométrica sin (arctan x) = √1+x
.

Nota: El tratamiento de las integrales también se puede realizar observando la simetría de la figura,
con el objetivo de simplificar los cálculos para los segmentos 1 y 3.
