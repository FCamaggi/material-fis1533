---
title: "Ayudantia 05"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_05.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_05_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 05

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 5
Ley de Gauss

Resumen
El flujo eléctrico corresponde a una representación cuantitativa de la cantidad de líneas de campo
que penetran una superficie. La forma de calcularlo es:
ż
⃗ ¨ dA
⃗
ΦE = E
(1)
S

Que en el caso de un campo uniforme y superficies planas, el calculo se reduce a,
⃗ ¨A
⃗ = EA cos(θ)
ΦE = E

(2)

donde θ es el ángulo entre el campo eléctrico y el vector en dirección normal a la superficie.
En el caso de que la superficie a la que se le calcula el campo eléctrico sea una superficie cerrada
(o gaussiana), su flujo eléctrico esta totalmente determinada por la carga encerrada, de la forma:
ż
⃗ ¨ dA
⃗ = qenc
(3)
Φe = E
ε0
s
Esta es la llamada Ley de Gauss. La ley de Gauss es una alternativa a la ley de Coulomb. Aunque
equivale por completo a la ley de Coulomb, la ley de Gauss ofrece una forma distinta de expresar
la relación entre la carga eléctrica y el campo eléctrico.

---

### Página 2

#### Problema 1
Una distribución de carga esférica ρ se extiende desde r = 0 a r = R, con
˙
ˆ
r2
ρ = ρ0 1 - 2
R
a) Calcule la carga total Q que posee la esfera.
b) Calcule el campo eléctrico en todo el espacio.

#### Problema 2
Se tiene un cilindro muy largo de radio R, con una densidad de carga volumétrica ρ. Se ha extraído
otro cilindro de radio R{2, dejando un hueco sin carga en el cilindro grande. El vector que une el
centro del cilindro de radio R con el centro del hueco es ⃗a, como se observa en la siguiente figura:

Obtenga el campo eléctrico en cualquier punto dentro de la cavidad que no pertenezca al eje sobre
el que se encuentra ⃗a.

---

### Página 3

#### Problema 3 [I1 2025-1]
El plano xy (descrito por z = 0) está cubierto de una densidad de carga superficial σ uniforme (es
decir, una placa de espesor infinitesimal). Inmediatamente al lado positivo del eje z hay una placa
también infinita de espesor a con carga eléctrica de densidad volumétrica ρ uniforme en 0 < z < a
(ver figura). Use el teorema de Gauss para calcular el campo eléctrico en todo el espacio.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Solución Ayudantía 5
Ley de Gauss

Resumen
El flujo eléctrico corresponde a una representación cuantitativa de la cantidad de líneas de campo
que penetran una superficie. La forma de calcularlo es:
ż
⃗ ¨ dA
⃗
ΦE = E
(1)
S

Que en el caso de un campo uniforme y superficies planas, el calculo se reduce a,
⃗ ¨A
⃗ = EA cos(θ)
ΦE = E

(2)

donde θ es el ángulo entre el campo eléctrico y el vector en dirección normal a la superficie.
En el caso de que la superficie a la que se le calcula el campo eléctrico sea una superficie cerrada
(o gaussiana), su flujo eléctrico esta totalmente determinada por la carga encerrada, de la forma:
ż
⃗ ¨ dA
⃗ = qenc
(3)
Φe = E
ε0
s
Esta es la llamada Ley de Gauss. La ley de Gauss es una alternativa a la ley de Coulomb. Aunque
equivale por completo a la ley de Coulomb, la ley de Gauss ofrece una forma distinta de expresar
la relación entre la carga eléctrica y el campo eléctrico.

---

### Página 2

#### Problema 1
Una distribución de carga esférica ρ se extiende desde r = 0 a r = R, con
ˆ
˙
r2
ρ = ρ0 1 - 2
R
a) Calcule la carga total Q que posee la esfera.
b) Calcule el campo eléctrico en todo el espacio.

