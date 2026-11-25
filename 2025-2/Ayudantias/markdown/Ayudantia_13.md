---
title: "Ayudantia 13"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_13_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_13_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 13

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Ayudantía 13
30 de Septiembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Medios Conductores

1.1

Medios Conductores - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Comprender los conceptos de intensidad de corriente y resistencia eléctrica.
□
✓ Calcular la densidad de corriente eléctrica que circula a través de una sección transversal
□
mediante la Ley de Ohm Microscópica.
✓ Calcular el campo eléctrico generado por una corriente eléctrica mediante la Ley de Ohm
□
Microscópica.
✓ Calcular la intensidad de corriente eléctrica que circula a través de una sección transversal
□
a partir de su definición.
□ Identificar y aplicar la condición de borde normal a la densidad de corriente eléctrica
cuando sea necesario.

✓ Identificar y aplicar la condición de borde tangencial al campo eléctrico cuando sea
□
necesario.
✓ Determinar la resistencia eléctrica de una configuración mediante la Ley de Ohm Macroscópica.
□
✓ Determinar la resistencia eléctrica de un cuerpo a partir de su definición.
□
✓ Modelar las variaciones de las dimensiones de un cuerpo mediante la ecuación de la recta.
□
□ Relacionar y comprender los conceptos de resistividad y conductividad de un material.
□ Calcular la densidad de corriente eléctrica que circula a través de una sección transversal
mediante la velocidad de deriva de sus portadores de carga.

✓ Conocer la unidad de medida para la intensidad de corriente y resistencia eléctrica.
□

---

### Página 2

1.2

Medios Conductores - Generalidades

En primer lugar, la corriente eléctrica se puede definir como:
I=

dQ
dt

(1)

Donde = dQ” es la carga neta que pasa por una sección transversal de área = A”
durante un tiempo infinitesimal = dt”. Por convención, la corriente tendrá el sentido
del movimiento de las cargas positivas y su unidad de medida en el S.I es el = Ampère”:

C
s
Luego, la corriente total a través de un cuerpo se puede escribir como:
1A=1

Densidad
Superficial
Volumétrica

Integral Intensidad Corriente
I=

R

(2)

Otras Expresiones

L (K(x) × n̂) · dl(x)

I=

RR

S J(x) · dS(x)

J = qnvd

Donde = K(x)” y = J(x)” son las densidades de corriente superficial y volumétrica,
“n̂” el vector normal a la superficie por donde circula la corriente, = vd ” la velocidad media
o de deriva de las cargas y = n” el número de portadores de carga por unidad de volumen.

Por otra parte, la ecuación de continuidad describe el principio de conservación de carga como:
⃗ · J(x, t) + δρ(x) = 0
∇
δt

(3)

Además, para corrientes en estado estacionario (i.e sin dependencia temporal) se cumple que:

⃗ · J(x) = 0
∇
J1n = J2n

(4)

E1t = E2t

(5)

Donde = t” y = n” son las componentes tangencial y normal, mientras que los subíndices = 1” y = 2”
denotan los medios de la interfaz. Por último, la solución de la ecuación de continuidad es:

ρ(x, t) = ρ0 (x)e−t/τ
Donde = τ = ε0 /σ” es el tiempo de decaimiento o relajación.

1.3

Medios Conductores - Ley de Ohm Macroscópica y Microscópica

La Ley de Ohm macroscópica se puede expresar como:
V = IR

(6)

Donde = R” es la resistencia eléctrica del material, la cual se opone al flujo de corriente eléctrica.
Su unidad de medida en el S.I es el = Ohm”:

---

### Página 3

V
A
Asimismo, la resistencia para un conductor tipo cable se puede modelar como:
Z
ρ
R=
dl
L A
1Ω=1

(7)

(8)

Donde = L” es el largo, = A” el área de la sección transversal y = ρ” la resistividad del material.
Ahora, se puede definir la conductividad de un material como:

σ=

ρ

(9)

En general, la resistividad y resistencia varían linealmente con la temperatura de acuerdo a:

ρ(T ) = ρ0 (1 + α(T − T0 ))
R(T )) = R0 (1 + α(T − T0 ))
Donde = α” es el coeficiente de temperatura de resistividad, mientras que
“ρ0 ” y = R0 ” es la resistividad y resistencia de referencia, respectivamente.

Por último, la Ley de Ohm puede ser escrita localmente como:
J(x) = σE(x)

(10)

De aquí, se extrae que el componente vectorial de J será igual que el de E.

1.4

Medios Conductores - Cómo Utilizarlo Correctamente I

Los pasos a seguir para calcular la resistencia de un conductor por definición son:
1. Generalmente, les pedirán determinar la resistencia entre dos caras de un cuerpo. El
camino entre estas caras constituirá el área de la sección transversal a calcular y pueden
modelarlo según su forma: si es una circunferencia será πr2 , si es un rectángulo será a · b,
entre otros.
2. Es probable que esta sección transversal varíe a lo largo del cuerpo y, con ello, el radio
de la circunferencia, el lado del rectángulo, etc. Pueden haber miles de métodos, pero
en coordenadas cartesianas será fácil calcular esta variación mediante una ecuación de la
recta, la cual pueden revisar en el Anexo ??.
3. Finalmente, se reemplaza el área (que puede o no estar en función de un parámetro a
integrar) y se utiliza la expresión por definición:
Z
ρ
dl
R=
L A
Es posible que no sea necesario integrar, sino solo conocer el largo del cuerpo. No obstante, y si
el área de la sección transversal varía a medida que se recorre el cuerpo, se deberá integrar.

---

### Página 4

1.5

Medios Conductores - Cómo Utilizarlo Correctamente II

El fuerte de esta sección será determinar la corriente y/o resistencia presente en una configuración. Para ello:
1. Se deberá utilizar la Ley de Ohm macroscópica. Generalmente entregarán la diferencia
de potencial a la que se encuentra la configuración, por lo que será un dato conocido y
quedará despejar = I” o = R” según corresponda:
V = IR
En caso de que no expliciten el lugar de la carga positiva/negativa, se asume que la
positiva se encuentra en el lugar más interno, mientras que la negativa en el más externo.

2. Nos podemos enfrentar a distintas situaciones:
a) En el caso de que no se presente ningún corte importante, nos saltamos al paso = 3”.
b) En el caso de que en una misma sección transversal hayan 2 o más conductividades
distintas, se tendrá que utilizar la siguiente condición de borde:
E1t = E2t
Si es que se utiliza esta condición, el orden de los pasos no se modifica
y se suman las intensidades de cada parte para dar con la intensidad total.

c) En el caso de que en distintas secciones transversales hayan 2 o más conductividades
distintas, se tendrá que utilizar la siguiente condición de borde:
J1n = J2n
Si es que se utiliza esta condición, se realiza el paso = 4” antes que el = 3”.

3. Luego, se tendrá que determinar la densidad de corriente a partir de la Ley de Ohm
microscópica:
J = σE
Para ello será necesario conocer el campo eléctrico,
ya sea por Ley de Gauss Generalizada o por definición.

4. Para llegar a la intensidad de corriente, se tendrá que recurrir a su definición:
ZZ
I=
J · dS
S

Si J es constante, este cálculo resultará en el producto entre el área de la superficie y
la componente ortogonal de la densidad de corriente. Además, y por producto punto,
la componente del diferencial de superficie a usar deberá ser igual que el de J.

---

### Página 5

1.5.1

“Problemas de Electromagnetismo”, 2.3.4, Sebastián Urrutia

Suponga que se construye una cuña y un cono truncado usando material de resistividad
ρ. Determine la resistencia de los cuerpos entre las caras A y B mostradas en la figura.

Figura 1. Esquema sobre la cuña y el cono en estudio.

Solución a) y b)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la resistencia entre las caras A y B de la cuña y el cono. Como se conoce
su resistividad, se utilizará la expresión de resistencia por definición:
Z
ρ
R=
dl
A
Como el área varía dependiendo del largo, es necesario integrar.

