---
title: "Ayudantia 28"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_28.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_28_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 28

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 28
Circuito RLC con Corriente Alterna

#### Problema 1
El circuito de la figura se denomina filtro RC pasa-altos porque transmite con mayor amplitud las
señales de alta frecuencia que las de baja. Si la tensión de entrada es Vin = V0 cos ωt, demostrar que
la de salida es
Vout = VR cospωt - ϕq,
donde
V0
VR = b
` 1 ˘2
1 ` ωRC
y estudie los casos en que ω ! RC
, ω = RC
y ω " RC
.

#### Problema 2
Considere el circuito de la figura con una fuente de voltaje V (t) = V0 cos(ωt), una resistencia R,
una inductancia L y dos condensadores C1 y C2 con C1 = C y C2 = 2C:

---

### Página 2

a) Encuentre la ecuación diferencial (de segundo grado) que debe satisfacer las corrientes del
circuito.
b) Determine la impedancia equivalente del sistema.
c) Encuentre la expresión para la corriente alterna en función del tiempo. Además, determine el
valor de C, en términos de ω y L, que maximiza la amplitud de la corriente.
#### Problema 3
Considere el circuito de la figura, donde
V (t) = V0 cos(ωt).
Si S1 y S2 se cierran inicialmente, encuentre (los datos son R, L, V0 y ω):

(a) La corriente en función del tiempo.
(b) La potencia promedio entregada al circuito.

---

### Página 3

(c) La corriente en función del tiempo mucho después de que S1 se abre.
(d) La capacidad C si S1 y S2 se abren y después de un tiempo largo, la corriente y el voltaje
están en fase.
(e) La impedancia cuando S1 y S2 se abren.
(f) La energía máxima almacenada en el condensador y la inductancia.
(g) La diferencia de fase entre voltaje y corriente si se dobla la frecuencia ω.
(h) La frecuencia para la cual la reactancia inductiva es igual a un medio de la reactancia capacitiva.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 28
Circuito RLC con Corriente Alterna

#### Problema 1
El circuito de la figura se denomina filtro RC pasa-altos porque transmite con mayor amplitud las
señales de alta frecuencia que las de baja. Si la tensión de entrada es Vin = V0 cos ωt, demostrar que
la de salida es
Vout = VR cospωt - ϕq,
donde
V0
VR = b
` 1 ˘2
1 ` ωRC
y estudie los casos en que ω ! RC
, ω = RC
y ω " RC
.

#### Solución
La impedancia del sistema viene dada por,
Z = R`

` ´1 ˘
“R`j
jωc
ωc

lo escribimos en forma fasorial para facilitar los cálculos,

(1)

---

### Página 2

c
iϕ

R2 `

Z “ |Z|e “

˙ȷ
„
exp i arctan
ω2C 2
ωRC

(2)