a) En el primer ítem se nos pide encontrar la carga total que posee la esfera, como ya se nos
está entregando la función que describe la densidad de carga dentro de la esfera, basta con
integrar esta en todo el volumen:
˙
¡
¡
żR ˆ
r2
Q“
ρ dV “
ρr drdΩ “
ρ0 1 ´ 2 r dr dΩ
R
˙
żR ˆ
r
“ 4π
ρ0 1 ´ 2 r2 dr
R
Como hay simetría angular en el problema (la densidad de carga no depende de ninguno
de los dos ángulos con los que parametrizamos una esfera, θ y ϕ), la integral angular la
expresamos como la integral sobre el ángulo sólido que ya de memoria sabemos que vale
4π, de todas formas, por si no lo recuerda:
ż 2π ż π
żπ
dΩ “
sin θ dθdϕ = 2π
sin θ dθ = 4π

Así, resolviendo la última integral, obtenemos que la carga neta de la esfera es:
˙
ˆ 3
˙
żRˆ
r2
r
r5 ˇˇR
Q = 4πρ0
1 - 2 r dr = 4πρ0
´
ˇ
R
5R2 0
Q“

8πρ0 R3

---

### Página 3

b) Ahora debemos calcular el campo eléctrico en todo el espacio, para esto utilizaremos Ley
de Gauss en su forma integral:
qenc
E dS “
Claramente tenemos dos casos de interés acá, cuando r < R y cuando r > R. ¿Por qué
tenemos que hacer esta distinción? Debemos entender como utilizaremos Ley de Gauss.
Para el cálculo de la integral, elegimos una superficie gaussiana, en la que aprovechamos la
simetría del problema, en este caso serán esferas. Si estamos dentro de la esfera con carga, y
trazamos distintas esferas gaussianas arbitrarias de radio r, a medida que aumentamos este
r (aún estando dentro de la esfera con carga), nuestra esfera gaussiana va encerrando cada
vez más carga. Viendo ahora el caso en el que estemos afuera de la esfera cargada, para
cualquiera esfera gaussiana de radio r, la carga encerrada siempre será la misma, la carga
total de la esfera, entonces:
r < R:
En este caso debemos calcular la carga que encerrará una esfera gaussiana arbitraria de radio
r, es decir:
¡
qenc “

ρ dV “

żr

ˆ 3
˙
r
r5
dΩ ρr dr = 4πρ0
´
5R2

Con la carga obtenida para cualquier valor de r, con r < R, utilizamos Ley de Gauss:
ˆ
˙
4πρ0 r3
r5
E dS “
´
5R2
ˆ 3
˙
4πρ0 r
r5
E dS “
´
5R2
ˆ 3
˙
4πρ0 r
r5
E ¨ 4πr “
´
5R2
ˆ
˙
ρ0 r
r3
E“
´
ϵ0 3 5R2
Finalmente, sabemos que este campo es radial, por lo tanto:
⃗ r q = ρ0
Ep⃗

ˆ

r
r3
´
3 5R2

˙
r̂ ,

r<R

r>R:
Este caso resulta más sencillo, principalmente porque ya calculamos la carga de toda la
esfera, es fácil notar que cualquier esfera gaussiana que cumpla con r > R (el caso que
estamos viendo) siempre encerrará la misma carga, la de toda la esfera. Entonces:

---

### Página 4

1 8πρ0 R3
E dS “
ϵ0 15
1 8πρ0 R3
E dS “
ϵ0 15
1 8πρ0 R3
E ¨ 4πr2 “
ϵ0 15

Finalmente:

⃗ = 2ρ0 R r̂,
15r2 ϵ0

r>R

