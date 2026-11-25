---
title: "Ayudantia 13"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_13.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_13_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 13

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 13
Dieléctricos

Resumen
Potencial de un objeto polarizado:
En general al hacer actuar un campo eléctrico externo sobre un material dieléctrico podemos obtener la expresión del potencial generado por un objeto polarizado, el cual es tal que:
ż
ż
⃗1 q
σ
p
r
ρp pr⃗1 q
p
dSpr⃗ q
`
d3 r 1
V p⃗rq “
4πϵ0 S
|⃗r ´ r⃗1 | 4πϵ0 V
|⃗r ´ r⃗1 |
Donde:
σp p⃗xq = P⃗ p⃗xq ¨ n̂p⃗xq
⃗ ¨ P⃗ p⃗xq
ρp p⃗xq = ´∇

Que serian las respectivas densidades de cargas superficial y volumétrica de polarización respectivamente.
Vector desplazamiento y ley de Gauss en dieléctricos
Se define el desplazamiento eléctrico como
⃗ xq “ ϵ0 Ep⃗
⃗ xq ` P⃗ p⃗xq
Dp⃗
Luego la ley de Gauss para dieléctricos en su forma integral y diferencial estaría dada por:
¿
⃗ ¨ dA
⃗ = Qlibre
D
BV

⃗ ¨D
⃗ = ρlibre
∇

---

### Página 2

Dieléctricos lineales
Los dieléctricos que se estudiarán este curso son los llamados dieléctricos lineales, esto debido a
que la polarización y el campo eléctrico están relacionados linealmente tal que:
⃗
P⃗ = χE
donde la cantidad escalar χ se llama susceptibilidad eléctrica del material. Así, una expresión para
⃗ xq en medios lineales seria tal que:
Dp⃗
⃗ xq = pϵ0 ` χqEp⃗
⃗ xq “ ϵEp⃗
⃗ xq
Dp⃗
donde ϵ “ ϵ0 ` χ es la permitividad del material.
Es más conveniente trabajar con una cantidad adimensional, κ, definida por
κ“

ϵ
“ ϵr
ϵ0

Esta constante se llama constante dieléctrica, de manera que
⃗ xq “ ϵEp⃗
⃗ xq “ ϵ0 κEp⃗
⃗ xq
Dp⃗

---

### Página 3

#### Problema 1
Una esfera conductora de radio a está enterrada en el suelo hasta la mitad y se mantiene a potencial
V0 . El aire tiene constante dieléctrica relativa « 1, mientras que el suelo tiene constante dieléctrica
relativa εr , y se puede considerar como un medio semi-infinito limitado por una superficie plana.
a) Calcule el campo eléctrico en todo el espacio. Suponga a priori que dicho campo tiene simetría esférica.
b) Calcule la densidad de carga libre sobre cada hemisferio conductor.
c) Calcule la capacitancia de la esfera con respecto al infinito.

#### Problema 2
Se tienen dos láminas metálicas a y b de ancho despreciable y con carga uniformemente distribuida
Q y ´Q respectivamente. Cada lámina tiene un área A y un largo L que es mucho mayor que
la separación entre las láminas. Entre a y b se encuentra una placa conductora de ancho d a una
distancia h de las placas a y b (ver figura).

Calcule:
⃗ en todo el espacio entre las láminas a y b.
a) El campo eléctrico E

---

### Página 4

b) La diferencia de potencial entre las láminas a y b.
c) La capacitancia del sistema.
Ahora suponga que en lugar de la placa metálica hay un dieléctrico de permitividad ϵ que tiene las
mismas dimensiones que la placa metálica anterior. En el espacio entre las láminas a y b calcule:
⃗
d) El vector de desplazamiento D.
⃗
e) El campo eléctrico E.
f) La capacitancia del sistema.
#### Problema 3
Un capacitor está formado por dos cilindros conductores concéntricos de largo L y radios a y c, respectivamente. El espacio entre los cilindros se llena con dos materiales dieléctricos de permitividad
ϵ1 y ϵ2 como se muestra en la figura (vista superior).

