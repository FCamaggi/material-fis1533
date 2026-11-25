---
title: "Ayudantia 27"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_27_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_27_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 27

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Ayudantía 27
18 de Noviembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Circuitos RL

1.1

Circuitos RL - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Aplicar las Leyes de Kirchoff para corrientes (KCL) y voltajes (KVL) en diversos circuitos
□
RL.
✓ Resolver EDOs de carácter separable en el contexto de circuitos RL.
□
✓ Determinar y aplicar las condiciones iniciales necesarias para la EDO según el contexto.
□
✓ Determinar el voltaje en un inductor según el contexto en diversos circuitos RL.
□
✓ Determinar la intensidad de corriente que circula por un inductor según el contexto en
□
diversos circuitos RL.
✓ Calcular el flujo magnético y energía almacenada en un inductor en el contexto de cir□
cuitos RL.
✓ Interpretar y determinar la constante de tiempo inductiva en diversos circuitos RL.
□
□ Identificar inductores conectados en serie y paralelo en diversas configuraciones.
□ Determinar la inductancia equivalente de una configuración mediante el método de conexiones.

✓ Utilizar límites matemáticos y técnicas relacionadas, tales como la regla de L’hopital.
□
✓ Utilizar derivadas y técnicas relacionadas, tales como la regla del producto y cuociente.
□

---

### Página 2

1.2

Circuitos RL - Inductores

Un inductor (o bobina) es un componente circuital pasivo de dos terminales que almacena
energía en forma de campo magnético, oponiéndose así a cambios bruscos en el valor de la
corriente. Un conjunto de = N ” inductores puede conectarse de distintas formas:
Conexión
Serie

Inductancia Equivalente
Leq =

Paralelo

PN

Efectos Eléctricos

Li

Misma Corriente en cada Li

PN 1
i Li
Leq =

Mismo Voltaje en cada Li

i

(a) Inductores conectados en serie

(b) Inductores conectados en paralelo

Figura 1. Diagramas sobre las configuraciones de inductores.

1.3

Circuitos RL - Cómo Utilizarlo Correctamente

Los llamados circuitos RL contienen tanto inductores como resistores. Una guía para resolver
este tipo de ejercicios se presenta a continuación:
1. En general, resulta más fácil utilizar el método de mallas, aunque el circuito puede ser
resuelto mediante cualquier método:
X
Vk = 0
malla

Al llegar al inductor se deberá sumar o restar su voltaje, dependiendo si la
corriente ingresa por el terminal positivo o negativo asignado previamente.

2. Automáticamente, los voltajes provenientes de resistores deberán ser reemplazados mediante la Ley de Ohm.
3. Luego, deberán expresar la diferencia de potencial en el inductor en función de la(s)
intensidad(es) de la(s) malla(s), de forma de armar la EDO respectiva:

dIL (t)
dΦL (t)
=L

(1)

---

### Página 3

Recordemos que la energía almacenada por el inductor cambia a medida que este se carga
o descarga. Además, la ecuación anterior proviene de la definición de voltaje y de flujo
magnético en el inductor = ΦL = LI”: al momento de reemplazar, solo la corriente se
verá afectado por el diferencial, puesto que la inductancia se considera como una constante.

4. En general, la EDO será de tipo separable y se recomienda resolverla para la corriente
del inductor, por lo que se dejará a un lado de la ecuación solo variables dependientes de
“IL ” y al otro solo variables dependientes del tiempo y/o constantes:
α(IL ) · dIL = β(t) · dt
Luego, quedará integrar a ambos lados y despejar = IL ”:

Z t

Z IL

β(t) · dt

α(IL ) · dIL =
t0

I0

Donde = α” y = β” son variables que dependen de = IL ” y = t”, respectivamente.
Por otra parte, = I0 ” es la condición inicial de corriente para el inductor y = t0 ”
el tiempo inicial o desde donde se considera la carga/descarga del mismo.

5. ¿Cómo determinar las condiciones iniciales del inductor? Se debe leer bien el enunciado:
a) En ocasiones se dirá explícitamente que el inductor se encontraba descargado (i.e
ϕL = 0), por lo que su intensidad de corriente también será nula.
b) En otros casos, se dirá implícitamente que el inductor se ha cargado completamente,
puesto que el circuito se ha estado alimentando = durante mucho tiempo” con una
entrada de voltaje. Al alcanzar su flujo magnético máximo, el inductor se comporta
como cortocircuito, puesto que ya no hay cambios en su corriente con respecto al
tiempo:
dΦL (t)
dIL (t)
=L
=0
6. Por último, les debería quedar una solución de la siguiente forma:
IL (t) = IL (∞) + (I0 − IL (∞))e−t/τ

(2)

Donde = τ ” es la constante de tiempo, la cual indica qué tan lento o rápido se carga el inductor.
Por otra parte, = IL (∞)” se refiere a cómo se comporta la corriente del inductor en el infinito.
Para circuitos de primer orden, se cumple que:

