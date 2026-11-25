---
title: "Ayudantia 29"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_29.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_29_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 29

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 28
Circuito RLC con Corriente Alterna II
#### Problema 1
Una antena FM tiene una inductancia L = 10´6 H, una capacidad C = 10´12 F, y una resistencia
R = 100 Ω. Una señal de radio induce una fem sinusoidal en la antena con amplitud 10´5 V.

(a) ¿A qué frecuencia angular ω0 de la señal incidente el circuito estará sintonizado, esto es, para
que ω0 la corriente en el circuito será máxima?
(b) Asumiendo que la onda incidente está sintonizada, ¿cuál será la amplitud de la corriente en
el circuito a esta frecuencia?
(c) ¿Cuál es la amplitud de la diferencia de potencial a través del condensador a esta frecuencia?
#### Problema 2
Considere el circuito de la figura, donde
V (t) = V0 cos(ωt).

---

### Página 2

Si S1 y S2 se cierran inicialmente, encuentre (los datos son R, L, V0 y ω):

(a) La corriente en función del tiempo.
(b) La potencia promedio entregada al circuito.
(c) La corriente en función del tiempo mucho después de que S1 se abre.
(d) La capacidad C si S1 y S2 se abren y después de un tiempo largo, la corriente y el voltaje
están en fase.
(e) La impedancia cuando S1 y S2 se abren.
(f) La energía máxima almacenada en el condensador y la inductancia.
(g) La diferencia de fase entre voltaje y corriente si se dobla la frecuencia ω.
(h) La frecuencia para la cual la reactancia inductiva es igual a un medio de la reactancia capacitiva.
#### Problema 3
Dado el circuito RLC en la figura:

---

### Página 3