Suponiendo que el capacitor posee una carga `Q en el cilindro interior y ´Q en el cilindro exterior
y despreciando los efectos de borde, determine:
a) El campo eléctrico y el vector de polarización en la región entre los cilindros conductores.
b) La densidad de carga de polarización σ en cada una de las superficies de los materiales
dieléctricos.
c) La capacitancia del sistema.
#### Problema 4
Se llena un condensador de placas paralelas de carga Q (la placa superior con carga positiva y la
inferior con carga negativa) con un dieléctrico inhomogéneo de constante dieléctrica κ(x). El área
de las placas es A y la distancia entre ellas es d. Encuentre una expresión formal general para la
capacidad. ¿Cuánto vale la capacidad cuando el dieléctrico consiste en dos capas, con espesores d1
y d2 y constantes dieléctricas κ1 y κ2 ?

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Solución Ayudantía 13
Dieléctricos

Resumen
Potencial de un objeto polarizado:
En general al hacer actuar un campo eléctrico externo sobre un material dieléctrico podemos obtener la expresión del potencial generado por un objeto polarizado, el cual es tal que:
ż
ż
⃗1 q
σ
p
r
ρp pr⃗1 q
p
dSpr⃗ q
`
d3 r 1
V p⃗rq “
4πϵ0 S
|⃗r ´ r⃗1 | 4πϵ0 V
|⃗r ´ r⃗1 |
Donde:
σp p⃗xq = P⃗ p⃗xq ¨ n̂p⃗xq
⃗ ¨ P⃗ p⃗xq
ρp p⃗xq = ´∇

Que serian las respectivas densidades de cargas superficial y volumétrica de polarización respectivamente.
Vector desplazamiento y ley de Gauss en dieléctricos
Se define el desplazamiento eléctrico como
⃗ xq “ ϵ0 Ep⃗
⃗ xq ` P⃗ p⃗xq
Dp⃗
Luego la ley de Gauss para dieléctricos en su forma integral y diferencial estaría dada por:
¿
⃗ ¨ dA
⃗ = Qlibre
D
BV

⃗ ¨D
⃗ = ρlibre
∇

---

### Página 2

Dieléctricos lineales
Los dieléctricos que se estudiarán este curso son los llamados dieléctricos lineales, esto debido a
que la polarización y el campo eléctrico están relacionados linealmente tal que:
⃗
P⃗ = χE
donde la cantidad escalar χ se llama susceptibilidad eléctrica del material. Así, una expresión para
⃗ xq en medios lineales seria tal que:
Dp⃗
⃗ xq = pϵ0 ` χqEp⃗
⃗ xq “ ϵEp⃗
⃗ xq
Dp⃗
donde ϵ “ ϵ0 ` χ es la permitividad del material.
Es más conveniente trabajar con una cantidad adimensional, κ, definida por
κ“

ϵ
“ ϵr
ϵ0

Esta constante se llama constante dieléctrica, de manera que
⃗ xq “ ϵEp⃗
⃗ xq “ ϵ0 κEp⃗
⃗ xq
Dp⃗

---

### Página 3

#### Problema 1
Una esfera conductora de radio a está enterrada en el suelo hasta la mitad y se mantiene a potencial
V0 . El aire tiene constante dieléctrica relativa « 1, mientras que el suelo tiene constante dieléctrica
relativa εr , y se puede considerar como un medio semi-infinito limitado por una superficie plana.
a) Calcule el campo eléctrico en todo el espacio. Suponga a priori que dicho campo tiene simetría esférica.
b) Calcule la densidad de carga libre sobre cada hemisferio conductor.
c) Calcule la capacitancia de la esfera con respecto al infinito.

a) Primero que nada, para el campo eléctrico dentro de la esfera no hay nada que calcular, es
conductor así que el campo eléctrico es 0.
Para la región fuera de la esfera, debemos utilizar ley de Gauss, pero con un pequeño cambio,
teniendo en consideración que los campos en cada región serán distintos, no podemos usar
una esfera completa como superficie gaussiana, entonces, lo que haremos será utilizar semiesferas cerrados con base circular en nuestra interfaz. ¿Qué haremos con la "base"de esta
esfera? No nos preocupa, el campo eléctrico dentro de nuestro conductor es 0 por lo tanto no
hay flujo y en la región fuera del conductor, en la interfaz, el campo eléctrico debe ser radial,
o sea paralelo a esta base imaginaria, no hay flujo.
Entonces solo basta con calcular el flujo del manto de esta semiesfera utilizando ley de Gauss
para dieléctricos como,
ż
⃗ i ¨ dS
⃗ = Di prq2πr2 = 2πa2 σi , i = 0, 1
D
Esta es una expresión que sirve para ambas regiones, digamos que el aire es i = 0 con ε = ε0
y el suelo es i = 1 con ε = ε1 = ε0 εr . De esta forma, despejando el vector de desplazamiento
y recordando que debe ser radial,
⃗ i (r) = σi a r̂
D
r2
⃗ i = εi E
⃗ i , entonces
Y el campo eléctrico se relaciona con el vector desplazamiento como D
el campo eléctrico es,

---

### Página 4

⃗ i = σi a ,
εi r 2

r>a

b) No conocemos la carga sobre la superficie de la esfera para calcular la densidad directamente, pero conoces el potencial al que está sometido la esfera, entonces,
ża
⃗ ¨ d⃗l
V0 = ´

Especializando para cada región,
ż8
V0 “
a

σi a2
σi a
dr “
εi r
εi

De acá podemos despejar la densidad de carga para cada región como,
σi “

V0 εi
a

c) Finalmente para calcular la capacitancia necesitamos la carga libre de la esfera, ya que
C = VQ , entonces,
Qtotal = 2πa2 σ0 ` 2πa2 σ1 = 2πaV0 pε0 ` ε1 q
Y ya conocemos el potencial de la esfera (V0 ), entonces basta con,
C = 2πapε0 ` ε1 q