τ=

L
RT h

(3)

Donde = RT h ” es la resistencia de Thèvenin.

7. Si es que piden determinar la diferencia de potencial en el inductor o el flujo magnético
de este a través del tiempo, se puede ingresar la solución obtenida en las expresiones
anteriores:
dΦL
dIL (t)
=L
ΦL (t) = LI(t)
Si es que se requiere otra variable (i.e la intensidad/voltaje en alguna resistencia),
siempre se puede utilizar KCL, KVL, Ley de Ohm, entre otros. Si se requiere analizar
variables en el infinito, se debe utilizar la herramienta de límite matemático.

---

### Página 4

1.3.1

“Problemas Resueltos de Electromagnetismo”, 16.12, Rodrigo Chi

En el circuito de la figura se ha tenido conectada la batería por mucho tiempo con el
interruptor S abierto. Luego en t = 0, el interruptor se cierra. Considere que V0 = 120 V,
R1 = R2 = 30 Ω y L = 50 mH.
a) Calcule el flujo magnético almacenado por el inductor en t = 0.
b) Determine la intensidad de corriente que circula por el inductor para t > 0.
c) Determine la diferencia de potencial en el inductor para t > 0.
d) ¿Cuál es la constante de tiempo inductiva luego de que se cierra el interruptor?
e) Encuentre la nueva corriente que circula por el inductor, luego de que ha transcurrido mucho tiempo con el interruptor cerrado.
f) Grafique la intensidad de corriente que circula por el inductor para t > 0.

Figura 2. Esquema Circuito RL.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el flujo magnético almacenado en t = 0 . Si el circuito ha estado operando
en tales estados durante mucho tiempo, la fuente de voltaje V0 entregará una constante alimentación al inductor y, eventualmente, alcanzará su flujo magnético máximo. En este punto
su flujo magnético ya no puede variar, por lo que se comportará como cortocircuito:
dΦL
=0
Finalmente, se utiliza la fórmula que relaciona flujo almacenado con inductancia:

ΦL = LI

---

### Página 5

Solución b), c), d), e) y f )
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la corriente I(t) que circula por el circuito, para un t ≥ 0. Luego, se deberá
resolver el circuito mediante algún método, de forma de armar la EDO respectiva:

dΦL
dIL (t)
=L

Además, se deben aplicar las condiciones iniciales en relación al inductor.

Circuitos de Segundo Orden

2.1

Circuitos de Segundo Orden - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Aplicar las Leyes de Kirchoff para corrientes (KCL) y voltajes (KVL) en diversos circuitos
□
RLC.
✓ Resolver EDOs de segundo orden homogéneas en el contexto de circuitos RLC.
□
□ Resolver EDOs de segundo orden no homogéneas en el contexto de circuitos RLC.

✓ Determinar y aplicar las condiciones iniciales necesarias para la EDO según el contexto.
□
✓ Determinar el voltaje e intensidad de corriente que circula por un componente circuital
□
según el contexto en diversos circuitos RLC.
✓ Identificar y determinar la frecuencia natural y el coeficiente de amortiguación en diversos
□
circuitos RLC.
✓ Identificar y conocer el tipo de respuesta para diversos circuitos RLC.
□
✓ Conocer el gráfico asociado a cada tipo de respuesta para diversos circuitos RLC.
□
✓ Utilizar límites matemáticos y técnicas relacionadas, tales como la regla de L’hopital.
□
✓ Utilizar derivadas y técnicas relacionadas, tales como la regla del producto y cuociente.
□

---

### Página 6

2.2

Circuitos de Segundo Orden - Generalidades

En circuitos de segundo orden, las corrientes y voltajes satisfacen una ecuación de la forma:
d2 x(t)
dx(t)
+ 2ζw0
+ w02 x(t) = g(t)

(4)

Donde = ζ” es el coeficiente de amortiguación y = w0 ” la frecuencia natural del sistema.

Luego, la solución de la ecuación será de la siguiente manera:
x(t) = xh (t) + xp (t)

(5)

Donde xh (t) y xp (t) son la solución homogénea y particular, respectivamente.
Reemplazando xh (t) = ert en la ecuación homogénea, se obtiene su polinomio característico:

r2 + 2ζw0 r + w02 = 0

(6)

De esta manera, las raíces del polinomio serán:

r1,2 = −ζw0 ± w0

p
ζ2 − 1

Dependiendo de sus valores, habrán tres tipos de soluciones:

Tipo Respuesta

Expresión Respuesta

Raíces

Valor ζ

Subamortiguada

xh (t) = e−ζw0 t (k1 cos (wd t) + k2 sin (wd t))

Complejas
Conjugadas

ζ<1

Críticamente
Amortiguada

xh (t) = k1 e−ζw0 t + k2 te−ζw0 t

Reales
e Iguales

ζ=1

Sobreamortiguada

xh (t) = k1 er1 t + k2 er2 t

