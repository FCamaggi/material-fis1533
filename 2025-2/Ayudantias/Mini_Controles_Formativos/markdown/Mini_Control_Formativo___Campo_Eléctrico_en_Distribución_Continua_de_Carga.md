---
title: "Mini Control Formativo   Campo Eléctrico en Distribución Continua de Carga"
source_enunciado: "Electro/2025-2/Ayudantias/Mini_Controles_Formativos/Enunciados/Enunciado_Mini_Control_Formativo___Campo_Eléctrico_en_Distribución_Continua_de_Carga.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Mini_Controles_Formativos/Soluciones/Solución_Mini_Control_Formativo___Campo_Eléctrico_en_Distribución_Continua_de_Carga.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Mini Control Formativo   Campo Eléctrico en Distribución Continua de Carga

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Mini Control Formativo
Campo Eléctrico en Distribución Continua de Carga
2° Semestre 2025 - Cuerpo de Ayudantes FIS1533
Ayudante Coordinador: Luis Rivera Ly - luisriveraly@uc.cl

“Ejercicios Teoría Electromagnética ”, 3.2.5, Fabián Cádiz
Un recipiente hemisférico no conductor de radio interior a tiene una carga total Q
repartida uniformemente en su superficie interior. Encuentre el campo eléctrico en el
centro de curvatura.

Figura 1. Esquema sobre el recipiente hemisférico.
a) E(0) = 0
b) E(0) = 4ε0Qπa2 k̂
c) E(0) = 8ε0Qπa2 k̂
d) E(0) = 16εQ
2 k̂
0 πa
e) E(0) = − 16εQ
2 k̂
0 πa

---

### Página 2

“I1 2022-2”, Problema 4, Facultad de Física
Considere una barra de longitud L y densidad de carga lineal no uniforme dada por
λ(x) = λL0 x , ubicada horizontalmente entre x = 0 y x = L, como muestra la figura. Si
l = L/6, ¿Cuál es el valor del campo eléctrico en el punto P = (−l, 0)?
R u du
a
Nota: Puede serle útil que (u+a)
2 = ln (u + a) + u+a + cte.

Figura 2. Esquema sobre la barra.
λ0
a) E(P ) = − 4πε
(ln 6 − 1) x̂
0L
λ0
(ln 4 − 43 ) x̂
b) E(P ) = − 4πε
0L
λ0
c) E(P ) = − 4πε
(ln 5 − 54 ) x̂
0L
λ0
d) E(P ) = − 4πε
(ln 7 − 76 ) x̂
0L
λ0
(ln 3 − 32 ) x̂
e) E(P ) = − 4πε
0L

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Mini Control Formativo
Campo Eléctrico en Distribución Continua de Carga
2° Semestre 2025 - Cuerpo de Ayudantes FIS1533
Ayudante Coordinador: Luis Rivera Ly - luisriveraly@uc.cl

“Ejercicios Teoría Electromagnética ”, 3.2.5, Fabián Cádiz
Un recipiente hemisférico no conductor de radio interior a tiene una carga total Q
repartida uniformemente en su superficie interior. Encuentre el campo eléctrico en el
centro de curvatura.

Figura 1. Esquema sobre el recipiente hemisférico.
a) E(0) = 0
b) E(0) = 4ε0Qπa2 k̂
c) E(0) = 8ε0Qπa2 k̂
d) E(0) = 16εQ
2 k̂
0 πa
e) E(0) = − 16εQ
2 k̂
0 πa

---

### Página 2

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en el centro de curvatura. Como la figura no posee
ninguna simetría apta para la Ley de Gauss, se aplicará la definición de campo eléctrico:
ZZ
E(x) =
σ(x ′ ) ds′
′ |3
4πε0
|x
−
x
S
Se nota que se usa la integral simple en virtud de la naturaleza del problema,
puesto que el cascarón hemisférico vive en dos dimensiones. No se entrega explícitamente
la densidad de carga del cascarón, por lo que se tendrá que utilizar la definición de carga:

ZZ
σ dS

Q=
S

