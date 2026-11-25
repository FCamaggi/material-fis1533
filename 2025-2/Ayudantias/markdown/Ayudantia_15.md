---
title: "Ayudantia 15"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_15_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_15_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 15

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 15
07 de Octubre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Circuitos RC

1.1

Circuitos RC - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Aplicar las Leyes de Kirchoff para corrientes (KCL) y voltajes (KVL) en diversos circuitos
□
RC.
✓ Resolver EDOs de carácter separable en el contexto de circuitos RC.
□
✓ Determinar y aplicar las condiciones iniciales necesarias para la EDO según el contexto.
□
✓ Determinar el voltaje en un capacitor según el contexto en diversos circuitos RC.
□
✓ Determinar la intensidad de corriente que circula por un capacitor según el contexto en
□
diversos circuitos RC.
✓ Calcular la carga y energía almacenada en un capacitor en el contexto de circuitos RC.
□
✓ Interpretar y determinar la constante de tiempo capacitiva en diversos circuitos RC.
□
□ Identificar capacitores conectados en serie y paralelo en diversas configuraciones.
□ Determinar la capacitancia equivalente de una configuración mediante el método de
conexiones.

✓ Utilizar límites matemáticos y técnicas relacionadas, tales como la regla de L’hopital.
□
✓ Utilizar derivadas y técnicas relacionadas, tales como la regla del producto y cuociente.
□

---

### Página 2

1.2

Circuitos RC - Condensadores

Un conjunto de = N ” capacitores puede conectarse de distintas formas:
Conexión

Capacitancia Equivalente

Efectos Eléctricos

Serie

PN 1
i Ci
Ceq =

Misma Corriente en cada Ci

Paralelo

Ceq =

PN
i

Ci

Mismo Voltaje en cada Ci

(a) Capacitores conectados en serie

(b) Capacitores conectados en paralelo

Figura 1. Diagramas sobre las configuraciones de capacitores.

1.3

Circuitos RC - Cómo Utilizarlo Correctamente

Los llamados circuitos RC contienen tanto capacitores como resistores. Una guía para resolver
este tipo de ejercicios se presenta a continuación:
1. En general, resulta más fácil utilizar el método de mallas, aunque el circuito puede ser
resuelto mediante cualquier método:
X
Vk = 0
malla

Al llegar al capacitor se deberá sumar o restar su voltaje, dependiendo si la
corriente ingresa por el terminal positivo o negativo asignado previamente.

2. Automáticamente, los voltajes provenientes de resistores deberán ser reemplazados mediante la Ley de Ohm.
3. Luego, deberán expresar la intensidad que circula por el capacitor en función de la(s)
intensidad(es) de la(s) malla(s), de forma de armar la EDO respectiva:
IC (t) =

dQ(t)
dVC (t)

(1)

---

### Página 3

Recordemos que la energía almacenada por el capacitor cambia a medida que este se carga
o descarga. Además, la ecuación anterior proviene de la definición de intensidad y de carga
en el capacitor = Q = CV ”: al momento de reemplazar, solo el voltaje se verá afectado por
el diferencial, puesto que la capacitancia se considera como una constante.

4. En general, la EDO será de tipo separable y se recomienda resolverla para el voltaje del
capacitor, por lo que se dejará a un lado de la ecuación solo variables dependientes de
“VC ” y al otro solo variables dependientes del tiempo y/o constantes:
α(VC ) · dVC = β(t) · dt
Luego, quedará integrar a ambos lados y despejar = VC ”:

Z t

Z VC

β(t) · dt

α(VC ) · dVC =
t0

V0

Donde = α” y = β” son variables que dependen de = VC ” y = t”, respectivamente.
Por otra parte, = V0 ” es la condición inicial de voltaje para el capacitor y = t0 ”
el tiempo inicial o desde donde se considera la carga/descarga del mismo.

