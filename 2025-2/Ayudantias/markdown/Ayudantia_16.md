---
title: "Ayudantia 16"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_16_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_16_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 16

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 16
#### Problema 1
En t = 0 el interruptor del circuito mostrado abajo se cierra. Obtenga las cargas en los condensadores, y las corrientes que fluyen por las resistencias, si los condensadores inicialmente
estaban descargados.

---

### Página 2

#### Problema 2
Se tiene N baterías, cada una con la misma FEM E y la misma resistencia interna Ri . Ellas
pueden ser conectadas todas en serie o bien todas en paralelo y, en ambos casos, el circuito
es cerrado con una resistencia adicional R. Determine las potencias Pser y Ppar que se disipan
en R en cada uno de los dos casos. Encuentre el valor Rser de R que permite obtener el mayor
valor para Pser y encuentre el valor Rpar de R que permite obtener el mayor valor para Ppar .
Determine en cuál de los dos casos la potencia disipada en R es mayor.

#### Problema 3
En el circuito que se muestra en la figura, ambos condensadores están inicialmente cargados
a 45 V. ¿Después de cuánto tiempo después de cerrar el interruptor S el potencial de ambos
condensadores se reduce a 10 V? Encuentre la corriente en este tiempo.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 16
#### Problema 1
En t = 0 el interruptor del circuito mostrado abajo se cierra. Obtenga las cargas en los condensadores, y las corrientes que fluyen por las resistencias, si los condensadores inicialmente
estaban descargados.

#### SOLUCION:
Supongamos que la corriente circula como muestra la figura de abajo y apliquemos Kirchhoff
a la malla del borde exterior

---

### Página 2

ε − I 1 R1 −

Q1
=0
C1

Mientras que en la malla interior,
ε−

Q2
− I2 R2 = 0
C2

Claramente, la tasa a la que se carga cada condensador es igual a la corriente que pasa por
dicho condensador. Así,
dQ2
dQ1
, I2 =
I1 =
dt
dt
Reemplazando en las ecuaciones,
ε − R1

dQ1 Q1
−
= 0,
dt
C1

ε−

Q2
dQ2
=0
− R2
C2
dt

Resolveremos detalladamente la primera ecuación mediante Separación de variables:
dQ1
ε
Q1
=
−
=
(εC1 − Q1 )
dt
R1 R1 C1
R1 C1

−→

dQ1
dt
=
εC1 − Q1
R1 C1

Así,
t
+A
R1 C1
Tomando la exponencial, y definiendo B = eA , una nueva constante,
ln (εC1 − Q1 ) = −

Q1 (t) = εC1 − Be−t/R1 C1
Como inicialmente el condensador estaba descargado, B = εC1 , y por tanto:

Q1 (t) = εC1 1 − e−t/R1 C1
Para el segundo condensador es un proceso análogo,
Q2 (t) = εC2 1 − e−t/R2 C2
Derivamos para obtener las corrientes,
ε −t/R1 C1
I1 (t) =
e
,
R1

I2 (t) =



ε −t/R2 C2
e
R2

---

### Página 3

#### Problema 2
Se tiene N baterías, cada una con la misma FEM E y la misma resistencia interna Ri . Ellas
pueden ser conectadas todas en serie o bien todas en paralelo y, en ambos casos, el circuito
es cerrado con una resistencia adicional R. Determine las potencias Pser y Ppar que se disipan
en R en cada uno de los dos casos. Encuentre el valor Rser de R que permite obtener el mayor
valor para Pser y encuentre el valor Rpar de R que permite obtener el mayor valor para Ppar .
Determine en cuál de los dos casos la potencia disipada en R es mayor.

En cada caso se puede calcular la potencia disipada por R como
P = RI 2
donde I corresponden a la corriente que pasa por la resistencia R. En el caso en serie, la
corriente es la misma que circula en todo el circuito, luego por Kirchhoff se tendrá que
N E − N Ri I − RI = 0
NE
⇒I=
N Ri + R

2
NE
⇒ Pser = R
N Ri + R
Por otro lado, en la conexión en paralelo por las N fuentes debe salir la misma corriente.
Entonces, si por cada batería sale una corriente I/N por la resistencia pasará una corriente

---

### Página 4

I. Por Kirchhoff nuevamente
I
− RI = 0
N
NE
⇒I=
Ri + N R
2

NE
⇒ Ppar = R
Ri + N R
E − Ri

Para hallar los Rser y Rpar que maximizan la potencia hay que derivar e igualar a cero. En
el caso en serie
dPser
(N E)2 (N Ri + R) (N Ri − R)
=
=0
dR
(N Ri + R)4
Despejando R, obtenemos
Rser = N Ri
Ahora para el caso en paralelo,
dPpar
(N E)2 (Ri + N R) (Ri − N R)
=0
=
dR
(Ri + N R)4
donde se obtiene
Rpar =

Ri
N

Al evaluar las potencias en sus respectivas resistencias, se obtiene que
Pser (Rser ) = Ppar (Rpar ) =

N E2
4Ri

Por lo que en ambos casos la potencia disipada es la misma.

---

### Página 5

#### Problema 3
En el circuito que se muestra en la figura, ambos condensadores están inicialmente cargados
a 45 V. ¿Después de cuánto tiempo después de cerrar el interruptor S el potencial de ambos
condensadores se reduce a 10 V? Encuentre la corriente en este tiempo.

Los condensadores, que están en paralelo, se descargaran de forma exponencial mediante
las resistencias. Como V es proporcional a Q, entonces V debe obedecer la misma ecuación
exponencial que Q:
V = V0 e−t/RC
Para encontrar el tiempo que toma el voltaje para llegar a 10 V, despejamos de la ecuación
de voltaje
 
V
t = −RC ln
V0
En el circuito ambas resistencias están en serie, por lo que Req = 80 Ω, y los condensadores
en paralelo entregan Ceq = 35 µF. Reemplazando
 
t = −(80 Ω)(35 µF) ln
= 4210 µs = 4,21 ms
Para la corriente, sabemos que V = IR de la ley de Ohm, entonces
I=

V0 −t/RC
e
R

Reemplazando el tiempo que encontramos y los demás valores, se obtiene
I = 0,125 A
