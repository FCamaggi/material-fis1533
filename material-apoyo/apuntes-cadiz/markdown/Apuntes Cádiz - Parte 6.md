---
title: "Parte 6"
source_pdf: "Electro/material-apoyo/apuntes-cadiz/Apuntes Cádiz - Parte 6.pdf"
pages: 34
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Parte 6

### Página 1

Parte VI
Inductancia y Corriente Alterna

---

### Página 2

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 3

#### Capítulo 13
Inductancia
A continuación veremos un fenómeno de acoplamiento magnético. Supongamos que tenemos
2 bobinas, cerca una de otra, como se muestra en la figura

La primera de ellas tiene N1 vueltas y lleva una corriente I1 , la que da origen a un campo
~ 1 . Debido a que ambas bobinas están cerca, algunas líneas de campo magnético a
magnético B
través de la bobina 1 también pasarán a través de la bobina 2, como se aprecia claramente en
la figura. Denotemos por Φ21 el flujo magnético total a través de la bobina 2 (que será N2 veces
el flujo a través de una sola vuelta) debido a la corriente I1 .
Ahora, al variar I1 en el tiempo, habrá una fem inducida en la bobina 2 debido al cambio de
flujo magnético en ella
ˆ ˆ
dΦ21
d
~ ·B
~1
dS
ε21 = −
=−
dt
dt
S2
Ahora, por regla de la cadena
dI1
dΦ21
dΦ21 dI1
=
= M21
dt
dI1 dt
dt

---

### Página 4

Notar que aquí hemos establecido que el flujo sobre 2 es proporcional a la corriente I1 , es decir, dφ21 /dI1 = M21 donde la constante de proporcionalidad M21 se llama inductancia mutua,
y depende únicamente de la geometría y es una medida de que tan bueno es el acoplamiento
magnético.
Vemos que es igual a
dΦ21
Φ21
M21 =
=
dI1
I1
esto último se debe a que los flujos siempre dependen linealmente de las corrientes que los
originan. La unidad S.I de la inductancia mutua es el Henry (H).
Análogamente, ahora suponga que existe una corriente I2 en la segunda bobina y que varía
en el tiempo. Así, se induce una fem en la bobina 1 dada por
ˆ ˆ
dΦ12
d
~1
~ 2 · dS
ε12 = −
=−
B
dt
dt

Este flujo variable en la bobina 1 es proporcional al cambio de corriente en la bobina 2
dI2
dΦ12
dΦ12 dI2
=
= M12
dt
dI2 dt
dt
donde

dΦ12
Φ12
=
dI2
I2
Utilizando la ley de Ampere y la de Biot-Savart se puede deducir la fórmula de Neumann,
y se puede demostrar que ámbas inductancias mutuas son iguales (muy útil!)
M12 =

M21 = M12 = M
Esto es claro al ver la expresión de la fórmula de Neumann para dos circuitos
˛ ˛
d~l1 · d~l2
µ0
M21 =
4π C2 C1 |~r2 − ~r1 |
la cual es totalmente simétrica, de manera que el intercambiar los índices por M12 no altera
el resultado.

Autoinductancia
Considere nuevamente una bobina de N vueltas que lleva una corriente I en el sentido contrareloj. Si la corriente es constante, entonces el flujo magnético a través de cada vuelta permanecerá constante. Ahora considere que la corriente I varía en el tiempo, luego, de acuerdo a
la ley de Faraday-Lenz, una fem inducida aparecerá para oponerse al cambio de flujo.

---

### Página 5

La corriente inducida irá en el sentido del reloj si dI/dt > 0 y contrareloj si dI/dt < 0. (Recordar
Ley de Lenz!). La propiedad de que su propio campo magnético se opone a cualquier cambio
en la corriente es lo que se llama inductancia propia o autoinductancia, y la fem generada
entre sus terminales se llama fem autoinducida, que se denota por εL . Todo elemento de este
tipo se denomina Indutancia. Matemáticamente, se tiene
ˆ ˆ
dΦB
d
~ · dS
~
εL = −
B
=−
dt
dt
dΦB dI
dI
dΦB
=
=L
dt
dI dt
dt
de manera que
εL = −L
donde L es la autoinductancia,

dI
dt

ΦB
I
Físicamente, la autoinductancia es una medida de la resitencia de una inductancia al cambio
de corriente, así, mientras más grande es el valor de L, más lenta será la tasa a la cual varía la
corriente.
La autoinductancia también se puede pensar (de hecho es equivalente en términos de la fórmula
de Neumann) como la indutancia mutua del circuito consigo mismo, es decir, L = M11 .
L=

---

### Página 6