5. ¿Cómo determinar las condiciones iniciales del capacitor? Se debe leer bien el enunciado:
a) En ocasiones se dirá explícitamente que el condensador se encontraba descargado
(i.e Q = 0), por lo que su diferencia de potencial también será nula.
b) En otros casos, se dirá implícitamente que el capacitor se ha cargado completamente,
puesto que el circuito se ha estado alimentando = durante mucho tiempo” con una
entrada de voltaje. Al alcanzar su carga máxima, el condensador se comporta como
circuito abierto, puesto que ya no hay cambios en su voltaje con respecto al tiempo:
IC (t) =

dQ(t)
dVC (t)
=0

6. Por último, les debería quedar una solución de la siguiente forma:
VC (t) = VC (∞) + (V0 − VC (∞))e−t/τ

(2)

Donde = τ ” es la constante de tiempo, la cual indica qué tan lento o rápido se carga el capacitor.
Por otra parte, = VC (∞)” se refiere a cómo se comporta el voltaje del capacitor en el infinito.
Para circuitos de primer orden, se cumple que:

τ = C · RT h

(3)

Donde = RT h ” es la resistencia de Thèvenin.

7. Si es que piden determinar la intensidad que circula por el capacitor o la carga de este a
través del tiempo, se puede ingresar la solución obtenida en las expresiones anteriores:
IC (t) =

dQ(t)
dVC (t)

Q(t) = CVC (t)
Si es que se requiere otra variable (i.e la intensidad/voltaje en alguna resistencia),
siempre se puede utilizar KCL, KVL, Ley de Ohm, entre otros. Si se requiere analizar
variables en el infinito, se debe utilizar la herramienta de límite matemático.

---

### Página 4

1.3.1

“Ejercicios Teoría Electromagnética ”, 11.5.5, Fabián Cádiz

Inicialmente, el circuito de la figura ha estado abierto durante mucho tiempo.
a) Calcule la carga que el condensador alcanza con el interruptor abierto.
b) Calcule la energía que el condensador alcanza con el interruptor abierto.
c) Determine el voltaje, la intensidad de corriente y carga que circula por el condensador en función del tiempo luego de que el interruptor es cerrado.
d) ¿Cuál es la constante de tiempo capacitiva luego de que el interruptor es cerrado?
e) Si el interruptor se cierra y transcurre mucho tiempo, encuentre la nueva carga del
condensador.

Solución a)
Paso Único: Condiciones Iniciales
Se pide determinar la carga en el condensador con el interruptor abierto. Si este ha estado
abierto durante mucho tiempo, la fuente de voltaje V2 entregará una constante alimentación al
capacitor y, eventualmente, alcanzará su carga máxima. En este punto su carga ya no puede
variar, por lo que se comportará como circuito abierto:
dQ
=0
Finalmente, se utiliza la expresión que relaciona carga almacenada con capacitancia:
IC =

Q = CVC

(4)

---

### Página 5

Solución b)
Paso Único: Energía Almacenada
Se pide determinar la energía almacenada en t = 0, por lo que se debe utilizar la siguiente
expresión:
U=

1 Q2
= CV 2 = QV
2 C

Solución c), d) y e)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el voltaje, la intensidad de corriente y la carga que circula por el condensador
en función del tiempo, luego de que el interruptor es cerrado. Luego, se deberá resolver el
circuito mediante algún método, de forma de armar la EDO respectiva:
IC =

dVC
dQ

Además, se deben aplicar las condiciones iniciales en relación al capacitor.

---

### Página 6

1.3.2

“Análisis de Circuitos Eléctricos”, 6.4, Berríos F. & Sáez C.

El circuito de la figura ha estado operando por mucho tiempo, hasta que en t = 0 un
interruptor cambia su topología.

a) Reduzca el circuito de manera que quede de la siguiente forma:

---

### Página 7

b) Calcule la carga almacenada por el capacitor en t = 0.
c) Determine el voltaje, la carga y la intensidad de corriente que circula por el capacitor para t > 0.
d) ¿Cuál es la constante de tiempo capacitiva luego de que el interruptor es cerrado?
e) Encuentre la nueva carga del condensador, luego de que ha transcurrido mucho
tiempo con el interruptor cerrado.