Reales
y Distintas

ζ>1

Donde ki son las condiciones iniciales del problema y wd = w0

(a) Gráfico Respuesta Subamortiguada.

p
1 − ζ 2.

(b) Gráfico Resp. Crít. Amortiguada.

(c) Gráfico Respuesta Sobreamortiguada.

Figura 3. Gráficos sobre los distintos tipos de respuesta.

---

### Página 7

2.3

Circuitos RLC - Cómo Utilizarlo Correctamente

Los llamados circuitos RLC contienen resistores, capacitores e inductores. Una guía para
resolver este tipo de ejercicios se presenta a continuación:
1. En general, resulta más fácil utilizar el método de mallas, aunque el circuito puede ser
resuelto mediante cualquier método:
X
Vk = 0
malla

Al llegar al inductor y/o capacitor se deberá sumar o restar su voltaje, dependiendo
si la corriente ingresa por el terminal positivo o negativo asignado previamente.

2. Automáticamente, los voltajes provenientes de resistores deberán ser reemplazados mediante la Ley de Ohm.
3. Luego, deberán expresar la diferencia de potencial en el inductor y/o la intensidad que
circula por el capacitor en función de la(s) intensidad(es) de la(s) malla(s), de forma de
armar la EDO respectiva:
dQ(t)
dVC (t)
IC (t) =
=C
dΦL (t)
dIL (t)
=L
4. Para obtener la EDO de segundo orden, es posible que sea necesario aplicar una derivada
temporal a ambos lados de la ecuación, notando aquellos componentes constantes.
5. Por último, les debería quedar una ecuación de la siguiente forma:
dx(t)
d2 x(t)
+ 2ζw0
+ w02 x(t) = g(t)

(7)

6. Para determinar el tipo de respuesta homogénea, se deberá identificar y calcular el coeficiente de amortiguación ζ y la frecuencia natural w0 . Una vez realizado, simplemente
se utiliza la expresión predeterminada respectiva a la respuesta.
7. En caso de que exista una solución particular, se deberá proponer una solución de acuerdo
a la forma que presenta g(t) (polinomial, trigonométrica, exponencial, entre otros) e
insertarla en la EDO de segundo orden, de forma de determinar las constantes asociadas.
8. Finalmente, será posible determinar las constantes ki de la solución imponiendo las condiciones iniciales del sistema.

---

### Página 8

2.3.1

“Análisis de Circuitos Eléctricos”, 7.1, Berríos F. & Sáez C.

Para el siguiente circuito RLC, asuma que la fuente de voltaje entrega un voltaje V
constante para todo t ≥ 0.
a) Encuentre la ecuación diferencial que modela a la corriente a través del inductor
para t ≥ 0.
Ahora, considere que IL (0) = 3 A, IL′ (0) = 0 A, C = 10 nF y L = 10 mH.
Determine la corriente que circula a través del inductor para t ≥ 0 y las condiciones
que se deben cumplir para que:
b) Sea una respuesta sobreamortiguada.
c) Sea una respuesta críticamente amortiguada.
d) Sea una respuesta subamortiguada.
Por último, suponga que la fuente de voltaje ahora entrega un voltaje V (t) = αt
para todo t ≥ 0.
e) Encuentre la ecuación diferencial y solución que modela a la corriente a través del
inductor para t ≥ 0.

Figura 4. Esquema Circuito RLC.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la ecuación diferencial que modela a la corriente a través del inductor para
t ≥ 0. Luego, se deberá resolver el circuito mediante algún método, de forma de armar la EDO
respectiva:
d2 x(t)
dx(t)
+ 2ζw0
+ w02 x(t) = g(t)

---

### Página 9

Solución b)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la corriente que circula a través del inductor para t ≥ 0 y las condiciones
que se deben cumplir para lograr cada tipo de respuesta:
Tipo Respuesta

Expresión Respuesta

Raíces

Valor ζ

Subamortiguada

xh (t) = e−ζw0 t (k1 cos (wd t) + k2 sin (wd t))

Complejas
Conjugadas

ζ<1

Críticamente
Amortiguada

xh (t) = k1 e−ζw0 t + k2 te−ζw0 t

Reales
e Iguales

ζ=1

Sobreamortiguada

xh (t) = k1 er1 t + k2 er2 t

Reales
y Distintas

ζ>1

Además, se debe identificar el coeficiente de amortiguación ζ
y aplicar las condiciones iniciales respectivas.

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Ayudantía 27
18 de Noviembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Circuitos RL

1.1

