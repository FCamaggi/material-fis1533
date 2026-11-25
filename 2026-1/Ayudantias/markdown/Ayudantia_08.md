---
title: "Ayudantia 08"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_08.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_08_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 08

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 8
Potencial Eléctrico

#### Problema 1
Considere la siguiente distribución de carga en coordenadas esféricas,
ρ(r) = Crλ

,

r<a

Calcule el potencial en el centro de la esfera tomando como referencia que V (∞) = 0 y asuma que
λ es una constante no negativa.

#### Problema 2
Un alambre, cuya densidad de carga lineal es λ, se extiende por el eje z desde z = -d hasta z = d.

(a) Calcule el potencial en un punto z > d sobre el eje del alambre.
(b) ¿Cual es el cambio de energía potencial de un electrón si se mueve de z = 4d hasta z = 3d?
(c) Si el electrón parte del reposo desde z = 4d ¿Cuál será su velocidad en z = 3d?
#### Problema 3
Se tienen dos anillos sobre un mismo eje y de mismo radio R sobre planos paralelos y separados
entre sí a una distancia L. Uno de los anillos tiene densidad λ y el otro ´λ.

---

### Página 2

Calcule la diferencia de potencial entre los centros de ambos anillos.

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Solución ayudantía 8
Potencial Eléctrico

#### Problema 1
Considere la siguiente distribución de carga en coordenadas esféricas,
ρ(r) = Crλ

,

r<a

Calcule el potencial en el centro de la esfera tomando como referencia que V (∞) = 0 y asuma que
λ es una constante no negativa.

#### Solución
Primero debemos calcular el campo eléctrico de esta configuración, tanto fuera como dentro de la
esfera, partimos calculando la carga encerrada para cualquier r < a,
żr

ż
Q(r) = 

Cr1λ`2 dr1 = 4πC

dΩ

rλ`3
λ`3

Entonces utilizamos ley de Gauss dentro de la esfera,
ż

⃗ ¨ d⃗s = Q
E
ϵ0

Como estamos dentro de la esfera, cada superficie gaussiana dibujada cambia la carga encerrada
según r, por tanto en ambos lados de la igualdad debe aparecer un r que varía (Veremos qué pasa
fuera luego),
4πr2 E “

4πC rλ`3
ϵ0 λ ` 3

Lo que da un campo eléctrico de la siguiente forma,

---

### Página 2

λ`1

⃗ = C r
E
r̂
ϵ0 λ ` 3

;

rďa

Para el caso fuera de la esfera (r > a) la idea es similar, con la salvedad de que sin importar que
tan grande sea el radio de mi superficie gaussiana, siempre encerraremos la misma carga (Hasta a),
por tanto,
4πC aλ`3
ϵ0 λ ` 3

4πr2 E “

Despejando obtenemos el campo fuera de la esfera,
λ`3
⃗ = C a
E
r̂
ϵ0 λ ` 3 r2

;

rďa

Falta calcular el potencial, utilizamos la definición mediante la integral de línea,
⃗l = ´
⃗
Eprqd

V = ´

ż0

ż0

ż0

⃗
Eprqr̂dr
“´

Eprqdr

Como la expresión de la integral no es igual en todo el dominio de integración, debe separar la
integral en una suma de la forma,
ża

C rλ`1
dr `
0 ϵ0 λ ` 3

ż8
a

C aλ`3 1
dr
ϵ0 λ ` 3 r2

Integrando obtenemos,
„
ȷ
C
aλ`2
aλ`2
V p0q “
`
ϵ0 pλ ` 3qpλ ` 2q λ ` 3
La suma la podemos realizar directamente llegando entonces a nuestro resultado final,

V p0q “

C aλ`2
ϵ0 λ ` 3

#### Problema 2
Un alambre, cuya densidad de carga lineal es λ, se extiende por el eje z desde z = -d hasta z = d.

(a) Calcule el potencial en un punto z > d sobre el eje del alambre.
(b) ¿Cual es el cambio de energía potencial de un electrón si se mueve de z = 4d hasta z = 3d?

---

### Página 3

(c) Si el electrón parte del reposo desde z = 4d ¿Cuál será su velocidad en z = 3d?

Para este problema no vamos a considerar los efectos gravitatorios por simplicidad. La configuración a la que nos estamos enfrentando es la siguiente,