Solución a)
Paso Único: Resistencia Equivalente
Se pide reducir el circuito hasta obtener la forma deseada. Es posible observar que se produce
un cortocircuito en la parte superior del circuito, puesto que una rama sin ningún componente
circuital está conectada en paralelo con otras ramas.

Solución b)
Paso Único: Condiciones Iniciales
Se pide determinar la carga almacenada por el capacitor en t = 0. Si el circuito ha estado
operando en este estado durante mucho tiempo, la fuente de voltaje V1 entregará una constante
alimentación al capacitor y, eventualmente, alcanzará su carga máxima. En este punto su carga
ya no puede variar, por lo que se comportará como circuito abierto:
IC =

dQ
=0

Solución c), d) y e)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el voltaje, la intensidad de corriente y la carga que circula por el capacitor
para t > 0, o sea, al cambiar la topología. Luego, se deberá resolver el circuito mediante algún
método, de forma de armar la EDO respectiva:
IC =

dQ
dVC

Además, se deben aplicar las condiciones iniciales en relación al capacitor.

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 15
07 de Octubre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Circuitos RC

1.1

Circuitos RC - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Aplicar las Leyes de Kirchoff para corrientes (KCL) y voltajes (KVL) en diversos circuitos
□
RC.
✓ Resolver EDOs de carácter separable en el contexto de circuitos RC.
□
✓ Determinar y aplicar las condiciones iniciales necesarias para la EDO según el contexto.
□
✓ Determinar el voltaje en un capacitor según el contexto en diversos circuitos RC.
□
✓ Determinar la intensidad de corriente que circula por un capacitor según el contexto en
□
diversos circuitos RC.
✓ Calcular la carga y energía almacenada en un capacitor en el contexto de circuitos RC.
□
✓ Interpretar y determinar la constante de tiempo capacitiva en diversos circuitos RC.
□
□ Identificar capacitores conectados en serie y paralelo en diversas configuraciones.
□ Determinar la capacitancia equivalente de una configuración mediante el método de
conexiones.

✓ Utilizar límites matemáticos y técnicas relacionadas, tales como la regla de L’hopital.
□
✓ Utilizar derivadas y técnicas relacionadas, tales como la regla del producto y cuociente.
□

---

### Página 2

1.2

Circuitos RC - Condensadores

Un conjunto de = N ” capacitores puede conectarse de distintas formas:
Conexión

Capacitancia Equivalente

Efectos Eléctricos

Serie

PN 1
i Ci
Ceq =

Misma Corriente en cada Ci

Paralelo

Ceq =

PN
i

Ci

Mismo Voltaje en cada Ci

(a) Capacitores conectados en serie

(b) Capacitores conectados en paralelo

Figura 1. Diagramas sobre las configuraciones de capacitores.

1.3

Circuitos RC - Cómo Utilizarlo Correctamente

Los llamados circuitos RC contienen tanto capacitores como resistores. Una guía para resolver
este tipo de ejercicios se presenta a continuación:
1. En general, resulta más fácil utilizar el método de mallas, aunque el circuito puede ser
resuelto mediante cualquier método:
X
Vk = 0
malla

Al llegar al capacitor se deberá sumar o restar su voltaje, dependiendo si la
corriente ingresa por el terminal positivo o negativo asignado previamente.

2. Automáticamente, los voltajes provenientes de resistores deberán ser reemplazados mediante la Ley de Ohm.
3. Luego, deberán expresar la intensidad que circula por el capacitor en función de la(s)
intensidad(es) de la(s) malla(s), de forma de armar la EDO respectiva:
IC (t) =

dQ(t)
dVC (t)
=C

(1)

---

### Página 3

Recordemos que la energía almacenada por el capacitor cambia a medida que este se carga
o descarga. Además, la ecuación anterior proviene de la definición de intensidad y de carga
en el capacitor = Q = CV ”: al momento de reemplazar, solo el voltaje se verá afectado por
el diferencial, puesto que la capacitancia se considera como una constante.