Energía almacenada en campos magnéticos
Debido a que una inductancia en un circuito se opone a cualquier cambio en la corriente a través
de ella, debe realizarse un trabajo por un agente externo (como una batería) para establecer
una corriente en la inductancia. La energía entonces se puede almacenar en ella!. El rol que
juega una inductancia en el caso magnético es análogo al de un condensador en el caso eléctrico.
La potencia, o tasa a la cual una fem externa trabaja para superar la fem autoinducida en la
inductancia (εL ) y lograr que pase una corriente I a través de ésta es
P =

dWext
= Iεext
dt

Si solo una fem externa y la indutancia están presentes, entonces ε = −εL , esto es
P = −IεL = IL

dI
dt

Si la corriente aumenta con dI/dt > 0, entonces P > 0 lo que significa que la fuente externa
está haciendo un trabajo positivo para transferir energía a la inductancia. Entonces, la energía
interna UB de la inductancia aumenta.
Por otro lado, si la corriente decrece dI/dt < 0, la fuente externa toma energía de la inductancia,
causando una disminución en la energía interna de ésta.
El trabajo total hecho por la fuente externa para aumentar la corriente desde 0 hasta I es
ˆ
ˆ I
LIdI = LI 2
Wext = dWext =
Esto es igual a la energía magnética almacenada en la inductancia
UB = LI 2
ésta expresión es análoga a la energía eléctrica almacenada en un condensador
1 Q2
UE =
2C
Existe una distinción importante entre una inductancia y una resistencia, desde el punto de
vista de la energía. Cuando una corriente I pasa a través de una resistencia, energía fluye a
través de la resistencia y se disipa en forma de calor, independiente si la corriente es constante
o dependiente del tiempo.
Por otro lado, energía fluye en una inductancia solo cuando existe una corriente que varía en
el tiempo , con dI/dt > 0. La energía no es disipada pero sí almacenada, y es liberada después
cuando dI/dt < 0

---

### Página 7

Circuitos RL
Considere el circuito RL que se muestra en la figura. En t=0, el interruptor es cerrado. Veremos
que la corriente no alcanza inmediatamente su máximo valor ε/R. Ésto se debe a la presencia
de una fem autoinducida en la inductancia.

Utilizando la ley de voltajes de Kirchhoff
−ε + IR + |εL | = −ε + IR + L

dI
=0
dt

se obtiene entonces una ecuación diferencial para la corriente
L

dI
= ε − IR
dt

la que se puede resolver por el método de separación de variables
LdI = dt(ε − IR) →

dI
dt
=
(ε − IR)
L

dt
dI
=
(ε/R − I)
L/R

Integrando a ambos lados de la ecuación

ln(I − ε/R) = −t

R
+ C1
L

así

R

I − ε/R = Ce−t L

I(t) = Ce−tR/L + ε/R
Imponiendo la condición I(0) = 0, se tiene C = −ε/R
I(t) =

ε
(1 − e−tR/L )
R

---

### Página 8

Se define entonces la constante de tiempo de este circuito como τ = L/R, así
I(t) =

ε
(1 − e−t/τ )
R

Notar que despues de un tiempo suficientemente largo, la corriente llega a su valor de
equilibrio ε/R. El hecho de que no alcanze este valor de forma inmediata se debe justamente a
que la inductancia tiende a oponerse a que la corriente varié de forma brusca. La constante de
tiempo τ es una medida de qué tan rápido se llega al estado de equilibrio, mientras mayor es
el valor de L, más tiempo le toma al circuito a llegar a éste estado.
Similarmente, la magnitud de la fem autoinducida se puede obtener como
|εL | = | − L

dI
| = εe−t/τ
dt

La cual es máxima cuando t=0 y desaparece cuando t tiende a infinito. Esto implica que
despues de un largo tiempo desde que el interruptor es cerrado, la autoinducción desaparece y
la inductancia siplemente actúa como un alambre conductor conectando 2 partes del circuito.
Para verificar que la energía se conserva, basta multiplicar la ecuación de Kirchhoff por I, para
obtener
dI
Iε = I 2 R + LI
dt
Notar que el lado izquierdo representa la potencia entregada por la batería, parte de ésta se
disipa en la resistencia (I 2 R) y el resto se almacena en la inductancia. La energía disipada por la
resistencia es irrecuperable, mientras que la almacenada por la inductancia se puede reutilizar
después

---

### Página 9

Para verificar esto último, considere ahora el circuito RL que se muestra en la figura. El
interruptor S1 ha estado cerrado por un tiempo muy largo tal que la corriente está en equilibrio
con valor ε/R. Que ocurre cuando en t=0 el interruptor S1 se cierra y el S2 se abre?

Sumando las caídas de potencial obtenemos que
−|εL | + IR = −L
L

dI
+ IR = 0
dt

