---
title: "Ayudantia 18"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_18.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_18_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 18

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 18
Circuito RC

#### Problema 1
Considere el siguiente circuito RC.

(a) Calcule la capacitancia equivalente del circuito y la constante de tiempo del circuito RC
resultante. ¿Qué pasa si C2 Ñ 8?
(b) Suponga que en t = 0 se conecta la batería con potencial VS con las 3 capacitancias totalmente descargadas. Calcule la corriente que fluye en la resistencia R en un instante de tiempo
t > 0.
(c) ¿Cuál es la carga total máxima almacenada por las capacitancias? ¿Cuál es la corriente máxima que fluye por la resistencia R?
#### Problema 2
En el circuito de la figura, los condensadores se encuentran completamente descargados.

---

### Página 2

Si el interruptor se cambia a la posición 1 en t = 0 s, determinar:
(a) La corriente I0 que suministra la fuente en el instante justo después de cerrar el interruptor.
(b) La carga máxima almacenada en el condensador C1 .
(c) La carga almacenada en el capacitor C1 en función del tiempo.
Si luego de mucho tiempo, el interruptor se cambia otra vez a la posición 2, determinar:
(d) La carga almacenada en C1 como función del tiempo.
#### Problema 3
Inicialmente el condensador de capacidad C1 tiene carga Q0 , y el segundo condensador está descargado. Encuentre la pérdida de energía al conectar ambos condensadores mediante un conductor
de resistencia R, como muestra la figura.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 18
Circuito RC

#### Problema 1
Considere el siguiente circuito RC.

(a) Calcule la capacitancia equivalente del circuito y la constante de tiempo del circuito RC
resultante. ¿Qué pasa si C2 Ñ 8?
(b) Suponga que en t = 0 se conecta la batería con potencial VS con las 3 capacitancias totalmente descargadas. Calcule la corriente que fluye en la resistencia R en un instante de tiempo
t > 0.
(c) ¿Cuál es la carga total máxima almacenada por las capacitancias? ¿Cuál es la corriente máxima que fluye por la resistencia R?

#### Solución
Para la primera parte solo tenemos que hacer uso de las ecuaciones para condensadores equivalentes, primero podemos juntar C1 y C2 de la siguiente forma,

---

### Página 2

´1
C12
“

`
C1 C2

Ñ

C12 “

C1 C2
C1 ` C 2

Ahora podemos juntar C12 con C13 como una sola resistencia de la forma,
Ceq = C3 ` C12 = C3 `

C1 C2
C1 ` C 2

Esto quiere decir que el sistema es equivalente a una resistencia R conectada en serie a un condensador Ceq , por definición la constante de tiempo se calcula como,
τ = RC = RpC3 `

C1 C2
q
C1 ` C 2

En el momento de hacer C2 Ñ 8, el denominador se puede aproximar a C1 ` C2 « C2 , quedando
la capacitancia equivalente como,
lím Ceq = C1 ` C3

C2 Ñ8

Es decir, como si el condensador C2 no estuviera.
Sabemos que la ecuación para la intensidad de corriente de un circuito RC tiene la siguiente forma,
I(t) = I0 e´τ {t
Donde I0 corresponde a la corriente incial, en este momento la capacitancia equivalente paraciera
que no está en el circuito, esto quiere decir que toda la diferencia de potencial del sistema viene
dado por la diferencia de potencial en la resistencia,
I(t) = 

Vs ´τ {t
e
R

Si conocemos la intensidad de corriente, conocemos la carga almacenada para cualquier momento
t, esto nos dará,
żt
Ipxqdx = Qmax p1 - e´τ {t q

Qp tq “

Donde Qmax = Vs ˚ Ceq . Esta es la carga máxima que puede almacenar todo el sistema de 3 condensadores.

---

### Página 3

#### Problema 2
En el circuito de la figura, los condensadores se encuentran completamente descargados.

Si el interruptor se cambia a la posición 1 en t = 0 s, determinar:
(a) La corriente I0 que suministra la fuente en el instante justo después de cerrar el interruptor.
(b) La carga máxima almacenada en el condensador C1 .
(c) La carga almacenada en el capacitor C1 en función del tiempo.
Si luego de mucho tiempo, el interruptor se cambia otra vez a la posición 2, determinar:
(d) La carga almacenada en C1 como función del tiempo.

#### Solución
Para el primer inciso, la segunda malla (derecha) es totalmente irrelevante, justo en el momento
en que se cierra este circuito, el condensador no es considerado ya que parte descargado, la ley de
malla dice entonces,
E - I0 R1 - I0 R3 = 0 Ñ Io = 

E
R1 ` R3

en el momento que la carga es máxima, ya no circula corriente, por lo que la caída de potencial en
las resistencias es 0, quedando la ley de malla como,
E´

Q1,max
“ 0 Ñ Q1,max = EC1

Ahora buscamos la ecuación de carga para cualquier tiempo t para el condensador C1 , para esto
escribimos la ley de mallas como,
E ´ I ¨ R1 ´

