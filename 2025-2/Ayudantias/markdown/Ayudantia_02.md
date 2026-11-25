---
title: "Ayudantia 02"
source_enunciado: "Electro/2025-2/Ayudantias/Enunciados/Ayudantia_02_Enunciado.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_02_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 02

## Enunciado

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudantes: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 2
#### Problema 1
Un alambre infinito con densidad lineal de carga λ se dobla en forma de horquilla, como se
muestra en la figura. Determine el campo eléctrico en el punto O.

#### Problema 2
Un recipiente hemisférico no conductor, de radio interior a, tiene una carga total Q repartida
uniformemente en su superficie. Encuentre el campo eléctrico en el centro de curvatura.

---

### Página 2

#### Problema 3
Considere un disco circular de radio a que tiene una densidad de carga superficial uniforme
σ.
a) Calcule el campo eléctrico en un punto sobre el eje del disco a una distancia z.
b) Obtenga, a partir del resultado anterior, el campo creado por un plano infinito con
densidad de carga σ.

---

## Solución

### Página 1

PONTIFICIA UNIVERSIDAD CATÓLICA DE CHILE
Facultad de Física
FIS1533-9 - Electricidad y Magnetismo
Profesora Macarena Domínguez
Ayudantes: Samuel Urrutia (samuel.urrutia@uc.cl)

Ayudantía 2
#### Problema 1
Un alambre infinito con densidad lineal de carga λ se dobla en forma de horquilla, como se
muestra en la figura. Determine el campo eléctrico en el punto O.

