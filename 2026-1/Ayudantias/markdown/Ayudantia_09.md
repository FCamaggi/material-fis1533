---
title: "Ayudantia 09"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_09.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_09_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 09

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 9
Potencial Eléctrico: Parte 2

Resumen
El potencial eléctrico V corresponde a la energía electrostática por unidad de carga, y se define
como:
U
V “
q
A partir de esto, podemos definir la diferencia de potencial ∆V como el trabajo por unidad de carga
para mover a una carga desde un punto A a otro punto B:
żB
⃗ ¨ d⃗l
∆V = ´
E
A

Al igual que para la energía potencial electrostática, podemos tomar como referencia el infinito tal
que V (∞) = 0, y así tendremos que para una carga Q el potencial es,
V = k

Q
r

donde r es la distancia entre la carga y el punto en donde se quiere medir el potencial. Así, al
considerar un sistema de N cargas puntuales tendremos que:
ÿ qi
V = k
r
i
Además, podemos obtener el campo eléctrico a partir del potencial según:
⃗ = ´∇V
E
Para una distribución continua de cargas, tendremos que:
ż
dq
V = k
|⃗r ´ ⃗r 1 |

---

### Página 2

#### Problema 1
Considere dos cascarones esféricos de radios a y b (a < b). El cascarón interior tiene una carga
homogéneamente distribuida Q y la exterior ´Q. Encuentre la diferencia de potencial entre ambos
cascarones.

#### Problema 2
Dos cables infinitos, paralelos al eje x, poseen densidades de carga uniformes λ y ´λ. Ellos están
a distancia a del origen. Encuentre el potencial en un punto px, y, zq usando el origen como punto
de referencia.
#### Problema 3
Un plano infinito y uniforme de carga eléctrica con densidad σ pasa por un punto O. Por O hay una
recta OX que es perpendicular al plano. A distancia a de 0 se encuentra una carga eléctrica puntual
´q.
a) Calcule el potencial eléctrico resultante en un (unto P px) cualquiera entre a y O.
b) Una partícula de masa m y carga eléctrica ´e se libera desde el punto medio entre O y a.
¿Con qué velocidad choca contra el plano de carga?

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Solución Ayudantía 9
Potencial Eléctrico: Parte 2

Resumen
El potencial eléctrico V corresponde a la energía electrostática por unidad de carga, y se define
como:
U
V “
q
A partir de esto, podemos definir la diferencia de potencial ∆V como el trabajo por unidad de carga
para mover a una carga desde un punto A a otro punto B:
żB
⃗ ¨ d⃗l
∆V = ´
E
A

Al igual que para la energía potencial electrostática, podemos tomar como referencia el infinito tal
que V (∞) = 0, y así tendremos que para una carga Q el potencial es,
V = k

Q
r

donde r es la distancia entre la carga y el punto en donde se quiere medir el potencial. Así, al
considerar un sistema de N cargas puntuales tendremos que:
ÿ qi
V = k
r
i
Además, podemos obtener el campo eléctrico a partir del potencial según:
⃗ = ´∇V
E
Para una distribución continua de cargas, tendremos que:
ż
dq
V = k
|⃗r ´ ⃗r 1 |

---

### Página 2

#### Problema 1
Considere dos cascarones esféricos de radios a y b (a < b). El cascarón interior tiene una carga
homogéneamente distribuida Q y la exterior ´Q. Encuentre la diferencia de potencial entre ambos
cascarones.

Calcularemos la diferencia de potencial integrando el campo eléctrico, esto resulta más sencillo porque debido a la simetría del problema, calcularemos el campo eléctrico con ley de
Gauss. Así, sabemos:
żb
⃗ ¨ d⃗l
∆V = V (b) - V (a) = - E
a

Ahora, como calcularemos la integral entre a y b, entonces solo nos interesa el campo entre
a y b:
ż
qenc
E ¨ dS “
ϵ0
Cualquier superficie entre a y b encierra la carga del primer cascarón, por lo tanto qenc = Q.
Utilizando ley de Gauss como lo hemos hecho siempre:
⃗ = Q 1 r̂
E
4πϵ0 r2
Ya con esto nos queda simplemente calcular la integral entre a y b, lo más fácil es elegir un
camino radial tal que, d⃗l = drr̂:
żb
Q
dr
∆V = ´
4πϵ0 a r2
Y realizando la integral llegamos a nuestro resultado final:
Q
∆V “
4πϵ0

ˆ

1 1
´
b a

˙

