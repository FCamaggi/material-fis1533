---
title: "Ayudantia 20"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_20_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_20_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 20

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 20
#### Problema 1
Un alambre largo se dobla en la forma de horquilla, como se muestra en la figura. Encuentre
la expresión exacta para el campo magnético en el punto P que se encuentra en el centro del
semicírculo.

---

### Página 2

#### Problema 2
Un cable de radio R lleva una densidad de corriente J⃗ = J0 ẑ. El cable tiene un hoyo cilíndrico
de radio α paralelo al eje del cable, a una distancia b de él. Muestre que el campo magnético
dentro de la cavidad es uniforme.

#### Problema 3
Considere una columna de corriente eléctrica que pasa a través de un plasma. Los filamentos
de corriente en el interior se atraen magnéticamente y se pueden apretar para crear una densidad de corriente muy grande en una región pequeña. así como un intenso campo magnético. A
veces la corriente puede ser interrumpida momentáneamente gracias a este efecto de constricción. Este efecto se puede demostrar haciendo que un recipiente de aluminio vacío conduzca
una corriente grande paralela a su eje. Suponga que R representa el radio del recipiente e I
la corriente hacia arriba, uniformemente distribuida en toda su pared curva. Determine
a) El campo magnético justo en el interior de la pared.
b) El campo magnético justo en el exterior de la pared.
c) La presión sobre la pared.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudante: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 20
#### Problema 1
Un alambre largo se dobla en la forma de horquilla, como se muestra en la figura. Encuentre
la expresión exacta para el campo magnético en el punto P que se encuentra en el centro del
semicírculo.

#### SOLUCION:
Usando el principio de superposición calculamos el campo magnético como la suma de las
contribuciones debidas a los dos alambres seminfinitos y al semicírculo de radio a. Por la ley
de Biot-Savart, los campos magnéticos producidos por estas tres fuentes son perpendiculares
a la hoja y entrando a ésta. Elijamos coordenadas cartesianas con origen en el punto P , con
el eje x paralelo a los alambres, eje y perpendicular a éstos, y eje z saliendo de la hoja. Por la
ley de Biot-Savart, el campo magnético producido por el alambre seminfinito de arriba está
dado por
Z ⃗
⃗
µ0 I
dR × (⃗0 − R)
⃗
B1 (0) =
(1)
⃗ 3
4π
|R|

---

### Página 2

⃗ = (r ŷ + x x̂) y x varía entre 0 e infinito. Entonces |R|
⃗ 3 = (r2 + x2 )3/2 , dR
⃗ = dx x̂
en que R
⃗ × (−R)
⃗ = −rdx ẑ. Reemplazando estas cantidades obtenemos,
y dR
Z
rdx
µ0 I ∞
ẑ
B1 (0) = −
4π 0 (r2 + x2 )3/2
Usando el reemplazo trigonométrico x = r tan α, podemos escribir la ecuación anterior de la
forma
Z
µ0 I π/2
B1 (0) = −
cos α dα ẑ = −
ẑ
4πr 0
4πr
⃗ 3 (0), es exactamente igual a B
⃗ 1 (0). Finalmente, el
La contribución del alambre inferior, B
⃗ 2 (0), está dado por el lado derecho de
campo producido por el semicírculo en el punto P , B
la ecuación (1), pero esta vez con R = r(− cos θx̂ + sin θŷ) y θ varía entre −π/2
 y +π/2.2 Así,
dR = r(sin θx̂ + cos θŷ)dθ, de modo que dR × (−R) = −r sin θ + cos θ dθẑ = −r dθẑ.
Obviamente |R| = r. Reemplazando en el lado derecho de (1) obtenemos,
⃗ 2 (0) = − µ0 I
4πr

Z π/2
dθẑ = −
−π/2

ẑ
4r

Sumando las contribuciones de los dos alambres rectos y del semicírculo (i.e., las expresiones
⃗ 1 (0), B
⃗ 2 (0) y B
⃗ 3 (0)) obtenemos finalmente,
para B


µ
+
ẑ
B(0)
=−
2r π 2

