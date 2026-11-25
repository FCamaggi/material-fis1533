---
title: "Ayudantia 12"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_12.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_12_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 12

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 12
Repaso I1: Ley de Gauss y Potencial

#### Problema 1
Considere una esfera de radio a con densidad de carga ρ = βr3{2 recubierta por un cascarón macizo
y conductor de radio b. Calcule el campo eléctrico en todo el espacio y luego calcule el potencial
eléctrico en el centro de la esfera.

#### Problema 2
Una esfera de metal de radio R y carga q está rodeada por un cascarón esférico de radio interior a
y externo b. El cascarón no tiene carga neta,
Encuentre la densidad de carga superficial en cada superficie.
Encuentre el potencial en el centro de la esfera tomando como referencia que en el infinito el
potencial es 0Si la esfera exterior se conecta a tierra (Se deja a potencial 0) ¿Cómo cambian las respuestas
anteriores?
#### Problema 3
Tres cáscaras esféricas conductoras concéntricas muy delgadas poseen radios a, b y c, respectivamente, siendo a < b < c. Inicialmente, la cáscara interior está descargada, la del medio posee una
carga total negativa ´Q y la externa una carga total positiva Q.

---

### Página 2

a) Encuentre el potencial electrostático en cada una de las cáscaras conductoras.
b) Si las cáscaras interior y exterior son conectadas mediante un alambre conductor muy delgado
que está aislado al pasar por la cáscara central, ¿cuál es ahora el potencial eléctrico de cada
una de las cáscaras? ¿Cuál es la carga en cada una de las esferas?
Propuesto
Dos cables infinitos paralelos al eje X poseen densidad de carga uniforme λ y ´λ. Ellos están a
distancia a del origen.

Encuentre el potencial en un punto arbitrario px, y, xq usando como referencia el origen.
Demuestre que las superficies equipotenciales son cilindros circulares.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 12
Repaso I1: Ley de Gauss y Potencial