#### Problema 2
Se tienen dos láminas metálicas a y b de ancho despreciable y con carga uniformemente distribuida
Q y ´Q respectivamente. Cada lámina tiene un área A y un largo L que es mucho mayor que
la separación entre las láminas. Entre a y b se encuentra una placa conductora de ancho d a una
distancia h de las placas a y b (ver figura).

---

### Página 5

Calcule:
⃗ en todo el espacio entre las láminas a y b.
a) El campo eléctrico E
b) La diferencia de potencial entre las láminas a y b.
c) La capacitancia del sistema.
Ahora suponga que en lugar de la placa metálica hay un dieléctrico de permitividad ϵ que tiene las
mismas dimensiones que la placa metálica anterior. En el espacio entre las láminas a y b calcule:
⃗
d) El vector de desplazamiento D.
⃗
e) El campo eléctrico E.
f) La capacitancia del sistema.
a) Para el primer caso la situación es bastante simple, utilizando una caja como superficie
para ley de Gauss, llegamos al resultados de un campo eléctrico generado por un plano
infinito (L, A " 2h ` d),
⃗ = σ x̂
2ϵ0
Y el campo eléctrico de la región conductora ya lo conocemos también,
⃗ = 0
De esta forma el campo para la región de vacío entre las placas es,
⃗ = σ x̂
ϵ0
b) Con el campo eléctrico ya caracterizado, es fácil calcular la diferencia de potencial entre
las dos placas, simplemente integrando el campo eléctrico,
ż 2h`d

żh
⃗ ¨ d⃗l = ´

∆V = ´

σ
dx ` 0 ´
0 ϵ0

Resolviendo, obtenemos que la diferencia de potencial es,
∆V = ´

2Qh
2hσ
“´
ϵ0
ϵ0 A

c) Y utilizando la definición de capacitancia,
C“

ϵ0 A
“
∆V
2h

ż 2h`d
h`d

σ
dx
ϵ0

---

### Página 6