Circuitos RL - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Aplicar las Leyes de Kirchoff para corrientes (KCL) y voltajes (KVL) en diversos circuitos
□
RL.
✓ Resolver EDOs de carácter separable en el contexto de circuitos RL.
□
✓ Determinar y aplicar las condiciones iniciales necesarias para la EDO según el contexto.
□
✓ Determinar el voltaje en un inductor según el contexto en diversos circuitos RL.
□
✓ Determinar la intensidad de corriente que circula por un inductor según el contexto en
□
diversos circuitos RL.
✓ Calcular el flujo magnético y energía almacenada en un inductor en el contexto de cir□
cuitos RL.
✓ Interpretar y determinar la constante de tiempo inductiva en diversos circuitos RL.
□
□ Identificar inductores conectados en serie y paralelo en diversas configuraciones.
□ Determinar la inductancia equivalente de una configuración mediante el método de conexiones.

✓ Utilizar límites matemáticos y técnicas relacionadas, tales como la regla de L’hopital.
□
✓ Utilizar derivadas y técnicas relacionadas, tales como la regla del producto y cuociente.
□

---

### Página 2

1.2

Circuitos RL - Inductores

Un inductor (o bobina) es un componente circuital pasivo de dos terminales que almacena
energía en forma de campo magnético, oponiéndose así a cambios bruscos en el valor de la
corriente. Un conjunto de = N ” inductores puede conectarse de distintas formas:
Conexión
Serie

Inductancia Equivalente
Leq =

Paralelo

PN

Efectos Eléctricos

Li

Misma Corriente en cada Li

PN 1
i Li
Leq =

Mismo Voltaje en cada Li

i

(a) Inductores conectados en serie

(b) Inductores conectados en paralelo

Figura 1. Diagramas sobre las configuraciones de inductores.

1.3

Circuitos RL - Cómo Utilizarlo Correctamente

Los llamados circuitos RL contienen tanto inductores como resistores. Una guía para resolver
este tipo de ejercicios se presenta a continuación:
1. En general, resulta más fácil utilizar el método de mallas, aunque el circuito puede ser
resuelto mediante cualquier método:
X
Vk = 0
malla

Al llegar al inductor se deberá sumar o restar su voltaje, dependiendo si la
corriente ingresa por el terminal positivo o negativo asignado previamente.

2. Automáticamente, los voltajes provenientes de resistores deberán ser reemplazados mediante la Ley de Ohm.
3. Luego, deberán expresar la diferencia de potencial en el inductor en función de la(s)
intensidad(es) de la(s) malla(s), de forma de armar la EDO respectiva:
VL (t) =

dIL (t)
dΦL (t)
=L

(1)

---

### Página 3

Recordemos que la energía almacenada por el inductor cambia a medida que este se carga
o descarga. Además, la ecuación anterior proviene de la definición de voltaje y de flujo
magnético en el inductor = ΦL = LI”: al momento de reemplazar, solo la corriente se
verá afectado por el diferencial, puesto que la inductancia se considera como una constante.

4. En general, la EDO será de tipo separable y se recomienda resolverla para la corriente
del inductor, por lo que se dejará a un lado de la ecuación solo variables dependientes de
“IL ” y al otro solo variables dependientes del tiempo y/o constantes:
α(IL ) · dIL = β(t) · dt
Luego, quedará integrar a ambos lados y despejar = IL ”:

Z t

Z IL

β(t) · dt

α(IL ) · dIL =
t0

I0

Donde = α” y = β” son variables que dependen de = IL ” y = t”, respectivamente.
Por otra parte, = I0 ” es la condición inicial de corriente para el inductor y = t0 ”
el tiempo inicial o desde donde se considera la carga/descarga del mismo.

5. ¿Cómo determinar las condiciones iniciales del inductor? Se debe leer bien el enunciado:
a) En ocasiones se dirá explícitamente que el inductor se encontraba descargado (i.e
ϕL = 0), por lo que su intensidad de corriente también será nula.
b) En otros casos, se dirá implícitamente que el inductor se ha cargado completamente,
puesto que el circuito se ha estado alimentando = durante mucho tiempo” con una
entrada de voltaje. Al alcanzar su flujo magnético máximo, el inductor se comporta
como cortocircuito, puesto que ya no hay cambios en su corriente con respecto al
tiempo:
dΦL (t)
dIL (t)
VL (t) =
=L
=0
6. Por último, les debería quedar una solución de la siguiente forma:
IL (t) = IL (∞) + (I0 − IL (∞))e−t/τ

(2)

Donde = τ ” es la constante de tiempo, la cual indica qué tan lento o rápido se carga el inductor.
Por otra parte, = IL (∞)” se refiere a cómo se comporta la corriente del inductor en el infinito.
Para circuitos de primer orden, se cumple que:

τ=

L
RT h

(3)

Donde = RT h ” es la resistencia de Thèvenin.

7. Si es que piden determinar la diferencia de potencial en el inductor o el flujo magnético
de este a través del tiempo, se puede ingresar la solución obtenida en las expresiones
anteriores:
dΦL
dIL (t)
VL (t) =
=L
ΦL (t) = LI(t)
Si es que se requiere otra variable (i.e la intensidad/voltaje en alguna resistencia),
siempre se puede utilizar KCL, KVL, Ley de Ohm, entre otros. Si se requiere analizar
variables en el infinito, se debe utilizar la herramienta de límite matemático.

