---
title: "Ayudantia 10"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_10_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_10_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 10

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 10
#### Problema 1 (I1 2018-2)
Considere una varilla plastica (aislante) cuya densidad de carga lineal λ0 es constante. La
varilla esta ubicada en el eje x, entre x = 0 y x = L.

a) Determine el valor y unidades del SI de λ0 si la carga total de la varilla es Q.
b) Encuentre el campo eléctrico para cualquier x > L.
c) Suponga ahora que se ubica una carga puntual q0 sobre el eje x en x = 2L.

Se desea mover la carga q0 desde el punto A hasta el punto B por el camino mostrado
en la figura. Calcule el trabajo realizado por el campo eléctrico.

---

### Página 2

#### Problema 2 (I1 2023-1)
Considere un cable coaxial de longitud L, el cual tiene una sección transversal como la mostrada en la figura. Este cable consiste de un alambre macizo de cobre de radio R rodeado por
dos mantos (cascarones) cilíndricos sucesivos concéntricos de material dieléctrico de constantes (permitividad relativa) κ1 y κ2 , respectivamente, y un envoltorio (cascarón) cilíndrico
metálico de radio interior 3R y espesor R/4.
a) Calcule la capacitancia del sistema, considerando que L ≫ R.
b) Si una batería de 12 V es conectada con su polo positivo al conductor macizo y su terminal negativo al conductor exterior, ¿cuál es la carga neta almacenada en el conductor
macizo?
c) ¿Cuál es la energía almacenada en el condensador cuando está completamente cargado?

#### Problema 3 (I1 2020-2)
Se tiene un condensador plano con placas cuadradas de largo a, distancia d entre las placas
y una carga total Q. Calcular la fuerza que se ejerce sobre un material dieléctrico cuando se
encuentra a una distancia x del punto O.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 10
#### Problema 1 (I1 2018-2)
Considere una varilla plastica (aislante) cuya densidad de carga lineal λ0 es constante. La
varilla esta ubicada en el eje x, entre x = 0 y x = L.

a) Determine el valor y unidades del SI de λ0 si la carga total de la varilla es Q.
b) Encuentre el campo eléctrico para cualquier x > L.
c) Suponga ahora que se ubica una carga puntual q0 sobre el eje x en x = 2L.

---

### Página 2

Se desea mover la carga q0 desde el punto A hasta el punto B por el camino mostrado
en la figura. Calcule el trabajo realizado por el campo eléctrico.
#### SOLUCION:
a) La carga total está dada por:
Z L

Z L

λ0 dx = λ0 L

λ(x)dx =

Q=

Por lo tanto:
λ0 =

Q
L

Las unidades de λ0 en el sistema internacional son simplemente C/m
b) Por simetría, el campo eléctrico sobre el eje x es solamente en la dirección +x El campo
eléctrico se calcula de la siguiente forma:
λ0 dx′
(x − x′ )2
Z L
dx′
Ex = kλ0
′ 2
0 (x − x )
dEx = k

L

Ex = kλ0
(x − x′ ) 0


Ex = kλ0
−
x−L x
De esta forma el campo eléctrico es:
⃗ =
E

Q
4πϵ0 L



−
x−L x


x̂

c) El trabajo del campo eléctrico para ir desde el punto A al punto B está dado por:
Z B
WA→B =

⃗ · d⃗l
q0 E

A

Como la fuerza eléctrica es conservativa, el trabajo es independiente del camino y
solamente depende del punto inicial y final. Por lo tanto, se podría tomar una trayectoria
sobre el eje x que va desde x = 2L hasta x = 5L/2

---

### Página 3

En este caso el trabajo es simplemente:
Z 5L/2
WA→B =
2L

Qq0
=
4πϵ0 L

q0 Ex dx
Z 5L/2 
2L

−
x−L x


dx
5L/2

Qq0
=
(ln(x − L) − ln(x))
4πϵ0 L
 
 2L

5L/2 − L
5L/2
Qq0
ln
− ln
=
4πϵ0 L
2L − L
2L
 



Qq0
5L/2 − L
5L/2
=
ln
− ln
4πϵ0 L
2L − L
2L
  
 
Qq0
=
ln
− ln
4πϵ0 L
 
Qq0
ln
WA→B =
4πϵ0 L

---

### Página 4