Ahora el conductor pasa a ser un dieléctrico, en este caso tendremos que aplicar ley de Gauss
en 3 regiones distintas, tomando como referencia la placa izquierda, la primera región entre
x = 0 y x = h, la segunda entre x = h y x = h ` d y la última entra x = h ` d y
x = 2h ` d, pero la forma en que utilizaremos ley de Gauss es la misma, la carga libre que
encierre cualquier superficie Gaussiana será la carga de placa izquierda,
d)
ż
⃗ i ¨ dSi = D ¨ A = Qenc
D
¨AÑD “
A
A
⃗ “ ϵE,
⃗ llegamos a que en la primera y tercera región
De esta forma, utilizando la relación D
σ¨A“

nuestro campo eléctrico es,
⃗ = Q x̂
ϵ0 A
Y en la región dieléctrica es,
⃗ = Q x̂
ϵA
e) Y siguiendo la misma idea anterior, debemos calcular el potencial integrando el campo
eléctrico,
ż 2h`d

żh
⃗ ¨ d⃗l “

∆V = ´

dx `
0 ϵ0 A

ż h`d
h

dx `
ϵA

ż 2h`d
h`d

dx
ϵ0 A

Resolviendo la integral, llegamos a la diferencia de potencial entre ambas placa,
∆V “
A

ˆ

2h d
`
ϵ0
ϵ

˙

f) Utilizando la definición de capacitancia, llegamos a que esta es,
ˆ
C = A

2h d
`
ϵ0
ϵ

˙´1

#### Problema 3
Un capacitor está formado por dos cilindros conductores concéntricos de largo L y radios a y c, respectivamente. El espacio entre los cilindros se llena con dos materiales dieléctricos de permitividad
ϵ1 y ϵ2 como se muestra en la figura (vista superior).

---

### Página 7

Suponiendo que el capacitor posee una carga `Q en el cilindro interior y ´Q en el cilindro exterior
y despreciando los efectos de borde, determine:
a) El campo eléctrico y el vector de polarización en la región entre los cilindros conductores.
b) La densidad de carga de polarización σ en cada una de las superficies de los materiales
dieléctricos.
c) La capacitancia del sistema.
a) La ley de Gauss para el campo eléctrico en presencia de dieléctricos es:
¿
⃗ ¨ dA
⃗ = Qlibre
ε
Consideramos una superficie gaussiana cilíndrica de radio r y longitud L.
Región I: a < r < b
E1 (r) ¨ 2πrL = 

⃗ 1 (r) = 
ñ E
r̂
ε1
2πε1 Lr

Región II: b < r < c
La carga encerrada sigue siendo Q, pero ahora estamos en otro dieléctrico:
⃗ 2 (r) = 

r̂
2πε2 Lr

Región III: r > c
En esta región no hay carga encerrada por la superficie gaussiana (ya que el cilindro exterior
tiene carga total ´Q), por lo tanto:
¿
⃗ ¨ dA
⃗“0ñ E
⃗ 3 (r) = 0 para r > c

---

### Página 8

Ahora, para un dieléctrico lineal, el vector de polarización es:
⃗
P⃗ = pε - ε0 qE
Así, para cada región:
Región I: a < r < b
P⃗1 (r) = pε1 - ε0 q ¨

r̂
2πε1 Lr

P⃗2 (r) = pε2 - ε0 q ¨

r̂
2πε2 Lr

Región II: b < r < c

Región III: r > c
No hay dieléctrico (sólo vacío), así que:
P⃗3 (r) = 0
b) La densidad de carga ligada superficial está dada por:
σlig = P⃗ ¨ n̂
donde n̂ es el vector normal hacia afuera del dieléctrico.
Por lo tanto, para cada material dieléctrico tendremos:
ϵ1 :

pϵ1 ´ ϵ0 q
σinterior = P⃗1 ¨ n̂ = P⃗1 ¨ p´r̂q = -Q
2πϵ1 aL
σexterior = P⃗1 ¨ n̂ = P⃗1 ¨ pr̂q = Q
ϵ2 :

pϵ1 ´ ϵ0 q
2πϵ1 bL

---

### Página 9

σinterior = P⃗2 ¨ n̂ = P⃗2 ¨ p´r̂q = -Q

pϵ2 ´ ϵ0 q
2πϵ2 bL

