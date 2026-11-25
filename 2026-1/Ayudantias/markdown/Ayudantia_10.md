---
title: "Ayudantia 10"
source_enunciado: "Electro/2026-1/Ayudantias/Enunciados/Ayudantia_10.pdf"
source_solucion: "Electro/2026-1/Ayudantias/Soluciones/Ayudantia_10_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 10

## Enunciado

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 10
Capacitores

#### Problema 1
Considere un cilindro sólido de radio a, conductor, rodeado por un cascarón cilíndrico de radio
interior b. La longitud de estos cilindros es L y se asume que b ´ a ! L. Este condensador se carga
de tal manera que el cilindro de radio a tiene carga Q y el exterior ´Q. Calcule la capacitancia del
sistema.

#### Problema 2
Considere un condensador esférico, que consiste de 2 esferas concéntricas de radios a y b. La
cáscara interior posee una carga Q distribuida sobre su superficie y la esfera exterior, de igual forma,
carga ´Q. ¿Cuál es la capacidad de esta configuración? También podemos estudiar la capacidad
de la esfera de radio a por sí sola, tomando que la otra terminal del condensador está muy lejos, es
decir b Ñ 8, calcule la capacidad en este caso también.

---

### Página 2

#### Problema 3
Dos conductores cilíndricos muy largos, de radios a1 y a2 , respectivamente, están dispuestos con
sus ejes paralelos y separados entre sí por una distancia d, tal que d " a1 y d " a2 .
a) Demuestre que la capacitancia por unidad de longitud de cilindro C para este arreglo está dada
aproximadamente por la expresión
˙ȷ´1
„ ˆ
d
.
(1)
C » πϵ0 ln ?
a1 a2
#### Problema 4
Se desea diseñar un condensador esférico a partir de un casquete conductor esférico de radio exterior a, que sea capaz de almacenar la mayor cantidad de energía posible, sujeto a la restricción de
que el campo eléctrico en la superficie de la esfera conductora interior, concéntrica con el casquete
y de radio b < a, no pueda exceder un valor dado E0 . Calcule, en función de E0 , a y constantes, el
valor que debe tener el radio b y la magnitud de la energía que puede almacenar el conductor.

---

### Página 3

