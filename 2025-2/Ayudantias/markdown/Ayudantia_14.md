---
title: "Ayudantia 14"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_14_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_14_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 14

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 14
#### Problema 1
Tomando R = 1 kΩ y E = 250 V en la figura, determine la dirección y magnitud de la
corriente en el cable horizontal entre los puntos a y e.

#### Problema 2
Seis resistencias forman los lados de un tetraedro. Cinco de los resistores son idénticos (R) y el
sexto es R1 . Se aplica una diferencia de potencial a través de uno de los resistores adyacentes
a R1 . Demuestre que la potencia disipada será máxima cuando R1 = 53 R

---

### Página 2

#### Problema 3
El interruptor que se muestra en la parte a) de la figura se cierra cuando ∆VC > 2∆V /3 y
se abre cuando ∆VC < ∆V /3. El voltímetro lee el voltaje como aparece en la parte b) de la
figura. ¿Cuál es el periodo T de la forma de onda en función de R1 , R2 y C?

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 14
#### Problema 1
Tomando R = 1 kΩ y E = 250 V en la figura, determine la dirección y magnitud de la
corriente en el cable horizontal entre los puntos a y e.

#### SOLUCION:
Definamos las siguientes corrientes:
I1 la corriente que circula por el ∆abc en dicho orden
I2 la corriente que circula por el ∆cde en dicho orden
I3 la corriente que circula por el ∆cea en dicho orden
Utilizando las reglas de Kirchhoff, se cumple que:
ε−I1 R−4R (I1 − I3 ) = 0,

−2RI2 −2ε−3R (I2 − I3 ) = 0,

−4R (I3 − I1 )−3R (I3 − I2 ) = 0

Escribiendo el sistema en forma matricial,


 

5R
−4R
I1
ε
 0
5R −3R   I2  =  −2ε 
−4R −3R 7R
I3

---

### Página 2

Así, I3 viene dada por:

I3 =

5R
ε
5R −2ε
−4R −3R 0
5R
−4R
5R −3R
−4R −3R 7R

=

5R(0 − 6εR) + ε (0 + 20R2 )
−10εR2
ε
=
= −50 mA
=
−
5R (35R2 − 9R2 ) − 4R (0 + 20R2 )
50R3
5R

y con ello sabemos que va en dirección a → e.

#### Problema 2
Seis resistencias forman los lados de un tetraedro. Cinco de los resistores son idénticos (R) y el
sexto es R1 . Se aplica una diferencia de potencial a través de uno de los resistores adyacentes
a R1 . Demuestre que la potencia disipada será máxima cuando R1 = 53 R

Supongamos que circulan corrientes como se muestra en la figura. Aplicando la ley de Kirchoff
en los nodos obtenemos lo siguiente:
i3 + i5 = i6
i = i1 + i2 + i3
i1 = i + i4 + i5
i6 + i2 + i4 = 0

(1)
(2)
(3)
(4)

Como ya sabemos, de estas cuatro ecuaciones solamente tres son linealmente independientes.
Por ejemplo, la condición en el nodo B se obtiene al sumar las demás. Podemos usar tres
cualesquiera según nuestra conveniencia.

---

### Página 3

Aplicando la segunda ley de Kirchoff obtenemos lo siguiente:
malla fuente
malla ABC
malla ABD
malla ACD
malla BCD

Ri1 = V
i3 R1 − Ri5 − Ri1 = 0
i3 R1 − Ri2 + Ri6 = 0
i6 R − Ri4 + Ri5 = 0
i2 R − Ri4 − Ri1 = 0

(5)
(6)
(7)
(8)
(9)

y lo que nos interesa calcular es la potencia disipada en R1 que es P = R1 (i3 )2 . De las cuatro
primeras ecuaciones elegimos usar (1), (2) y (4). De la ecuación (2) calcularemos i ya que
es el único lugar donde aparece. Para encontrar el resto de las corrientes usamos (1), (4),
(5)-(9). De (5) obtenemos i1 = V /R que eliminamos en las otras ecuaciones. Nos queda:
i3 R1 − i5 R − V = 0
i2 R − i4 R − V = 0

(10)
(11)

Las otras ecuaciones no cambian. Usamos (1) para eliminar i5 en términos de i6 e i3 . Nos
queda
(R1 + R) i3 = V + Ri6
2i6 = i4 + i3

(12)
(13)

Sumando (13) con (4) expresamos i2 de i3 e i6 : i2 = i3 − 3i6 . Reemplazamos i2 en (7) y
despejamos i6 en términos de i3 . Resulta i6 = i3 (R − R1 ) /(4R). Finalmente reemplazamos
este valor en (12) y obtenemos i3 que es lo que nos interesaba:
i3 =

4V
5R1 + 3R

La potencia disipada en R1 es:
P = R1 i23 =

16R1 V 2
(5R1 + 3R)2

La pregunta que nos hacen es, ¿para qué resistencia R1 será la potencia disipada máxima?
Para R1 tal que dP/dR1 = 0. Tomando la derivada encontramos:
dP
16V 2
=
(3R − 5R1 )
dR1
(5R1 + 3R)3
que se anula cuando R1 = (3/5)R. La potencia disipada por esta resistencia es Pmáx =
4V 2 /(15R).

---

### Página 4

#### Problema 3
El interruptor que se muestra en la parte a) de la figura se cierra cuando ∆VC > 2∆V /3 y
se abre cuando ∆VC < ∆V /3. El voltímetro lee el voltaje como aparece en la parte b) de la
figura. ¿Cuál es el periodo T de la forma de onda en función de R1 , R2 y C?

Partamos en el punto cuando el voltaje recién ha alcanzado el valor de 23 ∆V y el switch
acaba de cerrarse. Como la corriente circula por el camino con menor resistencia, el cierre del
interruptor produce que la sección donde se ubica el condensador haga cortocircuito, por lo
que comienza a descargarse. El voltaje es 23 ∆V y decae hacia 0 con una constante de tiempo
R2 C :
∆Vc (t) = ∆V e−t/R2 C
Queremos hallar t1 cuando ∆Vc alcanza el valor de 31 ∆V . Así,
∆V = ∆V e−t/R2 C −→ t1 = R2 C ln(2)
Después se abre el switch, el voltaje es 31 ∆V y crecerá hasta ∆Vc con una constante de tiempo
(R1 + R2 ) C :
∆Vc (t) = ∆V − ∆V e−t/(R1 +R2 )C
Ahora, queremos hallar t2 cuando ∆Vc alcanza el valor de 23 ∆V . Así,
∆V = ∆V − ∆V e−t/(R1 +R2 )C

−→

t2 = (R1 + R2 ) C ln(2)

Finalmente,
T = t1 + t2 = (R1 + 2R2 ) C ln(2)