Q1
´ I ¨ R3 = 0

---

### Página 4

donde I = dQ1 {dt, reemplazándolo en la ecuación llegamos a la EDO que debemos resolver,
E´

Q1
dQ1
¨ pR1 ` R3 q ´
“0
dt

Utilizando separación de variables (O si recuerdan directamente cuál es la solución a esta ecuación),
la solución obtenida es,
Q1 (t) = EC1 p1 - e´t{τ q

;

τ = C1 pR1 ` R3 q

(1)

Para el último inciso, luego de pasar mucho tiempo la carga del condensador C1 será EC1 , como
ya calculamos antes. Al cerrar el segundo circuito, la ecuación de mallas obtenidas es,
Q2
Q11
´ IR1 ´ IR2 ´
“0
C2
donde Q11 es la carga del condensador 1 en función del tiem(o, con Q1 p0) = EC1 . Como la carga
inicial es la anterior mencionada, para todo momento, por conservación de la carga, debe cumplirse
que,
dQ1
dQ2
“
dt
dt
Reemplazando en la ecuación y operando un poco, llegaremos eventualmente a la siguiente expresión,
Q11 ` Q2 = EC1 Ñ I = ´

Q11 `

EC1
dQ11
Req Ceq ´
Ceq = 0
dt
C2

La solución general de este problema tiene la siguiente forma,
Q11 (t) = Ae´t{τ ` B

(2)

Con A y B constantes a determinar. Lo primero que sabemos es la condición para t = 0,
Q1 (0) = EC1
Reemplazando nuestra idea de solución en la ecuación, llegaremos a que se debe cumplir que,
τ = Req Ceq
B = E

C12
C1 ` C 2

Solo nos quedaría por determinar A, utilizando lo conocido para Q11 p0q, llegaremos a,
A = ECeq

(3)

---

### Página 5

Siendo nuestra solución final,
Q11 (t) = ECeq e´t{τ ` E

Ceq
C2

#### Problema 3
Inicialmente el condensador de capacidad C1 tiene carga Q0 , y el segundo condensador está descargado. Encuentre la pérdida de energía al conectar ambos condensadores mediante un conductor
de resistencia R, como muestra la figura.

#### Solución
Si queremos obtener la energía disipada, nos conviene calcular la potencia, que se relaciona con la
intensidad que pasa por la resistencia, es decir, queremos obtener la ecuación de la intensidad de
corriente para este circuito.
Para esto partimos con la ley de mallas, como,
´V1 ` IR ` V2 = 0
podemos reemplazar los voltajes,
´

Q1
Q2
` IR `
“0
C2

Conocemos una relación entre las dos cargas, toda la corriente que entra a C2 , tuvo que haber salido
de C1 ,

---

### Página 6

I(t) = 

dQ1
dQ2
“´
dt
dt

Como queremos obtener la ecuación para la intensidad, derivamos la expresión que habíamos obtenido para la corriente,
´

1 dQ2
1 dQ1 I(t)
`
R`
“0
C1 dt
dt
C2 dt

Utilizando el hecho de que las tasa de cambio de las cargas de C1 y C2 deben ser iguales pero con
signos distintos,
dI(t)
1 dQ2
I(t) `
R`
“0
dt
C2 dt
Solucionando la edo,
C `C

´ 1 p C1 C 2 qt

I(t) = K ˚ e R

1 2

La constante K podemos determinarla de la siguiente forma. Tomamos la ley de mallas definida
con las cargas, la primera ecuación obtenida, y utilizamos que la carga total debe conservarse
(Q1 = Q0 - Q2 ),
´

Q2 (t)
Q0 Q2 (t)
`
` IptqR `
“0
C2

Que podemos escribir como,
Q0
´
`

ˆ

C1 ` C 2
C1 C2

˙
Q2 (t) ` IptqR = 0

Nos faltaría conocer Q2 , para esto integramos I(t),
żt

KRC1 C2
Q2 (t) = dτ I(τ ) = 
C1 ` C 2

ˆ
1´e

´R

pC1 `C2 q
t
C1 C2

˙

Reemplazando esto directamente en la ecuación anterior, llegaremos a una expresión que nos permite obtener K fácilmente, el resultado da,
K“

Q0
RC1

Es decir, nuestra intensidad de corriente para el circuito es,
I(t) = 

2 qt
Q0 ´ R1 p CC1 `C
1 C2
e
RC1

---

### Página 7

Utilizando la ecuación para la potencia de una resistencia,
ˆ

P (t) = RI (t) = R

2 qt
Q0 ´ R1 p CC1 `C
1 C2
e
RC1

˙2

Y por definición la potencia es energía disipada por unidad de tiempo, entonces la energía disipada
luego de un tiempo infinito va a ser,
ż8
∆E “

dt

1 `C2 q t
Q20 C2
Q20 ´ 2pC
RC1 C2
e
“
RC12
2C1 pC1 ` C2 q
