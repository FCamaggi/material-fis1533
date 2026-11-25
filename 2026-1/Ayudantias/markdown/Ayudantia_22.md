---
title: "Ayudantia 22"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_22.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_22_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 22

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 22
Ley de Biot-Savart

#### Problema 1
Un cable conductor desciende por el eje ŷ desde y = `8 hasta y = 0 y luego continúa por el eje x
hasta x “ `8 (ver figura (a)). Por el cable circula una corriente I. Determine el campo magnético
en el punto P de coordenadas x = y = L.
En la figura (b), una corriente 2I circula por un cable conductor proveniente desde infinito por la
diagonal x = y. Al llegar al origen se divide en dos cables (de corriente I cada uno) que se alejan
hacia infinito por los ejes x e y (ver figura (b)). Determine nuevamente el campo magnético en el
punto P que se encuentra sobre la diagonal.

---

### Página 2

#### Problema 2
Considere la espira de corriente formada por segmentos radiales y arcos de circunferencia como se
⃗ en el punto P .
muestra en la figura. Obtenga el campo magnético B

#### Problema 3
Dos espiras de radios a y b respectivamente, con b < a, están colocadas en forma perpendicular
a un eje común z. Las espiras portan corrientes estables I1 e I2 en distintos sentidos sobre cada
espira, y sus centros están separados una distancia L, tal como se muestra en la figura.
(a) Encuentre una expresión para el campo magnético generado por una espira de radio R a lo
largo del eje z (punto P ).
(b) Encuentre una expresión para el campo magnético resultante de ambas espiras a lo largo del
eje z (punto P ).
(c) Suponga que es posible regular la corriente I2 en la espira de radio b. Encuentre el valor de
I2 para que el campo en z = L{2 sea igual a cero.

---

### Página 3

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 22
Ley de Biot-Savart

#### Problema 1
Un cable conductor desciende por el eje ŷ desde y = `8 hasta y = 0 y luego continúa por el eje x
hasta x “ `8 (ver figura (a)). Por el cable circula una corriente I. Determine el campo magnético
en el punto P de coordenadas x = y = L.
En la figura (b), una corriente 2I circula por un cable conductor proveniente desde infinito por la
diagonal x = y. Al llegar al origen se divide en dos cables (de corriente I cada uno) que se alejan
hacia infinito por los ejes x e y (ver figura (b)). Determine nuevamente el campo magnético en el
punto P que se encuentra sobre la diagonal.

#### Solución

---

### Página 2

Para este problema recordemos la ley de Biot-Savart,
⃗ “ µ0

ż

Id⃗l ˆ p⃗r ´ ⃗r 1 q
|⃗r ´ ⃗r 1 |3

Volvemos a hacer el mismo protocolo que para el cálculo de campos eléctricos, definimos bien cada
vector y el diferencial de camino,

⃗r = Lx̂ ` Lŷ
⃗r 1 = y ŷ
⃗r - ⃗r 1 = pL - yqŷ ` Lx̂
d⃗l = dy ŷ Ñ dy P (8, 0)
Reemplazando en la ley de Biot-Savart,
⃗ “ µ0 I

ż0

dy ŷ ˆ ppL ´ yqŷ ` Lx̂q
ppL ´ yq2 ` L2 q3{2

Utilizando que ŷ ˆ x̂ = ´ẑ y ŷ ˆ ŷ = 0,
ˇ8
ˇ
µ
IL
y
´
L
ˇ
⃗ = 0
a
ˇ ẑ
4π L2 L2 ` pL ´ yq2 ˇ

Resultando en que el campo magnético generado por el alambre que baja por el eje y es,
⃗ “ µ0 I p1 ´ ?1 qẑ
4πL
Ahora toca calcular el segundo campo magnético, pero el cálculo de este campo magnético es
exactamente igual al del caso anterior. Para el módulo es fácil ver que será el mismo, para el signo
podemos simplemente usar la ley de la mano derecha para notar que ambos campos magnéticos se
suman al estar apuntando en la misma dirección, por lo tanto, el campo magnético total en el punto
P viene dado por,
⃗ T = 2B
⃗ “ µ0 I p2 ´
4πL

?
2qẑ

Para la segunda parte, no hay que calcular nada. La corriente que va por el cable en diagonal no
aporta con campo magnético, ya que el vector d⃗l apunta en la misma dirección que ⃗r ´ ⃗r 1 , al haber
un producto cruz en el cálculo del campo magnético, se hace 0.
Para los cables que van en el eje x e y, los módulos son igual al caso anterior, en el caso del cable
que va por el eje x la dirección es exactamente igual que antes, pero el cable del eje y cambió su

---

### Página 3

dirección, ahora estos campos de igual módulo, se anulan.
Por lo que el campo magnético en el segundo caso es 0.

#### Problema 2
Considere la espira de corriente formada por segmentos radiales y arcos de circunferencia como se
⃗ en el punto P .
muestra en la figura. Obtenga el campo magnético B

#### Solución
Hay 3 campos magnéticos que podemos decir que son 0 sin calcular nada, estos son los caminos
radiales ya que los vectores de corriente Id⃗l son paralelos a los vectores de ⃗r ´ ⃗r 1 . Por lo que solo
nos queda calcular los campos generados por los arcos, aunque solo basta con calcular uno ya que
son iguales en estructura, hagamos el segmente 2.
Utilizamos la ley de Biot-Savart,
⃗ “ µ0

ż

⃗ ˆ p⃗r ´ ⃗r 1 q
IdR
|⃗r ´ ⃗r 1 |3

Definimos los parámetros necesarios,

---

### Página 4

⃗r = 0
⃗r 1 = br̂
⃗ = bdθθ̂
dR
⃗ ˆ p⃗r - ⃗r 1 q = b2 dθk̂ Ñ r̂ ˆ θ̂ = k̂
dR

Reemplazando en nuestra integral llegamos a,
⃗ 2 “ µ0 I

żϕ

µ0 ϕI
b2 dθ
k̂ “
k̂
b
4πb

Ahora para calcular el campo magnético generado por el camino 4, el desarrollo será el mismo, con
dos excepciones, la primera es que ⃗r 1 = ar̂ y la segunda es que la corriente ahora es recorrida en
sentido horario, antes fue anti-horario, por lo que cambia el signo del campo magnético. Teniendo
ambas consideraciones, el campo magnético del camino 4 es,
⃗ 4 = - µ0 ϕI k̂
4πa
El campo total es la suma de todas las contribuciones, es decir,
⃗T = 0 ` B
⃗2 ` 0 ` B
⃗ 4 ` 0 “ µϕI

ˆ

1 1
´
b a

˙

#### Problema 3
Dos espiras de radios a y b respectivamente, con b < a, están colocadas en forma perpendicular
a un eje común z. Las espiras portan corrientes estables I1 e I2 en distintos sentidos sobre cada
espira, y sus centros están separados una distancia L, tal como se muestra en la figura.
(a) Encuentre una expresión para el campo magnético generado por una espira de radio R a lo
largo del eje z (punto P ).
(b) Encuentre una expresión para el campo magnético resultante de ambas espiras a lo largo del
eje z (punto P ).
(c) Suponga que es posible regular la corriente I2 en la espira de radio b. Encuentre el valor de
I2 para que el campo en z = L{2 sea igual a cero.

---

### Página 5

#### Solución
Primero nos piden calcular el campo magnético generado por CUALQUIER anillo cuya altura está
a una distancia z0 del origen y midiendo el campo a una distancia z sobre el eje del anillo, es decir,

Para definir Biot-Savart usamos:

⃗r = 0x̂ ` 0ŷ ` z0 ẑ

(1)

⃗r 1 = R cos θx̂ ` R sin θŷ ` z ẑ
d⃗l = Rdθθ̂

(2)
(3)

De esta manera, el campo eléctrico viene dado por la expresión,
⃗ z0 q “ µ0
Bpz,

ż

IRdθθ̂ ˆ rpz ´ z0 qẑ ´ Rr̂s
rpz ´ z0 q2 ` R2 s3{2

(4)

---

### Página 6

Luego de hacer los productos cruz nos quedamos con,
„
ȷ
ż 2π
ż 2π
pz ´ z0 q
R
µ0
⃗
r̂dθ `
dθẑ
Bpz, z0 q “
4π rpz ´ z0 q2 ` R2 s3{2 0
rpz ´ z0 q2 ` R2 s3{2 0

(5)

Ya hemos visto anteriormente porque la primera integral es cero, el vector unitario r̂ NO es fijo,
depende del ángulo: ⃗r = cos θx̂ ` sin θŷ, la integral en dθ es entonces 0. La otra integral es trivial,
con esto obtenemos:
⃗ z0 , R, Iq “
Bpz,

µo IR2
ẑ
2rpz ´ z0 q2 ` R2 s3{2

(6)

Para la segunda parte solo debemos usar el resultado anterior de la forma,
⃗ = Bpz,
⃗ 0q ` Bpz,
⃗ Lq

(7)

Notando que para la primera espira tenemos pz0 , R, Iq Ñ p0, a, I1 q y la segunda pz0 , R, Iq Ñ
pL, b, ´I2 q, por lo tanto, el campo de la configuración del problema es:
µ0
⃗
B(z)
“

˜

I1 a2
I2 b2
´
pz 2 ` a2 q3{2 rpz ´ Lq2 ` b2 s3{2

¸
ẑ

(8)

⃗
Para el último inciso, queremos que la expresión anterior cumpla con BpL{2q
“ 0, esto solo se
logra si I2 sigue la siguiente relación:

I2 = I1

´ a ¯2 „ L2 ` 4b2 ȷ3{2
L2 ` 4a2

b

(9)