dI
dI
dt
= −IR →
=−
dt
I
L/R

Integrando ambos lados de la ecuación
I(t) = Ce−t/τ
Imponiendo la condición I(0) = ε/R
I(t) =

ε −t/τ
e
R

Es decir, una vez que se desconecta la fuente de energía (batería), la energía almacenada
por la inductancia es liberada y entregada a la resistencia, quien disipa esta energía en forma
de calor

---

### Página 10

Circuitos de Corriente Alterna
En ayudantías anteriores vimos que un flujo magnético que cambia en el tiempo puede inducir
una fem de acuerdo a la ley de Faraday. En particular, si una espira rota con velocidad angular
w en la presencia de un campo magnético, la fem inducida varía sinusoidalmente en el tiempo
(con frecuencia w) y produce una corriente alterna (AC). Este es el caso típico de generación
de energía y de los grandes sistemas de potencia. El símbolo para una fuente de voltaje alterna
es

Un ejemplo de fuente AC es
V (t) = V0 cos wt
donde el valor máximo V0 se llama amplitud. El voltaje varía entre V0 y −V0 . Un gráfico
del voltaje como función del tiempo se muestra en la siguiente figura

Es una función periódica en el tiempo. La frecuencia f , definida como 1/T donde T es el
período, tiene unidades de 1/seg (hertz).
√ Se relaciona con la frecuencia angular según w = 2πf .
En nuestras casas obtenemos V0 = 220 2 y f = 50 Hz
Cuando una fuente de voltaje se conecta a un circuito RLC, después de un tiempo transiente,
una corriente alterna comenzará a fluír por el circuito como respuesta a la fuente de voltaje
forzante. La corriente será de la forma
I(t) = I0 cos(wt − φ)
Es decir,oscilará con la misma frecuencia de la fuente (esta es una propiedad de los sistemas
lineales), con amplitud I0 y fase φ que dependerán de la frecuencia forzante de la fuente
Antes de examinar circuitos RLC complejos, primero consideremos casos simples donde sólo un
elemento se conecta a una fuente de voltaje sinusoidal

---

### Página 11

Carga puramente resistiva
Considere un circuito puramente resistivo con una resistencia conectada a un generador AC,
como se muestra en la figura

Sumando las caídas de potencial, obtenemos
V (t) − VR (t) = V (t) − I(t)R = 0
donde VR (t) = I(t)R es el voltaje instantáneo a través de la resistencia. La corriente instantánea en la resistencia (y en el circuito) está dada por
VR (t)
V0 coswt
=
= IR0 cos wt
R
R
Notamos que φ = 0, lo que significa que I(t) y V (t) están en fase, es decir, alcanzan sus
valores máximos y mínimos al mismo tiempo.
I(t) =

Ahora, podemos representar voltajes y corrientes con números complejos, así, la fuente que
representamos como V (t) = V0 cos(wt) en forma compleja es, simplemente
V (t)∗ = V0 eiwt = Vo (cos wt + i sin wt) = V̂ eiwt
donde V̂ es el voltaje en forma de fasor. En este caso V̂ = Vo , pero en otras circunstancias
podría ser un número complejo. Por supuesto lo que entendemos aquí por voltaje es la parte
real de V ∗ (t). Similarmente las corrientes también las podemos escribir en forma fasorial.

---

### Página 12

Definimos la Impedancia de una resistencia por el número complejo
Ẑ = R
Esto corresponde a la resistencia expresado como fasor. En el caso de una resistencia es por
supuesto un número real. De esta forma
V̂

= Iˆ
Ẑ
Esto se cumple de forma general, de modo que al tratar estos problemas con fasores, siempre
se cumple que V̂ = IˆẐ, lo que simplifica enormemente los cálculos. En este caso en particular
V̂
= Iˆ
R
V0
V̂
=
Iˆ =
R
R
y entonces la corriente es
ˆ iwt = V0 eiwt
I(t)∗ = Ie
R
I(t) =

V0
cos wt
R

Carga puramente inductiva
Considere ahora una carga inductiva que consiste de una inductancia conectada a una fuente
AC

Se tiene
V (t) − VL (t) = V (t) − L

dI
=0
dt

lo que implica
dI
V (t)
Vo
=
=
cos wt
dt
L
L
Integrando
IL =

ˆ

Vo
dIL =
L

ˆ

dt cos wt =

V0
V0
sin wt =
cos(wt − π/2)
wL
wL

V0
de aquí vemos que la amplitud del voltaje en la inductancia es wL
= XV0L , donde XL = wL
se llama reactancia inductiva. Tiene unidades de Ohm (Ω), igual que las resistencias. Sin
embargo, a diferencia de una resistencia común, la reactancia depende de la frecuencia. Esto
se debe al hecho de que a frecuencias más altas la corriente varía de forma más rapida que
a frecuencias bajas. Por otro lado, esta reactancia se anula cuando w tiende a cero. También
, es decir, la corriente está en atraso con respecto al voltaje, como se
notamos que φ = −π
aprecia en la figura