---

### Página 3

#### Problema 2
Dos cables infinitos, paralelos al eje x, poseen densidades de carga uniformes λ y ´λ. Ellos están
a distancia a del origen. Encuentre el potencial en un punto px, y, zq usando el origen como punto
de referencia.
Como los cables son paralelos al eje x, su posición queda determinada por sus coordenadas en el plano transversal yz. La configuración simétrica más natural, consistente con que
ambos están a distancia a del origen, es:
Cable 1: (y, z) = (a, 0),

con carga lineal ` λ,

Cable 2: (y, z) = p´a, 0q,

con carga lineal ´ λ.

Como los cables son infinitos en la dirección x, el sistema es invariante por traslaciones a lo
largo de ese eje. Por ello, el potencial no puede depender de x; solamente dependerá de la
distancia del punto al eje de cada cable, medida en el plano yz.

Dado que los cables se extienden a lo largo del eje x, la distancia relevante no es la distancia
espacial tridimensional a un punto del cable, sino la distancia perpendicular al eje de cada
línea.
Distancia al cable con carga `λ: Ese cable está en (y, z) = (a, 0), por lo que la distancia
perpendicular desde el punto px, y, zq es
a
ρ` = py - aq2 ` z 2 .
Distancia al cable con carga -λ: Ese cable está en (y, z) = p´a, 0q, por lo que la distancia perpendicular es
a
ρ´ = py ` aq2 ` z 2 .

---

### Página 4

Obsérvese nuevamente que no aparece la coordenada x, porque al ser los cables infinitos en
esa dirección, todos los puntos con las mismas coordenadas py, zq son equivalentes.
Recordemos primero el resultado conocido para una línea infinita de carga con densidad
lineal λ. El campo eléctrico a una distancia perpendicular ρ de la línea es:
λ
2πε0 ρ
Este campo es radial en el plano perpendicular a la línea. Como el potencial satisface:
ż
⃗ ¨ d⃗ℓ,
∆V = - E
Epρq “

podemos obtener la diferencia de potencial entre dos distancias ρ0 y ρ desde la línea:
żρ
λ
V (ρ) - V (ρ0 ) = ´
dρ1 .
ρ0 2πε0 ρ
Aquí se usa una variable muda ρ1 para no confundirla con el límite superior ρ. Integrando:
żρ 1
λ
dρ
λ
ρ
V (ρ) - V (ρ0 ) = ´
“
´
rln ρ1 sρ0 .
2πε0 ρ0 ρ1
2πε0
Entonces:
ˆ ˙
ρ
λ
ln
V (ρ) - V (ρ0 ) = ´
2πε0
ρ0
Equivalentemente, esto puede escribirse como:
V (ρ) = ´
o también:

λ
ln ρ ` C,
2πε0

ˆ ˙
λ
ρ0
,
ln
V pρq “
2πε0
ρ

donde C o ρ0 representan la constante de referencia.
Para una sola línea infinita de carga, el potencial absoluto no puede fijarse tomando V (∞) = 
0, porque el logaritmo diverge cuando ρ Ñ 8. Por eso solo tienen sentido las diferencias de
potencial, o bien se debe fijar el cero en un punto específico. En este problema sí puede elegirse el origen como referencia porque la combinación de ambas líneas hace que el potencial
total quede bien definido respecto a ese punto.
Aplicamos ahora el resultado anterior a cada línea por separado.
Cable con carga `λ: Su potencial en el punto px, y, zq será:
V` (x, y, z) = ´

λ
ln ρ` ` C` .
2πε0

---

### Página 5

Cable con carga ´λ: Si reemplazamos λ Ñ ´λ en la expresión anterior, obtenemos:
V´ (x, y, z) = ´

λ
p´λq
ln ρ´ ` C´ “
ln ρ´ ` C´ .
2πε0
2πε0

El potencial eléctrico es una magnitud escalar, por lo que se suma directamente. Así,
V (x, y, z) = V` (x, y, z) ` V´ (x, y, z).
Sustituyendo:
V (x, y, z) = ´