---

### Página 6

1.5.2

“Control 2 2017-2”, Problema 1, Departamento de Física

Se dispone de dos placas conductoras planas y paralelas (i.e capacitor), de sección 2S
y separadas una distancia d. La mitad del espacio existente entre ellas está ocupado
por un material de conductividad g1 y permitividad ε1 . La otra mitad está ocupado
por un material de conductividad g2 y permitividad ε2 . El sistema se encuentra en
estado estacionario, conectado a un generador que establece una diferencia de potencial
V0 entre las placas, determine:
a) Los campos E y D entre las placas.
b) La densidad de corriente J entre las placas.
c) La intensidad de corriente (en cada medio y total) y la resistencia del sistema.
d) La carga libre en cada una de las placas. ¿Es la misma en ambas mitades? Explique
su resultado.
e) La potencia disipada por efecto Joule. ¿De dónde proviene esta energía disipada?
f) La capacitancia y la energía que almacena la configuración.
g) Si el generador se desconecta, explique cualitativamente qué sucederá. ¿Cuánta
energía se disiparía a lo largo del tiempo?

Figura 2. Condensador conectado a un generador.

Solución a), b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la resistencia entre las placas conductoras (i.e 0 < z < d). En primer lugar,
la intensidad de corriente estará dada por:
ZZ
I=
J(x) · dS(x)
S

Como la conductividad no es constante en la misma sección
transversal, se debe cumplir la siguiente condición de borde:

E1t = E2t

---

### Página 7

Ahora, la densidad de corriente se puede calcular como:

J(x) = σE(x)
Asimismo, el vector desplazamiento para un dieléctrico está dado por:

D = εE = ε0 κE
Luego, se puede utilizar la forma integral de la relación campo - potencial:
Z rb
E · dl
V (rb ) − V (ra ) = −
ra

Finalmente, la resistencia se puede calcular utilizando la Ley de Ohm Macroscópica:
V = IR

Solución d)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la densidad de carga libre total (superficial y volumétrica) en cada una de
las placas (i.e r = 0 y r = d), por lo que se utilizará la forma diferencial de la Ley de Gauss
Generalizada y la expresión relacionada con la discontinuidad del desplazamiento eléctrico:
∇ · D = ρf
D2n − D1n = σf
r=a

Luego, será necesario calcular los desplazamientos eléctricos
en las regiones colindantes a z = 0 y z = d: z > d y z < 0.
Como el espacio está relleno con distintos materiales dieléctricos,
se debe calcular por separado la densidad en tales regiones.

Solución f ), g) y h)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la energía almacenada y la capacitancia del sistema. La energía almacenada
en un condensador se puede expresar de distintas maneras:
U=

1 Q2
= CV 2 = QV
2 C

Por último, la capacitancia de un condensador de placas paralelas se puede escribir como:

C=

εA
d

---

### Página 8

Introducción a Circuitos Eléctricos

2.1

Introducción a Circuitos Eléctricos - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Identificar nodos y comprender sus implicancias eléctricas en diversos circuitos eléctricos.
□
✓ Identificar mallas y comprender sus implicancias eléctricas en diversos circuitos eléctricos
□
□ Identificar y utilizar convenientemente supernodos y supermallas en diversos circuitos
eléctricos.

✓ Aplicar la Ley de Kirchoff para corrientes (KCL) en diversos circuitos eléctricos.
□
✓ Aplicar la Ley de Kirchoff para voltajes (KVL) en diversos circuitos eléctricos.
□
✓ Analizar e interpretar los resultados obtenidos a partir de la aplicación de las Leyes de
□
Kirchoff en diversos contextos.
✓ Comprender la convención del sentido de la corriente en relación a la diferencia de po□
tencial existente en un componente circuital.
✓ Comprender y utilizar convenientemente el nodo tierra, de manera de aprovechar sus
□
efectos en el potencial eléctrico.
✓ Utilizar la Ley de Ohm para el cálculo de voltaje, intensidad o resistencia eléctrica según
□
el contexto.
✓ Identificar resistores conectados en serie y paralelo en diversas configuraciones.
□
✓ Determinar la resistencia equivalente de una configuración mediante el método de conex□
iones.
✓ Calcular la potencia eléctrica entregada o disipada por un elemento circuital mediante la
□
Ley de Joule según el contexto.
✓ Realizar balances de potencia eléctrica para diversos circuitos eléctricos.
□
✓ Identificar la presencia de cortocircuitos y sus efectos eléctricos según el contexto.
□
□ Identificar la presencia de circuitos abiertos y sus efectos eléctricos según el contexto.

✓ Resolver sistemas de ecuaciones de forma rápida y eficiente.
□
□ Conocer los instrumentos de medición circuitales básicos y sus respectivos usos.
□ Obtener los mínimos y máximos de una función mediante el método de la derivada.
□ Utilizar límites matemáticos y técnicas relacionadas, tales como la regla de L’hopital.
□ Comprender y utilizar convenientemente fuentes de prueba, de manera de aprovechar sus
efectos eléctricos.

✓ Conocer la unidad de medida para la potencia eléctrica.
□

---

### Página 9

2.2

Circuitos Eléctricos - Generalidades

Un dispositivo que suministra energía eléctrica a un circuito se llama fuente de fuerza electromotriz (fem):
dW
dq

ε=

(11)

Donde = dW ” es el trabajo hecho para mover la(s) carga(s) en cuestión.
Un ejemplo de fem sería una batería, la cual puede ser ideal
o real dependiendo si presenta o no resistencia interna:

(a) Circuito con batería ideal

(b) Circuito con batería real

Figura 3. Diagramas sobre los tipos de baterías.
Por otra parte, un conjunto de = N ” resistores puede conectarse de distintas formas:
Conexión
Serie

Resistencia Equivalente

Efectos Eléctricos

PN

i=1 Ri

Misma Corriente en cada Ri

PN 1
i=1 Ri
Req =

Mismo Voltaje en cada Ri

Req =

Paralelo

(a) Resistores conectados en serie
(b) Resistores conectados en paralelo

Figura 4. Diagramas sobre las configuraciones de resistores.

---

### Página 10

Finalmente, la energía eléctrica disipada por un resistor se puede expresar como:
Z t
E=
P dt

(12)

Donde = P ” es la potencia eléctrica disipada por el mismo,
la cual según la Ley de Joule se puede expresar como:

P = V I = I 2R =

V2
R

(13)

Además, y como es un tipo de potencia,
su unidad de medida en el S.I será el = Watt”:

1W=1

2.3

J
s

(14)

Circuitos Eléctricos - Instrumentos de Medición

Por último, existen dos instrumentos de medición básicos para la electrónica:
Instrumento
de Medición

¿Qué característica mide?

Condiciones Ideales

Amperímetro

Intensidad de Corriente

Conexión en Serie
y Resistencia Interna Baja

Voltímetro

Diferencia de Potencial

Conexión en Paralelo
y Resistencia Interna Alta

(a) Circuito en presencia de amperímetro
(b) Circuito en presencia de voltímetro

Figura 5. Diagramas sobre los instrumentos circuitales básicos de medición.

---

### Página 11

2.4

Circuitos Eléctricos - Casos Especiales

Es posible que se enfrenten a dos situaciones = especiales”:
a) ¿Qué es un cortocircuito? Se produce un cortocircuito cuando una rama sin ningún
componente circuital se encuentra conectada en paralelo con otras ramas. Luego, la
corriente preferirá movilizarse a través del camino que menos se le oponga. Además, y
si una fuente de voltaje se apaga, esta es retirada del circuito y sus terminales siguen
unidos.
b) ¿Qué es un circuito abierto? Se produce un circuito abierto cuando parte de este está
interrumpido o desconectado, provocando la imposibilidad de circulación de corriente
eléctrica en tal área. Además, y si una fuente de corriente se apaga, el circuito se abre y
sus terminales no siguen unidos.