---

### Página 13

Veamos como se obtiene este resultado de forma inmediata utilizando fasores, todo lo que
hay que saber es que la inductancia equivale a una impedancia igual a
ZL = iXL = iwL
De esta forma, el voltaje en la inductancia se relaciona con la corriente a través de ella según
V̂L = ẐL Iˆ
es decir, trabajando con fasores es una simple ley de Ohm (entre comillas). Como el voltaje
en la inductancia aquí es igual al voltaje de la fuente
V̂ = V̂L = iwLIˆ
Despejando la corriente
Iˆ =

i
1 −iπ/2
V̂ = −
V̂ =
e
V̂
jwL
wL
wL

En este caso, V̂ = Vo , con lo que la corriente en función del tiempo queda
ˆ iwt =
I(t)∗ = Ie
tomando la parte real
I(t) =

Vo i(wt−π/2)
e
wL

V0
cos(wt − π/2)
wL

---

### Página 14

Carga puramente capacitiva

Aquí, nuevamente tenemos
V (t) − VC (t) = V (t) −

Q(t)
=0
C

Q(t) = CV (t) = CVc (t) = CV0 cos wt
además, la corriente en el circuito está dada por
dQ
= −CwV0 sin wt = CwV0 cos(wt + π/2) = CwV (t)
dt
de aquí encontramos la relación entre la amplitud del voltaje y la amplitud de la corriente
a través del condensador
I(t) =

I0 = XC I0
Cw
donde Xc es la reactancia capacitiva del condensador. Vemos que en este caso la corriente
está desfasada en φ = −π/2 con respecto al voltaje (es decir, está en adelanto con respecto a
este)
V0 =

En términos de fasores, simplemente consideramos la impedancia de un condensador
ẐC =
de forma que

jwC

V̂ = ẐC Iˆ

despejando la corriente
V̂
Iˆ =
= iwC V̂ = iwCVo = wCVo eiπ/2
ẐC
Así

ˆ iwt = wCVo ei(wt+π/2)
I(t)∗ = Ie

---

### Página 15

tomando la parte real
I(t) = wCVo cos(wt + π/2)
Fácil fácil con fasores!
El circuito resonante RLC
Consideremos ahora el circuito RLC de la figura

Aquí tenemos
V (t) − VR (t) − VL (t) − VC = V (t) − IR − L

Q
dI
− =0
dt
C

lo que nos lleva a la siguiente ecuación diferencial
L

dI
Q
+ IR + = Vo cos wt
dt
C

Asumiendo que el condensador está inicialmente descargado, y considerando I = dQ
, podedt
mos reescribirla como
d2 Q
dQ Q
+R
+ = Vo cos wt
dt
dt
C
Una solución posible es (en régimen permanente)
L

Q(t) = Q0 sin(wt + φ)
donde la amplitud y la fase son, respectivamente
V0 /L
V0
Q0 = q
= p
1 2
w R2 + (wL − 1/wC)2
(Rw/L)2 + (w2 − LC
)
Q0 =
y
tanφ =

V0
p
w R + (XL − XC )2

XL − XR
(wL −
)=
R
wC
R

la correspondiente corriente es
I(t) =
con amplitud

dQ
= Io cos(wt + φ)
dt

V0
I0 = Q0 w = p
R2 + (XL − XC )2

---

### Página 16

Notar que la corriente tiene la misma amplitud y fase en todos los puntos del circuito RLC.
Por otro lado, el voltaje instantáneo a través de cada uno de los 3 elementos tiene diferente
amplitud y fase con respecto a la corriente. Habrán notado que resolver los problemas mediante
esta forma puede resultar complicado, de forma que indicaré una solución con fasores, y sacarán
sus propias conclusiones.
En términos de fasores, podemos ver el circuito como una sola impedancia equivalente, como
la resistencia, la inductancia y el condensador se encuentran en serie, tenemos
Ẑeq = R + iwL +

= R + i(wL −
)
iwC
wC

la amplitud de este número complejo es, simplemente
mod Z

mod =

r

R2 + (wL −

1 2
)
wC

y la fase
wL − wC
φ = arctan(
)
R