λ
λ
ln ρ` `
ln ρ´ ` pC` ` C´ q.
2πε0
2πε0

Agrupando términos:
V px, y, zq “

λ
pln ρ´ ´ ln ρ` q ` C,
2πε0

donde:
C = C ` ` C´ .
Usando la propiedad del logaritmo:
ˆ ˙
A
ln A - ln B = ln
,
B
queda:
ˆ ˙
ρ´
λ
ln
` C.
V px, y, zq “
2πε0
ρ`
Sustituyendo las distancias ρ` y ρ´ :
˜a
¸
py ` aq2 ` z 2
λ
V px, y, zq “
ln a
` C.
2πε0
py ´ aq2 ` z 2
El problema indica que debe usarse el origen como referencia. Eso significa que:
V (0, 0, 0) = 0.
Evaluemos primero las distancias desde el origen a cada cable:
ρ` p0, 0, 0q “

a

p0 - aq2 ` 02 = a,

ρ´ p0, 0, 0q “

a

p0 ` aq2 ` 02 = a.

Por lo tanto,
V p0, 0, 0q “

´a¯
λ
λ
ln
`C “
lnp1q ` C.
2πε0
a
2πε0

---

### Página 6

Como ln(1) = 0, resulta:
V (0, 0, 0) = C.
Pero la condición de referencia exige que:
V (0, 0, 0) = 0,
así que necesariamente:
C = 0.
Entonces el potencial buscado es:
˜a
¸
py ` aq2 ` z 2
λ
V px, y, zq “
ln a
2πε0
py ´ aq2 ` z 2

#### Problema 3
Un plano infinito y uniforme de carga eléctrica con densidad σ pasa por un punto O. Por O hay una
recta OX que es perpendicular al plano. A distancia a de 0 se encuentra una carga eléctrica puntual
´q.
a) Calcule el potencial eléctrico resultante en un (unto P px) cualquiera entre a y O.
b) Una partícula de masa m y carga eléctrica ´e se libera desde el punto medio entre O y a.
¿Con qué velocidad choca contra el plano de carga?

---

### Página 7

a) Tomaremos el eje x sobre la recta OX, con:
O ” x = 0,

plano cargado en x = 0,

carga - q en x = a.

El punto donde queremos calcular el potencial es
P (x),

0 < x < a.

Como el plano es infinito y uniforme, el problema tiene simetría plana: el campo del plano
sólo depende del lado del plano en que se esté, y en cada lado es constante y perpendicular
al plano.
El potencial total se obtiene por superposición:
ϕpxq = ϕplano (x) ` ϕcarga (x).
Por lo tanto, calcularemos por separado el aporte del plano y el de la carga puntual.
Campo eléctrico debido al plano infinito:
Sabemos que un plano infinito con densidad superficial de carga σ produce un campo eléctrico de magnitud constante:
σ
2ε0
Si σ > 0, el campo sale perpendicularmente del plano hacia ambos lados. Como estamos
trabajando en la región x > 0, el campo apunta en la dirección `î:
Eplano “

⃗ (lano px) = σ î.
E
2ε0
Es importante notar que este campo:
no depende de x;
tiene la misma magnitud en cualquier punto del semiespacio x > 0.
Potencial debido al plano:
Recordemos la relación entre potencial y campo:
żB
⃗ ¨ d⃗ℓ.
E

ϕpBq - ϕpAq = ´
A

Tomemos dos puntos sobre el eje x: uno en x y otro en R, con R > x. Entonces, para el
plano,
żx
⃗ plano ¨ d⃗ℓ.
ϕplano (x) - ϕplano (R) = ´
E
R

---

### Página 8

También puede escribirse de manera equivalente como:
żR
⃗ plano ¨ d⃗ℓ.
E

ϕplano (x) - ϕplano (R) = 
x

Como sobre el eje x se tiene:
d⃗ℓ = dx1 î,
y
⃗ plano = σ î,
E
2ε0
entonces:
żR
ϕplano (x) - ϕplano (R) = 

σ
σ
dx1 “
pR ´ xq.
2ε0
x 2ε0

De aquí obtenemos:
σ
σ
R´
x.
2ε0
2ε0
Agrupando los términos constantes en una sola constante C:
ϕplano (x) = ϕplano (R) `

ϕplano (x) = C ´

σ
x,
2ε0

C “ ϕplano pRq `

σ
R.
2ε0

donde:

Potencial debido a la carga puntual ´q:
La carga puntual se encuentra en x = a. La distancia desde el (unto P px) hasta esa carga es:
r “ |a ´ x|.
Como estamos en la región 0 < x < a, se cumple que a - x > 0, así que:
r = a - x.
El potencial de una carga puntual Q a una distancia r es:
ϕ“

1 Q
4πε0 r

Aquí Q = -q, por lo tanto:

---

### Página 9

1 ´q
4πε0 a ´ x

ϕcarga (x) = 
Es decir,

ϕcarga (x) = ´

q
4πε0 pa ´ xq

Por superposición,
ϕpxq = ϕplano (x) ` ϕcarga (x).
Sustituyendo las expresiones halladas:
ˆ
˙
σ
q
ϕpxq = C ´
x ´
2ε0
4πε0 pa ´ xq
Así, el potencial resultante para 0 < x < a es:
ϕpxq = ´