Paso 1: Componentes Campo Eléctrico - r
Desde ahora en adelante, nuestro sistema de referencia será el centro de curvatura y se utilizarán
coordenadas esféricas por la geometría del ejercicio. Se recuerda que el vector r parte en el
origen y se extiende hasta el punto en donde se quiere calcular el campo:
r=0
Como el origen coincide con el punto a calcular el vector es nulo.

Paso 2: Componentes Campo Eléctrico - r ′
Luego, el vector r ′ parte en el origen y recorre todo el cuerpo con carga:
π
r ′ = ar̂, θ ∈ [ , π[, ϕ ∈ [0, 2π[
Donde = a” es el radio de la esfera y = r̂” la componente radial en coordenadas esféricas.

Paso 3: Componentes Campo Eléctrico - r − r ′
Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = −ar̂
Calculando el módulo del vector anterior:

|r − r ′ | = a
Paso 4: Componentes Campo Eléctrico - dq
Considerando que la densidad de carga es superficial y que la única componente constante para
el cascarón es r:
dq(x ′ ) = σ(x ′ ) ds′ = σ · a2 sin θ dθdϕ
Para llegar a lo anterior se utilizó el diferencial de superficie para esféricas,
observando la componente constante y omitiendo el sentido vectorial.

---

### Página 3

Paso 5: Densidad de Carga - σ
No se entrega explícitamente la densidad de carga del cascarón, por lo que se tendrá que utilizar
la definición de carga:
ZZ
σ dS
Q=
S

Por enunciado, la carga contenida en el cascarón es Q.
Como la densidad de carga del cascarón es uniforme,
se puede tratar como una constante y sale de la integral:

ZZ
Q=σ·

dS
S

Utilizando el diferencial de superficie para esféricas y
considerando que la única componente constante para el cascarón es r:

Z 2π Z π

Q=σ·

a2 sin θ dθdϕ

π

Q = σ · 2π · a · (− cos θ)

π
Q = σ · 2π · a · (− cos + cos 0)
Q = σ · 2π · a2
Q
σ=
2πa2

(1)

Paso 6: Campo Eléctrico - E
Finalmente, se utiliza la definición de campo eléctrico considerando los límites de integración
propuestos con anterioridad:
ZZ
E(0) =
σ(x ′ ) ds′
′ 3
4πε0
S |x − x |
Z 2π Z π
−ar̂
=
σ · a2 sin θ dθdϕ
π
4πε0 0
a3
Z 2π Z π
−ar̂ Q
=
· a2 sin θ dθdϕ
π
4πε0 0
a3 2πa2
Z 2π Z π
−Qr̂
=
· sin θ dθdϕ
π
4πε0 0
2πa2
Z 2π Z π
−Q
= 2 2
r̂ · sin θ dθdϕ
π
8π ε0 a 0

Utilizando que r̂ = sin θ cos ϕ x̂ + sin θ sin ϕ ŷ + cos θ ẑ:

−Q
E(0) = 2 2
8π ε0 a

Z 2π Z π
(sin θ cos ϕ x̂ + sin θ sin ϕ ŷ + cos θ ẑ) · sin θ dθdϕ

π

---

### Página 4

Para simplificar los cálculos, y por temas de simetría, se pueden
obviar las integrales asociadas a las componentes x e y. De esta manera:

E(0) =
=

−Q
8π 2 ε0 a2

Z 2π Z π
cos θ ẑ · sin θ dθdϕ
π

−Q
· 2π ·
8π 2 ε0 a2

Z π
sin θ cos θ ẑ dθ
π

Utilizando la identidad trigonométrica sin 2θ = 2 sin θ cos θ se obtiene que:

−Q
E(0) = 2 2 · 2π ·
8π ε0 a

Z π

−Q
= 2 2 · 2π ·
8π ε0 a

Z 2π

π

π

sin 2θ ẑ dθ
sin β ẑ dβ

2π
−Q
ẑ
= 2 2 · 2π · (− cos β)
8π ε0 a
π
−Q
= 2 2 · 2π · (− cos 2π + cos π) ẑ
8π ε0 a
−Q
= 2 2 · 2π · · −2 ẑ
8π ε0 a
Q
ẑ
=
8πε0 a2

(2)

Notar que se realizó un cambio de variable β = 2θ → dβ = 2 dθ.

Nota: Las componentes x̂ y ŷ del campo se puede obviar además por razones
matemáticas. Resolviendo las integrales respectivas:
Z 2π Z π

Z 2π
(sin θ cos ϕ x̂ + sin θ sin ϕ ŷ) · sin θ dθdϕ =

cos ϕ dϕ

π

π

Z 2π

Z π

+

sin ϕ dϕ

=0

Z π

π

sin2 θ dθ x̂
sin2 θ dθ ŷ

---

### Página 5

“I1 2022-2”, Problema 4, Facultad de Física
Considere una barra de longitud L y densidad de carga lineal no uniforme dada por
λ(x) = λL0 x , ubicada horizontalmente entre x = 0 y x = L, como muestra la figura. Si
l = L/6, ¿Cuál es el valor del campo eléctrico en el punto P = (−l, 0)?
R u du
a
Nota: Puede serle útil que (u+a)
2 = ln (u + a) + u+a + cte.

Figura 2. Esquema sobre la barra.
λ0
a) E(P ) = − 4πε
(ln 6 − 1) x̂
0L
λ0
(ln 4 − 43 ) x̂
b) E(P ) = − 4πε
0L
λ0
c) E(P ) = − 4πε
(ln 5 − 54 ) x̂
0L
λ0
d) E(P ) = − 4πε
(ln 7 − 76 ) x̂
0L
λ0
(ln 3 − 32 ) x̂
e) E(P ) = − 4πε
0L

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el campo eléctrico en el punto = P ”. Como la figura no posee ninguna
simetría apta para la Ley de Gauss, se aplicará la definición de campo eléctrico:
Z
E(x) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |3
Se nota que se usa la integral simple en virtud de la naturaleza del problema,
puesto que la barra se puede describir con solo una componente variable en coordenadas cartesianas.

