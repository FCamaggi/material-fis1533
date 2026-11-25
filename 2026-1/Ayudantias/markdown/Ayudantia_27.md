---
title: "Ayudantia 27"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_27.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_27_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 27

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 27
Inductancia y Circuito RLC

#### Problema 1
Considere la configuración de dos circuitos de la figura presente más adelante. Consiste en un
alambre infinito y una espira rectangular con dos lados paralelos al alambre y coplanar a este.

(a) Calcule la inductancia mutua M12 entre el alambre y la espira.
(b) Suponga que por el alambre circula una corriente I = I0 e´αt y que la espira rectangular
posee una resistencia R. Calcule la corriente inducida en la espira rectangular.
(c) Ahora suponga que la corriente del alambre es constante I0 y que la espira se comienza a
mover con rapidez constante v0 paralela al alambre. Calcule la corriente inducida I2 que
circula por la espira.
(d) Repita el cálculo anterior, pero ahora la espira se aleja de manera perpendicular.

---

### Página 2

#### Problema 2
Considere los circuitos LC y RLC que se observan en la figura. Suponga que el condensador tiene
una carga inicial Q0 . Si el interruptor se cierra en t = 0:

a) Encuentre la ecuación diferencial para la carga del condensador mediante consideraciones
energéticas para el circuito LC.
b) Utilizando las leyes de Kirchhoff, encuentre I(tq y Qpt) para el circuito LC.
c) Encuentre la EDO para el circuito RLC.
#### Problema 3
Considere el circuito de la figura.

Determine la corriente por cada resistencia:
1. Inmediatamente después de cerrar el interruptor.
2. Después de que ha pasado mucho tiempo de cerrado el interruptor.
3. Suponga que el interruptor es reabierto después de que ha estado mucho tiempo cerrado,
encuentre nuevamente las corrientes:
a) Inmediatamente después de que es abierto.
b) Después de un largo tiempo.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 27
Inductancia y Circuito RLC

#### Problema 1
Considere la configuración de dos circuitos de la figura presente más adelante. Consiste en un
alambre infinito y una espira rectangular con dos lados paralelos al alambre y coplanar a este.

(a) Calcule la inductancia mutua M12 entre el alambre y la espira.
(b) Suponga que por el alambre circula una corriente I = I0 e´αt y que la espira rectangular
posee una resistencia R. Calcule la corriente inducida en la espira rectangular.
(c) Ahora suponga que la corriente del alambre es constante I0 y que la espira se comienza a
mover con rapidez constante v0 paralela al alambre. Calcule la corriente inducida I2 que
circula por la espira.

---

### Página 2

(d) Repita el cálculo anterior, pero ahora la espira se aleja de manera perpendicular.

#### Solución
Por definición el coeficiente de inductancia mutua M12 se calcula como,
M12 “

Φ2
I1

(1)

es decir, necesitamos calcular el flujo magnético que pasa a través de la espira rectangular debido a
la corriente del alambre. Por ley de faraday sabemos que el campo magnético de un alambre es,
µ0 I1
B⃗1 “
θ̂
2πr
donde r corresponde a la distancia perpendicular al cable. Justo en el plano de la espira, el campo
magnético apunta en ẑ, por lo tanto θ̂ Ñ ẑ. Calculamos el flujo a través de la espira,
żbżh

ż
⃗ 1 ¨ dA
⃗2 “
B

Φ2 “
S

a

µ0 I1 h
µ0 I1 1
dxdy “
ln
2π
0 2π y

ˆ ˙
b
a

(2)

entonces,
µ0 h
ln
M12 “
2π

ˆ ˙
b
a

(3)

La fem inducida es
E(t) = ´

dΦ21
dI
“ -M12
“ -M12 p´αI0 e´αt q = αM12 I0 e´αt .
dt
dt

Por ley de Ohm en la espira,
E(t)
αM12
α µ0 h
“
I0 e´αt “
ln
I2 (t) = 
R
R
R 2π