Propuesto
Un esferoide es el análogo a una elipse en 3D, su volumen viene definido por,
Vesf eroide = πab2
Donde a y b son el largo de los semiejes. Notamos que cuando a = b recuperamos el volumen de
una esfera. La capacidad de esta configuración puede ser escrita en términos de un parámetros de
excentricidad como,
8πϵ0 aη
C“
ln 1`η
1´η

c
con

η“

1´

b2
a2

(a) Verifique que cuando b Ñ a, recuperamos el resultado para una esfera (Ejercicio anterior).
(b) Imagine que el esferoide es una gotita de agua cargada. Si la gotita de agua es deformada de
manera arbitraria, pero siempre manteniendo el volumen y la carga almacenada constante,
desde una esfera a un esferoide alargado. ¿Que sucede con la energía almacenada, aumenta
o disminuye?

---

## Solución

### Página 1

P ONTIFICIA U NIVERSIDAD C ATÓLICA DE C HILE - FACULTAD DE F ÍSICA
Electricidad y Magnetismo - FIS1533-2 - 2026-1
Profesor: Rodrigo López
Ayudantes: Javiera Villalobos (jvvillalobos@uc.cl), Vicente Strauch (vicente.strauch@uc.cl)

Ayudantía 10
Capacitores

#### Problema 1
Considere un cilindro sólido de radio a, conductor, rodeado por un cascarón cilíndrico de radio
interior b. La longitud de estos cilindros es L y se asume que b ´ a ! L. Este condensador se carga
de tal manera que el cilindro de radio a tiene carga Q y el exterior ´Q. Calcule la capacitancia del
sistema.

#### Solución
Como queremos calcular la capacitancia de esta configuración, debemos determinar primero la
diferencia de potencial entre ambos conductores. Para ello, nos interesa la región comprendida
entre los cilindros, es decir, para
a < r < b.
Debido a la simetría cilíndrica del sistema, el campo eléctrico en esta región es radial y depende
solo de r. Aplicando la ley de Gauss sobre una superficie cilíndrica coaxial de radio r y longitud
L, se obtiene
¿
⃗ ¨ dA
⃗ = E(rq p2πrL) = Q ,
E
ε0

---

### Página 2

de donde resulta
⃗
E(r)

Q 1
r̂,
2πε0 L r

a < r < b.

La diferencia de potencial entre el cilindro interior y el cilindro exterior se obtiene integrando el
campo eléctrico a lo largo de un camino radial. Entonces,
żb
ża
⃗
⃗
E ¨ dl “
E(r) dr.
V (a) - V (b) = ´
b

a

Sustituyendo la expresión del campo,
żb

Q 1
V paq ´ V pbq “
dr “
2πε0 L
a 2πε0 L r

żb

dr
,
a r

y por lo tanto,
ˆ ˙
b
V paq ´ V pbq “
ln
.
2πε0 L
a
Con esto ya tenemos todo lo necesario para calcular la capacitancia:
C“

V paq ´ V pbq

2πε0 L
ˆ ˙“
.
b
lnpb{aq
ln
2πε0 L
a

IMPORTANTE: notar que el cálculo de la capacitancia depende de la diferencia de potencial entre
dos superficies equipotenciales, en este caso la superficie del cilindro interior r = a y la superficie
interna del conductor exterior r = b.
#### Problema 2
Considere un condensador esférico, que consiste de 2 esferas concéntricas de radios a y b. La
cáscara interior posee una carga Q distribuida sobre su superficie y la esfera exterior, de igual forma,
carga ´Q. ¿Cuál es la capacidad de esta configuración? También podemos estudiar la capacidad
de la esfera de radio a por sí sola, tomando que la otra terminal del condensador está muy lejos, es
decir b Ñ 8, calcule la capacidad en este caso también.

---

### Página 3

Nos interesa calcular el potencial, y para esto tenemos que integrar el campo eléctrico entre los
extremos de la región que nos interesa, es decir, para a < r < b, acá siempre vamos a estar
encerrados la superficie de la esfera de radio a, donde está toda la carga Q, es decir, nuestra carga
encerrada es qenc = Q. Utilizando la ley de Gauss para una superficie esférica, obtenemos que el
campo eléctrico en esta región es,
⃗
E(r)

1 Q
r̂
4πϵ0 r2

Para el cálculo del potencial integramos este campo en un camino que conecte la superficie definida
por a con la definida por b, como siempre elegimos un camino radial,
żb
∆V = Vb - Va = ´

Q dr
Q 1 1
Q b´a
´
p
´
q
´
p
q
4πϵ0 a b
4πϵ0 ab
a 4πϵ0 r

De esta forma, la capacidad de la configuración es,
C“

ab
“ 4πϵ0
|∆V |
b´a

¿Qué sucede en el límite cuando b Ñ 8?, obtenemos la capacidad de la esfera de radio a,
Ca = lím C = 4πϵ0 a
bÑ8

#### Problema 3
Dos conductores cilíndricos muy largos, de radios a1 y a2 , respectivamente, están dispuestos con
sus ejes paralelos y separados entre sí por una distancia d, tal que d " a1 y d " a2 .

---

### Página 4

a) Demuestre que la capacitancia por unidad de longitud de cilindro C para este arreglo está dada
aproximadamente por la expresión
˙ȷ´1
„ ˆ
d
C » πϵ0 ln ?
.
(1)
a1 a2

La ley de Gauss nos dice que el campo eléctrico generado por un cilindro, fuera de la configuración,
viene dado por,
⃗ “
E

1 Q
r̂
2πϵ0 L r

Asumimos una carga Q para la totalidad del cilindro (Esta carga debe estar en su superficie al tratarse de un conductor), como nos piden capacitancia, luego esta Q será simplificada y el resultado
no dependerá de haber asumido esto.
Si tomamos como origen de nuestro sistema, el centro del cilindro de radio a1 , el campo eléctrico
total en función de la distancia al origen del sistema sería,
⃗ “
E

„
ȷ
´
x̂
2πϵ0 L x
d´x

Para el cálculo de la diferncia de potencial, debemos integrar el campo eléctrico entre a1 y d ´ a2 ,
que corresponden a los bordes de los cilindros (Dento de estos el campo eléctrico es nulo al ser un
conductor) entonces,
ż a1
∆V = ´

⃗ ¨ d⃗l “
EE

da2

„
ȷ ˇd´a2
ˇ
x
ˇ
ln
2πϵ0 L
d ´ x ˇa1

De esta manera la diferencia de potencial viene dada por,
„
ȷ
pd ´ a2 qpd ´ a1 q
∆V “
ln
2πϵo L
a1 a2
Cuando d " a1 , a2 , d ´ a1 « d y d « d ´ a1 , de esta forma la diferencia de potencial es,
„
ȷ
d
∆V “
ln ?
πϵ0 L
a1 a2
y la capacitancia por unidad de largo la sacamos simplemente por definición,
„ ˆ
˙ȷ´1
C
1 Q
d
c“
“ πϵ0 ln ?
L
L |∆V |
a1 a2

---

### Página 5

#### Problema 4
Se desea diseñar un condensador esférico a partir de un casquete conductor esférico de radio exterior a, que sea capaz de almacenar la mayor cantidad de energía posible, sujeto a la restricción de
que el campo eléctrico en la superficie de la esfera conductora interior, concéntrica con el casquete
y de radio b < a, no pueda exceder un valor dado E0 . Calcule, en función de E0 , a y constantes, el
valor que debe tener el radio b y la magnitud de la energía que puede almacenar el conductor.

Primer necesitamos calcular el campo eléctrico en la región intermedia, si asumimos que dentro de
la esfera de radio b hay una carga Q, entonces el campo eléctrico viene dado por,
⃗ “
E

r̂
4πr2 ϵ0

e integrando este potencial a través de una línea que une ambos casquetes, obtenemos la diferencia
de potencial,
żb

ˆ

C“

4πϵ0 ab
|∆V |
a´b

⃗ ¨ d⃗l = Q
∆V = - E
4πϵ0
a

1 1
´
b a

˙

y esto nos entrega la capacitancia,

nos dicen además que en la superficie de la esfera interior, el campo eléctrico no puede ser mayor que E0 , entonces nos vamos al caso extremo en que en dicho punto, el campo eléctrico es
exactamente E0 , entonces,
Epr = bq = 

“ E0 Ñ Q = 4πb2 ϵ0 E0
4πϵ0 b2

---

### Página 6

Este Q lo necesitamos para calcular la energía del capacitor, ya que es de la forma,
U“

2πϵ0 b3 E02 pa ´ bq
2C
a

Queremos que esta expresión sea máxima para algún valor de b, entonces buscamos que la derivada
respecto a b sea 0,
dU
2πϵ0 E02
3a
p3ab2 - 4b3 q = 0 Ñ b = 
db
a
este b asegura que alcanzará un valor extremo ¿Cómo sabremos si es mínimo o máximo? con la
segunda derivada,
d2 U
2πϵ0 Eo2
p6ab ´ 12b2 q
db2
a
Evaluamos en b = 3a{4,
d2 U
3a
2πϵ0 E02
pb
q
db2
a

ˆ

18a2 ´ 27a2

˙

Esta expresión es siempre menor que 0, por tanto cuando b = 3a{4, alcazamos el máximo valor de
energía almacenada,

U pb = 3a{4q = 

27πϵ0 E02 a3

(2)

Propuesto
Un esferoide es el análogo a una elipse en 3D, su volumen viene definido por,
Vesf eroide = πab2
Donde a y b son el largo de los semiejes. Notamos que cuando a = b recuperamos el volumen de
una esfera. La capacidad de esta configuración puede ser escrita en términos de un parámetros de
excentricidad como,
8πϵ0 aη
C“
ln 1`η
1´η