---

### Página 4

1.3.1

“Problemas Resueltos de Electromagnetismo”, 16.12, Rodrigo Chi

En el circuito de la figura se ha tenido conectada la batería por mucho tiempo con el
interruptor S abierto. Luego en t = 0, el interruptor se cierra. Considere que V0 = 120 V,
R1 = R2 = 30 Ω y L = 50 mH.
a) Calcule el flujo magnético almacenado por el inductor en t = 0.
b) Determine la intensidad de corriente que circula por el inductor para t > 0.
c) Determine la diferencia de potencial en el inductor para t > 0.
d) ¿Cuál es la constante de tiempo inductiva luego de que se cierra el interruptor?
e) Encuentre la nueva corriente que circula por el inductor, luego de que ha transcurrido mucho tiempo con el interruptor cerrado.
f) Grafique la intensidad de corriente que circula por el inductor para t > 0.

Figura 2. Esquema Circuito RL.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el flujo magnético almacenado en t = 0 . Si el circuito ha estado operando
en tales estados durante mucho tiempo, la fuente de voltaje V0 entregará una constante alimentación al inductor y, eventualmente, alcanzará su flujo magnético máximo. En este punto
su flujo magnético ya no puede variar, por lo que se comportará como cortocircuito:
dΦL
=0
Finalmente, se utiliza la fórmula que relaciona flujo almacenado con inductancia:
VL (t) =

ΦL = LI

---

### Página 5

Paso 1: Condiciones Iniciales - IL (0)
Es posible observar que se produce un cortocircuito y un circuito abierto por el interruptor en
la parte inferior y derecha del circuito, respectivamente. Así, la caída de potencial se vuelve
cero y la corriente eléctrica no puede circular por tal rama, por lo que el circuito queda como:

Figura 3. Esquema sobre las condiciones iniciales del circuito.
Luego, la corriente que circula por el inductor estará dado por:

V0
R1
Finalmente, se utiliza la fórmula que relaciona flujo almacenado con inductancia:
IL (0) =

ΦL (0) = LIL (0)
V0
=L
R1
Reemplazando valores se obtiene que:

ΦL (0) = 50 mH ·

120 V
30 Ω

= Wb

(4)

Solución b), c), d), e) y f )
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la corriente I(t) que circula por el circuito, para un t ≥ 0. Luego, se deberá
resolver el circuito mediante algún método, de forma de armar la EDO respectiva:
VL (t) =

dΦL
dIL (t)
=L

Además, se deben aplicar las condiciones iniciales en relación al inductor.

---

### Página 6

Paso 1: Preparación KVL
Para t ≥ 0, el circuito queda como:

Figura 4. Esquema KVL del circuito (interruptor cerrado).
Como se presenta una única malla, se preferirá realizar este ejercicio mediante ese método.
Los polos de las fuentes de voltaje están predefinidos por el tamaño de las placas.
Además, y como R1 está conectado en paralelo con R2 , es posible reducir el circuito como:

R = R1 //R2
Reemplazando valores se obtiene que:

R1 R2
R1 + R2
30 · 30
=
Ω
30 + 30
= 15 Ω

R=

(5)

Paso 2: Resolución KVL - IA
Para armar las ecuaciones de KVL debemos observar una malla y recorrerla en el sentido
otorgado. Al pasar por un elemento circuital, se sumará su voltaje si se entra de + a − (en
caso contrario se resta):
Malla

Ecuación KVL

A

−V0 + VR + VL = 0

Luego, los voltajes provenientes de resistores son reemplazados mediante Ley de Ohm:

---

### Página 7

Malla

Ecuación KVL

A

−V0 + IA R + VL = 0

Para obtener la EDO se aplicará la expresión VL = L dIdtL = L dIdtA :

dIL
=0

−V0 + IL R + L

(6)

Paso 3: Resolución EDO - IL (t)
La EDO se puede tratar mediante el método de separación de variables, por lo que se dejará a
un lado de la ecuación solo variables dependientes de = IL ” y al otro solo variables dependientes
del tiempo y/o constantes:
−V0 + IL R + L

dIL
=0
dIL
=
L
V0 − IL R

Integrando con condiciones iniciales generales:

Z t

=
t0 L

Z IL

dIL
IL (0) V0 − IL R