(a) Ejemplo de cortocircuito

(b) Ejemplo de circuito abierto

Figura 6. Diagramas sobre los casos circuitales especiales.

2.5

Circuitos Eléctricos - Cómo Utilizarlo Correctamente I

Lo más importante será reducir resistencias/capacitores para simplificar cálculos:
a) ¿Cómo identificar resistencias/capacitores en serie? Estos estarán en una misma rama,
es decir, en una misma línea sin = cortes”. De esta manera, la corriente será la misma
para cada uno de los componentes circuitales.
b) ¿Cómo identificar resistencias/capacitores en paralelo? Estos tendrán terminales idénticos,
es decir nacerán en un mismo nodo y llegarán a otro nodo conjuntamente. De esta manera, la diferencia de potencial será la misma para cada uno de los componentes circuitales.

---

### Página 12

2.6

Circuitos Eléctricos - Leyes de Kirchoff

Gracias a la 1° Ley de Kirchoff (KCL), se determina que la suma de corrientes que llegan a un
nodo debe ser igual a la suma de corrientes que salen por el mismo:
X
X
Ik =
Ij
(15)
entrada

salida

Un nodo es un conjunto de puntos que poseen el mismo voltaje.
Pese a que no es del todo correcto, se tiende a pensar que
un nodo es solo la intersección entre varias ramas circuitales.

Por otra parte, la 2° Ley de Kirchoff (KVL) enuncia que la suma de los voltajes en cada malla
debe ser igual a 0:
X
Vk = 0
(16)
malla

Una malla es un camino cerrado formado por variados elementos circuitales.

Figura 7. Esquema circuital sobre ramas, nodos y mallas.

2.7

Circuitos Eléctricos - Cómo Utilizarlo Correctamente II

Estos métodos se usarán prácticamente en todos los ejercicios y serán útiles para circuitos más
complejos:
a) Método de Nodos (KCL):
1. ¿Cuándo elegir método de nodos? Se utilizará cuando se presenten varias fuentes
independientes/dependientes de corriente y/o bastantes mallas.
2. Luego, se tendrá que elegir de forma arbitraria el voltaje a tierra y nombrar el
voltaje de los nodos. Se debe notar que el voltaje se mantendrá constante mientras
no pase por algo que sume o reste potencial (i.e resistores, fuentes, etc).
3. Asignar arbitrariamente el sentido de la corriente que circula por cada uno de los
elementos circuitales, notando que esta ingresa por el polo positivo.

---

### Página 13

4. Armar las ecuaciones de nodos. Para ello, se debe observar cada nodo y considerar
las corrientes que entran y salen de este:
X
X
Ik =
Ij
entrada

salida

Luego, las intensidades provenientes de resistores deberán ser reemplazadas
mediante la Ley de Ohm. Es importante destacar que la diferencia de potencial
en cada resistor se debe hacer en el mismo sentido que circula la corriente:

I=

∆V
Vb − Va
=
R
R

Donde Vb y Va son los voltajes del nodo inicial y final, respectivamente.

5. ¿Cuántas ecuaciones armar? La cantidad de ecuaciones debe ser igual a la cantidad
de incógnitas que haya. En caso de que falten ecuaciones, se puede utilizar la Ley
de Ohm en algún resistor, KVL y/o construir un supernodo. Esta última opción se
aplicará cuando haya una rama ”vacía/inútil” (sin que haya cortocircuito) o cuando
se presente una fuente de voltaje en medio de un nodo.
6. Finalmente, se resuelve el sistema de ecuaciones.
b) Método de Mallas (KVL):
1. ¿Cuándo elegir método de mallas? Se utilizará cuando se presenten varias fuentes
independientes/dependientes de voltaje y/o pocas mallas.
2. Luego, se tendrá que nombrar arbitrariamente las corrientes que circulan por las
mallas. Por simplicidad, se espera que sus sentidos sean iguales (o todos horarios o
todos antihorarios).
3. También, se deberá asignar arbitrariamente el sentido de la corriente que circula por
cada uno de los elementos circuitales, notando que esta ingresa por el polo positivo.
4. Armar las ecuaciones de mallas. Para ello, se debe observar cada malla y recorrerla
en un sentido arbitrario, ojalá en el sentido otorgado anteriormente. Al pasar por
un elemento circuital, se sumará su voltaje si se entra de + a − (en caso contrario
se resta):
X
Vk = 0
malla

El sumar o restar voltaje es una convención propia y se puede usar otra mientras se sea
consistente. Luego, los voltajes provenientes de resistores deberán ser reemplazados
mediante la Ley de Ohm. Es importante destacar que la diferencia de potencial debe
respetar la convención utilizada con respecto a la corriente en cada resistor:

∆V = IR = (Ib − Ia )R
Donde Ib e Ia son las intensidades de las mallas que
ingresan por el polo positivo y negativo, respectivamente.

5. ¿Cuántas ecuaciones armar? La cantidad de ecuaciones debe ser igual a la cantidad
de incógnitas que haya. En caso de que falten ecuaciones, se puede utilizar la Ley
de Ohm en algún resistor, KCL y/o construir una supermalla. Esta última opción
se aplicará cuando se presente una fuente de corriente en medio de la malla.
6. Finalmente, se resuelve el sistema de ecuaciones.

---

### Página 14

2.7.1

“I2 2022-2”, Problema 2, Facultad de Física

Considere el circuito de la figura, donde Ra = 2 Ω, Rb = 4 Ω, Rc = 3 Ω, Rd = 2 Ω,
Re = 5 Ω, εA = 24 V y εB = 12 V.
a) Calcule el valor de las seis corrientes indicadas en este circuito.
b) Realice un balance de potencia para este circuito.
c) Para lograr que una sustancia eleve su temperatura rápidamente se requiere de un
aparato que libere energía a una tasa mínima de 150 Joules por segundo, ¿serviría
el circuito mostrado en la figura para realizar esta tarea?
d) Ahora, suponga que se apaga la fuente de voltaje εA . Determine la resistencia
equivalente de este nuevo circuito, vista desde los terminales de la fuente voltaje
εB .

Figura 8. Esquema circuital en estudio.

---

### Página 15

Solución a), b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la potencia entregada y/o disipada por cada elemento circuital. En primer
lugar, la potencia eléctrica se puede calcular utilizando la Ley de Joule:
P = V I = I 2R =

V2
R

Luego, se deberá resolver el circuito mediante algún método.
Finalmente, se debe comprobar que la potencia entregada es equivalente a la disipada:

X

PE =

X

PD

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 13
30 de Septiembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Medios Conductores

1.1

Medios Conductores - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Comprender los conceptos de intensidad de corriente y resistencia eléctrica.
□
✓ Calcular la densidad de corriente eléctrica que circula a través de una sección transversal
□
mediante la Ley de Ohm Microscópica.
✓ Calcular el campo eléctrico generado por una corriente eléctrica mediante la Ley de Ohm
□
Microscópica.
✓ Calcular la intensidad de corriente eléctrica que circula a través de una sección transversal
□
a partir de su definición.
□ Identificar y aplicar la condición de borde normal a la densidad de corriente eléctrica
cuando sea necesario.

✓ Identificar y aplicar la condición de borde tangencial al campo eléctrico cuando sea
□
necesario.
✓ Determinar la resistencia eléctrica de una configuración mediante la Ley de Ohm Macroscópica.
□
✓ Determinar la resistencia eléctrica de un cuerpo a partir de su definición.
□
✓ Modelar las variaciones de las dimensiones de un cuerpo mediante la ecuación de la recta.
□
□ Relacionar y comprender los conceptos de resistividad y conductividad de un material.
□ Calcular la densidad de corriente eléctrica que circula a través de una sección transversal
mediante la velocidad de deriva de sus portadores de carga.