(a) ¿Cuál es la impedancia entre los terminales de conexión?
(b) Se aplica el voltaje alterno U (t) = U0 cos(ωt) a los terminales de conexión. Calcule la amplitud de oscilación de la corriente alterna I(t) que entra al circuito.
(c) ¿Cuál es la potencia que se disipa en el circuito durante un período de oscilación del voltaje
alterno cuando la frecuencia angular del voltaje es ω = 1{(LC)?
#### Problema 4
Un circuito contiene dos resistencias R, dos inductancias L y una capacitancia C. Estos elementos
están conectados a una fuente de voltaje alterna V (t) = V0 cos(ωt), como se observa en la figura.
Se pide:

(a) La impedancia vista desde la fuente de voltaje.
(b) El fasor de corriente del circuito y el fasor de voltaje V̂L .
(c) Determine la frecuencia ω0 que debe tener la fuente de voltaje, de modo que la amplitud
de la corriente que sale de la fuente sea máxima. Además, calcule cuál será dicha amplitud
máxima.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 29
Circuito RLC con Corriente Alterna II

#### Problema 1
Una antena FM tiene una inductancia L = 10´6 H, una capacidad C = 10´12 F, y una resistencia
R = 100 Ω. Una señal de radio induce una fem sinusoidal en la antena con amplitud 10´5 V.

(a) ¿A qué frecuencia angular ω0 de la señal incidente el circuito estará sintonizado, esto es, para
que ω0 la corriente en el circuito será máxima?
(b) Asumiendo que la onda incidente está sintonizada, ¿cuál será la amplitud de la corriente en
el circuito a esta frecuencia?
(c) ¿Cuál es la amplitud de la diferencia de potencial a través del condensador a esta frecuencia?

#### Solución
El circuito corresponde a un circuito RLC en serie. La impedancia total del circuito es

---

### Página 2

Z = R ` iωL `

iωC

Usando que 1{i = -i, se puede escribir como
ˆ

Z = R ` i ωL ´
ωC

˙

Por lo tanto, el módulo de la impedancia es
d
ˆ
|Z| “

R2 `

ωL ´
ωC

˙2

La amplitud de la corriente inducida en el circuito está dada por
I0 “

E0
,
|Z|

donde E0 es la amplitud de la fem inducida.
(a) La corriente será máxima cuando la impedancia sea mínima. Como R es constante, esto
ocurre cuando la parte reactiva se anula:
ωL ´

“ 0.
ωC

Entonces,
ωL “

ωC

Multiplicando por ωC, se obtiene
ω 2 LC = 1.
Por lo tanto, la frecuencia angular de resonancia es
ω0 “ ?
LC
(b) En resonancia, la parte inductiva y capacitiva de la impedancia se cancelan, por lo que
Z(ω0 ) = R.
Así, la amplitud de la corriente es
I0 “

E0

---

### Página 3

(c) La amplitud de la diferencia de potencial en el condensador es
VC,0 = I0 XC ,
donde la reactancia capacitiva es
XC “

ωC

Evaluando en resonancia,
ω0 C

VC,0 = I0
Como

ω0 “ ?
,
LC
entonces
1?
“
LC “
ω0 C
C

c

L
C

c
VC,0 = I0

L
C

Usando I0 = E0 {R, también se puede escribir como
E0
VC,0 “

c

L
C

Ahora reemplazamos los valores numéricos:
L = 10´6 H,

C = 10´12 F,

R = 100 Ω,

Para la frecuencia angular de resonancia,
ω0 “ ?
“a
´6
LC
p10 qp10´12 q
Entonces,
“ -9 = 109 rad{s.
ω0 “ ?
10´18

E0 = 10´5 V.

---

### Página 4

Para la amplitud de la corriente,
I0 “

10´5
E0
“
“ 10´7 A.

Finalmente, para la amplitud del voltaje en el condensador,
VC,0 = I0

ω0 C

Reemplazando,
VC,0 = p10´7 q

p109 qp10´12 q

Como
p109 qp10´12 q = 10´3 ,
se obtiene
VC,0 = p10´7 q(103 ) = 10´4 V.
ω0 = 109 rad{s
I0 = 10´7 A
VC,0 = 10´4 V
#### Problema 2
Considere el circuito de la figura, donde
V (t) = V0 cos(ωt).
Si S1 y S2 se cierran inicialmente, encuentre (los datos son R, L, V0 y ω):

---

### Página 5

(a) La corriente en función del tiempo.
(b) La potencia promedio entregada al circuito.
(c) La corriente en función del tiempo mucho después de que S1 se abre.
(d) La capacidad C si S1 y S2 se abren y después de un tiempo largo, la corriente y el voltaje
están en fase.
(e) La impedancia cuando S1 y S2 se abren.
(f) La energía máxima almacenada en el condensador y la inductancia.
(g) La diferencia de fase entre voltaje y corriente si se dobla la frecuencia ω.
(h) La frecuencia para la cual la reactancia inductiva es igual a un medio de la reactancia capacitiva.

#### Solución
La fuente del circuito es
V (t) = V0 cos(ωt).
Como inicialmente S1 y S2 están cerrados, la inductancia queda cortocircuitada por S1 y el condensador queda cortocircuitado por S2 . Por lo tanto, inicialmente el circuito se reduce solo a la
resistencia R.
(a) Corriente en función del tiempo.
Con S1 y S2 cerrados, el circuito es puramente resistivo. Entonces,
I(t) = 

V (t)

---

### Página 6

I(t) = 

V0
cospωtq .

(b) Potencia promedio entregada al circuito.
La potencia instantánea es
P (t) = V ptqI(t).
Como

V0
cospωtq,

V (t) = V0 cos(ωt),

I(t) = 

P (t) = 

V02
cos2 pωtq.

se tiene

Usando que
xcos2 pωtqy “ ,
resulta
Pprom “

V02
2R

(c) Corriente mucho tiempo después de que S1 se abre.
Al abrir S1 , la inductancia deja de estar cortocircuitada. Si S2 permanece cerrado, el condensador sigue cortocircuitado. Por lo tanto, el circuito queda como un circuito RL en serie.
La impedancia del circuito es
ZRL = R ` iωL.
Su módulo es
|ZRL | “

a
R2 ` pωLq2 .

La amplitud de la corriente es
V0
I0 = a
R ` pωLq2
La diferencia de fase satisface
tan ϕ “

ωL
ˆ

ϕ = arctan

ωL

˙

En un circuito inductivo, la corriente se atrasa respecto del voltaje. Así,
V0
I(t) = a
cospωt ´ ϕq
R ` pωLq2

---

### Página 7

donde
ˆ
ϕ = arctan

ωL

˙

(d) Capacidad C para que, con S1 y S2 abiertos, la corriente y el voltaje estén en fase.
Si S1 y S2 están abiertos, el circuito es un circuito RLC en serie.
La impedancia es
ˆ

Z = R ` i ωL ´
ωC

˙

Para que la corriente y el voltaje estén en fase, la parte imaginaria de la impedancia debe ser
cero. Es decir,
ωL ´
“ 0.
ωC
Entonces,
ωL “

ωC

Despejando C,
C“

ω2L

(e) Impedancia cuando S1 y S2 se abren.
Con ambos interruptores abiertos, el circuito es RLC en serie. Por lo tanto,
ˆ

Z = R ` i ωL ´
ωC

˙

El módulo de la impedancia es
d
ˆ

|Z| “

R2 ` ωL ´
ωC

Si se usa el valor de C encontrado en la parte anterior,
C“

,
ω2L

entonces el circuito está en resonancia y
ωL “

ωC

Por lo tanto,|
Z = R.

˙2

---

### Página 8

(f) Energía máxima almacenada en el condensador y en la inductancia.
En el circuito RLC en serie, la amplitud de la corriente es
I0 “

V0
|Z|

La energía almacenada en la inductancia es
UL = LI 2 .
Por lo tanto, su valor máximo es
UL,máx = LI02 .
Como
I0 “

V0
,
|Z|

también podemos escribir
UL,máx = L
Para el condensador,

ˆ

V0
|Z|

˙2

UC = CVC2 .

La amplitud del voltaje en el condensador es
VC,0 = I0 XC = I0

ωC

Entonces,
UC,máx = C

ˆ

I0
ωC

˙2

UC,máx “

I02
2ω 2 C

Si el circuito está en resonancia, usando
C“

,
ω2L

se obtiene
I0 “

|Z| = R,
V0

---

### Página 9

Así,
V0

˙2

V0

˙2

UL,máx = L

ˆ

UC,máx = L

ˆ

y

Por lo tanto, en resonancia,
UL,máx = UC,máx .
(g) Diferencia de fase entre voltaje y corriente si se dobla la frecuencia.
Ahora la frecuencia angular es
Ω = 2ω.
La impedancia del circuito RLC es
ˆ

Z = R ` i ΩL ´
ΩC

˙

La diferencia de fase entre voltaje y corriente satisface
ΩL ´ ΩC

tan ϕ “

ˆ
ϕ = arctan

ΩL ´ ΩC

˙

Como Ω = 2ω,
ˆ
ϕ = arctan
Si usamos
C“
entonces

2ωL ´ 2ωC

˙

,
ω2L

ωL
“
2ωC

Luego,
2ωL ´

ωL
“ 2ωL ´
“ ωL.
2ωC

ˆ
ϕ = arctan

3ωL
2R

˙

Como la reactancia neta es positiva, el circuito es inductivo. Por lo tanto, la corriente se atrasa
respecto del voltaje.

---

### Página 10

(h) Frecuencia para la cual la reactancia inductiva es igual a la mitad de la reactancia
capacitiva.
La reactancia inductiva es
XL = ΩL,
mientras que la reactancia capacitiva es
XC “

ΩC

Se pide que
X L = XC .
Entonces,
ΩL “

1 1
2 ΩC

Multiplicando por ΩC,
Ω2 LC “ .
Ω2 “

2LC

Así,
Ω“ ?
2LC
Si se usa el valor resonante
C“
entonces
Ω = b

,
ω2L

` ˘.
2L ω21L

Luego,
ω
Ω“ ? .
#### Problema 3
Dado el circuito RLC en la figura:

---

### Página 11

(a) ¿Cuál es la impedancia entre los terminales de conexión?
(b) Se aplica el voltaje alterno U (t) = U0 cos(ωt) a los terminales de conexión. Calcule la amplitud de oscilación de la corriente alterna I(t) que entra al circuito.
(c) ¿Cuál es la potencia que se disipa en el circuito durante un período de oscilación del voltaje
alterno cuando la frecuencia angular del voltaje es ω 2 = 1{(LC)?

#### Solución
El circuito visto desde los terminales de conexión tiene dos ramas en paralelo. La primera rama
contiene solamente una resistencia R. La segunda rama contiene una resistencia R, una inductancia
L y una capacitancia C, todos en serie.
Trabajaremos en notación fasorial. Si el voltaje aplicado es
U (t) = U0 cos(ωt),
entonces su fasor asociado es
Û = U0 eiωt .
La impedancia de la rama central es simplemente
Z1 = R.
La impedancia de la rama derecha es
Z2 = R ` iωL `

iωC

Como
i
“´
,
iωC
ωC

---

### Página 12

tenemos
ˆ

Z2 = R ` i ωL ´
ωC

˙

Definimos
X(ω) = ωL ´

ωC

Entonces,
Z2 = R ` iX.
(a) Como ambas ramas están en paralelo, la impedancia equivalente cumple
“
` .
Zeq
Z1 Z2
“ `
Zeq
R R ` iX
Sumando,
R ` iX ` R
“
Zeq
RpR ` iXq
Luego,
2R ` iX
“
Zeq
RpR ` iXq
Zeq “

RpR ` iXq
2R ` iX

Reemplazando Xpωq, queda
“
`
˘‰
R R ` i ωL ´ ωC
`
˘ .
Zeq “
2R ` i ωL ´ ωC

---

### Página 13

(b) El fasor de corriente total que entra al circuito es
Û
Iˆ “
Zeq
Usando la expresión de la admitancia,
ˆ
Iˆ “ Û

`
R R ` iX

˙
e´iϕZ .

Como Û = U0 eiωt , tenemos
2R ` iX ipωt´ϕZ q
Iˆ = U0
e
RpR ` iXq
Para encontrar la amplitud de la corriente, calculamos el módulo:
ˆ
I0 “ |I|.
Entonces,
ˇ
ˇ
ˇ 2R ` iX ˇ
ˇ
ˇ.
I0 = U0 ˇ
RpR ` iXq ˇ
Como
|2R ` iX| “

?
4R2 ` X 2 ,

|R ` iX| “

?
R2 ` X 2 ,

y

se obtiene
U0
I0 “

c

4R2 ` X 2
R2 ` X 2

Reemplazando Xpωq,
g
`
˘
f
1 2
4R2 ` ωL ´ ωC
U0 f
e
I0 “
`
˘ .
1 2
R2 ` ωL ´ ωC

---

### Página 14

(c) Ahora se pide la potencia disipada durante un período cuando
ω2 “

LC

Esta es la condición de resonancia, porque
ω0 “ ?
LC
En resonancia,
ω0 L “

ω0 C

X(ω0 ) = ω0 L ´

“ 0.
ω0 C

Entonces, la rama derecha queda con impedancia
Z2 (ω0 ) = R.
La rama central también tiene impedancia
Z1 = R.
Por lo tanto, en resonancia el circuito equivale a dos resistencias R en paralelo:
Zeq (ω0 ) = R ∥ R.
Luego,
Zeq pω0 q “

La amplitud de la corriente total es
I0 pω0 q “

U0
R{2

I0 pω0 q “

2U0

Entonces,

---

### Página 15

U (t) = U0 cos(ω0 t),
e
2U0
cospω0 tq.

I(t) = 

La potencia instantánea entregada al circuito es
P (t) = U ptqI(t).
Reemplazando,
P (t) = U0 cos(ω0 t)

2U0
cospω0 tq.

Entonces,
2U02
cos2 pω0 tq.

P (t) = 

La potencia media disipada durante un período T es
xP y “
T

żT
P (t) dt.

xP y “
T

żT

2U02
cos2 pω0 tq dt.

Sacando las constantes fuera de la integral,
2U02 1
xP y “
R T

żT
cos2 pω0 tq dt.

Usamos la identidad trigonométrica
cos2 pω0 tq “
Entonces,

1 ` cosp2ω0 tq

---

### Página 16

żT

żT

cos pω0 tq dt “

1 ` cosp2ω0 tq
dt.

Separando,
żT

cos pω0 tq dt “

żT

dt `

żT
cosp2ω0 tq dt.

La primera integral es

żT
dt “

T

La segunda integral es

„
ȷT
1 sinp2ω0 tq
cosp2ω0 tq dt “
2ω0

żT

Como T = 2π{ω0 , se tiene
sin(2ω0 T ) = sin(4π) = 0.
Además,
sin(0) = 0.
żT
cos2 pω0 tq dt “

T

Luego,
T

żT

cos2 pω0 tq dt “ .

Finalmente,
xP y “

2U02 1
R 2

xP y “

U02

---

### Página 17

#### Problema 4
Un circuito contiene dos resistencias R, dos inductancias L y una capacitancia C. Estos elementos
están conectados a una fuente de voltaje alterna V (t) = V0 cos(ωt), como se observa en la figura.
Se pide:

(a) La impedancia vista desde la fuente de voltaje.
(b) El fasor de corriente del circuito y el fasor de voltaje V̂L .
(c) Determine la frecuencia ω0 que debe tener la fuente de voltaje, de modo que la amplitud
de la corriente que sale de la fuente sea máxima. Además, calcule cuál será dicha amplitud
máxima.

#### Solución
El circuito está formado por dos resistencias R, dos inductancias L y una capacitancia C, todos
conectados en serie con la fuente de voltaje alterna
V (t) = V0 cos(ωt).
Trabajaremos usando fasores. Tomamos como referencia el voltaje de la fuente, de modo que
V̂ = V0 eiωt .
La impedancia de una resistencia es
ZR = R,
la impedancia de una inductancia es
ZL = iωL,
y la impedancia de un condensador es

---

### Página 18

i
“´
iωC
ωC

ZC “

Como el circuito tiene dos resistencias, dos inductancias y un condensador en serie, la impedancia
total vista desde la fuente es
Zeq = R ` R ` iωL ` iωL `

iωC

Zeq = 2R ` i2ωL ´

i
ωC

Agrupando la parte imaginaria,
ˆ

Zeq = 2R ` i 2ωL ´
ωC

˙

Definimos
X(ω) = 2ωL ´

ωC

Así, la impedancia equivalente queda
Zeq = 2R ` iX
es decir,
ˆ

Zeq = 2R ` i 2ωL ´
ωC

˙

(a) La impedancia vista desde la fuente de voltaje es
ˆ

Zeq = 2R ` i 2ωL ´
ωC

˙

Su módulo es
d
ˆ

|Zeq | “

p2Rq2 ` 2ωL ´
ωC

˙2

---

### Página 19

d
ˆ

|Zeq | “

4R2 ` 2ωL ´
ωC

˙2

Luego,
ˆ
´1

ϕZ = tan

2ωL ´ ωC
2R

˙

Entonces, en forma polar,
Zeq “ |Zeq |eiϕZ .
(b) El fasor de corriente se obtiene mediante la ley de Ohm en forma fasorial:
V̂
Iˆ “
Zeq
Como V̂ = V0 eiωt , se tiene
V0
ipωt´ϕZ q
Iˆ = b
`
˘2 e
4R ` 2ωL ´ ωC
Ahora calculemos el fasor de voltaje en la inductancia indicada en la figura. Como el voltaje
de una inductancia satisface
ˆ
V̂L = ZL I,
y
ZL = iωL,
se obtiene
ˆ
V̂L = iωLI.

V̂L = iωL b

V0
eipωt´ϕZ q .
`
˘
4R2 ` 2ωL ´ ωC

---

### Página 20

Además, i = eiπ{2 . La fase del voltaje en la inductancia tiene una constante extra de π{2,
quedando como resultado final,

V̂L = ωL b

V0
ipωt´ϕZ `π{2q
˘2 e
`
4R2 ` 2ωL ´ ωC

(c) La amplitud de la corriente que sale de la fuente es
V0
I0 (ω) = b
˘
`
1 2
4R2 ` 2ωL ´ ωC
Para que esta amplitud sea máxima, el denominador debe ser mínimo. Como 4R2 es constante, basta exigir que la parte reactiva se anule:
2ωL ´

“ 0.
ωC

Entonces,
2ωL “

ωC

Multiplicando por ωC, obtenemos
2ω 2 LC = 1.
ω02 “

2LC

Así, la frecuencia angular que maximiza la corriente es
ω0 “ ?
2LC
En esta frecuencia, la impedancia equivalente queda puramente resistiva:
Zeq (ω0 ) = 2R.
Por lo tanto, la amplitud máxima de la corriente es

I0,max “

V0
2R