El interruptor cambia de posición en t = 0 (i.e t ∈ [0, ∞[).
V0
:
Asimismo, el condensador estará sometido a cierta diferencia de potencial inicial IL (0) = R

Z t

=
0 L

−t

R
=
L

Z IL
V0
R1

dIL
V0 − I L R

Z V0 −IL R
V R

V0 − R0

du
u

R
V0 − I L R
−t = ln (
)
L
V0 − VR0 R

Notar que se realizó un cambio de variable u = V0 − IL R → du = −R dIL .
Por último, despejamos IL aplicando exponencial:
R

e−t L =
IL (t) =

V0 − IL R
V0 − VR01R

R
V0
V0
V0
+(
− )e−t L
R
R1
R

(7)

Reemplazando valores se obtiene que:

120 V
120 V 120 V −t 15 Ω
+(
−
)e 50 mH
15 Ω
30 Ω
15 Ω
= 8 − 4e−300t A

IL (t) =

Como los componentes están en serie, se concluye que I(t) = IL (t).

(8)

---

### Página 8

Paso 4: Corriente Inductor Infinito - IL (∞)
Además, y si transcurre mucho tiempo luego de que el interruptor se cierra (i.e t → ∞), la
corriente que circula por el capacitor será:
IL (∞) = lim IL (t)
t→∞

= lim

V0

t→∞ R

=

+(

R
V0
V0
− )e−t L
R1
R

V0
R

Reemplazando valores se obtiene que:

120 V
15 Ω
=8A

IL (∞) =

(9)

Paso 5: Voltaje Inductor - VL (t)
Utilizando la expresión que relaciona la intensidad de corriente con el voltaje en el inductor:
dIL (t)
R
d V0
V0
V0
=L ( +(
− )e−t L )
dt R
R1
R
V0
V0 −t R
R
= L(
− )e L · −
R1
R
L
V0
V0 −t R
= −R(
− )e L
R1
R

VL (t) = L

Reemplazando valores se obtiene que:
R
V0
V0
− )e−t L
R1
R
120 V 120 V −t 15 Ω
= −15 Ω · (
−
)e 50 mH
30 Ω
15 Ω
= 60e−300t V

VL (t) = −R(

(10)

Paso 6: Constante de Tiempo Inductiva - τ
Observando y comparando lo obtenido, la constante de tiempo inductiva vendrá dada por:
−

t
tR
=−
τ
L
L
τ=
R

Reemplazando valores se obtiene que:

50 mH
15 Ω
=
s

τ=

(11)

---

### Página 9

Paso 7: Gráfico Corriente - I(t)
Finalmente, se requiere graficar la corriente I(t) en función del tiempo. Notando los límites
inferior y superior, además de la forma de la gráfica, se tiene que:

Figura 5. Gráfico de I(t).

---

### Página 10

Circuitos de Segundo Orden

2.1

Circuitos de Segundo Orden - Resultados de Aprendizaje

Al término de este módulo, se espera que el estudiante sea capaz de:

✓ Aplicar las Leyes de Kirchoff para corrientes (KCL) y voltajes (KVL) en diversos circuitos
□
RLC.
✓ Resolver EDOs de segundo orden homogéneas en el contexto de circuitos RLC.
□
□ Resolver EDOs de segundo orden no homogéneas en el contexto de circuitos RLC.

✓ Determinar y aplicar las condiciones iniciales necesarias para la EDO según el contexto.
□
✓ Determinar el voltaje e intensidad de corriente que circula por un componente circuital
□
según el contexto en diversos circuitos RLC.
✓ Identificar y determinar la frecuencia natural y el coeficiente de amortiguación en diversos
□
circuitos RLC.
✓ Identificar y conocer el tipo de respuesta para diversos circuitos RLC.
□
✓ Conocer el gráfico asociado a cada tipo de respuesta para diversos circuitos RLC.
□
✓ Utilizar límites matemáticos y técnicas relacionadas, tales como la regla de L’hopital.
□
✓ Utilizar derivadas y técnicas relacionadas, tales como la regla del producto y cuociente.
□
2.2

Circuitos de Segundo Orden - Generalidades

En circuitos de segundo orden, las corrientes y voltajes satisfacen una ecuación de la forma:
dx(t)
d2 x(t)
+ 2ζw0
+ w02 x(t) = g(t)

(12)

Donde = ζ” es el coeficiente de amortiguación y = w0 ” la frecuencia natural del sistema.

Luego, la solución de la ecuación será de la siguiente manera:
x(t) = xh (t) + xp (t)

(13)

Donde xh (t) y xp (t) son la solución homogénea y particular, respectivamente.
Reemplazando xh (t) = ert en la ecuación homogénea, se obtiene su polinomio característico:

r2 + 2ζw0 r + w02 = 0
De esta manera, las raíces del polinomio serán:

r1,2 = −ζw0 ± w0

p
ζ2 − 1

Dependiendo de sus valores, habrán tres tipos de soluciones:

(14)

---

### Página 11

Tipo Respuesta

Expresión Respuesta

Raíces

Valor ζ

Subamortiguada

xh (t) = e−ζw0 t (k1 cos (wd t) + k2 sin (wd t))

Complejas
Conjugadas

ζ<1

Críticamente
Amortiguada

xh (t) = k1 e−ζw0 t + k2 te−ζw0 t

Reales
e Iguales

ζ=1

Sobreamortiguada

xh (t) = k1 er1 t + k2 er2 t

Reales
y Distintas

ζ>1

Donde ki son las condiciones iniciales del problema y wd = w0

(a) Gráfico Respuesta Subamortiguada.

p
1 − ζ 2.

(b) Gráfico Resp. Crít. Amortiguada.

(c) Gráfico Respuesta Sobreamortiguada.

Figura 6. Gráficos sobre los distintos tipos de respuesta.

2.3

Circuitos RLC - Cómo Utilizarlo Correctamente

Los llamados circuitos RLC contienen resistores, capacitores e inductores. Una guía para
resolver este tipo de ejercicios se presenta a continuación:
1. En general, resulta más fácil utilizar el método de mallas, aunque el circuito puede ser
resuelto mediante cualquier método:
X
Vk = 0
malla

Al llegar al inductor y/o capacitor se deberá sumar o restar su voltaje, dependiendo
si la corriente ingresa por el terminal positivo o negativo asignado previamente.

2. Automáticamente, los voltajes provenientes de resistores deberán ser reemplazados mediante la Ley de Ohm.

---

### Página 12

3. Luego, deberán expresar la diferencia de potencial en el inductor y/o la intensidad que
circula por el capacitor en función de la(s) intensidad(es) de la(s) malla(s), de forma de
armar la EDO respectiva:
dQ(t)
dVC (t)
IC (t) =
=C
dΦL (t)
dIL (t)
VL (t) =
=L
4. Para obtener la EDO de segundo orden, es posible que sea necesario aplicar una derivada
temporal a ambos lados de la ecuación, notando aquellos componentes constantes.
5. Por último, les debería quedar una ecuación de la siguiente forma:
d2 x(t)
dx(t)
+ 2ζw0
+ w02 x(t) = g(t)

(15)

6. Para determinar el tipo de respuesta homogénea, se deberá identificar y calcular el coeficiente de amortiguación ζ y la frecuencia natural w0 . Una vez realizado, simplemente
se utiliza la expresión predeterminada respectiva a la respuesta.
7. En caso de que exista una solución particular, se deberá proponer una solución de acuerdo
a la forma que presenta g(t) (polinomial, trigonométrica, exponencial, entre otros) e
insertarla en la EDO de segundo orden, de forma de determinar las constantes asociadas.
8. Finalmente, será posible determinar las constantes ki de la solución imponiendo las condiciones iniciales del sistema.

---

### Página 13

2.3.1

“Análisis de Circuitos Eléctricos”, 7.1, Berríos F. & Sáez C.

Para el siguiente circuito RLC, asuma que la fuente de voltaje entrega un voltaje V
constante para todo t ≥ 0.
a) Encuentre la ecuación diferencial que modela a la corriente a través del inductor
para t ≥ 0.
Ahora, considere que IL (0) = 3 A, IL′ (0) = 0 A, C = 10 nF y L = 10 mH.
Determine la corriente que circula a través del inductor para t ≥ 0 y las condiciones
que se deben cumplir para que:
b) Sea una respuesta sobreamortiguada.
c) Sea una respuesta críticamente amortiguada.
d) Sea una respuesta subamortiguada.
Por último, suponga que la fuente de voltaje ahora entrega un voltaje V (t) = αt
para todo t ≥ 0.
e) Encuentre la ecuación diferencial y solución que modela a la corriente a través del
inductor para t ≥ 0.