✓ Conocer la unidad de medida para la intensidad de corriente y resistencia eléctrica.
□

---

### Página 2

1.2

Medios Conductores - Generalidades

En primer lugar, la corriente eléctrica se puede definir como:
I=

dQ
dt

(1)

Donde = dQ” es la carga neta que pasa por una sección transversal de área = A”
durante un tiempo infinitesimal = dt”. Por convención, la corriente tendrá el sentido
del movimiento de las cargas positivas y su unidad de medida en el S.I es el = Ampère”:

C
s
Luego, la corriente total a través de un cuerpo se puede escribir como:
1A=1

Densidad
Superficial
Volumétrica

Integral Intensidad Corriente
I=

R

(2)

Otras Expresiones

L (K(x) × n̂) · dl(x)

I=

RR

S J(x) · dS(x)

J = qnvd

Donde = K(x)” y = J(x)” son las densidades de corriente superficial y volumétrica,
“n̂” el vector normal a la superficie por donde circula la corriente, = vd ” la velocidad media
o de deriva de las cargas y = n” el número de portadores de carga por unidad de volumen.

Por otra parte, la ecuación de continuidad describe el principio de conservación de carga como:
⃗ · J(x, t) + δρ(x) = 0
∇
δt

(3)

Además, para corrientes en estado estacionario (i.e sin dependencia temporal) se cumple que:

⃗ · J(x) = 0
∇
J1n = J2n

(4)

E1t = E2t

(5)

Donde = t” y = n” son las componentes tangencial y normal, mientras que los subíndices = 1” y = 2”
denotan los medios de la interfaz. Por último, la solución de la ecuación de continuidad es:

ρ(x, t) = ρ0 (x)e−t/τ
Donde = τ = ε0 /σ” es el tiempo de decaimiento o relajación.

1.3

Medios Conductores - Ley de Ohm Macroscópica y Microscópica

La Ley de Ohm macroscópica se puede expresar como:
V = IR

(6)

Donde = R” es la resistencia eléctrica del material, la cual se opone al flujo de corriente eléctrica.
Su unidad de medida en el S.I es el = Ohm”:

---

### Página 3

V
A
Asimismo, la resistencia para un conductor tipo cable se puede modelar como:
Z
ρ
R=
dl
L A
1Ω=1

(7)

(8)

Donde = L” es el largo, = A” el área de la sección transversal y = ρ” la resistividad del material.
Ahora, se puede definir la conductividad de un material como:

σ=

ρ

(9)

En general, la resistividad y resistencia varían linealmente con la temperatura de acuerdo a:

ρ(T ) = ρ0 (1 + α(T − T0 ))
R(T )) = R0 (1 + α(T − T0 ))
Donde = α” es el coeficiente de temperatura de resistividad, mientras que
“ρ0 ” y = R0 ” es la resistividad y resistencia de referencia, respectivamente.

Por último, la Ley de Ohm puede ser escrita localmente como:
J(x) = σE(x)

(10)

De aquí, se extrae que el componente vectorial de J será igual que el de E.

1.4

Medios Conductores - Cómo Utilizarlo Correctamente I

Los pasos a seguir para calcular la resistencia de un conductor por definición son:
1. Generalmente, les pedirán determinar la resistencia entre dos caras de un cuerpo. El
camino entre estas caras constituirá el área de la sección transversal a calcular y pueden
modelarlo según su forma: si es una circunferencia será πr2 , si es un rectángulo será a · b,
entre otros.
2. Es probable que esta sección transversal varíe a lo largo del cuerpo y, con ello, el radio
de la circunferencia, el lado del rectángulo, etc. Pueden haber miles de métodos, pero
en coordenadas cartesianas será fácil calcular esta variación mediante una ecuación de la
recta, la cual pueden revisar en el Anexo ??.
3. Finalmente, se reemplaza el área (que puede o no estar en función de un parámetro a
integrar) y se utiliza la expresión por definición:
Z
ρ
dl
R=
L A
Es posible que no sea necesario integrar, sino solo conocer el largo del cuerpo. No obstante, y si
el área de la sección transversal varía a medida que se recorre el cuerpo, se deberá integrar.

---

### Página 4

1.5

Medios Conductores - Cómo Utilizarlo Correctamente II

El fuerte de esta sección será determinar la corriente y/o resistencia presente en una configuración. Para ello:
1. Se deberá utilizar la Ley de Ohm macroscópica. Generalmente entregarán la diferencia
de potencial a la que se encuentra la configuración, por lo que será un dato conocido y
quedará despejar = I” o = R” según corresponda:
V = IR
En caso de que no expliciten el lugar de la carga positiva/negativa, se asume que la
positiva se encuentra en el lugar más interno, mientras que la negativa en el más externo.

2. Nos podemos enfrentar a distintas situaciones:
a) En el caso de que no se presente ningún corte importante, nos saltamos al paso = 3”.
b) En el caso de que en una misma sección transversal hayan 2 o más conductividades
distintas, se tendrá que utilizar la siguiente condición de borde:
E1t = E2t
Si es que se utiliza esta condición, el orden de los pasos no se modifica
y se suman las intensidades de cada parte para dar con la intensidad total.

c) En el caso de que en distintas secciones transversales hayan 2 o más conductividades
distintas, se tendrá que utilizar la siguiente condición de borde:
J1n = J2n
Si es que se utiliza esta condición, se realiza el paso = 4” antes que el = 3”.

3. Luego, se tendrá que determinar la densidad de corriente a partir de la Ley de Ohm
microscópica:
J = σE
Para ello será necesario conocer el campo eléctrico,
ya sea por Ley de Gauss Generalizada o por definición.

4. Para llegar a la intensidad de corriente, se tendrá que recurrir a su definición:
ZZ
I=
J · dS
S

Si J es constante, este cálculo resultará en el producto entre el área de la superficie y
la componente ortogonal de la densidad de corriente. Además, y por producto punto,
la componente del diferencial de superficie a usar deberá ser igual que el de J.

---

### Página 5

1.5.1

“Problemas de Electromagnetismo”, 2.3.4, Sebastián Urrutia

Suponga que se construye una cuña y un cono truncado usando material de resistividad
ρ. Determine la resistencia de los cuerpos entre las caras A y B mostradas en la figura.

Figura 1. Esquema sobre la cuña y el cono en estudio.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la resistencia entre las caras A y B de la cuña. Como se conoce su
resistividad, se utilizará la expresión de resistencia por definición:
Z
ρ
R=
dl
A
Como el área varía dependiendo del largo, es necesario integrar.

Paso 1: Relación Área y Largo Cuña - A(x)
Las caras del cuerpo son rectangulares, por lo que su área puede escribirse como:
A=h·d
Donde = h” es la altura y = d” la medida del lado que toca el suelo.
No obstante, y si posicionamos nuestro origen en la cara = B”, esta altura aumenta a
medida que varía el largo. Para conocer tal relación, se hará uso de una ecuación de la recta:

P1 (x, y) = (0, a)
P2 (x, y) = (L, a + b)


y−a=

(a + b) − a
(x − 0)
L−0

Se utilizó P1 (x, y) para armar la ecuación, pero se puede utilizar cualquiera de los
dos puntos para reemplazar (x1 , y1 ). Luego, la altura de la cuña vendrá dada por:

h(x) = a +

bx
L

Finalmente, se obtiene que el área es:

A(x) = (a +

bx
)d
L

(11)

---

### Página 6

Paso 2: Definición Resistencia Cuña - R
Finalmente, se utiliza la definición de resistencia, considerando los límites de integración propuestos con anterioridad:
Z
ρ
R=
dl
A
Z L
ρ
=
dx
bx
0 (a + L )d
Z a+b
ρL 1
=
dt
bd t
a
(12)
a+b
ρL
=
(ln t)
bd
a
ρL
=
(ln (a + b) − ln (a))
bd
b
ρL
ln (1 + )
=
bd
a
b
Notar que se realizó un cambio de variable t = a + bx
L → dt = L dx.