de esta forma, si el voltaje de la fuente es
V̂ = V0 ∠0
entonces la corriente a través del circuito es
wL − wC
V̂
V0
ˆ
I=
)
=q
∠arctan(
R
1 2
Ẑ
R2 + (wL − wC
)

Por último, recordando que
ˆ iwt =| I | ei(wt+φ)
I(t)∗ = Ie
V0
I(t) = q
cos(wt + φ)
1 2
R2 + (wL − wC
)
wL− 1

donde φ = arctan( R wC )
Notar que la amplitud de la corriente I0 = VZ0 alcanza un máximo cuando Z es mínimo.
Esto ocurre cuando XL = XC , o wL = wC
, llevando a
w0 = √

LC

Este fenomeno en que I0 alcanza su máximo se llama Resonancia, y la frecuencia a la cual
ocurre, w0 , se llama frecuencia de resonancia. En resonancia, la impedancia se transforma en
Z = R (puramente resistiva), y la amplitud de la corriente es
I0 =

V0
R

y la fase φ = 0

---

### Página 17

El circuito resonante es últil en varias aplicaciones, como sintonizadores y tarjetas electrónicas, donde se desea que el circuito responda a señales de un rango de frecuencias limitado.

---

### Página 18

El transformador
Un transformador es un dispositivo utilizado para aumentar o disminuír el voltaje AC en un
circuito. Una típica configuración consiste de 2 bobinas, (primaria y secundaria), enrolladas en
un núcleo de hierro, como se muestra en la figura

La bobina primaria, con N1 vueltas, es conectada a una fuente alterna V1 (t). La secundaria
tiene N2 vueltas y se conecta a una resistencia de carga R2 . La forma en que funcionan los
transformadres se basa en la ley de Faraday, la corriente alterna en el primario induce una fem
alterna en la segunda bobina, debido a su inductancia mutua.
En el circuito primario, despreciando la resistencia de la bobina, la ley de Faraday implica
V1 = −N1

dΦB
dt

donde ΦB es el flujo magnético a través de la bobina primaria. El nucleo de hierro sirve para
incrementar el flujo magnético producido por la bobina 1 (el hierro tiene permeabilidad µ mucho
mayor a la del vacío) y para asegurar que prácticamente todo el flujo magnético por el primario
también atraviese la bobina secundaria. Así, el voltaje inducido en el secundario es
V2 = −N2

dΦB
dt

En un transformador ideal, la pérdida de potencia debida al efecto Joule se puede despreciar,
de manera que la potencia administrada a la bobina primaria es transferida completamente a
la secundaria
I1 V1 = I2 V2
También estamos suponiendo que no hay flujo magnético que escape afuera del núcleo de
hierro. Combinando esto obtenemos
N2
V2
=
V1
N1
I2
N1
=
I1
N2
vemos que la razón para los voltajes está completamende determinada por la razón entre el
número de vueltas entre el primario y el secundario. El transformador tiene una infinidad de
aplicaciones, todos los equipos elécticos utilizan uno para transformar los 220 V efectivos en el
voltaje deseado de operación. Notar que con corriente continua un transformador simplemente
no funciona (Es una de las razones de las porqué no se genera en corriente continua).

---

### Página 19

#### Problema 1
Considere dos espiras coplanares y concéntricas, de radios R1 y R2 con R1
R2 . Encuentre la
inductancia mutua entre ambas espiras.

#### Solución
La inductancia mutua se puede obtener suponiendo que por el anillo más grande circula una
corriente I1 , como muestra la figura:

Anteriormente vimos que el campo magnético en el centro de un anillo que lleva corriente
I1 está dado por
~ 1 = µ0 I1 k̂
B
2R1
Debido a que R1
R2 , aproximamos el campo magnético sobre toda la espira interior por
~
B1 . Así, el flujo a través de la espira interior es
~1 · S
~
Φ21 = B
Si definimos la normal a la superficie encerrada por el anillo interior según el eje k̂
µ0 I1 2 µ0 I1 πR22
πR2 =
2R1
2R1
Finalmente, la inductancia mutua está dada por
Φ21 = B1 S =

M=

Φ21
µ0 πR22
=
I1
2R1

---

### Página 20

#### Problema 2
Considere un toroide de N vueltas y de sección rectangular de lado h, radio interior a y radio
exterior b.

a) Calcule la autoinductancia y discuta que ocurre cuando a
b − a
b) Calcule la energía magnética almacenada en el toroide
#### Solución
Utilizando la ley de Ampere, el campo magnético se obtiene como
˛
˛
˛
~ · d~l = Bdl = B dl = B(2πr) = µ0 N I
B
donde se ha integrado el campo sobre una circunferencia de radio r ubicada en el centro del
toroide
µ0 N I
B=
2πr
El flujo magnético sobre una vuelta del toroide se puede obtener al integrar sobre todas las
secciones rectangulares, con dA = hdr como elemento diferencial de área

ˆ b

µ0 N Ih
µ0 N I
hdr =
ln(b/a)
2πr
2π
a
y el flujo total sobre el toroide será N ΦB . Con esto, la autoinductancia es
ΦB =

