---
title: "Ayudantia 28"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_28_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_28_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 28

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 28
#### Problema 1
En la figura, el interruptor se cierra en t < 0 y se establece una condición de estado estable.
El interruptor se abre después en t = 0.

a) ¿Cuál es la energía almacenada en la bobina justo antes de abrir el interruptor?
b) Encuentre la diferencia de potencial en la bobina justo después de abrir el interruptor
¿Cuál extremo de la bobina está a mayor potencial, a o b?
c) Realice gráficas a mano de las corrientes en las resistencias, como funciones del tiempo.
d) ¿Cuánto tiempo después de t = 0 la corriente en R2 es i?

---

### Página 2

#### Problema 2
En el circuito de la figura, ni la batería ni los inductores tienen una resistencia apreciable,
los condensadores están inicialmente descargados y el interruptor S ha estado en la posición
1 durante mucho tiempo.
a) ¿Cuál es la corriente en el circuito?
b) De repente, el interruptor se coloca en la posición 2. Encontrar la carga máxima que
recibirá cada condensador y el tiempo que tardarán en adquirirla después de accionar
el interruptor.

#### Problema 3
Considere el circuito de la figura

Determine la corriente por cada resistencia:
a) Inmediatamente después de cerrar el interruptor.

---

### Página 3

b) Después que ha pasado mucho tiempo de cerrado el interruptor.
c) Suponga que el interruptor es reabierto después que ha estado mucho tiempo cerrado,
encuentre nuevamente las corrientes:
i. Inmediatamente después que es abierto.
ii. Después de un largo tiempo.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 28
#### Problema 1
En la figura, el interruptor se cierra en t < 0 y se establece una condición de estado estable.
El interruptor se abre después en t = 0.

a) ¿Cuál es la energía almacenada en la bobina justo antes de abrir el interruptor?
b) Encuentre la diferencia de potencial en la bobina justo después de abrir el interruptor
¿Cuál extremo de la bobina está a mayor potencial, a o b?
c) Realice gráficas a mano de las corrientes en las resistencias, como funciones del tiempo.
d) ¿Cuánto tiempo después de t = 0 la corriente en R2 es i?
#### SOLUCION:
a) Cuando se ha alcanzado un equilibrio estable, la corriente en un circuito LR ya no
varía en el tiempo, y por ende ya no hay diferencia de potencial entre los extremos del
inductor. Decimos en ese caso que el inductor se comporta como un cortocircuito y el
circuito de la figura es simplemente una pila con dos resistencias. Suponiendo que la

---

### Página 2

corriente circula en sentido horario en la malla derecha, y anti-horario en la izquierda,
la ley de las mallas -aplicada a la malla derecha- implica que:
ε − I1 R1 = 0
en donde I1 es la corriente que pasa por R1 . Esta es la misma corriente que pasa por el
inductor, IL = ε/R1 . La energía en el inductor es, entonces,
UL =

Lε2
LIL 2
=
2R1 2

b) Justo después de cambiar el estado del circuito abriendo el interruptor, la corriente
a través del inductor es la misma que justo antes, pues el inductor se opone a los
cambios en la corriente circulante. Esta es, por ende, la corriente que circula en toda la
malla exterior. Note que la corriente en R2 se ha invertido. La ley de mallas nos indica
entonces que, en t = 0+ ,



εL 0+ − I 0+ R1 − I 0+ R2 = 0
con I (0+ ) = ε/R1 . Despejando la diferencia de potencial,
 R1 + R2
ε
εL 0+ =
R1
y como la corriente circula en sentido horario -en la malla externa-, el potencial en b es
mayor que en a.
c) Para un instante t > 0, la ley de las mallas nos dice que
εL − I (R1 + R2 ) = 0
˙ por Lenz. La ecuación queda
en donde εL = −LI,
R
I˙ + I = 0
L

−→

(D + α)I = 0

con α = R/L y R = R1 + R2 . Usando el Método del operador diferencial aprendido en
el curso de Ecuaciones Diferenciales,
I(t) = Ke−αt
Reemplazando I(0) = ε/R1 ,

ε −αt
e
R1
Este resultado era el esperado: en ausencia de una fem externa, la corriente decae
exponencialmente en un circuito LR. Toda la energía almacenada en el inductor es
disipada por la resistencia. Esta corriente es la misma que circula en ambas resistencias.
Un bosquejo de ambas corrientes es parecido al que aparece a continuación. Los números
corresponden a ε = 18 V, R1 = 2 kΩ, R2 = 6 kΩ y L = 0,4 H.
I(t) =