Solución b)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la resistencia entre las caras A y B del cono. Como se conoce su resistividad,
se utilizará la expresión de resistencia por definición:
Z
ρ
R=
dl
A
Como el área varía dependiendo del largo, es necesario integrar.

Paso 1: Relación Área y Largo - A(x)
Las caras del cuerpo son circunferenciales, por lo que su área puede escribirse como:
A = πr2
Donde = r” es la el radio de la circunferencia.
No obstante, y si es que posicionamos nuestro origen en la cara = A”, este radio aumenta a
medida que varía el largo. Para conocer tal relación, se hará uso de una ecuación de la recta:

P1 (x, y) = (0, a)
P2 (x, y) = (h, a + b)


y−a=

(a + b) − a
(x − 0)
h−0

Se utilizó P1 (x, y) para armar la ecuación, pero se puede utilizar cualquiera de los dos puntos para
reemplazar (x1 , y1 ). Luego, el radio del cono vendrá dado por:

r(x) = a +

bx
h

Finalmente, se obtiene que el área es:

A(x) = π(a +

bx 2
)
h

(13)

---

### Página 7

Paso 2: Definición Resistencia Cono - R
Finalmente, se utiliza la definición de resistencia, considerando los límites de integración propuestos con anterioridad:
Z
ρ
R=
dl
A
Z h
ρ
=
dx
bx 2
0 π(a + h )
Z a+b
ρh 1
=
dt
bπ t2
a
(14)
ρh
1 a+b
=
(− )
bπ
r a
ρh 1
− )
=− (
bπ a + b a
b
ρh
=
bπ a(a + b)
b
Notar que se realizó un cambio de variable t = a + bx
h → dt = h dx.

---

### Página 8

1.5.2

“Control 2 2017-2”, Problema 1, Departamento de Física

Se dispone de dos placas conductoras planas y paralelas (i.e capacitor), de sección 2S
y separadas una distancia d. La mitad del espacio existente entre ellas está ocupado
por un material de conductividad g1 y permitividad ε1 . La otra mitad está ocupado
por un material de conductividad g2 y permitividad ε2 . El sistema se encuentra en
estado estacionario, conectado a un generador que establece una diferencia de potencial
V0 entre las placas, determine:
a) Los campos E y D entre las placas.
b) La densidad de corriente J entre las placas.
c) La intensidad de corriente (en cada medio y total) y la resistencia del sistema.
d) La carga libre en cada una de las placas. ¿Es la misma en ambas mitades? Explique
su resultado.
e) La potencia disipada por efecto Joule. ¿De dónde proviene esta energía disipada?
f) La capacitancia y la energía que almacena la configuración.
g) Si el generador se desconecta, explique cualitativamente qué sucederá. ¿Cuánta
energía se disiparía a lo largo del tiempo?

Figura 2. Condensador conectado a un generador.

Solución a), b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la resistencia entre las placas conductoras (i.e 0 < z < d). En primer lugar,
la intensidad de corriente estará dada por:
ZZ
I=
J(x) · dS(x)
S

Como la conductividad no es constante en la misma sección
transversal, se debe cumplir la siguiente condición de borde:

E1t = E2t

---

### Página 9

Ahora, la densidad de corriente se puede calcular como:

J(x) = σE(x)
Asimismo, el vector desplazamiento para un dieléctrico está dado por:

D = εE = ε0 κE
Luego, se puede utilizar la forma integral de la relación campo - potencial:
Z rb
V (rb ) − V (ra ) = −
E · dl
ra

Finalmente, la resistencia se puede calcular utilizando la Ley de Ohm Macroscópica:
V = IR
Paso 1: Condición Estacionaria
En primer lugar, el sistema se encuentra en estado estacionario, es decir:
∇·J=0
Luego, y por la geometría del problema, se llega a que:

J = J ẑ
Gracias a la ecuación de continuidad, se concluye que la densidad
de corriente es constante y, con ello, el campo también.

Paso 2: Campo Eléctrico - E0<z<d
Dada la configuración de placas paralelas, se conoce que el campo entre ellas es constante y de
la forma:
E0<z<d = E0<z<d ẑ
Como V0 = ∆V , se calculará la diferencia de potencial eléctrico entre z = 0 y z = d. Los medios
se encuentran conectados en paralelo (i.e misma diferencia de potencial), pues sus terminales
son los mismos:
Z 0
E0<z<d · dl
V0 = V (0) − V (d) = −
d

Por propiedades de integrales se pueden invertir los límites
y la única componente en juego es la normal, por lo que:

Z d
V0 =

E0<z<d dz

V0 = E0<z<d · d
V0
E0<z<d =
d
Imponiendo la condición de borde (i.e E1t = E2t ) en la región 0 < z < d, se tiene que:

E0<z<d,1 = E0<z<d,2 =

V0
ẑ
d

Finalmente, y como el campo eléctrico es un vector, se agrega la componente normal:

E0<z<d,1 = E0<z<d,2 =

V0
ẑ
d

(15)

---

### Página 10

Paso 3: Desplazamiento Eléctrico - D0<z<d,1
Luego, el vector desplazamiento para el medio 1 está dado por:
D = εE = ε0 κE
Es importante notar que se puede ocupar cualquiera de las dos expresiones anteriores.
Por conveniencia se utilizará la primera, pues por enunciado se entrega = ε”:

D0<z<d,1 = ε1 E0<z<d,1
V0
ẑ
= ε1
d

(16)

Se usó = ε1 ” debido a que es la permitividad del dieléctrico que se encuentra en 0 < z < d (medio 1).

Paso 4: Desplazamiento Eléctrico - D0<z<d,2
Luego, el vector desplazamiento para el medio 2 está dado por:
D = εE = ε0 κE
Es importante notar que se puede ocupar cualquiera de las dos expresiones anteriores.
Por conveniencia se utilizará la primera, pues por enunciado dan el dato de = ε”:

D0<z<d,2 = ε2 E0<z<d,2
V0
= ε2
ẑ
d

(17)

Se usó = ε2 ” debido a que es la permitividad del dieléctrico que se encuentra en 0 < z < d (medio 2).

Paso 5: Ley de Ohm Microscópica - J0<z<d,1
Ahora, y ocupando la Ley de Ohm Microscópica en la región 0 < z < d para el medio 1, se
obtiene que:
J0<z<d,1 = σ0<z<d,1 E0<z<d,1
V0
= g1
ẑ
d

(18)

Paso 6: Ley de Ohm Microscópica - J0<z<d,2
Ahora, y ocupando la Ley de Ohm Microscópica en la región 0 < z < d para el medio 2, se
obtiene que:
J0<z<d,2 = σ0<z<d,2 E0<z<d,2
V0
= g2
ẑ
d

(19)

Paso 7: Intensidad de Corriente - I1
En primer lugar, se utiliza la definición de intensidad de corriente en la región 0 < z < d para
el medio 1:
ZZ
I1 =
J1 (x) · dS1 (x)
S1

---

### Página 11

Se conoce que J = J ẑ → E = E ẑ, por lo que se utilizará
el diferencial de superficie que contiene a “ẑ” en coordenadas cartesianas:

ZZ
J0<z<d,1 ẑ · dxdy ẑ
ZZ
dxdy
= J0<z<d,1 ·

I1 =

S

S

Cada medio rellena la mitad del espacio existente (i.e su sección superficial es de S), por lo que:

I1 = g1

V0
·S
d

(20)

Paso 8: Intensidad de Corriente - I2
Asimismo, se utiliza la definición de intensidad de corriente en la región 0 < z < d para el
medio 2:
ZZ
I2 =
J2 (x) · dS2 (x)
S2

Se conoce que J = J ẑ → E = E ẑ, por lo que se utilizará
el diferencial de superficie que contiene a “ẑ” en coordenadas cartesianas:

ZZ
J0<z<d,2 ẑ · dxdy ẑ
ZZ
= J0<z<d,2 ·
dxdy

I2 =

S

S

Cada medio rellena la mitad del espacio existente (i.e su sección superficial es de S), por lo que:

I2 = g2

V0
·S
d

(21)

Paso 9: Intensidad Equivalente - Ieq
Ahora, y como su disposición es paralela, se sumarán las corrientes que circulan por ambos
medios para obtener la intensidad de corriente total:
Ieq = I1 + I2
V0
V0
= g1
· S + g2
·S
d
d
V0
= S(g1 + g2 )
d

(22)

Paso 10: Ley de Ohm Macroscópica - Req
Finalmente, utilizando la Ley de Ohm Macroscópica en la región 0 < z < d se obtiene que:

---

### Página 12

Req =

Veq
Ieq

V0
S(g1 + g2 ) Vd0
d
=
S(g1 + g2 )
=

(23)

Solución d)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la densidad de carga libre total (superficial y volumétrica) en cada una de
las placas (i.e r = 0 y r = d), por lo que se utilizará la forma diferencial de la Ley de Gauss
Generalizada y la expresión relacionada con la discontinuidad del desplazamiento eléctrico:
∇ · D = ρf
D2n − D1n = σf
r=a

Luego, será necesario calcular los desplazamientos eléctricos
en las regiones colindantes a z = 0 y z = d: z > d y z < 0.
Como el espacio está relleno con distintos materiales dieléctricos,
se debe calcular por separado la densidad en tales regiones.

Paso 1: Densidad Carga Libre Volumétrica - ρf,1−2
Utilizando la forma diferencial de la Ley de Gauss Generalizada para ambos medios se obtiene
que:
ρf,1−2 = ∇ · D0<z<d,1−2
V0
= ∇ · (ε1−2
ẑ)
d
=0
Concuerda con lo esperado, puesto que se están estudiando superficies.

Paso 2: Densidad Carga Libre Superficial - σf,1
Dada la configuración de placas paralelas, se conoce que el campo fuera de ellas es nulo, por
lo que el desplazamiento también lo será. Posteriormente, se utiliza la expresión de densidad
de carga libre superficial evaluada en el límite z = 0 en el medio 1:
σf,01 = D0<z<d,1 − Dz<0,1
z=0

= D0<z<d,1 − 0
z=0

V0
= ε1
d z=0
V0
= ε1
d

(24)

---

### Página 13

Se usó = ε1 ” debido a que es la permitividad del dieléctrico que se encuentra en 0 < z < d (medio 1).
Análogamente, se nota que la densidad de carga es independiente de la distancia, por lo que:

σf,d1 = Dz>d,1 − D0<z<d,1
z=d

= 0 − D0<z<d,1
z=d

(25)

V0
= − ε1
d z=d
V0
= −ε1
d
Paso 3: Densidad Carga Libre Superficial - σf,2
Dada la configuración de placas paralelas, se conoce que el campo fuera de ellas es nulo, por
lo que el desplazamiento también lo será. Posteriormente, se utiliza la expresión de densidad
de carga libre superficial evaluada en el límite z = 0 en el medio 2:
σf,02 = D0<z<d,2 − Dz<0,2
z=0

= D0<z<d,1 − 0
z=0

(26)

V0
= ε2
d z=0
V0
= ε2
d
Se usó = ε2 ” debido a que es la permitividad del dieléctrico que se encuentra en 0 < z < d (medio 2).
Análogamente, se nota que la densidad de carga es independiente de la distancia, por lo que:

σf,d2 = Dz>d,2 − D0<z<d,2
z=d

= 0 − D0<z<d,2
z=d

(27)

V0
= − ε2
d z=d
V0
= −ε2
d
Paso 4: Análisis Carga Libre Superficial
Luego, podemos notar que σf,1 ̸= σf,2 , debido a que se aplica un mismo campo eléctrico a
distintos materiales dieléctricos. De esta manera, las cargas libres no pueden ser iguales para
generar el mismo campo eléctrico en ambos medios por la condición de borde tangencial.

---

### Página 14

Solución f ), g) y h)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la energía almacenada y la capacitancia del sistema. La energía almacenada
en un condensador se puede expresar de distintas maneras:
U=

1 Q2
= CV 2 = QV
2 C

Por último, la capacitancia de un condensador de placas paralelas se puede escribir como:

C=

εA
d

Paso 1: Capacitancia - C
La capacitancia de un condensador de placas paralelas se puede escribir como:
C=

εA
d

Esta configuración puede ser traducida como dos capacitores en
paralelo (medio con dieléctrico 1 junto con dieléctrico 2), pues están
a una misma diferencia de potencial, es decir, todos sus terminales
positivos y negativos están conectadas a un punto en común:

Ceq = C1 + C2
Para el caso = C1 ”, ε = ε1 , d1 = d y A1 = S, mientras
que para el caso = C2 ”, ε = ε2 , d2 = d y A2 = S:

ε1 S ε2 S
+
d
d
(ε1 + ε2 )S
=
d

Ceq =

(28)

Paso 2: Energía Almacenada - U
La energía almacenada en un condensador se puede expresar de distintas maneras:
U=

1 Q2
= CV 2 = QV
2 C

Es importante notar que todas son equivalentes e igual de válidas.
Por conveniencia, se utilizará la que relaciona = C” y = V ”, pues son datos conocidos:

1 (ε1 + ε2 )S 2
U = CV 2 =
V0
d

(29)

Por enunciado, se dice que la diferencia de potencial es = V0 ”.

Paso 3: Análisis Desconexión Generador
En un comienzo, el generador estaba conectado y permitía la aparición de campos eléctricos
en la región 0 < z < d. Al desconectar el generador, la diferencia de potencial entre las placas
se vuelve 0, lo que implica necesariamente la descarga de las placas y, con ello, la desaparición
de los campos en tal región. De esta manera, la energía final del condensador se volverá nula.

---

### Página 15

Introducción a Circuitos Eléctricos

2.1

Introducción a Circuitos Eléctricos - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Identificar nodos y comprender sus implicancias eléctricas en diversos circuitos eléctricos.
□
✓ Identificar mallas y comprender sus implicancias eléctricas en diversos circuitos eléctricos
□
□ Identificar y utilizar convenientemente supernodos y supermallas en diversos circuitos
eléctricos.

✓ Aplicar la Ley de Kirchoff para corrientes (KCL) en diversos circuitos eléctricos.
□
✓ Aplicar la Ley de Kirchoff para voltajes (KVL) en diversos circuitos eléctricos.
□
✓ Analizar e interpretar los resultados obtenidos a partir de la aplicación de las Leyes de
□
Kirchoff en diversos contextos.
✓ Comprender la convención del sentido de la corriente en relación a la diferencia de po□
tencial existente en un componente circuital.
✓ Comprender y utilizar convenientemente el nodo tierra, de manera de aprovechar sus
□
efectos en el potencial eléctrico.
✓ Utilizar la Ley de Ohm para el cálculo de voltaje, intensidad o resistencia eléctrica según
□
el contexto.
✓ Identificar resistores conectados en serie y paralelo en diversas configuraciones.
□
✓ Determinar la resistencia equivalente de una configuración mediante el método de conex□
iones.
✓ Calcular la potencia eléctrica entregada o disipada por un elemento circuital mediante la
□
Ley de Joule según el contexto.
✓ Realizar balances de potencia eléctrica para diversos circuitos eléctricos.
□
✓ Identificar la presencia de cortocircuitos y sus efectos eléctricos según el contexto.
□
□ Identificar la presencia de circuitos abiertos y sus efectos eléctricos según el contexto.

✓ Resolver sistemas de ecuaciones de forma rápida y eficiente.
□
□ Conocer los instrumentos de medición circuitales básicos y sus respectivos usos.
□ Obtener los mínimos y máximos de una función mediante el método de la derivada.
□ Utilizar límites matemáticos y técnicas relacionadas, tales como la regla de L’hopital.
□ Comprender y utilizar convenientemente fuentes de prueba, de manera de aprovechar sus
efectos eléctricos.