4. En general, la EDO será de tipo separable y se recomienda resolverla para el voltaje del
capacitor, por lo que se dejará a un lado de la ecuación solo variables dependientes de
“VC ” y al otro solo variables dependientes del tiempo y/o constantes:
α(VC ) · dVC = β(t) · dt
Luego, quedará integrar a ambos lados y despejar = VC ”:

Z t

Z VC

β(t) · dt

α(VC ) · dVC =
t0

V0

Donde = α” y = β” son variables que dependen de = VC ” y = t”, respectivamente.
Por otra parte, = V0 ” es la condición inicial de voltaje para el capacitor y = t0 ”
el tiempo inicial o desde donde se considera la carga/descarga del mismo.

5. ¿Cómo determinar las condiciones iniciales del capacitor? Se debe leer bien el enunciado:
a) En ocasiones se dirá explícitamente que el condensador se encontraba descargado
(i.e Q = 0), por lo que su diferencia de potencial también será nula.
b) En otros casos, se dirá implícitamente que el capacitor se ha cargado completamente,
puesto que el circuito se ha estado alimentando = durante mucho tiempo” con una
entrada de voltaje. Al alcanzar su carga máxima, el condensador se comporta como
circuito abierto, puesto que ya no hay cambios en su voltaje con respecto al tiempo:
IC (t) =

dQ(t)
dVC (t)
=C
=0

6. Por último, les debería quedar una solución de la siguiente forma:
VC (t) = VC (∞) + (V0 − VC (∞))e−t/τ

(2)

Donde = τ ” es la constante de tiempo, la cual indica qué tan lento o rápido se carga el capacitor.
Por otra parte, = VC (∞)” se refiere a cómo se comporta el voltaje del capacitor en el infinito.
Para circuitos de primer orden, se cumple que:

τ = C · RT h

(3)

Donde = RT h ” es la resistencia de Thèvenin.

7. Si es que piden determinar la intensidad que circula por el capacitor o la carga de este a
través del tiempo, se puede ingresar la solución obtenida en las expresiones anteriores:
IC (t) =

dQ(t)
dVC (t)
=C

Q(t) = CVC (t)
Si es que se requiere otra variable (i.e la intensidad/voltaje en alguna resistencia),
siempre se puede utilizar KCL, KVL, Ley de Ohm, entre otros. Si se requiere analizar
variables en el infinito, se debe utilizar la herramienta de límite matemático.

---

### Página 4

1.3.1

“Ejercicios Teoría Electromagnética ”, 11.5.5, Fabián Cádiz

Inicialmente, el circuito de la figura ha estado abierto durante mucho tiempo.
a) Calcule la carga que el condensador alcanza con el interruptor abierto.
b) Calcule la energía que el condensador alcanza con el interruptor abierto.
c) Determine el voltaje, la intensidad de corriente y carga que circula por el condensador en función del tiempo luego de que el interruptor es cerrado.
d) ¿Cuál es la constante de tiempo capacitiva luego de que el interruptor es cerrado?
e) Si el interruptor se cierra y transcurre mucho tiempo, encuentre la nueva carga del
condensador.

Solución a)
Paso Único: Condiciones Iniciales
Se pide determinar la carga en el condensador con el interruptor abierto. Si este ha estado
abierto durante mucho tiempo, la fuente de voltaje V2 entregará una constante alimentación al
capacitor y, eventualmente, alcanzará su carga máxima. En este punto su carga ya no puede
variar, por lo que se comportará como circuito abierto:
dQ
=0
Es posible observar que se produce un circuito abierto tanto por el interruptor en la parte
izquierda como por el capacitor en la parte central del circuito. La corriente eléctrica no puede
circular por tales ramas, por lo que el circuito queda como:
IC =

---

### Página 5

Figura 2. Esquema sobre las condiciones iniciales del circuito.
Luego, el voltaje entre los terminales del capacitor estará dado por:

VC (0) = V2
Finalmente, se utiliza la expresión que relaciona carga almacenada con capacitancia:
Q(0) = CVC (0)
= CV2

(4)

Solución b)
Paso Único: Energía Almacenada
Se pide determinar la energía almacenada en t = 0, por lo que se debe utilizar la siguiente
expresión:
U=