ˆ ˙
b
I0 e´αt .
a

ahora la corriente en el alambre es constante, la expresión para el flujo sobre la espira sigue siendo,
µ0 I1 h
ln
Φ2 “
2π

ˆ ˙
b
a

si la espira se aleja de forma paralela al alambre ¿Qué parámetros de acá cambian en el tiempo?
Ninguno, la distancia d sigue siendo constante ya que se mueve en la dirección vertical, por lo
tanto,
E = ´

dΦ2
“ 0 Ñ I2 = 0
dt

---

### Página 3

Para el siguiente caso, las distancias a y b cambian con el tiempo porque la espira se va alejando
según a(t) = a0 ` v0 t y b(t) = b0 ` v0 t.

„
ȷ
a(t)
µ0 I0 h d
ln
E(t) = ´
2π dt
b(t)
calculando la derivada obtenemos,
E(t) = ´

µ0 I0 h
2π

˜

b9 a9
´
b a

¸

recordando que a9 = b9 = v0 ,
|E|
µ0 hI0
I2 “
“
v0
R
2πR

ˆ

´
a0 ` v 0 t b 0 ` v 0 t

˙

#### Problema 2
Considere los circuitos LC y RLC que se observan en la figura. Suponga que el condensador tiene
una carga inicial Q0 . Si el interruptor se cierra en t = 0:

a) Encuentre la ecuación diferencial para la carga del condensador mediante consideraciones
energéticas para el circuito LC.
b) Utilizando las leyes de Kirchhoff, encuentre I(tq y Qpt) para el circuito LC.
c) Encuentre la EDO para el circuito RLC.

#### Solución
Como hay resistencias en nuestro circuito, no hay energía disipada, eso quiere decir que la energía
total del sistema es constante y no varía en el tiempo,
U = UC ` U L = 
Como no se pierde energía, dU {dt = 0,

Q2 I 2 L
`
2C

---

### Página 4

Q dQ
dI
` LI
“0
C dt
dt
Toda la corriente que pasa por la inductancia es la carga que el condensador va perdiendo, es decir,
I = -dQ{dt,
Q
dI
p´Iq ` LI
“0
C
dt
´

Q
dI
`L = 0
C
dt

Q
d2 Q
´ -L 2 = 0
C
dt
Ordenando esta ecuación,
d2 Q
Q
`L 2 = 0
C
dt
Utilizando la ley de kirchoff llegamos a la siguiente ecaución de mallas,
Q
dI
Q
d2 Q
´ L = 0 ÝÑ ` L 2 = 0
C
dt
C
dt
Esta ecuación ya la conocemos, es un oscilador armónico con ω 2 = 1{LC, cuya solución viene
dada de forma general por,
Q(t) = A cos(ωt) ` B sin(ωt)
Las constantes las definimos a partir de las condiciones iniciales; como el condensador parte con
carga Q0 ,
Q(0) = Q0 = A
La constante B la sacamos a partir del hecho que la corriente inicial es nula,
I(t) = Q0 ω sin(ωt) ` Bω cos(ωt)
I(0) = 0 = Bω
ω es una constante que no puede ser 0, por lo tanto la única forma de que esto se cumpla es que
B = 0, quedando las ecuaciones de carga y corriente como,
Q(t) = Q0 cos(ωt)

---

### Página 5

I(t) = Q0 ω sin(ωt)
La energía podría entonces ser escrita como,
U“

ˆ

˙
Q20
cos pωtq ` LQ0 ω sinpωtq
C

Para la última pregunta, utilizando ley de Kirchoff (También se puede hacer con la energía) la
ecuación de malla viene dada por,
L

d2 Q
dQ Q
` = 0
`R
dt
dt
C