c
con

η“

1´

b2
a2

(a) Verifique que cuando b Ñ a, recuperamos el resultado para una esfera (Ejercicio anterior).

---

### Página 7

(b) Imagine que el esferoide es una gotita de agua cargada. Si la gotita de agua es deformada de
manera arbitraria, pero siempre manteniendo el volumen y la carga almacenada constante,
desde una esfera a un esferoide alargado. ¿Que sucede con la energía almacenada, aumenta
o disminuye?

Este ejercicio no es para nada fácil, iremos paso a paso; sirve para estudiar un ejercicio un tanto
distinto a los que estamos acostumbrados.
Lo primero que se nos pide es ver qué sucede con la capacitancia cuando b Ñ a, notamos que esto
es equivalente a η Ñ 0, es decir, tenemos que calcular el siguiente límite,
lím C = 8πϵ0 a lím

η

ηÑ0 ln 1`η
1´η

ηÑ0

Este límite corresponde a una indeterminación del tipo 0{0, por lo que podemos usar L’Hopital de
la siguiente forma,
d
1`η
pln
q“
dη
1´η
1 ´ η2
Reemplazando en el límite que queríamos calcular obtenemos la capacitancia de esta configuración
en el límite cuanto b Ñ a,
C = 4πϵ0 a
Como obtuvimos en el ejercicio anterior.
Para la parte b, sabemos una cosa sobre el volumen, parte desde una esfera y a medida que se ve
volviendo esferoide, conserva su volumen, esto quiere decir,
4 3 4
πR = πab2 = cte
Esto nos permite obtener la siguiente relación,
R3
a

