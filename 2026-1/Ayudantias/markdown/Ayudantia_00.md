---
title: "Ayudantia 00"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_00.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_00_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 00

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 0
Repaso Matemático

Resumen
1. Vectores y operaciones básicas
⃗ y B.
⃗
Vectores: magnitudes con dirección, como E
Suma y resta: componente a componente.

⃗`B
⃗ = pAx ı̂ ` Ay ȷ̂ ` Az k̂q ` pBx ı̂ ` By ȷ̂ ` Bz k̂q
A
“ pAx ` Bx q ı̂ ` pAy ` By q ȷ̂ ` pAz ` Bz q k̂
Producto escalar:
⃗¨B
⃗ = Ax Bx ` Ay By ` Az Bz
A
ş
⃗
Ejemplo: trabajo W = F⃗ ¨ dl.
Producto vectorial:

ı̂
ȷ̂
k̂
⃗ˆB
⃗ = Ax Ay Az
A
Bx By Bz
“ pAy Bz - Az By q ı̂ ` pAz Bx - Ax Bz q ȷ̂ ` pAx By - Ay Bx q k̂
Ejemplo: Torque ⃗τ “ ⃗r ˆ F⃗ .

---

### Página 2

Determinante:

a11 a12 a13
det(A) = a21 a22 a23
a31 a32 a33
“ a11 pa22 a33 - a23 a32 q - a12 pa21 a33 - a23 a31 q ` a13 pa21 a32 - a22 a31 q
2. Coordenadas comunes
Cartesiano: px, y, zq.
Cilíndrico: pρ, ϕ, zq, útil para cables y solenoides.
Esférico: pr, θ, ϕq, útil para cargas puntuales y simetría radial.
Relaciones entre coordenadas:
Coordenadas cilíndricas:
ρ̂ = cos ϕ î ` sin ϕ ĵ
ϕ̂ = - sin ϕ î ` cos ϕ ĵ
ẑ = k̂
Coordenadas esféricas:

r̂ = sin θ cos ϕ î ` sin θ sin ϕ ĵ ` cos θ k̂
θ̂ = cos θ cos ϕ î ` cos θ sin ϕ ĵ - sin θ k̂
ϕ̂ = - sin ϕ î ` cos ϕ ĵ
3. Cálculo diferencial vectorial
Gradiente: En coordenadas cartesianas:
∇f “

Bf
Bf
Bf
ı̂ `
ȷ̂ `
Bx
Bz

Divergencia: En cartesianas:
⃗ = BAx ` BAy ` BAz
∇¨A
Bx
Bz

---

### Página 3

Rotacional: En cartesianas:
⃗“
∇ˆA

ı̂

ȷ̂

B
Bx

B

B
Bz

Ax Ay Az
Laplaciano: Para un escalar f :
∇2 f “

B2f
B2f
B2f
`
`
Bx2
By 2
Bz 2

Integrales de línea, superficie y volumen
1. Integral de línea
Para un campo escalar f p⃗rq:

ż
f p⃗rq ds
C

Para un campo vectorial F⃗ p⃗rq:

ż
F⃗ ¨ d⃗l
C

2. Integral de superficie
Para un campo escalar f p⃗rq sobre una superficie S:
ĳ
f p⃗rq dS
S

Para un campo vectorial F⃗ p⃗rq:

ĳ
F⃗ ¨ dS
S

3. Integral de volumen
Para un campo escalar f p⃗rq:

¡
f p⃗rq dV
V

dV = dx dy dz
Para un campo vectorial F⃗ p⃗rq:

¡
F⃗ dV
V

---

### Página 4

4. Cálculo integral vectorial
Teorema de Gauss:

¿

¡
⃗ dV
p∇ ¨ Aq

⃗ ¨ dS
⃗“
A
V

BV

Teorema de Stokes:

¿

ĳ
⃗ ¨ d⃗l “
A

⃗ ¨ dS
p∇ ˆ Aq
S

BS

Teorema del gradiente:
ż P2

∇f ¨ d⃗l = f (P2 ) - f (P1 )

P1

5. Derivadas parciales y funciones multivariables
Los campos dependen de x, y, z.
x
Ejemplo: BE
significa la variación de Ex al movernos en y manteniendo x, z fijos.

Regla de la cadena para cambios de coordenadas (cilíndrico/esférico).
6. Integrales múltiples
Doble:

ť

Triple:

ţ

S

f dS.
V

f dV .
dVesf = r2 sin θ dr dθ dϕ.