#### Problema 2 (I1 2023-1)
Considere un cable coaxial de longitud L, el cual tiene una sección transversal como la mostrada en la figura. Este cable consiste de un alambre macizo de cobre de radio R rodeado por
dos mantos (cascarones) cilíndricos sucesivos concéntricos de material dieléctrico de constantes (permitividad relativa) κ1 y κ2 , respectivamente, y un envoltorio (cascarón) cilíndrico
metálico de radio interior 3R y espesor R/4.
a) Calcule la capacitancia del sistema, considerando que L ≫ R.
b) Si una batería de 12 V es conectada con su polo positivo al conductor macizo y su terminal negativo al conductor exterior, ¿cuál es la carga neta almacenada en el conductor
macizo?
c) ¿Cuál es la energía almacenada en el condensador cuando está completamente cargado?

#### SOLUCION:
a) Fijándonos en la configuración que tenemos, podemos notar que esto no es otra cosa
más que dos capacitores en serie, tal como se muestra a continuación

---

### Página 5

De este modo, tenemos que
−1
+
Ceq =
C1 C2
y por lo tanto el problema radica en calcular las capacitancias C1 y C2 .


Para calcular las capacitancias, consideremos el caso de un cable coaxial sin dieléctrico,
que tiene un radio interior Ri y exterior Rf . Por ley de Gauss, el campo electrico entre
ambos radios viene dado por
Z
⃗ · dS
⃗ = qe → E · 2πrL = qe
E
ϵ0
ϵ0
S
q
⃗ =
⇒E
r̂
2πϵ0 Lr
Ahora, el potencial entre los dos electrodos es
Z Rf
⃗ · d⃗r = −
E
∆V = −

Z Rf
q
dr
2πϵ0 L Ri r
Ri
 
q
Rf
⇒ |∆V | =
ln
2πϵ0 L
Ri

y por ultimo la capacitancia es
C=

2πϵ0 L
Q
=
|∆V |
ln(Rf /Ri )

la cual es la capacitancia de un condensador cilíndrico. Para aplicar este resultado a
nuestros condensadores, recordemos que C = κC0 , de modo que
C1 = κ1

2πϵ0 L
,
ln(2)

C2 = κ2

2πϵ0 L
ln(3/2)

De esta manera, la capacitancia del sistema esta dada por
1 ln(3/2)
1 ln(2)
+
=
[κ2 ln(2) + κ1 ln(3/2)]
=
Ceq
κ1 2πϵ0 L κ2 2πϵ0 L
κ1 κ2 2πϵ0 L
κ1 κ2 2πϵ0 L
⇒ Ceq =
κ2 ln(2) + κ1 ln(3/2)
b) Si la batería conecta su polo positivo al conductor macizo, este ultimo queda cargado
positivamente con carga Q+ . Entonces
Q+ = (12 V ) · C = (12 V )

κ1 κ2 2πϵ0 L
κ2 ln(2) + κ1 ln(3/2)

c) La energía almacenada por el condensador después de conectar la batería es, simplemente
(12 V )2
κ1 κ2 2πϵ0 L
U = QV =
κ2 ln(2) + κ1 ln(3/2)

---

### Página 6

#### Problema 3 (I1 2020-2)
Se tiene un condensador plano con placas cuadradas de largo a, distancia d entre las placas
y una carga total Q. Calcular la fuerza que se ejerce sobre un material dieléctrico cuando se
encuentra a una distancia x del punto O.

#### SOLUCION:
La energía potencial asociada a esta configuración es
U (x) =

1 Q2
2 C(x)

Notemos que es función de la posición x, puesto que la capacitancia también lo es. El sistema
se puede ver como dos condensadores en paralelo, uno de ellos con un dieléctrico de constante
κ. Así
ϵ0 a(x + κ[a − x])
ϵ0 ax κϵ0 a(a − x)
+
=
Ceq = C1 + C2 =
d
d
d
Con esto, la energía potencial eléctrica almacenada es
U (x) =

Q2 d
2 ϵ0 a(x + κ[a − x])

Para obtener la fuerza, consideremos que para un sistema aislado a Q = cte la conservación
de energía nos dice que el trabajo que hace el sistema mas la variación de energía del sistema
es cero. O sea, si esta aislado, el trabajo que haga el sistema es a costa de su propia energía.
Entonces
dW + dU = 0
Como dW = F⃗ · d⃗r y dU = ∇U · d⃗r, esto implica que F⃗ = −∇U . Así, la fuerza que se ejerce
sobre el dieléctrico será
Fx x̂ = −

dU
Q2 d
1−κ
x̂ → Fx =
dx
2ϵ0 a (x + κ[a − x])2

Notemos que 1 − κ < 0, lo que significa que la fuerza apunta según −x̂. Esto quiere decir
que la placa dieléctrica es atraída hacia el interior del condensador. En este caso que es
conservativo, la fuerza que hace el sistema es para ir a una configuración de menor energía,
y tira al dieléctrico hacia dentro.