✓ Conocer la unidad de medida para la potencia eléctrica.
□

---

### Página 16

2.2

Circuitos Eléctricos - Generalidades

Un dispositivo que suministra energía eléctrica a un circuito se llama fuente de fuerza electromotriz (fem):
ε=

dW
dq

(30)

Donde = dW ” es el trabajo hecho para mover la(s) carga(s) en cuestión.
Un ejemplo de fem sería una batería, la cual puede ser ideal
o real dependiendo si presenta o no resistencia interna:

(a) Circuito con batería ideal

(b) Circuito con batería real

Figura 3. Diagramas sobre los tipos de baterías.
Por otra parte, un conjunto de = N ” resistores puede conectarse de distintas formas:
Conexión
Serie

Resistencia Equivalente

Efectos Eléctricos

PN

i=1 Ri

Misma Corriente en cada Ri

PN 1
i=1 Ri
Req =

Mismo Voltaje en cada Ri

Req =

Paralelo

(a) Resistores conectados en serie
(b) Resistores conectados en paralelo

Figura 4. Diagramas sobre las configuraciones de resistores.

---

### Página 17

Finalmente, la energía eléctrica disipada por un resistor se puede expresar como:
Z t
E=
P dt

(31)

Donde = P ” es la potencia eléctrica disipada por el mismo,
la cual según la Ley de Joule se puede expresar como:

P = V I = I 2R =

V2
R

(32)

Además, y como es un tipo de potencia,
su unidad de medida en el S.I será el = Watt”:

1W=1

2.3

J
s

(33)

Circuitos Eléctricos - Instrumentos de Medición

Por último, existen dos instrumentos de medición básicos para la electrónica:
Instrumento
de Medición

¿Qué característica mide?

Condiciones Ideales

Amperímetro

Intensidad de Corriente

Conexión en Serie
y Resistencia Interna Baja

Voltímetro

Diferencia de Potencial

Conexión en Paralelo
y Resistencia Interna Alta

(a) Circuito en presencia de amperímetro
(b) Circuito en presencia de voltímetro

Figura 5. Diagramas sobre los instrumentos circuitales básicos de medición.

---

### Página 18

2.4

Circuitos Eléctricos - Casos Especiales

Es posible que se enfrenten a dos situaciones = especiales”:
a) ¿Qué es un cortocircuito? Se produce un cortocircuito cuando una rama sin ningún
componente circuital se encuentra conectada en paralelo con otras ramas. Luego, la
corriente preferirá movilizarse a través del camino que menos se le oponga. Además, y
si una fuente de voltaje se apaga, esta es retirada del circuito y sus terminales siguen
unidos.
b) ¿Qué es un circuito abierto? Se produce un circuito abierto cuando parte de este está
interrumpido o desconectado, provocando la imposibilidad de circulación de corriente
eléctrica en tal área. Además, y si una fuente de corriente se apaga, el circuito se abre y
sus terminales no siguen unidos.

(a) Ejemplo de cortocircuito

(b) Ejemplo de circuito abierto

Figura 6. Diagramas sobre los casos circuitales especiales.

2.5

Circuitos Eléctricos - Cómo Utilizarlo Correctamente I

Lo más importante será reducir resistencias/capacitores para simplificar cálculos:
a) ¿Cómo identificar resistencias/capacitores en serie? Estos estarán en una misma rama,
es decir, en una misma línea sin = cortes”. De esta manera, la corriente será la misma
para cada uno de los componentes circuitales.
b) ¿Cómo identificar resistencias/capacitores en paralelo? Estos tendrán terminales idénticos,
es decir nacerán en un mismo nodo y llegarán a otro nodo conjuntamente. De esta manera, la diferencia de potencial será la misma para cada uno de los componentes circuitales.

---

### Página 19

2.6

Circuitos Eléctricos - Leyes de Kirchoff

Gracias a la 1° Ley de Kirchoff (KCL), se determina que la suma de corrientes que llegan a un
nodo debe ser igual a la suma de corrientes que salen por el mismo:
X
X
Ik =
Ij
(34)
entrada

salida

Un nodo es un conjunto de puntos que poseen el mismo voltaje.
Pese a que no es del todo correcto, se tiende a pensar que
un nodo es solo la intersección entre varias ramas circuitales.

Por otra parte, la 2° Ley de Kirchoff (KVL) enuncia que la suma de los voltajes en cada malla
debe ser igual a 0:
X
Vk = 0
(35)
malla

Una malla es un camino cerrado formado por variados elementos circuitales.

Figura 7. Esquema circuital sobre ramas, nodos y mallas.

2.7

Circuitos Eléctricos - Cómo Utilizarlo Correctamente II

Estos métodos se usarán prácticamente en todos los ejercicios y serán útiles para circuitos más
complejos:
a) Método de Nodos (KCL):
1. ¿Cuándo elegir método de nodos? Se utilizará cuando se presenten varias fuentes
independientes/dependientes de corriente y/o bastantes mallas.
2. Luego, se tendrá que elegir de forma arbitraria el voltaje a tierra y nombrar el
voltaje de los nodos. Se debe notar que el voltaje se mantendrá constante mientras
no pase por algo que sume o reste potencial (i.e resistores, fuentes, etc).
3. Asignar arbitrariamente el sentido de la corriente que circula por cada uno de los
elementos circuitales, notando que esta ingresa por el polo positivo.

---

### Página 20

4. Armar las ecuaciones de nodos. Para ello, se debe observar cada nodo y considerar
las corrientes que entran y salen de este:
X
X
Ik =
Ij
entrada

salida

Luego, las intensidades provenientes de resistores deberán ser reemplazadas
mediante la Ley de Ohm. Es importante destacar que la diferencia de potencial
en cada resistor se debe hacer en el mismo sentido que circula la corriente:

I=

∆V
Vb − Va
=
R
R

Donde Vb y Va son los voltajes del nodo inicial y final, respectivamente.

5. ¿Cuántas ecuaciones armar? La cantidad de ecuaciones debe ser igual a la cantidad
de incógnitas que haya. En caso de que falten ecuaciones, se puede utilizar la Ley
de Ohm en algún resistor, KVL y/o construir un supernodo. Esta última opción se
aplicará cuando haya una rama ”vacía/inútil” (sin que haya cortocircuito) o cuando
se presente una fuente de voltaje en medio de un nodo.
6. Finalmente, se resuelve el sistema de ecuaciones.
b) Método de Mallas (KVL):
1. ¿Cuándo elegir método de mallas? Se utilizará cuando se presenten varias fuentes
independientes/dependientes de voltaje y/o pocas mallas.
2. Luego, se tendrá que nombrar arbitrariamente las corrientes que circulan por las
mallas. Por simplicidad, se espera que sus sentidos sean iguales (o todos horarios o
todos antihorarios).
3. También, se deberá asignar arbitrariamente el sentido de la corriente que circula por
cada uno de los elementos circuitales, notando que esta ingresa por el polo positivo.
4. Armar las ecuaciones de mallas. Para ello, se debe observar cada malla y recorrerla
en un sentido arbitrario, ojalá en el sentido otorgado anteriormente. Al pasar por
un elemento circuital, se sumará su voltaje si se entra de + a − (en caso contrario
se resta):
X
Vk = 0
malla

El sumar o restar voltaje es una convención propia y se puede usar otra mientras se sea
consistente. Luego, los voltajes provenientes de resistores deberán ser reemplazados
mediante la Ley de Ohm. Es importante destacar que la diferencia de potencial debe
respetar la convención utilizada con respecto a la corriente en cada resistor:

∆V = IR = (Ib − Ia )R
Donde Ib e Ia son las intensidades de las mallas que
ingresan por el polo positivo y negativo, respectivamente.