#### Problema 2
Un cable de radio R lleva una densidad de corriente J⃗ = J0 ẑ. El cable tiene un hoyo cilíndrico
de radio α paralelo al eje del cable, a una distancia b de él. Muestre que el campo magnético
dentro de la cavidad es uniforme.

---

### Página 3

Resolveremos el problema por superposición de dos corrientes, una del cilindro completo con
densidad de corriente J0 ẑ, y otra en la cavidad con densidad −J0 ẑ. El campo magnético al
interior de un cable se puede obtener mediante Ley de Ampere, por lo que consideremos
una curva circular de radio r, y dada la simetría cilíndrica de la distribución de corriente, el
campo magnético es constante y tangente sobre la curva. Así
Z
⃗ · d⃗r = B(r)2πr = µ0 J⃗ · dS
⃗ = µ0 J0 πr2
S

µ0 J0 r
θ̂
⇒ B(r)
=
Consideremos ahora un punto arbitrario P al interior de la cavidad

donde el vector r⃗1 va desde el centro del cable al punto P , tal que r⃗1 = r1 ρˆ1 , y r⃗2 va desde
el centro de la cavidad al punto P , de modo que r⃗2 = r2 ρˆ2 .
Por principio de superposición, es claro que el campo magnético en P es
⃗ ) = µ0 J0 r1 θ̂1 − µ0 J0 r2 θ̂2
B(P
pero podemos escribir nuestras direcciones polares como
θ̂1 = ẑ × ρ̂1 ,

θ̂2 = ẑ × ρ̂2

Reemplazando esto,
⃗ ) = µ0 J0 (r1 ẑ × ρ̂1 − r2 ẑ × ρ̂2 )
B(P
µ0 J0
=
(ẑ × r1 ρ̂1 − ẑ × r2 ρ̂2 )
µ0 J0
=
(ẑ × ⃗r1 − ẑ × ⃗r2 )
µ0 J0
=
ẑ × (⃗r1 − ⃗r2 )

---

### Página 4

A partir del dibujo, notemos que ⃗r1 − ⃗r2 = ⃗b, el cual es el vector que va desde el centro del
cable al centro de la cavidad. De este modo
⃗ ) = µ0 J0 ẑ × ⃗b
B(P
Esto es un campo uniforme.

#### Problema 3
Considere una columna de corriente eléctrica que pasa a través de un plasma. Los filamentos
de corriente en el interior se atraen magnéticamente y se pueden apretar para crear una densidad de corriente muy grande en una región pequeña. así como un intenso campo magnético. A
veces la corriente puede ser interrumpida momentáneamente gracias a este efecto de constricción. Este efecto se puede demostrar haciendo que un recipiente de aluminio vacío conduzca
una corriente grande paralela a su eje. Suponga que R representa el radio del recipiente e I
la corriente hacia arriba, uniformemente distribuida en toda su pared curva. Determine
a) El campo magnético justo en el interior de la pared.
b) El campo magnético justo en el exterior de la pared.
c) La presión sobre la pared.
a) Partamos de la Ley de Ampere

⃗ · d⃗s = µ0 Ie

Consideremos un circulo de radio r ligeramente menor a R. Ya que no encierra ninguna
corriente, tenemos que
B(2πr) = 0 −→ B = 0
b) Ahora, si consideramos que r es ligeramente más grande que R, por Ley de Ampere se
obtiene
B=
2πR
y utilizando la regla de la mano derecha, encontramos que la dirección es en sentido
antihorario tangente a la superficie del cilindro.
c) Consideremos una tira de la pared de anchura dx y longitud ℓ. Su anchura es tan
pequeña comparada con 2πR que el campo en su posición sería esencialmente el mismo
si la corriente en la tira se apagara. La corriente que lleva esta tira es
Is =

Idx
hacia arriba
2πR

---

### Página 5

La fuerza en este elemento es, entonces


µ0 I 2 ℓdx
Idx
ℓ
(arriba × dentro) =
F = Is ℓ × B =
radialmente hacia dentro
2πR
2πR
4π 2 R2
Finalmente, la presión sobre la tira y todo el cilindrio es
P =

µ0 I 2 ℓdx
µ0 I 2
F
= 2 2
=
hacia dentro
A
4π R ℓdx
(2πR)2