ˆ ˆ

~ · dS
~=
B

N ΦB
µ0 N 2 h
L=
=
ln(b/a)
I
2π
cuando a
b − a, se tiene
ln(b/a) = ln(1 +
y la autoinductancia es
L=

b−a
b−a
)≈
a
a

µ0 N 2 h b − a
2π
a

---

### Página 21

recordando que el área de una sección del toroide es A = h(b − a)
µ0 N 2 A
L=
2πa
y con l = 2πa

µ0 N 2 A
l
que es justamente la autoinductancia de un solenoide.
L=

b) La energía almacenada en el toroide es simplemente
µ0 N 2 I 2 h
U = LI 2 =
ln(b/a)
4π

---

### Página 22

#### Problema 3
Considere el siguiente circuito LC. Suponga que el condensador tiene una carga inicial Q0 . En
t=0, el interruptor se cierra.

a) Encuentre la ecuación diferencial para la carga en el condensador mediante consideraciones
energéticas.
b) Utilizando las leyes de Kirchhoff encuentre I(t) y Q(t)

#### Solución
a) En ausencia de una resistencia, la energía total se transforma constantemente en energía
eléctrica y magnética, esto se llama osilación electromagnética.
Le energía total del circuito LC en un instante arbitrario es
U = UC + UL =

1 Q2 1 2
+ LI
2C

Por el principio de conservación de la energía
d 1 Q2 1 2
dU
= (
+ LI ) = 0
dt
dt 2 C
dI
Q dQ
+ LI
=0
C dt
dt
Además, hay que notar que I = −dQ/dt
Q
dI
Q
d2 Q
− I + LI
=0→− −L 2 =0
C
dt
C
dt
Finalmente la ecuación diferencial para la carga en el condensador es
Q
d2 Q
+L 2 =0
C
dt
b)Utilizando la ley de voltajes de Kirchhoff,
−VC + VL = −

Q
dI
+L =0
C
dt

y relacionando la corriente con la carga en el condensador
Q
dQ2
+L 2 =0
C
dt

---

### Página 23

dQ2
Q
=0
+
dt
LC
la solución general es de la forma
Q(t) = Q0 cos(w0 t + φ)
donde la frecuencia angular w0 está dada por
w0 = √

LC

La corriente por la inductancia es
I(t) = −

dQ
= w0 Q0 sin(w0 t + φ) = I0 sin(w0 t + φ)
dt

donde I0 = w0 Q0 . De las condiciones iniciales Q(0) = Q0 e I(0) = 0, la fase φ es simplemente
0.
Con esto, las soluciones para la carga y la corriente en el circuito LC es
Q(t) = Q0 cos(w0 t)
I(t) = I0 sin(w0 t)
la dependencia de Q(t) e I(t) se muestra en la figura:

La energía eléctrica y magnética están dadas por
UE =

Q2
Q2 (t)
= ( 0 )cos2 (w0 t)
C
2C

LI 2
Q2
UL = LI 2 (t) = 0 sin2 (w0 t) = 0 sin2 (w0 t)
2C
Se ve fácilmente que la energía permanece constante
Q2
Q2
Q20
)cos2 (w0 t) + 0 sin2 (w0 t) = 0
2C
2C
2C
La oscilación de energía magnética y eléctrica en el tiempo se ve en la figura
U =(

---

### Página 24

El análogo mecánico de este circuito LC es el sistema masa-resorte

---

### Página 25

#### Problema 4
Considere el circuito RLC en serie, que consta de una resistencia, una inductancia, y un condensador

Mediante consideraciones energéticas encuentre la ecuación diferencial para la carga en el condensador
#### Solución
La energía en un instante arbitrario t está dada por
U = UE + UL =

1 Q2 1 2
+ LI
2C

A diferencia del circuito LC, parte de la energía del circuito será disipada por la resistencia.
Esto es, la tasa a la cual la energía es disipada es
dU
= −I 2 R
dt
donde el signo negativo implica que la energía total disminuye en el tiempo. Así
Q dQ
dI
dU
=
+ LI
= −I 2 R
dt
C dt
dt
Aquí, nuevamente se tiene I = −dQ/dt
dI
Q
= −I 2 R
− I + LI
C
dt
−

dI
Q
+ L = −IR
C
dt

dQ
Q
dQ2
−L 2 =
R
C
dt
dt
Finalmente, la ecuación diferencial para Q es
−

L

dQ2 dQ
Q
+
R+ =0
dt
dt
C

---

### Página 26

#### Problema 5
Considere el circuito de la figura

Determine la corriente por cada resistencia
a) inmediatamente después de cerrar el interruptor
b) después de que ha pasado mucho de tiempo de cerrado el interruptor
Suponga que el interruptor es reabierto después de que ha estado mucho tiempo cerrado, encuentre nuevamente las corrientes:
d) inmediatamente después de que es abierto
e) después de un largo tiempo
#### Solución
a) Inmediatamente después de que el interruptor es cerrado, la corriente a través de la inductancia es cero ya que la fem autoinducida evita que la corriente crezca abruptamente.
Así, I3 = 0.
Debido a que I1 = I2 + I3 , se tiene que I1 = I2