---

### Página 3

Note que, en R2 , la corriente se vuelve negativa. Esto es porque el sentido se ha invertido
respecto de su sentido original.
d) Sea t∗ el instante en el cual la corriente vale i. Matemáticamente, I (t∗ ) = i. Reemplazando en la ecuación de la corriente, podemos despejar el tiempo en función de la
corriente deseada,
i = I (t∗ ) =

ε −αt∗
e
R1

−→

iR1
∗
= e−αt
ε

Tomando logaritmo y despejando el tiempo,




ε
iR1
L
∗
t = − ln
ln
=
α
ε
R1 + R2
iR1

#### Problema 2
En el circuito de la figura, ni la batería ni los inductores tienen una resistencia apreciable,
los condensadores están inicialmente descargados y el interruptor S ha estado en la posición
1 durante mucho tiempo.
a) ¿Cuál es la corriente en el circuito?
b) De repente, el interruptor se coloca en la posición 2. Encontrar la carga máxima que
recibirá cada condensador y el tiempo que tardarán en adquirirla después de accionar
el interruptor.

---

### Página 4

#### SOLUCION:
a) En estado estacionario con el interruptor en posición 1, no fluye corriente a los condensadores y los inductores pueden sustituirse por cables. Por lo tanto
i=

ε
75 V
=
= 0,6 A
R
125 Ω

b) Una vez el interruptor se encuentra en la posición 2, el problema puede reducirse calculando las capacitancias e inductancias equivalentes del circuito
=
+
−→ Ceq = 14,6 µF
Ceq
25 µF 35 µF
Leq = 15 mH + 5 mH = 20 mH
Para obtener la carga máxima, consideremos conservación de energía
q2
= Li20
2C
Resolviendo por q, obtenemos
√
q = i0 LC = 3,24 × 10−4 C
Ahora, con el interruptor en la posición 2, el circuito equivalente toma la forma de un
circuito LC, cuya corriente oscila en el tiempo de la forma
q = Q cos(ωt + ϕ) = Q cos(ωt − π/2)
con ϕ = −π/2 ya
pque los condensadores están en un principio descargados para después
cargarse y ω = 1/LC.
Notemos que esta función tiene su máximo cuando t = T /4, por lo tanto
1 2π
π√
t= T =
=
LC = 8,49 × 10−4 s
4 ω

---

### Página 5

#### Problema 3
Considere el circuito de la figura

Determine la corriente por cada resistencia:
a) Inmediatamente después de cerrar el interruptor.
b) Después que ha pasado mucho tiempo de cerrado el interruptor.
c) Suponga que el interruptor es reabierto después que ha estado mucho tiempo cerrado,
encuentre nuevamente las corrientes:
i. Inmediatamente después que es abierto.
ii. Después de un largo tiempo.
#### SOLUCION:
a) Inmediatamente después de que el interruptor es cerrado, la corriente a través de la
inductancia es cero ya que la fem autoinducida evita que la corriente crezca abruptamente. Así, I3 = 0.
Debido a que I1 = I2 + I3 , se tiene que I1 = I2 . Utilizando las reglas de Kirchhoff,
ϵ − I1 R1 − I1 R2 = 0
ϵ
⇒ I1 = I2 =
R1 + R2
b) Después de un largo tiempo, no hay fem autoinducida en la inductancia y las corrientes
pasan a ser constantes. Para la malla inferior, se tiene ahora
ϵ − I1 R1 − I2 R2 = 0

---

### Página 6

y para la malla superior,
I3 R3 − I2 R2 = 0
por último, por regla de nodos, I1 = I2 + I3 . Resolviendo, se obtiene
ϵ(R2 + R3 )
R1 R2 + R1 R3 + R2 R3
ϵR3
I2 =
R1 R2 + R1 R3 + R2 R3
ϵR2
I3 =
R1 R2 + R1 R3 + R2 R3

I1 =

c)

i. Inmediatamente después de que el interruptor es abierto nuevamente, la corriente
a través de R1 es 0. Esto implica que I2 + I3 = 0. La malla superior ahora forma
un circuito RL que decae e I3 tiende a mantenerse en el tiempo. Así
I3 = −I2 =

ϵR2
R1 R2 + R1 R3 + R2 R3

ii. Despues de mucho tiempo, toda la energía se disipa, por lo que
I1 = I2 = I3 = 0