pϵ2 ´ ϵ0 q
σexterior = P⃗2 ¨ n̂ = P⃗2 ¨ pr̂q = Q
2πϵ2 cL
c) En un capacitor cilíndrico con simetría axial, donde entre los conductores concéntricos
existen dos regiones con distintas permitividades dieléctricas ε1 (de r = a a r = b) y ε2 (de
r = b a r = c), podemos determinar la diferencia de potencial entre los cilindros conductores
integrando el campo eléctrico en dirección radial.
Sabemos que el campo eléctrico en coordenadas cilíndricas para un cilindro cargado con
carga lineal Q es:
2πεLr
Donde L es la longitud del cilindro y ε la permitividad del medio.
La diferencia de potencial se calcula mediante:
E(r) = 

ż0
⃗ ¨ d⃗l

∆V “

Como el campo sólo existe entre los cilindros (r P ra, cs), podemos descomponer la integral
en tres partes, considerando las contribuciones en cada región:
żc

żb

⃗ 2 ¨ d⃗l

⃗ 1 ¨ d⃗l `

∆V “

b

a

Sustituyendo el campo eléctrico en cada región:
żb

∆V “
dr `
a 2πε1 Lr

żc

dr
b 2πε2 Lr

Factorizamos la constante:
∆V “
2πL

ˆ

ε1

żb

dr `
ε2
a r

żc

dr
b r

˙

Evaluando las integrales logarítmicas:
„
ˆ ˙
ȷ
b
1 ´c¯
∆V “
ln
` ln
2πL ε1
a
ε2
b
La capacitancia se define como:
C“

∆V

Por lo tanto:
„

C = 2πL
ln
ε1

ˆ ˙
ȷ´1
b
1 ´c¯
` ln
a
ε2
b

---

### Página 10

#### Problema 4
Se llena un condensador de placas paralelas de carga Q (la placa superior con carga positiva y la
inferior con carga negativa) con un dieléctrico inhomogéneo de constante dieléctrica κ(x). El área
de las placas es A y la distancia entre ellas es d. Encuentre una expresión formal general para la
capacidad. ¿Cuánto vale la capacidad cuando el dieléctrico consiste en dos capas, con espesores d1
y d2 y constantes dieléctricas κ1 y κ2 ?

⃗ = Dpxqx̂ , y que la carga se distriSi despreciamos los efectos de borde, tendremos que D
buye uniformemente en las placas. Sea σ = Q{A. Usando Gauss para dieléctricos:
ĳ
⃗ ¨ d⃗a = qenc,libre
D
D¨A = Q
⃗ = -σx̂
D
⃗ = -σx̂ entre las placas y D
⃗ = 0 fuera de estas. Como D
⃗ = κϵ0 E, el campo eléctrico:
Así, D
⃗ = ´

σ
x̂,
ϵ0 κ(x)

0<x<d

Ahora, tenemos la carga, así que nos falta ∆V para obtener C:
żd
⃗ ¨ d⃗x
∆V = V (d) - V (0) = - E
żd
σ dx
“
0 ϵ0 κ(x)
No tenemos κ(x), así que dejamos la integral expresada. Como σ = Q{A:
C“

σA
“ şd
σ dx
∆V

0 ϵ0 κ(x)

ˆż d
C “ ϵ0 A

dx
0 κ(x)

˙´1

---

### Página 11

En el caso donde el dieléctrico tiene 2 capas, es como si fueran 2 capacitores en serie ya que
el ∆V total se reparte entre ambos:

Por lo tanto, utilizando el resultado anterior:
ˆ
˙´1
C“
`
C1 C2
Con:
ˆż d

˙´1

ˆż d

˙´1

dx
C1 “ ϵ0 A
0 κ1
ϵ0 Aκ1
C1 “
d1
Y análogamente:
dx
C2 “ ϵ0 A
0 κ2
ϵ0 Aκ2
C2 “
d2
Finalmente obtenemos:

˙´1
d1
d2
C“
`
ϵ0 Aκ1 ϵ0 Aκ2
˙´1
ˆ
d1 κ1 ` d2 κ2
C “ ϵ0 A
κ1 κ2
ˆ
˙
κ1 κ2
C “ ϵ0 A
d1 κ1 ` d2 κ2
ˆ