q
σ
`C ´
x
4πε0 pa ´ xq
2ε0

p0 < x < aq,

donde C es una constante arbitraria de referencia.
b) Ahora consideramos una partícula de masa m y carga ´e que se libera desde el punto
medio entre O y la carga ´q.
Eso significa que la partícula parte desde:
a
xi “ ,
y termina impactando con el plano en:
xf = 0.
Supondremos que:
se libera desde el reposo;
podemos despreciar efectos radiativos y cualquier fenómeno no electrostático;
el campo electrostático es conservativo.
Entonces podemos usar conservación de la energía mecánica.
Antes de escribir ecuaciones, conviene entender el movimiento.
El plano tiene carga positiva, así que una carga negativa ´e es atraída hacia el plano.
La carga puntual fija es también negativa (´q). Por lo tanto repele a la partícula ´e.

---

### Página 10

Como la carga ´q está a la derecha de la partícula, esa repulsión empuja a la partícula hacia
la izquierda, es decir, también hacia el plano.
Por lo tanto, ambas interacciones hacen que la partícula acelere hacia el plano. Eso anticipa
que la rapidez final será mayor que cero.
La energía potencial de una carga Q1 en un potencial ϕ es:
U = Q1 ϕ.
Como la partícula de prueba tiene carga:
Q1 = -e,
su energía potencial es:
U (x) = -e ϕpxq.
La conservación de la energía entre el punto inicial x = a{2 y el punto final x = 0 da:
Ki ` Ui = Kf ` Uf .
Como la partícula parte del reposo,
Ki = 0.
Entonces,
U

´a¯

“ U (0) ` mvf2 .

Sustituyendo U (x) = -eϕpxq:
´a¯
“ -e ϕp0q ` mvf2 .
´e ϕ
Reordenando,
”
´ a ¯ı
1 2
mvf = e ϕp0q - ϕ
Por tanto,
´ a ¯ı
2e ”
ϕp0q ´ ϕ
m
Así que ahora necesitamos calcular la diferencia de potencial entre esos dos puntos.
Partimos de:
vf2 “

ϕpxq = ´

q
σ
`C ´
x.
4πε0 pa ´ xq
2ε0

---

### Página 11

Potencial en el plano (x = 0):
ϕp0q = ´

σ
q
`C ´
p0q.
4πε0 pa ´ 0q
2ε0

Por lo tanto,
q
ϕp0q = ´
` C.
4πε0 a
`
˘
Potencial en el punto inicial x = a2 :
´a¯
q
σ a
˘ `C ´
`
ϕ
“´
a
2ε0 2
4πε0 a ´ 2
Como
a´

a
a
“ ,

entonces:
´a¯
q
σa
ϕ
“´
`C ´
4πε0 pa{2q
4ε0
Y simplificando:
´a¯
2q
σa
“´
`C ´
ϕ
4πε0 a
4ε0
Es decir,
´a¯
q
σa
“´
`C ´
ϕ
2πε0 a
4ε0
Ahora calculamos:
ϕp0q ´ ϕ

´a¯

Sustituyendo:
ϕp0q ´ ϕ

´a¯

ˆ
“

q
´
`C
4πε0 a

˙

ˆ

2q
σa
´ ´
`C ´
4πε0 a
4ε0

Distribuyendo el signo menos:
ϕp0q ´ ϕ

´a¯

“´

q
2q
σa
`C `
´C `
4πε0 a
4πε0 a
4ε0

Se cancelan las constantes C:
ϕp0q ´ ϕ

´a¯

“

q
σa
`
4πε0 a 4ε0

˙

---

### Página 12

Esto muestra claramente por qué la constante arbitraria del potencial no afecta el resultado
físico.
Sustituimos en:
2e
vf2 “

”

2e
vf2 “

ˆ

ϕp0q ´ ϕ

m

´ a ¯ı

Entonces:

m

q
σa
`
4πε0 a 4ε0

˙

Por lo tanto, la rapidez con que choca contra el plano es:
d
vf “

2e
m

ˆ

q
σa
`
4πε0 a 4ε0

˙