b2 “

Lo que podemos reemplazar en nuestra expresión para la excentricidad de la forma,
c
η“

b2
1´ 2 “
a

c
1´

R3
R
Ñ
“ p1 - η 2 q1{3
a
a

---

### Página 8

Queremos comparar como luce la energía U para la esfera U = Q2 {2Cesfera , con la energía almacenada por un esferoide cualquiera, como además la carga Q se mantiene constante, basta con
estudiar que pasa cuando cambia Cesfera Ñ Cesferoide .

ˆ
„
ȷ˙
Q2
1`η
¨
ln
U“
2Cesferoide
8πϵ0 aη
1´η
˜
¸
„
ȷ
Q2
1`η
¨
¨ ln
R
1´η
8πϵ0 a R η
„
ˆ
ȷ˙
1`η
Q2
¨ ln
¨
2C0
2 ¨ Ra η
1´η
ˆ
„
ȷ˙
1 R
1`η
¨
¨ ln
2C0
2η a
1´η
˜
„
ȷ¸
1`η
Q2
p1 ´ η 2 q 3
¨ ln
¨
2C0
2η
1´η
Q2

Donde definimos entremedio C0 = Cesfera = 4πϵ0 R
Como vemos, tenemos el término Q2 {2C0 representando la energía de una esfera, y a medida que
se va haciendo menos esférico el esferoide, η aumenta, entonces queremos saber si el término que
multiplica a nuestra energía de la esfera hace más gránde nuestra energía o más chica; para esto
utilizaremos una expansión de taylor en torno a η = 0, quedando de la siguiente forma,
Q2
U«
2C0

ˆ

˙
η4
64η 6
1´
´
´ Opη q
45 2835

Los términos siguientes al leading order, restan energía a la esfera, es decir, a medida que aumenta
la excentricidad de nuestra esfera, disminuye la energía que almacena.