Paso 1: Componentes Campo Eléctrico - r
Desde ahora en adelante, nuestro sistema de referencia será el centro del disco y se utilizarán
coordenadas cartesianas por la geometría del ejercicio. Se recuerda que el vector r parte en el
origen y se extiende hasta el punto en donde se quiere calcular el campo:
r = −lx̂,

---

### Página 6

Paso 2: Componentes Campo Eléctrico - r ′
Luego, el vector r ′ parte en el origen y recorre todo el cuerpo con carga:
r ′ = xx̂,

x ∈ [0, L]

Paso 3: Componentes Campo Eléctrico - r − r ′
Con lo anterior, también se construyen las demás componentes de la integral:
r − r ′ = −lx̂ − xx̂
Calculando el módulo del vector anterior:

|r − r ′ | = l + x
Paso 4: Componentes Campo Eléctrico - dq
Considerando que la densidad de carga es lineal y que la única componente variable para la
barra es x:
dq(x ′ ) = λ(x ′ ) dl′ =

λ0 x
dx
L

Para llegar a lo anterior se utilizó el diferencial de línea para cartesianas,
observando las componentes constantes y omitiendo el sentido vectorial.

Paso 5: Campo Eléctrico - E(P )
Finalmente, se utiliza la definición de campo eléctrico considerando los límites de integración
propuestos con anterioridad:
Z
E(P ) =
λ(x ′ ) dl′
4πε0 L |x − x ′ |3
Z L
−(l + x) x̂ λ0 x
=
dx
4πε0 0
(l + x)3
L
Z L
λ0
x
=−
dx x̂
4πε0 L 0 (l + x)2
Utilizando que

R

a
u du
(u+a)2 = ln (u + a) + u+a + cte:

L
λ0
l
(ln (x + l) +
) x̂
4πε0 L
x+l 0
λ0
l
l
=−
(ln (L + l) +
− ln (0 + l) −
) x̂
4πε0 L
L+l
0+l
λ0
l
=−
(ln (L + l) +
− ln (l) − 1) x̂
4πε0 L
L+l
λ0
L+l
−L
=−
(ln (
)+
) x̂
4πε0 L
l
L+l

E(P ) = −

---

### Página 7

Por último, y como l = L/6, se obtiene que:

λ0
L + L/6
−L
(ln (
)+
) x̂
4πε0 L
L/6
L + L/6
λ0
=−
(ln 7 − ) x̂
4πε0 L

E(P ) = −

(3)