1 Q2
= CV 2 = QV
2 C

Es importante notar que todas son equivalentes e igual de válidas.
No obstante, por conveniencia se utilizará la que relaciona = C” y = V ”, pues son datos que ya se tienen:

U (0) = CVC (0)2
CV22
=

(5)

Solución c), d) y e)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el voltaje, la intensidad de corriente y la carga que circula por el condensador
en función del tiempo, luego de que el interruptor es cerrado. Luego, se deberá resolver el
circuito mediante algún método, de forma de armar la EDO respectiva:
IC =

dQ
dVC
=C

Además, se deben aplicar las condiciones iniciales en relación al capacitor.

---

### Página 6

Paso 1: Preparación KVL
Como se presentan pocas mallas, se preferirá realizar este ejercicio mediante ese método:

Figura 3. Esquema KVL del circuito (interruptor cerrado).
Por simplicidad, se asignarán arbitrariamente corrientes que circulan en un mismo sentido.
Además, los polos de las fuentes de voltaje están predefinidos por el tamaño de las placas.

Paso 2: Resolución KVL - I1 e I2
Para armar las ecuaciones de KVL debemos observar una malla y recorrerla en el sentido
otorgado. Al pasar por un elemento circuital, se sumará su voltaje si se entra de + a − (en
caso contrario se resta):
Malla

Ecuación KVL

−V1 + VC + VR1 = 0

−VC + V2 + VR2 = 0

Luego, los voltajes provenientes de resistores son reemplazados mediante Ley de Ohm:

Malla

Ecuación KVL

−V1 + VC + I1 R1 = 0

−VC + V2 + I2 R2 = 0

C
Para obtener la EDO, se aplicará la expresión IC = I1 − I2 = C dV
dt :

Malla

Ecuación KVL

−V1 + VC + (I2 + C dVdtC )R1 = 0

I2 = VCR−V

---

### Página 7

Combinando ambas ecuaciones:

VC − V 2
dVC
+C
)R1 = 0
R2
dVC
R1 V2
R1
−V1 −
+ VC (1 +
) + CR1
=0
R2
R2
−V1 + VC + (

(6)

Por simplicidad, se reescribirá α = −V1 − RR1 V2 2 y β = 1 + R
R2 :

α + βVC + CR1

dVC
=0

(7)

Paso 3: Resolución EDO - VC (t)
La EDO se puede tratar mediante el método de separación de variables, por lo que se dejará a
un lado de la ecuación solo variables dependientes de = VC ” y al otro solo variables dependientes
del tiempo y/o constantes:
dVC
=0
dVC
−
=
CR1
α + βVC

α + βVC + CR1

Integrando con condiciones iniciales generales:

Z t

−
=
CR1
t0

Z VC

dVC
VC (0) α + βVC

Arbitrariamente, diremos que el interruptor se cierra en t = 0 (i.e t ∈ [0, ∞[).
Asimismo, el condensador estará sometido a cierta diferencia de potencial inicial VC (0) = V2 :

Z t
−

=
CR1

Z VC
V2

dVC
α + βVC

Z α+βVC

t
du
=
CR1
βu
α+βV2
βt
α + βVC
−
= ln (
)
CR1
α + βV2
−

Notar que se realizó un cambio de variable u = α + βVC → du = β dVC .
Por último, despejamos VC aplicando exponencial:

α + βVC
α + βV2
α
α
− βt
VC (t) = − + ( + V2 )e CR1
β
β
βt
− CR

e

=

(8)

---

### Página 8

Paso 4: Constante de Tiempo Capacitiva - τ
Observando y comparando lo obtenido, la constante de tiempo capacitiva vendrá dada por:
−

t
βt
=−
τ
CR1
CR1
τ=
β

Reescribiendo se obtiene que:

τ=

CR1 R2
R1 + R 2

(9)

Paso 5: Intensidad Corriente Capacitor - IC (t)
Utilizando la expresión que relaciona la intensidad de corriente con el voltaje en el capacitor:
dVC (t)
d
α
α
− βt
= C (− + ( + V2 )e CR1 )
dt β
β
β
α
− βt
= C( + V2 )e CR1 · −
β
CR1
βt
β α
− CR
= − ( + V2 )e
R1 β

IC (t) = C

(10)

Paso 6: Carga Capacitor - Q(t) y Q(∞)
Por último, se ocupa la expresión que relaciona carga almacenada con capacitancia:
Q(t) = CVC (t)
Cα
α
− βt
=−
+ C( + V2 )e CR1
β
β
Además, y si transcurre mucho tiempo luego de que el interruptor se cierra (i.e t → ∞), la
carga en el capacitor será:
Q(∞) = lim Q(t)
t→∞

= lim −
t→∞

=−

Cα
α
− βt
+ C( + V2 )e CR1
β
β

Cα
β

Reescribiendo se obtiene que:

Cα
β
C(V1 + RR1 V2 2 )

Q(∞) = −
=

1 + R1 /R2
R1 V2 + R2 V1
= C(
)
R1 + R2

(11)

---

### Página 9

1.3.2

“Análisis de Circuitos Eléctricos”, 6.4, Berríos F. & Sáez C.

El circuito de la figura ha estado operando por mucho tiempo, hasta que en t = 0 un
interruptor cambia su topología.

a) Reduzca el circuito de manera que quede de la siguiente forma:

---

### Página 10

b) Calcule la carga almacenada por el capacitor en t = 0.
c) Determine el voltaje, la carga y la intensidad de corriente que circula por el capacitor para t > 0.
d) ¿Cuál es la constante de tiempo capacitiva luego de que el interruptor es cerrado?
e) Encuentre la nueva carga del condensador, luego de que ha transcurrido mucho
tiempo con el interruptor cerrado.