con esto podemos calcularla corriente (Fasorial) que pasa por la resistencia R como,
V̂
V0 e´iϕ
Iˆ “
“a
Z
R2 ` 1{ω 2 C 2 eiωt

(3)

con esta corriente podemos calcular la diferencia de potencial a través de R, que al estar conectado
en paralelo a la salida, coincide con Vout ,
ipωt´ϕq
ˆ R = aRV0 e
V̂ = IZ
R2 ` 1{ω 2 C 2

(4)

recordemos que solo nos interesa la parte real de este resultado,
RV0
cospωt ´ ϕq
Vout = RepV̂out q = a
R ` 1{ω 2 C 2

(5)

Si ω ! 1{RC (Frecuencias pequeñas),
V0 cospωt ´ ϕq
Vout = a
1 ` 1{ω 2 C 2 R2

(6)

Si ω ! 1{RC Ñ 1 ! 1{ωRC, entonces el denominador es muy grande, por lo que el voltaje de
salida es muy bajo, el sistema filtra las frecuencias bajas.
En el caso ω = 1{RC entonces,
Vout “ ? cospωt ´ ϕq

(7)

Nada especial, este ω se conoce como frecuencia de corte.
Para el caso ω " 1{RC se cumple que 1 " 1{ωRC entonces,
Vout “

V0 cospωt ´ ϕq
?
« V0 cospωt ´ ϕq
1`0

Este sistema deja pasar casi por completo las frecuencias altas.

(8)

---

### Página 3

#### Problema 2
Considere el circuito de la figura con una fuente de voltaje V (t) = V0 cos(ωt), una resistencia R,
una inductancia L y dos condensadores C1 y C2 con C1 = C y C2 = 2C:

a) Encuentre la ecuación diferencial (de segundo grado) que debe satisfacer las corrientes del
circuito.
b) Determine la impedancia equivalente del sistema.
c) Encuentre la expresión para la corriente alterna en función del tiempo. Además, determine el
valor de C, en términos de ω y L, que maximiza la amplitud de la corriente.

#### Solución
Partimos directamente con ley de Kirchhoff,
V = IR `

Q2
9 ` Q1
` IL
C2
C1

(9)

:
Derivamos respecto al tiempo para dejar todo en términos de I, I9 y I,
V9 = RI9 ` LI: `
I
2C

(10)

la derivada de V se calucla directamente,
V = V0 cos(ωt) Ñ V9 = -ωVo sin(ωt)

(11)

Entonces la ecuación de segundo orden a resolver sería,
I
´ωV0 sin(ωt) = LI: ` RI9 `
2C
Para la impedancia solo reemplazamos de forma directa,

(12)

---

### Página 4

˙
Zeq = R ` jωL `
`
“ R ` j ωL ´
jωC 2jωC
2ωC

(13)

Escribimos el voltaje y la impedancia en forma de fasores,
d
iϕ

Z “ |Z|e “

R2 `

ωL ´
2ωC

˙2
eiϕ

V̂ = V0 eiωt

(14)
(15)

Entonces la intensidad de corriente,
˜ ¸
V̂
“
Repeipωt´ϕq q
I(t) = Re
Z
|Zeq |

(16)

Entonces la intensidad de corriente es,
I(t) = b
`
˘2 cospωt ´ ϕq
R ` ωL ´ 2ωC

(17)

Queremos que el denominador sea lo más chico posible, como R es un valor fijo, solo nos queda,
ωL ´

“0
2ωC

(18)

2ω 2 L

(19)

Entonces,
C“

#### Problema 3
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
R

---

### Página 6

Por lo tanto,
I(t) = 

cospωtq .
R

(b) Potencia promedio entregada al circuito.
La potencia instantánea es
P (t) = V ptqI(t).
Como

cospωtq,
R

V (t) = V0 cos(ωt),

I(t) = 

P (t) = 

V02
cos2 pωtq.
R

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
I0 = a
R ` pωLq2
La diferencia de fase satisface
tan ϕ “
Por lo tanto,

ωL
R

ϕ = arctan

ωL
R

˙

En un circuito inductivo, la corriente se atrasa respecto del voltaje. Así,
I(t) = a
cospωt ´ ϕq
R ` pωLq2

---

### Página 7

donde
ϕ = arctan

ωL
R

˙

(d) Capacidad C para que, con S1 y S2 abiertos, la corriente y el voltaje estén en fase.
Si S1 y S2 están abiertos, el circuito es un circuito RLC en serie.
La impedancia es

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

Z = R ` i ωL ´
ωC

˙

El módulo de la impedancia es
d

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

|Z|

La energía almacenada en la inductancia es
UL = LI 2 .
Por lo tanto, su valor máximo es
UL,máx = LI02 .
Como
I0 “

,
|Z|

también podemos escribir
UL,máx = L
Para el condensador,

|Z|

˙2

UC = CVC2 .

La amplitud del voltaje en el condensador es
VC,0 = I0 XC = I0

ωC

Entonces,
UC,máx = C

I0
ωC

˙2

Por lo tanto,
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
R

---

### Página 9

Así,
R

˙2

R

˙2

UL,máx = L

UC,máx = L

y

Por lo tanto, en resonancia,
UL,máx = UC,máx .
(g) Diferencia de fase entre voltaje y corriente si se dobla la frecuencia.
Ahora la frecuencia angular es
Ω = 2ω.
La impedancia del circuito RLC es

Z = R ` i ΩL ´
ΩC

˙

La diferencia de fase entre voltaje y corriente satisface
ΩL ´ ΩC
R

tan ϕ “
Por lo tanto,

ϕ = arctan

ΩL ´ ΩC
R

˙

Como Ω = 2ω,
ϕ = arctan
Si usamos
C“
entonces

2ωL ´ 2ωC
R

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

Por lo tanto,
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
Por lo tanto,
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