5. ¿Cuántas ecuaciones armar? La cantidad de ecuaciones debe ser igual a la cantidad
de incógnitas que haya. En caso de que falten ecuaciones, se puede utilizar la Ley
de Ohm en algún resistor, KCL y/o construir una supermalla. Esta última opción
se aplicará cuando se presente una fuente de corriente en medio de la malla.
6. Finalmente, se resuelve el sistema de ecuaciones.

---

### Página 21

2.7.1

“I2 2022-2”, Problema 2, Facultad de Física

Considere el circuito de la figura, donde Ra = 2 Ω, Rb = 4 Ω, Rc = 3 Ω, Rd = 2 Ω,
Re = 5 Ω, εA = 24 V y εB = 12 V.
a) Calcule el valor de las seis corrientes indicadas en este circuito.
b) Realice un balance de potencia para este circuito.
c) Para lograr que una sustancia eleve su temperatura rápidamente se requiere de un
aparato que libere energía a una tasa mínima de 150 Joules por segundo, ¿serviría
el circuito mostrado en la figura para realizar esta tarea?
d) Ahora, suponga que se apaga la fuente de voltaje εA . Determine la resistencia
equivalente de este nuevo circuito, vista desde los terminales de la fuente voltaje
εB .

Figura 8. Esquema circuital en estudio.

---

### Página 22

Solución a), b) y c)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la potencia entregada y/o disipada por cada elemento circuital. En primer
lugar, la potencia eléctrica se puede calcular utilizando la Ley de Joule:
P = V I = I 2R =

V2
R

Luego, se deberá resolver el circuito mediante algún método.
Finalmente, se debe comprobar que la potencia entregada es equivalente a la disipada:

X

PE =

X

PD

Paso 1: Preparación KVL
Es posible observar que se produce un cortocircuito en la parte inferior del circuito, puesto
que una rama sin ningún componente circuital está conectada en paralelo con otras ramas. La
corriente preferirá circular por aquel camino que menos se le oponga (i.e I4 = 0), por lo que el
circuito queda como:

Figura 9. Esquema KVL del circuito.
Como se presentan pocas mallas, se preferirá realizar este ejercicio mediante ese método.
Por simplicidad, se asignarán arbitrariamente corrientes que circulan en un mismo sentido.

---

### Página 23

Paso 2: Resolución KVL - IA e IB
Para armar las ecuaciones de KVL debemos observar una malla y recorrerla en el sentido
otorgado. Al pasar por un elemento circuital, se sumará su voltaje si se entra de + a − (en
caso contrario se resta):
Malla

Ecuación KVL

A

−εA + VRa + VRb + VRc = 0

B

−εB − VRc + VRd = 0

Luego, los voltajes provenientes de resistores son reemplazados mediante Ley de Ohm:

Malla

Ecuación KVL

A

−εA + IA Ra + IA Rb + (IA − IB )Rc = 0

B

−εB − (IA − IB )Rc + IB Rd = 0

Finalmente, se resuelve el sistema de ecuaciones:
IA =
IB =

εB Rc + εA (Rc + Rd )
(1 + Ra + Rb )(Rc + Rd )

εA Rc + εB (Ra + Rb + Rc )
(1 + Ra + Rb )(Rc + Rd )

Reemplazando valores se obtiene que:

A
IB = 5 A

IA =

(36)
(37)

---

### Página 24

Paso 3: Análisis Corrientes
Finalmente, se interpreta lo obtenido en relación a lo que se pide determinar por enunciado:
Intensidad

Expresión KVL

Valor

I1

−IA

− 13
3 A

I2

IA − IB

− 23 A

I3

IB

5A

I4

0A

I5

IB

5A

I6

IB

5A

Debemos siempre observar el sentido de las corrientes para dar con el resultado correcto.
Por ejemplo, IA e I1 circulan en sentidos contrarios dentro de la misma rama.

Paso 4: Balance Potencia Eléctrica
Finalmente, la potencia eléctrica entregada y/o disipada por cada uno de los componentes
circuitales se puede calcular utilizando la Ley de Joule:
P = V I = I 2R =

V2
R

Es importante notar que todas son equivalentes e igual de válidas.
Por conveniencia, se utilizará la que relaciona = I” y = R” para las resistencias
y la que relaciona = V ” e = I” para las fuentes, pues son datos conocidos:

Componente

Tipo Potencia

Expresión Potencia

Valor

εA

Entregada

PA = εA IA

104 W

εB

Entregada

PB = εB IB

60 W

Ra

Disipada

2R
Pa = IA
a

9 W

Rb

Disipada

2R
Pb = IA
b

9 W

Rc

Disipada

Pc = (IA − IB )2 Rc

3 W

Rd

Disipada

2R
Pd = IB
d

50 W

Re

Disipada

Pe = I42 Re

0W

---

### Página 25

Luego, y para el balance de potencia, es fácil comprobar que:

X
X

PD =

PE = 104 + 60 W = 164 W
338 676 4
+
+ + 50 W = 164 W

Finalmente, la potencia entregada es equivalente a la disipada
y, como 164 W > 150 W, el circuito sirve para realizar la tarea propuesta.

Paso Extra: Resolución KCL
Para otorgar una respuesta más completa, también se resolverá el circuito mediante el método
de nodos. Sabemos que en la rama inferior se produce un cortocircuito, por lo que el circuito
queda como:

Figura 10. Esquema KCL del circuito.
Por simplicidad, se asignará el nodo tierra en la esquina inferior izquierda.
También, se define el sentido de las corrientes que circulan por todo el circuito.

---

### Página 26

Para armar las ecuaciones de KCL debemos observar un nodo y considerar las corrientes que
entran y salen de este:
Nodo

Ecuación KCL

A

VA − 0 = εB

B

IRa +Rb = IRc + IRd

Se consideró que I2 = IRc y I3 = IRd .
Luego, las intensidades provenientes de resistores son reemplazados mediante la Ley de Ohm:

Nodo

Ecuación KCL

A

VA = εB

B

VA +εA −VB
A
= VBR−V
+ VBR−0
Ra +Rb
c
d

Finalmente, se resuelve el sistema de ecuaciones:
VA = εB
(εA Rc + εB (Ra + Rb + Rc ))Rd
VB =
(1 + Ra + Rb )(Rc + Rd )
Reemplazando valores se obtiene que:

VA = 12 V

(38)

VB = 10 V
(39)
Finalmente, se interpreta lo obtenido en relación a lo que se pide determinar por enunciado:
Intensidad

Expresión KCL

Valor

I1

VB −(VA +εA )
Ra +Rb

− 13
3 A

I2

VB −VA
Rc

− 23 A

I3

VB −0
Rd

5A

I4

0A

I5

VB −0
Rd

5A

I6

VB −0
Rd

5A

Debemos siempre observar el sentido de las corrientes para dar con el resultado correcto.
Además, I5 = I6 pues circulan en el mismo sentido dentro de la misma rama.
El análisis es análogo para el resto de los ítems a partir del método KCL.

---

### Página 27

Solución d)
Paso Único: Resistencia Equivalente
Se pide determinar la resistencia equivalente del circuito luego de apagar εA . Si una fuente de
voltaje se apaga, esta es retirada y sus terminales siguen unidos, por lo que el circuito queda
como:

Figura 11. Esquema sobre la reducción de resistencias del circuito.
Del esquema, se nota que Ra está conectada en serie con Rb :

R1 = Ra + Rb
Asimismo, se nota que Ra + Rb está conectada en paralelo con Rc :

R2 = (Ra + Rb )//Rc
Finalmente, se nota que (Ra + Rb )//Rc está conectada en serie con Rd :

Req = (Ra + Rb )//Rc + Rd
Rc (Ra + Rb )
=
+ Rd
Ra + Rb + Rc
Reemplazando valores se obtiene que:

Req = 4 Ω

(40)