Utilizando las leyes de Kirchhoff a la malla 1, se tiene
−ε + I1 R1 + I1 R2 = 0
ε
R1 + R2
b) Después de un largo tiempo, no hay fem autoinducida en la inductancia y las corrientes
pasan a ser constantes. Para la malla 1, se tiene ahora
I1 = I2 =

−ε + I1 R1 + I2 R2 = 0
y para la malla 2

---

### Página 27

I3 R3 − I2 R2 = 0
por último, por la ley de nodos, I1 = I2 + I3 . Resolviendo, se obtiene
I1 =

(R2 + R3 )ε
R1 R2 + R1 R3 + R2 R3

I2 =

R3 ε
R1 R2 + R1 R3 + R2 R3

I3 =

R2 ε
R1 R2 + R1 R3 + R2 R3

c) Inmediatamente después de que el interruptor es abierto nuevamente, la corriente a través
de R1 es 0, I1 = 0. Esto implica que I2 + I3 = 0.
La malla 2 ahora forma un circuito RL que decae e I3 comienza a decaer. Así
I3 = −I2 =

R3 ε
R1 R2 + R1 R3 + R2 R3

d)Después de mucho tiempo , todas las corrientes son cero, esto es, I1 = I2 = I3 = 0

---

### Página 28

#### Problema 6
Considere el circuito de la figura, donde V (t) = Vo cos wt. Si S1 y S2 se cierran inicialmente,
encuentre (Datos son R, L, Vo y w)

a) La corriente en función del tiempo
b) La potencia promedio entregada al circuito
c) La corriente en función del tiempo largo tiempo después de que S1 se abre
d) La capacidad C si S1 y S2 se abren y después de un tiempo largo, la corriente y el voltaje
están en fase
e) La impedancia cuando S1 y S2 se abren
f) La energía máxima almacenada en el condensador y la inductancia
g) La diferencia de fase entre voltaje y corriente si se dobla la frecuencia w
h) La frecuencia para la cual la reactancia inductiva es igual a un medio de la reactancia capacitiva
#### Solución
a) Al cerrar ambos interruptores, no circulará corriente ni por la inductancia ni por el condensador. La impedancia equivalente en este caso es Zeq = R de modo que la corriente es,
simplemente
Vo
I(t) =
cos wt
R

b) La potencia instantánea consumida por la resistencia es
P (t) = V (t)I(t) =

Vo2
cos2 wt
R

Claramente una función periódica, el promedio temporal es entonces
< P (t) >=
T

ˆ T
o

dtP (t) =

Vo2
2R

c) Cuando se abre S1 , se conecta la inductancia al circuito. La impedancia equivalente en
este caso es
Zeq = R + iwL =

√

wL

R2 + w2 L2 eiarctan( R )

Luego, la corriente es
wL
V̂
Vo
Iˆ =
=√
e−iarctan( R )
Zeq
R 2 + w 2 L2

---

### Página 29

Así,
ˆ iwt ) = √
I(t) = Re(Ie

Vo
cos(wt − tan−1 (wL/R))
R +w L

d) Ahora se conecta además el condensador, de modo que la impedancia equivalente en este
caso es
Zeq = R + iwL +

= R + i(wL −
) =| Z | eiφ
iwC
wC

donde está dado por
(wL − wC
)
R
como no hay desfase entre voltaje y corriente, φ = 0 (el circuito está en resonancia!), esto
quiere decir que w = wo

φ = tan−1

φ = 0 → tan−1 = 0
wo L =
C=

wo C

wo2 L

e) El circuito está en resonancia, luego
r
| Z |=

R2 + (wL −

1 2
) =R
wC

f) La energía máxima en el condensador es (Vc representa la amplitud del voltaje en el
condensador)
Io 2
)
UEmax = CVc2 = C(
2 wC
1 Vo 2 1
V02 L
UEmax = C
=
2 R wo2 C 2
2R2
En el√último paso se ha usado que la frecuencia es igual a la frecuencia de resonancia
w0 = 1/( LC) Ahora, la energía máxima almacenada por la inductancia
LVo2
ULmax = LIo2 =
2R2

g) Si la frecuencia es ahora
w = 2wo = √

LC

el ángulo de desfase entre voltaje y corriente queda

---