Figura 7. Esquema Circuito RLC.

Solución a)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la ecuación diferencial que modela a la corriente a través del inductor para
t ≥ 0. Luego, se deberá resolver el circuito mediante algún método, de forma de armar la EDO
respectiva:
d2 x(t)
dx(t)
+ 2ζw0
+ w02 x(t) = g(t)

---

### Página 14

Paso 1: Preparación KVL
Para t ≥ 0, el circuito queda como:

Figura 8. Esquema Circuito RLC.
Como se presenta una única malla, se preferirá realizar este ejercicio mediante ese método.

Paso 2: Resolución KVL - IA
Para armar las ecuaciones de KVL debemos observar una malla y recorrerla en el sentido
otorgado. Al pasar por un elemento circuital, se sumará su voltaje si se entra de + a − (en
caso contrario se resta):
Malla

Ecuación KVL

A

−V + VR + VL + VC = 0

Luego, los voltajes provenientes de resistores son reemplazados mediante Ley de Ohm:

Malla

Ecuación KVL

A

−V + IA R + VL + VC = 0

Además, es posible utilizar la expresión VL = L dIdtL = L dIdtA :

−V + IA R + L

dIA
+ VC = 0

---

### Página 15

Aplicando una derivada temporal a ambos lados de la ecuación,
notando aquellos componentes constantes (i.e V ), se obtiene que:

−

dIA R
d2 IA dVC
dV
+
+L 2 +
=0
dIA
d2 IA dVC
R
+L 2 +
=0

C
Para obtener la EDO se utilizará la expresión IA = IC = C dV
dt :