#### SOLUCION:
Primero calcularemos el campo eléctrico producido por la semicircunferencia, luego el campo
producido por los dos semiejes y finalmente usaremos el principio de superposición para
calcular el campo total en O. Para calcular cada una de estas tres contribuciones usaremos
la expresión del campo eléctrico producido por una distribución lineal de cargas, es decir,
⃗ r) =
E(⃗

4πϵ0

Z

⃗
⃗r − R
⃗
λ(R)dℓ
⃗ 3
|⃗r − R|

(1)

⃗ denota la densidad lineal de carga, ⃗r es el punto donde deseamos calcular el
en que λ(R)
⃗ recorre los puntos de distribución y dℓ es el elemento de longitud de la línea donde
campo, R
se encuentra la carga.

---

### Página 2

Pondremos el origen del sistema de coordenadas en el punto O, de modo que ⃗r = 0. En
⃗ = Rρ̂ y dℓ = Rdθ. Reemplazando
primer lugar, para la semicircunferencia, tenemos que R
en (1)
Z 3π/2
λ
ρ̂(θ)dθ
E1 (0) = −
4πϵ0 R π/2
Escribimos ρ̂(θ) = cos θ x̂ + sin θ ŷ y resolvemos la integral, obteniendo
⃗ 1 (0) =

λ
x̂
2πϵ0 R

Ahora calcularemos la contribución al campo debido al alambre superior, ubicado en y = R,
⃗ = x x̂+R ŷ y dℓ = dx. Reemplazando
y que se extiende desde x = 0 a x = ∞. En este caso R
en (1)
Z ∞

Z ∞
x
dx
λ
dx
⃗ 2 (0) = −
x̂ + R
ŷ
4πϵ0 0 (x2 + R2 )3/2
(x2 + R2 )3/2
La primera integral es casi directa. Reemplazamos u = x2 + R2 → du = 2x dx
Z
Z ∞
∞
1 ∞ 1
x dx
√
du
−
3/2
3/2
(x + R )
2 R2 u
R
u R2

Para la segunda integral, sustituimos x = R tan(u) → dx = R sec2 (u)du
Z ∞
Z π/2
dx
R sec2 (u)
du
(x2 + R2 )3/2
(R2 tan2 (u) + R2 )3/2
Recordemos que tan2 α + 1 = sec2 α, por lo tanto R2 tan2 u + R2 = R2 sec2 u. Tenemos que
Z π/2
Z π/2
Z π/2
R sec2 (u)
du = 2
= 2
cos(u) = 2
(4)
R sec (u)
R 0
sec(u)
R 0
R
Reemplazando (3) y (4) en (2), obtenemos


λ
E2 (0) = −
x̂ + 2 ŷ
4πϵ0 R
R
El calculo de la contribución de campo producida por el alambre inferior, ubicado en y = −R,
es análoga y resulta en


λ
E3 (0) = −
x̂ − 2 ŷ
4πϵ0 R
R
Finalmente, utilizamos el principio de superposición para obtener el campo eléctrico total
producido por la distribución de carga
⃗ 1 (0) + E
⃗ 2 (0) + E
⃗ 3 (0)
E(0)
=E




λ
λ
E(0)
− −
x̂ +
0 − 2 + 2 ŷ
4πϵ0 R R R
R
R
E(0)
= 0.

---

### Página 3

#### Problema 2
Un recipiente hemisférico no conductor, de radio interior a, tiene una carga total Q repartida
uniformemente en su superficie. Encuentre el campo eléctrico en el centro de curvatura.

Tomamos como origen el centro de curvatura de la semiesfera. A partir de esto, podemos
determinar la contribución de un elemento diferencial de carga en la superficie al campo
eléctrico en el eje que pasa por el centro de curvatura, que coincide con la dirección ẑ (El
⃗ por simetría, solo tendrá componente en ẑ ).
campo E,

⃗ =
dE

1 ⃗r − R
σdS
4πϵ0 |⃗r − R|

donde el elemento diferencial de superficie sobre la esfera está dado por
dS = a2 sin θdθdϕ

y, como la carga está uniformemente distribuida, la densidad superficial es simplemente
Q
2πa2

σ=

Reemplazando (2) y (3) en (1), podemos determinar el campo total integrando sobre toda la
superficie:
⃗ r) = a
E(⃗

Z 2π Z 0
sin θ

−π/2

Q ⃗r − R
dθdϕ
2πa2 |⃗r − R|

(4)

---

### Página 4

→
−
Evaluando en ⃗r = 0 obtenemos el campo en el centro de curvatura:
⃗C = − Q
8π 2 ϵ0

Z 2π Z 0
sin θ
−π/2

R
dθdϕ
|R|

⃗ = aρ̂ = a sin θ cos ϕx̂ + a sin θ sin ϕŷ + a cos θẑ, entonces |R|
⃗ = a. Por el
Si tomamos R
argumento de simetría, solo interesa la componente según ẑ. De todas formas, se puede
verificar calculando explícitamente las integrales en x̂, ŷ. Con esto,
Z 0
Z 0
Q
Q
Q
cos
θ
sin
θdθ
−
sin
2θdθ
EC = −
4πϵ0 a2 −π/2
8πϵ0 a2 −π/2
8πϵ0 a2
|
{z
}
=−1

Finalmente,
⃗ C = EC ẑ =

Q
ẑ
8πϵ0 a2

#### Problema 3
Considere un disco circular de radio a que tiene una densidad de carga superficial uniforme
σ.
a) Calcule el campo eléctrico en un punto sobre el eje del disco a una distancia z.
b) Obtenga, a partir del resultado anterior, el campo creado por un plano infinito con
densidad de carga σ.
a) Para calcular el campo eléctrico producido por el disco en un punto cualquiera de su
eje, consideremos la expresión de campo eléctrico producto de un anillo que se calculó
en la ayudantía anterior,
z
Q
z
aλ
ẑ =
ẑ
E(z)
3/2
2ϵ0 (z + a )
4πϵ0 (z + a2 )3/2

Q
donde se usó λ = Q
= 2πa
. Vamos a considerar el disco como un conjunto de anillos
L
concéntricos, y usaremos el principio de superposición para sumar las aportaciones de
todos ellos. En forma diferencial, tenemos

⃗ =
dE

z
dq ẑ
4πϵ0 (z + r2 )3/2

---

### Página 5

Aquí, r es el radio de cada anillo y dq el elemento de carga de cada uno, es decir
dq = σdS = 2πσrdr

Reemplazamos (3) en (2) e integramos entre 0 y a,
Z a
2r dr
E(z) =
· πσ · z
ẑ
2 3/2
0 (z + r )
Reemplazamos u = z 2 + r2 → du = 2r dr
σz
E(z)
4ϵ0

σz
4ϵ0

Z z2 +a2
z2

du
ẑ
u3/2
!
z +a

−√
u z2

ẑ



σz
− 2
+
ẑ
4ϵ0
(z + a2 )1/2 z


z
σ
1− 2
ẑ
2ϵ0
(z + a2 )1/2
b) Un plano infinito con densidad de carga σ lo podemos considerar como un disco de
radio infinito. Como (z2 +a12 )1/2 → 0 cuando a → ∞, encontramos que el campo eléctrico
es constante, pero cambia su dirección al atravesar el plano cargado en z = 0,
⃗ = σ ẑ.
2ϵ0