#### Problema 2
Se tiene un cilindro muy largo de radio R, con una densidad de carga volumétrica ρ. Se ha extraído
otro cilindro de radio R{2, dejando un hueco sin carga en el cilindro grande. El vector que une el
centro del cilindro de radio R con el centro del hueco es ⃗a, como se observa en la siguiente figura:

Obtenga el campo eléctrico en cualquier punto dentro de la cavidad que no pertenezca al eje sobre
el que se encuentra ⃗a.
Para este problema debemos usar el principio de superposición de una manera muy interesante. En este problema no podemos llegar y utilizar directamente Ley de Gauss por que no
hay una simetría que nos convenga.
Modelaremos esta configuración de otra forma: queremos un cilindro cargado que tiene otro
cilindro dentro sin carga, para esto imaginaremos el cilindro de radio R que ya teníamos,
pero completo, sin ninguna zona sin carga, y vamos a superponer otro cilindro de carga
opuesta en el lugar donde queremos el hueco sin carga.

---

### Página 5

Entonces nuestro problema se reduce a calcular dos campos eléctricos, el generado por el
cilindro de radio R con densidad de carga ρ y el generado por el cilindro de radio R{2 con
carga ´ρ, ambos superpuestos, y queremos saber el campo eléctrico solo dentro de cada
cilindro.
Utilizando Ley de Gauss podemos directamente conocer estos campos eléctricos, para esto
necesitamos calcular la carga encerrada por una superficie gaussiana arbitraria dentro del
cilindro (este cálculo es válido tanto para el cilindro de densidad ρ como de densidad ´ρ):
ż 2π ż L
¡
żr
ρr dr
dϕ
dz = ρπr2 L
qenc “
ρ dV “

Estamos asumiendo un largo L del cilindro, ya veremos después que no esto no importará
para el resultado.
Nos queda entonces aplicar Ley de Gauss directamente para calcular el campo eléctrico:
qenc
E dS “
qenc
E dS “
E ¨ 2πrL = ρπr2 L
ρr
ρ
E“
r̂ “
⃗r
El calculo anterior es válido para ambos cilindros, ahora hay que tener precaución en como
definimos nuestro r, porque estas expresiones de campo eléctrico solo son válidas si r es la
distancia radial a la que uno se encuentra del centro, entonces, además de tener en consideración que las densidad de carga son opuestas, nuestros r serán distintos, digamos entonces
que ⃗r1 corresponde al vector que define el campo eléctrico del cilindro de densidad ρ y ⃗r2 al
de densidad ´ρ. Con la siguiente imagen se entiende mejor:

---

### Página 6

Entonces, tenemos estos dos campos eléctricos:
⃗ = ρ r⃗1 ,

⃗ = -ρ r⃗2

Utilizando el principio de superposición:
⃗ t = ρ p⃗r1 - ⃗r2 q
Y podemos notar a partir de la figura, que ⃗r1 ´ ⃗r2 es equivalente a ⃗a. Así, finalmente:
⃗ t = ρ ⃗a
Es decir, el campo dentro de la cavidad es constante y siempre apunta en la dirección del
vector que une los centros (⃗a), sin importar en que punto dentro de la cavidad esté midiendo
el campo.

#### Problema 3 [I1 2025-1]
El plano xy (descrito por z = 0) está cubierto de una densidad de carga superficial σ uniforme (es
decir, una placa de espesor infinitesimal). Inmediatamente al lado positivo del eje z hay una placa
también infinita de espesor a con carga eléctrica de densidad volumétrica ρ uniforme en 0 < z < a
(ver figura). Use el teorema de Gauss para calcular el campo eléctrico en todo el espacio.

---

### Página 7

No hay suficiente simetría para usar el teorema de Gauss de una sola vez, así que lo aplicamos
en dos etapas y utilizamos superposición.
Primero calculamos el campo producido por el plano z = 0 (ver figura).

La superficie gaussiana inventada es tipo cilindro de largo L y tapas de forma arbitraria con
área A, y ubicado de modo que el plano z = 0 lo corta por la mitad.
La ley de Gauss nos dice que:
¿
⃗ ¨ dA
⃗“Q
S

La simetría del problema nos indica que la dirección del campo eléctrico va según ẑ. En el
⃗ son perpendiculares, por lo que el manto
manto del cilindro el campo eléctrico y el vector dA
⃗ y dA
⃗ tienen la misma dirección por lo que cada
no contribuye a la integral. En las tapas E
tapa contribuye lo mismo. En cada tapa el campo eléctrico no cambia y puede salir fuera de
la integral. La carga encerrada por la superficie gaussiana es Q = σA. La ley de Gauss nos
dice entonces,
¿
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
E ¨ dA “
E ¨ dA `
E ¨ dA `
E ¨ dA = 0 ` 2 E dA
S

m

t1

t2

dA “

2E
t

t

Q
σA
“

ecuación de la cual deducimos que el módulo del campo es E = σ{p2ϵ0 q. Incluyendo la
información de la dirección y de la posición tenemos,

⃗1 “

$ σ
ẑ
’
’
& 2ϵ0

z>0

’
’
% - σ z<0

donde el sub-índice 1 se refiere al campo producido por el plano.
Luego calculamos el campo eléctrico producido por la placa de espesor a fuera de ella. La
superficie gaussiana útil está dibujada en la figura,

---

### Página 8

La superficie gaussiana sigue siendo un cilindro de largo L y tapas de área A. El que estemos
interesados en el campo fuera de la placa significa L > a.
La situación se parece al caso 1: La simetría nos dice que el campo en las dos tapas es igual.
El campo el perpendicular a la placa. La contribución del manto es nula. La contribución de
una tapa es igual a la contribución de la otra. El campo es constante en toda la tapa. Lo que
es diferente es cuanta carga hay dentro de la superficie gaussiana,
¿
⃗ ¨ dA
⃗ = 2EA = Q = ρAa
S

con lo cual deducimos,
⃗ 2f “

$ ρa
ẑ
’
’
& 2ϵ

z>a

’
’
% - ρa z < 0
La ecuación anterior no incluye cuanto vale el campo en el interior de la placa (0 < z < a).
Eso lo calculamos ahora.
Queremos calcular el campo eléctrico que produce la placa, dentro de la placa. Para ello
inventamos una superficie gaussiana como las anteriores, pero con L < a para que las tapas
de la superficie tipo cilindro queden dentro de la placa, como indica la figura.

---

### Página 9

La ley de Gauss es análoga como en los casos anteriores, y nuevamente la diferencia radica
en la carga eléctrica encerrada por la superficie gaussiana. Esta carga es la densidad por el
volumen,
¿
⃗ ¨ dA
⃗ = 2EA = Q = ρAL
S

Entonces, el campo en la tapa externa y en la interna tienen modulo ρL{p2ϵ0 q. En la tapa
externa z = pa ` Lq{2 y en la interna z = pa - Lq{2, con lo cual el campo dentro de la placa
queda,
$
ρp2z ´ aq
’
’
ẑ a{2 < z < a
’
’
&
⃗ 2d “
’
’
ρpa ´ 2zq
’
’
0 < z < a{2
% ´
Juntamos el campo dentro y fuera producido por la placa obteniendo:

⃗2 “

$ ρa
’
ẑ
’
2ε0
’
’
& ρp2z´aq ẑ

2ε0
ρpa´2zq
’
´
ẑ
’
2ε0
’
’
% ρa
´ 2ε0 ẑ

z>a
a{2 < z < a
0 < z < a{2
z<0

⃗1 y E
⃗ 2 ):
Finalmente sumamos (superposición) los campos del plano y de la placa (E

⃗ “

$ σ`ρa
’
ẑ
’
2ε0
’
’
& σ`ρp2z´aq ẑ
2ε0
σ´ρpa´2zq
’
ẑ
’
2ε0
’
’
% σ`ρa
´ 2ε0 ẑ

z>a
a{2 < z < a
0 < z < a{2
z<0