dIA
d2 IA IA
+L 2 +
=0
C
IA
d2 IA R dIA
+
+
=0
L dt
LC

R

(16)

Solución b)
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar la corriente que circula a través del inductor para t ≥ 0 y las condiciones
que se deben cumplir para lograr cada tipo de respuesta:
Tipo Respuesta

Expresión Respuesta

Raíces

Valor ζ

Subamortiguada

xh (t) = e−ζw0 t (k1 cos (wd t) + k2 sin (wd t))

Complejas
Conjugadas

ζ<1

Críticamente
Amortiguada

xh (t) = k1 e−ζw0 t + k2 te−ζw0 t

Reales
e Iguales

ζ=1

Sobreamortiguada

xh (t) = k1 er1 t + k2 er2 t

Reales
y Distintas

ζ>1

Además, se debe identificar el coeficiente de amortiguación ζ
y aplicar las condiciones iniciales respectivas.

Paso 1: Coeficiente de Amortiguación - ζ
Observando y comparando lo obtenido, la frecuencia natural vendrá dada por:
w02 =

LC
r

w0 =

LC

Reemplazando valores se obtiene que:

r

10 mH · 10 nF
rad
= 100000
s

w0 =

(17)

---

### Página 16

Análogamente, el coeficiente de amortiguación vendrá dado por:
R
L
R 1
ζ=
L 2w0
r
R C
=
2 L

2ζw0 =

(18)

Paso 2: Respuesta Subamortiguada
Para lograr una respuesta subamortiguada se debe cumplir que:
ζ<1
R

r

C
<1
L
r
R<2

L
C

Reemplazando valores se obtiene que:

r

10 mH
10 nF
< 2000 Ω
En este caso, la respuesta se puede escribir como:
R<2

IA (t) = e−ζw0 t (k1 cos (wd t) + k2 sin (wd t))

(19)

Aplicando una derivada temporal a la expresión anterior se obtiene que:
′
IA
(t) = e−ζw0 t (k2 wd cos (wd t) − k1 wd sin (wd t)) − ζw0 e−ζw0 t (k1 cos (wd t) + k2 sin (wd t))

Imponiendo las condiciones iniciales respectivas:

Condición

Ecuación Condición

IA (0) = 3

k1 + k2 · 0 = 3

′ (0) = 0
IA

k2 wd − ζw0 k1 = 0

Finalmente, se resuelve el sistema de ecuaciones:
k1 = 3

(20)

k2 = 3ζ

(21)

---

### Página 17

Paso 3: Respuesta Críticamente Amortiguada
Para lograr una respuesta críticamente amortiguada se debe cumplir que:
ζ=1
R

r

C
=1
L
r
R=2

L
C

Reemplazando valores se obtiene que:

r

10 mH
10 nF
= 2000 Ω
En este caso, la respuesta se puede escribir como:
R=2

IA (t) = k1 e−ζw0 t + k2 te−ζw0 t

(22)

Aplicando una derivada temporal a la expresión anterior se obtiene que:
′
IA
(t) = −ζw0 k1 e−ζw0 t + k2 e−ζw0 t − ζw0 k2 te−ζw0 t

Imponiendo las condiciones iniciales respectivas:

Condición

Ecuación Condición

IA (0) = 3

k1 + k2 · 0 = 3

′ (0) = 0
IA

−ζw0 k1 + k2 − ζw0 k2 · 0 = 0

Finalmente, se resuelve el sistema de ecuaciones:
k1 = 3

(23)

k2 = 3ζw0

(24)

---

### Página 18

Paso 4: Respuesta Sobremortiguada
Para lograr una respuesta sobreamortiguada se debe cumplir que:
ζ>1
R

r

C
>1
L
r
R>2

L
C

Reemplazando valores se obtiene que:

r

10 mH
10 nF
> 2000 Ω
En este caso, la respuesta se puede escribir como:
√
√
IA (t) = k1 e(−ζw0 +w0 ζ −1)t + k2 e(−ζw0 −w0 ζ −1)t
R>2

(25)

Aplicando una derivada temporal a la expresión anterior se obtiene que:
′
IA
(t) = k1 (−ζw0 + w0

√
√
p
p
ζ 2 − 1)e(−ζw0 +w0 ζ −1)t + k2 (−ζw0 − w0 ζ 2 − 1)e(−ζw0 −w0 ζ −1)t
Imponiendo las condiciones iniciales respectivas:

Condición

Ecuación Condición

IA (0) = 3

k 1 + k2 = 3

′ (0) = 0
IA

k1 (−ζw0 + w0

p
p
ζ 2 − 1) + k2 (−ζw0 − w0 ζ 2 − 1) = 0

Finalmente, se resuelve el sistema de ecuaciones:
p
3(ζ + ζ 2 − 1)
p
k1 =
2 ζ2 − 1
p
3(ζ − ζ 2 − 1)
p
k2 = −
2 ζ2 − 1

(26)
(27)