Calculamos el potencial eléctrico, como sabemos,

dq 1
|r ´ r1 |

(1)

Como siempre recordamos, r1 parametriza la región donde hay carga y r un punto (en principio
arbitrario) donde queremos medir el potencial eléctrico. Entonces,

r = z

(2)

r1 = z 1

,

dq = λdz

z 1 P r´d, ds

(3)
(4)

entonces la integral a calcular pasa a ser,
V (z) = 

żd

λ
dz 1
´d |z ´ z |

(5)

Como nos interesan puntos sobre la barra, es decir z > d, el valor absoluto puede eliminarse ya
que en todos estos puntos z > z 1 . El potencial que resulta de resolver la integral es,
λ
V (z) = 
ln

ˆ

z`d
z´d

˙
(6)

Recordemos que el potencial eléctrico se relaciona directamente con la energía potencial que percibe una carga de la forma U = qV , siendo q la carga de la partícula y V el potencial que percibe en

---

### Página 4

el punto donde se encuentra. Por tanto, la diferencia de energía potencial entre los puntos pedidos
es,
qλ
ln
∆U = U (3d) - U (4d) = q(V p3d) - V (4dq) = 

ˆ ˙

(7)

Para calcular la velocidad en el punto z = 3d utilizaremos la conservación de energía mecánica, en
z = 4d no hay energía cinética; por tanto,
qλ
U (4d) ` T (4d) = U (3d) ` T (3d) Ñ T (3d) = ´∆U = 
ln

ˆ ˙

(8)

y recordando T = mv 2 {2, obtenemos que la velocidad en z = 3d,
d
vp3dq “

mqλ
ln

ˆ ˙

(9)

#### Problema 3
Se tienen dos anillos sobre un mismo eje y de mismo radio R sobre planos paralelos y separados
entre sí a una distancia L. Uno de los anillos tiene densidad λ y el otro ´λ.

Calcule la diferencia de potencial entre los centros de ambos anillos.

En esta solución, utilizaremos el método de calcular el potencial eléctrico de manera directa utilizando.

dq
|r ´ r1 |

---

### Página 5

Haremos un desarrollo un poco distinto a modo de prepararnos para cualquier ejercicio, calcularemos el potencial para cualquier punto en el eje de simetría del anillo, para un anillo a cualquier
altura, es decir, tendremos V pzo , zq, donde z0 es la altura del anillo y z la posición donde medimos
el potencial.
Tenemos que definir nuestro r, r1 y dq (Como lo hemos hecho todo este mes),

r = z ẑ
r1 = R cos θx̂ ` R sin θŷ ` z0 ẑ
|r - r1 |2 = R2 ` pz - z0 q2
dq = λRdθ
Entonces la integral nos queda de la forma,
V pz0 , zq “

ż 2π

λRdθ
a
“
2πλR a
pz ´ z0 q ` R
pz ´ z0 q2 ` R2

Quedando nuestro potencial general de la forma,
V pz0 , zq “

2ϵ0

a

Rλ
pz ´ z0 q2 ` R2

Hasta acá no hemos tomado en cuenta ningún dato del problema, solo calculamos el potencial
eléctrico que genera un anillo a cierta altura y en un punto cualquiera. Lo hicimos así porque
tenemos dos anillos que calcular en este ejercicio, entonces utilizando superposición, podemos
solamente sumar ambos potencial generados, coloquemos nuestro origen del sistema en el centro
de nuestro anillo de densidad ´λ, quedando el potencial total de la forma,
V (z) = V` (L, z) ` V´ (0, z) = 

Rλ
pa
´? 2
q
2ϵ0
z ` R2
pz ´ Lq2 ` R2

Esto es solamente el potencial que genera esta configuración a cualquier altura medida desde el
centro del anillo de densidad ´λ, y nos están preguntando la diferencia de potencial de los centros
de los anillos, esto es simplemente,
∆V = V (L) - V (0) = 

Rλ
Rλ 1
?
p ´? 2
q
´
p
´
q
2ϵ0 R
2ϵ0 L2 ` R2 R
L ` R2

Simplificando la expresión anterior„ llegamos a la diferencia de potencial entre ambos centros,
∆V “

Rλ 1
q
p ´? 2
ϵ0 R
L ` R2