#### Problema 1
Considere una esfera de radio a con densidad de carga ρ = βr3{2 recubierta por un cascarón macizo
y conductor de radio b. Calcule el campo eléctrico en todo el espacio y luego calcule el potencial
eléctrico en el centro de la esfera.

#### Solución
Para encontrar el campo eléctrico usamos simetría esférica y la ley de Gauss. La densidad de carga
en la esfera de radio a es
ρ(r) = βr3{2 ,

0ďr<a

La carga encerrada dentro de una superficie gaussiana esférica de radio r < a es

βr

ρ(r ) dτ = 4π

Qenc (r) = 

żr

żr

żr

13{2 12

r dr = 4πβ

Como
żr

r17{2 dr1 = r9{2

resulta
Qenc (r) = 

8πβ 9{2
r

Entonces, por la ley de Gauss,
¿

r17{2 dr1 .

⃗ ¨ dA
⃗ = Qenc (r) .
E
ε0

---

### Página 2

Como el problema tiene simetría esférica,
¿
⃗
E(r)
“ Eprqr̂

⃗ ¨ dA
⃗ = E(r) 4πr2

y por tanto
1 8πβ 9{2
ε0 9

E(r) 4πr2 = 
Despejando,
2β 5{2
⃗
r r̂,
E(r)
“
9ε0

0ďr<a

La carga total de la esfera es
Q“

r7{2 dr “

ρ(r) dτ = 4πβ

8πβ 9{2

En la región conductora a < r < b, el campo debe ser nulo en equilibrio electrostático, de modo
que
⃗
E(r)
“ 0,

a<r<b

Para r > b, la superficie gaussiana encierra toda la carga neta del sistema, que es simplemente Q,
ya que el conductor es neutro y solo redistribuye carga entre sus superficies. Entonces,
E(r) 4πr2 = 

Q
ε0

es decir,
1 Q
1 1
⃗
E(r)
“
r̂
“
4πε0 r2
4πε0 r2

ˆ

˙
8πβ 9{2
r̂

Por lo tanto,
9{2

2βa
⃗
E(r)
“
r̂,
9ε0 r2

r>b

En consecuencia, el campo eléctrico en todo el espacio queda dado por
$
2β 5{2
’
’
r r̂, 0 ď r < a,
’
’
’
’ 9ε0
’
&
⃗
a < r < b,
E(r) = 0,
’
’
’
’
’
2βa9{2
’
’
r̂, r > b.
%
9ε0 r2

---

### Página 3

Ahora calculamos el potencial en el centro usando directamente la definición
ż0
⃗ ¨ d⃗l.

V (0) - V (∞) = ´

Tomando V (∞) = 0, resulta
ż0
⃗ ¨ d⃗l

V (0) = ´

Como el recorrido es radial, podemos escribir d⃗l = dr r̂, y entonces
ż0
E(r) dr

V (0) = ´

Ahora separamos la integral en las distintas regiones del espacio:
E(r) dr

E(r) dr ´

E(r) dr ´

V (0) = ´

ż0

Para r > b,
2βa9{2
9ε0 r2

E(r) = 
mientras que en la región conductora a < r < b,

E(r) = 0,
y para 0 < r < a
E(r) = 

2β 5{2
9ε0

Sustituyendo, obtenemos

2βa9{2
V (0) = ´
dr ´
8 9ε0 r

ż0

2β 5{2
r dr
a 9ε0

0 dr ´

Esto es,
2βa9{2
V (0) = ´
9ε0

dr
2β
´
9ε0
8 r

ż0
r5{2 dr

Calculamos cada integral por separado. Para la primera,
„ ȷb
dr
“ ´
“´
r 8
8 r

---

### Página 4

de modo que

2βa9{2
´
9ε0

dr
2βa9{2
“
´
9ε0
8 r

ˆ

´

˙
“

2βa9{2
9ε0 b

Para la segunda,
ż0

ȷ0
2 7{2
“ - a7{2
dr “
„

5{2

y por tanto
2β
´
9ε0

ż0

5{2

2β
dr = ´
9ε0

ˆ

´ a7{2

˙
“

4β 7{2
63ε0

Sumando ambas contribuciones, obtenemos finalmente
2βa9{2 4βa7{2
V p0q “
`
9ε0 b
63ε0
#### Problema 2
Una esfera de metal de radio R y carga q está rodeada por un cascarón esférico de radio interior a
y externo b. El cascarón no tiene carga neta,
Encuentre la densidad de carga superficial en cada superficie.
Encuentre el potencial en el centro de la esfera tomando como referencia que en el infinito el
potencial es 0Si la esfera exterior se conecta a tierra (Se deja a potencial 0) ¿Cómo cambian las respuestas
anteriores?

#### Solución
Una esfera conductora de radio R con carga total q está en equilibrio electrostático, por lo que toda
su carga se distribuye uniformemente sobre su superficie. Entonces, la densidad de carga superficial
sobre la esfera interior es
σR “

q
4πR2

Ahora consideremos el cascarón conductor de radio interior a y radio exterior b, el cual no tiene
carga neta. Como en el material conductor el campo eléctrico debe ser nulo, si tomamos una superficie gaussiana dentro del espesor del cascarón, la carga encerrada debe ser cero. Como la esfera

---

### Página 5

interior tiene carga q, necesariamente debe inducirse una carga ´q sobre la superficie interna del
cascarón. Como el cascarón en total no tiene carga neta, sobre la superficie externa debe aparecer
una carga `q
Por lo tanto, las densidades de carga superficial en las superficies del cascarón son
σa = ´

q
4πa2

q
4πb2

σb “

Para obtener el potencial en el centro, primero determinamos el campo eléctrico en cada región
usando la ley de Gauss. Para r > b, la carga encerrada es q, ya que el cascarón es globalmente
neutro, luego
⃗
E(r)
“

1 q
r̂
4πε0 r2

Para a < r < b, estamos dentro del material conductor, así que
⃗
E(r)
“0
Para R < r < a, una superficie gaussiana encierra solamente la carga q de la esfera interior, de
modo que
⃗
E(r)
“

1 q
r̂
4πε0 r2

Finalmente, para r < R, estamos dentro de la esfera conductora maciza, luego
⃗
E(r)
“0
Entonces, el potencial en el centro puede obtenerse directamente desde
ż0
⃗ ¨ d⃗l

V (0) - V (∞) = ´

Tomando V (∞) = 0, queda
ż0
⃗ ¨ d⃗l

V (0) = ´

Como el recorrido es radial, escribimos d⃗l = dr r̂, y separamos la integral por regiones

⃗ ¨ d⃗l ´

V (0) = ´

żR
⃗ ¨ d⃗l ´

ż0
⃗ ¨ d⃗l ´

⃗ ¨ d⃗l
R

---

### Página 6

Sustituyendo el campo en cada zona, obtenemos

1 q
V (0) = ´
dr ´
8 4πε0 r

żR

0 dr ´

1 q
dr ´
4πε0 r2

ż0
0 dr
R

Por lo tanto
q
V (0) = ´
4πε0

żR

dr
q
´
4πε0
8 r

dr
r2

Ahora,
„ ȷb
dr
“´
“ ´
r 8
8 r

y
„ ȷR
dr
“
´
“
´
`
r2
r a
R a

żR

Entonces
´

˙

q
´
4πε0

q
V p0q “
4πε0

ˆ

1 1
´ `
R a b

q
V (0) = ´
4πε0

ˆ

ˆ

´ `
R a

˙

de donde resulta
˙

Ahora supongamos que el cascarón exterior se conecta a tierra, es decir, el conductor queda a
potencial cero. La carga inducida sobre la superficie interna debe seguir siendo ´q, porque eso
garantiza que el campo en el material conductor sea nulo. Sea Qb la carga sobre la superficie
externa. Para encontrarla, notamos que fuera del sistema el campo sería
⃗
E(r)
“

1 q ´ q ` Qb
1 Qb
r̂ “
r̂
4πε0
4πε0 r2

Como el cascarón está conectado a tierra, su potencial debe ser cero. Evaluamos entonces el potencial en r = b usando la integral de camino desde el infinito hasta b
⃗ ¨ d⃗l

V (b) - V (∞) = ´

Como V (∞) = 0 y V (b) = 0, se tiene
0 = ´

1 Qb
dr
8 4πε0 r

---

### Página 7

Esto solo es posible si
Qb = 0
Por lo tanto, al conectar a tierra, las cargas quedan distribuidas como
QR = q
Qa = -q
Qb = 0
y las densidades superficiales son
σR “

q
4πR2

σa = ´

q
4πa2

σb = 0
El campo eléctrico en las distintas regiones pasa a ser el siguiente. Para r > b,
⃗
E(r)
“0
Para a < r < b,
⃗
E(r)
“0
Para R < r < a,
⃗
E(r)
“

1 q
r̂
4πε0 r2

Para r < R,
⃗
E(r)
“0
Entonces, el potencial en el centro se obtiene otra vez mediante
ż0
⃗ ¨ d⃗l

V (0) - V (∞) = ´

---

### Página 8

o sea

⃗ ¨ d⃗l ´

V (0) = ´

żR
⃗ ¨ d⃗l ´

⃗ ¨ d⃗l ´

ż0
⃗ ¨ d⃗l

R

1 q
dr ´
4πε0 r2

ż0

Sustituyendo los campos de cada región
żR

0 dr ´

0 dr ´

V (0) = ´

Entonces
q
V (0) = ´
4πε0

żR

dr
r2

Usando
żR

dr
“´ `
R a

queda
q
V (0) = ´
4πε0

ˆ

´ `
R a

q
V p0q “
4πε0

ˆ

´
R a

˙

y por tanto
˙

En resumen, sin conexión a tierra
q
4πR2

σR “

σa = ´
σb “
q
V p0q “
4πε0

q
4πa2

q
4πb2

ˆ

1 1
´ `
R a b

y con el cascarón exterior conectado a tierra
σR “

q
4πR2

˙

0 dr
R

---

### Página 9

σa = ´

q
4πa2

σb = 0
q
V p0q “
4πε0

ˆ

´
R a

˙

#### Problema 3
Tres cáscaras esféricas conductoras concéntricas muy delgadas poseen radios a, b y c, respectivamente, siendo a < b < c. Inicialmente, la cáscara interior está descargada, la del medio posee una
carga total negativa ´Q y la externa una carga total positiva Q.

a) Encuentre el potencial electrostático en cada una de las cáscaras conductoras.
b) Si las cáscaras interior y exterior son conectadas mediante un alambre conductor muy delgado
que está aislado al pasar por la cáscara central, ¿cuál es ahora el potencial eléctrico de cada
una de las cáscaras? ¿Cuál es la carga en cada una de las esferas?

#### Solución
Para calcular el potencial sobre cada cáscara, necesitamos primero el campo eléctrico en todo el
espacio, lo primero a notar es que la primera zona con carga es en r = b es decir, antes de esto
(r < b) la carga encerrada será 0 y, por tanto, el campo eléctrico nulo.
De igual manera, para r > c encerramos tanta carga Q como -Q, por tanto el campo eléctrico
también será 0 fuera de la configuración.
La única región con carga entonces será la región con b < r < c , donde la carga encerrada es Q,
por tanto,

---

### Página 10

$
’
0,
’
’
’
&
Q
⃗
E(r)
“ ´
r̂,
’
4πε0 r2
’
’
’
%0,

r < b,
b < r < c,
r>c.

Ahora vamos a calcular el potencial en cada cascarón, de afuera hacia dentro,
r = c: En este caso el campo eléctrico fuera es 0, por tanto,
żc
0 dr = 0

ϕpcq = ´

r = b: En este caso debemos ya considerar el primer campo eléctrico,

żc
⃗ ¨ d⃗l “

ϕpbq = ´

Q
Q
dr ` ϕpcq “
´
4πε0 r
4πϵ0

ˆ

b´c
bc

˙

r = a: En este caso falta considerar un último tramos donde el campo eléctrico es 0, por lo
tanto,

⃗ ¨ d⃗l “

ϕpaq = ´

Q
0 dr ` ϕpbq “
4πϵ0

ˆ

b´c
bc

˙

Ahora conectamos un cable entre los casquetes en r = c y r = a, esto llevará a una redistribución
de la carga Q de la forma,

a pesar de que la carga se redistribuyó, siempre se debe cumplir que Qa ` Qc = Q, la carga tiene
que conservarse, no se pudo haber ido a otro lado.
Nuevamente las regiones a < r y c < r el campo eléctrico es nulo, no así las otras regiones.
Aplicando la ley de Gauss, como hemos hecho siempre, los campos eléctricos vienen dados por,

---

### Página 11

$
’
0,
r < a,
’
’
’
’
’
’
’
& Qa ,
a<r<b
⃗
E(r)
“ 4πϵ0 r
Qa ´ Q
’
’
’
r̂, b < r < c,
’
’
4πε
’
’
’
%
0,
r>c.
Ahora calculamos los potenciales siguiendo el mismo procedimiento que hicimos antes,
r = c: Nuevamente en este caso no hay campo eléctrico por tanto,
żc
ϕpcq = ´

0 dl = 0

r = b: Aquí ya pasamos por un campo eléctrico que debemos considerar,
⃗ ¨ d⃗l ` ϕpcq “

⃗ ¨ d⃗l “

ϕpbq = ´

żc

żc

Qa ´ Q
dr
b 4πϵ0 r

Lo que da como resultado,
ϕpbq “

Qa ´ Q ` c ´ b ˘
4πϵ0
bc

r = a: Seguimos la misma idea,
⃗ ¨ d⃗l “

ϕpaq = ´

QA
dr ` ϕpbq
a 4πϵ0 r

(1)

lo que lleva a,
ϕpaq “ ϕpbq `

Qa ` c ´ b ˘
4πϵ0 bc

El haber conectado ambas cáscaras mediante un cable fuerza a que el potencial en ambas sea el
mismo. Entonces,
ϕpaq = ϕpcq = 0

(2)

Qa ´ Q ` c ´ b ˘
Qa ` c ´ b ˘
`
“0
4πϵ0
bc
4πϵ0 bc

(3)

Desarrollando,

---

### Página 12

De acá podemos despejar Qa para concluir que,
Qa = Q

apc ´ bq
bpc ´ aq

(4)

Propuesto
Dos cables infinitos paralelos al eje X poseen densidad de carga uniforme λ y ´λ. Ellos están a
distancia a del origen.

Encuentre el potencial en un punto arbitrario px, y, xq usando como referencia el origen.
Demuestre que las superficies equipotenciales son cilindros circulares.