dVcil = ρ dρ dϕ dz,

---

### Página 5

#### Problema 1
Resuelva la siguiente integral:
λ
Ey “
4πϵ0

żL
´L

ydx
px2 ` y 2 q3{2

#### Problema 2
Considere una esfera de radio R, cuya densidad de masa ρ(r) depende únicamente de la distancia
radial r:
$ ´
r¯
’
&ρ0 1 `
R
ˆ
´ r ¯2 ˙
ρ(r) = 
’
%ρ0 2 ´
R

R
0ďr<
R
ďrďR

Calcule la masa total M de la esfera.
#### Problema 3
Dos pequeñas esferas de igual masa m y carga q (desconocida) cuelgan de dos hilos sin masa, sin
carga y de largo l. Cada esfera forma un ángulo θ con el eje vertical, calcule la carga q.

#### Problema 4
La densidad de carga volumétrica de un cilindro infinito es:
ρpρ, ϕ, zq = ρ0 e´ρ{a
Calcula el gradiente de ρ en coordenadas cilíndricas y evalúalo en ρ = a, ϕ = π{4 y z = 0.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Solución Ayudantía 0
Repaso Matemático

Resumen
1. Vectores y operaciones básicas
⃗ y B.
⃗
Vectores: magnitudes con dirección, como E
Suma y resta: componente a componente.

⃗`B
⃗ = pAx ı̂ ` Ay ȷ̂ ` Az k̂q ` pBx ı̂ ` By ȷ̂ ` Bz k̂q
A
“ pAx ` Bx q ı̂ ` pAy ` By q ȷ̂ ` pAz ` Bz q k̂
Producto escalar:
⃗¨B
⃗ = Ax Bx ` Ay By ` Az Bz
A
ş
⃗
Ejemplo: trabajo W = F⃗ ¨ dl.
Producto vectorial:

ı̂
ȷ̂
k̂
⃗ˆB
⃗ = Ax Ay Az
A
Bx By Bz
“ pAy Bz - Az By q ı̂ ` pAz Bx - Ax Bz q ȷ̂ ` pAx By - Ay Bx q k̂
Ejemplo: Torque ⃗τ “ ⃗r ˆ F⃗ .

---

### Página 2

Determinante:

a11 a12 a13
det(A) = a21 a22 a23
a31 a32 a33
“ a11 pa22 a33 - a23 a32 q - a12 pa21 a33 - a23 a31 q ` a13 pa21 a32 - a22 a31 q
2. Coordenadas comunes
Cartesiano: px, y, zq.
Cilíndrico: pρ, ϕ, zq, útil para cables y solenoides.
Esférico: pr, θ, ϕq, útil para cargas puntuales y simetría radial.
Relaciones entre coordenadas:
Coordenadas cilíndricas:
ρ̂ = cos ϕ î ` sin ϕ ĵ
ϕ̂ = - sin ϕ î ` cos ϕ ĵ
ẑ = k̂
Coordenadas esféricas:

r̂ = sin θ cos ϕ î ` sin θ sin ϕ ĵ ` cos θ k̂
θ̂ = cos θ cos ϕ î ` cos θ sin ϕ ĵ - sin θ k̂
ϕ̂ = - sin ϕ î ` cos ϕ ĵ
3. Cálculo diferencial vectorial
Gradiente: En coordenadas cartesianas:
∇f “

Bf
Bf
Bf
ı̂ `
ȷ̂ `
k̂
Bx
By
Bz

Divergencia: En cartesianas:
⃗ = BAx ` BAy ` BAz
∇¨A
Bx
By
Bz

---

### Página 3

Rotacional: En cartesianas:
⃗“
∇ˆA

ı̂

ȷ̂

k̂

B
Bx

B
By

B
Bz

Ax Ay Az
Laplaciano: Para un escalar f :
∇2 f “

B2f
B2f
B2f
`
`
Bx2
By 2
Bz 2

Integrales de línea, superficie y volumen
1. Integral de línea
Para un campo escalar f p⃗rq:

ż
f p⃗rq ds
C

Para un campo vectorial F⃗ p⃗rq:

ż
F⃗ ¨ d⃗l
C

2. Integral de superficie
Para un campo escalar f p⃗rq sobre una superficie S:
ĳ
f p⃗rq dS
S

Para un campo vectorial F⃗ p⃗rq:

ĳ
⃗
F⃗ ¨ dS
S

3. Integral de volumen
Para un campo escalar f p⃗rq:

¡
f p⃗rq dV
V

dV = dx dy dz
Para un campo vectorial F⃗ p⃗rq:

¡
F⃗ dV
V

---

### Página 4

4. Cálculo integral vectorial
Teorema de Gauss:

¿

¡
⃗ dV
p∇ ¨ Aq

⃗ ¨ dS
⃗“
A
V

BV

Teorema de Stokes:

¿

ĳ
⃗ ¨ d⃗l “
A

⃗ ¨ dS
⃗
p∇ ˆ Aq
S

BS

Teorema del gradiente:
ż P2

∇f ¨ d⃗l = f (P2 ) - f (P1 )

P1

5. Derivadas parciales y funciones multivariables
Los campos dependen de x, y, z.
x
Ejemplo: BE
significa la variación de Ex al movernos en y manteniendo x, z fijos.
By

Regla de la cadena para cambios de coordenadas (cilíndrico/esférico).
6. Integrales múltiples
Doble:

ť

Triple:

ţ

S

f dS.
V

f dV .
dVesf = r2 sin θ dr dθ dϕ.

dVcil = ρ dρ dϕ dz,

---

### Página 5

#### Problema 1
Resuelva la siguiente integral:
żL

λ
Ey “
4πϵ0

´L

ydx
px2 ` y 2 q3{2

Ya conocemos las constantes que aparecen fuera de la integral.
Esta es una integral típica que aparece al calcular campos eléctricos, con esto vamos a ir
soltando la mano.
La integral a resolver es,
λ
Ey “
4πε0

żL
´L

y dx
px2 ` y 2 q3{2

Como la función es par en x, podemos simplificar la integral:
żL
y dx
λ
¨2
Ey “
2 3{2
4πε0
0 px ` y q
Usamos la sustitución trigonométrica:
x = y tan θ

dx = y sec2 θ dθ

ñ

x2 ` y 2 = y 2 tan2 θ ` y 2 = y 2 sec2 θ ñ px2 ` y 2 q3{2 = y 3 sec3 θ
Sustituyendo en la integral:
2λ
Ey “
4πε0

ż θ2

λ
y ¨ y sec2 θ dθ
“
y sec θ
2πε0 y
θ1

ż θ2
cos θ dθ
θ1

Donde los límites de integración son:
θ1 = tan´1 (0) = 0,

θ2 = tan´1 pL{yq

Entonces:
` ´1
˘
´1 pL{yq
λ
λ
rsin θstan
“
¨
sin
tan
pL{yq
2πε0 y
2πε0 y
Recordando la identidad trigonométrica:
Ey “

`
˘
L
sin tan´1 pL{yq = a
L2 ` y 2

---

### Página 6

Finalmente, obtenemos:
Ey “

λ
L
λL
a
¨a
“
2πε0 y
L2 ` y 2
2πε0 y L2 ` y 2

#### Problema 2
Considere una esfera de radio R, cuya densidad de masa ρ(r) depende únicamente de la distancia
radial r:
$ ´
r¯
’
&ρ0 1 `
R
ˆ
´ r ¯2 ˙
ρ(r) = 
’
%ρ0 2 ´
R

R
0ďr<
R
ďrďR

Calcule la masa total M de la esfera.
Para obtener la masa total, integramos la densidad sobre todo el volumen de la esfera. Como
la densidad depende solo de la distancia radial r, usamos coordenadas esféricas, donde el
volumen diferencial es:
dV = r2 sin θ drdθdϕ
Este factor r2 sin θ es fundamental: se trata del jacobiano de la transformación desde coordenadas cartesianas a esféricas. Si no se incluye este jacobiano, el resultado de la integral
sería físicamente incorrecto, por favor siempre que calculemos integrales en esféricas, recordemos considerar esto.
Entonces, la masa total es:
ż 2π

ż
M“

ρ(r) dV = 

żπ
dϕ

esfera

żR
ρprqr2 dr

sin θ dθ

Como ρ(r) no depende de θ ni ϕ, las integrales angulares se evalúan de inmediato:
ż 2π

żπ
dϕ = 2π,

żR
sin θ dθ = 2

ñ

ρprqr2 dr

M = 4π

Ahora dividimos la integral según los tramos definidos en ρ(r):
«ż
ff
ˆ
żR
´
´ r ¯2 ˙
R{2
r¯ 2
M = 4π
ρ0 1 `
r dr `
ρ0 2 ´
r2 dr
R
R
R{2

---

### Página 7

Primera integral:
„ 3
ȷR{2
ż R{2
ż R{2 ´
r3
r
r4
R3 R3
11R3
r¯ 2
r ` dr “
r dr “
`
“
`
“
1`
R
R
4R 0
Segunda integral:
żR ˆ
2´
R{2

´ r ¯2 ˙
R

żR ˆ

r4
2r ´ 2
R

˙

r dr “
R{2

ȷR
r5
2r3
´
dr “
5R2 R{2
„

Evaluamos en los extremos:
ˆ

˙
ˆ
˙
2R3
R5
2 1
´
“R
´
“ R3 ¨
5R
3 5
ˆ
ˆ
˙
˙
2pR{2q
pR{2q
R
R
¨
´
“
´
“
R
´
“
R
5R2
12 160
12 160
Entonces:
ˆ
Segunda integral = R

´
15 480

˙
“ R3 ¨

Masa total:
ˆ
M = 4πρ0 R

`
192 4800

˙

M“

“ 4πρ0 R3 ¨

931π
“
ρ0 R3
12000

931π
ρ0 R 3

#### Problema 3
Dos pequeñas esferas de igual masa m y carga q (desconocida) cuelgan de dos hilos sin masa, sin
carga y de largo l. Cada esfera forma un ángulo θ con el eje vertical, calcule la carga q.

---

### Página 8

Para esto, primero recordamos de dinámica cómo descomponemos las fuerzas en un péndulo.
En este caso, utilizando el ángulo θ, obtenemos las siguientes ecuaciones de movimiento,

Fx = T sin θ - Fe = max
Fy = T cos θ - mg = may
Como en nuestro caso las cargas se encuentran en equilibrio dinámico, las aceleraciones
cumplen con ax = ay = 0.
Entonces de la primera ecuación despejamos,
q2
Ñ q 2 = 4πϵ0 T sin θr2
4πϵ0 r2
Necesitamos deshacernos de T , esto lo hacemos viendo la segunda ecuación, donde notamos,
T sin θ = Fe = 

mg
cos θ
Además r tampoco es un dato del problema, pero viendo el dibujo notamos rapidamente que
r = 2l sin θ, de esta forma el resultado final es,
T “

q “ ˘4l sin θ

a
πϵ0 mg tan θ

#### Problema 4
La densidad de carga volumétrica de un cilindro infinito es:
ρpρ, ϕ, zq = ρ0 e´ρ{a
Calcula el gradiente de ρ en coordenadas cilíndricas y evalúalo en ρ = a, ϕ = π{4 y z = 0.

---

### Página 9

El operador gradiente en coordenadas cilíndricas está dado por:
∇ = ρ̂

B
1 B
B
` ϕ̂
` ẑ
Bρ
ρ Bϕ
Bz

Dado que ρpρ, ϕ, zq = ρ0 e´ρ{a , observamos que la función solo depende de la coordenada
radial ρ.
Componente radial:
Bρ
B
“ pρ0 e´ρ{a q
Bρ
Bρ
ˆ ˙
´ρ{a
“ ρ0 e
¨ ´
a
ρ0 ´ρ{a
“´ e
a

(1)
(2)
(3)

Componente azimutal:
1 B
1 Bρ
“
pρ0 e´ρ{a q
ρ Bϕ
ρ Bϕ
“0

(4)
(5)

ya que la función no depende de ϕ.
Componente axial:
Bρ
B
“ pρ0 e´ρ{a q
Bz
Bz
“0

(6)
(7)

ya que la función no depende de z.
Por lo tanto, el gradiente de la densidad de carga es:
∇ρ = ´

ρ0 ´ρ{a
e
ρ̂
a

Evaluando en ρ = a, ϕ = π{4, z = 0:
ˇ
ˇ
∇ρˇ

ρ0 ´a{a
e
ρ̂
a
ρ = a
ρ0
“ - e´1 ρ̂
a
ρ0
“ - ρ̂
ae
“´

Finalmente:
ˇ
ˇ
∇ρˇ

ρ = a,ϕ = π{4,z = 0

“´

ρ0
ρ̂
ae

(8)
(9)
(10)

---

### Página 10

El gradiente apunta radialmente hacia adentro (signo negativo) con magnitud ρae0 . Esto tiene
sentido físico ya que la densidad de carga decrece exponencialmente con el radio, por lo que
el gradiente indica la dirección de mayor crecimiento de la función, que es hacia el centro
del cilindro.