### Página 30

√
√
wL − 1/(wC)
−1 2/( LC)L − ( LC/(2C))
φ = tan (
) = tan (
)
R
R
r
L
)
φ = tan−1 (
2R C
−1

h) Finalmente, la frecuencia para que XL = 12 XC debe cumplir
wL =
luego
w=√

1 1
2 wC

wo
=√
2LC

---

### Página 31

#### Problema 7
Una antena FM tiene una inductancia L = 10−6 H, una capacidad C = 10−12 F, y una
resistencia R = 100 Ω. Una señal de radio induce una fem sinusoidal en la antena con amplitud
10−5 V

a) A que frecuencia angular w0 de la señal incidente el circuito estará sintonizado, esto es, para
que w0 la corriente en el circuito será máxima?
b) Asumiendo que la onda incidente está sintonizada, cual será la amplitud de la corriente en
el circuito a esta frecuencia?
c) Cuál es la amplitud de la diferencia de potencial a través del condensador a esta frecuencia?
#### Solución
a) La antena estará sintonizada con la señal incidente a la frecuencia de resonancia, esto es, la
señal debe tener una velocidad angular dada por
r
r
= 109
w0 =
=
−6
LC
10 10−12
y la frecuencia asociada es
f=

1 9
w0
=
10 = 0, 159 ∗ 109
2π
2π

Equivalentemente f = 0, 159Ghz.
b) A la frecuencia de resonancia, la corriente máxima es
10−5
V0
=
= 0, 1µA
R
c)La amplitud del voltaje en la inductancia
I0 =

VL = I0 XL = I0 w0 L = 0, 1 ∗ 10−6 2π ∗ 0, 159 ∗ 109 ∗ 10−6 = 9, 99 ∗ 10−5 V

---

### Página 32

#### Problema 1
Dado el circuito de la figura, suponer que el interruptor S se ha cerrado durante un largo tiempo,
de modo que existen corrientes estacionarias en el inductor de L = 2H y que su resistencia es
despreciable. Además R1 = 10 Ω, ε = 10 V
(a) Determinar la intensidad de corriente suministrada por la batería, la corriente que circula
por la resistencia R2 = 100 Ω y la intensidad que circula por el inductor
(b) Determinar el voltaje inicial entre los extremos del inductor cuando se abre el interruptor
S

#### Problema 2
El circuito de la figura se denomina filtro RC pasa-altos porque transmite con mayor amplitud
las señales de alta frecuencia que las de baja. Si la tensión de entrada es Vin = V0 cos wt,
demostrar que la de salida es Vsal = VR cos(wt − φ), donde
V0
VR = q
1 + ( wRC
)2

#### Solución problema 1

Cuando el interruptor S ha estado cerrado por largo tiempo, las corrientes llegan a un estado
de regimen permanente. Si IL (t) denota la corriente a través de la inductancia, se tiene que el
voltaje a través de ésta es

---

### Página 33

vL (t) = L

dIL
dt

En régimen estacionario

dIL
=0
dt
Así, no hay diferencia de potencial entre los extremos de la inductancia. Esto significa que
en régimen permanente la inductancia se comporta como un cortocircuito

En esta situación, toda la corriente se irá por la inductancia, de esta forma
IR100Ω = 0
Para obtener la intensidad que circula por el circuito, simplemente sumamos las caídas de
potencial y se obtiene
−ε + IR1 = 0
I=

ε
=
= 1A
R1

b) En el instante en que se abre nuevamente el interruptor, circula corriente a través de la
inductancia y la resistencia de 100Ω

Sea I(t) la corriente que fluye en este caso. Por continuidad, I(0) = 1A, con esto
IR2 + VL = 0
VL = −IR2 = −1 ∗ 100 = −100V

---

### Página 34

#### Solución Problema 2
El circuito consiste en un condensador en serie con una resistencia

La impedancia equivalente está dada por
=R−i
iwC
wC
Conviene expresar esta impedancia en su forma polar
r
Ẑ = R2 + 2 2 eiφ
w C
donde φ está dado por
)
φ = tan−1 (
wRC
De esta forma, se tiene
Ẑ = R +

V̂in = Ẑ Iˆ
V̂in
Vo
Iˆ =
=q
Ẑ
R2 + w21C 2 eiφ
Vo
e−iφ
Iˆ = q
R2 + w21C 2

Finalmente, Vout es el voltaje entre los extremos de la resistencia
RVo
e−iφ
V̂out = Ẑr Iˆ = RIˆ = q
R2 + w21C 2

Con esto

Vo
V̂out = q
e−iφ
1 + R2 w 2 C 2
Vo
cos(wt − φ)
Vout (t) = Re(V̂out eiwt ) = q
1 + R2 w12 C 2