La pregunta era llegar a la EDO y no resolverla, de todas formas esta se puede hacer pro(oniendo Qpt) = Aeλt , donde λ se obtiene resolviendo el polinomio característico y A a partir de las
condiciones iniciales.
#### Problema 3
Considere el circuito de la figura.

Determine la corriente por cada resistencia:
1. Inmediatamente después de cerrar el interruptor.
2. Después de que ha pasado mucho tiempo de cerrado el interruptor.
3. Suponga que el interruptor es reabierto después de que ha estado mucho tiempo cerrado,
encuentre nuevamente las corrientes:
a) Inmediatamente después de que es abierto.

---

### Página 6

b) Después de un largo tiempo.

#### Solución
Denotemos por I1 la corriente que pasa por R1 , por I2 la corriente que pasa por R2 y por I3 la
corriente que pasa por R3 , siguiendo los sentidos indicados en la figura.
1. Inmediatamente después de cerrar el interruptor
Justo después de cerrar el interruptor, la corriente en la bobina no puede cambiar instantáneamente.
Como antes de cerrar el interruptor no circulaba corriente por la bobina, se tiene
I3 p0` q = 0.
Por lo tanto, la rama superior se comporta como un circuito abierto. El circuito equivalente queda
formado solamente por R1 y R2 en serie con la fuente ε. Entonces,
I1 p0` q = I2 p0` q = 

ε
.
R1 ` R2

Así,
I1 p0` q “

ε
R1 ` R2

I2 p0` q “

ε
R1 ` R2

I3 p0` q = 0
2. Después de mucho tiempo con el interruptor cerrado
Después de mucho tiempo, el circuito alcanza un estado estacionario. En corriente continua, la
bobina se comporta como un cable ideal, es decir, como un cortocircuito.
Por lo tanto, la rama superior queda equivalente a una resistencia R3 , y esta queda en paralelo con
R2 . La resistencia equivalente de esas dos ramas es
R23 “

R2 R3
.
R2 ` R3

Esta combinación está en serie con R1 , por lo que la corriente total es
I1 “

ε
.
R1 ` R23

---

### Página 7

Reemplazando R23 ,
I1 “

ε

.

R3
R1 ` RR22`R

Equivalentemente,
I1 “

εpR2 ` R3 q
.
R1 pR2 ` R3 q ` R2 R3

Definimos
D = R1 pR2 ` R3 q ` R2 R3 .
Entonces,
I1 “

εpR2 ` R3 q
D

La diferencia de potencial sobre las ramas en paralelo es
V23 = I1 R23 .
Por lo tanto,
I2 “

V23
,
R2

I3 “

V23
.
R3

De aquí se obtiene
I2 “

εR3
D

I3 “

εR2
D

y

donde
D = R1 pR2 ` R3 q ` R2 R3 .

---

### Página 8

3. Se reabre el interruptor después de mucho tiempo cerrado
Antes de abrir el interruptor, el circuito estaba en estado estacionario. Por lo tanto, la corriente en
la rama de la bobina era
I3 “

εR2
.
D

Al abrir el interruptor, la fuente queda desconectada del circuito. Sin embargo, la corriente en la
bobina no puede cambiar instantáneamente. Por eso,
I3 p0` q “

εR2
.
D

Ahora la corriente inducida por la bobina circula en el lazo formado por R3 , L y R2 . Como en la
rama superior la corriente mantiene el mismo sentido que tenía antes, en la resistencia R2 debe
circular en sentido contrario al indicado en la figura.
Por lo tanto,
I3 p0` q “

εR2
D

I2 p0` q = ´

εR2
D

Además, como la fuente queda desconectada, no circula corriente por R1 . Entonces,
I1 p0` q = 0
4. Después de un largo tiempo de haber abierto el interruptor
Después de mucho tiempo, la energía almacenada en la bobina se disipa en las resistencias. Por lo
tanto, la corriente en la bobina tiende a cero.
Así, todas las corrientes se anulan:
I1 = 0
I2 = 0
I3 = 0