Solución a)
Paso Único: Resistencia Equivalente
Se pide reducir el circuito hasta obtener la forma deseada. Es posible observar que se produce
un cortocircuito en la parte superior del circuito, puesto que una rama sin ningún componente
circuital está conectada en paralelo con otras ramas. La corriente preferirá circular por aquel
camino que menos se le oponga, por lo que el circuito queda como:

Figura 4. Esquema sobre la reducción de resistencias del circuito.

---

### Página 11

Del esquema, se nota que R1 está conectada en serie con R2 :

Req,1 = R1 + R2
Asimismo, se nota que R1 + R2 está conectada en paralelo con R3
y que R5 está conectada en paralelo con R8 :

Req,2 = (R1 + R2 )//R3
Req,3 = R5 //R8
Finalmente, se nota que (R1 + R2 )//R3 está conectada en serie con R5 //R8 :

Ra = [(R1 + R2 )//R3 ] + R5 //R8

(12)

Solución b)
Paso Único: Condiciones Iniciales
Se pide determinar la carga almacenada por el capacitor en t = 0. Si el circuito ha estado
operando en este estado durante mucho tiempo, la fuente de voltaje V1 entregará una constante
alimentación al capacitor y, eventualmente, alcanzará su carga máxima. En este punto su carga
ya no puede variar, por lo que se comportará como circuito abierto:
dQ
=0
Es posible observar que se produce un circuito abierto tanto por el interruptor como por el
capacitor en la parte central del circuito. La corriente eléctrica no puede circular por tales
ramas, por lo que el circuito queda como:
IC =

Figura 5. Esquema sobre las condiciones iniciales del circuito.
Luego, el voltaje entre los terminales del capacitor estará dado por:

VC (0) = V1
Finalmente, se utiliza la expresión que relaciona carga almacenada con capacitancia:
Q(0) = CVC (0)
= CV1

(13)

---

### Página 12

Solución c), d) y e)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el voltaje, la intensidad de corriente y la carga que circula por el capacitor
para t > 0, o sea, al cambiar la topología. Luego, se deberá resolver el circuito mediante algún
método, de forma de armar la EDO respectiva:
IC =

dQ
dVC
=C

Además, se deben aplicar las condiciones iniciales en relación al capacitor.

Paso 1: Preparación KVL
Para t > 0, el circuito queda como:

Figura 6. Esquema KVL del circuito (interruptor cerrado).
Como se presentan pocas mallas, se preferirá realizar este ejercicio mediante ese método.
Por simplicidad, se asignarán arbitrariamente corrientes que circulan en un mismo sentido.

Paso 2: Resolución KVL - IA e IB
Para armar las ecuaciones de KVL debemos observar una malla y recorrerla en el sentido
otorgado. Al pasar por un elemento circuital, se sumará su voltaje si se entra de + a − (en
caso contrario se resta):
Malla

Ecuación KVL

A

−VC + V2 + VR6 = 0

B

−VR6 − V3 + VR7 = 0

Luego, los voltajes provenientes de resistores son reemplazados mediante Ley de Ohm:

---

### Página 13

Malla

Ecuación KVL

A

−VC + V2 + (IA − IB )R6 = 0

B

−(IA − IB )R6 − V3 + IB R7 = 0
Para obtener la EDO:

Malla

Ecuación KVL

A

−VC + V2 + (IA − IB )R6 = 0

B

6 +V3
IB = IARR
6 +R7

C
Combinando ambas ecuaciones y aplicando la expresión IC = −IA = C dV
dt :

IA R6 + V3
)R6 = 0
R6 + R7
R6
V3 R6
−VC + V2 + IA R6 (1 −
)−
=0
R6 + R7
R6 + R 7
dVC R6 R7
V3 R6
−VC + −C
−
+ V2 = 0
dt R6 + R7 R6 + R7
−VC + V2 + (IA −

R7
R6
+ V2 y β = RR66+R
:
Por simplicidad, se reescribirá α = − RV63+R

−VC − βC

dVC
+α=0

(14)

Paso 3: Resolución EDO - VC (t)
La EDO se puede tratar mediante el método de separación de variables, por lo que se dejará a
un lado de la ecuación solo variables dependientes de = VC ” y al otro solo variables dependientes
del tiempo y/o constantes:
−VC − βC

dVC
+α=0
dVC
=
βC
α − VC

Integrando con condiciones iniciales generales:

Z t

=
βC
t0

Z VC

dVC
α
− VC
VC (0)

El interruptor cambia de posición en t = 0 (i.e t ∈ [0, ∞[).
Asimismo, el condensador estará sometido a cierta diferencia de potencial inicial VC (0) = V1 :

---

### Página 14

Z t

=
0 βC

Z VC
V1

dVC
α − VC

Z α−VC
du
t
−
=
βC
u
α−V1
t
α − VC
)
−
= ln (
βC
α − V1
Notar que se realizó un cambio de variable u = α − VC → du = −dVC .
Por último, despejamos VC aplicando exponencial:

e

t
− βC

=

α − VC
α − V1

(15)
t
− βC

VC (t) = α + (V1 − α)e
Paso 4: Constante de Tiempo Capacitiva - τ

Observando y comparando lo obtenido, la constante de tiempo capacitiva vendrá dada por:
−

t
t
=−
τ
βC
τ = βC

Reescribiendo se obtiene que:

τ=

CR6 R7
R6 + R 7

(16)

Paso 5: Intensidad Corriente Capacitor - IC (t)
Utilizando la expresión que relaciona la intensidad de corriente con el voltaje en el capacitor:
dVC (t)
d
− t
= C (α + (V1 − α)e βC )
− t
= C(V1 − α)e βC · −
βC
− t
= − (V1 − α)e βC
β

IC (t) = C

Paso 6: Carga Capacitor - Q(t) y Q(∞)
Por último, se utiliza la expresión que relaciona carga almacenada con capacitancia:
Q(t) = CVC (t)
t
− βC

= Cα + C(V1 − α)e

(17)

---

### Página 15

Además, y si transcurre mucho tiempo luego de que el interruptor se cierra (i.e t → ∞), la
carga en el capacitor será:
Q(∞) = lim Q(t)
t→∞

t
− βC

= lim Cα + C(V1 − α)e
t→∞

= Cα
Reescribiendo se obtiene que:

Q(∞) = C(−

V3 R6
+ V2 )
R6 + R7

(18)
