---
title: "Ejercicios Teoría Electromagnética - Fabián Cádiz"
source_pdf: "Electro/material-apoyo/apuntes-cadiz/Teoría Electromagnética - Fabián Cádiz (libro completo).pdf"
pages: 564
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Ejercicios Teoría Electromagnética - Fabián Cádiz

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física

Teoría Electromagnética
Con ejercicios resueltos

Fabián Cádiz

---

### Página 2

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 3

Parte I
Electrostática

---

### Página 4

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 5

#### Capítulo 1
Elementos de Cálculo vectorial
1.1.

Álgrebra de Vectores en R3

Esta es una lista de identidades elementales del álgebra vectorial, que se supondrán bien
conocidas
⃗·B
⃗ = Ax Bx + Ay By + Az Bz
A
⃗×B
⃗ = (Ay Bz − Az By ) î + (Az Bx − Ax Bz ) ĵ + (Ax By − Ay Bz ) k̂
A
⃗×A
⃗=0
A
!
"
⃗· A
⃗×B
⃗ =0
A

!
" !
"
⃗
⃗
⃗
⃗
⃗
⃗
A· B×C = A×B ·C

!
" !
"
!
"
⃗× B
⃗ ×C
⃗ = A
⃗·C
⃗ B
⃗− A
⃗·B
⃗ C
⃗
A

1.2.

Cálculo diferencial en R3

Sea f : [R3 ] → R una función real. También es llamada campo escalar, pues a cada punto
del espacio (R3 ) le asocia un número real (un escalar). Ejemplo de un campo escalar puede ser
la temperatura en cierta región del espacio T : [Ω ⊆ R3 → R]

Fig. 1.1: T (x, y, z) representa un campo escalar sobre Ω
Además de la existencia de campos escalares, también existen campos vectoriales. La
idea es bien simple, a cada punto del espacio se le asocia un vector. En R3 , el tipo de campos
vectoriales que nos interesarán son de la forma F⃗ : [Ω ⊆ R3 ] → R3 .

---

### Página 6

Fig. 1.2: La velocidad de los átomos de un objeto que rota es un ejemplo de campo vectorial

1.2.1.

Derivadas de un campo escalar

Si f es un campo escalar diferenciable (y por lo tanto una función continua) sobre un
dominio D ⊆ R3 , entonces está definido el Gradiente de f
#
$
∂f (x, y, z) ∂f (x, y, z) ∂f (x, y, z)
⃗
∇f (x, y, z) =
+
+
∂x
∂y
∂y

El gradiente es un campo vectorial, pues a cada punto en D le asocia un vector. Es
inmediato notar que el gradiente es perpendicular a curvas en donde el campo escalar f es
constante, como las curvas que se muestran en la figura 1. (Llamadas isotermas en el caso de
que el campo escalar sea la temperatura). En efecto, la curva
f (x, y, z) = C
puede ser parametrizada
f (x(t), y(t), z(t)) = C

Derivando con respecto a t, se obtiene
∂f ′
∂f ′
∂f ′
x (t) +
y (t) +
z (t) = 0
∂x
∂y
∂z
#

∂f (x, y, z) ∂f (x, y, z) ∂f (x, y, z)
+
+
∂x
∂y
∂y

$

· (x′ (t), y ′ (t), z ′ (t)) = 0

y entonces el gradiente es perpendicular a la dirección tangente a la curva. Más aún, si û es
un vector unitario, se define la derivada direccional de f en la dirección û como
⃗ (x, y, z) · û
Dû f (x, y, z) = ∇f
Se puede demostrar que la derivada direccional se maximiza en la dirección del gradiente,
es decir, el gradiente entrega la dirección de máxima variación de f .

---

### Página 7

1.3.

⃗ como un operador
∇

Conviene considerar al gradiente como algo independiende de que función se está derivando.
⃗ al operador
Llamamos ∇
#
$
∂
∂
∂
⃗ =
∇
, ,
∂x ∂y ∂z
⃗ debe operar
Por supuesto que este operador así escrito no significa nada. El operador ∇
sobre una función, por ejemplo
$
#
∂f ∂f ∂f
⃗
,
,
∇f =
∂x ∂y ∂z

Tiene completo sentido en este caso. Hemos ”multiplicado” al operador por una cantidad
escalar. Hay que tener ciertas precauciones con este tipo de notación, por ejemplo, del álgebra
de vectores es sabido que si α es un escalar
⃗ = Aα
⃗
αA
⃗ no tiene sentido por si mismo, en efecto, es un nuevo operador
sin embargo, f ∇
#
$
∂
∂
∂
⃗
f∇ = f , f , f
∂x ∂y ∂z

1.3.1.

Divergencia y Rotor

Si F⃗ es un campo vectorial, entonces
⃗ · F⃗
∇
⃗ como un
debe ser un escalar, y por lo tanto puede tener un sentido físico. Entendiendo ∇
operador vectorial, se tiene
#
$
∂ ∂ ∂
⃗
⃗
∇·F =
, ,
· (Fx , Fy , Fz )
∂x ∂y ∂z
⃗ · F⃗ = ∂ Fx + ∂ Fy + ∂ Fz
∇
∂x
∂y
∂z
A esta cantidad escalar asociada a un campo vectorial se le llama divergencia de F⃗ .
⃗ × F⃗ ?.
Veamos que más es posible definir a partir del operador gradiente. ¿Qué ocurre con ∇
Por supuesto que el resultado debe ser un campo vectorial, de hecho, muy útil en el análisis de
funciones vectoriales. Desarrollando este producto cruz según el álgebra de vectores
!

⃗ × F⃗
∇

"

!

⃗ × F⃗
∇

"

!

⃗ × F⃗
∇

x

y

=

∂Fz ∂Fy
−
∂y
∂z

=

∂Fx ∂Fz
−
∂z
∂x

∂Fy ∂Fx
−
∂x
∂y
z
A esta combinación se le llama rotor. En resumen, hemos definido las siguientes cantidades
"

=

---

### Página 8

⃗ → Vector
∇f
⃗ · F⃗ → Escalar
∇

⃗ × F⃗ → Vector
∇

---

### Página 9

1.3.2.

Segundas derivadas

Hasta ahora hemos definido cantidades que involucran únicamente primeras derivadas.
Veamos que ocurre con las siguientes combinaciones
! "
⃗ · ∇f
⃗
(a)∇
! "
⃗ × ∇f
⃗
(b)∇
!
"
⃗ ∇
⃗ · F⃗
(c)∇
!
"
⃗ · ∇
⃗ × F⃗
(d)∇

!
"
⃗
⃗
⃗
(e)∇ × ∇ × F
Veamos la primera de ellas, es claro que debe obtenerse un campo escalar. Desarrollando
#
$
! "
∂f ∂f ∂f
⃗
⃗
⃗
∇ · ∇f = ∇ ·
,
,
∂x ∂y ∂z
! " ∂2f
∂2f
∂2f
⃗ · ∇f
⃗
=
∇
+
+
∂x2
∂y 2
∂z 2
Se ve que esto se puede reescribir como
! "
!
"
⃗
⃗
⃗
⃗
⃗
⃗
⃗ 2f
∇ · ∇f = ∇ · ∇f = ∇ · ∇ f = ∇

⃗ 2 como un nuevo operador, y como aparece mucho en física, tiene un nombre. Es
Vemos a ∇
llamado Laplaciano
∂2
∂2
∂2
+
+
∂x2 ∂y 2 ∂z 2
debido a que el Laplaciano es un operador escalar, podría aplicarse sobre un vector
⃗2=
Laplaciano → ∇

⃗ 2 F⃗
∇
por supuesto esto significa que el operador Laplaciano opera sobre cada componente de F⃗
"
!
⃗ 2 Fx , ∇
⃗ 2 Fy , ∇
⃗ 2 Fz
⃗ 2 F⃗ = ∇
∇
Veamos que ocurre con la expresión (b). Notemos que tiene la siguiente forma
"
! " !
⃗
⃗×A
⃗ f =0
⃗ × Af
A
= A
Esperamos que

! "
⃗
⃗ × ∇f
∇

sea cero para cualquier campo escalar f . Podemos verificarlo tomando alguna de las componentes

---

### Página 10

! "
! "
⃗
⃗
⃗
⃗
⃗
⃗
[∇ × ∇f ]x = ∇z ∇f − ∇y ∇f
y

⃗ × ∇f
⃗ ]x =
[∇

∂
∂z

#

∂f
∂y

$

−

∂
∂y

#

∂f
∂z

Del mismo modo se muestra para las demás componentes

$

z

=0

La expresión (c) es por supuesto un campo vectorial
!
"
⃗ ∇
⃗ · F⃗
∇

Sin embargo, no hay nada muy especial que decir acerca de él. Es simplemente un campo
vectorial que podría aparecer en el futuro
La expresión (d) tiene la forma

Es decir, esperamos que

!
"
⃗· A
⃗×B
⃗ =0
A
!
"
⃗ · ∇
⃗ × F⃗ = 0
∇

Para cualquier campo vectorial F⃗ . Es así, y es fácil de verificar
Por último, veamos que sucede con la expresión (e)
"
!
⃗ × F⃗
⃗ × ∇
∇

Ésta tiene la forma de

"
"
!
" !
!
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
A× B×C =B A·C − A·B C

Podríamos seguir utilizando esta expresión y escribir
!
"
!
" !
"
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
∇ × ∇ × F = ∇ ∇ · F − ∇ · ∇ F⃗
El último término es el Laplaciano
!
"
!
"
⃗
⃗
⃗
⃗
⃗
⃗
⃗ 2 F⃗
∇× ∇×F =∇ ∇·F −∇

En resumen, hemos encontrado
! "
⃗
⃗
⃗ 2 f → Laplaciano sobre f, campo escalar
∇ · ∇f
=∇

! "
⃗
⃗
∇ × ∇f
=0
"
!
⃗ · F⃗ → Campo vectorial
⃗ ∇
∇
!
"
⃗ · ∇
⃗ × F⃗ = 0
∇
!
"
!
"
⃗ × F⃗ = ∇
⃗ · F⃗ − ∇
⃗ × ∇
⃗ ∇
⃗ 2 F⃗ → campo vectorial
∇

---

### Página 11

1.3.3.

Dos teoremas adicionales

En muchos problemas físicos, sucede que un determinado campo vectorial F⃗ tiene rotor
nulo. Es decir
⃗ × F⃗ = 0
∇

Hemos visto que el rotor de un gradiente es siempre cero. Podría ser ciento entonces, que
F⃗ fuera el gradiente de algún campo escalar, de esta forma su rotor sería siempre nulo. Lo
interesante es que esto es siempre así, y enunciaremos el siguente teorema
Si
Existe un campo escalar ψ, tal que

⃗ × F⃗ = 0
∇
⃗
F⃗ = ∇ψ

Del mismo modo, hemos visto que la divergencia de un rotor es siempre cero. Luego, si la
divergencia de un campo vectorial F⃗ es nula, podria tenerse que F⃗ fuera el rotor de un campo
vectorial. De ser así, estaría garantizado que su divergencia sea nula. En efecto, enunciamos el
segundo teorema
Si
⃗ tal que
Existe un campo vectorial A,

⃗ · F⃗ = 0
∇
⃗ ×A
⃗
F⃗ = ∇

1.4.

Cálculo Integral en R3

1.4.1.

Integral de línea de un campo vectorial

Sea F⃗ : [Ω ⊆ R3 ] → R3
Consideremos una curva Γ contenida en Ω. Sea ⃗x0 , ⃗x1 , ...⃗xn una partición de Γ, (xk , yk ) un
punto en el trazo de Γ que va de ⃗xk−1 a ⃗xk , y ∆⃗xk = ⃗xk − ⃗xk−1 . Se define la integral de línea
de F⃗ (⃗x) por
ˆ
d⃗x · F⃗ (⃗x) = lím F⃗ (xk , yk ) · ∆⃗xk
n→∞

Γ

Esto se puede reescribir como
ˆ
ˆ
∆⃗xk
⃗
⃗
d⃗x · F (⃗x) = lím F (xk , yk ) ·
| ∆⃗xk |= dsT̂ (⃗x) · F⃗ (⃗x)
n→∞
| ∆⃗xk |
Γ
Γ
donde T̂ (⃗x) es la tangente unitaria a la curva Γ en ⃗x. Así
ˆ
ˆ
⃗
d⃗x · F (⃗x) = dsT̂ (⃗x) · F⃗ (⃗x)
Γ

Γ

La integral de línea de un campo vectorial sobre una curva Γ corresponde a sumar las
proyeccciones de F⃗ (⃗x) en la dirección tangente a la curva en todo punto.

---

### Página 12

1.4.2.

Integral de superficie de un campo vectorial

Sea F⃗ : [Ω ⊆ R3 ] → R3 y S una superficie contenida en Ω. Se define la integral de flujo del
campo F⃗ sobre S como
¨
¨
⃗ x) · F⃗ (⃗x) =
dS(⃗
dS(⃗x)n̂(⃗x) · F⃗ (⃗x)
S

S

corresponde a sumar la proyección del campo F⃗ sobre la normal a la superficie S en cada
punto.

1.4.3.

Teorema de la Divergencia

Sea Ω ⊆ R3 una región. Sea F⃗ un campo vectorial continuo y diferenciable en Ω. Entonces
ˆˆ
˚
✞☎ ⃗
3 ⃗
⃗
x) · F⃗ (⃗x)
d x∇ · F = ✝ ✆ dS(⃗
δΩ

Ω

1.4.4.

Teorema de Stokes

Sea S una superficie en R3 . Sea F⃗ un campo vectorial continuo y diferenciable en una región
que contiene a S. Entonces
¨
!
" ˛
⃗
⃗
⃗
dS(⃗x) · ∇ × F (⃗x) =
d⃗x · F⃗ (⃗x)
S

δS

donde δS es el contorno de S (una curva en R )

---

### Página 13

#### Capítulo 2
Introducción
Este curso trata sobre los fundamentos de la teoría Electromagnética, una teoría realmente
exitosa y que es capaz de explicar y predecir una gran cantidad de fenómenos. Una de las
dificultades en su construcción fue la gran cantidad de fenómenos complejos, que en un principio
aparentemente no tenían relación unos con otros. Sin embargo uno de los mayores logros de
la electrodinámica es mostrar que en realidad están todos relacionados, además de permitir la
creación de nuevas aplicaciones, que no aparecen de forma inmediata en la naturaleza y que
han cambiado la vida de todo el mundo. Absolutamente toda la teoría se encuentra resumida
en un conjunto de cuatro ecuaciones diferenciales, llamadas Ecuaciones de Maxwell

Éstas 4 ecuaciones resumen todos los resultados empíricos acumulados durante años por
los estudios de los físicos Coulomb, Gauss, Ampère, Faraday y muchos otros. Fueron presentadas en 1873 por el matemático inglés James Clerk Maxwell1 . Además de explicar todos
los fenómenos eléctricos y magnéticos conocidos hasta la época, muestran que electricidad y
magnetismo no son fenómenos independientes, y explica la forma en como ambos se relacionan.
Las ecuaciones de Maxwell fueron capaces de predecir la creación de ondas electromagnéticas
de energía cuya velocidad de propagación teórica coincidía con la velocidad de la luz (hecho que
corroboró Heinrich Hertz en 1887). Hoy se sabe que la luz es un tipo de onda electromagnética,
luego, todas las leyes de la óptica, también son explicadas de forma consistente por las ecuaciones de Maxwell. Esto fue un gran suceso pues logró mostrar que fenómenos que parecían
totalmente diferentes provenían de los mismos principios físicos. Radiación infraroja, luz visible, radiación ultravioleta, rayos x, rayos gama, son todos diferentes tipos de ondas oscilatorias,
y sólo se diferencian en sus frecuencias. Todas reciben el nombre de radiación, debido a que
propagan (irradian) energía.
En este curso se pretenden desarrollar las bases empíricas para las ecuaciones de Maxwell,
⃗ y magnético B.
⃗
mediante la introducción del campo eléctrico E

A Dynamical Theory of the Electromagnetic Field, James Clerk Maxwell

---

### Página 14

Primeramente estudiaremos el caso estático, en donde los campos no tienen dependencia
temporal. En este caso las ecuaciones de Maxwell se transforman en:
⃗ ·E
⃗ = ρ
∇
ϵo
⃗ ×E
⃗ =0
∇

⃗ ·B
⃗ =0
∇
⃗ ×B
⃗ = µo J⃗
∇
Notemos que ahora hay 2 ecuaciones para cada campo totalmente independientes entre sí, en
otras palabras, electricidad y magnetismo son fenómenos absolutamente independientes mientras los campos sean estáticos. Las dos primeras ecuaciones corresponden a la Electrostática,
mientras que las 2 últimas a la Magnetostática. Desarollaremos las ideas y principios fundamentales de ambos casos estáticos, para luego estudiar los campos variantes en el tiempo y
derivar las ecuaciones de Maxwell.

Fig. 2.1: James Clerk Maxwell
James Maxwell (1831-1879) Físico Escocés. Es el creador de la electrodinámica moderna
y el fundador de la teoria cinética de los gases. Sus teorías constituyeron el primer intento de
unificar dos campos de la física que, antes de sus trabajos, se consideraban completamente
independientes: la electricidad y el magnetismo (conocidos como electromagnetismo). Además,
en el año 1859 Maxwell formuló la expresión termodinámica que establece la relación entre la
temperatura de un gas y la energía cinética de sus moléculas.

---

### Página 15

#### Capítulo 3
Electrostática
Una de las propiedades fundamentales de la materia corresponde a lo que se conoce como
carga eléctrica. Esta propiedad es el origen de las fuerzas eléctricas. Considere un sistema de
dos cargas puntuales y en reposo, q1 y q2 , separadas por una distancia r en el vacío. Por dos
cargas puntuales, nos referimos por supuesto a objetos cuyo diámetro máximo es muchísimo
menor que la separación entre ellos.
Las fuerza entre cargas estáticas fue estudiada por Charles Augustin de Coulomb, (Físico e
Ingeniero francés), encontrando una gran similitud entre la forma de las fuerzas electrostáticas
y las de gravitación, pero notando que, a diferencia de la fuerza gravitacional, las fuerzas
electrostáticas también pueden ser repulsivas.

Fig. 3.1: Fuerza entre cargas puntuales puede ser repulsiva y atractiva
La fuerza que ejerce q ′ sobre q está dada por la ley de Coulomb
F⃗q =

qq ′
(⃗x − ⃗x′ )
4πϵ0 | ⃗x − ⃗x′ |3

---

### Página 16

Es decir, la fuerza electrostática es proporcional al producto de las cargas e inversamente
proporcional al cuadrado de la distancia entre ellas. Notar que la dirección
(⃗x − ⃗x′ )
| ⃗x − ⃗x′ |
va siempre desde la carga q ′ hacia la carga q. El signo de la fuerza estará determinado entonces
por el producto de las cargas, así, si ambas son iguales, la fuerza será repulsiva, mientras que
si son de signo opuesto, la fuerza será atractiva.
En el sistema S.I., la constante de proporcionalidad está dada por
= 8, 9875 × 109 N m2 /C 2
4πϵo
Donde ϵ0 se conoce como la permitividad del vacío.
K=

Similarmente, la fuerza sobre q ′ debido a q está dada por F⃗q′ = −F⃗q , como debe ser por la
tercera ley de Newton. La ley de Coulomb describe perfectamente las fuerzas entre 2 cargas
puntuales, luego, resulta de interés estudiar qué sucede cuando hay más de dos cargas presentes.
Supongamos que existen N cargas qj con j = 1, 2, ...N . Supongamos que hay una carga q en
la posición ⃗x y que la posición de la carga qj es ⃗xj . La fuerza que ejercen las N cargas sobre q
está dada por el principio de superposición
F⃗q =

N
%
qqj
(⃗x − ⃗xj )
4πϵ
|
⃗
x
−
⃗
x
|
j
j=1

Es decir, la suma de cada fuerza por separado. El principio de superposición implica que la
fuerza neta entre 2 cargas es independiente de la prescencia de otras cargas. Esto es cierto
siempre y cuando las cargas estén en posiciones fijas (recordar que son fuerzas electrostáticas).
Podrán notar inmediatamente, que como estamos considerando cargas estáticas que se ejercen
fuerzas entre sí, deben necesariamente existir fuerzas externas que las mantengan en equilibrio.
Supondremos entonces que las cargas están forzadas a mantenerse en su posición, de forma que
las leyes que hemos establecido hasta ahora son válidas.

Fig. 3.2: Charles-Augustin de Coulomb (1736-1806)

---

### Página 17

3.1.

Campo Eléctrico

La fuerza electrostática, como la fuerza gravitacional, es una fuerza que actúa a distancia, es decir, no requiere que los objetos estén en contacto entre sí. Entonces, si tenemos 2
cargas puntuales, digamos, q y q0 , podemos medir la fuerza que ejerce q sobre q0 . A q0 se le
llamará carga de prueba, y la posicionaremos en diferentes lugares del espacio y mediremos
la fuerza que siente debido a la presencia de la carga fija q. En este sentido, se piensa que
q genera algo en todo el espacio que debe ser independiente de si colocamos o no la carga
de prueba q0 . Se dice que una carga eléctrica genera un campo eléctrico (matemáticamente
descrito por un campo vectorial) en todo el espacio, el cual es capaz de actuar sobre otras cargas.
Justamente para cuantificar la magnitud del campo creado por la carga, podemos medir la
fuerza que experimenta una carga positiva de prueba qo en algún punto del espacio.
⃗ se define formalmente como
El campo eléctrico E
⃗
⃗ = lím Fq0
E
q0 →0 q0
Es decir, el campo existe en todo el espacio y es independiente de la carga de prueba. La
sutileza de elegir una carga de prueba infinitamente pequeña es para que el campo producido
por q0 no altere de ninguna forma a la fuente del campo que queremos cuantificar.

Diremos entonces con este nuevo enfoque que la carga q es una fuente (crea) un campo
⃗ que ejerce una fuerza F⃗q0 = q0 E(⃗
⃗ x) sobre una carga q0 ubicada en ⃗x
eléctrico E
Usando la definición de Campo Eléctrico y la Ley de Coulomb, se obtiene que el campo eléctrico
a una distancia r de la carga puntual q está dado por
1 q
r̂
4πϵ0 r2
donde r̂ es la dirección radial desde la carga q
⃗ =
E

⃗ para una carga positiva(izq) y negativa
Fig. 3.3: Representación gráfica del campo vectorial E
(der)

---

### Página 18

Lógicamente, el principio de superposición es también válido para el campo eléctrico, bajo
las mismas condiciones mencionadas anteriormente. Así, el campo en ⃗x de una distribución
discreta de N cargas puntuales ubicadas en qj ,j = 1, 2, ...N está dado por
⃗ x) =
E(⃗

N
%
qj
(⃗x − ⃗xj )
4πϵ0 | ⃗x − ⃗xj |3
j=1

(3.1)

La ley de Coulomb y el principio de superposición son las leyes empíricas fundamentales
de la Electrostática. Más adelante, veremos que las ecuaciones de Maxwell para el campo
Electrostático
⃗ · E(⃗
⃗ x) = ρ
∇
ϵ0
⃗ × E(⃗
⃗ x) = 0
∇
contienen exactamente la misma información que acabamos de presentar (y por supuesto, contienen muchísima información adicional!), pero de una forma mucho más general, simple y
elegante.

3.2.

Distribuciones continuas de carga - Integrales de
Coulomb

Se pueden extender estas ideas para cuando se tiene una gran cantidad de cargas distribuídas
en una región del espacio. Supongamos una distribución continua de carga encerrada en un
volumen V , por ésto entendemos una región del espacio en donde se puede definir una densidad
volumétrica de carga en cada punto, digamos ρ(⃗x) (C / m3 )

En el caso de obtener una distribución continua de carga, se utiliza una partición del volumen
V en celdas de volumen infinitesimal d3 x′ . En la posición ⃗x′ , se encuentra un pequeño volumen
con carga dada por
dq(⃗x′ ) = d3 x′ ρ(⃗x′ )
Como esta es una carga infinitesimal, el campo que genera en ⃗x será el de una carga puntual
⃗ x′ ) =
dE(⃗

d3 x′ ρ(⃗x′ ) ⃗x − ⃗x′
4πε0 | ⃗x − ⃗x′ |3

---

### Página 19

Para obtener el campo generado por toda la distribución de carga, basta con sumar (integrar)
sobre el volumen V las contribuciones individuales de cada elemento de volumen, luego
⃗ x) = 1
E(⃗
4πϵ0

d3 x′ ρ(⃗x′ )
(⃗x − ⃗x′ )
′ |3
|
⃗
x
−
⃗
x
V

˚

En el caso de obtener una superficie S de carga, en donde para cada ⃗x′ en S se tiene
una densidad superficial de carga (que denotaremos σ(⃗x′ ) para diferenciarla de una densidad
volumétrica), se obtiene
¨
ds′ σ(⃗x′ )
⃗
E(⃗x) =
(⃗x − ⃗x′ )
4πϵ0 S | ⃗x − ⃗x′ |3
Por último, para una distribución lineal Γ, en donde para cada ⃗x′ en Γ se tiene una densidad
lineal de carga, denotada λ(⃗x′ ) entonces el campo en ⃗x está dado por
ˆ
dx′ λ(⃗x′ )
⃗
E(⃗x) =
(⃗x − ⃗x′ )
′
4πϵ0 Γ | ⃗x − ⃗x |
Éstas son las integrales de Coulomb y son una extensión al caso de una distribución discreta
de cargas, a distribuciones continuas en el espacio
Ejemplo: Campo de un anillo de carga
Consideremos un anillo con densidad lineal de carga constante y dada por λ. El objetivo es
calcular el campo eléctrico generado por esta distribución de carga en un punto sobre el eje de
simetría a distancia z del origen

Un elemento diferencial de longitud sobre el anillo está dado por dl = Rdφ donde φ es el
ángulo polar. Este elemento posee una carga dq = λdl = λRdφ, de forma que el campo eléctrico
en un punto ⃗x debido a esta carga infinitesimal está dado por la ley de Coulomb
′
′
⃗ x) = dq ⃗x − ⃗x = dφRλ ⃗x − ⃗x
E(⃗
4πϵ0 | ⃗x − ⃗x′ |3
4πϵ0 | ⃗x − ⃗x′ |3

donde ⃗x′ es la posición del elemento de carga, en este caso
!
"
⃗x′ = Rr̂ = R cos φî + sin φj

---

### Página 20

de forma que el campo total se obtiene integrando sobre todo el anillo (abarcando todo el
rango de φ)
⃗ x) = R
E(⃗
4πϵ0

ˆ 2π

dφ

⃗x − Rr̂
| ⃗x − Rr̂ |3

ahora, se desea el campo en un punto sobre el eje simetría del anillo, a distancia z del origen,
de forma que
⃗x = z k̂
y queda
⃗ k̂) = R
E(z
4πϵ0

ˆ 2π

dφ

por supuesto que

z k̂ − Rr̂

| z k̂ − Rr̂ |3

&
'1/2
| z k̂ − Rr̂ |= z 2 + R2
⃗ k̂) = R
E(z
4πϵ0

ˆ 2π

z k̂ − R cos φî − R sin φĵ

dφ

(z 2 + R2 )3/2

De estas tres integrales (en î, ĵ, k̂), la única que no es nula es la según k̂. Esto es fácil de
ver apelando a la simetría de la distribución de carga

⃗ k̂) = Rz
E(z
4πϵ0

ˆ 2π

dφ

(z 2 + R2 )3/2

k̂

z
⃗ k̂) = 2πR
E(z
k̂
4πϵ0 (z 2 + R2 )3/2
esto se puede escribir de otra forma considerando que Q = 2πRλ es la carga total del anillo
z
⃗ k̂) = Q
k̂
E(z
4πϵ0 (z 2 + R2 )3/2

---

### Página 21

Si z es suficientemente grande en comparación con las dimensiones del anillo (z >> R),
entonces
⃗ k̂) ≈ Q k̂
E(z
4πϵ0 z 2
que sería el campo a distancia z de una carga puntual Q en el origen

---

### Página 22

Problema
Dos pequeñas esferas de igual masa m y carga q, cuelgan por 2 hilos sin masa, sin carga y de
largo l. Cada esfera forma un ángulo ϑ con el eje vertical, como se muestra en la figura

Calcule la carga q
#### Solución
Debido a la simetría del sistema, bastará con hacer análisis de fuerzas para una de las cargas.
Consideramos el equilibrio entre las tres fuerzas que actúan: la fuerza de repulsión (las dos
cargas son de igual signo) electrostática Fe , la tensión sobre el hilo T , y la fuerza gravitacional
mg.

De la segunda ley de Newton para la esfera
Fx = T sinϑ − F e = max = 0
Fy = T cosϑ − mg = may = 0

Como el sistema se encuentra en equilibrio, ax = ay = 0, entonces la primera ecuación
equivale a
T sin ϑ =

q2
4πε0 r2

donde r es la separación entre las 2 cargas
q 2 = 4πε0 T sin ϑr2
O equivalentemente,
q = ±r

(
4πε0 T sin ϑ

---

### Página 23

Del equilibrio de fuerzas para el eje vertical obtenemos
T =

mg
cosθ

Y además, r = 2l sin ϑ. Finalmente se obtiene
qeq = ±2lsinϑ

(
(
4πε0 mgtgϑ = ±4lsinϑ πϵ0 mgtanϑ

---

### Página 24

Problema
Se tiene una línea homogénea de carga con densidad lineal λ, y de longitud finita a. Calcular
el campo eléctrico en el punto P a distancia x del extremo

#### Solución
Tomamos un pequeño elemento dµ de la línea de carga, situado a una distancia µ del punto A,
y obtenemos el campo eléctrico en el punto P debido a este elemento diferencial
⃗ )=
dE(P

λdµ
î
4πϵ0 (a + x − µ)2

Y el campo eléctrico total se obtiene integrando para toda la línea de carga. Esto es

⃗ )=
E(P

4πϵ0

ˆ a

λdµ
î
(a + x − µ)2

Sea z = a + x − µ, así, dz = −dµ y el campo queda
⃗ = −λ
E
4πϵ0

ˆ x

#
$
dz
λ 1 ))x
λ
λ
î =
−
î
) î =
4πϵ0 z a+x
4πϵ0 x 4πϵ0 (a + x)
a+x z

λa
Q
⃗ = λ(x + a) − λx î =
î =
î
E
4πϵ0 x(x + a)
4πϵ0 x(x + a)
4πϵ0 x(x + a)
Con Q la carga total de la línea.
Notar que si x ≫ a

⃗ ≈
E

Q
î
4πε0 x2

que concuerda con el campo de una carga puntual

---

### Página 25

Problema
Una barra delgada con densidad de carga uniforme λ se dobla con la forma de un arco de
círculo de radio R. El arco subiende un ángulo total 2ϑ0 , simétrico con respecto al eje x, como
⃗ en el origen O?. Vea que sucede cuando
se muestra en la figura. ¿Cuál es el campo eléctrico E
ϑ0 → π

#### Solución
Considere un elemento diferencial de longitud dl = Rdϑ, que forma un ángulo ϑ con respecto
al eje x. La cantidad de carga que contiene este elemento es dq = λdl = λRdθ

Su contribución al campo eléctrico en O es
⃗ =−
dE

1 dq
1 dq
1 λdϑ
(− cos ϑî − sin ϑĵ)
r̂ =
(− cos ϑî − sin ϑĵ) =
4πϵ0 r
4πϵ0 R
4πϵ0 R

Integrando para ϑ entre −ϑ0 y ϑ0 , se obtiene
ˆ
1 λ ϑ0
⃗
dϑ(− cos ϑî − sin ϑĵ)
E=
4πϵ0 R −ϑ0

⃗ =
E

) ϑ0
1 λ
1 2λ sin ϑ0
)
(− sin ϑî + cos ϑĵ))
î
=−
4πϵ0 R
4πϵ0
R
−ϑ0

Vemos que el campo eléctrico solo tiene componente en el eje x, lo que concuerda con la
simetría del problema.

---

### Página 26

Si tomamos el límite cuando θ0 → π, el arco se transforma en un anillo circular. Ya que
sin θ = 0, la ecuación anterior implica que el campo eléctrico en el centro de un anillo de carga
es nulo. Esto se esperaría por argumentos de simetría. (Comparar además con el campo de un
anillo de carga calculado en este capítulo)
Por otro lado, para ángulos muy pequeños, sin ϑ0 ≈ ϑ0 , recuperamos el caso de una carga
puntual
⃗ ≈ − 1 2λθ0 î = − 1 2λϑ0 R î = − 1 Q î
E
4πϵ0 R
4πϵ0 R2
4πϵ0 R2
Donde la carga total del arco es Q = λl = λ(2Rϑ0 )

---

### Página 27

Problema
Un recipiente hemisférico no conductor de radio interior a tiene una carga total Q repartida
uniformemente en su superficie interior. Encuentre el campo eléctrico en el centro de curvatura

#### Solución
Tomamos como origen el centro de curvatura de la semiesfera. A partir de esto podemos determinar la contribución de un elemento diferencial de carga en la superficie al campo eléctrico
⃗ por
en el eje que pasa por el centro de curvatura, que coincide con la direccion k̂ (El campo E,
simetría, solo tendrá componente en k̂).

⃗ x) =
dE(⃗

1 (⃗x − ⃗x′ )
σds′
4πϵ0 |⃗x − ⃗x′ |3

Un elemento diferencial de superficie sobre la esfera está dado por
ds = a2 sin ϑdϑdφ
y como la carga está distribuída uniformemente, la densidad superficial es simplemente
σ=

Q
2πa2

Con esto, podemos determinar el campo total integrando sobre toda la superficie
ˆ π
ˆ
Q (⃗x − ⃗x′ )
1 2 2π
⃗
a
dφ
dϑ sin ϑ
E(⃗x) =
4πϵ0
2πa2 |⃗x − ⃗x′ |3
π/2
Evaluando en ⃗x= 0 obtenemos el campo en el centro de curvatura
ˆ 2π ˆ π
Q
−⃗x′ 2
⃗
E(0) =
a sin ϑdθdφ
4πϵ0 0
x′ |3
π/2 2πa | − ⃗

⃗
E(0)
=

4πϵ0

ˆ 2π

Q
2πa2

ˆ π

−⃗x′ 2
a sin ϑdθdφ
x′ |3
π/2 | − ⃗

El vector ⃗x′ que recorre la superficie está dado por
⃗x′ = a cos ϑk̂ + a sin ϑ cos φî + a sin ϑ sin φĵ

---

### Página 28

Por el argumento de simetría, solo interesa la componente según k̂. De todas formas se
puede verificar calculando explícitamente las integrales en î y ĵ . Con esto
ˆ π
Q
−a cos ϑ 2
⃗
E(0) =
a sin ϑdϑk̂
4ϵ0 πa π/2
a3
ˆ π
ˆ π
Q
Q
⃗
E(0) =
− cos ϑ sin ϑdϑk̂ =
− sin(2ϑ)dϑk̂
4ϵ0 πa2 π/2
8ϵ0 πa2 π/2
Finalmente el campo en el centro de curvatura es
⃗
E(0)
=

Q
k̂
8ϵ0 πa2

---

### Página 29

Problema
Considere un alambre muy delgado como el de la figura, éste está compuesto por dos rectas
infinitas y un arco de círculo de 135 grados. El alambre tiene una densidad lineal de carga λ
constante. Encuentre el campo eléctrico producido en el punto P

#### Solución
Este problema se resuelve mediante integrales de Coulomb y el principio de superposición.
Descomponemos el problema en subproblemas más simples, una distribución de carga lineal y
otra en un arco de círculo (ya visto en el problema anterior). Resolvamos entonces el problema
de una distribución lineal infinita de carga

Un elemento de longitud dx′ a distancia x′ del origen genera una contribución al campo en
P dada por
′
′
⃗ ) = dx λ ⃗x − ⃗x
dE(P
4πε0 | ⃗x − ⃗x′ |3
donde ⃗x = Rĵ es el vector posición del punto P , y ⃗x′ = x′ î el vector que recorre la distribución
de carga (parámetro x′ ). Por el principio de superposición, el campo eléctrico en P se obtiene
sumando sobre toda la distribución
⃗ )=
E(P

λ
4πε0

ˆ ∞

dx′

Rĵ − x′ î

(x′2 + R2 )3/2
ˆ ∞
ˆ ∞
λ
Rλ
x′
dx′
′
⃗
E(P ) = −
dx
î
+
ĵ
4πε0 0
4πε0 0 (x′2 + R2 )3/2
(x′2 + R2 )3/2

Calculemos primero la integral
I1 =

ˆ ∞

dx′ x′
(x′2 + R2 )3/2

con el trivial cambio de variable u = x′2 , du = 2x′ dx′

---

### Página 30

I1 =

ˆ ∞

=
3/2
(u + R2 )
du

ˆ ∞

2 −3/2

du(u + R )

I1 =
Ahora, obtenemos
I2 =

ˆ ∞

R

)∞
2 −1/2 )
= −2 ∗ (u + R )
)

dx′
(x′2 + R2 )3/2

y utilizamos la conocida sustitución x′ = R tan ϑ, dx′ = Rsec2 ϑdϑ. Con esto la integral
queda de la forma
I=

ˆ

dϑRsec2 ϑ
=
(R2 tan2 ϑ + R2 )3/2

ˆ

dϑRsec3 ϑ
= 2
R sec ϑ
R

I=

ˆ

dϑ
= 2
secϑ
R

ˆ

dϑ cos ϑ

sin ϑ
R2

Utilizando que x′ /R = tan ϑ
sin ϑ = √

x′
x′2 + R2

de forma que
I2 =

)∞
x′
x′
)
√
√
=
lím
)
R2 x′2 + R2 0
R2 x′ →∞ x′2 + R2

I2 =

*
lím
= 2
′
R x →∞
R
12 + (R/x′ )2

Luego el campo eléctrico debido al alambre en el punto P es
⃗ 1 (P ) =
E

4πε0

#

−λ
λ
î + ĵ
R
R

$

√ #
$
λ
⃗ 1 (P ) =
√ (−î + ĵ)
E
4πε0 R

La contribución del sector de arco de círculo ya fue obtenida en un problema anterior, uego
es inmediato que
⃗ 2 (P ) =
E

2λ
sin
4πε0 R

#

3π

$

î

---

### Página 31

Finalmente, el campo total en P se obtiene por superposición. Veamos que ocurre con el
campo que produce el segmento rectilíneo superior

⃗ 1 en P forma un ángulo de 3π/8 con la horizontal. De esta forma, la superposición
El campo E
de los 3 campos es como sigue

⃗ )=
E(P

⃗ )= 1
E(P
4πε0

⃗ )=
E(P

#

#

⃗ 2 | −2 | E
⃗ 1 | cos
|E

#

3π

$

#

#

$

sin

3π

3π

$$

λ√
2 cos
−2
R

2λ
sin
R

λ
2πε0 R

#

−

√

2 cos

#

î

#

3π

3π

$$

$$

î

î

---

### Página 32

Problema
Se pide calcular el campo eléctrico a distancia r del centro de una distribución uniforme de
carga ρ0 localizada dentro de una esfera de radio R, mediante la integral de Coulomb, o sea,
calcule
˚
⃗x − ⃗x′
ρ
⃗ x) =
E(⃗
d3 x′
4πε0
| ⃗x − ⃗x′ |3
V
puesto que
+
ρ0 si | ⃗x′ |≤ R
′
ρ(⃗x ) =
0 si | ⃗x′ |> R
para r > R

#### Solución
Ubiquemos el centro de la esfera en el origen

Sea ⃗x un punto a distancia r del origen
⃗x = rr̂
y ⃗x′ un punto dentro de la distribución de carga
⃗r′ = r′ r̂′
El campo eléctrico está dado por la integral de Coulomb sobre la distribución de carga
˚
˚
x − ⃗x′
⃗x − ⃗x′
ρ0
3 ′
′
3 ′ ⃗
⃗
E(⃗x) =
d x ρ(⃗x )
=
d
x
4πε0
| ⃗x − ⃗x′ |3
4πε0
| ⃗x − ⃗x′ |3
V
V

⃗ x) = ρ0
E(⃗
4πε0

ˆ 2π

′

dφ

ˆ π

′

dϑ sin ϑ

′

ˆ R

dr′ r′2

r̂r − r̂′ r
| r̂r − r̂′ r′ |3

De la simetría de la distribución de carga, es claro que el campo eléctrico será sólo función
de la distancia r y su dirección será radial, es decir
⃗ x) = E(r)r̂
E(⃗
esto nos permite además orientar el vector ⃗x según la dirección k̂, de forma que

⃗ x) = ρ0
E(⃗
4πε0

ˆ 2π

'1/2
&
| r̂r − r̂′ r′ |= r2 + r′2 − 2rr′ cos ϑ′
′

dφ

ˆ π

′

dϑ sin ϑ

′

ˆ R

dr′ r′2

r̂r − r̂′ r

(r2 + r′2 − 2rr′ cos ϑ′ )3/2

= E(r)r̂

---

### Página 33

⃗ = 2πρ0
E(r) = r̂ · E
4πε0

ˆ π

′

dϑ sin ϑ

′

ˆ R

dr′ r′2

r − r′ cos ϑ′

(r2 + r′2 − 2rr′ cos ϑ′ )3/2

Hasta ahora, esta expresión es absolutamente general. Sin embargo, el valor de la integral
dependerá si el punto ⃗x se encuentra dentro o fuera de la distribución
Campo externo, r > R

se tiene
r = r′ cos ϑ′ + | ⃗x − ⃗x′ | cos α

Sea s =| ⃗x − ⃗x′ |, luego

r − r′ cos ϑ′

′ 3/2

(r2 + r′2 − 2rr′ cos ϑ )

=

s cos α
cos α
=
s3
s2

de la relación

se puede obtener para cos ϑ′

r2 + r′2 − 2rr′ cos ϑ′ = s2
cos ϑ′ =

r2 + r′2 − s2
2rr′

y utilizando el teorema del coseno para r′
r2 + s2 − 2rs cos α = r′2
de aquí obtenemos que
cos α =

Por último

r2 + s2 − r′2
2rs

∂
s
2s
dϑ′
=
−
cos ϑ′ = − sin ϑ′
=−
∂s
ds
2rr′
rr′

---

### Página 34

Luego

ˆ R

dr

=

ˆ R

′

ˆ π

dϑ′ sin ϑ′ r′2

r − r′ cos ϑ′

(r2 + r′2 − 2rr′ cos ϑ′ )3/2

ˆ r+r′

s
r2 + s2 − r′2
ds ′ r′2
dr
=
rr
2rs3
r−r ′

ˆ R

ˆ r+r′

#

′

= 2
2r

ˆ R

ˆ r+r′

r′
ds 2
dr
2r
r−r′
′

r2 − r′2
dr r
ds 1 +
s2
r−r′
′ ′

#

r2 − r′2
1+
s2

$

$

y
ˆ r+r′

r2 − r′2
ds 1 +
s2
r−r′
#

$

=

ˆ r+r′
r−r ′

ds + (r − r )

r2 − r′2
= (r + r ) − (r − r ) +
−2 + 1
′

′

= 2r′ − (r2 − r′2 )
Así
2r2

ˆ R

ˆ r+r′

#

de forma que
2πρ0
E(r) =
4πε0

ˆ π

′

dϑ sin ϑ

′

ˆ R

#

ˆ r+r′
r−r′

−
r + r′ r − r′

ds
s2

$

(r − r′ ) − (r + r′ )
= 4r′
r2 − r′2

r2 − r′2
dr r
ds 1 +
s2
r−r′
′ ′

′2

dr′ r′2

$

= 2
r

ˆ R

dr′ r′2 =

2R3
3r2

r − r′ cos ϑ′

ρR3
=
3ε0 r2
(r2 + r′2 − 2rr′ cos ϑ′ )3/2

Así, para r > R

⃗ x) = ρR r̂
E(⃗
3ε0 r2
si Q = 43 πR3 ρ0 es la carga total de la esfera, entonces
⃗ x) =
E(⃗

Q
r̂
4πε0 r2

es decir, fuera de la esfera, el campo eléctrico es igual al campo de una carga puntual de
carga total Q ubicada en el origen

---

### Página 35

La integral de Coulomb para r < R es levemente más compleja, y para calcularla resulta
útil manejar los conceptos sobre integrales de ángulo sólido. El valor pedagógico de este cálculo
no es espantar al lector del estudio de la electrostática, sino de mostrar explícitamente que,
aunque la geometría del problema es muy sencilla, la integral para el campo eléctrico no lo
es. Esto por supuesto motiva a desarrollar más herramientas matemáticas para el cálculo de
campos eléctricos, que en muchos casos facilitarán la vida (Comparar en el próximo capítulo
con el cálculo mediante la Ley de Gauss). De todas formas, integrar bien es un arte en muchos
casos, muy util

---

### Página 36

3.3.

Apéndice Matemático sobre la Delta de Dirac

En cursos de Electrodinámica, es muy utilizada la delta de Dirac δ(x), que satisface
δ(x) = 0, x ̸= 0
ˆ ∞
dxδ(x) = 1
−∞

Semejante función no existe en el análisis ordinario. La δ(x) de Dirac es una función generalizada (o distribución de Schwarz).
Funciones Generalizadas
Utilizaremos funciones complejas f (x) de cuadrado integrable bajo el producto interno dado
por
(f, g) =

ˆ ∞

dxf ∗ (x)g(x)

−∞

Sea

{gn (x), n = 1, 2, 3, ...}
una sucesión de funciones de cuadrado integrable, esto es
ˆ ∞
(gn , gn ) =
dx[gn (x)]2 < ∞
−∞

Llamaremos función de prueba cualquier función f (x) de cuadrado integrable
ˆ ∞
dx[f (x)]2 < ∞
(f, f ) =
−∞

Definimos la Función Generalizada g(x) asociada a la sucesión {gn (x)} como
.
g(x) = lím {gn (x)}
n→∞

Este símbolo se define mediante el límite de las integrales, es decir, g(x) es una función
generalizada asociada a la sucesión {gn (x)} si
ˆ ∞
ˆ ∞
dxg(x)f (x) = lím
dxgn (x)f (x)
n→∞

−∞

−∞

para cualquier función de prueba f (x)
Nota 1 Por la desigualdad de Schwarz
(gn , f )2 ≤ (gn , gn )(f, f ) < ∞
vemos que toda sucesión de funciones de cuadrado integrable define una función generalizada
Nota 2 En rigor, las funciones generalizadas están definidas detrás de la integral, no es
necesario que la sucesión sea convergente en el sentido ordinario, esto quiere decir que no es
necesario que se tenga
lím gn (x) = g(x)
n→∞

para que la función generalizada exista. g(x) existe rigurosamente en el límite de las integrales

---

### Página 37

3.3.1.

Delta de Dirac δ(x)

El ejemplo mas ilustre y sobresaliente de función generalizada es la delta de dirac, que
será fundamental para el desarollo de muchas teorías de la física, así como del Análisis de
Señales (Disciplina de la Ingeniería Eléctrica). Existen varias sucesiones que definen a la delta
de Dirac, comenzaremos con una sucesión de la forma
⎧
⎪
x < −1/n
⎨0
δn (x) = n/2 −1/n < x < 1/n
⎪
⎩
x > 1/n

Fig. 3.4: Primeras 3 funciones dadas por la sucesión δn (x)
Notar que a medida que aumenta n, la función se asemeja a un rectángulo cada vez más
angosto en torno al origen y de mayor amplitud. Sin embargo, siempre el área bajo δn (x) es
uno. Físicamente usaremos la delta de Dirac para modelar distribuciones de carga que son nulas
excepto en un punto del espacio
Veamos que en efecto δn (x) define una sucesión de funciones de cuadrado integrable
ˆ ∞
ˆ 1/n
! n "2 ! n " 2 # 2 $ n
(δn (x), δn (x)) =
dx[δn (x)] =
dx
=
=
n
−∞
−1/n
Además

ˆ ∞

dxδn (x) =

−∞

ˆ 1/n

n2
n
=1
dx( ) =
2n
−1/n

Veamos que ocurre con
ˆ ∞

dxδn (x)f (x)

−∞

donde f (x) es cualquier función de cuadrado integrable. Se tiene que

Fig. 3.5: Utilizando el teorema del valor medio integral

---

### Página 38

ˆ ∞

n
dxδn (x)f (x) =
−∞

ˆ 1/n

dxf (x) =

−1/n

n2
fn = fn
2n

donde fn es el valor de la función para algún x entre −1/n < x < 1/n . De esta forma, es
claro que
ˆ ∞
dxδn (x)f (x) = lím fn = f (0)
lím
n→∞

n→∞

−∞

En resumen, la sucesión δn (x) define la función generalizada δ(x), llamada delta de Dirac,
cuyas propiedades fundamentales son
ˆ ∞
dxδ(x) = 1
−∞

ˆ ∞

dxδ(x)f (x) = f (0)

−∞

δ(x) = 0, x ̸= 0

Del mismo modo, podemos interpretar δ(x − xo ) en base a
ˆ ∞
dxδ(x − x0 ) = 1
−∞

ˆ ∞

−∞

dxδ(x − x0 )f (x) = f (xo )

δ(x − x0 ) = 0, x ̸= x0

Nota
No existe ninguna función ordinaria con éstas propiedades, pero sí existe una función generalizada! Ahora que se tiene en claro el significado de las integrales recién mencionadas, se puede
tratar la delta de Dirac como una función ordinaria, sin olvidar el significado real de ésta.
Físicamente, la Delta puede representar una señal o Impulso de gran amplitud y de extensión
infinitamente pequeña. Por ejemplo, δ(t − to ) puede representar un sonido o una fuerza de gran
amplitud que ocurre en el instante t = to , y de extensión prácticamente nula en el tiempo (Un
aplauso o el impulso que actúa sobre una pelota cuando rebota contra una pared). En electricidad y magnetismo, ρ = qδ(x − xo )δ(y − yo )δ(z − z0 ) representará la densidad volumétrica de
una carga puntual q ubicada en (x0 , y0 , z0 ), es decir, es nula en todo el espacio excepto en el
punto (xo , y0 , z0 )
Igualdad de Funciones Generalizadas
Dos funciones generalizadas
g(x) = lím {gn (x)}
n→∞

h(x) = lím {hn (x)}
n→∞

son iguales si y sólo si, con cualquier función f (x) se tiene

---

### Página 39

ˆ ∞

−∞

dx[g(x) − h(x)]f (x) = 0

Es decir
.
g(x) = h(x) ⇐⇒

ˆ ∞

−∞

dx[g(x) − h(x)]f (x) = 0

Anteriormente mostramos como una sucesión de funciones rectangulares (δn (x)) definen a
δ(x). De igual forma, se puede construír la delta de Dirac con una sucesión de Gaussianas
n
2 2
hn (x) = √ e−n x
π
de forma que
δ(x) = lím {hn (x)}
n→∞

Fig. 3.6: Construcción de δ(x) mediante una sucesión de Gaussianas
Este tipo de funciones nos es familiar, sabemos que siempre una distribución Gaussiana
tiene como integral total 1 (es una distribución de Probabilidad). Para demostrar que esta
sucesión define igualmente a la delta basta con demostrar que
ˆ ∞
n
2 2
dx{δn (x) − √ e−n x }f (x) = 0
I = lím
n→∞ −∞
π

---

### Página 40

3.4.

Propiedades de la delta de Dirac
ˆ ∞

dxδ(x)f (x) = f (0)

−∞

δ(x)f (x) = f (0)δ(x)
δ(−x) = δ(x)
δ(ax) =
ˆ ∞

−∞

δ(x)
|a|

dxδ ′ (x)f (x) = −f ′ (0)

δ(x − x′ ) = 0, x ̸= x
ˆ b
a

dx′ δ(x − x′ ) = 1, a < x < b
δ(x − x′ ) = δ(x′ − x)

ˆ ∞

−∞

ˆ ∞

−∞

dx′ δ(x − x′ )f (x′ ) = f (x)

dx′′ δ(x′′ − x′ )δ(x′′ − x) = δ(x′ − x)
N
%
δ(x − xi )
δ(f (x)) =
| f ′ (x) |x=xi
i=1

donde xi son los ceros simples de f (x)

Delta de Dirac en 3 dimensiones
Se define
δ(⃗x − ⃗x′ ) = δ(x − x′ )δ(y − y ′ )δ(z − z ′ )
la cual cumple
˚

3 ′

′

d x δ(⃗x − ⃗x ) =

V

˚

R3

˚

R3

+

1 si ⃗x ∈ V
0 si ⃗x ∈
/V

d3 x′ δ(⃗x − ⃗x′ ) = 1

d3 x′ δ(⃗x − ⃗x′ )f (⃗x′ ) = f (⃗x)

---

### Página 41

Fig. 3.7: Paul Dirac
Paul Dirac(1902-1984) Físico Inglés. Se graduó de Ingeniero Eléctrico en 1921, posteriormente estudió matemáticas y fue recibido en la Universidad de Cambridge. En 1926 desarrolló una versión de la mecánica cuántica en la que unía el trabajo previo de Werner Heisenberg
y de Erwin Schrödinger en un único modelo matemático que asocia cantidades medibles con
operadores que actúan en el espacio vectorial de Hilbert y describe el estado físico del sistema.
Por este trabajo recibió un doctorado en física por Cambridge. En 1928, trabajando en los
spines no relativistas de Pauli, halló la ecuación de Dirac, una ecuación relativista que describe
al electrón. Este trabajo permitió a Dirac predecir la existencia del positrón, la antipartícula
del electrón

---

### Página 42

Problema
Muestre que una distribución discreta de cargas qi , i = 1, 2, ...N ubicada en los puntos ⃗xi ,
i = 1, 2, ...N es consistente con una distribución volumétrica de carga
N
%

ρ(⃗x) =

qi δ(⃗x − ⃗xi )

i=1

#### Solución
Para ver que la distribución de carga se puede escribir de esta forma, se debe verificar que el
campo eléctrico que genera es el correcto. En efecto
˚
⃗x − ⃗x′
⃗
d3 x′ ρ(⃗x′ )
E(⃗x) =
| ⃗x − ⃗x′ |3
R3

⃗ x) =
E(⃗

˚

3 ′

dx

R3

N
%
i=1

qi δ(⃗x − ⃗xi )

⃗x − ⃗x′
| ⃗x − ⃗x′ |3

Si la distribución es finita (N es un número finito) podemos intercambiar la integral con la
suma (y nos aseguramos que no se espante ningún matemático)
⃗ x) =
E(⃗

N
%
i=1

qi

˚

⃗ x) =
E(⃗

3 ′

R3

d x δ(⃗x − ⃗x′i )

N
%

qi

i=1

⃗x − ⃗x′
| ⃗x − ⃗x′ |3

⃗x − ⃗xi
| ⃗x − ⃗xi |3

que es el campo correcto generado por la distribución de carga

---

### Página 43

Problema
Demuestre la propiedad
δ(f (x)) =
donde xi son los ceros simples de f (x)

% δ(x − xi )
| f ′ (x) |x=xi
i

#### Solución
Sea la sucesión de funciones de cuadrado integrable
⎧
⎪
x < −1/n
⎨0
δn (x) = n/2 −1/n < x < 1/n
⎪
⎩
x > 1/n
δ(x) es la función generalizada asociada a la sucesión δn (x)
.
δ(x) = lím {δn (x)}
n→∞

Ahora usaremos el hecho de que dos funciones generalizadas
.
g(x) = lím {gn (x)}
n→∞

.
h(x) = lím {hn (x)}
n→∞

son iguales si y solo si , con cualquier función de prueba f (x) se tiene
ˆ ∞
dx (g(x) − h(x)) f (x) = 0
∞

Se define la función generalizada
g(x) =

% δ(x − xi )
df
| dx
|x=xi

i

donde xi son los ceros simples de f . Por supuesto
.
g(x) = lím {gn (x)}
n→∞

con

gn (x) =

% δn (x − xi )

(x)
| dfdx
|x=xi

i

Sea y(x) una función de prueba
ˆ ∞
ˆ ∞
% δn (x − xi )
y(x)
dxgn (x)y(x) =
dx
df (x)
|
|
−∞
−∞
x=x
i
i
dx
ˆ ∞

−∞

dxgn (x)y(x) =

%ˆ ∞
i

−∞

dx

δn (x − xi )

(x)
| dfdx
|x=xi

Por el teorema del valor medio integral
ˆ ∞
%
dxgn (x)y(x) =
−∞

i

y(x) =

% ˆ xi +1/n
i

n/2
(x)
| dfdx
|x=x∗

dx

xi −1/n

(2/n) y(x∗ )

n/2
(x)
| dfdx
|x=xi

y(x)

---

### Página 44

con x∗ ∈ [−1/n + xi , 1/n + xi ]. Con esto
ˆ ∞
ˆ ∞
%
lím
dxgn (x)y(x) =
dxg(x)y(x) =
n→∞

−∞

−∞

i

y(xi )
df
| dx |x=xi

Ahora, veamos que ocurre con la función generalizada
.
h(x) = lím {hn (x)}
n→∞

con
hn (x) = δn [f (x)]
⎧
⎪
f (x) < −1/n
⎨0
hn (x) = n/2 −1/n ≤ f (x) ≤ 1/n
⎪
⎩
f (x) > 1/n

sea Ij = [x1j , x2j ], j = 1, 2, ... tal que ∀x ∈ Ij , −1/n ≤ f (x) ≤ 1/n (x2j ≥ x1j ) y tal que
Ij
Ii = φ

∀i ̸= j (intervalos disjuntos). Así, por el teorema del valor medio integral
ˆ ∞
%n
% ˆ x2i n
y(x∗i ) (x2i − x1i )
dxhn (x)y(x) =
dx y(x) =
−∞
x1i
i
i
con x∗i ∈ Ii . Además, está garantizada la existencia de un x′i ∈ Ii tal que
|
Luego

df (x)
| 2/n |
2/n
|x=x′i =
=
dx
x2i − x1i
x2i − x1i

ˆ ∞

dxhn (x)y(x) =

−∞

(2/n) (2/n) y(x∗i )
(x)
| dfdx
|x=x′i

Si n → ∞, Ij = xj tal que f (xj ) = 0. Así
ˆ ∞
lím dxhn (x)y(x) =
dxh(x)y(x) =
n→∞

−∞

y(xi )
df (x)
| dx |x = xi

Por lo tanto, se ha demostrado la igualdad entre las funciones generalizadas
δ[f (x)] =

% δ(x − xi )
i

(x)
| dfdx
|x=xi

---

### Página 45

#### Capítulo 4
Ley de Gauss
En el capítulo anterior hemos visto las leyes empíricas fundamentales de la electrostática en
el espacio vacío (sin un medio material presente), las cuales se pueden resumir en lo siguiente
1) Las cargas eléctricas estáticas son fuentes de campos eléctricos, los cuales actúan sobre
otras cargas

2) El campo de una carga puntual está dado por la Ley de Coulomb, esto es, su magnitud
es proporcional a la magnitud de la carga y decrece según el inverso del cuadrado de la distancia
3) Si hay más de una carga presente, el campo total será la suma vectorial de los campos debido
a cada carga individual (Principio de Superposición)
Estas leyes son toda la electrostática! Si combinamos la ley de Coulomb y el principio de
superposición, no necesitamos (en teoría) saber nada más. A partir de estas leyes vimos además
que si se tiene una distribución continua de carga encerrada en un volumen V , el campo eléctrico
en un punto ⃗x se obtiene evaluando la integral de Coulomb
˚ 3 ′ ′
d x ρ(⃗x )(⃗x − ⃗x′ )
⃗
E(⃗x) =
4πϵ0
| ⃗x − ⃗x′ |3
V
Más adelante no utlizaremos demasiado ésta fórmula, la escribimos sólo para enfatizar el
hecho de que hemos resuelto completamente el problema de la electrostática en que conocemos
exactamente la distribución espacial de todas las cargas. Es decir, conocemos ρ(⃗x′ ) en todo el
espacio.

---

### Página 46

Problema que hemos resuelto: Dadas las cargas, ¿cómo son los campos?
Nuestra respuesta es : Resuelva esta integral
˚ 3 ′ ′
d x ρ(⃗x )(⃗x − ⃗x′ )
⃗
E(⃗x) =
4πϵ0
| ⃗x − ⃗x′ |3
V
Así que aparentemente no hay nada más que resolver, todo se trata de calcular integrales en 3
dimensiones. (que en la práctica pueden ser nada de sencillas). Con las integrales de Coulomb
podemos encontrar de forma relativamente sencilla los campos producidos por un plano de
carga, de una línea de carga, de una cáscara esférica de carga, o de alguna otra distribución
más o menos simple.
El gran problema es, que en muchas situaciones reales de la electrostática, la distribución
es más compleja, o peor aún, no conocemos inicialmente cómo están distribuídas las cargas,
luego las cosas se nos complican. Las posiciones de las cargas pueden depender del campo
eléctrico, y el campo eléctrico a su vez dependerá de la posición de las cargas. Por ejemplo,
veremos más adelante que si acercamos un cuerpo cargado a un conductor (es un material
que cumple ciertas propiedades) , los electrones en el conductor se moverán hasta alcanzar un
equilibrio electrostático. La densidad de carga ρ puede ser conocida en parte, (la carga que
hemos acercado), pero habrá otra parte debida a las cargas que se mueven en el conductor que
definitivamente no conocemos inicialmente. Y para calcular la integral de Coulomb, toda la
distribución de carga se debe conocer.
Luego, deberemos introducir otras leyes y herramientas matemáticas necesarias para resolver los problemas de Electrostática, y veremos que la situación no siempre es tan fácil como
se podría pensar

4.1.

Ley de Gauss de la Electrostática

Comensaremos por definir una cantidad escalar llamada flujo de un campo vectorial.

⃗ = S n̂ como el vector de área, cuya
Considere la superficie plana de la figura. Se define S
magnitud es el área de la superficie, S, y apunta en la dirección normal n̂ (perpendicular en
todo punto a la superficie). Si la superficie se encuentra sumergida en un campo eléctrico
⃗ que apunta siempre en la misma dirección de n̂ (perpendicular a la superficie S),
uniforme E
⃗ sobre el vector S
⃗
el flujo sobre la superficie es la proyección de E
⃗ ·S
⃗=E
⃗ · n̂S = ES
ΦE = E
Ahora, si el campo eléctrico sigue siendo uniforme pero forma un ángulo ϑ con n̂, el flujo
será

---

### Página 47

⃗ ·S
⃗ = EScosϑ
ΦE = E

Es decir, el flujo de un campo vectorial sobre una superficie mide en cierta forma la componente
normal a la superficie. Notar que según la definición del vector normal n̂, el flujo eléctrico es
positivo si las líneas de campo eléctrico están saliendo a través de la superficie, y será negativo
si las líneas entran a través de la superficie.
Generalización
Hemos definido el flujo del campo eléctrico sobre una superficie muy simple (plana). Además
hemos supuesto que el campo es uniforme (magnitud y dirección constantes). En general,una
⃗ puede variar sobre la superficie (tanto en
superficie S puede ser curva, y el campo eléctrico E
magnitud como en dirección).
Nos resultará de particular interés aquellas superficies que son cerradas. Una superficie
cerrada es aquella que envuelve completamente a un volumen (es el contorno de un volumen).
Para calcular el flujo del campo sobre una superficie cerrada, se divide la superficie en una
⃗i = ∆Si n̂i , como se ve en la figura.
suma de elementos de área infinitesimales, ∆S

⃗i es
El flujo a través de ∆S
⃗ i · ∆S
⃗i = Ei ∆Si cosθ
∆ΦE = E
El flujo total a través de la superficie se obtiene sumando sobre todos los elementos de
superficie. (A la Riemann) Tomando el límite cuando ∆Si → 0 se obtiene la integral de flujo
ˆˆ
%
☎ ⃗
⃗ i · dS
⃗i = ✞
⃗ x)
∆ΦE = lím
E
x) · E(⃗
✝ ✆dS(⃗
∆Si →0

S

Le ley de Gauss establece que el flujo eléctrico a través de una superficie cerrada es
proporcional a la carga encerrada por ella. Más concretamente
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = qenc
x ) · E(⃗
ΦE = ✝ ✆dS(⃗
ϵ0
S

---

### Página 48

o, escribiendo de forma explícita la carga encerrada por S
ˆˆ
˚
✞☎ ⃗ ′
′
⃗
x ) · E(⃗x ) =
d3 x′ ρ(⃗x′ )
✝ ✆dS(⃗
ε0
S
V (S)
Esta ley es consecuencia directa de la Ley de Coulomb y la geometría Euclídea. Notar que
campos eléctricos creados por cargas fuera de la superficie no contribuyen al flujo total. Es
decir, el flujo sobre una superficie cerrada sólo depende de la carga encerrada por ella.
La forma de la superficie puede ser elegida arbitrariamente. Para las superficies de la figura,
el mismo resultado se obtiene para el flujo eléctrico (ΦE = Q/ϵ0 ).

La ley de Gauss es extremadamente útil en muchos casos. Hay que notar, que a partir de
la Ley de Gauss es posible recuper la Ley de Coulomb, es decir, conociendo la ley de Gauss
uno podría determinar la forma de los campos. Hay que notar además, que hay casos en los
cuales esta ley no es práctica, es útil sólo en problemas donde la integral de flujo es simple
de calcular.
Ejemplo: Campo de una distribución esférica homogénea de carga
Tal como en el capítulo 1, se desea obtener el campo eléctrico de una distribución de carga
+
ρ0 si | ⃗x′ |≤ R
′
ρ(⃗x ) =
0 si | ⃗x′ |> R

donde el origen del sistema de coordenadas coincide con el centro de la distribución de carga.
Una forma de resolver esto es evaluando la integral de Coulomb (no muy recomendable). Otra,
es considerando la evidente simetría esférica del campo eléctrico, es claro que éste sólo puede
depender de la distancia r al origen. Además, su dirección debe coincidir con la dirección radial
r̂. De esta forma, para obtener el campo exterior, escogemos una superficie Gaussiana esférica
de radio r > R, como se muestra en la figura

El flujo del campo eléctrico sobre esta superficie es
ˆˆ
ˆˆ
ˆˆ
✞☎ ⃗ ′
✞☎
✞☎
′
⃗
Φ = ✝ ✆dS(⃗x ) · E(⃗x ) = ✝ ✆dS r̂ · E(r)r̂ = E(r) ✝ ✆dS
S

S

S

---

### Página 49

Φ = E(r)4πr2 =

Q
ε0

donde Q es la carga total de la distribución
Q
r̂
4πε0 r2
es decir, igual al de una carga puntual Q en el origen. En términos de la densidad ρ0
⃗ = E(r)r̂ =
E

Q = πR3 ρ0

⃗ = E(r)r̂ = ρ0 R r̂
E
3ε0 r2
Mismo resultado obtenido en el capítulo anterior (ahora de forma mucho más simple). Ahora,
para el campo interno, nuevamente escogemos una superficie Gaussiana de radio r < R

Nuevamente el flujo es
✞☎ ⃗ ′
⃗ x′ ) = E(r)4πr2 = qin
x ) · E(⃗
Φ = ✝ ✆dS(⃗
ε0
S

ˆˆ

donde qin es la carga encerrada por la superficie S, en este caso
qin = πr3 ρ0
de forma que
E(r)4πr2 =

4πr3 ρ0
3ε0

rρ0
3ε0
es decir, el campo eléctrico en el interior de la distribución es lineal en r. Finalmente
rρ0
r̂ si | ⃗x |≤ R
⃗
E(⃗x) = ρ3ε
0R
r̂ si | ⃗x |> R
3ε0 r2
E(r) =

---

### Página 50

Notar que el campo es continuo en | x |= R

pero no es diferenciable en dicho punto!
Ejemplo: Plano infinito de carga
Consideremos un plano infinito en X − Y con densidad superficial de carga uniforme σ. Se
desea determinar el campo eléctrico en todo el espacio

⃗
Debido a que la carga está distribuída uniformemente en la superficie, el campo eléctrico E
⃗ = E k̂. Además, la magnitud del campo es constante en
debe ser perpendicular al plano , E
planos paralelos al plano de carga. Elegimos como superficie Gaussiana un cilindro (llamado
por muchos autores como caja de píldoras)

el flujo sobre esta superficie es
ˆˆ
¨
¨
¨
✞☎ ⃗ ′
′
⃗
⃗
⃗
⃗
⃗
⃗3 · E
⃗3
Φ = ✝ ✆dS(⃗x ) · E(⃗x ) =
dS1 · E1 +
dS2 · E2 +
dS
S

donde se ha dividido la superficie cerrada en la superficies S1 y S2 (tapas), y en S3 (manto).
Claramente el flujo sobre este último es cero, pues el campo es perpendicular en todo punto al
vector normal a S3 . Con esto
ˆˆ
¨
¨
✞☎ ⃗ ⃗
⃗
⃗
⃗2 · E
⃗2
Φ = ✝ ✆dS · E =
dS1 · E1 +
dS
S

---

### Página 51

S1 y S2 están a la misma distancia del plano infinito, luego, en ambas superficies la magnitud
del campo debe ser la misma, digamos, E, luego
#¨
$
ˆˆ
¨
✞☎ ⃗ ⃗
Φ = ✝ ✆dS · E = E
dS1 +
dS2 = 2AE
S

donde A es la superficie total de S1 y S2 . Por la ley de Gauss, el flujo del campo eléctrico es
Φ = 2AE =

qin
ε0

donde la carga encerrada por esta superficie es
qin = σA
de forma que
E=

σ
2ε0

en notación vectorial
⃗ x) =
E(⃗

σ
k̂
2ε0
σ
− 2ε0 k̂

si z > 0
si z < 0

notar que el campo tiene una discontinuidad en z = 0
σ
⃗
⃗
− lím− E(z)
=
lím+ E(z)
z→0
z→0
ε0
Veremos que el campo eléctrico siempre es discontinuo al atravesar una superficie cargada

---

### Página 52

Problema
Se tiene una cáscara esférica de radio a y de carga Q distribuída uniformemente sobre su superficie. Encuentre el campo eléctrico en todo el espacio
#### Solución
Por la simetría esférica de la distribución de carga, y utilizando un sistema de coordenadas
cuyo origen coincide con el centro de la distribución, se tiene que el campo eléctrico debe ser
de la forma
⃗ = E(r)r̂
E
Para r < a, elegimos una superficie Gaussiana esférica de radio r, como se muestra en la
figura

de la ley de Gauss
qin
✞☎ ⃗ ⃗
✝ ✆dS · E =

ˆˆ

ε0

S

Es claro que en este caso no hay carga encerrada por la superficie, de forma que
ˆˆ

✞☎ ⃗ ′
⃗ x′ ) = E(r)4πr2 = 0 → E(r) = 0
x ) · E(⃗
✝ ✆dS(⃗
S

Para r > a, nuevamente elegimos una superficie Gaussiana esférica de radio r

✞☎ ⃗ ′
⃗ x′ ) = 4πr2 E(r) = Q
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ε0

S

⃗ = E(r)r̂ =
E

Q
r̂
4πε0 r2

es decir, para r > a el campo es igual al de una carga puntual Q en el origen.

---

### Página 53

⃗ x) =
E(⃗

+

⃗0
Q
r̂
4πε0 r2

si | ⃗x |< a
si | ⃗x |> a

El campo es discontinuo en r = a (siempre lo es al atravesar una superficie cargada)

Notar que

Q
σ
=
r→a+
r→a−
4πε0 a
ϵ0
donde σ es la densidad superficial de carga. Notar que se obtuvo lo mismo en la interfaz de un
plano cargado (En efecto, es un resultado general)
lím E(r) − lím E(r) =

---

### Página 54

Problema
Considere un cable coaxial muy largo, el cable está compuesto por un cilindro sólido interior,
de radio a que lleva una densidad de carga volumétrica ρ (constante) y por un cilindro exterior
hueco de radio b (b > a) que lleva una densidad de carga superficial σ, esta densidad es tal que
el cable es eléctricamente neutro. Encuentre el campo eléctrico producido por el cable en todo
el espacio

#### Solución
Establecemos un sistema de coordenadas cilíndricas en el centro del cable

Distinguimos tres regiones,I, II y III dadas por r > b, a < r < b y r < a respectivamente. Por
simetría, el campo (de existir) en la región I debe ser radial, y su magnitud únicamente función
de r (La figura posee una clara simetría azimutal, es decir, es invariante ante una rotación del
ángulo polar ϕ). Por ley de Gauss
✞☎ ⃗ ′
⃗ x′ ) = 1 Qint
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

donde S es cualquier superficie cerrada y Qint la carga encerrada por ésta
Qint =

˚

d3 x′ ρ(⃗x′ )

V (S)

⃗ x′ )//n̂(⃗x′ ) y | E(⃗
⃗ x′ ) |
Debemos encontrar una superficie con las siguientes características: E(⃗
′
constante ∀⃗x ∈ S . Dada la simetría del problema usamos como superficie un cilindro de radio
r > b y altura h S

---

### Página 55

Luego
¨

ˆˆ

✞☎ ⃗ ′
⃗ x) =
x ) · E(⃗
✝ ✆dS(⃗
S

M anto

⃗ x′ ) · E(⃗
⃗ x′ ) +
dS(⃗

¨

T apas

⃗ x′ ) · E(⃗
⃗ x′ )
dS(⃗

⃗ x′ ) = dS(⃗x′ )n̂(⃗x′ ) = rdϕdzr̂(ϕ), y E(⃗
⃗ x′ ) = E(r)r̂(ϕ), de forma
Para todo ⃗x′ en el manto, dS(⃗
que
¨

M anto

⃗ x′ ) · E(⃗
⃗ x′ ) = E(r)
dS(⃗

¨

dS(⃗x′ ) = 2πrhE(r)

M anto

⃗ x′ ) = rdϕdrẑ, y en la tapa inferior
Por otro lado, para todo ⃗x′ en las tapa superior, dS(⃗
⃗ x′ ) = E(r)r̂(ϕ)⊥dS(⃗
⃗ x′ ), luego
⃗ x′ ) = −rdϕdrẑ , mientras que E(⃗
dS(⃗
¨

T apas

⃗ x′ ) · E(⃗
⃗ x′ ) = 0
dS(⃗

con esto
ˆˆ

✞☎ ⃗ ′
⃗ x) = E(r)2πrh
x ) · E(⃗
✝ ✆dS(⃗
S

pero como el cable es neutro, Qint = 0. Luego
E(r)2πrh = 0 → E(r) = 0, r > b
Notar que
Qint = πa2 hρ + σ2πbh = 0
luego
σ=−

ρa2
2b

En la región II: a < r < b, la simetría nuevamente implica la naturaleza radial del campo
eléctrico (al igual que su dependencia en r y no en ϕ). Nuevamente utilizamos como superficie
cerrada un cilindro de radio r y altura h

---

### Página 56

✞☎ ⃗ ′
⃗ x) = 1 Qint
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0
Por los mismos argumentos utilizados anteriormente, la integral de flujo se reduce a
ˆˆ
✞☎ ⃗ ′
⃗ x) = E(r)2πrh
x ) · E(⃗
✝ ✆dS(⃗
S

S

y
Qint =

˚

3 ′

′

d x ρ(⃗x ) = ρ

V (S)

entonces

˚

d3 x′ = ρπa2 h

V (S)

πa2 h
E(r)2πrh = ρ
ϵ0

⃗ x) = a ρ r̂
E(⃗
2ϵ0 r
si r ∈ [a, b]
Por último, para la región III: r < a, se escoge nuevamente un cilindro de radio r y altura
h. Los mismos argumentos de simetría son válidos aquí para determinar el campo eléctrico.
Resulta
ˆˆ
✞☎ ⃗ ′
⃗ x) = 1 Qint
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
y
ˆˆ
✞☎ ⃗ ′
⃗ x) = E(r)2πrh
x ) · E(⃗
✝ ✆dS(⃗
S
˚
˚
3 ′
′
Qint =
d x ρ(⃗x ) = ρ
d3 x′ = ρπr2 h
V (S)

V (S)

entonces
E(r)2πrh = ρ

πr2 h
ϵ0

⃗ x) = ρr r̂
E(⃗
2ϵ0
En resumen (notar discontinuidad al atravesar la superficie cargada r = b)
⎧ ρr
⎨ 2ϵ0 si 0 ≤ r < a
⃗ x) = a2 ρ si a < r < b
E(⃗
⎩ 2ϵ0 r
si b < r

---

### Página 57

Problema
Considere dos esferas no concéntricas de radio R. La primera de ellas lleva una densidad
volumétrica de carga ρ y la segunda −ρ. Los centros de las esferas están a distancia menor
que 2R. si d⃗ es el vector que va del centro de la esfera positiva al centro de la negativa, demuestre que el campo eléctrico en la intersección de las esferas es constante, y encuentre su
valor

#### Solución
Este problema se resuelve por superposición y recordando la forma del campo eléctrico generado
por una distribución homogénea y esférica de carga (resuelto anteriormente)

⃗ x) =
E(⃗

ρr
r̂
3ϵ0
ρR3
r̂
3ϵ0 r2

si r ≤ R
si r > R

donde r es la distancia al centro de la distribución. Ahora, sea P un punto arbitrario dentro
de la región de la intersección

---

### Página 58

El campo en P producido por la distribución de carga positiva es
⃗ 1 = ρ ⃗r
E
3ϵ0
y el de la distribución de carga negativa
⃗ 2 = −ρ ⃗r′
E
3ϵ0
Por el principio de superposición, el campo eléctrico en P está dado por
⃗ )=E
⃗1 + E
⃗ 2 = ρ ⃗r + −ρ ⃗r′
E(P
3ϵ0
3ϵ0
Pero
de forma que

d⃗ + ⃗r′ = ⃗r
⃗r′ = ⃗r − d⃗
!
"
⃗ ) = ρ ⃗r + −ρ ⃗r − d⃗
E(P
3ϵ0
3ϵ0

⃗ ) = ρ d⃗
E(P
3ϵ0
P fue escogido de manera arbitraria, luego, para todo ⃗x dentro de la distribución, el campo
eléctrico es uniforme y está dado por
⃗ x) = ρ d⃗
E(⃗
3ϵ0
notar que es paralelo a la dirección que une ambos centros

---

### Página 59

Problema
Se tiene un cilindro de radio R muy largo y con densidad de carga homogénea ρ. Se ha suprimido
un cilindro con eje paralelo con el mismo largo y radio R/2. El vector que une el centro del
cilindro con el centro de la cavidad es ⃗a para una sección transversal. Se pide obtener la expresión
del campo eléctrico en un punto cualquiera de la cavidad que no pertenezca a la recta que une
los centros del cilindro y de la cavidad

#### Solución
Este problema se puede resolver de forma muy simple utilizando el principio de superposición.
Evidentemente podemos considerar el problema del cilindro lleno con densidad ρ, y superponer
un cilindro menor con densidad −ρ. Primero, debemos encontrar una expresión para el campo
eléctrico al interior de un cilindro muy largo de radio R.
Debido a la simetría, es evidente que el campo eléctrico al interior del cilindro debe ser
radial y constante a una cierta distancia r del centro.

Luego, utilizamos como superficie de Gauss un cilindro de radio r y largo L.
✞☎ ⃗ ′
⃗ x′ ) = Qin
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

Ahora, notemos que el cilindro lo podemos dividir en 3 superficies

---

### Página 60

Luego la ley de Gauss queda
ˆˆ
¨
¨
¨
✞☎ ⃗ ′
′
⃗
⃗
⃗
⃗
⃗
⃗3 · E
⃗3
x ) · E(⃗x ) =
dS1 · E1 +
dS2 · E2 +
dS
✝ ✆dS(⃗
S

S

S

S

Notar que en todos los puntos de la superficie S1 el campo eléctrico es perpendicular al
vector normal. Lo mismo sucede con la superficie S2 , luego, las dos primeras integrales de flujo
son nulas. Se tiene entonces
¨
¨
ˆˆ
✞☎ ⃗ ′
′
⃗
⃗
⃗
x ) · E(⃗x ) =
dS3 · E3 =
Er r̂ · dS3 r̂
✝ ✆dS(⃗
S

S

E(r)

¨

S

dS3 = E(r)2πrL

S

Ahora, la carga encerrada por la superficie de Gauss es
˚
d3 x′ ρ(⃗x′ )
Qin =
V (S)

donde V (S) es el volumen encerrado por S. Como ρ es constante,
˚
Qin = ρ
d3 x′ = ρπr2 L
V

Luego la ley de Gauss queda
E(r)2πrL = ρπr2 L
ρr
E(r) =
Ahora, eligiendo un punto P dentro de la cavidad, tendremos que el campo total será la
suma vectorial del campo eléctrico debido a un cilindro homogéneo de carga y del campo debido
a un cilindro homogéneo de carga negativa, tal como indica la figura

⃗ 1 = ρr r̂
E
⃗ 2 = − ρx r̂′
E
donde
r̂′ =

(⃗r − ⃗a)
(rr̂ − ⃗a)
=
x
x

Sumando ambos campos

---

### Página 61

⃗ = ρr r̂ − ρx (rr̂ − ⃗a)
E
x
⃗ = ρr r̂ − ρrr̂ + ρ⃗a
E
⃗ = ρ⃗a
E
El campo en todo punto de la cavidad es uniforme y paralelo al vector ⃗a

---

### Página 62

Problema
Considere un plano infinito de carga con densidad superficial σ > 0. Se practica un orificio
circular de radio R.
a) Calcule el campo eléctrico en cualquier punto de abscisa x perteneciente al eje del orificio
b) A lo largo del eje del orificio se coloca una línea de carga de largo a, densidad lineal λ > 0
y cuyo punto más próximo se encuentra a distancia µ del centro del orificio. Calcule la fuerza
de repulsión que experimenta la línea de carga.

#### Solución
Una forma natural de solucionar este problema es utilizando el principio de superposición.
Esto es, considerar al plano con un orificio como la suma de un plano completo con un disco
de densidad superficial −σ. Ya se vió que el campo debido a un plano infinito de carga es
homogéneo y está dado por
⃗ 1 = σ k̂
E
2ϵ0
Ahora, para calcular el campo en el eje de un disco, de radio R y densidad σ

Un elemento de superficie del disco está dado por dA = rdrdφ, que tiene asociado un
elemento diferencial de carga, dado por dq = σdA = σrdrdφ.
Así, el campo eléctrico en P debido a este elemento de superficie será
⃗2 =
dE

1 dq(⃗x − ⃗x′ )
4πϵ0 | ⃗x − ⃗x′ |3

donde ⃗x = xk̂, ⃗x′ = r(cos φî + sin φĵ) así

---

### Página 63

| ⃗x − ⃗x′ |= (r2 + x2 )1/2
⃗x − ⃗x′ = xk̂ − r(cos φî + sin φĵ)
Con esto la contribución al campo total en P debido al elemento de superficie es
⃗2 =
dE

1 σrdrdφ(xk̂ − rr̂)
4πϵ0 (r2 + x2 )3/2

Así, el campo eléctrico total en P debido al disco completo será
⃗ 2 = σx
E
4πϵ0

ˆ 2π

dφ

ˆ R

r
σ
dr 2
k̂ −
3/2
(r + x )
4πϵ0

ˆ 2π

dφ(cos φî + sin φĵ)

ˆ R

dr

r2
(r2 + x2 )3/2

La segunda integral es 0, y esto se puede mostrar calculándola directamente o usando el
argumento de simetría, ya que es evidente que el campo eléctrico resultante en el eje solo
tendrá componente en k̂. Sea u = r2 + x2 , así, du = 2rdr , con esto
ˆ R2 +x2

⃗ 2 = 2π σx
E
4πϵ0

x2

du
k̂
2u3/2

Donde el factor 2π sale de integrar dφ entre 0 y 2π. Finalmente
)x2 +R2
σx
σx
σx 1
−1/2 )
⃗
√
− 2u
k̂ = −
+
E2 =
k̂
)2
4ϵ0
2ϵ0 R + x
2ϵ0 x
x
√
−σx
+
σ
R 2 + x2
⃗2 =
√
k̂
E
2ϵ0 R2 + x2

⃗2 = σ
E
2ϵ0

#

x
1− √
R 2 + x2

$

k̂

Notar que si R → ∞ se recupera el campo de un plano infinito
⃗ = σ k̂
E
2ϵo
⃗ 2 , ya que el disco tiene
⃗ 1 y -E
Finalmente el campo eléctrico total en P , será la suma de E
densidad de carga −σ
⃗ )= σ + σ
E(P
2ϵ0 2ϵ0

#

$
x
√
− 1 k̂
R 2 + x2

⃗ )= σ √ x
k̂
E(P
2ϵ0 R2 + x2

b)

---

### Página 64

Para calcular la fuerza sobre el alambre de carga, bastará con tomar un elemento diferencial
de longitud dx y obtener la fuerza electrostática que actúa sobre éste
⃗
⃗
dF⃗ = dq E(x)
= λdxE(x)
=

σx
λ
√
dxk̂
2ϵ0 R2 + x2

Con lo que la fuerza total sobre la línea de carga será
$
ˆ µ+a #
σx
λ
√
dx
F =
k̂
2ϵ0 R2 + x2
µ
Sea z = R2 + x2 , con lo que dz = 2xdx. Finalmente
λσ
F⃗ =
4ϵ0

ˆ R2 +(µ+a)2
R2 +µ

"
(
dz
σλ !( 2
√ î =
R + (µ + a)2 − R2 + µ2 k̂
2ϵ0
z

---

### Página 65

Problema
Considere la siguiente distribución volumétrica de carga en coordenadas esféricas
ρ(r) =

k
,a ≤ r ≤ b
r2

Encuentre el campo eléctrico en todo el espacio
#### Solución
Se tiene la distribución de carga dada por
ρ(r) =

k
,a ≤ r ≤ b
r2

Consideremos las distribuciones auxiliares
ρ1 (r) =

k
,0 ≤ r ≤ b
r2

k
ρ2 (r) = − 2 , 0 ≤ r ≤ a
r
Es fácil ver que
ρ(r) = ρ1 (r) + ρ2 (r)
Luego, podemos calcular por separado ambos campos eléctricos para luego superponerlos.
Consideremos entonces, el problema
ρ′ =

k′
,0 ≤ r ≤ R
r2

Sea la región del espacio en que r > R. Dada la simetría esférica de la distribución, escogemos
como superficie Gaussiana S una esfera concéntrica al origen y de radio r > R

---

### Página 66

El flujo a través de S será
ˆˆ

✞☎ ⃗ ′
⃗ x′ ) = 4πr2
x ) · E(⃗
✝ ✆dS(⃗
S

La carga encerrada por esta superficie es
˚
ˆ 2π
ˆ π
ˆ R
k′
3 ′
′
Qint =
d x ρ(⃗x ) =
dϕ
dϑ sin ϑ
drr2 2 = 4πRk ′
r
V (S)
Por ley de Gauss
E(r)4πr2 =

4πRk ′
ϵ0

′

Rk
⃗
r̂, r > R
E(r)
=
ϵ0 r 2
Ahora, para r < R, nuevamente se utiliza una superficie esférica de radio r y se resuelve en
forma análoga a la anterior, lo único que varía es la carga encerrada
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 4πr2
x ) · E(⃗
✝ ✆dS(⃗
S

esta vez la carga encerrada es la carga contenida en todo el volumen de la superficie de
Gauss
˚
Q=
d3 x′ ρ(⃗x′ ) = 4πrk ′
S(V )

entonces

4πrk ′
E(r)4πr =
ϵ0

′

k
⃗
E(r)
=
r̂
ϵ0 r
Ahora, superponemos los campos generados por ρ1 y ρ2 . Si r > b > a
⃗ = bk r̂ + (−k)a r̂
E
ϵ0 r 2
ϵ0 r 2
⃗ = k(b − a) r̂
E
ϵ0 r 2
Si a < r < b

(−k)a
k
⃗
r̂
r̂ +
E(r)
=
ϵ0 r
ϵ0 r 2
#
$
k
ak
⃗
E(r) =
−
r̂
ϵ0 r ϵ0 r 2

Por último, para
r<a
#
$
k
k
⃗
E(r) =
−
r̂
ϵ0 r ϵ0 r
⃗
E(r)
=0

---

### Página 67

En resumen
⃗
E(r)
=

⎧
⎪
⎨!
⎪
⎩

si r < a

k
− ϵak
ϵ0 r
0r
k(b−a)
r̂
ϵ0 r 2

"

r̂ si a < r < b
sir > b > a

Notar que este problema se podría haber resolvido fácilmente utilizando directamente la
ley de Gauss. Sin embargo, utilizar el principio de superposición facilita mucho el cálculo en
algunos otros casos

---

### Página 68

Problema
Dos planos infinitos y paralelos, a distancia a uno del otro, delimitan una región del espacio que
contiene una distribución continua y uniforme de carga eléctrica cuya densidad volumétrica es
ρ constante.
a) Calcular el campo eléctrico en el punto A a distancia x del plano central y el campo en un
punto exterior P a distancia r del plano central

b) Ahora en la distribución de carga anterior se reemplaza una esfera como en la figura por
una distribución con carga de densidad uniforme −ρ. Calcular el campo en el centro de la esfera
, y en un punto P exterior a distancia x del plano central

#### Solución
Para encontrar el campo eléctrico al interior de la distribución, podemos utilizar la Ley de
Gauss. Notar que como la región esta limitada por planos infinitos, por un argumento de
⃗ solo tendrá componente en la dirección î.
simetría el campo E
Notar además, que para x > 0, el campo tendrá dirección x̂, mientras que si x < 0, el campo
tendrá dirección −x̂. Utilizando un cilindro como superficie de Gauss, de radio x , se tiene
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = qin
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
En este caso sólo habrá flujo a través de las tapas del cilindro, puesto que el campo es
horizontal y perpendicular a la normal del cilindro sobre el manto. Luego
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = E(x)2S
x ) · E(⃗
✝ ✆dS(⃗
S

---

### Página 69

donde S es el área de cada tapa. Ahora, la carga encerrada por este cilindro será simplemente
qin = ρV = ρ2xS
Con esto
2SE(x) =

ρ2xS
ϵ0

E(x) =

ρx
ϵ0

Finalmente, para | x |< a/2

⃗ = ρx î
E
ϵ0

Ahora, para obtener el campo en un punto exterior a distancia r > a/2 del plano central,
volvemos a utilizar la ley de Gauss, como se aprecia en la figura

Nuevamente sólo habrá flujo por S1 y S2 , luego
#¨
$
¨
ˆˆ
✞☎ ⃗ ′
′
⃗
x ) · dE(⃗x ) = E(r)
dS1 +
dS2
✝ ✆dS(⃗
S

S1

S2

ˆˆ

✞☎ ⃗ ⃗
✝ ✆dS · E = E(r)2S
S

la carga encerrada por el cilindro será
qin = ρaS
Luego
E(r)2S =

ρaS
ϵ0

de donde se obtiene, para | r |> a/2
⃗ = ρa î
E
2ϵ0
Notar que no depende de la distancia al plano central.
b) Por el principio de superposición, este problema equivale a considerar la distribución de
carga de la parte a) más una esfera de densidad volumétrica de carga −2ρ.
El campo en el centro de la esfera, debido a la esfera misma es nulo, por simetría. Así, el
⃗
⃗ es el campo interior creado por la
campo total en el centro será, simplemente E(a/4)
donde E
distribución entre planos calculado anteriormente.

---

### Página 70

⃗ centro = ρa î
E
4ϵ0
Ahora, para obtener el campo en el punto P, calculemos primero el campo debido a la esfera
de carga usando la Ley de Gauss,

✞☎ ⃗ ′
⃗ x′ ) = qin
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

ˆˆ

ˆˆ

ˆˆ

☎
✞☎
✞☎ ⃗ ′
⃗ x′ ) = ✞
x ) · E(⃗
✝ ✆dS r̂ · E(r)r̂ = E(r) ✝ ✆dS
✝ ✆dS(⃗
S

S

S

ˆˆ

✞☎ ⃗ ′
⃗ x′ ) = E(r)4πr2
x ) · E(⃗
✝ ✆dS(⃗
S

y la carga encerrada por la superficie de Gauss es
qin = −2ρ

πa3
4π(a/4)3
= −ρ

Con esto
E(r) = −

ρa3
96r2 ϵ0

Esto corresponde al campo debido a la esfera, donde r es la distancia entre el punto P y el
centro de la esfera. En este caso, el centro de la esfera se encuentra en x = a/4, con lo que el
campo total en P sera

con | x |> a/2

ρa3
⃗ ) = ρa î −
E(P
î
2ϵ0
96ϵ0 (x − a/4)2

---

### Página 71

Problema
Calcule la fuerza por unidad de largo que se ejercen una huincha muy larga de ancho b y
densidad de carga σ y un alambre igualmente largo con densidad lineal de carga λ, puesto en
el mismo plano que la huincha a distancia d del borde inferior, como muestra la figura

#### Solución
Podemos optar por calcular la fuerza que ejerce la distribución lineal de carga sobre la distribución plana, o viceversa. Utilizaremos la primera opción, y para ello necesitamos obtener
el campo eléctrico generado por la distribución lineal. Esto ya ha sido resuelto anteriormente
con ley de Gauss, considerando la simetría cilíndrica del campo eléctrico en presencia de una
distribución linal infinita de carga

Si la superficie Gaussiana es un cilindro de radio r y largo h, y utilizando coordenadas
cilíndricas
ˆˆ
ˆ 2π
ˆ h
λh
✞☎ ⃗ ′
′
⃗ x)=
⃗
x ) · E(⃗
dϕr
dzr̂(ϕ) · E(r)r̂(ϕ)
= 2πrhE(r) =
✝ ✆dS(⃗
ϵ0
S
y entonces
⃗
E(r)
=

λ
r̂
2πϵ0 r

De esta forma, en el plano que contiene a ambas distribuciones, y definiendo las direcciones
î, ĵ (como se indica en la figura)

---

### Página 72

el campo eléctrico generado por la distribución lineal tiene la forma
λ
ĵ
2πϵ0 r
donde r es la distancia vertical entre ⃗x y el alambre. Fijando el origen de coordenadas según
lo indicado en la figura, calculemos la fuerza que se ejerce sobre una porción de largo L de la
distribución plana de carga con densidad σ. Un elemento de área de coordenadas (x, y) posee
una carga dada por
⃗ x) =
E(⃗

dq(x, y) = σdxdy
y el campo eléctrico en dicho punto debido a la distribución lineal es
⃗
E(x,
y) =

λ
ĵ
2πϵ0 (d + y)

Luego, la fuerza que se ejerce sobre este elemento de área es
dF⃗ (x, y) = dxdyσ

λ
ĵ
2πϵ0 (d + y)

consideremos la distribución dada por 0 ≤ x ≤ L, 0 ≤ y ≤ b. La fuerza neta sobre esta
porción es
ˆ L ˆ b
σλ
⃗
F =
ĵ
dx
0 2πϵ0 (d + y)
ˆ b
)b
σλL
σλL
)
ln(d + y)) ĵ
ĵ =
F⃗ =
2πϵ0 0 d + y
2πϵ0
$
#
σλL
d+b
⃗
ĵ
F =
ln
2πϵ0
d
y la fuerza por unidad de largo es

$
#
F⃗
σλ
d+b
=
ĵ
ln
L
2πϵ0
d

---

### Página 73

#### Capítulo 5
El potencial Electrostático
Vimos anteriormente que el campo Electrostático generado por una distribución de carga
se escribe en su forma más general como una integral de Coulomb
˚
(⃗x − ⃗x′ )
⃗
E(⃗x) =
d3 x′ ρ(⃗x′ )
4πϵ0
|⃗x − ⃗x′ |3
R3
Hemos establecido además una relación interesante entre el flujo del campo sobre una superficie cerrada y la carga encerrada por ésta (Ley de Gauss). Esta relación es consistente con
la ley de Coulomb y establece que el flujo del campo eléctrico sobre cualquier superficie cerrada
S es
ˆˆ
˚
✞ ☎ ⃗′ ⃗ ′
x)=
d3 x′ ρ(⃗x′ )
✝ ✆dS · E(⃗
ε
S
V (S)
Ahora, veremos una segunda ley muy importante en electrostática, y para enunciarla demostraremos el siguiente lema
⃗
∇
Demostración
Esta es trivial considerando que

⃗x − ⃗x′
=
−
| ⃗x − ⃗x′ |
|⃗x − ⃗x′ |3

'1/2
&
| ⃗x − ⃗x′ |= (x − x′ )2 + (y − y ′ )2 + (z − z ′ )2

y
⃗
∇

∂
∂
∂
=
î +
ĵ +
k̂
′
′
′
| ⃗x − ⃗x |
∂x | ⃗x − ⃗x |
∂y | ⃗x − ⃗x |
∂z | ⃗x − ⃗x′ |

veamos que ocurre con la componente según î
∂
∂
| ⃗x − ⃗x′ | î
î
=
−
∂x | ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |2 ∂x
'−1/2
∂
1&
2(x − x′ )î
î = −
(x − x′ )2 + (y − y ′ )2 + (z − z ′ )2
′
′
∂x | ⃗x − ⃗x |
| ⃗x − ⃗x | 2
∂
x − x′
î
î = −
∂x | ⃗x − ⃗x′ |
| x − x′ |3

---

### Página 74

El cálculo es análogo para las demás componentes, y se demuestra que
⃗
∇

⃗x − ⃗x′
=
−
| ⃗x − ⃗x′ |
|⃗x − ⃗x′ |3

¿Qué tendrá que ver esto con electrostática? No es difícil reconocer el parecido del campo
vectorial
⃗x − ⃗x′
|⃗x − ⃗x′ |3
con el campo electrostático, puesto que en su forma más general puede ser escrito como
˚
(⃗x − ⃗x′ )
⃗ x) =
d3 x′ ρ(⃗x′ )
E(⃗
4πϵ0
|⃗x − ⃗x′ |3
R3
Utilizando el lema recién demostrado, esto se reescribe como
˚
⃗
⃗
E(⃗x) = −
d3 x′ ρ(⃗x′ )∇
4πϵ0
| ⃗x − ⃗x′ |
R3
⃗ x) = −∇
⃗ 1
E(⃗
4πϵ0

˚

d3 x′ ρ(⃗x′ )

R3

| ⃗x − ⃗x′ |

Se obtiene que el campo eléctrico es menos el gradiente de un campo escalar. Se define el
potencial electrostático de una distribución de cargas como
˚
ρ(⃗x′ )
φ(⃗x) =
d3 x′
4πϵ0
| ⃗x − ⃗x′ |
R3
y el campo eléctrico cumple

⃗ x) = −∇φ(⃗
⃗ x)
E(⃗

Notar que es inmediato que el potencial de una carga puntual ubicada en ⃗x′ estará dado
por
φ(⃗x) =

q
4πϵ0 | ⃗x − ⃗x′ |

Potencial de una distribución discreta
Supongamos que se tiene una distribución discreta de cargas qj , j = 1, 2, ...N ubicadas en las
posiciones ⃗xj , j = 1, 2, ...N . El potencial de ésta distribución se puede obtener fácilmente a
partir del potencial de una sola carga utilizando el principio de superposición
N

φ(⃗x) =

1 %
qj
4πϵ0 i=1 | ⃗x − ⃗xi |

por supuesto, esto es consistente con la densidad de carga en términos de la delta de Dirac
ρ(⃗x) =

N
%
i=1

qi δ(⃗x − ⃗xi )

---

### Página 75

en efecto, de la definición para el potencial
φ(⃗x) =
4πϵ0

ρ(⃗x′ )
=
dx
| ⃗x − ⃗x′ |
4πϵ0
R3

˚

3 ′

N

1 %
φ(⃗x) =
qi
4πϵ0 i=1

˚

d3 x′

R3

N
%
qi δ(⃗x′ − ⃗xi )
| ⃗x − ⃗x′ | i=1

N

x′ − ⃗xi )
3 ′ δ(⃗

1 %
qi
=
dx
| ⃗x − ⃗xi |
4πϵ0 i=1 | ⃗x − ⃗xi |
R3

˚

N

1 %
qj
φ(⃗x) =
4πϵ0 i=1 | ⃗x − ⃗xi |

5.1.

Interpretación Física del Potencial

Supongamos que se tiene una distribución de carga en el espacio, ésta generará un campo
⃗ x). Consideremos el trabajo efectuado contra las fuerzas del campo al trasladar
eléctrico E(⃗
cuasiestáticamente una carga puntual q desde un punto ⃗x1 hasta el punto ⃗x2 , siguiendo una
trayectoria cualquiera Γ. Por cuasiestáticamente, se entiende que no se altera la energía cinética
al mover a la carga. Esto se puede lograr exclusivamente si la fuerza neta sobre la carga es cero
(recordar Teorema del Trabajo). De esta forma, debemos ejercer una fuerza de igual magnitud
y contraria a la fuerza electrostática que actúa sobre la carga. Esto es
ˆ ⃗x2
⃗ x)
d⃗x · q E(⃗
W =−
⃗
x1

Podría ser que este trabajo dependiera de la trayectoria utilizada para ir desde ⃗x1 hasta ⃗x2 .
Sin embargo, como
⃗ x) = −∇φ(⃗
⃗ x)
E(⃗
W =−

ˆ ⃗x2
⃗
x1

⃗ x) = q
d⃗x · q E(⃗

ˆ ⃗x2
⃗
x1

⃗ x)
d⃗x · ∇φ(⃗

Utilizando la parametrización de la curva Γ: ⃗x = ⃗x(l′ ), donde l ∈ [0, l]
ˆ l
d⃗x ⃗
W =q
dl′ ′ · ∇φ(⃗
x(l′ ))
dl

---

### Página 76

W =q

ˆ l

ˆ φ2
x(l′ ))
′ dφ(⃗
dφ = q (φ2 − φ1 )
dl
=q
dl′
φ1

Finalmente hemos obtenido
W = −q

ˆ ⃗x2
⃗
x1

⃗ x) = q (φ2 − φ1 )
d⃗x · E(⃗

Independiente de la curva Γ!
Si tomamos una carga unitaria, q = 1, la interpretación de éste resultado es como sigue:
El trabajo necesario para mover una carga unitaria cuasiestáticamente desde el punto x1 hasta
el punto x2 contra el campo eléctrico es igual a la diferencia de potencial entre x2 y x1
Ahora, notemos que
ˆ ⃗x2
⃗
x1

⃗ x) = − (φ2 − φ1 )
d⃗x · E(⃗

Por lo tanto, sobre una trayectoria cerrada
˛
⃗ x) = 0
d⃗x · E(⃗
el campo eléctrico es conservativo. Obsérvese que este resultado físico es consecuencia de
Coulomb y la geometría Euclídea
Notar que U (⃗x) = qφ(⃗x) es la Energía Potencial de una carga q en la posicion ⃗x. En
efecto, la fuerza asociada a esta interacción es
⃗ (⃗x) = q E(⃗
⃗ x)
F⃗ = −∇U

Otro enfoque para la electrostática
La introducción del campo escalar φ presenta muchas ventajas para resolver matemáticamente
el problema de la electrostática. Como vimos, si conocemos la distribución de carga, es decir, conocemos explícitamente ρ(⃗x), podemos calcular el campo resolviendo las integrales de
Coulomb. Sin embargo, como ya se dijo anteriormente, éstas integrales pueden ser complicadas,
un método alternativo sería resolver las integrales de Coulomb para el potencial
˚
d3 x′ ρ(⃗x′ )
φ(⃗x) =
4πϵ0
x − ⃗x′ |
R3 | ⃗

Notar que calcular esta integral es notoriamente más simple que calcular la integral para
el campo eléctrico. En primer lugar, no aparece ninguna cantidad vectorial. En segundo lugar,
el potencial sólo depende del inverso de la distancia a la fuente, en cambio el campo eléctrico
depende del cuadrado de la distancia. Notemos que una vez obtenido el potencial en todo el
⃗ x) = −∇φ(⃗
⃗ x),
espacio, determinar el campo eléctrico es muy sencillo, sólo basta con evaluar E(⃗
y todos sabemos que derivar es mucho más sencillo que integrar.
Ahora, aún no hemos dicho nada sobre qué hacer cuándo la distribución de carga no es
conocida, eso lo veremos más adelante, pero justamente el potencial electrostático es una herramienta muy poderosa a la hora de resolver ese tipo de problemas más complejos.

---

### Página 77

5.2.

Energía Potencial de una distribución de carga discreta

El trabajo necesario para traer una carga q cuasiestáticamente desde el infinito hasta un
punto ⃗x es, simplemente
W = qφ(⃗x)
suponiendo que el potencial en el infinito es cero (Esto se cumple si, por ejemplo, toda la
carga está localizada dentro de un volumen finito). Luego, esta carga ha adquirido una energía
potencial igual a U (⃗x) = qφ(⃗x). De la misma forma, una distribución de carga tiene una energía
potencial asociada, ya que un trabajo se debe realizar para mantener la distribución en su lugar.
Calculemos la energía potencial de un sistema electrostático de cargas puntuales. Para ello
inicialmente traemos una carga q1 hasta un punto cualquiera ⃗x1 . El trabajo necesario para esto
es nulo, ya que inicialmente no existe un campo eléctrico alguno que ejerza una fuerza sobre
q1 . Con esto
W1 = 0
y el sistema en este estado posee una energía potencial igual a
U = W1 = 0
Ahora, para traer una carga q2 hasta un punto ⃗x2 , como se aprecia en la figura

se requiere hacer un trabajo igual a
W2 = φ(x2 )q2 =

q1
q2
4πϵ0 | ⃗x1 − ⃗x2 |

Con esta configuración, el sistema tiene asociada una energía potencial dada por
U = W1 + W 2 =

q1
q2
4πϵ0 | ⃗x1 − ⃗x2 |

Ahora, para traer una tercera carga q3 , como se ve en la figura

---

### Página 78

el trabajo necesario será
W3 = q3 φ(⃗x3 ) =

#

q1
q2
+
4πϵ0 | ⃗x1 − ⃗x3 | 4πϵ0 | ⃗x2 − ⃗x3 |

$

q3

En síntesis, el trabajo necesario para formar esta configuración de 3 cargas a distancias r12 ,
r13 , r23 es
1 q1
1 q2
1 q1
q3 +
q3 +
q2
4πϵ0 r13
4πϵ0 r23
4πϵ0 r12
Y es igual a la energía potencial total de esta configuración, que se puede reescribir como
U = W 1 + W2 + W3 =

U=

U=

##

1 1 q1 q 2 q2 q1 q1 q3 q 3 q1 q 2 q3 q3 q2
(
+
+
+
+
+
)
2 4πϵ0 r12
r21
r13
r31
r23
r32

1 q2
1 q3
+
4πϵ0 r21 4πϵ0 r31

$

q1 +

#

1 q1
1 q3
+
4πϵ0 r12 4πϵ0 r32

$

q2 +

#

1 q1
1 q2
+
4πϵ0 r13 4πϵ0 r23

$ $
q3

(φ(⃗x1 )q1 + φ(⃗x2 )q2 + φ(⃗x3 )q3 )
Donde φ(⃗xi ) no es más que el potencial en la posición de la carga i debido a las demás
cargas. En general, para un sistema de N cargas, se tiene que la energía potencial asociada al
sistema es
N
1%
U=
qi φ(⃗xi )
2 i=1
U=

Esto se puede extender al caso continuo, donde la energía potencial de una distribución
continua de carga es, equivalentemente
˚
˚
′
′
U=
φ(⃗x )dq(⃗x ) =
d3 x′ ρ(⃗x′ )φ(⃗x′ )
V
V

---

### Página 79

5.3.

El dipolo Eléctrico

Definiremos una cantidad absolutamente general asociada con una distribución de cargas
ρ(⃗x), llamada Momento Dipolar
˚
p⃗ =
d3 x′⃗x′ ρ(⃗x′ )
V

donde V es un volumen que contiene todas las cargas. Notar en primer lugar que p⃗ es
un vector constante que dependerá de la forma en que están distribuídas las cargas. De cierta
forma, es una suma de las posiciones ponderadas por sus respectivas cargas. El momento dipolar
de una distribución discreta de N cargas es, por supuesto
p⃗ =

N
%

⃗xi qi

i=1

Dipolo Eléctrico
Estudiemos ahora un cierto tipo muy particular de distribución de carga. Primeramente, imaginemos 2 cargas cualquiera q1 , q2 separadas una distancia a, como muestra la figura

El momento dipolar está dado por
p⃗ = q1⃗x1 + q2⃗x2
Definamos además, el vector ⃗x como el vector posición del punto medio entre q1 y q2 , y la
dirección k̂ que apunta desde q1 hacia q2 . De esta forma, es claro que
a
⃗x1 = ⃗x − k̂
a
⃗x2 = ⃗x + k̂
luego

a
a
p⃗ = q1 (⃗x − k̂) + q2 (⃗x + k̂)

a(q2 − q1 )
k̂
Ahora, consideremos que ambas cargas son iguales en magnitud, pero de signo opuesto.
Digamos q2 = q, q1 = −q. Esto es lo que se conoce como dipolo eléctrico y entonces
p⃗ = (q1 + q2 ) ⃗x +

p⃗ = qak̂

---

### Página 80

En resumen, para un dipolo eléctrico, el momento dipolar es un vector de magnitud qa y su
dirección va siempre desde la carga negativa hacia la carga positiva. Esta configuración es muy
importante en electrostática.

5.4.

Campo de un Dipolo

Calculemos el potencial eléctrico en un punto P debido a un dipolo. Para ello consideremos
un dipolo en el eje vertical, como se muestra en la figura.

Por el principio de superposición, el potencial en el punto P está dado por
#
$
q
q
φ(P ) =
−
4πϵ0 r + r−

Donde, por el teorema del coseno

= r2 + d2 − 2dr cos ϑ
r+
r−
= r2 + d2 + 2dr cos ϑ

r+ = r

(
1 + (d/r)2 − 2(d/r) cos ϑ

Para el límite en que d << r, se puede desarrollar en series de Taylor
#
$
'−1/2 1
1&
1 + (d/r) − 2(d/r) cos ϑ)
1 − (d/r) + (d/r) cos ϑ + ...
=
=
r+
r
r

Conservaremos los términos hasta segundo orden en d/r, como en la expansión (1 + x)n ≈
1 + nx + n(n − 1)/2x2 , cuando x ≪ 1
#
$
1 − (d/r) + (d/r) cos ϑ
≈
r+
r
De forma análoga

≈
r−
r

#

1 − (d/r)2 − (d/r) cos ϑ

$

---

### Página 81

Con esto, el potencial en P puede aproximarse por
q 2d cos ϑ
4πϵ0 r
r
Si a = 2d es la separación entre las cargas del dipolo
φ(P ) ≈

φ(P ) ≈

p cos ϑ
q a cos ϑ
=
4πϵ0 r r
4πϵ0 r2

Donde p⃗ = aq ĵ es justamente el momento dipolar eléctrico. Notar entonces que el potencial
eléctrico debido a un dipolo microscópico (a << r) queda absolutamente determinado por
su momento dipolar p⃗ y disminuye según el cuadrado de la distancia (es un potencial más débil
que el de una carga puntual). Escribiendolo en su forma más general posible
φ(⃗x) =

p⃗ · r̂
p⃗ · ⃗x
=
4πϵ0 r
4πϵ0 | ⃗x |3

Notar que existe una clara simetría azimutal, pues el potencial no depende del ángulo polar ϕ

Fig. 5.1: Un dipolo eléctrico y sus líneas de campo eléctrico
Podemos obtener el campo eléctrico como el antigradiente del potencial
⃗ = ∂f r̂ + 1 ∂f ϑ̂ + 1 ∂f φ̂
∇f
∂r
r ∂ϑ
r sin φ ∂φ
El campo eléctrico sólo tendrá componentes en las direcciones r̂ y θ̂.
p cos ϑ
∂φ
=
∂r
2πϵ0 r3
1 ∂φ
p sin ϑ
Eϑ = −
=
r ∂ϑ
4πϵ0 r3
Er = −

Así
p
(2 cos ϑr̂ + sin ϑϑ̂)
4πϵ0 r3
El campo eléctrico debido a un dipolo microscópico disminuye según el inverso del cubo
de la distancia. Notar que un dipolo microscópico corresponde a un dipolo visto desde muy
lejos. Lo interesante es que si bien es eléctricamente neutro, produce un campo eléctrico, y
también interactúa con campos eléctricos externos. La explicación de ésto es que, si bien un
⃗ =
E

---

### Página 82

dipolo es neutro en su totalidad, posee una deformación eléctrica (cargas positivas y negativas
concentradas en distintos puntos del espacio).
El dipolo es importante en el estudio de la electrostática. Recordemos que hasta ahora las
leyes que hemos establecido son válidas en el vacío (en la ausencia de un medio material). ¿Cómo
se verán afectados los campos en un medio material?. El punto clave está en que la materia
está compuesta de moléculas, que si bien son eléctricamente neutras, poseen una deformación
eléctrica, y por lo tanto, un momento dipolar. Es por ésto que la materia se puede modelar
como una suma de muchos dipolos microscópicos, que generan campos eléctricos e interactúan
ante la presencia de un campo externo.

5.5.

Energía potencial de un dipolo

Supongamos un dipolo sumergido en un campo electrostático

La energía potencial asociada al dipolo será
U = −qφ(⃗x) + qφ(⃗x + ⃗a)
Podemos desarrollar φ(⃗x + ⃗a) en serie de Taylor (hasta primer orden)
φ(⃗x + ⃗a) = φ(x, y, z) +

∂φ(x, y, z)
∂φ(x, y, z)
∂φ(x, y, z)
ax +
ay +
az
∂x
∂y
∂z

⃗ x) · ⃗a
φ(⃗x + ⃗a) = φ(⃗x) + ∇φ(⃗
de forma que
⃗ x)
U = q⃗a · ∇φ(⃗
U = p⃗ · ∇φ(⃗x)
o, equivalentemente
⃗ x)
U = −⃗p · E(⃗

5.6.

Fuerza sobre un dipolo situado en un campo externo

El hecho de que el campo electrostático (y por lo tanto, la fuerza electrostática) sea conservativo, nos permite obtener la fuerza que siente un dipolo inmerso en un campo eléctrico
⃗ como el antigradiente de la energía potencial, esto es
externo E,

---

### Página 83

⃗
F⃗ = −∇U
!
"
⃗
⃗
⃗
F = ∇ p⃗ · E(⃗x)
⃗ E(⃗
⃗ x)
F⃗ = (⃗p · ∇)

---

### Página 84

Problema
Un pequeño objeto de masa m tiene una carga q y está suspendido por un hilo entre dos planos
infinitos verticales de densidad σ y −σ. La separación entre planos es d. Si el hilo forma un
ángulo ϑ con la vertical.
a) ¿Cuánto vale σ?
b) ¿Cuál será la diferencia de potencial entre los planos?

#### Solución
a) Como se tienen 2 planos inifnitos de carga, con densidad σ y −σ respectivamente, se tendrá que el campo eléctrico es nulo fuera de la región entre planos y será uniforme como indica
la figura para la región limitada por ambos. Esto es fácil de ver utilizando el principio de superposición. Si elegimos un eje horizontal, digamos, x̂,y el origen sobre el plano de la izqueirda,
tendremos que el campo debido al plano cargado positivamente es

⃗ 1 (⃗x) =
E

σ
î
2ϵ0
σ
− 2ϵ0 î

si x > 0
si x < 0

Ahora, para el plano cargado negativamente
σ
⃗ 2 (⃗x) = − 2ϵ0 î si x > d
E
σ
î si x < d
2ϵ0
El campo eléctrico total se obtiene de la suma de ambos campos, luego, es fácil ver que
⃗ = σ î
E
ϵ0
para la región entre planos, y es nulo fuera de ella.

---

### Página 85

Ahora, la esfera está en equilibrio, por lo que
Fx = −T sin ϑ + Fe = 0
En que Fe es la fuerza eléctrostática que actúa sobre la esfera.
Fy = T cos ϑ − mg = 0
El balance de fuerzas en el eje vertical entrega T = mg/ cos ϑ. Así
−mgtgϑ + qE = 0
De esta forma
⃗ = mgtgϑ î
E
q
Igualando, se obtiene que

mgtgϑ
σ
=
ϵ0
q

de donde la densidad superficial de carga está dada por
σ=

mgϵ0 tgϑ
q

b) La diferencia de potencial entre los planos se puede obtener integrando el campo eléctrico
sobre una trayectoria cualquiera entre la placa izquierda y la placa derecha. Por supuesto,
elegimos una trayectoria horizontal, de manera que el campo es paralelo en todo instante a la
curva
ˆ 0
ˆ d
mgtgϑd
mgtgϑ
⃗
dx =
φ(0) − φ(d) = −
d⃗x · E =
q
q
d
Ensayemos la interpretación física del potencial. Sabemos que si tomamos una carga unitaria
y la ponemos en algun punto sobre el plano izquierdo, ésta sentirá una fuerza hacia la derecha,
luego, si la soltamos, esta acelerará hasta pegarse al plano derecho. ¿Qué trabajo habrá que hacer para impedir que la carga acelere, y entonces, viaje desde 0 hasta d con velocidad constante?
Justamente será
mgtgϑd
φd − φ0 = −
q
. El signo negativo se debe a que deberíamos ejercer una fuerza contraria al movimiento de
desplazamiento.

---

### Página 86

Problema
Considere un anillo de radio R uniformemente cargado con densidad λ. ¿Cuál es el potencial
electostático a una distancia z sobre el eje del anillo?. En seguida, calcule el potencial en el eje
de un anillo de radio interior a y radio exterior b y densidad σ.

#### Solución
Tomemos un elemento infinitesimal de longitud en el anillo dl = Rdφ′ , como se aprecia en la
figura

Este elemento posee una carga
dq = dφ′ Rλ
Su contribución al potencial en P es
dφ′ Rλ
1 dq
√
=
dφ(P ) =
4πϵ0 r
4πϵ0 R2 + z 2
Luego, el potencial debido al anillo completo está dado por
ˆ 2π
dφ′
Rλ
√
φ(P ) =
4πϵ0 R2 + z 2
φ(P ) =

2πRλ
√
4πϵ0 R2 + z 2

notar que Q = 2πRλ es la carga total del anillo, luego
V (P ) =

Q
√
4πϵ0 R + z 2

---

### Página 87

Es fácil ver que si z >> R, se tiene el potencial de una carga puntual
1 Q
V (P ) =
4πϵ0 | z |
Ahora, el campo eléctrico en el punto P se puede obtener a partir del potencial como
⃗ ) = −∇φ(P
⃗
E(P
)

⃗ es necesario conocer φ(x, y, z). Aún así, veamos que sucede
Sin embargo, para evaluar ∇φ
con
−

∂φ
k̂
∂z

2zπRλ
⃗ )
k̂ = E(P
4πϵ0 (R2 + z 2 )3/2
y se recupera el resultado obtenido anteriormente para el campo en el eje. ¿Qué nos dice
esto acerca de las derivadas parciales con respecto a x e y del potencial en un punto de la forma
(0, 0, z)?
Ahora, para obtener el potencial de un disco de radios a y b, simplemente se considera la
superposición de anillos inifintesimales

Tomamos un anillo de radio r y ancho infinitesimal dr, sabemos que el potencial en el eje
está dado por
dQ
√
4πϵ0 r2 + z 2
donde dQ = σ2πrdr es la carga que contiene ese anillo
Luego
dφ(P ) =

dφ(P ) =

2πσ
drr
√
4πϵ0 r2 + z 2

Y el potencial es

ˆ b
drr
σ
√
φ(P ) =
2ϵ0 a
r2 + z 2
Sea u = r + z , con esto du = 2rdr , y por lo tanto
ˆ
ˆ
√
du
drr
√
=
= u1/2 = r2 + z 2
1/2
u
r2 + z 2
Finalmente
"
√
σ !√ 2
φ(P ) =
b +z − a +z
2ϵ0

---

### Página 88

Problema
Considere dos cascarones esféricos de radios a y b (a < b), el cascarón interior tiene densidad
superficial de carga constante Q y el exterior −Q. Encuentre la diferencia de potencial entre el
cascarón b y el a

#### Solución
El campo eléctrico en todo el espacio (de existir) es esféricamente simétrico. Lo mismo sucede
con el potencial, que será constante en una superficie esférica. Lo que se pide es
∆V = φ(b) − φ(a)

Se debe evaluar entonces
φ(b) − φ(a) = −

ˆ b
a

⃗ x)
d⃗x · E(⃗

⃗ x) y elegir un camino desde a a
Para evaluar la integral, claramente debemos encontrar E(⃗
b . Utilizamos una superficie Gaussiana S esférica de radio r, con a < r < b, como muestra la
figura

Por ley de Gauss

✞☎ ⃗ ′
⃗ x′ ) = E(r)4πr2 = Q
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

Luego, en la región entre los dos cascarones
⃗ x) =
E(⃗

Q
r̂
4πϵ0 r2

---

### Página 89

Dada la forma del campo, resulta inteligente elegir un camino radial
Γ : ⃗x = rr̂
r:a→b
Luego
d⃗x = drr̂
y
⃗ x) = dr
d⃗x · E(⃗
Entonces

Q
4πϵ0 r2

ˆ b

ˆ b
drQ
dr
Q
=−
φ(b) − φ(a) = −
4πϵ0 a r2
a 4πϵ0 r
ˆ b
Q
Q 1 ))a
dr
φ(b) − φ(a) =
=−
)
4πϵ0 a r2
4πϵ0 r b
Q
∆V =
4πϵ0

Notar que

#

1 1
−
b a

$

φ(b) − φ(a) < 0 → φ(b) < φ(a)
Es decir, cuesta más trabajo llevar una carga a a que a b desde el infinito

---

### Página 90

Problema
Considere la siguiente distribución de carga en coordenadas polares esféricas
ρ(r) = Crλ , r < a
Encuentre φ(r) tomando como punto de referencia el infinito
#### Solución
Encontremos primero el campo eléctrico. Se tiene una distribución esféricamente simétrica de
carga (la densidad sólo es función de la variable r). Por lo mismo, podemos encontrar el campo
por ley de Gauss, utilizando una superficie esférica de radio r > a concéntrica al centro de la
distribución

✞☎ ⃗ ′
⃗ x′ ) = 4πr2 = Qint
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

la carga encerrada por S está dada por la siguiente integral
˚
ˆ 2π
ˆ π ˆ a
3 ′
′
d x ρ(⃗x ) =
dϕ
dϑ
drr2 sin ϑCrλ
Qint =

V (S)

Qint =

4πC λ+3
a
=Q
λ+3

luego

Q
r̂, r > a
4πϵ0 r2
Si ahora se utiliza una superficie esférica de radio r < a, la carga interior será
⃗
E(r)
=

qint =

4πC λ+3
r
λ+3

Luego, el campo interior tiene la forma
⃗
E(r)
=

C λ+1
r r̂
λ+3

Para evaluar φ(r) debemos calcular
φ(r) = −

ˆ ∞
r

⃗ x)
d⃗x · E(⃗

Hay que tener cuidado al realizar este cálculo si r > a o r < a.

---

### Página 91

i) Potencial exterior r > a

φ(r) = −

ˆ ∞
r

⃗ x) =
d⃗x · E(⃗

ˆ ∞
r

⃗ x)
d⃗x · E(⃗

Por comodidad elegimos un camino radial
⃗x = r′ r̂
r′ : r → ∞
d⃗x = dr′ r̂

Luego
⃗ x) = dr′
d⃗x · E(⃗

φ(r) =

ˆ ∞
r

Q
4πϵ0 r′2

Q
dr′ Q
=
4πϵ0 r′2
4πϵ0

entonces
φ(r) =

#

− ′
r

Q
,r ≥ a
4πϵ0 r

$)
)∞
)
r

Caλ+3
,r ≥ a
φ(r) =
(λ + 3) ϵ0 r
ii) Si r < a

φ(r) =

ˆ ∞
r

⃗ x) =
d⃗x · E(⃗

ˆ a
r

⃗+
d⃗x · E

ˆ ∞
a

⃗ x)
d⃗x · E(⃗

)
)
la segunda integral se obtiene al evaluar φ(r))
con φ(r) el potencial exterior encontrado
r=a
anteriormente. La primera integral resulta (tomando un camino radial)
⃗x = r′ r̂
r′ : r → a
d⃗x = dr′ r̂

ˆ a
r

⃗ · ⃗x = dr′ C r′λ+1
E
λ+3
ˆ a
ˆ a
C
C r′λ+2 ))a
′ ′λ+1
⃗
d⃗x · E(⃗x) =
dr r
=
)
λ+3 r
λ+3λ+2 r
r

⃗ x) =
d⃗x · E(⃗

& λ+2
'
Caλ+2
Crλ+2
C
− rλ+2
−
= 2
a
(λ + 3)(λ + 2) (λ + 3)(λ + 2)
λ + 5λ + 6

---

### Página 92

la segunda integral es
ˆ ∞
a

⃗ x) =
d⃗x · E(⃗

Caλ+1
C aλ+2
=
ϵ0 a λ + 3
ϵ0 (λ + 3)

Finalmente, para r < a
φ(r) =

& λ+2
'
Caλ+1
C
− rλ+2
+ 2
a
ϵ0 (λ + 3) λ + 5λ + 6

---

### Página 93

Problema
Iones de carga q son acelerados desde el reposo hasta una diferencial de potencial ∆V0 , para
luego entrar a una región entre dos electrodos cilíndricos muy largos A y B, de radios a y
b respectivamente (a < b). El ión recorre media circunferencia de radio r0 describiendo una
trayectoria circular. Despreciando los efectos de borde y asumiendo que los cilindros son muy
largos en comparación al espacio que los separa, encuentre la diferencia de potencial ∆VBA

#### Solución
Primero debemos encontrar la velocidad con la que los iones ingresan a la región entre cilindros.
Éstos son acelerados a partir del reposo desde una región a potencial φ = V0 hasta una región
a potencial φ = 0. La energía inicial está dada por
E1 = qV0
la energía final (justo antes de ingresar entre los electrodos)
E2 = mv 2
Por conservación de la energía
2qV0
m
Ahora, dentro de la región entre cilindros existe un campo eléctrico radial que se puede
obtener con la ley de Gauss
E1 = E2 → v 2 =

---

### Página 94

Utilizando una superficie cilíndrica de radio r (a < r < b) y altura h, se tiene
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 2πrhE(r) = qin
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
donde la carga encerrada por la superficie S es
qin = σ2πha
σ es la densidad superficial de carga sobre el cilindro de radio a. De aquí
2πrhE(r) =

σh2πa
ϵ0

σa
⃗
E(r)
=
r̂
ϵ0 r
En particular

⃗ 0 ) = σa r̂
E(r
ϵ 0 r0

Este campo es por supuesto el responsable de la fuerza que siente un ión (en dirección
radial), y que permite la trayectoria circular. El equilibrio de fuerzas en la dirección radial
sobre un Ión de carga q es
⃗ 0) = q
q E(r

σa
v2
r̂ = −m r̂
ϵ 0 r0
r0

de donde
σa
2qV0
= −m
ϵ 0 r0
mr0
la densidad superficial de carga sobre el cilindro A resulta ser
q

σ=−

2ϵ0 V0
a

y el campo eléctrico queda, para r, a < r < b
2ϵ0 V0 a
σa
⃗
r̂ = −
r̂
E(r)
=
ϵ0 r
a ϵ0 r
V0
⃗
E(r)
= −2 r̂
r
La diferencia de potencial entre los cilindros es
ˆ b
⃗ x)
∆V = φ(b) − φ(a) = −
d⃗x · E(⃗
a

tomando un camino radial
$
ˆ b
ˆ b #
ˆ b
dr
2V0
⃗
∆V = −
d⃗r · E(r) = −
dr −
= 2V0
r
a
a
a r
∆V = φ(b) − φ(a) = 2V0 ln (b/a)

---

### Página 95

Problema
Un plano infinito y uniforme de carga eléctrica con densidad σ pasa por un punto O. Por O
hay una recta OX que es perpendicular al plano. A distancia a de 0 se encuentra una carga
eléctrica puntual - q.
a) Calcule el potencial eléctrico resultante en un punto P (x) cualquiera entre A y O
b) Una partícula de masa m y carga eléctrica -e se libera desde el punto medio entre O y A.
¿Con qué velocidad choca contra el plano de carga?

#### Solución
Para calcular el potencial en el eje x̂ podemos primero calcular el campo eléctrico. Naturalmente,
⃗ 1 el campo eléctrico debido al plano
éste se puede obtener fácilmente por superposición. Sea E
infinito, sabemos que éste es uniforme y no depende de la distancia al plano. Para x > 0 es
⃗ 1 (x) = σ î
E
2ϵ0
Podemos obtener el potencial asociado al plano integrando el campo eléctrico sobre una
trayectoria horizontal que pasa por Ox, entre ⃗x1 = xî y ⃗x2 = Rî (R > x)
φ1 (x) − φ1 (R) =

ˆ ⃗x2
⃗
x1

⃗ x′ ) =
d⃗x · E(⃗
′

ˆ R
x

dx′

σ
2ϵ0

σ
σ
R−
x
2ϵ0
2ϵ0
El potencial en un punto x debido a la carga puntual −q está dado por
φ1 (x) = φ1 (R) +

φ2 (x) =
por el principio de superposición
φ(x) =

−q
4πϵ0 | a − x |

−q
σ
σ
+ φ1 (R) +
R−
x
4πϵ0 | a − x |
2ϵ0
2ϵ0

---

### Página 96

b) Si colocamos una partícula de masa m y carga -e, ésta sentirá una fuerza que la acelerará en la dirección -î. En teoría, una vez que se mueve la carga ocurren fenómenos complejos que
no estamos considerando en el caso estático. Suponiendo que podemos despreciar estos efectos,
y utilizar las leyes estáticas, la energía debe conservarse (campo electrostático es conservativo)
U (a/2) = U (0) + mvf2
−eφ(a/2) = −eφ(0) + mvf2
vf2 =
2e
vf2 =
m

#

2e
(φ(0) − φ(a/2))
m

1 −q
1 −2q
σ
−
+
a
4πϵ0 a
4πϵ0 a
4ϵ0

2e
vf2 =
m

#

q
σa
+
4πϵ0 a 4ϵ0

$

$

---

### Página 97

Problema
Una varilla delgada de longitud L tiene una carga uniforme definida por su densidad lineal λ.
Calcular el potencial en un punto cualquiera del espacio que lo rodea

#### Solución
Sea P un punto de coordenadas (x, y). Tomemos un elemento diferencial de longitud en la
barra, a una distancia l del origen, como se aprecia en la figura

La contribución de este elemento infinitesimal al potencial en P es
dφ =
yr=

(
(x − l)2 + y 2 . Con esto

φ(P ) =
4πϵ0

1 dlλ
4πϵ0 r

ˆ L

dlλ
(
(x − l)2 + y 2

Sea t = x − l, con lo que dt = −dl, así
λ
φ(P ) = −
4πϵ0

ˆ x−L
x

dtλ
(
t2 + y 2

Aquí es inmediato que se usa la sustitución t = y tan ϑ, luego dt = ysec2 ϑdϑ. Con esto
tenemos
ˆ
ˆ
ˆ
dϑsec2 ϑy
dt
(
(
=
= dϑsecϑ
y 2 (1 + tan2 ϑ)
t2 + y 2
Y esta integral es muy familiar y vale
ˆ
dϑsecϑ = ln(secϑ + tan ϑ)

---

### Página 98

Ahora, tanϑ = yt y secϑ =

√

t2 +y 2
y

Con todo esto, tenemos
φ(P ) = −
φ(P ) = −
Finalmente

)x−L
(
λ
)
(ln(t + t2 + y 2 )))
4πϵ0
x

"
(
(
λ !
ln(x + x2 + y 2 ) − ln(x − L + (x − L)2 + y 2 )
4πϵ0

λ
φ(P ) = −
ln
4πϵ0
y llamando

(
x + x2 + y 2
(
(x − L + (x − L2 ) + y 2 )

(
a = x2 + y 2
(
b = (x − L)2 + y 2

λ
φ(P ) = −
ln
4πϵ0

#

x+a
(x − L + b)

$

Fig. 5.2: La figura muestra las curvas equipotenciales del alambre de carga

---

### Página 99

Problema
Encuentre el potencial dentro y fuera de una esfera sólida cargada uniformemente cuyo radio
es R y su carga total es Q. Use infinito como punto de referencia.
#### Solución
Para encontrar el potencial en todo el espacio, se puede determinar primeramente el campo
eléctrico debido a la distribución esférica de carga. Considerando el origen en el centro de la
esfera, por argumentos de simetría es fácil ver que el campo eléctrico debe ser radial y su magnitud una función de la distancia r al origen.
Campo interior
Ahora, para el campo interior, se elige una superficie de Gauss esférica y de radio r < R, como
se aprecia en la figura

Luego, utilizamos la ley de Gauss para obtener el campo eléctrico
ˆˆ
qin
✞☎ ⃗ ⃗
r) =
✝ ✆dS · E(⃗
ϵ0
S
⃗ = E(r)r̂ y dS
⃗ = dS r̂, luego la integral de flujo del campo eléctrico es, simplemente
donde E
ˆˆ
ˆˆ
ˆˆ
✞☎
✞☎
✞☎ ⃗ ⃗
r) = ✝ ✆dSE(r)r̂ · r̂ = ✝ ✆dSE(r)
✝ ✆dS · E(⃗
S

S

S

Como en la superficie S el radio r es constante
ˆˆ
ˆˆ
✞☎
✞☎
✝ ✆dSE(r) = E(r) ✝ ✆dS = E(r)4πr
S

S

Por otra parte, la carga encerrada por la superficie de Gauss es
˚
d3 x′ ρ(⃗x′ )
qin =
V (S)

como la esfera está cargada uniformemente, su densidad volumétrica de carga es
ρ=

Q
3Q
=
V
4πR3

---

### Página 100

De esta forma, y considerando d3 x′ = r2 sinϑdrdϑdφ
qin =

ˆ 2π

dφ

qin = 4πρ

ˆ π

dϑsinϑ

ˆ r

drr2 ρ

ˆ r

Qr3
drr2 = 4πρ r3 = 3
R

Finalmente, la ley de Gauss queda
Qr3
ϵ0 R 3

E(r)4πr2 =
de donde, para r < R
E(r) =

Qr
4πϵ0 R3

Campo exterior
Ahora, para obtener el campo exterior, se construye una superficie de Gauss esférica y ahora
de radio r > R

El flujo eléctrico sobre esta superficie es, de manera análoga al caso anterior
ˆˆ

✞☎ ⃗ ⃗
✝ ✆dS · E· = E(r)4πr
S

mientras que la carga encerrada en este caso está dada por
qin = Q
Con esto
E(r)4πr2 =

E(r) =

Q
ϵ0

Q
4πϵ0 r2

En resumen, se tiene
⃗ x) =
E(⃗

Qr
r̂
4πϵ0 R3
Q
r̂
4πϵ0 r2

si | ⃗x |≤ R
si | ⃗x |> R

---

### Página 101

Notar que el campo es continuo al atravesar un volumen cargado, pero no es diferenciable
Potencial exterior
Ahora, para obtener el potencial electrostático, calculamos la integral de línea
ˆ r
⃗
⃗ · dr
φ(r) = −
E
∞

⃗ = drr̂, así, para r > R
a lo largo de una trayectoria radial. Luego dr
ˆ r
E(r)dr
φ(r) = −
∞

ˆ r

Q
Q
φ(r) = −
dr
=−
4πϵ0 r
4πϵ0
∞
φ(r) =

ˆ r

dr 2
r
∞

Q
4πϵ0 r

Potencial interior
Ahora, para r < R, tenemos
drE(r) −

ˆ r

drE(r)

Q
dr
−
φ(r) = −
4πϵ0 r2
∞

ˆ r

dr

Qr
4πϵ0 R3

ˆ r

drr

φ(r) = −

ˆ R
∞

ˆ R

R

R

Q
Q
−
φ(r) =
4πϵ0 R 4πϵ0 R3
φ(r) =

Q(R2 − r2 )
Q
+
4πϵ0 R
8πϵ0 R3

φ(r) =

φ(r) =

R

Q(3R2 − r2 )
8πϵ0 R3

Q(3R2 −r2 )
8πϵ0 R3
Q
4πϵ0 r

si r ≤ R
si r > R

---

### Página 102

Problema
Un alambre cuya densidad lineal de carga es λ se extiende en el eje z desde z = −d hasta z = d.
a) Calcule el potencial en un punto z > d sobre el eje del alambre
b) Cuál es el cambio de energía potencial de un electrón si se mueve de z = 4d hasta z = 3d?
c) Si el electrón parte del reposo desde z = 4d, cuál es su velocidad en z = 3d?
Observación: No considere efectos gravitacionales
#### Solución Problema 2
a) Tomamos un elemento diferencial de longitud dl a una distancia l del origen:

El potencial a una distancia z > d sobre el eje del alambre debido a este elemento infinitesimal de carga está dado por
dφ(z) =

dq
4πϵ0 (z − l)

dφ(z) =

dq
4πϵ0 (z − l)

donde dq = dlλ

dφ(z) =
con esto, el potencial total está dado por

dlλ
4πϵ0 (z − l)

λ
φ(z) =
4πϵ0

ˆ d

dl
−d (z − l)

sea u = z − l, luego du = −dl
λ
φ(z) = −
4πϵ0

ˆ z−d

du
u

λ
φ(z) =
ln
4πϵ0

#

$

z+d

z+d
z−d

---

### Página 103

b) Un electrón se mueve desde z = 4d hasta z = 3d, luego, su cambio en energía potencial
está dado por
∆U = U (4d) − U (3d) = −e (φ(4d) − φ(3d)) = eφ(3d) − eφ(4d)
#

$
λ
λ
ln2 −
ln( )
∆U = e
4πϵ0
4πϵ0
# $
λ
∆U = e
ln
4πϵ0
c) Por conservación de la energía
U (4d) + K(4d) = U (3d) + K(3d)
como el electrón parte del reposo, K(4d) = 0, luego
U (4d) = U (3d) + K(3d)
U (4d) − U (3d) = K(3d)
luego, el cambio de energía potencial calculado en la parte b) es equivalente a la energía
cinética que adquiere el electrón
# $
λ
K(3d) = ∆U = e
ln
4πϵ0
#
$
mv 2
λ
ln
=e
4πϵ0
# $
2λ
v= e
ln
4πϵ0 m

---

### Página 104

Problema
Se tiene una distribución rectilínea de carga de densidad λ homogénea. Un punto P está a una
distancia r de la distribución, y su proyección sobre la recta de carga está a las distancias l1 y
l2 de sus extremos.

a) Calcule el campo eléctrico en P
b) Vea que sucede cuando r es mucho mayor que l1 y l2
c) Haga una aproximación para los casos en que r es mucho menor que l1 y l2 ¿Qué ocurre
cuando l1 y l2 tienden a infinito? Compruebe su resultado con Ley de Gauss
d) Obtenga el potencial en el punto P debido a un alambre infinito de carga
#### Solución
a) Tomemos un elemento diferencial de longitud, a una distancia l del origen, como se aprecia
en la figura

De la Ley de Coulomb, este elemento diferencial de carga crea un campo eléctrico en P que
está dado por
1 dq(⃗x − ⃗x′ )
⃗
dE(P ) =
4πϵ0 | ⃗x − ⃗x′ |3

---

### Página 105

En este caso, tenemos
⃗x = rr̂
donde r̂ es el vector radial en coordenadas cilíndricas que apunta desde el origen hasta el
punto P . Además
⃗x′ = lk̂
Luego
⃗x − ⃗x′ = rr̂ − lk̂
| ⃗r − ⃗r′ |=

√

r2 + l2

De esta forma , la contribución del elemento diferencial al campo es
⃗ )=
dE(P

1 λdl(rr̂ − lk̂)
4πϵ0 (r2 + l2 )3/2

Utilizando el principio de superposición, el campo total en P será la suma de todas las
contribuciones infinitesimales de la distribución, esto es
⃗ )=
E(P

λ
4πϵ0

#

ˆ l1

dl
rr̂
− k̂
2 3/2
−l2 (l + r )

ˆ l1

ldl
2 3/2
−l2 (l + r )

$

Ahora, la integral
ˆ

ldl
(r2 + l2 )3/2

se resuelve con la sustitución u = r2 + l2 , luego du = 2ldl, con esto
ˆ
ˆ
du
ldl
=
= − 1/2 = − √
3/2
3/2
(r + l )
u
u
r + l2
y la integral
ˆ

dl
(r2 + l2 )3/2

se resuelve con la sustitución trigonométrica l = rtanϑ, asi dl = rsec2 ϑdϑ
ˆ

ldl
=
(r + l2 )3/2
ˆ

ˆ

dϑrsec2 ϑ
=
(r2 + r2 tan2 ϑ)3/2

ldl
=
(r + l2 )3/2

ˆ

dϑ
r2 secϑ

Ahora, de la figura vemos que sin ϑ = √r2l+l2

=

ˆ

dϑrsec2 ϑ
r3 sec3 ϑ

sinϑ
r2

---

### Página 106

luego
ˆ

ldl
(r2 + l2 )3/2

=

l
√
r r2 + l2

Con esto, el campo total en P es
#
) l1
) l1 $
l
λ
)
)
⃗
E(P ) =
rr̂ 2 √
) + k̂ √ 2
)
4πϵ0
r r + l −l2
r + l −l2
⃗ )= λ
E(P
4πϵ0

r̂
r

l2

l1

(
+(
r2 + l12
r2 + l22

+ k̂

(
−(
r2 + l12
r2 + l22

b) En el límite cuando r >> l1 y r >> l2 , se tiene que ( a cero orden)
*
*
r + l1 ≈ r2 + l22 ≈ r
Luego el campo queda

⃗ )≈ λ
E(P
4πϵ0

#

r̂
r

#

⃗ )≈
E(P

l1 l2
+
r
r

$

+ k̂

#

1 1
−
r r

$$

λ l1 + l2
r̂
4πϵ0 r r

pero λ(l1 + l2 ) no es más que la carga total contenida en la distribución, digamos, q, luego
el campo toma la forma
q
⃗ ≈
r̂
E
4πϵ0 r2
que es el campo de una carga puntual
c) Ahora, en el límite cuando l1 >> r y l2 >> r, se tiene que
*
r2 + l12 ≈ l1
*
r2 + l22 ≈ l2

y el campo queda
⃗ )≈
E(P

λ 2
( r̂ + k̂( − ))
4πϵ0 r
l1 l2

y si l1 → ∞, l2 → ∞, se tiene
λ
r̂
2πϵ0 r
que es el campo eléctrico de un alambre infinito de carga.
⃗ )≈
E(P

---

### Página 107

Comprobemos este último resultado con la Ley de Gauss. Tomando como superficie Gaussiana un cilindro de radio r y cuyo eje de simetría coincide con el de la distribución lineal de
carga

Es claro que debido a que la distribución es infinita, el campo posee una simetría cilíndrica,
luego el campo es radial y depende únicamente de la distancia r. Con esto, no hay flujo por
las tapas del cilindro, y en el manto el campo eléctrico es siempre normal a la superficie y de
mangnitud constante, luego
ˆˆ
¨
¨
✞☎ ⃗
⃗
dS r̂E(r)r̂ = E(r)
dS = E(r)2πrl
✝ ✆dS · dE =
S

manto

manto

la carga encerrada por este cilindro es qin = λl, luego
E(r)2πrl =
E(r) =

λl
ϵ0

λ
2πrϵ0

El mismo resultado obtenido anteriormente
d) El campo del alambre infinito está dado por
⃗
E(r)
=

λ
r̂
2πrϵ0

Sabemos que en electrostática se cumple
⃗
⃗
E(r)
= −∇φ(r)
Debido a la simetría, el potencial será sólo función de r, luego
dφ
⃗
∇φ(r)
=
r̂
dr
con esto
V (r) = −

ˆ

V (r) = −

drE(r) + C

λ
ln r + C
2πϵ0

---

### Página 108

Donde C es una constante arbitraria. Notar que el potencial diverge en el infinito, ésto debido a que la carga eléctrica total no es finita. (Sólo en esos casos podemos fijar el potencial
igual a cero en infinito)
Notar que las superficies equipotenciales son cilindros de radio r, y que para r = 1
φ(1) = C
Luego la constante C no es más que el potencial de todos los puntos que están sobre el
manto de cilindro de radio unitario! Así
φ(r) = −

λ
ln r + V (1)
2πϵ0

---

### Página 109

Problema
Dos cables infinitos paralelos al eje X poseen densidad de carga uniforme λ y −λ. Ellos están
a distancia a del origen.
a) Encuentre el potencial en un punto (x, y, z) usando el origen como punto de referencia.
b) Demuestre que las superficies equipotenciales son cilindros circulares
#### Solución
a) Tenemos dos alambres infinitos cada uno a distancia a del origen, como se aprecia en la
figura (notar que el eje X sale de la página)

Por el principio de superposición, el potencial total en el punto P será la suma de los
potenciales debidos a cada distribución individual. El potencial debido al alambre de densidad
λ es
λ
ln s+ + C1
φ1 (P ) = −
2πϵ0
y el potencial debido al alambre de densidad −λ es
φ1 (P ) =

λ
ln s− + C2
2πϵ0

Ahora, como nos piden que la referencia sea el origen, las constantes C1 y C2 deben satisfacer
φ1 (a) = 0 = φ2 (a)
Con esto
φ1 (a) = −
φ2 (a) =

λ
λ
ln a + C1 = 0 → C1 =
ln a
2πϵ0
2πϵ0

λ
λ
ln a + C2 = 0 → C2 = −
ln a
2πϵ0
2πϵ0

Notar que C1 + C2 = 0.

---

### Página 110

El potencial en el punto P es
φ(P ) = φ1 (P ) + φ2 (P ) = −

λ
λ
ln s+ +
ln s−
2πϵ0
2πϵ0

Si P = (x, y, z), entonces
(
(y − a)2 + z 2
(
s+ = (y + a)2 + z 2

s+ =
Finalmente, el potencial es
φ(P ) = +

(
(
λ
λ
ln( (y + a)2 + z 2 ) −
ln( (y − a)2 + z 2 )
2πϵ0
2πϵ0
2(
(y
+
a)
+
z
λ
φ(P ) =
ln (
2πϵ0
(y − a)2 + z 2
λ
ln
φ(P ) =
4πϵ0

#

(y + a)2 + z 2
(y − a)2 + z 2

$

b) Las superficies equipotenciales están dadas por
(y + a)2 + z 2
=k
(y − a)2 + z 2
donde k es una constante. Esto equivale a
(y + a)2 + z 2 = k((y − a)2 + z 2 )

O equivalentemente

y 2 + 2ay + a2 + z 2 = k(y 2 − 2ay + a2 + z 2 )

y 2 (k − 1) + z 2 (k − 1) + a2 (k − 1) − 2ay(k + 1) = 0

Dividiendo por k − 1
k+1
=0
k−1
Notar que la ecuación de una circunferencia con centro en y0 y radio R es
y 2 + z 2 + a2 − 2ay

(y − y02 ) + z 2 = R2
y 2 + z 2 − 2yy0 + (y02 − R2 ) = 0

De aquí es claro que en planos perpendiculares a los alambres, las equipotenciales son
circunferencias con
k+1
y0 = a
k−1

---

### Página 111

Despejando se obtiene que

√
2a k
R=
|k−1|

En definitiva las superficies equipotenciales son cilindros

Fig. 5.3: Equipotenciales en plano y − z son curvas circulares

---

### Página 112

Problema
Un dipolo con momento dipolar p⃗ se localiza a una distancia r de una barra muy delgada con
largo infinito y homogéneamente cargada con densidad lineal de carga λ > 0. Asuma que el
dipolo está orientado con el campo eléctrico debido a la barra cargada como muestra la figura

a) Suponiendo que la separación fija l entre las cargas que conforman el dipolo es tal que
l << r, determine la fuerza sobre el dipolo, a primer orden en l/r
b) Partiendo de la respuesta del inciso anterior, demuestre que la fuerza sobre el dipolo puede
ser escrita como
!
"
⃗
⃗
⃗ x)
F (⃗x) = p⃗ · ∇ E(⃗
(válido para un dipolo puntual)

#### Solución
Ya fue obtenido anteriormente el campo eléctrico de una distribución lineal de carga muy larga
y de densidad λ. Definiendo un sistema de coordenadas cilíndricas, donde el eje z coincide con
el eje de la barra, como se ve en la figura

El campo eléctrico creado por la barra está dado por
⃗
E(r)
=

λ
r̂
2πϵ0 r

La fuerza sobre el dipolo está dada por
⃗ + l/2) − q E(r
⃗ − l/2) = q (E(r + l/2) − E(r − l/2)) r̂
F⃗ = q E(r
$
−
r̂
r + l/2 r − l/2
qλ
r̂
F⃗ =
−
2πϵ0 r 1 + 2rl
1 − 2rl

qλ
F⃗ =
2πϵ0

#

---

### Página 113

qλ
F⃗ =
2πϵ0 r

2#

l
1+
2r

$−1

#

l
− 1−
2r

$−1 3

r̂

Recordar la expansión a primer orden de (1 + x)n , buena aproximación cuando x << 1
(1 + x)n ≈ 1 + nx
De esta forma, la fuerza se puede aproximar (en primer orden de l/r)
#
#
$$
qλ
l
l
⃗
F ≈
1−
r̂
− 1+
2πϵ0 r
2r
2r
# $
qλ
l
⃗
F ≈
−
r̂
2πϵ0 r
r
−qlλ
−pλ
F⃗ ≈
r̂
=
r̂
2πϵ0 r2
2πϵ0 r2
donde p es la magnitud del momento dipolar del dipolo
b) Notar que si l << r, se espera obtener para la fuerza el resultado que se obtuvo para el
dipolo puntual
!
"
⃗ E(⃗
⃗ x)
F⃗ (⃗x) = p⃗ · ∇
Utilizando coordenadas cilíndricas, y recordando la naturaleza radial del campo eléctrico
$
#
!
"
∂
⃗
⃗
⃗
⃗
F (r) = p⃗ · ∇ E(r) = pr̂ · r̂ E(r)
∂r
$
#
$
#
λ
∂
∂ ⃗
⃗
E(r) = p
r̂
F (r) = p
∂r
∂r 2πϵ0 r

λ
r̂
2πϵ0 r2
que es el mismo resultado que se obtuvo en la parte anterior
F⃗ (r) = −p

---

### Página 114

Problema
Considere un dipolo de momento dipolar p⃗ formando un ángulo ϑ con la horizontal. Suponga
⃗ = E x̂.
que existe un campo eléctrico externo uniforme dado por E
a) Calcule la fuerza total y explícitamente el torque que se ejerce sobre el dipolo
b) ¿Qué ocurre si el campo no es uniforme?

#### Solución
Como se aprecia en la figura, se tiene que la fuerza total sobre el dipolo será
F⃗ = F⃗+ + F⃗−
F⃗ = qE î − qE î = ⃗0
La fuerza neta sobre el dipolo en un campo externo uniforme es nula. Calculemos ahora el
torque que se ejerce sobre el dipolo, con respecto a su centro de masa(origen)
⃗τ = ⃗r+ × F⃗+ + ⃗r− × F⃗−
⃗τ = (a cos ϑî + a sin ϑĵ) × qE î + (−acosϑî − a sin ϑĵ) × −qE î
⃗τ = a sin ϑĵ × qE î + a sin ϑĵ × qE î
⃗τ = 2a sin ϑĵ × qE î = −2aqsinϑE k̂
Existe un torque sobre el dipolo, a pesar que la fuerza neta sobre él es nula! La dirección del
torque es según −k̂ (hacia dentro de la página). Es decir, el dipolo tiende a girar en el sentido
del reloj de forma que el dipolo se alinea con respecto al campo. (Deja de haber torque cuando
p⃗ y Ê son paralelos). Ahora, la magnitud del momento dipolar es
p = 2aq
Luego, se puede reescribir
⃗τ = −pEsinϑk̂
Escrito en forma más general, se tiene
⃗
⃗τ = p⃗ × E
que es consistente con la expresión general para el torque sobre un dipolo de momento dipo⃗
lar p⃗ situado en un campo eléctrico E.

---

### Página 115

b) Si el campo externo no es uniforme, seguirá existiendo un torque sobre el dipolo hasta
que éste esté alineado con respecto al campo eléctrico. Eso sí, la fuerza neta sobre el dipolo
no necesariamente será nula , por lo que además de girar, se desplazará hacia donde el campo
eléctrico sea más intenso.

---

### Página 116

Problema
Se tiene dos anillos coaxiales de radio R cargados uniformemente (cargas totales q1 y q2 desconocidas) y separados una distancia 2a. El trabajo necesario para traer una carga q desde
el infinito hasta el centro de cada uno de los anillos es W1 y W2 respectivamente. Calcule las
cargas totales q1 y q2
#### Solución
Resolvamos primero el problema auxiliar del potencial en el eje de un anillo con carga q y radio
R

El potencial está dado por
φ(⃗x) =
4πϵ0

dx′ λ
x − ⃗x′ |
Γ |⃗

˛

interesa obtener el potencial para ⃗x = z k̂. La parametrización de la distribución de carga
está dada por
⃗x′ = Rr̂(ϑ)
r̂(ϑ) = cos ϑî + sin ϑĵ
dx = Rdϑ
Luego
φ(z) =
4πϵ0
y la densidad lineal es

ϑ : 0 → 2π
ˆ 2π

dϑ √

λR
z 2 + R2

=

λR
√
2ϵ0 z 2 + R2

q
2πR
q
√
φ(z) =
4πϵ0 z 2 + R2
λ=

Consideremos ahora dos anillos separados una distancia 2a

---

### Página 117

El potencial sobre un punto a distancia z del origen es
φ(z) =
donde

q
q
(1
(2
+
4πϵ0 z12 + R2 4πϵ0 z22 + R2
z2 = z

z1 = z − 2a
φ(z) =
Además se tiene

q
q1
(
√2
+
4πϵ0 (z − 2a)2 + R2 4πϵ0 z 2 + R2

$
q2
q1
√
+
W1 = qφ(2a) = q
4πϵ0 R 4πϵ0 4a2 + R2
#
$
q1
q2
√
W2 = qφ(0) = q
+
4πϵ0 4a2 + R2 4πϵ0 R
#

De aquí se puede resolver para q1 y q2
√
& √
'
πϵ0 R 4a2 + R2 W1 4a2 + R2 − W2 R
q1 =
qa2
√
& √
'
πϵ0 R 4a2 + R2 W2 4a2 + R2 − W1 R
q2 =
qa2

---

### Página 118

Problema
Muestre que la energía potencial almacendada en una esfera sólida cargada uniformemente con
carga Q y de radio R es
#
$
Q2
U=
5 4πϵ0 R
#### Solución
De la forma general para la energía potencial de una distribución de carga
˚
U=
d3 x′ ρ(⃗x′ )φ(⃗x′ )
V
Utilizando coordenadas esféricas
ˆ π
ˆ R
ˆ
1 2π
U=
dϕ
dϑ sin ϑ
drr2 ρ(r, ϕ, ϑ)φ(r, ϕ, ϑ)
2 0
la densidad de carga es constante
ρ(r, ϕ, ϑ) =

Q
3Q
=
4/3πR3
4πR3

y el potencial interior fue calculado anteriormente
φ(r, ϕ, ϑ) = φ(r) =

con esto

Q(3R2 − r2 )
8πϵ0 R3

ˆ R
3Q
2 Q(3R − r )
U = 4π
drr
8πR3 0
8πϵ0 R3
#
$
ˆ R
3Q2
3Q2
R5
R −
U=
drr (3R − r ) =
16πϵ0 R6 0
16πϵ0 R6

U=

4 5 3 Q2
3Q2
×
R =
16πϵ0 R6 5
5 4πϵ0 R

---

### Página 119

Problema
Una distribución de fuentes localizadas en un volumen V se define como
+
ρ(⃗x) si ⃗x ∈ V
ρ=
0 si ⃗x ∈
/V
Demuestre que en primera aproximación en la magnitud de V (diámetro máximo), el campo
eléctrico distante debido a fuentes localizadas en V , puede descomponerse en
⃗ x) =
E(⃗

" ⃗x
⃗x
1 !
⃗
q(V )
−
p
⃗
(V
)
·
∇
4πϵ0
| ⃗x |3 4πϵ0
| ⃗x |3

donde

˚

d3 x′ ρ(⃗x′ )

˚

d3 x′ ρ(⃗x′ )⃗x′

q(V ) =

V

es la carga total de la distribución, y
p⃗(V ) =

V

es el momento dipolar de la distribución
#### Solución
Pondremos el origen ⃗0 ∈ V , con lo que por campo distante estamos pensando en
| ⃗x |>>| ⃗x′ |, ⃗x′ ∈ V
es decir, la distancia a la distribución es mucho mayor que las dimensiones de ésta

El campo está dado por la integral de Coulomb
˚
˚
⃗x − ⃗x′
⃗x − ⃗x′
3 ′
′
3 ′
′
⃗
E(⃗x) =
d x ρ(⃗x )
=
d
x
ρ(⃗
x
)
4πϵ0
| ⃗x − ⃗x′ |
4πϵ0
| ⃗x − ⃗x′ |
R3
V
Ahora, utilizaremos la siguiente expansión en Taylor
!
"
⃗ f⃗(⃗x) + O(2)
f⃗(⃗x − ⃗x′ ) = f⃗(⃗x) − ⃗x′ · ∇

de forma que

!
" ⃗x
⃗x − ⃗x′
⃗x
′ ⃗
=
−
⃗
x
·
∇
+ O(2)
| ⃗x − ⃗x′ |
| ⃗x |3
| ⃗x |3

---

### Página 120

Así
⃗ x) =
E(⃗

⃗ x) ≈ 1
E(⃗
4πϵ0

4πϵ0

˚

⃗x − ⃗x′
d x ρ(⃗x )
| ⃗x − ⃗x′ |3
V

˚

3 ′

+

′

!
" ⃗x
⃗x
′ ⃗
− ⃗x · ∇
| ⃗x |3
| ⃗x |3

3 ′

′

q(V ) =

˚

d3 x′ ρ(⃗x′ )

˚

d3 x′ ρ(⃗x′ )⃗x′

d x ρ(⃗x )

V

definiendo

V

p⃗(V ) =

V

queda
⃗ x) ≈
E(⃗

" ⃗x
⃗x
1 !
⃗
p
⃗
(V
)
·
∇
q(V )
−
4πϵ0
| ⃗x |3 4πϵ0
| ⃗x |3

Notar que el primer término corresponde al campo creado por una carga puntual q(V ) en
el origen. Por supuesto ésta sería la aproximación a cero orden del campo, en donde esperamos
obtener la ley de Coulomb. El segundo término de esta expansión, equivale al campo eléctrico
generado por un dipolo puntual p⃗(V ) en el origen.
Esta expansión del campo se conoce como Expansión Multipolar, y se verá con más detalle
un poco más adelante (de hecho, en la próxima página).

---

### Página 121

5.7.

Expansión Multipolar

Consideraremos una fuente localizada caracterizada por la siguiente densidad de carga
+
ρ(⃗x) si ⃗x ∈ V
ρ=
0 si ⃗x ∈
/V
El potencial está dado por
φ(⃗x) =
4πϵ0

˚

d3 x′

V

donde

ρ(⃗x′ )
| ⃗x − ⃗x′ |

71/2
| ⃗x − ⃗x′ |= ⃗x2 + ⃗x′2 − 2⃗x · ⃗x′

entonces

=
′
| ⃗x − ⃗x |
| ⃗x |

5−1/2
+
⃗x · ⃗x′
⃗x′2
1+ 2 −2 2
⃗x
⃗x

Recordando la expansión en taylor

13 2
(1 + z)−1/2 = 1 − z +
z + O(3)
y la expansión hasta segundo orden es
#
$
#
$2 8
⃗x · ⃗x′
⃗x · ⃗x′
1 ⃗x′2
3 ⃗x′2
−2 2
−2 2
≈
{1 −
+
| ⃗x − ⃗x′ |
| ⃗x |
2 ⃗x2
⃗x
8 ⃗x2
⃗x
:8
9# $
#
$2
⃗x · ⃗x′
(⃗x · ⃗x′ )⃗x′2
⃗x · ⃗x′ 1 ⃗x′2 3
⃗x′2
+
+4
−4
1+ 2 −
⃗x
2 ⃗x2
⃗x2
⃗x2
⃗x4
9#
#
$2
$3 :8
⃗x · ⃗x′ 1 ⃗x′2 3 ⃗x · ⃗x′
| ⃗x′ |
1+ 2 −
=
+
+O
| ⃗x |
⃗x
2 ⃗x2
⃗x2
| ⃗x |

=
| ⃗x |

Con esto, la expansión del potencial electrostático a segundo orden es
˚
˚
⃗x
1 1
3 ′
′
φ(⃗x) =
d x ρ(⃗x ) +
·
d3 x′ ρ(⃗x′ )⃗x′
4πϵ0 | ⃗x |
4πϵ0 | ⃗x |
V
V
˚
6 ′ ′
1 1 xi xj
3 ′
′ 2
3x
ρ(⃗x′ ) + ...
+
d
x
x
−
δ
|
⃗
x
|
ij
i
j
4πϵ0 2 | ⃗x |
V
Se define el momento monopolar (escalar)
˚
d3 x′ ρ(⃗x′ )
q=
V

que es la carga total de la distribución. Además
˚
p⃗ =
d3 x′ ρ(⃗x′ )⃗x′
V

es el momento dipolar (vector) de la distribución.

---

### Página 122

⃗ =
Q

˚

V

;
'<
&
d3 x′ ρ(⃗x′ ) 3⃗x′ · ⃗x′T − I⃗ ⃗x′T · ⃗x′

es el momento cuadripolar (tensor)
˚
d3 x′ ρ(⃗x′ ) 3x′i x′j − δij | ⃗x′ |2
Qij =
V

la expansión queda

φ(⃗x) =
4πϵ0

⃗ · ⃗x
p⃗ · ⃗x
1 ⃗xT · Q
q
+
+
+ ...
| ⃗x | | ⃗x |3 2 | ⃗x |5

Expandir el potencial de una distribución en términos de sus momentos (monopolar, dipolar,
cuadripolar, etc) es muy útil en el estudio de radiación

---

### Página 123

#### Capítulo 6
Las dos leyes fundamentales de la
Electrostática
Hasta ahora se han establecido los principios fundamentales en el estudio de la electrostática.
Éstos son la ley de Coulomb (que proviene de un estudio empírico de las fuerzas entre cargas),
y el principio de superposición. Hemos visto que éstos principios tienen como consecuencia un
par de leyes que ha simpificado mucho el estudio de los campos para ciertos casos particulares.
Éstas son la ley de Gauss
ˆˆ
˚
✞☎ ⃗
⃗
x) · E(⃗x) =
d3 xρ(⃗x)
✝ ✆dS(⃗
ϵ
S
V
y la ley de circulación del campo eléctrico
˛
⃗ x) = 0
d⃗x · E(⃗
Γ

Éstas dos ecuaciones integrales entregan información global acerca del campo. Sin embargo,
es posible llevarlas a su forma más simple en un par de ecuaciones diferenciales para el campo
electrostático.
A partir de la ley de Gauss, y utilizando el teorema de la divergencia, se obtiene
ˆˆ
˚
˚
✞☎ ⃗ ⃗
3 ⃗
⃗
x) =
d x∇ · E(⃗x) =
d3 xρ(⃗x)
✝ ✆dS · E(⃗
ϵ
S
V
V
#

⃗ · E(⃗
⃗ x) − ρ(⃗x)
dx ∇
ϵ0
V

˚

$

=0

esto es independiente del volumen V de integración. Consecuencia de esto es que
⃗ · E(⃗
⃗ x) = ρ(⃗x)
∇
ϵ0
Del mismo modo, a partir de la ley de circulación y utilizando el teorema de Stokes
¨
˛
"
!
⃗ × E(⃗
⃗ x) = 0
⃗
⃗ x) · ∇
d⃗x · E(⃗x) =
dS(⃗
Γ

S(Γ)

para cualquier superficie cuyo contorno sea Γ. De aquí se desprende que
⃗ × E(⃗
⃗ x) = 0
∇

---

### Página 124

En resumen, las dos leyes integrales fundamentales del campo electrostático tienen una
formulación equivalente en dos ecuaciones diferenciales para el campo
⃗ · E(⃗
⃗ x) = ρ(⃗x)
∇
ϵ0
⃗ × E(⃗
⃗ x) = 0
∇
La primera de ellas relaciona la divergencia del campo electrostático en cada punto con la
densidad de carga. La segunda establece que el campo eléctrico es conservativo o irrotacional.
Éstas ecuaciones son las dos primeras Ecuaciones de Maxwell en el vacío y para campos
estáticos. Veremos que éstas contienen absolutamente toda la teoría de la electrostática, es decir,
basta con ellas para determinar completamente el campo eléctrico. Lo que hemos hecho aquí es
encontrar expresiones matemáticas simples que resumen absolutamente todo el conocimiento
empírico sobre la teoría del campo eléctrico estático.

---

### Página 125

Problema
Demuestre el siguiente teorema
⃗2
∇

= −4πδ(⃗x − ⃗x′ )
′
| ⃗x − ⃗x |

#### Solución
Sea V (S) un volumen en R3 y S = δV su contorno. Sea además una carga puntual q en el
punto ⃗x′ , es sabido que el campo electrostático creado por esta carga es
⃗ x) =
E(⃗

q
⃗x − ⃗x′
4πϵ0 | ⃗x − ⃗x′ |3

La ley de Gauss establece
ˆˆ
˚
q ✞☎ ⃗
⃗x − ⃗x′
x) ·
=
d3 xqδ(⃗x − ⃗x′ )
✝ ✆dS(⃗
4πϵ0 S
| ⃗x − ⃗x′ |3
ϵ0
V
o equivalentemente

⃗x − ⃗x′
= 4π
| ⃗x − ⃗x′ |3

ˆˆ

✞☎ ⃗
x) ·
✝ ✆dS(⃗
S

˚

V

d3 xδ(⃗x − ⃗x′ )

Utilizando el teorema de la divergencia
˚
ˆˆ
⃗x − ⃗x′
⃗x − ⃗x′
✞☎ ⃗
3 ⃗
d
S(⃗
x
)
·
=
d
x
∇
·
✝✆
| ⃗x − ⃗x′ |3
| ⃗x − ⃗x′ |3
S
V
y recordando que

⃗x − ⃗x′
=−
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |3
ˆˆ
˚
⃗x − ⃗x′
✞☎ ⃗
⃗ ·∇
⃗
x) ·
=−
d3 x∇
✝ ✆dS(⃗
′
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |
S
V
ˆˆ
˚
˚
⃗x − ⃗x′
✞☎ ⃗
3 ⃗2
x) ·
=−
d x∇
d3 xδ(⃗x − ⃗x′ )
= 4π
✝ ✆dS(⃗
′ |3
′ |
|
⃗
x
−
⃗
x
|
⃗
x
−
⃗
x
S
V
V
⃗
∇

luego

˚

V

#

⃗2
dx ∇

Finalmente
⃗2
∇

$
′
+ 4πδ(⃗x − ⃗x )
| ⃗x − ⃗x′ |

= −4πδ(⃗x − ⃗x′ )
| ⃗x − ⃗x′ |

---

### Página 126

6.1.

Completitud de la teoría Electrostática

6.1.1.

Descomposición de Helmhotz

⃗ x) un campo vectorial tal que
Sea A(⃗
ˆˆ

✞☎
✝✆

S(∞)

⃗ x′ ) ·
dS(⃗

⃗ x′ )
A(⃗
=0
| ⃗x′ − ⃗x |

definamos los campos
⃗ L (⃗x) = − 1 ∇
⃗
A
4π

˚

d3 x′

R3

⃗ T (⃗x) = 1 ∇
⃗ ×∇
⃗ ×
A
4π

˚

⃗ ′ · A(⃗
⃗ x′ )
∇
| ⃗x − ⃗x′ |

d3 x′

R3

entonces se cumple

⃗ x′ )
A(⃗
| ⃗x − ⃗x′ |

⃗ T (⃗x)
⃗ x) = A
⃗ L (⃗x) + A
1)A(⃗
⃗ ×A
⃗ L (⃗x) = 0
2)∇
⃗ ·A
⃗ T (⃗x) = 0
3)∇

⃗
⃗ L (⃗x) se llama parte longitudinal (irrotacional) de A
A
⃗ T (⃗x) se lama parte transversal (solenoidal) de A
⃗
A
Demostración del teorema de Helmhotz
1) Utilizando la identidad
⃗ · (f⃗g) = g ∇
⃗ · f⃗ + f⃗ · ∇g
⃗
∇
se tiene
⃗′·
∇
de forma que

⃗ x′ )
⃗ ′ · A(⃗
⃗ x′ )
A(⃗
∇
⃗′
⃗ x′ ) · ∇
=
+ A(⃗
′
′
| ⃗x − ⃗x |
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |

˚
⃗ ′ ⃗ x′ ) ˚
⃗ x′ )
A(⃗
3 ′ ∇ · A(⃗
3 ′⃗ ′
⃗ x′ ) · ∇
⃗′
dx
d x∇ ·
d3 x′ A(⃗
=
−
′
′
| ⃗x − ⃗x |
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |
R3
R3
R3

˚

˚
⃗ ′ ⃗ x′ ) ˆ✞ˆ ☎
⃗ x′ )
A(⃗
3 ′ ∇ · A(⃗
′
⃗
⃗ x′ ) · ∇
⃗
= ✝ ✆ dS(⃗x ) ·
+
dx
d3 x′ A(⃗
′
′
| ⃗x − ⃗x |
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |
R3
S(∞)
R3

˚

en este último paso hemos utilizado el teorema de la divergencia y el hecho que
⃗′
∇

⃗
= −∇
′
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |

utilizando la hipótesis del teorema
˚
⃗ ′ ⃗ x′ ) ˚
⃗ x′ )
3 ′ ∇ · A(⃗
3 ′⃗ ′
3 ′ A(⃗
⃗
⃗
dx
d x A(⃗x ) · ∇
dx
=
=∇·
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
R3
R3

˚

---

### Página 127

por lo tanto
⃗ x′ )
A(⃗
| ⃗x − ⃗x′ |
R3
Ahora ocupamos la siguiente identidad (muy utilizada en teoría electromagnética)
⃗ L (⃗x) = −∇
⃗∇
⃗ ·
4π A

˚

d3 x′

⃗ ×∇
⃗ × f⃗ = ∇
⃗∇
⃗ · f⃗ − ∇
⃗ 2 f⃗
∇
˚
⃗ x′ )
⃗ x′ )
A(⃗
3 ′ A(⃗
⃗
x
−
∇
dx
d
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
R3
˚
⃗
⃗
⃗ x′ )∇
⃗2
4π AL (⃗x) = −4π AT (⃗x) −
d3 x′ A(⃗
| ⃗x − ⃗x′ |
R3
por último, utilizando el teorema
⃗ ×∇
⃗ ×
⃗ L (⃗x) = −∇
4π A

˚

3 ′

= −4πδ(⃗x − ⃗x′ )
| ⃗x − ⃗x′ |
˚
!
"
⃗ x′ )δ(⃗x − ⃗x′ )
⃗
⃗
d3 x′ A(⃗
4π AL (⃗x) + AT (⃗x) = 4π
⃗2
∇

R3

y se demuestra que

⃗ x) = A
⃗ L (⃗x) + A
⃗ T (⃗x)
A(⃗

⃗ ×∇
⃗
⃗ ×A
⃗ L (⃗x) = ∇
b) − 4π ∇

˚

R

⃗ ′ ⃗ x′ )
3 ′ ∇ · A(⃗
= ⃗0
dx
| ⃗x − ⃗x′ |

⃗ ×A
⃗ L (⃗x) = 0
∇

⃗ ·A
⃗ T (⃗x) = ∇
⃗ ·∇
⃗ ×∇
⃗ ×
c)4π ∇

˚

R3

d3 x′

⃗ x′ )
A(⃗
=0
| ⃗x − ⃗x′ |

⃗ ·A
⃗ T (⃗x) = 0
∇
Observación
La validez del teorema de Helmhotz es
ˆˆ
✞☎
✝✆

S(∞)

⃗ x′ ) ·
dS(⃗

⃗ x′ )
A(⃗
=0
| ⃗x − ⃗x′ |

Podemos escoger esta superficie como una esfera centrada en ⃗x y de radio a, con a → ∞
ˆˆ
ˆˆ
⃗ x′ )
⃗ x′ )
A(⃗
x′ ) · A(⃗
✞☎
✞☎
′
′ n̂(⃗
⃗
x)·
dS(⃗
x
)
=
lím
✝
✆
✝ ✆ dS(⃗
| ⃗x − ⃗x′ | a→∞ S(⃗x,a)
| ⃗x − ⃗x′ |
S(∞)
sobre la superficie

---

### Página 128

⃗x′ − ⃗x = an̂(⃗x′ )
| ⃗x − ⃗x′ |= a

dS(⃗x′ ) = a2 dΩ(⃗x)
donde dΩ(⃗x) = sin2 ϑdϑdφ es el elemento de ángulo sólido con vértice en ⃗x
= ˆ
=ˆˆ
=
4π
′
⃗
⃗ x′ ) |
A(⃗x ) =
x′ ) · A(⃗
=
= ✞☎
′
2 | n̂(⃗
⃗
dΩ(⃗x) lím a
=≤
= ✝ ✆ dS(⃗x ) ·
a→∞
= S(∞)
| ⃗x − ⃗x′ | =
a

= ˆ
=ˆˆ
ˆ 4π
=
4π
⃗ x′ ) =
A(⃗
=
= ✞☎
′
′
′
⃗
⃗
⃗ x′ ) |
dΩ(⃗x) lím a | n̂(⃗x ) · A(⃗x ) |=
dΩ lím
| ⃗x − ⃗x′ || A(⃗
=≤
= ✝ ✆ dS(⃗x ) ·
′ |→∞
a→∞
= S(∞)
|⃗
x
| ⃗x − ⃗x′ | =
=

ˆ 4π

⃗ x′ ) |
dΩ lím | ⃗x′ || A(⃗
|⃗
x|→∞

por lo tanto
ˆˆ
✞☎
⃗
lím | ⃗x || A(⃗x) |= 0 → ✝ ✆

|⃗
x|→∞

S(∞)

⃗ x′ ) ·
dS(⃗

⃗ x′ )
A(⃗
=0
| ⃗x − ⃗x′ |

A continuación, demostraremos dos teoremas que nos permitirán escribir el teorema de
Helmhotz de una forma más conveniente
Teorema 1
˚
ˆˆ
✞☎
3 ⃗
⃗ x)ψ(⃗x)
d x∇ψ(⃗x) = ✝ ✆ dS(⃗
V

S(V )

Demostración
Ustamos el teorema de la divergencia
ˆˆ
˚
☎
3 ⃗
⃗ x) = ✞
d x∇ · A(⃗
✝✆
V

S(V )

⃗ x) · A(⃗
⃗ x)
dS(⃗

⃗ x) = Bψ(⃗
⃗ x), con B
⃗ un vector constante arbitrario
con A(⃗
˚
˚
˚
3 ⃗
3 ⃗ ⃗
⃗
⃗
⃗ x)
d x∇ · Bψ(⃗x) =
d xB · ∇ψ(⃗x) = B ·
d3 x∇ψ(⃗
V

˚

V

V

ˆˆ

☎
⃗ · Bψ(⃗
⃗ x) = ✞
d3 x∇
✝✆

S(V )

⃗·
B

+˚

V

V

ˆˆ

☎
⃗ x) · Bψ(⃗
⃗ x) = B
⃗· ✞
dS(⃗
✝✆

⃗ x)ψ(⃗x)
dS(⃗

S(V )

ˆˆ
✞☎
⃗
d x∇ψ(⃗x) − ✝ ✆

S(V )

⃗
dS(⃗x)ψ(⃗x) = 0

---

### Página 129

⃗ fue escogido de forma arbitraria
como B
˚
ˆˆ
✞☎
3 ⃗
d x∇ψ(⃗x) = ✝ ✆
V

⃗ x)ψ(⃗x)
dS(⃗

S(V )

Teorema 2
˚

⃗ × A(⃗
⃗ x) = ✝ ✆
d x∇

V

Demostración
˚

✞☎
S(V )

⃗ x) × A(⃗
⃗ x)
dS(⃗

˚
˚
"
⃗
⃗
⃗
⃗ b Ac
d x ∇×A =
d xϵabc ∇b Ac = ϵabc
d3 x∇
!

V

ˆˆ

a

V

V

pero del teorema anterior

⃗ aψ = ✝ ✆
d x∇

˚

!

"

ˆˆ

⃗ ×A
⃗
dx ∇

V

✞☎

V

así

ˆˆ

˚

a

dSa ψ

S(V )

✞☎
= ϵabc ✝ ✆

=

S(V )

ˆˆ

✞☎
✝✆

S(V )

!

ˆˆ

✞☎

dSb Ac = ✝ ✆

ϵabc dSb Ac

S(V )

⃗ ×A
⃗
dS

"

a

⃗ x) como
Con este teorema, podemos escribir la parte transversal de A(⃗
⃗ ×
⃗ T (⃗x) = 1 ∇
A
4π

˚

d3 x′

R3

En efecto, consideremos
⃗ ×
∇
˚

R3

3 ′⃗

⃗ x′ )
⃗ ′ × A(⃗
∇
| ⃗x − ⃗x′ |

˚
⃗ x′ )
A(⃗
3 ′⃗ ′
⃗
x
A(⃗
x
)
×
∇
dx
=
−
d
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
R3

˚

⃗′
d x A(⃗x ) × ∇
′

3 ′

=
| ⃗x − ⃗x′ |

⃗ x′ )
⃗ ′ ⃗ x′ ) ˚
A(⃗
3 ′ ∇ × A(⃗
3 ′⃗ ′
x
∇
×
−
dx
d
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
R3

˚

⃗ ′ ⃗ x′ ) ˆ✞ˆ ☎
⃗ x′ )
A(⃗
3 ′ ∇ × A(⃗
′
⃗
dx
−
d
S(⃗
x
)
×
✝✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
S(∞)

˚

pero si se cumple la hipótesis del teorema de Helmhotz
ˆˆ

⃗ x) |= 0 → ✝ ✆
lím | ⃗x || A(⃗
✞☎

|⃗
x|→∞

luego
⃗ ×
∇

S(∞)

⃗ x′ ) ×
dS(⃗

⃗ x′ )
A(⃗
= ⃗0
| ⃗x − ⃗x′ |

˚
⃗ x′ )
⃗ ′ ⃗ x′ )
A(⃗
3 ′ ∇ × A(⃗
dx
dx
=
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
R3

˚

3 ′

---

### Página 130

y entonces

6.1.2.

˚
⃗ x′ )
1 ⃗
A(⃗
⃗
⃗
AT (⃗x) =
∇×∇×
d3 x′
4π
| ⃗x − ⃗x′ |
R3
˚
⃗ ′ × A(⃗
⃗ x′ )
1 ⃗
∇
⃗
∇×
d3 x′
AT (⃗x) =
4π
| ⃗x − ⃗x′ |
R3

Teorema de Helmhotz, segunda forma

⃗ es un campo vectorial tal que
Si A
⃗ x) |= 0
lím | ⃗x || A(⃗

|x|→∞

entonces

⃗ T (⃗x)
⃗ x) = A
⃗ L (⃗x) + A
A(⃗

con
⃗ L (⃗x) = − 1 ∇
⃗
A
4π

˚

d3 x′

⃗ ′ · A(⃗
⃗ x′ )
∇
| ⃗x − ⃗x′ |

⃗ T (⃗x) = 1 ∇
⃗ ×
A
4π

˚

d3 x′

⃗ ′ × A(⃗
⃗ x′ )
∇
| ⃗x − ⃗x′ |

donde

R3

R3

⃗ ×A
⃗ L (⃗x) = 0
∇
⃗ ·A
⃗ T (⃗x) = 0
∇

6.1.3.

Corolario del Teorema de Helmhotz

Dadas la divergencia

⃗ · A(⃗
⃗ x) = 4πD(⃗x)
∇

y el rotor

⃗ × A(⃗
⃗ x) = 4π R(⃗
⃗ x)
∇

⃗ x), sobre todo el espacio, entonces ese campo vectorial está comde un campo vectorial A(⃗
pletamente determinado en todos los puntos del espacio mediante la siguiente representación
integral- diferencial
⃗ x) = −∇
⃗
A(⃗

D(⃗x′ )
⃗ ×
dx
+∇
′ |
|
⃗
x
−
⃗
x
R

˚

3 ′

˚

R3

d3 x′

⃗ x)
R(⃗
| ⃗x − ⃗x′ |

⃗ x) y R(⃗
⃗ x) nos son dadas, son las fuentes del campo A(⃗
⃗ x).
Observación: las funciones D(⃗
Pero
;
<
⃗ = {D, Rx , Ry , Rz }
D, R
son 4 funciones, mientras que

; <
⃗ = {Ax , Ay , Az }
A

---

### Página 131

son 3 funciones. Sin embargo, no hay sobredeterminación pues
!
"
⃗ ×A
⃗ = 4π ∇
⃗ ·R
⃗ =0
⃗ · ∇
∇
⃗ debe ser solenoidal
luego R

⃗ · R(⃗
⃗ x) = 0
∇

esto agrega 1 condición. Con esto, la construcción de Helmhotz define un problema bien
determinado

6.2.

Completitud de la Electrostática

Hemos encontrado que
⃗ · E(⃗
⃗ x) = ρ(⃗x)
∇
ϵ0
⃗ × E(⃗
⃗ x) = ⃗0
∇
El teorema de Helmhotz nos dice que , dadas la divergencia y el rotor del campo eléctrico,
este esta absolutamente determinado por la forma integral
˚
1 ⃗
ρ(⃗x′ )
⃗
E(⃗x) = −
d3 x′
∇
4πϵ0
| ⃗x − ⃗x′ |
R3
y la electrostática es una teoría completa: el conjunto de ecuaciones diferenciales que representan las leyes fundamentales de la teoría es suficiente para determinar completamente el
campo electrostático

---

### Página 132

Problema
La descomposición de Helmholtz requiere que
⃗ x) |= 0
lím | ⃗x || A(⃗

|⃗
x|→∞

demuestre que
˚

R3

;
<
⃗ x) | < ∞
d3 x | D(⃗x) | + | R(⃗

es condición suficiente para la validez de la representación integro-diferencial de Helmholtz
#### Solución
⃗ x) = −∇
⃗
A(⃗

D(⃗x′ )
⃗ ×
dx
+∇
′ |
|
⃗
x
−
⃗
x
R

˚

Entonces

3 ′

˚

R3

d3 x′

⃗ x′ )
R(⃗
| ⃗x − ⃗x′ |

=
=
˚
˚
=
=
′
′
⃗
D(⃗
x
)
R(⃗
x
)
=
3 ′
⃗ ×
⃗
⃗ x) |=| ⃗x | =
x
+
∇
| ⃗x || A(⃗
d3 x′
d
=
=−∇
′ |
′ |=
=
|
⃗
x
−
⃗
x
|
⃗
x
−
⃗
x
R
R

=
=
=
˚
=
=
=
′
′
⃗
⃗ x)×∇
= + | ⃗x |
=
=R(⃗
d
≤| ⃗x |
x
=
| ⃗x − ⃗x′ | =
| ⃗x − ⃗x′ | =
R3
R3
˚
˚
′
⃗x − ⃗x′
3 ′
′
3 ′
⃗ x′ ) || ⃗x − ⃗x |
|
+
|
⃗
x
|
x
|
R(⃗
≤| ⃗x |
d x | D(⃗x ) ||
d
| ⃗x − ⃗x′ |3
| ⃗x − ⃗x′ |3
R3
R3
˚
<
| ⃗x | ;
′
⃗ x′ ) |
d3 x′
|
D(⃗
x
=
)
|
+
|
R(⃗
| ⃗x − ⃗x′ |2
R3
˚

=
=
⃗
d x =D(⃗x′ )∇
3 ′=

Luego

˚

⃗ x) |≤ lím
lím | ⃗x || A(⃗

|⃗
x|→∞

|⃗
x|→∞

=

˚

R3

si

<
| ⃗x | ;
′
⃗ x′ ) |
|
D(⃗
x
)
|
+
|
R(⃗
| ⃗x − ⃗x′ |2

| ⃗x |
|⃗
x|→∞ | ⃗
x − ⃗x′ |2
;
<
3 ′
′
′
⃗
d x | D(⃗x ) | + | R(⃗x ) | = 0

;
<
⃗ x′ ) | lím
d3 x′ | D(⃗x′ ) | + | R(⃗

= lím
|⃗
x|→∞ | ⃗
x|
0<

R3

d3 x′

˚

˚

R3

R3

<
;
′
′
⃗
d x | D(⃗x ) | + | R(⃗x ) | < ∞
3 ′

---

### Página 133

Problema
Demuestre que si
lím | ⃗x || D(⃗x) |= 0

|⃗
x|→∞

y

⃗ x) |= 0
lím | ⃗x || R(⃗

|⃗
x|→∞

entonces la representación de Helmholtz puede escribirse
⃗ x) = −
A(⃗

˚

d3 x′

R3

⃗ ′ D(⃗x′ ) − ∇
⃗ ′ × R(⃗
⃗ x′ )
∇
| ⃗x − ⃗x′ |

#### Solución
De la representación de Helmholtz
⃗ x) = −∇
⃗
A(⃗
⃗ x) =
A(⃗

˚

3 ′

+
| ⃗x − ⃗x′ |

⃗′
d x D(⃗x )∇
3 ′

R3

D(⃗x′ )
⃗
+∇
dx
′ |
|
⃗
x
−
⃗
x
R

˚

′

˚

˚

R3

d3 x′

R3

⃗ x′ )
R(⃗
| ⃗x − ⃗x′ |

⃗ x′ ) × ∇
⃗′
d3 x′ R(⃗

| ⃗x − ⃗x′ |

˚
⃗ ′ x′ ) ˚
⃗ ′ ⃗ x′ ) ˚
⃗ x′ )
x′ )
R(⃗
3 ′ ∇ D(⃗
3 ′ ⃗ ′ D(⃗
3 ′ ∇ × R(⃗
3 ′⃗ ′
dx
+
d
+
d
−
d
x
∇
x
x
∇
×
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
R3
R3
R3

⃗ x) = −
A(⃗

˚

⃗ x) = −
A(⃗

˚

ˆˆ
˚
⃗ x′ )
⃗′
⃗ ′ ⃗ x′ ) ˆ✞ˆ ☎
D(⃗x′ )
R(⃗
x′ ) ✞ ☎
3 ′ ∇ · D(⃗
′
3 ′ ∇ × R(⃗
′
⃗
⃗
d
S(⃗
x
)
x
d
S(⃗
x
)×
+
+
−
dx
d
✝✆
✝✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
S(∞)
R3
S(∞)
⃗ x) = −
A(⃗

En efecto

˚

R3

d3 x′

⃗ ′ D(⃗x′ ) − ∇
⃗ ′ × R(⃗
⃗ x′ )
∇
| ⃗x − ⃗x′ |
D(⃗x′ )
=0
| ⃗x − ⃗x′ |

ˆˆ

lím | ⃗x || D(⃗x) |= 0 → ✝ ✆

⃗ x′ )
dS(⃗

ˆˆ
✞☎
⃗
lím | ⃗x || R(⃗x) |= 0 → ✝ ✆

⃗ x′ ) ×
dS(⃗

✞☎

|⃗
x|→∞

|⃗
x|→∞

S(∞)

S(∞)

⃗ x′ )
R(⃗
=0
| ⃗x − ⃗x′ |

---

### Página 134

6.3.

Apendice: Descomposición de Helmholtz en un volumen finito

⃗ x) satisface idénticamente la siguiente relación
Se demuestra que cualquier campo vectorial A(⃗
⃗ x) = − 1 ∇
⃗
A(⃗
4π

˚
⃗ ′ ⃗ x′ )
⃗ ′ ⃗ x′ )
1 ⃗
3 ′ ∇ · A(⃗
3 ′ ∇ × A(⃗
dx
d
x
∇
×
+
| ⃗x − ⃗x′ |
4π
| ⃗x − ⃗x′ |
V
V

˚

#
$
#
$
ˆˆ
ˆˆ
⃗x′ − ⃗x
1 ✞☎
⃗x′ − ⃗x
1 ✞☎
′
′
′
⃗
⃗
⃗
⃗ x′ )
+
dS(⃗x ) · ′
A(⃗x ) +
dS(⃗x ) × ′
× A(⃗
✝✆
✝✆
4π S(V )
| ⃗x − ⃗x |3
4π S(V )
| ⃗x − ⃗x |3
donde V es cualquier región cerrada, δV = S(V ) es su frontera, y ⃗x ∈ V
Demostración
Tenemos
˚
˚
˚
⃗ ′ ⃗ x′ )
⃗ x′ )
A(⃗
3 ′ ∇ · A(⃗
3 ′⃗ ′
′
3 ′⃗ ′
⃗
=
−
+
dx
d
x
A(⃗
x
)
·
∇
d
x
∇
·
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V
V
V
ˆˆ
⃗ ′ ⃗ x′ ) ˚
⃗ ′
✞☎
3 ′ ∇ · A(⃗
3 ′⃗ ′
⃗
⃗ x′ ) · A(⃗x )
=
+
dx
d
x
A(⃗
x
)
·
∇
d
S(⃗
✝
✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V
V
S(V )

˚

˚
ˆˆ
⃗ x′ )
⃗ ′ ⃗ x′ )
⃗ ′
✞☎
3 ′ ∇ · A(⃗
3 ′ A(⃗
⃗
⃗ x′ ) · A(⃗x )
=
∇
·
+
dx
d
x
d
S(⃗
✝
✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V
V
S(V )

˚
con esto
⃗
∇

˚
ˆˆ
⃗ ′ ⃗ x′ )
⃗ x′ )
⃗ ′
✞☎
3 ′ ∇ · A(⃗
3 ′ A(⃗
⃗
⃗
⃗
⃗ x′ ) · A(⃗x )
=
∇
∇
·
+
∇
dx
d
x
d
S(⃗
✝
✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V
V
S(V )

˚

y utilizando la identidad

!
"
⃗ ∇
⃗ ·A
⃗ =∇
⃗ ×∇
⃗ ×A
⃗+∇
⃗ 2A
⃗
∇
⃗
∇

˚
˚
ˆˆ
⃗ x′ )
⃗ x′ )
⃗ ′ ⃗ x′ )
A(⃗
A(⃗
✞☎
3 ′ ∇ · A(⃗
′
′
⃗ x′ )·A(⃗
⃗ x′ )∇
⃗ ∇×
⃗
⃗
dx
dx
dx
= ∇×
+∇
+ ✝ ✆ dS(⃗
′
′
′
| ⃗x − ⃗x |
| ⃗x − ⃗x |
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |
V
V
V
S(V )

˚

˚
ˆˆ
′
⃗ x′ )
A(⃗
✞☎
3 ′⃗ ′ ⃗2
⃗ x′ ) · A(⃗
⃗ x′ ) ⃗x − ⃗x
dx
d
x
A(⃗
x
)
∇
d
S(⃗
+
−
✝
✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |3
V
V
S(V )

⃗ ×∇
⃗ ×
=∇

˚

⃗ ×∇
⃗ ×
=∇

˚

3 ′

˚
ˆˆ
′
′
⃗ x′ )
A(⃗
✞☎
3 ′⃗ ′
′
⃗ x′ ) · A(⃗
⃗ x′ ) ⃗x − ⃗x
−
4π
dx
d
x
)δ(⃗
x
−
⃗
x
)
+
d
S(⃗
A(⃗
x
✝
✆
| ⃗x − ⃗x′ |
| ⃗x′ − ⃗x |3
V
V
S(V )
3 ′

Luego si ⃗x ∈ V
⃗
⃗ x) = − 1 ∇
A(⃗
4π

ˆˆ
˚
′
⃗ ′ ⃗ x′ ) 1
⃗ x′ )
1 ✞☎
3 ′ ∇ · A(⃗
3 ′ A(⃗
⃗ x′ )·A(⃗
⃗ x′ ) ⃗x − ⃗x
⃗
⃗
dx
d
x
d
S(⃗
∇×
∇×
+
+
✝
✆
| ⃗x − ⃗x′ | 4π
| ⃗x − ⃗x′ | 4π S(V )
| ⃗x − ⃗x′ |3
V
V

˚

---

### Página 135

Ahora bien

⃗ ×
∇

˚
˚
⃗ x′ )
A(⃗
3 ′⃗ ′
⃗
⃗ x′ ) × ∇
⃗′
dx
d x A(⃗x ) × ∇
d3 x′ A(⃗
=−
=
′
′
| ⃗x − ⃗x |
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |
V
V
V

˚

3 ′

˚
⃗ x′ )
⃗ ′ ⃗ x′ ) ˚
⃗ x′ )
A(⃗
A(⃗
3 ′ ∇ × A(⃗
3 ′⃗ ′
=
−
dx
d
x
d
x
×
∇
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V
V
V
˚
˚
⃗ x′ )
⃗ ′ ⃗ x′ ) ˆ✞ˆ ☎
⃗ ′
3 ′ A(⃗
3 ′ ∇ × A(⃗
⃗
⃗ x′ ) × A(⃗x )
∇×
=
−
dx
d
x
d
S(⃗
✝
✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V
V
S(V )
˚

⃗ ×
∇

3 ′

Luego
˚
ˆˆ
⃗ x′ )
⃗ ′ ⃗ x′ )
⃗ ′
A(⃗
✞☎
3 ′ ∇ × A(⃗
⃗
⃗
⃗ x′ ) × A(⃗x )
=
∇
×
−
∇
×
dx
d
x
d
S(⃗
✝
✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V
V
S(V )

˚

⃗ ×∇
⃗ ×
∇

⃗ ×∇
⃗×
∇

˚
"
⃗ x′ )
⃗ ′ ⃗ x′ ) ˆ✞ˆ ☎ !
A(⃗
3 ′ ∇ × A(⃗
′
′
⃗
⃗
⃗
⃗
= ∇×
+ ✝✆
dS(⃗x ) × A(⃗x ) × ∇
dx
dx
′
′
| ⃗x − ⃗x |
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |
V
V
S(V )

˚

⃗ ×∇
⃗ ×
∇

3 ′

3 ′

˚
"
⃗ x′ )
⃗ ′ ⃗ x′ ) ˆ✞ˆ ☎ !
A(⃗
⃗x′ − ⃗x
3 ′ ∇ × A(⃗
′
′
⃗
⃗
⃗
d
S(⃗
x
dx
d
x
)
×
A(⃗
x
)
×
=
∇
×
+
✝
✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V
V
S(V )

˚

3 ′

Así
⃗
⃗ x) = − 1 ∇
A(⃗
4π

˚
⃗ ′ ⃗ x′ )
⃗ ′ ⃗ x′ )
1 ⃗
3 ′ ∇ · A(⃗
3 ′ ∇ × A(⃗
dx
d
x
∇
×
+
| ⃗x − ⃗x′ |
4π
| ⃗x − ⃗x′ |
V
V

˚

ˆˆ
ˆˆ
"
′
1 ✞ ☎ ! ⃗ ′ ⃗ ′ " ⃗x − ⃗x′
1 ✞☎ ! ⃗ ′
⃗ x′ ) × ⃗x − ⃗x
+
dS(⃗x ) · A(⃗x )
d
S(⃗
x
+
)
×
A(⃗
✝✆
✝
✆
4π S(V )
| ⃗x − ⃗x′ |3 4π S(V )
| ⃗x′ − ⃗x |3
Por otra parte
!

luego

"
!
"
!
"
!
"
⃗·B
⃗ C
⃗+ A
⃗×B
⃗ ×C
⃗ = A
⃗·B
⃗ C
⃗ −C
⃗× A
⃗×B
⃗
A

!

"
!
"
!
"
!
"
!
"
⃗·B
⃗ C
⃗+ A
⃗×B
⃗ ×C
⃗ = A
⃗·B
⃗ C
⃗− C
⃗ ·B
⃗ A
⃗+ C
⃗ ·A
⃗ B
⃗
A

!

"
!
"
!
"
!
"
!
"
⃗·B
⃗ C
⃗+ A
⃗×B
⃗ ×C
⃗ = B
⃗ ·A
⃗ C
⃗− B
⃗ ·C
⃗ A
⃗+ C
⃗ ·A
⃗ B
⃗
A
!

"
!
"
!
" !
"
⃗·B
⃗ C
⃗+ A
⃗×B
⃗ ×C
⃗ =B
⃗× C
⃗ ×A
⃗ + C
⃗ ·A
⃗ B
⃗
A

!

"
!
"
!
"
!
"
⃗·B
⃗ C
⃗+ A
⃗×B
⃗ ×C
⃗ = A
⃗×C
⃗ ×B
⃗+ A
⃗·C
⃗ B
⃗
A

---

### Página 136

Finalmente

!

"
!
"
!
"
!
"
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
A·B C + A×B ×C = A·C B+ A×C ×B

⃗
⃗ x) = − 1 ∇
A(⃗
4π

˚
⃗ ′ ⃗ x′ )
⃗ ′ ⃗ x′ )
1 ⃗
3 ′ ∇ · A(⃗
3 ′ ∇ × A(⃗
+
∇
×
dx
d
x
| ⃗x − ⃗x′ |
4π
| ⃗x − ⃗x′ |
V
V

˚

#
$
#
$
ˆˆ
ˆˆ
1 ✞☎
⃗x′ − ⃗x
1 ✞☎
⃗x′ − ⃗x
′
′
′
⃗
⃗
⃗ x′ )
⃗
dS(⃗x ) · ′
dS(⃗x ) × ′
× A(⃗
A(⃗x ) +
+
✝✆
✝✆
4π S(V )
| ⃗x − ⃗x |3
4π S(V )
| ⃗x − ⃗x |3
⃗ x) está determinado por
Vemos que A(⃗
⃗ · A(⃗
⃗ x) = 4πD(⃗x)
∇

⃗ × A(⃗
⃗ x) = 4π R(⃗
⃗ x)
∇
para ⃗x ∈ V
⃗ x) = A
⃗ H (⃗x)
A(⃗
para ⃗x ∈ S(V )

---

### Página 137

Parte II
Conductores, Ecuaciones de Poisson y
Laplace

---

### Página 138

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 139

#### Capítulo 7
Conductores
Hasta aquí hemos terminado con los problemas donde la distribución de carga es conocida
desde el comienzo. (Integrales de Coulomb). Hasta ahora han sido problemas sin mayores complicaciones que calcular correctamente las integrales. Ahora atacaremos otro tipo de problemas,
la determinación de los campos cerca de conductores.
La materia se puede clasificar gruesamente en conductores y aislantes ( o dieléctricos). Un
material dieléctrico posee electrones fuertemente ligados a los átomos, de manera que ante la
presencia de un campo eléctrico las partículas cargadas pueden cambiar sus posiciones ligeramente, pero se mantienen ligadas a sus moléculas. Por otro lado, un material conductor (como
un metal) es aquél que en su interior posee un gran número de electrones libres, y éstos se
pueden mover libremente en el conductor, responden a campos eléctricos casi infinitesimales y
continúan su movimiento mientras experimentan un campo. Esta corriente de electrones debe
estar constantemente provista de fuentes externas de energía, o sino el movimiento de los electrones se detendrá cuando cancelen el efecto de la fuente que produce el campo original (se
alcanza un equilibrio estático).
Campo eléctrostático dentro de un conductor es nulo
En electrostática, no consideramos fuentes continuas de corriente, de manera que los electrones
se moverán hasta que se arreglen de forma que produzcan un campo eléctrico nulo en cualquier
parte dentro del conductor (esto suele pasar en una fracción de segundo). Si quedara algún
campo dentro del conductor, este campo movería más electrones, luego la única solución electrostática es que el campo es cero en cualquier punto interior del conductor.
La carga en un conductor se distribuye en su superficie
Consecuencia directa de la propiedad anterior es que la carga en un conductor debe distribuírse
en su superficie. De la ley de gauss, es evidente que si existiera una carga neta al interior del
conductor, el flujo eléctrico sobre la superficie de la figura sería distinto de cero, y por lo tanto,
existiría un campo eléctrico en su interior

---

### Página 140

ˆˆ

✞☎ ⃗ ′
⃗ x′ ) = 0 → qin = 0
x ) · E(⃗
✝ ✆dS(⃗
S

Notar que como el campo eléctrico es cero en el interior de un conductor, entonces
⃗ =0
−∇φ
Esto significa que al interior de un conductor el potencial es constante.
La dificultad que se presenta cuando hay condutores presentes es evidente. Suponga que estamos en la situación en que se carga un conductor con una carga Q. Ahora no estamos en
condiciones de saber exactamente dónde están las cargas, sólo sabemos que ellas se van a distribuír sobre toda la superficie. ¿Cómo podemos determinar la forma en que se distribuyen las
cargas? Veremos que ellas se deben distribuír de forma que que la superficie del conductor forme
una equipotencial. Si la superficie de un conductor no fuera equipotencial, entonces habría
un campo eléctrico distinto de cero en el interior del conductor, y las cargas en el conductor se
seguirán moviendo hasta que finalmente el campo en su interior se anula. (y se alcanze nuevamente un estado de equilibrio electrostático)
⃗ en la superficie de un conductor es cero
Componente tangencial de E
Considere la integral de línea sobre el camino cerrado de la figura
˛
⃗
d⃗x · E

Como el campo eléctrico es conservativo, la integral de línea sobre el camino cerrado abcda es
cero.
˛
⃗ = Et (∆l) − En (∆x′ ) + 0(∆l) + En (∆x) = 0
d⃗x · E
abcda

donde En y Et son las componentes normal y tangencial del campo eléctrico, respectivamente, y hemos escogido el segmento ab paralelo a Et en todos los puntos.
En el límite cuando ∆x′ → 0 y ∆x → 0, se tiene
Et ∆l = 0

---

### Página 141

Como ∆l es una longitud finita, se concluye que la componente tangencial del campo eléctrico sobre la superficie de un conductor es cero. Esto es algo sumamente importante, ya que consecuencia de ésto es que un conductor en equilibrio electrostático es una Superficie equipotencial. Mostrar esto ahora resulta evidente, considere 2 puntos A y B sobre la superficie de
un conductor, y calcule la diferencia de potencial entre estos dos puntos

φB − φA = −

ˆ B
A

⃗ x) = 0
d⃗x · E(⃗

⃗ sólo tiene componente normal a la curva . Luego, los puntos A y B se encuentran
ya que E
al mismo potencial
⃗ es normal a la superficie de un conductor
El campo E
Si la componente tangencial del campo fuera distinta de cero, las cargas entonces se moverían
hasta que ésta componente desaparezca. Luego, en un conductor en equilibrio, sólo sobrevive
la componente normal del campo eléctrico. Para obtener el campo eléctrico sobre la superficie
de un conductor, considere la superficie de Gauss de la figura

De la ley de Gauss obtenemos
✞☎ ⃗ ′
⃗ x′ ) = En A + 0A = σA
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

de aquí
En =

σ
ϵ0

Es decir, el campo eléctrico justo sobre la superficie de un conductor es normal a ella y su
magnitud está directamente relacionada con la densidad superficial de carga sobre el punto del
conductor. Éstas consecuencias son absolutamente generales. Notar que ésto nos permite determinar la densidad superficial de carga sobre un conductor, sin embargo, ! se requiere conocer
el campo eléctrico ! ¿Cómo podemos determinar el campo eléctrico sin conocer primeramente
la densidad de carga en el conductor?. Veremos más adelante que esto es posible al resolver la
ecuación diferencial que satisface el potencial electrostático
Como conclusión, el campo eléctrico cerca de un conductor tiene la forma de la figura

---

### Página 142

Como ejemplo, considere un campo uniforme en la dirección horizontal en una región del
espacio. Imaginemos que colocamos una esfera conductora en este campo uniforme. Cargas
sobre el conductor se moveran y distribuirán hasta alcanzar un equilibrio electrostático, es
decir, hasta que el campo en su interior se anule y la componente tangencial del campo sobre la
superficie también, de manera que toda las cargas se encuentren en equilibrio en su superficie.
La situación de equilibrio será tal cual muestra la figura

Es decir, el campo eléctrico se ve deformado cerca de la esfera conductora, de manera que
líneas de campo sean normales en su superficie. El potencial electrostático sobre la superficie
esférica es una constante. Otro ejemplo de líneas de campo y superficies equipotenciales se
aprecia en la siguiente figura, donde dos conductores se encuentran cercanos

Una aplicación interesante es que la energía potencial de un conductor es muy simple de
calcular. Esto se debe a que en un conductor toda la carga se concentra en la superficie, y que
sobre ella el potencial es constante. Luego , la energía potencial asociada a un conductor de
carga Q y potencial V está dada por

---

### Página 143

¨
¨
¨
′
′
′
U=
φ(⃗x )dq(⃗x ) = φ
dq(⃗x ) = φ
σ(⃗x′ )dS(⃗x′ ) = φQ
2 S
S
S
La energía potencial de un conductor con carga Q y a potencial φ está dada por
U = φQ

7.1.

Condensadores

Un condensador es un dispositivo capaz de acumular carga eléctrica. Éstos pueden variar
en tamaño y forma, pero su configuración básica consiste en 2 conductores cargados con cargas
iguales y opuestas. Los condensadores son de gran importancia en electrónica, y entre sus
aplicaciones más conocidas están el almacenamiento de energía eléctrica, amortiguamiento de
los cambios de voltaje cuando se conectan a resistencias, filtros de frecuencias, reguladores de
tensión y muchas más.

Cuando se encuentran descargados, la carga en ambos conductores es cero. Durante el proceso
de carga, una carga Q se mueve desde un conductor a otro, dándole a uno una carga neta +Q
y al otro carga neta −Q. Una diferencia de potencial entre ambos ∆V se crea, con el conductor
cargado positivamente a un potencial más alto que el conductor cargado negativamente. Notar
que aunque esté cargado o descargado, la carga total del condensador como un todo es cero.
El ejemplo más simple de un condensador consiste de 2 placas conductoras de área A, paralelas
entre sí, separadas a una distancia d

La carga Q almacenada en un condensador es linealmente proporcional a la diferencia de potencial entre los conductores |∆V |. Así
Q = C|∆V |
Donde C es una constante positiva llamada capacidad. Físicamente, es una medida de
la capacidad de almacenar carga eléctrica en sus conductores para una diferencia de potencial
dada ∆V . La unidad de capacidad es C/V (Coulomb/ Volt), también conocida como F (Farad).

---

### Página 144

El Farad es una unidad muy grande, condensadores típicos no poseen una capacidad superior
a 1 µ F.

7.2.

Ecuaciones de Poisson y Laplace

Dadas las ecuaciones fundamentales de la electrostática
⃗ · E(⃗
⃗ x) = ρ(⃗x)
∇
ϵ0
⃗ × E(⃗
⃗ x) = 0
∇
Interesa encontrar una formulación matemática equivalente de este problema. Efectivamente, uno podría relacionar ambas ecuaciones, y obtener una única ecuación general que
permita solucionar cualquier problema electrostático. De la segunda ecuación, se desprende que
⃗ × E(⃗
⃗ x) = 0 → E(⃗
⃗ x) = −∇φ(⃗
⃗ x)
∇

Utilizando ésto en la primera ecuación
⃗ · (−∇φ(⃗
⃗ x)) = ρ(⃗x)
∇
ϵ0
Se obtiene la Ecuación de Poisson
⃗ 2 φ(⃗x) = − ρ(⃗x)
∇
ϵ0
⃗2=∇
⃗ ·∇
⃗ es el conocido Laplaciano. Con esto, hemos logrado reducir
Donde el operador ∇
aún más el problema de la electrostática, y todo consiste en encontrar un campo escalar que
satisfaga la ecuación de Poisson en una región del espacio con las condiciones de borde ade⃗ x) = −∇φ(⃗
⃗ x) y
cuadas. Una vez resuelta esta ecuación, se puede obtener el campo como E(⃗
luego todo el problema estará completo.
La ecuación de Poisson es una ecuación diferencial parcial, que en coordenadas cartesianas
equivale a
∂ 2 φ(x, y, z) ∂ 2 φ(x, y, z) ∂ 2 φ(x, y, z)
+
+
= − ρ(x, y, z)
∂x
∂y
∂z
ϵ0

En regiones del espacio libres de carga (ρ(⃗x) = 0), se debe resolver la Ecuación de Laplace
con condiciones de borde adecuadas
⃗ 2 φ(⃗x) = 0
∇

Las ecuaciones de Poisson y Laplace aparece en diversas ramas de la física, como en gravitación, dinámica de fluídos, propagación del calor, etc

---

### Página 145

Evidentemente, resolver las ecuaciones de Poisson o Laplace puede resultar analíticamente
muy complejo, sin embargo existen casos donde la simetría permite resolver éstas ecuaciones
sin mayor dificultad. En electrostática existen varios métodos para resolver problemas Poisson
- Laplace, algunos de ellos son
Método de las imágenes
Expansión del potencial en polinomios ortogonales
Funciones complejas analíticas, que resuelven Laplace en 2 dimensiones
Método de las funciones de Green
Métodos numéricos
Algunos de estos métodos serán desarrollados en detalle en capítulos siguientes

---

### Página 146

Problema
Una esfera de metal de radio R y carga q está rodeada por un cascarón esférico metálico de
radio interior a y radio exterior b. El cascarón no tiene carga neta
a) Encuentre la densidad superficial de carga en cada superficie
b) Encuentre el potencial en el centro utilizando infinito como punto de referencia
c) Si la esfera exterior se conecta a tierra bajando su potencial a cero (igual que en infinito),
¿Cómo cambian las respuestas anteriores?

#### Solución
a) Como la esfera de radio R es metálica (conductora), toda la carga debe estar concentrada
en su superficie. Dada la simetría esférica del problema, esta distribución de carga debe ser
uniforme, es decir
q
4πR2
Ahora, el cascarón es eléctricamente neutro, sin embargo en sus superficies (Sa y Sb ) se
induce carga de forma que el campo eléctrico en su interior sea nulo
σR =

⃗ x) = ⃗0 para a < r < b. Tomando una superficie Gaussiana esférica de
Debe tenerse que E(⃗
radio r, a < r < b
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 0
x ) · E(⃗
✝ ✆dS(⃗
S

⃗ x) es nulo en todos los puntos interiores del cascarón. Por otro lado
ya que E(⃗
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = Qint
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
luego Qint = 0, donde

---

### Página 147

Qint = q + σa 4πa2 = 0
y se obtiene la densidad superficial de carga en la superficie interior del cascarón
σa = −

q
4πa2

Como el cascarón es neutro, debe tenerse que
σa 4πa2 + σb 4πb2 = 0
−q + σb 4πb2 = 0
q
4πb2
Es decir, sobre la superficie interna se induce una carga total −q, y sobre la superficie externa, por supuesto, q.
σb =

b) Distinguimos 4 regiones, como se indica en la figura

Como las regiones I y III están contenidas en el interior de un conductor
⃗ x) = 0, ⃗x ∈ I, ⃗x ∈ III
E(⃗
Para encontrar el campo eléctrico en las regiones II, y IV , utilizamos la ley de Gauss.
Tomando una superficie esférica de radio r con R < r < a (región II), se tiene
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 4πr2 E(r) = q
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
⃗
E(r)
=

q
r̂, R < r < a
4πr2 ϵ0

Del mismo modo, para una superficie esférica de radio r, con r > b (región IV ), se tiene
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 4πr2 E(r) = q
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
⃗
E(r)
=

q
r̂, b < r
4πr2 ϵ0

---

### Página 148

Con esto, podemos calcular el potencial en el origen
ˆ ∞
⃗ x′ )
φ(0) =
d⃗x′ · E(⃗

tomando, por supuesto, un camino radial
⃗x′ = rr̂
d⃗x′ = drr̂
r ∈ [r, ∞]
φ(0) =

ˆ ∞

φ(0) =

ˆ R

drE(r) +

ˆ a

⃗
drr̂ · E(r)r̂
=

ˆ a

drE(r) +

R

drq
φ(0) =
+
R 4πϵ0 r

ˆ ∞

ˆ b

drE(r)

drE(r) +

a

ˆ ∞
b

drq
q
=
4πϵ0 r
4πϵ0

ˆ ∞

drE(r)

b

!

+ −
b R a

"

c) Ahora, se tiene

⃗ x) = 0 para ⃗x ∈ III (interior de un conductor). Esto
Al igual que antes debe tenerse que E(⃗
simplemente se traduce en
q + σa 4πa2 = 0
(por ley de Gauss). Es decir, al igual que antes
q
4πa2
Además el potencial ahora es nulo sobre la superficie exterior Sb , esto quiere decir que
ˆ ∞
⃗ x′ ) = 0
φ(b) =
d⃗x′ · E(⃗
σa = −

b

para cualquier camino entre b y el infinito. Por supuesto, esto requiere que
⃗ x′ ) = 0∀⃗x ∈ IV
E(⃗

---

### Página 149

Notar que esto implica que la carga encerrada por una superficie Gaussiana contenida en
IV necesariamente es cero. Es decir, el cascarón ya no es un objeto eléctricamente neutro (se
debe inducir una carga neta en el, igual a −q).
q + σa 4πa2 + σb 4πb2 = q − q + σb 4πb2 = 0
σb = 0

---

### Página 150

Problema
Una esfera metálica se encuentra inicialmente descargada. Ahora imagine que una carga positiva
q es colocada en algún lugar (no necesariamente al medio) dentro de la esfera y sin tocar las
paredes.

a) ¿Qué carga se induce en la pared interior y exterior de la esfera? Indicar cualitativamente la
concentración de densidad de carga inducida . Describir cómo son las líneas de campo eléctrico
dentro y fuera de la esfera
b) Suponga que se mueve la carga q dentro de la cavidad. ¿Cambia la distribución en la superficie
exterior de la esfera?
c) Ahora se coloca la carga q en contacto con la superficie interior de la esfera.¿Cómo queda la
distribución de carga en la superficie interior y exterior?
d) ¿Qué sucede si ahora se acerca otra carga q ′ cerca de la superficie exterior del conductor?
#### Solución
a) La carga q en el interior de la esfera metálica inducirá una separación de carga en el metal. Sea
qint la carga total inducida en la superficie interior, y qout la carga total inducida en la superficie
exterior. Debido a que la esfera inicialmente se encuentra descargada, la ley de conservación de
la carga indica que se debe tener
qin + qout = 0
¿Cuánto vale qint ? Tomemos una superficie Gaussiana contenida enteramente dentro del
cascarón esférico como se muestra en la figura

La carga total encerrada por esta superficfie es
qenc = qint + q
⃗ es cero en el interior de metal, la ley de Gauss
Pero, debido a que el campo eléctrico E
indica

---

### Página 151

✞☎ ⃗
⃗ x) = (qint + q) = 0
x) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0
De esta forma qint = −q, y entonces qout = q. La distribución de éstas cargas y sus respectivas
líneas de campo son como se aprecia en la siguiente figura

La carga negativa en la superficie interna se concentra mayoritariamente en la parte de la
esfera más cercana a la carga q. En contraste, la carga positiva de la superficie exterior se distribuye uniformemente sobre la superficie exterior. Ésto último debido a que la esfera metálica
es una superficie equipotencial, y la única forma de que esto suceda es que el campo sea radial
y uniforme sobre la superficie exterior
El campo eléctrico fuera de la esfera es
⃗
E(r)
=

1 q
r̂
4πϵ0 r2

tal como si la carga q se encontrara en el centro del conductor
b) La distribución de carga en el exterior no cambia al mover la carga q en el interior, por
la misma razón anterior. Por supuesto, la carga inducida en el interior de la superficie si se
vuelve a distribuír en la medida que movemos q, para asegurar que el campo en su interior siga
⃗ = 0. Ésto resulta interesante, pues desde el exterior del conductor podríamos
siendo nulo E
saber cuanta carga se encuentra en el interior, pero no podremos asegurar en que posición se
encuentra.
c) Cuando la carga q toca la superficie interior, la carga inducida −q se concentrará enteramente en el punto de contacto y cancelará la carga q.
d) Si se acerca ahora otra carga q ′ al exterior de la esfera, entonces la carga se distribuirá en
la superficie exterior de forma de ser una equipotencial. La distribución de carga al interior no
cambia debido a la prescencia de una carga en el exterior. En otras palabras, si una cavidad
está encerrada en un conductor, ninguna distribución estática de carga en el exterior podrá producir campos dentro. Este principio se conoce como shielding, y explica el por qué los aparatos
eléctricos se encuentran en cubiertas metálicas. .

---

### Página 152

Problema
Dos cavidades esféricas, de radios a y b están contenidas en el interior de una esfera conductora
neutra de radio R. En el centro de cada cavidad hay una carga puntual qa y qb

a) Encuentre las densidades de carga superficiales
b) ¿ Cuál es el campo eléctrico fuera del conductor?
c) ¿Cuál es el campo dentro de cada cavidad?
#### Solución
a) Sobre las superficies Sa y Sb en cada cavidad se inducirá carga de forma de anular el efecto de
las cargas puntuales en el interior del conductor. Sean dos superficies S1 y S2 como se muestra
en la figura

Como S1 está contenida en el interior del conductor
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 0 = Qint
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
se obtiene
Qint = 0 = qa + σa 4πa2 = 0
se obtiene la densidad superficial de carga inducida en la cavidad
σa =

−qa
4πa2

Del mismo modo, y utilizando la ley de Gauss con la superficie S2 , se obtiene
qb
4πb2
Como el conductor es neutro, se inducirá carga en la superficie exterior, de forma que
σb = −

−qa − qb + σR 4πR2 = 0
σR =

qa + q b
4πR2

---

### Página 153

b) El efecto de las cargas puntuales qa y qb es anulado mediante las cargas inducidas en las
cavidades. Con esto, el campo exterior posee una simetría esférica, y se puede obtener por la
ley de Gauss

✞☎ ⃗ ′
⃗ x′ ) = 4πr2 E(r) = qa + qb
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

qa + q b
⃗
E(r)
=
r̂, r > R
4πr2 ϵ0
c) Dentro de la cavidad a, el campo es simplemente el de la carga puntual qa
⃗a =
E

qa r̂a
4πϵ0 ra2

donde ra es la distancia desde un punto interior a la cavidad a a la carga puntual qa . Del
mismo modo, dentro de la cavidad b
⃗b =
E

qb r̂b
4πϵ0 rb2

---

### Página 154

Problema
Un sistema de dos esferas de radio a y b (con a > b) conductoras cargadas posee una carga total
Q. Si ellas están separadas por una gran distancia y se les conecta con un alambre conductor de
dimensiones despreciables, calcule la carga total sobre cada esfera y la magnitud aproximada
del campo eléctrico sobre la superficie de cada una.

#### Solución
Sabemos lo siguiente: Cada esfera tiene una carga desconocida, pero su suma sí lo es
QA + QB = Q
Notemos que el sistema entero es un conductor, y por lo tanto, es un equipotencial. Además,
como las esferas están separadas por una gran distancia, entonces el campo producido por una
afecta de manera despreciable el campo de la otra. En la vecindad exterior de A, el campo es
de la forma
QA
r̂
2 A
4πϵ0 rA

⃗A =
E
y en la vecindad de B es de la forma

QB
r̂
2 B
4πϵ0 rB

⃗B =
E

Ahora usemos el hecho que el sistema completo es un conductor, y por lo tanto φ(a)−φ(b) =
ˆ a

⃗ A · d⃗l = QA
E
4πaϵ0
∞
ˆ b
⃗ A · d⃗l = QB
φ(b) = −
E
4πbϵ0
∞

φ(a) = −

De donde
QB
QA
=
4πϵ0 a
4πϵ0 b
Lo que equivale a
QA = QB

a
b

y usando que Q = QA + QB
QA =

aQ
a+b

---

### Página 155

bQ
a+b
Con esto, el campo eléctrico sobre la superficie de la esfera A tiene como magitud
QB =

EA =

aQ
4πϵ0 (a + b)a2

EA =

Q
4πϵ0 (a + b)a

⃗B =
E

bQ
4πϵ0 (a + b)b2

⃗B =
E

Q
4πϵ0 (a + b)b

y para la esfera B

De esta forma,
EA
b
= <1
EB
a
Es decir, el campo eléctrico sobre la esfera de radio menor es mayor que el campo sobre la
esfera de radio mayor. Los campos están en proporción inversa de los radios.
Éste es un efecto muy conocido, y ocurre cuando se carga un conductor que no es esférico, por
ejemplo, alguno que tenga una punta o un lado muy puntiaguido, como el de la figura

Entonces una cantidad relativamente pequeña de carga acumulada en la punta puede generar una densidad superficial de carga muy grande, y como consecuencia, un mayor campo justo
afuera. Este resultado es técnicamente muy importante, por que por ejemplo el aire se vuelve
conductor si el campo es demasiado grande.
Lo que sucede es que un ion cerca de la punta es acelerado por este campo intenso, y si
el campo es lo suficientemente grande, el ion puede obtener suficiente energía cinética antes
que golpee otro atomo y entonces podrá arrancar otro electrón de éste atomo. Como resultado,
se producen más y más iones. Este movimiento constituye una descarga. Si se desea cargar
entonces un conductor a un potencial alto y que no se produzcan descargas sobre él en el aire,
hay que asegurarse que la superficie sea suave, de forma que no hayan partes donde el campo
sea anormalmente alto

---

### Página 156

Problema
Considere dos placas metálicas conductoras de igual área A y separadas una distancia d. La
placa superior posee carga Q mientras que la placa inferior tiene carga −Q. Encontrar la capacidad del sistema

#### Solución
Para encontrar la capacidad C, primero debemos conocer la forma del campo eléctrico en
el interior del condensador (y luego determinar la diferencia de potencial entre placas). Por
supuesto que un condensador real tiene un largo finito, luego, las líneas de campo cerca del
borde de las placas se deforman, y el campo no está contenido totalmente entre las placas. En
la figura se aprecian las líneas de campo considerando el efecto de los bordes

De todas formas, ignoraremos éste tipo de efectos asumiendo una situación ideal, en donde
las líneas de campo son rectas . En el límite cuando las placas tienen largo infinito (o bien un
largo mucho mayor que la separación), el campo tendrá simetría plana y entonces podemos
usar la ley de Gauss para determinar su magnitud
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = qin
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S

Elegimos una superficie de Gauss con forma de caja, de área A′ , tal como muestra la figura

---

### Página 157

Como el campo en el interior del conductor es nulo, sólo hay flujo sobre una de las tapas, de
esta forma la ley de Gauss queda
ˆˆ
′
✞☎ ⃗ ′
⃗ x′ ) = EA′ = qin = σA
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
ϵ0
S
de donde el campo eléctrico al interior del condensador tiene magnitud igual a
E=

σ
ϵ0

Ahora, la diferencia de potencial entre las placas del condensador se obtiene integrando el
campo sobre una curva que va desde la placa positiva hasta la placa negativa. Por supuesto
elegimos una trayectoria paralela en todo instante al campo
ˆ −
⃗ · d⃗l = −Ed
E
∆V = φ− − φ+ = −
+

Para obtener la capacidad, el término relevante es el valor absoluto de esta diferencia de
potencial, digamos
| ∆V |= Ed
De esta forma, la capacidad de un condensador plano está dada por
C=

Q
ϵ0 A
=
| ∆V |
d

Claramente depende únicamente de la geometría del condensador, y aumenta linealmente
con el área de las placas. Mientras mayor área, mayor capacidad de almacenar carga tiene para
una misma diferencia de potencial entre sus placas. Además es inversamente proporcional a la
distancia d entre placas, esto debido a que mientras menor es la distancia, menor es la diferencia
de potencial entre ambas para una carga fija Q.
Ahora, si tenemos un condensador plano de área cuadrada y de lado 10 cm, tendremos
A = 0, 1 × 0, 1 = 0, 01 m2
Suponiendo un ancho d = 1 cm, tenemos que la capacidad vale
C=

9 × 10−12 × 0, 01
0, 01

C = 9 × 10−12 F
Como ejemplo, si al condensador se aplica una diferencia de potencial de 1, 5 Volts (pila
2A), será capaz de almacenar una carga igual a
Q = C∆V = 1, 5 × 9 ∗ 10−12 = 1, 35 × 10−11

---

### Página 158

Problema
Considere un cilindro sólido de radio a rodeado por una cáscara cilíndrica de radio interior
b. La longitud de ambos cilindros es L y consideramos que este largo es mucho mayor que las
dimensiones de b−a, la separación entre cilindros, de manera que se puede despreciar los efectos
de borde. El condensador se carga de forma que el cilindro interior posea carga Q y el exterior
carga −Q. ¿Cuál es la capacidad?

#### Solución
Para obtener la capacidad debemos primero obtener el campo eléctrico en cualquier parte en
la región entre ambos conductores. Debido a la simetría cilíndrica del sistema, elegimos por
supuesto una superficie Gaussiana como un cilindro coaxial con longitud l < L y radio r donde
a < r < b. Usando la ley de gauss, tenemos

ˆˆ

ˆˆ

☎
✞☎ ⃗ ′
⃗ x′ ) = ✞
x ) · E(⃗
✝ ✆E(r)r̂ · dS r̂ = E(r)2πrl
✝ ✆dS(⃗
S

S

Ahora, notar que por la simetría, para que los cilindros sean equipotenciales, el campo debe
ser radial a sus superficies, y luego, deben tener una densidad superficial de carga uniforme σ.
La carga encerrada por el cilindro de Gauss es, simplemente
2πalσ
ϵ0

qin =
Con esto,

aσ
ϵ0 r
Notar que el campo eléctrico es diferente de cero únicamente en la region a < r < b. Para
r < a la carga encerrada es qenc = 0 ya que la carga neta del conductor de radio a debe ubicarse
sobre su superficie. Del mismo modo, para r > b, la carga total encerrada es 0, debido a que un
condensador en su totalidad es neutro, es decir, cualquier superficie que encierre completamente
al condensador encierra una carga total igual a cero.
E(r) =

La diferencia de potencial está dada por
∆V = φb − φa = −
aσ
φb − φa = −
ϵ0

ˆ b
a

ˆ b

⃗ · d⃗l = −
E

ˆ b

dr
aσ
= − ln
ϵ0
a r

Er dr

a

! "
b
a

---

### Página 159

donde el camino de integración tiene la dirección radial del campo eléctrico. Como era
de esperarse, el conductor exterior con carga negativa tiene menor potencial. De esta forma
tenemos
C=

Q
2πϵ0 L
σ2πaLϵ0
=
=
b
∆V
ln(b/a)
aσln( a )

Claramente sólo función de los factores geométricos. Consideremos un condensador cilíndrico de largo L = 5 cm
b = 0, 5 cm, a = 0, 1cm
C=

2π9 × 10−12 × 0, 05
= 1, 75 ∗ 10−12 F
ln(5)

Si conectamos una bateria de 5 Volt a este condensador, se almacenará una carga de
Q = C∆V = 8, 784 × 10−12 C

---

### Página 160

Problema
Considere un condensador esférico, que consiste de 2 esféras concéntricas de radios a y b. La
cáscara interior posee carga Q distribuída uniformemente sobre su superficie, y la esfera exterior
posee una carga igual pero opuesta −Q. Cuál es la capacidad de esta configuración?

#### Solución
El campo eléctrico sólo es distinto de cero en la región a < r < b. Usando la ley de Gauss con
una superficie esférica y de radio r como se muestra en la figura

✞☎ ⃗ ′
⃗ x′ ) = Er A = Er 4πr2 = Q
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

de donde

1 Q
4πϵ0 r2
La diferencia de potencial entre las dos cáscaras conductoras es
ˆ b
⃗
d⃗l · E
∆V = φb − φa = −
E(r) =

a

Q
φb − φa = −
4πϵ0
de donde obtenemos

ˆ b

Q
dr
=−
4πϵ0
a r

!

1 1
−
a b

Q
C=
= 4πϵ0
| ∆V |

!

"

ab
b−a

Q
=−
4πϵ0
"

!

b−a
ab

"

Ahora, para un conductor esférico aislado, también se puede hablar de capacidad, ésta se
obtiene tendiendo el radio b a infinito, luego, la capacidad de la esfera conductora de radio a es
!
"
ab
a
Ca = lím C = 4πϵ0 lím
= 4πϵ0 lím
a = 4πϵ0 a
b→∞
b→∞
b→∞ (1 − )
b−a
b
Luego, para una esfera conductora de radio R, su capacidad es
C = 4πϵ0 R

---

### Página 161

Este resultado también se podría obtener considerando que una esfera de radio R con carga
Q uniformemente distribuída sobre su superficie posee un potencial φ = 4πϵQ0 R , usando infinito
como referencia para el potencial, esto da
C=

Q
Q
=
= 4πϵ0 R
| ∆V |
Q/4πϵ0 R

---

### Página 162

Problema
Considere un conductor esférico de radio a dentro de otro de radio b. En el espacio entre ambos conductores se introduce un cascarón esférico (concéntrico) conductor de radios interno y
externo c y d, respectivamente. Si el conductor de radio a tiene carga Q y el exterior de radio
b tiene −Q, discuta que ocurre con la capacidad al introducir el cascarón

#### Solución
En el problema anterior se obtuvo que la capacidad de un condensador esférico está dada por
!
"
Q
ab
C=
= 4πϵ0
| ∆V |
b−a

Veamos que ocurre cuando se introduce un conductor neutro entre a y b. Distinguimos 3
regiones, como se indica en la figura

Claramente el campo (de existir) en todo el espacio presenta una dependencia radial. Por
ley de Gauss,utilizando una superficie esférica de radio r, con a < r < c
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = E(r)4πr2 = Q
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
⃗
E(r)
=

Q
r̂, a < r < c
4πϵ0 r2

Para la región II, dada por c < r < d
⃗ x) = 0, ∀⃗x ∈ II
E(⃗
pues corresponde al interior de un conductor. En consecuencia, se induce una carga −Q
sobra la superficie interna del cascarón. Dado que éste es neutro, sobre su superficie exterior sei
induce carga Q. Para la región III, exactamente el mismo resultado encontrado en la región I

---

### Página 163

⃗
se obtiene para el campo eléctrico E(r),
d < r < b. Vemos que este conductor altera el campo
eléctrico en el interior (con respecto al caso en que no está), donde la única diferencia es que
se anula para cierta región interior, claramente disminuyendo la diferencia de potencial entre el
conductor de radio a y el conductor de radio b, en consecuenctia, aumentará la capacidad del
sistema. En efecto
ˆ b
ˆ b
⃗
⃗
∆V = φa − φb =
d⃗x · E(⃗x) =
d⃗r · E(r)
a

a

donde se ha utilizado un camino radial para calcular la integral de línea, dada la naturaleza
del campo
ˆ c
ˆ d
ˆ b
⃗
⃗
⃗
∆V =
d⃗r · E(r) +
d⃗r · E(r) +
d⃗r · E(r)
a

c

d

⃗
y como E(r)
= 0 ∀c < r < d
∆V =

ˆ c

∆V =

ˆ c

a

∆V =
Pero c < d, entonces

ˆ b

⃗
d⃗r · E(r)

Q
+
4πϵ0 r2

ˆ b

dr

Q
4πϵ0 r2

1 1 1 1
− + −
a c d b

"

Q
4πϵ0

dr

a

∆V =

⃗
d⃗r · E(r)
+

!
!

d

d

1 1 1 1
− + −
a b d c

"

Q
4πϵ0

1 1
> ⇒ − <0
c
d
d c
En consecuencia, la diferencia de potencial entre el conductor interior y exterior disminuye
en comparación al caso en que no está el cascarón. De esta forma
C=

Q
∆V

es mayor que el del condensador esférico original

---

### Página 164

Problema
Tres cáscaras esféricas conductoras concéntricas muy delgadas poseen radios a,b, y c, respectivamente, siendo a < b < c. Inicialmente la cáscara interior está descargada, la del medio posee
una carga total negativa −Q y la externa una carga total positiva Q

a) Encuentre el potencial electrostático en cada una de las cáscaras conductoras
b) Si las cáscaras interior y exterior son conectadas mediante un alambre conductor muy delgado que está aislado al pasar por la cáscara central, ¿Cuál es ahora el potencial eléctrico de
cada una de las cáscaras? ¿Cuál es la carga en cada una de las esferas?
#### Solución
Distinguimos naturalmente tres regiones del espacio, dadas por I : r < a, II : a < r < b,
III : b < r < c, IV : r > d. En cada una de ellas el campo eléctrico posee dirección radial y su
magnitud depende únicamente de la distancia r al centro del conductor interno. Utilizando la
ley de Gauss para la región I : r < a
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 0, ∀S ∈ I
x ) · E(⃗
✝ ✆dS(⃗
S

⃗ x) = 0 ∀⃗x ∈ I (interior de un conductor). Para la región II
pues E(⃗
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = Qint = 0
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
pues la cáscara de radio a se encuentra inicialmente descargada. De esta forma, el campo
⃗ x) = 0 ∀⃗x ∈ II. Del mismo modo, utilizando una
eléctrico también es nulo en esta región, E(⃗
superficie esférica de radio r, con b < r < c
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 4πr2 E(r) = −Q
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
−Q
⃗
E(r)
=
r̂
4πϵ0 r2
Por último, para r > d
ˆˆ

✞☎ ⃗ ′
⃗ x′ ) = 0, ∀S ∈ IV
x ) · E(⃗
✝ ✆dS(⃗
S

pues la carga encerrada por cualquier superficie contenida en la región IV es cero. En
resumen
⎧
si r < b
⎨ 0
−Q
⃗
r̂
si
b<r<c
E(r) = 4πϵ0 r2
⎩
sir > c

---

### Página 165

El potencial en la cáscara exterior es
φ(c) =

ˆ ∞
c
′

⃗ x)
d⃗x′ · E(⃗

tomando por supuesto un camino radial ⃗x = rr̂, d⃗x′ = drr̂, r ∈ (c, ∞)
ˆ ∞
⃗
drr̂ · E(r)
=0
φ(c) =
c

El potencial en la cáscara de radio b es
ˆ ∞
ˆ c
−Q
φ(b) =
drr̂ · E(r)r̂ =
dr
4πϵ0 r2
b
b
ˆ c
dr
Q
Q &&c
φ(b) = −
=
&
4πϵ0 b r2
4πϵ0 r b
!
"
Q
b−c
φ(b) =
4πϵ0
bc

por último, el potencial en r = a es
ˆ b
ˆ c
ˆ ∞
ˆ ∞
drr̂ · E(r)r̂ =
drE(r) +
drE(r) +
drE(r)
φ(a) =
a

a

φ(a) =

ˆ c

b

drE(r) = φ(b) =

b

Q
4πϵ0

c

!

b−c
bc

"

b) Ahora se tiene la siguiente configuración

Los conductores de radio a y c se encuentran unidas al mismo potencial. De esta forma,
la carga contenida inicialmente en estos dos conductores se distribuirá, donde por supuesto se
debe tener
Qa + Qc = Q
Definiendo las mismas regiones anteriores, nuevamente se tiene
⃗ x) = 0, ∀⃗x ∈ I
E(⃗
⃗ x) = 0, ∀⃗x ∈ IV
E(⃗

(región I es el interior de un conductor y la carga total del sistema sigue siendo nula). El
campo en la región II se obtiene con la ley de Gauss (superficie esférica de radio r, a < r < b)

---

### Página 166

✞☎ ⃗ ′
⃗ x′ ) = E(r)4πr2 = Qa
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

Qa
r̂
4πϵ0 r2
y del mismo modo, tomando una superficie esférica de radio r, b < r < c
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = E(r)4πr2 = −Q + Qa
x ) · E(⃗
✝ ✆dS(⃗
ϵ0
S
⃗
E(r)
=

Qa − Q
⃗
E(r)
=
r̂
4πϵ0 r2
El potencial en r = c es, por supuesto, nulo
ˆ ∞
drE(r) = 0
φ(c) =
c

además
ˆ c

ˆ c

Qa − Q
4πϵ0 r2
b
b
b
!
"
ˆ
Qa − Q c 1
Qa − Q c − b
φ(b) =
dr 2 =
4πϵ0
r
4πϵ0
bc
b

φ(b) =

y

ˆ ∞

φ(a) =

drE(r) =

ˆ ∞

drE(r) =

drE(r) =

a

ˆ b

dr

drE(r) + φ(b)

a

ˆ b

Qa
Qa
φ(a) = φ(b) +
dr
=
φ(b)
+
4πϵ0 r2
4πϵ0
a
pero las cargas inducidas en a y c deben ser tal que

!

b−a
ab

"

=0

"

φ(a) = φ(c) = 0
luego
Qa − Q
φ(a) =
4πϵ0

!

c−b
bc

"

Qa
+
4πϵ0

b−a
ab

c−b
b−a
+ Qa
=0
bc
ab
!
"
c−b b−a
c−b
+
=Q
Qa
bc
ab
bc
"
"
!
!
c−b
ac − ab + bc − ac
b(c − a)
=Q
→ Qa
= Q(c − b)
Qa
abc
bc
a
φ(a) = (Qa − Q)

Finalmente

!

Qa = Q

a(c − b)
b(c − a)

---

### Página 167

Problema
Considere un condensador de placas paralelas cargadas con densidades σ y −σ , como muestra
la figura. Se arroja una carga q horizontalmente por el espacio entre las placas con velocidad
vx . Encuentre la trayectoria seguida por la partícula cargada y el ángulo que forma su vector
velocidad con la horizontal al momento de salir, considerando que l es lo suficientemente grande
como para que la carga no choque con alguna de las placas. Considere además que en todo
instante la carga q siente una fuerza electrostática

#### Solución
El campo eléctrico en la región entre placas, despreciando efectos de borde y considerando
d >> l está dado por
⃗ x) = σ ĵ + σ ĵ
E(⃗
2ϵ0
2ϵ0
⃗ x) = σ ĵ
E(⃗
ϵ0
Así, la fuerza electrostática que siente la carga q está dada por
σ
F⃗ = q ĵ
ϵ0
Notar que estrictamente esto es válido únicamente cuando q está quieta, sin embargo consideraremos que esta fuerza de interacción se mantiene a medida que la carga se mueve. De la
segunda ley de Newton
⃗a =

1 ⃗
qσ
F =
ĵ
m
mϵ0

De esta forma, la cinemática de la carga está descrita por
x(t) = vx t
y(t) =

1 qσ 2
t
2 mϵ0

y las velocidades
Vx (t) = vx
qσ
Vy (t) = at =
t
mϵ0
donde el origen coincide con la posición inicial de la carga la momento de ingresar a la
región. Para obtener la trayectoria, utilizamos
t=

x(t)
vx

---

### Página 168

y entonces
y(x) =

1 qσ x2
2 mϵ0 vx2

la trayectoria es una parábola en el plano x − y

El tiempo que demora la carga en llegar al extremo derecho es
d
vx
con esto, la velocidad vertical en el momento en que sale es
td =

Vy (td ) = atd =

qσ d
mϵ0 vx

!

"

y el ángulo α está dado por
−1

α = tan

−1

α = tan

!

Vy (td )
Vx (td )
qσd
mϵ0 vx2

"

---

### Página 169

Problema
Dos cilindros muy largos y concéntricos, de radios a y b, con b > a, se encuentran inicialmente
descargados. La región entre ambos se llena con una densidad homogénea de carga ρ, y luego
cada uno de los cilindros se conectan a tierra. Calcule, resolviendo a -la- Poisson, el potencial
y el campo eléctrico en la región interior.

#### Solución
En la región interior a ambos cilindros, es decir a < r < b, el potencial satisface la ecuación de
Poisson
⃗ 2 φ(⃗x) = − ρ(⃗x)
∇
ϵ0
Si usamos coordenadas cilíndricas, el potencial podría depender de ϑ, r y z. Sin embargo,
de la simetría del problema es evidente que
∂φ
=0
∂ϕ
con lo que φ = φ(r, z). Además, debido a que la longitud de los cilindros es mucho mayor a
(b−a), el potencial también debe ser simétrico con respecto a z. De esta forma, podemos despreciar efectos de borde y considerar que el potencial es sólo una función radial de la forma φ = φ(r)
Ahora, el Laplaciano en coordenadas cilíndricas para una función que sólo depende de r es
⃗ 2 φ(r) = 1 ∂ (r ∂φ(r) )
∇
r ∂r
∂r
De esta forma, la ecuación de Poisson se transforma en
ρ
1 ∂ ∂φ
(r ) = −
r ∂r ∂r
ϵ0
Equivalentemente

Luego

∂ ∂φ
rρ
(r ) = −
∂r ∂r
ϵ0
∂φ
r
=−
∂r

ˆ

dr

rρ
+C
ϵ0

∂φ
r2 ρ
r
+C
=−
∂r
2ϵ0
∂φ
rρ
C
=−
+
∂r
2ϵ0
r

---

### Página 170

Finalmente
φ(r) = −

ˆ

rρ
dr
+
2ϵ0

ˆ

dr

C
r

r2 ρ
+ C ln r + A
4ϵ0
Esta es la solución general de la ecuación de Poisson para un potencial de simétría cilíndrica,
dependencia radial, y densidad de carga constante. Ahora debemos imponer las condiciones de
borde adecuadas para que la solución sea única (Problema Poisson-Dirichlet)
φ(r) = −

Tenemos φ(a) = 0 Equivale a imponer que la superficie cilíndrica de radio a es una equipotencial conectada a tierra. Luego
φ(a) = −

a2 ρ
+ C ln a + A = 0
4ϵ0

Además, φ(b) = 0, con esto
b2 ρ
+ C ln b + A = 0
4ϵ0
Restando ambas ecuaciones, obtenemos
φ(b) = −

(b2 − a2 )ρ
0 = C(ln a − ln b) +
4ϵ0
De donde obtenemos la constante C
C=

(a2 − b2 )ρ
4ϵ0 ln(a/b)

De la primera condición despejamos A
A=
A=

a2 ρ
(a2 − b2 )ρ
− ln a
4ϵ0
4ϵ0 ln(a/b)

a2 ln(a/b)ρ − lna(a2 − b2 )ρ
4ϵ0 ln(a/b)
A=

ρ(b2 ln a − a2 ln b)
4ϵ0 ln(a/b)

Con esto, la solución del potencial para a < r < b es
φ(r) = −

r2 ρ
(a2 − b2 )ρ
ρ(b2 ln a − a2 ln b)
+
ln r +
4ϵ0 4ϵ0 ln(a/b)
4ϵ0 ln(a/b)

Hermoso resultado. Ahora, para obtener el campo eléctrico, usamos el hecho
⃗ x) = −∇φ(⃗
⃗ x)
E(⃗
el operador gradiente en coordenadas cilíndricas para una función que sólo depende de r es
∂φ(r)
⃗
r̂
∇φ(r)
=
∂r
de manera que

---

### Página 171

∂φ
⃗
E(r)
= − r̂
∂r
!
"
(a
rρ
−
b
)ρ
⃗
−
E(r)
=
r̂
2ϵ0 4ϵ0 r ln(a/b)

⃗ es nulo, ya
que es el campo eléctrico para a < r < b. Para r < a es claro que el campo E
que no hay carga encerrada por el conductor interior.
Calculemos las densidades de cargas sobre los conductores. Para el conductor interior, tenemos que el campo eléctrico sobre su superficie tiene magnitud
E(a) =

(a2 − b2 )ρ
aρ
−
2ϵ0 4ϵ0 a ln(a/b)

La densidad de carga sobre la superficie de un conductor se relaciona con el campo eléctrico
según
σ
E=
ϵ0
Con esto la densidad de carga será
!
"
(a2 − b2 )ρ
aρ
−
σ1 = ϵ0
2ϵ0 4ϵ0 a ln(a/b)
El campo eléctrico en la superficie del conductor exterior tiene magnitud
E(b) =

(a2 − b2 )ρ
bρ
−
2ϵ0 4ϵ0 b ln(a/b)

!

(a2 − b2 )ρ
bρ
−
2ϵ0 4ϵ0 b ln(a/b)

y la densidad de carga será
σ2 = ϵ0

"

---

### Página 172

Problema
Considere el siguiente dispositivo

a) Determine el potencial y el campo eléctrico entre las placas.
b) Determine la capacidad por unidad de largo.
Desprecie los efectos de borde.
#### Solución
a) Sabemos que las líneas equipotenciales deben respetar la geometría del dispositivo. De esta
forma, las equipotenciales serán rectas radiales, es decir

Por lo tanto, las líneas de campo, al ser perpendiculares a las equipotenciales, deben seguir la
dirección θ̂, es decir, son arcos concéntricos.

Si suponemos que el dispositivo es muy largo en la dirección Z, entonces se puede suponer que
⃗ = E(r, ϑ)ϑ̂
E
Pero
∂φ
1 ∂φ
⃗ = −∇φ(r,
⃗
E
ϑ) = − r̂ −
ϑ̂
∂r
r ∂ϑ

---

### Página 173

Como el campo tiene dirección θ̂, ∂φ
=0
∂r
Luego, se tiene que el potencial sólo depende de ϑ, lo cual era de esperarse.
Planteamos la ecuación de Laplace en coordenadas cilíndricas:

⃗ 2φ = 0 = 1 ∂ φ = 0
∇
r2 ∂ϑ2
φ(ϑ) = Aϑ + B
Pero la placa inferior está conectada a tierra
φ(0) = 0 → B = 0
φ(ϑ0 ) = φ0 → A =
Finalmente
φ(ϑ) =

φ0
ϑ0

φ0
ϑ
ϑ0

⃗ ϑ) = − 1 φ0 ϑ̂
E(r,
r ϑ0
b)Calculemos la capacidad por unidad de largo.
Q
V
La carga por unidad de largo, Q, de una de las placas puede calcularse a partir de la
densidad de carga σ que aparece en cada placa del condensador. Su valor puede determinarse
directamente del campo eléctrico
C=

⃗ · n̂ = σ
E
ϵ0
De donde obtenemos
σ=

ϵ0 V0
r θ0

Así, el valor de Q es
Q=1

ˆ b

σ(r)dr =

a

ˆ b

ϵ0 φ0
φ0
b
dr = ϵ0 ln( )
ϑ0
a
a r ϑ0

Finalmente
C=

ϵ0
b
ln( )
ϑ0
a

---

### Página 174

Problema
El campo eléctrico sobre la superficie de la Tierra está dado por la expresión
⃗
E(z)
= −(ae−αz + be−βz )k̂
Con α, β > 0, y z la altura desde la superficie de la tierra.
a) Determine la densidad de carga
b) Calcule la cantidad total de carga contenida en una columna vertical de sección S que se
extiende teóricamente desde x=0 hasta x = ∞

#### Solución
a) Para obtener la densidad de carga, utilizamos la forma diferencial de la ley de Gauss
⃗ · E(⃗
⃗ x) = ρ(⃗x)
∇
ϵ0
En este caso
⃗ · E(⃗
⃗ x) = ∂Ex + ∂Ey + ∂Ez
∇
∂x
∂y
∂z
⃗ en x e y son nulas, así
Las componentes de E
αae−αz + βbe−βz =

ρ(z)
ϵ0

Finalmente
ρ(z) = ϵ0 (αae−αz + βbe−βz )

b) La carga total contenida en una columna vertical de sección S será
˚
ˆ ∞
ˆ ∞
Q=
ρ(z)d x = S
ρ(z)dz = S
ϵ0 (αae−αz + βbe−βz )dz

Q = Sϵ0 (a + b)

---

### Página 175

Problema
Se tienen dos cilindros conductores coaxiales, uno de radio a y el otro de radio b, conectados a
una diferencia de potencial V0 .
⃗ x) y φ(⃗x) en todo el espacio y σ en cada superficie.
Calcule ρ(⃗x),E(⃗

#### Solución
Utilizaremos la ecuacion de Laplace, esto es
⃗ 2 φ(r) = 0
∇
El laplaciano en coordenadas cilíndricas es
⃗ 2 φ = 1 ∂ (r ∂φ ) + 1 ∂ φ + ∂ φ
∇
r ∂r ∂r
r2 ∂φ2 ∂z 2

Si suponemos que el par de conductores cilíndricos es mucho más alto que su radio, entonces
se puede afirmar que el potencial no debe depender de la coordenada z, y por lo tanto ∂V
= 0.
∂z
Así mismo, como las características de los conductores no varían con el ángulo φ, también debe
cumplirse que ∂V
= 0.
∂φ
De esta forma la ecuación diferencial que debemos resolver es
1 ∂ ∂φ
(r ) = 0
r ∂r ∂r
Con condiciones de borde
φ(a) = V0 , φ(b) = 0
Esta ecuación se puede resolver integrándola directamente
φ(r) = A ln r + B
Esta solución general más las condiciones de borde nos entregan un sistema lineal de ecuaciones
A ln(a) + B = V0
A ln(b) + B = 0
De donde obtenemos
A=

V0
ln(a/b)

---

### Página 176

B=−

V0
ln b
ln(a/b)

Y el potencial entre las placas conductoras es
φ(r) =

V0
ln(r/b)
ln(a/b)

Válida solo entre a < r < b
⃗ x) = −∇φ(⃗
⃗ x), es decir
El campo eléctrico se puede calcular como E(⃗
E(r) = −

∂φ(r)
V0 1
=
,a < r < b
∂r
ln(b/a) r

⃗
E(r)

V0 1
r̂, a < r < b
ln(b/a) r

⃗ · E,
⃗ pero
La densidad de carga es ρ(r) = ϵ0 ∇
⃗ · ( r̂ ) = 0
∇
r
Con lo que ρ(r) = 0, es decir, no hay densidad de carga entre los conductores.
Para determinar las densidades de carga superficial en cada conductor hay que usar el hecho
de que el campo en la superficie de un conductor cumple
⃗ · n̂ = σ
E
ϵ0
De esta forma, para el conductor a
σa = ϵ0

V0
a ln(b/a)

Y para el conductor b
σb = −ϵ0

V0
b ln(b/a)

Todo el desarrollo anterior es válido para a < r < b.
En el cilindro interno, (r < a)
⃗
E(r)
=0
ya que dentro de un conductor en equilibrio electrostático el campo eléctrico es siempre
nulo. De esta forma
φ(r) = V0
ρ(r) = 0
Ahora, si r > b, para calcular el campo utilizamos
φ(b) − φ(∞) =

ˆ b
∞

⃗ · d⃗l =
E

ˆ b
∞

drE(r)

---

### Página 177

Pero φ(b) = 0, con lo que
E(r) = 0
Si el campo es 0, entonces φ = cte = φ(b) = 0, y ρ(r) = 0

---

### Página 178

Problema
Dos conos conductores concéntricos, cuyas ecuaciones en coordenadas esféricas son ϑ1 = π/6,
y ϑ2 = π/4 respectivamente, se muestran en la figura. Los conos son de extensión infinita y en
r = 0 están separados por una distancia infinitesimal. Si el cono interior está a un potencial de
⃗ en la región interior a
0 V, y el exterior a 50 V , determinar el potencial y el campo eléctrico E
ambos conductores

#### Solución
Sea V la región delimitada por ϑ1 < ϑ < ϑ2 . Si no hay densidad de carga libre en V , el potencial
satisface la ecuación de Laplace en V
⃗ 2φ = 0
∇
Dada la geometría del problema, es conveniente utilizar coordenadas esféricas
!
"
!
"
∂2φ
1 ∂
∂
∂φ
2 ∂φ
⃗
∇ φ(r, ϑ, ϕ) = 2
r
+ 2
sin ϑ
+ 2 2
r ∂r
∂r
r sin ϑ ∂ϑ
∂ϑ
r sin ϑ ∂ϕ2
El problema posee una clara simetría azimutal (el potencial claramente no depende del
ángulo polar ϕ). Además, debe existir una independencia en la coordenada r, pues la extensión
de los conos es infinita. De esta forma, el potencial debe ser únicamente función de ϑ, y se debe
resolver
!
"
∂
∂φ
⃗
∇ φ(r, ϑ, ϕ) = 2
sin ϑ
=0
r sin ϑ ∂ϑ
∂ϑ
Equivalentemente
∂
∂ϑ

!

∂φ
sin ϑ
∂ϑ

sin ϑ

"

=0

∂φ
= C1
∂ϑ

∂φ
= C1 cscϑ
∂ϑ
ˆ
dϑ
φ(ϑ) = C1
+ C2
sin ϑ
Además

ˆ

dϑ
= ln (tan ϑ/2) + C
sin ϑ

---

### Página 179

En efecto
d
(ln (tan ϑ/2) + C) =
sec2 ϑ/2 =
=
dϑ
tan ϑ/2
2 cos ϑ/2 sin ϑ/2
sin ϑ
con esto
φ(ϑ) = C1 ln (tan ϑ/2) + C2
Debemos imponer las condiciones de borde en las superficies conductoras. Se tiene
φ(ϑ1 ) = 0

φ(π/6) = C1 ln (tan π/12) + C2 = 0
Además
φ(ϑ2 ) = 50

φ(π/4) = C1 ln (tan π/8) + C2 = 50

Resolviendo el sistema para C1 y C2
50 = C1 (ln (tan π/8) − ln (tan π/12))
50 = C1 ln

C1 =
y

ln

!
'

tan π/8
tan π/12
tan π/8
tan π/12

"

(

C2 = −C1 ln (tan π/12)
Evaluando
C1 = 114,78834
C2 = 151,171411
y la solución es
φ(ϑ) = 114,78834 ln (tan ϑ/2) 151,171411

---

### Página 180

Para encontrar el campo eléctrico, utilizamos que
⃗ x) = −∇φ(⃗
⃗ x)
E(⃗
En coordenadas esféricas, y considerando que φ solo depende de ϑ
⃗ ϑ) = − 1 ∂φ ϑ̂
E(r,
r ∂ϑ
⃗ ϑ) = − 1 114,78834 ϑ̂
E(r,
r 2 sin ϑ

---

### Página 181

7.3.

Almacenamiento de Energía en un condensador

Los condensadores se suelen utilizar para el almacenamiento de energía eléctrica. La cantidad
de energía almacenada se puede pensar como el trabajo necesario para cargar al condensador,
así, durante el proceso de carga, una fuente de voltaje realiza el trabajo para mover cargas
desde una placa a la otra.

Imaginemos que el condensador está inicialmente descargado. En cada placa del condensador
hay muchas cargas negativas y positivas, pero estan en equilibrio, por lo que la carga total en
ambas es cero, y por consiguiente no existe ningún campo eléctrico entre ellas.
Comencemos extrayendo una carga positiva +dq de la placa inferior, llevándola hasta la superior. Al hacer esto, la placa de abajo queda con carga neta −dq. Se repite este proceso una
y otra vez, de esta manera cargamos el condensador y creamos un campo eléctrico donde no
había inicialmente.
Supongamos que la cantidad de carga en la placa superior en un instante dado es +q, y la
diferencia de potencial correspondiente es ∆V = q/C. Para traer otro elemento de carga +dq
a la placa superior, el trabajo necesario será dU = ∆V dq (Recordar la interpretación física
del potencial!). Si al final del proceso la carga en cada placa es de Q (en módulo), entonces el
trabajo realizado (energía entregada al sistema) durante el proceso es
U=

ˆ Q
O

dU =

ˆ Q

dq∆V =

ˆ Q

dq

q
1 Q2
=
C
2C

Esto es igual a la energía potencial eléctrica almacenada en un condensador
1 Q2
U=
= Q∆V = C∆V 2
2C

7.4.

Fuerzas entre conductores cargados

Pensemos ahora en una aplicación directa de esta idea de energía electrostática. ¿Cuál será la
fuerza entre las placas de un condensador cargado? Evidentemente debe existir una fuerza, ya
que ambas placas están cargadas con cargas de signo opuesto. Esta fuerza es fácil de obtener
usando el resultado para la energía electrostática de un condensador, usando el principio de
trabajo virtual.
Usemos este método para determinar la fuerza entre las placas de un condensador de placas
paralelas. Si imaginamos que el espacio entre las placas es incrementado una pequeña cantidad,
digamos ∆z, entonces el trabajo mecánico realizado para moverlas será
W = F ∆z

---

### Página 182

donde F es la fuerza entre las placas. Este trabajo debe ser igual al cambio en la energía
electrostática del condensador. Notando que
U=

1 Q2
2C

El cambio en la energía ( si la carga permanece constante) es
∆U = Q2 ∆( )
C
Luego, se tiene
F ∆z =

Q2
∆( )
C

Esto se puede reescribir como
F ∆z = −

Q2
∆C
2C 2

Esta fuerza, por supuesto, resulta de la atracción de las cargas en las placas, pero vemos que
no nos tenemos que preocupar en detalle sobre como están distribuídas, lo único que necesitamos
conocer es la capacidad C. En el límite cuando ∆z → 0
Q2 dC
F =− 2
=−
2C dz
En general

!

'
(&
&
⃗
⃗
F = − ∇U &

dU
dz

"&
&
&

Q=cte

Q=cte

Notar que para éste cálculo hemos asumido que la carga en el condensador permanece
constante (es decir el condensador se encuentra aislado y no está eléctricamente conectado a
otros objetos, de forma que la carga total no cambia). Supongamos que en vez de eso hubieramos
imaginado que el condensador es mantenido a una diferencia de potencial constante y utilizamos
el desplazamiento virtual. Entonces habríamos tenido
U = CV 2
y entonces
F ∆z = V 2 ∆C
que en el límite equivale a
1 dC
F = V2
=
dz
En general

!

dU
dt

'
(&
&
⃗
⃗
F = ∇U &

"&
&
&

V =cte

V =cte

---

### Página 183

7.5.

Condensadores en circuitos eléctricos

Un condensador se puede cargar al conectar sus terminales a una batería, que mantiene una
diferencia de potencial ∆V entre sus placas.

La conexión resulta de compartir cargas entre los terminales y las placas. Por ejemplo, si la
placa se conecta al terminal positivo, adquirirá carga positiva. Esto produce una reducción
momentánea de carga en los terminales, y por lo tanto decrece el potencial entre éstos. Luego,
reacciones químicas dentro de la batería transfieren más carga desde un terminal al otro para
compensar la pérdida y mantener el voltaje en su nivel inicial. La batería se puede pensar
entonces como una bomba de carga que trae carga Q de una placa a la otra

7.5.1.

Conexión en paralelo

Si tenemos dos condensadores, de capacidad C1 y C2 y con cargas Q1 y Q2 y se conectan
en paralelo, como en la figura

Las placas izquierdas de cada condensador son conectadas al terminal positivo de la batería y
están al mismo potencial que la terminal positiva. De forma similar, las placas derechas están
conectadas al terminal negativo y poseen el mismo potencial de éste. La diferencia de potencial
entre las placas de ambos condensadores es la misma, luego
C1 =

Q1
| ∆V |

Q2
| ∆V |
Estos condensadores se pueden ver como un condensador equivalente de capacidad equivalente
Ceq , con una carga Q administrada por la batería. Debe tenerse que
C2 =

de forma que

Q = Q1 + Q2 = C1 | ∆V | +C2 | ∆V |= (C1 + C2 ) | ∆V |
Ceq =

Q
= C1 + C2
| ∆V |

---

### Página 184

Luego, condensadores conectados en paralelo suman su capacidad, en general
Ceq = C1 + C2 + C3 + ... + CN =

N
)

Ci

i=1

7.5.2.

Conexión en serie

Supongamos que tenemos dos condensadores inicialmente descargados C1 y C2 conectados
en serie. Una diferencia de potencial | ∆V | se aplica entre ambos condensadores. La placa
izquierda del condensador 1 está conectada al terminal positivo y se carga positivamente con
+Q, mientras que la placa derecha del condensador 2 se conecta al terminal negativo y se
carga negativamente con −Q. ¿Qué sucede con las placas interiores? Ellas estaban inicialmente
descargadas, ahora ambas placas exteriores tienen cargas iguales pero opuestas. De esta forma
la placa derecha del condensador 1 adquirirá carga −Q y la placa izquierda del condensador 2
+Q

Las diferencias de potencial en los condensadores son
| ∆V1 |=

Q
C1

Q
C2
respectivamente. Vemos que la diferencia de potencial ∆V es simplemente la suma de las
diferencias individuales en cada condensador
| ∆V2 |=

| ∆V |=| ∆V1 | + | ∆V2 |
Estos dos condensadores se pueden reemplazar por un único condensador equivalente
Ceq =
Luego

Q
| ∆V |

Q
Q
Q
=
+
Ceq
C1 C2
y la capacidad equivalente para dos condensadores en serie está dada por
=
+
Ceq
C1 C2
En general
N
)
=
+
+ ... +
=
Ceq
C1 C2
CN
Ci
i=1

---

### Página 185

Problema
Considere la configuración de la figura. Encuentre la capacidad equivalente asumiendo que
todos los condensadores tienen la misma capacidad C

#### Solución
Para los condensadores conectados en serie, la capacidad equivalente esta dada por
N
)
=
+
+ ... +
=
Ceq
C1 C2
Cn
Ci
i=1

Por otro lado, para los condensadores conectados en paralelo, la capacidad equivalente es
Ceq = C1 + C2 + ... + CN =

N
)

Ci

i=1

Con esto, se obtiene el siguiente circuito equivalente

Notar que ahora tenemos 3 condensadores en paralelo. La capacidad equivalente es
Ceq = C(1 +

1 1
+ )= C
2 3

---

### Página 186

Problema
Se tiene un condensador plano con capacidad C1 y un condensador esférico con capacidad C2 .
El primero tiene cargas eléctricas q1 y −q1 y el segundo tiene cargas eléctricas q2 y −q2 . Luego
se conectan ambos condensadores como lo muestra la figura

a) Obtenga las nuevas cargas q1′ , −q1′ , q2′ , −q2′ una vez obtenido el equilibrio eléctrico
b) ¿Cuánto vale la pérdida de energía potencial eléctrica?
c) Según su sentido físico ¿dónde se pierde dicha energía?
d) Se coloca un dipolo eléctrico p⃗ entre las dos esferas del condensador eléctrico. ¿Qué sucede
con él?
#### Solución
a) Por conservación de la carga eléctrica, al conectar ambos condensadores, la carga total sólo
debe distribuírse, luego
q1 + q2 = q1′ + q2′
Al producirse el equilibrio eléctrico, los conductores unidos quedan a un mismo potencial,
digamos V , luego la diferencia de potencial entre sus terminales es común para ambos condensadores (están conectados en paralelo), esto es
q1′ = C1 V
q2′ = C2 V
Luego

q1′
C1
=
′
q2
C2

Con esto
q1′ =

C1 (q1 + q2 )
C1 + C2

q2′ =

C2 (q1 + q2 )
C1 + C2

Ui =

1 q12
1 q22
+
2 C1 2 C2

b) La energía inicial está dada por

Y la energía final por

---

### Página 187

Uf =

1 q1′2 1 q2′2
+
2 C1 2 C2

La diferencia de energía es
!
"
1 q12
q22
q1′2
q2′2
Ui − Uf =
+
−
−
2 C1 C2 C1 C2
!
"
1 q12
q22
C1 (q1 + q2 )2 C2 (q1 + q2 )2
+
−
−
Ui − Uf =
2 C1 C2
(C1 + C2 )2
(C1 + C2 )2
!
"
1 q12
q22
(q1 + q2 )2
+
−
Ui − Uf =
2 C1 C2
C1 + C2

Ui − Uf =

1 (q1 C2 − q2 C1 )2
2 C1 C2 (C1 + C2 )

Esta es la pérdida de energía
c) La pérdida de energía se produce debido a que al conectar ambos condensadores, se produce una redistribución de carga en ellos (y entonces en un intervalo de tiempo breve circula
una corriente eléctrica en los conductores). La energía que se pierde corresponde a la energía
disipada en forma de calor en los conductores
d) El dipolo gira para orientarse en el sentido del campo eléctrico entre ambas cáscaras
esféricas. Además, como el campo no es uniforme en esta región, el dipolo se desplaza hacia
donde el campo eléctrico es más intenso, es decir, hacia la cáscara negativa

---

### Página 188

Problema
Hay dos condensadores con capacidades C1 y C2 conectados a una batería de potencial Vo . A
continuación se desconectan de la batería y se unen como en la figura de abajo

Calcular la nueva diferencia de potencial entre las placas en función de C1 , C2 y Vo
#### Solución
Se tiene que inicialmente C1 y C2 están conectados en serie, luego su capacidad equivalente es
+
=
Ceq1
C1 C2
Con esto

C1 C2
C1 + C2
Si Q1 es la carga almacenada por el sistema (igual en cada condensador), entonces
Ceq1 =

Ceq1 =
Q1 = Ceq1 Vo =

Q1
Vo
C1 C2
Vo
C1 + C2

Ahora, los condensadores se conectan en paralelo, por lo que en esta situación la capacidad
equivalente es
2Q1
V
Ojo! El factor 2 se debe a que inicialmente la carga total es 2Q1 (en cada condensador
inicialmente se almacena carga Q1 ). V es la nueva diferencia de potencial en los condensadores.
Ademas se tiene que
Ceq2 = C1 + C2
Ceq2 =

Así
C1 + C2 = 2

!

C1 C2
C1 + C2

"

Vo

V

---

### Página 189

de aquí obtenemos que
V =2
Finalmente

!

C1 C2
C1 + C2

V =2

"!
Vo

C1 + C2

C1 C2
Vo
(C1 + C2 )2

"

---

### Página 190

Problema
Se tiene un circuito como el que se muestra en la figura.

a) Encontrar la carga de cada condensador cuando se cierra el interruptor S1.
b) Cuando se cierra también el interruptor S2
#### Solución
a) Cuando sólo se cierra el interruptor 1, se tiene

En este caso, C1 y C3 están en serie, asi como también C2 y C4 .
La capacidad equivalente entre C1 y C3 está dada por
=
+
= 1 + µ = (µF )−1
Ceq1
C1 C3
Con lo que

Ceq1 = µF
Del mismo modo, para la capacidad equivalente entre C2 y C4
1 1
=
+
= + (µF )− 1 = (µF )−1
Ceq2
C2 C4
2 4
Así
Ceq2 = µF
Por último, Ceq1 y Ceq2 están en paralelo, por lo que la capacidad total será
Ceq = Ceq1 + Ceq2 =

3 4
+ = µF
4 3

---

### Página 191

Con esto podemos determinar la carga total suministrada por la fuente, dada por
µF = 25µC
Ahora, sea Qi la carga acumulada por el condensador i. Se tiene que Q1 = Q3 , Q2 = Q4 , ya
que se encuentran en serie. Sea Vi la diferencia de potencial entre los terminales del condensador
i. Así
Q = ∆V C = 12

Q1 = 1µV1
Q2 = 2µV2
Q3 = 3µV3 = Q1
Q4 = 4µV4 = Q2

Además, los voltajes están relacionados según
12 = V1 + V3 = V2 + V4
Resolviendo este sistema, se tiene
Q1 = V1 , Q2 = 2V2 , Q1 = 36 − 3V1 , Q2 = 48 − 4V2
Así,
V1 = 36 − 3V1 , 2V2 = 48 − 4V2
De donde se obtiene finalmente
V1 = 9V, V2 = 8V, V3 = 3V, V4 = 4V
Por último
Q1 = 9µC
,Q2 = 16µC. Q3 = 9µC, Q4 = 16µC
Se comprueba que Q1 + Q2 = Q3 + Q4 = 25µC = Q
b) Ahora se tiene lo siguiente

---

### Página 192

Aquí, se tiene a los condensadores C1 y C2 en paralelo, lo mismo sucede con C3 y C4
Ceq1 = C1 + C2 = 3µF
Ceq2 = C3 + C4 = 7µF

Y estos dos se encuentran en serie, por lo que
1 1
= + (µF )− 1 = (µF )− 1
Ceq
3 7
Así
Ceq =

µF

Y la carga suministrada por la fuente será
Q=

21 · 12
V =
=
= 25, 2µC

Además, se tiene V1 = V2 , V3 = V4 , ya que se encuentran en paralelo. Así
V1 =

1µ
2µ
= V2 =
Q1
Q2

V3 =

3µ
4µ
= V4 =
Q3
Q4

Con esto
2Q1 = Q2
4Q3 = 3Q4
También debe tenerse que
Q1 + Q2 = Q3 + Q4 = 25, 2µC
Así
2Q1 = Q2 = 25, 2 − Q1 → Q1 = 8, 4µC
Q3 = 25, 2 − Q4 = 25, 2 − Q3 → Q3 = 10, 8µC
Q4 = Q3 = 14, 4µC

---

### Página 193

Problema
Considere el circuito de la figura

Primero se carga C1 cerrando el interruptor S1 . Después este interruptor es abierto, y el condensador cargado se conecta al otro condensador descargado cerrando al interruptor S2 . Calcule
la carga final en cada uno de los condensadores
#### Solución
Al cerrar el interruptor S1 , se conecta el condensador C1 a los terminales de la fuente de voltaje,
luego éste acumula una carga igual a
Q = CV = 6µ20 = 120µ(C)
Ahora, se abre el interruptor S1 y se cierra el interruptor S2 , es decir, se desconecta la fuente
de voltaje y se conectan ambos condensadores en paralelo. Básicamente lo que ocurre aquí es
una redistribución de la carga almacenada.
Sea Q1 la carga final en el condensador 1 , y Q2 la carga final en el condensador 2. Se sabe
que la carga total debe conservarse, es decir
Q = Q1 + Q2 = 120µ(C)
Y en cada condensador se tiene
Q1 = 6µV1
Q2 = 3µV2
Como están en paralelo, V1 = V2 , así
Q2
Q1
Q1
=2
=
→
6µ
3µ
Q2
De donde se obtiene, Q1 = 80µ (C), y Q2 = 40µ

---

### Página 194

Problema
Dos placas conductoras cuadradas de lado a se disponen con sus caras paralelas y muy próximas
entre sí. La distancia entre las placas es x, como se indica en la figura. Calcule la fuerza sobre
la placa B en las direcciones x y z cuando la diferencia de potencial entre las placas es Vo

#### Solución
La energía almacenada en el condensador es
U = CVo2
donde la capacidad está dada por
C(x, z) =

ϵo A
ϵo a(a − z)
=
x
x

De esta forma
⃗ = dU î + dU k̂
F⃗ = ∇U
dx
dz
!
"
ϵ
ϵ
(a
−
z)a
a
o
î +
k̂
F⃗ = − Vo
x2
x

1 ϵo (a − z)a
1 ϵo a
F⃗ = − Vo2
î − Vo2
k̂
x
x

---

### Página 195

#### Capítulo 8
Ecuaciones de Poisson y Laplace
Hemos concluído nuestra revisión de la electrostática demostrando que la teoría es completa.
En efecto, hemos visto que la conducta de un campo electrostático queda totalmente descrita por
dos ecuaciones diferenciales de primer orden, las cuales son consecuencia de la ley de Coulomb
y el principio de superposición
⃗ x) = ρ(⃗x)
⃗ · E(⃗
∇
ϵ0
⃗ × E(⃗
⃗ x) = ⃗0
∇
Ahora comenzaremos un estudio sobre la teoría del potencial. Esta nos brindará las herramientas matemáticas necesarias para resolver los problemas electrostáticos que se nos presentan en la práctica. Notar que la teoría electrostática ya está competa (es una teoría de
estructura muy simple, en efecto): solamente nos falta ampliar nuestra capacidad de aplicarla

8.1.

Ecuaciones de Poisson y Laplace

La segunda ecuación
es equivalente a

⃗ × E(⃗
⃗ x) = 0
∇
⃗ x) = −∇φ(⃗
⃗ x)
E(⃗

Combinada con la primera, se obtiene una ecuación diferencial de segundo orden
⃗ 2 φ(⃗x) = − ρ(⃗x)
∇
ϵ0
Esta es la ecuación de Poisson. En regiones libres de cargas tenemos
⃗ 2 φ(⃗x) = 0
∇
la ecuación de Laplace.

---

### Página 196

Interpretación del teorema fundamental
⃗2
∇

= −4πδ(⃗x − ⃗x′ )
| ⃗x − ⃗x′ |

Esta es la ecuación de Poisson para una carga q = 4πϵ0 puntual localizada en el punto ⃗x′ .
(Ecuación singular de Poisson). Hemos establecido que
⃗ x) = −∇φ(⃗
⃗ x)
E(⃗
a partir de la ley de Coulomb
⃗ x) =
E(⃗

4πϵ0

˚

d3 x′ ρ(⃗x′ )

R3

⃗x − ⃗x′
| ⃗x − ⃗x′ |3

utilizando el siguiente argumento
⃗x − ⃗x′
⃗
= −∇
′
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |
⃗ x) = −∇
⃗ 1
E(⃗
4πϵ0

˚

d3 x′

R3

Ahora lo vamos a demostrar directamente
Teorema

φ(x) =
4πϵ0

˚

d3 x′

R3

ρ(⃗x′ )
| ⃗x − ⃗x′ |

ρ(⃗x′ )
| ⃗x − ⃗x′ |

es la solución de la ecuación de Poisson con condiciones de contorno adecuadas en el infinito,
es decir
⃗ 2 φ(⃗x) = − ρ(⃗x′ )
∇
ϵ0
C.C.S(∞)

*

⇔ φ(x) =
4πϵ0

˚

d3 x′

R3

ρ(⃗x′ )
| ⃗x − ⃗x′ |

Demostración
1) Sea
φ(x) =
4πϵ0
Luego

˚

d3 x′

R3

ρ(⃗x′ )
| ⃗x − ⃗x′ |

ρ(⃗x′ )
| ⃗x − ⃗x′ |
R3
˚
˚
4π
3 ′
′ ⃗2
⃗
∇ φ(⃗x) =
=−
d x ρ(⃗x )∇
d3 x′ ρ(⃗x′ )δ(⃗x − ⃗x′ )
4πϵ0
| ⃗x − ⃗x′ |
4πϵ0
R3
R3
⃗ 2 φ(⃗x) = ∇
⃗2 1
∇
4πϵ0

˚

d3 x′

⃗ 2 φ(⃗x) = − ρ(⃗x)
∇
ϵ0

---

### Página 197

2) Sea
⃗ 2 φ(⃗x) = − ρ(⃗x)
∇
ϵ0
⃗ ′2 φ(⃗x′ )
∇
ρ(⃗x′ )
=−
⃗x − ⃗x′
ϵ0 | ⃗x − ⃗x′ |

con esto

⃗ ′2 φ(⃗x′ )

=−
dx
′
| ⃗x − ⃗x |
ϵ0
R3

˚
pero

3 ′∇

d3 x′

R3

ρ(⃗x′ )
| ⃗x − ⃗x′ |

⃗′·∇
⃗ ′ φ(⃗x′ )
∇
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
R3
˚
˚
,
+
⃗ ′ φ(⃗x′ )
∇
3 ′ ⃗′
′
′
3 ′⃗ ′
⃗
x
∇
·
d x ∇ φ(⃗x ) · ∇
+
d
=−
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
R3
R3
˚

=

˚

⃗′·∇
⃗′
d x φ(⃗x )∇
3 ′

R3

=

˚

R3

′

⃗ ′2
d x φ(⃗x )∇
3 ′

′

⃗ ′2 φ(⃗x′ )

˚

3 ′∇

dx

−
| ⃗x − ⃗x′ |

˚

=

˚

d3 x′

⃗′
d x ∇ · φ(⃗x′ )∇
3 ′⃗ ′

R3

. ˆˆ
′
⃗′
✞☎
⃗ x′ ) · ∇ φ(⃗x )
+
d
S(⃗
✝
✆
| ⃗x − ⃗x′
| ⃗x − ⃗x′ |
S(∞)

ˆˆ
ˆˆ
⃗ ′
⃗x − ⃗x′
✞☎
✞☎
′
′
⃗
⃗ x′ ) · E(⃗x )
+
φ(⃗
x
d
S(⃗
x
)
·
)
−
d
S(⃗
✝
✆
✝
✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
S(∞)
S(∞)

Ahora supondremos que las condiciones de borde son apropiadas (y que entonces las integrales de superficie son nulas)
˚
˚
x′ )
3 ′ ρ(⃗
−
= −4π
dx
d3 x′ φ(⃗x′ )δ(⃗x − ⃗x′ ) = −4πφ(⃗x)
′
ϵ0
| ⃗x − ⃗x |
R3
R3
˚
ρ(⃗x′ )
d3 x′
φ(⃗x) =
4πϵ0
| ⃗x − ⃗x′ |
R3

8.1.1.

Acerca de las condiciones en el infinito

Veremos que
ˆˆ

✞☎

lím φ(⃗x) = 0 ⇒ ✝ ✆

|⃗
x|→∞

S(∞)

⃗ x′ ) ·
dS(⃗

ˆˆ
✞☎
⃗
lím | ⃗x || ∇φ(⃗x) |= 0 ⇒ ✝ ✆

|⃗
x|→∞

⃗x − ⃗x′
φ(⃗x′ ) = 0
| ⃗x − ⃗x′ |3

S(∞)

⃗ x′ ) ·
dS(⃗

⃗ x′ )
E(⃗
| ⃗x − ⃗x′ |

la segunda de ellas ya se discutió en el teorema de completitud de Helmholtz. Lo que se hace
es escoger como superficie de integración una esfera centrada en ⃗x y de radio a =| ⃗x − ⃗x′ |→ ∞

ˆˆ

✞☎
✝✆

S(∞)

⃗ x′ ) ·
dS(⃗

ˆˆ
˛ 4π
⃗x − ⃗x′
✞☎
′
φ(⃗x ) = lím ✝ ✆ dΩ(n̂)φ(⃗x + an̂) =
dΩ(n̂) lím φ(⃗x′ )
a→∞
a→∞
| ⃗x − ⃗x′ |3
S(a)

---

### Página 198

luego debe tenerse que
lím

|⃗
x−⃗
x′ |→∞

φ(⃗x′ ) = 0 ⇒ lím φ(⃗x) = 0
|⃗
x|→∞

del mismo modo
ˆˆ
⃗ x′ )
E(⃗
✞☎
′
⃗
⃗ x + an̂)
= lím ✝ ✆ dΩ(n̂)an̂ · E(⃗
dS(⃗x ) ·
′
a→∞
|
⃗
x
−
⃗
x
|
S(∞)
S(a)
˛ 4π
⃗ x + an̂)
dΩ(n̂) lím an̂ · E(⃗
=

ˆˆ

✞☎
✝✆

a→∞

luego basta tener

⃗ x) = 0
lím ⃗x · E(⃗

|⃗
x|→∞

y

⃗ x) ≤ lím | ⃗x | · | E(⃗
⃗ x) |
lím ⃗x · E(⃗

|⃗
x|→∞

8.1.2.

|⃗
x|→∞

Corolario: Condición de validez para ρ(⃗x)

De la condición necesaria para el potencial
lím φ(⃗x) = 0

|⃗
x|→∞

|⃗
x|→∞ | ⃗
|⃗
x|→∞
x − ⃗x′ |
R3
˚
˚
3 ′
′
=
= lím
d x ρ(⃗x ) lím
d3 x′ ρ(⃗x′ ) = 0
|⃗
x|→∞ | ⃗
x | |⃗x|→∞ | ⃗x |
R3
R3
lím

si

ρ(⃗x′ )
=
dx
| ⃗x − ⃗x′ |
R3

˚

3 ′

−∞ <

¨

R3

˚

d3 x′ ρ(⃗x′ ) lím

d3 x′ ρ(⃗x′ ) < ∞

Basta que la carga total de las fuentes sea finita (razonable!)
Luego, como corolario
*
˚
⃗ 2 φ(⃗x) = − ρ(⃗x′ )
x′ )
∇
3 ′ ρ(⃗
ϵ
˝
d
x
⇒
φ(x)
=
4πϵ0
| ⃗x − ⃗x′ |
d3 x′ | ρ(⃗x′ ) |< ∞
R3
R3
Pero en la práctica, éste no es el problema de contorno típico de la electrostática
Nota sobre el potencial en el infinito
Es bien sabido que a la función potencial siempre es posible sumarle una constante arbitraria
finita, ya que, obviamente, semejante adición no modifica en nada el campo electrostático que
ese potencial determina. Sumarle una constante al potencial equivale a cambiar arbitrariamente
su valor en el infinito. Sin embargo, pareciera concluirse de nuestro análisis previo que el valor
del potencial en el infinito está perfectamente determinado por la naturaleza de las fuentes

---

### Página 199

cargadas. Esta situación, aparentemente paradojal, merece ser estudiada con cierto cuidado.
Sea
*
⃗ 2 φ(⃗x) = − ρ(⃗x′ )
∇
ϵ0
˝
d3 x′ | ρ(⃗x′ ) |< ∞
R3
Luego

˚
ρ(⃗x′ )
φ(⃗x) =
d3 x′
4πϵ0
| ⃗x − ⃗x′ |
R3
lím ρ(⃗x) = 0
|⃗
x|→∞

⃗ x) |= 0
lím | ⃗x || ∇φ(⃗

|⃗
x|→∞

Transformemos este potencial
φ(⃗x) → ψ(⃗x) = φ(⃗x) + ψ∞
Se tiene ahora
a)
⃗ 2 ψ(⃗x) = ∇
⃗ 2 [φ(⃗x) + ψ∞ ] = ∇
⃗ 2 φ(⃗x)
∇
⃗ 2 ψ(⃗x) = − ρ(⃗x)
∇
ϵ0
b)
ψ(⃗x) =
4πϵ0

˚

d3 x′

R3

ρ(⃗x′ )
+ ψ∞
| ⃗x − ⃗x′ |

c) lím|⃗x|→∞ ψ(⃗x) = lím|⃗x|→∞ (φ(⃗x) + ψ∞ ) = lím|⃗x|→∞ φ(⃗x) + ψ∞
lím ψ(⃗x) = ψ∞

|⃗
x|→∞

⃗ [φ(⃗x) + ψ∞ ] = ∇φ(⃗
⃗ x)
d) ψ(⃗x) = ∇
⃗ x) |= 0
lím | ⃗x || ∇ψ(⃗

|⃗
x|→∞

Veamos ahora si todo ésto es consistente
˚

R3

−4π

˚

R3

⃗ ′2 ψ(⃗x′ )

3 ′∇

dx

| ⃗x − ⃗x′ |
ˆˆ

✞☎
d x ψ(⃗x )δ(⃗x − ⃗x ) + ✝ ✆
3 ′

′

′

= −4π

S(∞)

˚

d3 x′

R3

′

′

ρ(⃗x′ )
| ⃗x − ⃗x′ |
ˆˆ

✞☎

dΩ(⃗x , ⃗x)ψ(⃗x ) + ✝ ✆

S(∞)

= −4πψ(⃗x) + 4πψ∞ + 0

luego hay consistencia y no hay paradoja alguna!

⃗ x′ ) ·
dS(⃗

⃗ ′ ψ(⃗x′ )
∇
| ⃗x − ⃗x′ |

---

### Página 200

8.2.

Ecuación Integral de Poisson: Teoremas de Green

A) Problemas simples de la electrostática
Los problemas formalmente más simples de la electrostática consisten en calcular φ(⃗x) para
todos los puntos del espacio, habiéndose dado la distribución de las fuentes eléctricas ρ(⃗x) (por
lo general, localizadas dentro de una región V ), sin condiciones de contorno prescritas para
⃗ x) en el infinito
φ(⃗x) o E(⃗

la solución de estos problemas simples es, formalmente, inmediata
˚
ρ(⃗x′ )
φ(⃗x) =
d3 x′
4πϵ0
| ⃗x − ⃗x′ |
V
⃗ x) = −∇φ(⃗
⃗ x)
E(⃗

B) Problemas de contorno
Pero, por lo general, los problemas prácticos de la electrostática se refieren a regiones (finitas
o infinitas) que solamente abarcan una porción del espacio, con o sin cargas en su interior, y
con condiciones de contorno presecritas en las superficies que las limitan. (Por ejemplo, esta
superficie de contorno puede representar un conductor a un potencial fijo). La solución formal
de éstos problemas de contorno no es tan sencilla. Para manejar los problemas de contorno
necesitaremos nuevas herramientas matemáticas que procedemos a construír

8.3.

Teoremas de Green

A partir del teorema de la divergencia
˚
ˆˆ
✞☎
3 ′⃗
⃗
d x ∇ · A = ✝✆
V

S(V )

⃗ ·A
⃗
dS

y utilizamos un campo vectorial de la forma
⃗ = φ∇ψ
⃗
A
con φ, ψ, dos campos escalares. Recordar que
'
(
⃗ ·A
⃗=∇
⃗ · φ∇ψ
⃗
⃗ · ∇ψ
⃗ + φ∇
⃗ 2ψ
∇
= ∇φ

---

### Página 201

˚

V

'

⃗2

(

ˆˆ

☎
⃗ · ∇ψ
⃗ + φ∇ ψ = ✞
d x ∇φ
✝✆
3 ′

S(V )

Se obtiene la Primera Identidad de Green
˚
( ˆˆ
'
☎
3 ′ ⃗
⃗ + φ∇
⃗ ψ = ✞
d x ∇φ · ∇ψ
✝✆
V

⃗ · ∇ψφ
⃗
dS

dSφ

S(V )

∂ψ
∂n

donde

⃗ = ∂ψ
n̂ · ∇ψ
∂n
es la derivada direccional de ψ en la dirección normal a S(V )
⃗ = ψ ∇φ,
⃗ y obtenemos el siguiente par de identidades
Ahora, también es posible escoger A
de Green
˚
( ˆˆ
'
∂ψ
✞☎
3 ′ ⃗
⃗
⃗
d x ∇φ · ∇ψ + φ∇ ψ = ✝ ✆ dSφ
∂n
S(V )
V
ˆ
ˆ
˚
(
'
∂φ
☎
⃗ · ∇φ
⃗ + φ∇
⃗ 2φ = ✞
d3 x′ ∇ψ
✝ ✆ dSψ
∂n
V
S(V )
Restándolas, obtenemos el Teorema de Green
˚
+
, ˆˆ
✞☎
⃗
⃗
d x φ∇ ψ − ψ ∇ φ = ✝ ✆

/
*
∂ψ
∂φ
ds φ
−ψ
∂n
∂n
S(V )

V

8.3.1.

Ecuación Integral de Poisson

Usaremos el teorema de Green para transformar la ecuación de Poisson en una ecuación
integral en la región de interés. Elijamos
ψ(⃗x, ⃗x′ ) =
Sea

| ⃗x − ⃗x′ |
′

⃗ ′2 φ(⃗x′ ) = − ρ(⃗x )
∇
ϵ0
⃗ ′2 ψ(⃗x, ⃗x′ ) = −4πδ(⃗x − ⃗x′ )
∇

Luego, integrando sobre la región de interés V
˚

V

/
˚
,
+
′ ⃗ ′2
′
′ ⃗ ′2
′
3 ′
d x φ(⃗x )∇ ψ(⃗x, ⃗x ) − ψ(⃗x, ⃗x )∇ φ(⃗x ) = −4π
d x φ(⃗x′ )δ(⃗x − ⃗x′ ) −
3 ′

V

/
*
x, ⃗x′ )
x′ )
′ ∂ψ(⃗
′ ∂φ(⃗
dS(⃗x ) φ(⃗x )
− ψ(⃗x, ⃗x )
=
∂n′
∂n′
S(V )
ˆˆ
∂φ(⃗
x′ )
✞☎
′
′ ∂
∂n′
= ✝ ✆ dS(⃗x ) φ(⃗x ) ′
−
∂n | ⃗x − ⃗x′ | | ⃗x − ⃗x′ |
S(V )
ˆˆ

✞☎
✝✆

′

ρ(⃗x′ )
4πϵ0 | ⃗x − ⃗x′ |

*

---

### Página 202

Se obtiene la ecuación integral de Poisson

φ(⃗x)

d x δ(⃗x−⃗x ) =
4πϵ0
V

˚

3 ′

′

0 ∂φ(⃗x′ )
ˆˆ
1 ✞☎
ρ(⃗x′ )
∂
′
′
′
∂n
+
− φ(⃗x ) ′
dx
x)
✝ ✆ dS(⃗
| ⃗x − ⃗x′ | 4π S(V )
| ⃗x − ⃗x′ |
∂n | ⃗x − ⃗x′ |
V

˚

3 ′

Consideremos ⃗x ∈ V
⃗x ∈ V →
dS(⃗x′ )

˚

V

d3 x′ δ(⃗x − ⃗x′ ) = 1

′
∂
′
′
⃗′
⃗ x′ ) · ⃗x − ⃗x
)n̂(⃗
x
)
·
∇
=
dS(⃗
x
=
d
S(⃗
∂n′ | ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |3

dS(⃗x′ )

′
∂
⃗ x′ ) · ⃗x − ⃗x
=
−d
S(⃗
∂n′ | ⃗x − ⃗x′ |
| ⃗x′ − ⃗x |3

dS(⃗x′ )

∂φ(⃗x′ )
⃗ x′ ) · ∇
⃗ ′ φ(⃗x′ )
= dS(⃗
∂n′

y entonces la ecuación interior es
φ(⃗x) =

ˆˆ
ˆˆ
′
⃗ x′ ) · ∇
⃗ ′ φ(⃗x′ )
1 ✞ ☎ dS(⃗
1 ✞☎
ρ(⃗x′ )
⃗ x′ ) · ⃗x − ⃗x φ(⃗x′ )
dx
d
S(⃗
+
+
✝
✆
✝
✆
| ⃗x − ⃗x′ | 4π S(V )
| ⃗x − ⃗x′ |
4π S(V )
| ⃗x′ − ⃗x |3
V

˚

3 ′

Primera Observación
Si V = R3 , S(V ) → S(∞)
ˆˆ

✞☎
✝✆

S(V )

⃗ x′ ) ·
dS(⃗

⃗x′ − ⃗x
φ(⃗x′ ) →
| ⃗x′ − ⃗x |3

ˆ 4π

dΩ(x̂) lím
φ(⃗x′ )
′
|⃗
x |→∞

y también
ˆˆ
⃗ x′ ) · ∇
⃗ ′ φ(⃗x′ )
⃗ ′ x′ ) |
dS(⃗
✞☎
′ | ∇ φ(⃗
|
|≤
dS(⃗
x
)
✝✆
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
S(V )
S(V )
ˆˆ
ˆ 4π
dS(⃗x′ )
✞☎
′
′
′
⃗
⃗ ′ φ(⃗x′ ) |
= ✝✆
| ⃗x − ⃗x || ∇ φ(⃗x ) |→
dΩ(x̂) lím
| ⃗x − ⃗x′ || ∇
′ |2
′ |→∞
|⃗
x
|
⃗
x
−
⃗
x
S(V )
ˆˆ

✞☎
✝✆

Luego
′

ˆˆ

✞☎

lím
φ(⃗x ) = 0 ⇒ ✝ ✆
′

|⃗
x |→∞

S(∞)

⃗ x′ ) ·
dS(⃗

⃗x′ − ⃗x
φ(⃗x′ ) = 0
′
| ⃗x − ⃗x |

⃗ x′ ) · ∇
⃗ ′ φ(⃗x′ )
dS(⃗
| ⃗x − ⃗x′ |
S(∞)

ˆˆ
✞☎
′
′
⃗
lím
| ⃗x || ∇ φ(⃗x ) |= 0 ⇒ ✝ ✆
′
′

|⃗
x |→∞

y entonces
φ(⃗x) =
4πϵ0

ρ(⃗x′ )
dx
| ⃗x − ⃗x′ |
R3

˚

3 ′

---

### Página 203

esto impone sobre ρ las condiciones de consistencia dadas que ya conocemos
˚
d3 x′ | ρ(⃗x′ ) |< ∞
R3

Segunda observación
Si la región de interés V está libre de cargas
⃗x ∈ V : ρ(⃗x) = 0
entonces, se obtiene la ecuación integral de Laplace
0 ∂φ(⃗x′ )
ˆˆ
1 ✞☎
∂
′
′
′
∂n
φ(⃗x) =
x)
− φ(⃗x ) ′
✝ ✆ dS(⃗
4π S(V )
| ⃗x − ⃗x′ |
∂n | ⃗x − ⃗x′ |

8.4.

Condiciones de Contorno: Unicidad de las soluciones

A) Los problemas de contorno en electrostática son de la forma
⃗ 2 φ(⃗x) = −
⃗x ∈ V : ∇

ρ(⃗x)
ϵ0

∂φ
⃗x ∈ S(V ) : Condiciones de contorno para φ o para ∂n

o bien
⃗ 2 φ(⃗x) = 0
⃗x ∈ V : ∇

∂φ
⃗x ∈ S(V ) : Condiciones de contorno para φ o para ∂n

Surge la cuestión sobre cuáles son las condiciones de contorno adecuadas para que dentro
del volumen de interés V la solución sea matemáticamente única, y físicamente razonable.
La experiencia física nos hace esperar que un problema único de potencial se obtiene:
a) Especificando el potencial φ(⃗x) sobre una superficie cerrada S(V ) que limita la región de
interés V (problema de Dirichlet)
⃗x ∈ S(V ) : φ(⃗x) = φD (⃗x)

⃗ x) sobre el contorno cerrado S(V ) de la región de
b) Especificando el campo eléctrico E(⃗
interés V (problema Neumann)
⃗ x) = E
⃗ N (⃗x)
⃗x ∈ S(V ) : E(⃗

En efecto vamos a demostrar que tanto el problema de Dirichlet como el problema de Neumann dan origen a una solución única

---

### Página 204

8.4.1.

Unicidad para problemas de contorno Dirichlet

El problema Poisson Dirichlet tiene la siguiente forma
⃗ 2 φ(⃗x) = − ρ(⃗x)
⃗x ∈ V : ∇
ϵ0
⃗x ∈ S(V ) : φ(⃗x) = φD (⃗x)
Sean φ1 (x) y φ2 (x) dos soluciones de este problema. Se define
ψ(⃗x) = φ2 (⃗x) − φ1 (⃗x)
Evidentemente ψ(⃗x) es solución de la ecuación de Laplace con condiciones de contorno
Dirichlet Homogéneas
⃗ 2 ψ(⃗x) = 0
⃗x ∈ V : ∇

⃗x ∈ S(V ) : ψ(⃗x) = 0

Usemos la primera identidad de Green
˚
+
, ˆˆ
✞☎
⃗
⃗
⃗
d x ∇ψ · ∇ψ + ψ ∇ ψ = ✝ ✆
V

dSψ

S(V )

˚

V

⃗ · ∇ψ
⃗ =
d3 x∇ψ

Pero
˚

V

˚

V

∂ψ
=0
∂n

⃗ |2 = 0
d3 x | ∇ψ

⃗ |≥ 0
| ∇ψ
⃗ |2 = 0 ⇒ ∇ψ(⃗
⃗ x) = ⃗0, ⃗x ∈ V
d3 x | ∇ψ

Luego ψ(⃗x) es constante para ⃗x ∈ V . Pero entonces, como
se tiene

ψ(⃗x) = 0, ⃗x ∈ S(V )
ψ(⃗x) = 0, ⃗x ∈ V

y por lo tanto

Luego, para ⃗x ∈ V

ψ(⃗x) = φ2 (⃗x) − φ1 (⃗x) = 0, ⃗x ∈ V
φ2 (⃗x) = φ1 (⃗x)

Obsérvese el importante resultado

y también

*
⃗ 2 ψ(⃗x) = 0
⃗x ∈ V : ∇
⇒ ψ(⃗x) = 0, ⃗x ∈ V
⃗x ∈ S(V ) : ψ(⃗x) = 0
*
⃗ 2 ψ(⃗x) = 0
∇
⇒ ψ(⃗x) = 0, ∀x
⃗x ∈ S(∞) : ψ(⃗x) = 0

---

### Página 205

8.4.2.

Unicidad para condiciones de contorno de Neumann

El problema Poisson-Neumann tiene la forma
⃗ 2 φ(⃗x) = −
⃗x ∈ V : ∇
⃗x ∈ S(V ) :

ρ(⃗x)
ϵ0

∂φ(⃗x)
= −EN (⃗x)
∂n

El desarrollo es análogo al caso anterior. Sean
φ1 (⃗x), φ2 (⃗x)
dos soluciones del problema Poisson-Neuman en V . Definimos
ψ(⃗x) = φ2 (⃗x) − φ1 (⃗x)
Entonces ψ(⃗x) es solución de la ecuación de Laplace con condiciones de contorno de Neumann Homogéneas
⃗ 2 ψ(⃗x) = 0
⃗x ∈ V : ∇
⃗x ∈ S(V ) :

∂φ(⃗x)
=0
∂n

Ahora
˚

V

ˆˆ
✞☎
⃗
d x | ∇ψ | = ✝ ✆

dSψ

S(V )

∂ψ
=0
∂n

luego
⃗ = ⃗0
∇ψ
y ψ(⃗x) es constante para ⃗x ∈ V . Pero ahora
∂ψ
= 0, ⃗x ∈ S(V )
∂n
Por lo tanto
ψ(⃗x) = C, ⃗x ∈ S(V )
luego
φ2 (⃗x) = φ1 (⃗x) + C, ⃗x ∈ V
Observemos que

⃗ 2 ψ(⃗x) = 0
⃗x ∈ V : ∇
⇒ ψ(⃗x) = C, ⃗x ∈ V
x)
=0
⃗x ∈ S(V ) : ∂ψ(⃗
∂n

La constante aditiva C es arbitraria y carece de importancia física pues no altera al campo
⃗ x)
eléctrico E(⃗

---

### Página 206

8.4.3.

Condiciones de Contorno de Cauchy

Un problema Poisson-Cauchy tendría la siguiente forma
⃗ 2 φ(⃗x) = − ρ(⃗x)
⃗x ∈ V : ∇
ϵ0
/
φ(⃗x) = φC (⃗x)
⃗x ∈ S(V ) ∂φ(⃗x)
= −EC (⃗x)
∂n
Pero este problema lo podemos desglosar
*
⃗ 2φ = − ρ
⃗x ∈ V : ∇
ϵ0
⇒ φ(⃗x) = φD (⃗x), ⃗x ∈ V
⃗x ∈ S : φ = φC
Este problema de Poisson Dirichlet posee solución única!
⃗ 2φ = − ρ
⃗x ∈ V : ∇
ϵ0
⇒ φ(⃗x) = φN (⃗x), ⃗x ∈ V
∂φ
= −EC
⃗x ∈ S : ∂n
Este problema de Poisson Neumann también posee solución única. Los datos de Cauchy son
{φC , EC } sobre S. (Ambas son funciones arbitrarias). Al resolver el problema Poisson Dirichlet
⃗ C , al resolver el problema Poisson
obtenemos una solución φD , haciendo caso omiso del dato E
Neumann obtenemos φN , haciendo caso omiso de φC . Es obvio que, en general, resultará
/ ∂φD (⃗x)
x)
N (⃗
̸= ∂φ∂n
= −EC (⃗x)
∂n
⃗x ∈ S(V ) :
φN (⃗x) ̸= φD (⃗x) = φC (⃗x)
Luego no hay consistencia: no existe, en general, solución de la ecuación de Poisson con
condiciones de contorno de Cauchy sobre una superficie cerrada

8.5.

Funciones de Green: Solución formal a los problemas de contorno

El problema típico en electrostática es resolver un problema de contorno de la forma
⃗ 2 φ(⃗x) = − ρ(⃗x)
⃗x ∈ V : ∇
ϵ0
⃗ 2 φ(⃗x) = 0
⃗x ∈ V : ∇
con condiciones de borde de Dirichlet
⃗x ∈ S(V ) : φ = φD
o de Neumann
⃗x ∈ S(V ) :

∂φ
= −EN
∂n

la solución de este problema es única.
Una carga puntual (positiva) 4πϵ0 ubicada en el punto ⃗x se representa por la densidad de carga
singular
ρ(⃗x′ ) = 4πϵ0 δ(⃗x − ⃗x′ )
y su potencial en el punto ⃗x′ es

---

### Página 207

ψ(⃗x, ⃗x′ ) =

| ⃗x − ⃗x′ |

Obsérvese que el rol de ⃗x y ⃗x′ puede invertirse. Este potencial unitario satisface la ecuación
de Poisson singular
⃗ ′2
= −4πδ(⃗x − ⃗x′ )
∇
′
| ⃗x − ⃗x |
Vamos a generalizar esta idea

Funciones de Green G(⃗x, ⃗x′)

8.6.

En general, son aquellas funciones que satisfacen la ecuación de Poisson singular
⃗ ′2 G(⃗x′ , ⃗x) = −4πδ(⃗x, ⃗x′ ), ⃗x′ ∈ V
∇

Sea L(⃗x′ , ⃗x) una solución de la ecuación de Laplace en el interior de una región V , ⃗x′ ∈ V
⃗ ′2 L(⃗x′ , ⃗x) = 0
∇
entonces podemos considerar
G(⃗x, ⃗x′ ) =

+ L(⃗x, ⃗x′ )
′
| ⃗x − ⃗x |

Esta es una función de Green dentro de la región V . Consideremos la estructura
⃗x′ ∈ V

′

⃗ ′2 φ(⃗x′ ) = − ρ(⃗x )
∇
ϵ0
⃗ ′2 G(⃗x′ , ⃗x) = −4πδ(⃗x − ⃗x′ )
∇
G(⃗x′ , ⃗x) =

| ⃗x′ − ⃗x |

+ L(⃗x′ , ⃗x)

⃗ ′2 L(⃗x, ⃗x′ ) = 0
∇
Entonces, usando la segunda identidad de Green
˚

*
/
∂φ(⃗x′ )
x′ , ⃗x)
′
′ ∂G(⃗
dS(⃗x ) G(⃗x , ⃗x)
− φ(⃗x )
∂n′
∂n′
S(V )

+
, ˆˆ
✞☎
′
′2
′
′ ⃗ 2′
′
⃗
d x G(⃗x , ⃗x)∇ φ(⃗x ) − φ(⃗x )∇ G(⃗x , ⃗x) = ✝ ✆
3 ′

V

′

para ⃗x ∈ V , resulta
*
/
˚
′
′
′
′
d x − G(⃗x , ⃗x)ρ(⃗x ) + 4πφ(⃗x )δ(⃗x − ⃗x) = −
d3 x′ ρ(⃗x′ )G(⃗x′ , ⃗x) + 4πφ(⃗x)
ϵ
ϵ
V
V

˚

3 ′

=

/
*
∂φ(⃗x′ )
x′ , ⃗x)
′
′ ∂G(⃗
dS(⃗x ) G(⃗x , ⃗x)
− φ(⃗x )
∂n′
∂n′
S(V )

ˆˆ

✞☎
✝✆

′

---

### Página 208

o sea, con ⃗x ∈ V en general se tiene
φ(⃗x) =
4πϵ0

ˆˆ
ˆˆ
1 ✞☎
x′ )
1 ✞☎
x′ , ⃗x)
′ ∂φ(⃗
′
′
′ ∂G(⃗
d x ρ(⃗x )G(⃗x , ⃗x)+
dS(⃗
x
)
G(⃗
x
,
⃗
x
)−
dS(⃗
x
)φ(⃗
x
)
✝✆
✝✆
4π S(V )
∂n′
4π S(V )
∂n′
V

˚

3 ′

′

′

Apliquemos este resultado a los problemas de contorno de Dirichlet y de Neumann

8.6.1.

Solución formal del problema Dirichlet

Hay que resolver
/

⃗ 2 φ(⃗x) = − ρ(⃗x)
⃗x ∈ V : ∇
ϵ0
⃗x ∈ S(V ) : φ(⃗x) = φD (⃗x)

Resolvamos entonces
/ ′
⃗ ′2 GD (⃗x′ , ⃗x) = −4πδ(⃗x′ − ⃗x)
⃗x ∈ V : ∇
⃗x ∈ V
′
⃗x ∈ S(V ) : GD (⃗x′ , ⃗x) = 0
o sea, resolvamos el problema
⃗x ∈ V

⃗ ′2 LD (⃗x′ , ⃗x) = 0
⃗x′ ∈ V : ∇
⃗x′ ∈ S(V ) : LD (⃗x′ , ⃗x) = − |⃗x′1−⃗x|

y hacemos
GD (⃗x′ , ⃗x) =

| ⃗x′ − ⃗x |

+ LD (⃗x′ , ⃗x)

GD (⃗x′ , ⃗x) es la función de Green del problema Dirichlet. La solución formal es
˚
ˆˆ
1 ✞☎
∂GD (⃗x′ , ⃗x)
3 ′
′
′
φ(⃗x) =
d x ρ(⃗x )GD (⃗x, ⃗x ) −
x′ )φD (⃗x′ )
✝ ✆ dS(⃗
4πϵ0
4π S(V )
∂n′
V

8.6.2.

Solución formal del problema de Neumann

Hay que resolver

⃗ 2 φ(⃗x) = − ρ(⃗x)
⃗x ∈ V : ∇
ϵ0
x)
=
−E
x)
⃗x ∈ S(V ) : ∂φ(⃗
N (⃗
∂n

Resultaría ventajoso resolver
⃗ ′2 GN (⃗x′ , ⃗x) = −4πδ(⃗x′ − ⃗x)
⃗x′ ∈ V : ∇
⃗x ∈ V
′
⃗x′ ∈ S(V ) : ∂GN∂n(⃗x′ ,⃗x) = 0
pero ésto es, en general, imposible. En efecto, el teorema de Gauss nos da
˚
˚
3 ′ ⃗ ′2
′
⃗ ′ GN (⃗x′ , ⃗x)
⃗′·∇
d x ∇ GN (⃗x , ⃗x) =
d3 x′ ∇
V

V

---

### Página 209

=

ˆˆ

✞☎
✝✆

⃗′

S(V )

ˆˆ

⃗ x ) · ∇ GN (⃗x , ⃗x) = ✝ ✆
dS(⃗
′

✞☎

′

dS(⃗x′ )

S(V )

= −4π

˚

V

d3 x′ δ(⃗x′ − ⃗x) = −4π

luego
ˆˆ

✞☎
✝✆

∂
GN (⃗x′ , ⃗x)
′
∂n

dS(⃗x′ )

∂
GN (⃗x′ , ⃗x) = −4π
′
∂n

ˆˆ

dS(⃗x′ ) = S

S(V )

ahora bien, puesto que
✞☎
✝✆

S(V )

con S el área total de S(V ), la condición de contorno más simple es
⃗x′ ∈ S(V ) :

∂GN (⃗x′ , ⃗x)
4π
=−
′
∂n
S

Luego, debemos resolver
⃗ ′2 GN (⃗x′ , ⃗x) = −4πδ(⃗x′ − ⃗x)
⃗x′ ∈ V : ∇
⃗x ∈ V
′
⃗x′ ∈ S(V ) : ∂GN∂n(⃗x′ ,⃗x) = − 4π
S
o sea, resolvemos
⃗x ∈ V

⃗ ′2 LN (⃗x′ , ⃗x) = 0
⃗x′ ∈ V : ∇
′
∂L
∂
− ∂n
⃗x′ ∈ S(V ) : N∂n(⃗x′ ,⃗x) = − 4π
′ |⃗
S
x′ −⃗
x|

puesto que
GN (⃗x′ , ⃗x) =

| ⃗x′ − ⃗x |

+ LN (⃗x′ , ⃗x)

la solución formal del problema de Neumann es
φ(⃗x) =
4πϵ0

ˆˆ
1 ✞☎
d x ρ(⃗x )GN (⃗x , ⃗x) −
x′ )EN (⃗x′ )GN (⃗x′ , ⃗x) + ⟨φ⟩S
✝ ✆ dS(⃗
4π S(V )
V

˚

3 ′

′

′

donde ⟨φ⟩S es el valor medio del potencial sobre toda la superficie S(V )
ˆˆ
1 ✞☎
x)φ(⃗x)
⟨φ⟩S =
✝ ✆ dS(⃗
S S(V )
⃗ en V
La presencia de este término es un inconveniente. Pero no afecta E

---

### Página 210

Problema
El promedio temporal del potencial de un átomo de hidrógeno neutro es dado por
1 e−αr '
αr (
φ(r) =
q
1+
4πϵ0 r
donde q es la magnitud de la carga del electrón y α = a0 /2, siendo a0 el radio de Bohr.
Encuentre la distribución de cargas (continua y discreta) correspondiente a este potencial e
interprete físicamente su resultado
#### Solución
⃗ 2φ = − ρ
∇
ϵ0
En coordenadas esféricas, el operador laplaciano es
⃗2= 1 ∂ r+ 1∇
⃗ 2 (ϑ, φ)
∇
r ∂r2
r2

Sea
ψ(r) =
f (r) =
o sea

r
'

αr (
qe−αr 1 +
4πϵ0
φ(r) =

f (r)
r

y utilizamos la identidad
'
(
⃗ 2 ψf = ∇
⃗ · ∇ψf
⃗
⃗ · ψ ∇f
⃗ + f ∇ψ
⃗
∇
=∇
⃗ 2f + f ∇
⃗ 2 ψ + 2∇ψ
⃗ · ∇f
⃗
⃗ 2 ψf = ψ ∇
∇
r =| ⃗x |

⃗ 2ψ = ∇
⃗ 2 1 = −4πδ(⃗x)
∇
r
⃗ =∇
⃗ 1 = − ⃗x3 = − r̂2
∇ψ
r
|⃗
x|
r

⃗ 2 f (r) = 1 d rf (r) = 1 d (rf ′ + f )
∇
r dr2
r dr

=
y

con todo esto

(rf ′′ + 2f ′ ) = f ′′ + f ′
r
r

⃗ · ∇f
⃗ = − 2 r̂ · ∇f
⃗ = − 2 ∂ f = − 2 f′
2∇ψ
r
r2 ∂r
r2
⃗ 2 φ = 1 f ′′ + 2 f ′ − 4πf (r)δ(⃗x) − 2 f ′
∇
r
r2
r2
1 d2 f (r)
= −4πf (0)δ(⃗x) +
r dr2

y
f (0) =

q
4πϵ0

---

### Página 211

'
'
αr ((
−αr α
=
−α 1+
f =
qe
qe−αr
4πϵ0
4πϵ0
′

f′ = −
f ′′ = −

!

α2 r
α
−α−

1 αq −αr
e
(1 + αr)
4πϵ0 2

1 αq −αr
e
(α − α(1 + αr))
4πϵ0 2

f ′′ = −

1 αq −αr 2
e
α − α − α2 r)
4πϵ0 2
f ′′ =

1 α3 q −αr
re
4πϵ0 2

finalmente
⃗ 2 φ = − ρ = − q δ(⃗x) + 1 qα e−αr
∇
ϵ0
ϵ0
4πϵ0 2

Luego
ρ(⃗x) = qδ(⃗x) −

qα3 −αr
e
8π

La interpretación física es la siguiente
qδ(⃗x)
representa al protón en el origen. Mientras que
qα3 −αr
e
8π
es la densidad (media-temporal) de la nube orbital electrónica
−

"

---

### Página 212

Problema: Teorema del valor medio
Demuestre que para un espacio sin cargas, el potencial electrostático en cualquier punto es igual
al potencial promedio sobre cualquier esfera centrada en ese punto
#### Solución
Utilizaremos el teorema de Green
˚
'
( ˆˆ
'
(
☎
⃗ ψ − ψ∇
⃗ φ = ✞
⃗
⃗
d x φ∇
ds
n̂
·
∇ψφ
−
ψn̂
·
∇φ
✝✆
V

δV

En electrostática, el potencial escalar satisface
⃗ 2 φ(⃗x) = − ρ(⃗x)
∇
ϵ0
y se define la función de Green-Dirichlet
⃗ 2 GD (⃗x, ⃗x′ ) = −4πδ(⃗x − ⃗x′ ), ⃗x, ⃗x′ ∈ V
∇
⃗ D (⃗x, ⃗x′ ) = 0, ⃗x′ ∈ δV
G

del teorema de Green
˚

3 ′

V

'

′ ⃗ ′2

′

′

⃗ ′2 ′

d x φ ∇ GD (⃗x, ⃗x ) − GD (⃗x, ⃗x )∇ φ

−

˚

V

3 ′

′

′

d x 4πδ(⃗x − ⃗x )φ +

φ(⃗x) =
πϵ0

(

'
(
✞☎
⃗ ′ GD (⃗x, ⃗x′ ) − GD (⃗x, ⃗x′ )n̂′ · ∇
⃗ ′ φ′
= ✝ ✆ ds′ φ′ n̂′ · ∇
ˆˆ

δV

ˆˆ
ρ(⃗x′ )
✞☎
⃗ ′ GD (⃗x, ⃗x′ )
d x GD (⃗x, ⃗x )
= ✝ ✆ ds′ φ′ n̂′ · ∇
ε
V
δV

˚

3 ′

′

ˆˆ
1 ✞☎
⃗ ′ GD (⃗x, ⃗x′ )
d x GD (⃗x, ⃗x )ρ(⃗x ) −
x′ )φ(⃗x′ )n̂(⃗x′ ) · ∇
✝ ✆ dS(⃗
4π
V
δV

˚

3 ′

′

′

ahora, si V es una región libre de cargas
ˆˆ
1 ✞☎
⃗ ′ GD (⃗x, ⃗x′ )
x′ )φ(⃗x′ )n̂(⃗x′ ) · ∇
φ(⃗x) = −
✝ ✆ dS(⃗
4π δV
Escogemos ahora V como una esfera de radio a centrada en ⃗x, de forma que la función de
Green queda
GD (⃗x, ⃗x′ ) =
de esta forma

−
′
| ⃗x − ⃗x | a

⃗ ′ GD (⃗x, ⃗x′ ) =
∇

⃗x − ⃗x′
| ⃗x − ⃗x′ |3

---

### Página 213

Luego, para ⃗x′ ∈ S(V )

Así

′
′
⃗ ′ GD (⃗x, ⃗x′ ) = ⃗x − ⃗x · ⃗x − ⃗x = −
n̂(⃗x′ ) · ∇
=− 2
′
′
′
| ⃗x − ⃗x | | ⃗x − ⃗x |
| ⃗x − ⃗x |
a

ˆˆ
1 ✞☎
φ(⃗x) =
x′ )φ(⃗x′ ) = φ(⃗x, a)
✝ ✆ dS(⃗
4πa2 δV
con V : ϵ(⃗x, a)
Observación
La única condición sobre la esfera es que ella quede totalmente contenida en el vacío

---

### Página 214

Problema
Demuestre el siguiente corolario del teorema del valor medio. El campo electrostático en el vacío
satisface idénticamente las siguientes relaciones
⃗ x′ ) · E(⃗
⃗ x′ )
dS(⃗
=0
| ⃗x − ⃗x′ |
S(⃗
x)

ˆˆ

✞☎
✝✆

˚

V (S)

⃗ x′ ) ·
d3 x′ E(⃗

⃗x − ⃗x′
=0
| ⃗x − ⃗x′ |3

donde S es la superficie de una esfera de radio arbitrario con centro en ⃗x, y V (S) es su
volumen
#### Solución
En el espacio vacío de cargas
⃗ 2 φ(⃗x) = 0
∇
Utilizando el teorema de Green con
ψ(⃗x′ , ⃗x) =

˚

3 ′

dx

V (⃗
x)

⃗ ′2 φ(⃗x′ )
∇
⃗ ′2
− φ(⃗x′ )∇
′
| ⃗x − ⃗x |
| ⃗x − ⃗x′ |
=

ˆˆ

✞☎
✝✆

dS(⃗x′ )

S(⃗
x)

| ⃗x′ − ⃗x |

= 4π

˚

V (⃗
x)

d3 x′ φ(⃗x′ )δ(⃗x − ⃗x′ ) = 4πφ(⃗x)

∂φ(⃗
x′ )
∂n′

∂
− φ(⃗x′ ) ′
′
| ⃗x − ⃗x |
∂n | ⃗x − ⃗x′ |

luego
.
ˆˆ
ˆˆ
⃗ x′ ) · ∇
⃗ ′ φ(⃗x′ )
1 ✞☎
1 ✞ ☎ dS(⃗
′
′
′
⃗
⃗
dS(⃗x ) · ∇
φ(⃗
x
φ(⃗x) = −
)
+
✝✆
✝
✆
4π S(⃗x)
| ⃗x − ⃗x′ |
4π S(⃗x)
| ⃗x − ⃗x′ |
ˆˆ
ˆˆ
⃗ x′ ) · E(⃗x′ )
1 ✞☎ ⃗ ′
⃗x′ − ⃗x
1 ✞ ☎ dS(⃗
′
φ(⃗x) =
x)· ′
φ(⃗x ) −
✝ ✆ dS(⃗
✝✆
4π S(⃗x)
| ⃗x − ⃗x |3
4π S(⃗x) | ⃗x − ⃗x′ |
ˆˆ
ˆˆ
⃗ x′ ) · E(⃗x′ )
1 ✞☎
1 ✞ ☎ dS(⃗
′
′
φ(⃗x) =
dS(⃗
x
)φ(⃗
x
)
−
✝✆
✝✆
4πa2 S(⃗x)
4π S(⃗x) | ⃗x − ⃗x′ |
donde a =| ⃗x − ⃗x′ | es el radio de la esfera. (Independiente de ⃗x′ ).
Por el teorema del valor medio
ˆˆ
1 ✞☎
φ(⃗x) =
x′ )φ(⃗x′ )
✝ ✆ dS(⃗
4πa2 S(⃗x)
Luego
⃗ x′ ) · E(⃗
⃗ x′ )
dS(⃗
=0
| ⃗x − ⃗x′ |
S(⃗
x)

ˆˆ

✞☎
✝✆

---

### Página 215

Además

˚
⃗ x′ )
⃗ x′ )
E(⃗
E(⃗
3 ′⃗ ′
⃗ x)·
dS(⃗
d
x
∇
·
=
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
S(⃗
x)
V (S)
˚
⃗ ′ · E(⃗
⃗ x′ )
∇
⃗′
⃗ x′ ) · ∇
d3 x′
=
+ E(⃗
′ |
|
⃗
x
−
⃗
x
| ⃗x − ⃗x′ |
V (S)
/
*
˚
⃗x − ⃗x′
ρ(⃗x′ )
3 ′
′
⃗
+ E(⃗x ) ·
dx
=
ϵ0 | ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |3
V (S)
˚
′
⃗ x′ ) · ⃗x − ⃗x = 0
=−
d3 x′ E(⃗
| ⃗x′ − ⃗x |3
V (S)

ˆˆ

✞☎
✝✆

′

---

### Página 216

Problema
Demuestre que el campo electrostático en el vacío satisface idénticamente la siguiente relación
⃗ ·
∇

˚

V (⃗
x)

d3 x′

⃗ x′ )
E(⃗
=0
| ⃗x − ⃗x′ |

donde V (⃗x) es el volumen de una esfera de radio arbitrario y centro en ⃗x
#### Solución
Sabemos que, en el vacío

⃗x′ − ⃗x
=0
| ⃗x′ − ⃗x′ |3
V (⃗
x)
˚
˚
⃗ x′ )
E(⃗
3 ′⃗
′
3 ′⃗
⃗
=
d x E(⃗x ) · ∇
d
x
∇
·
0=
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
V (⃗
x)
V (⃗
x)
˚
⃗ x′ )
E(⃗
⃗
0=∇·
d3 x′
| ⃗x − ⃗x′ |
V (⃗
x)
˚

⃗ x′ ) ·
d3 x′ E(⃗

---

### Página 217

#### Capítulo 9
Solución de la Ecuación de Poisson y
Laplace
9.1.

Método de las Imágenes

La solución formal de los problemas de contorno en electrostática se logra mediante el método de las Funciones de Green. En los problemas prácticos no siempre es fácil descubrir o
calcular la función de Green correcta. Para ello se usan algunas técnicas especiales, como el
método de las imágenes o la expansión en funciones ortogonales. El método de las imágenes
se usa en problemas de una o más cargas puntuales en presencia de superficies de frontera, se
trata de conductores conectados a tierra o mantenidos a un potencial fijo. Este método de las
imágenes nos ayuda a encontrar la función de Green adecuada en los problemas de contorno
Dirichlet con φD = cte

Se trata de resolver el siguiente problema Dirichlet
/
⃗ 2 φ(⃗x, ⃗x′ ) = − qδ(⃗x−⃗x′ )
⃗x ∈ V : ∇
′
ϵ0
⃗x ∈ V :
⃗x ∈ S(V ) : φ(⃗x, ⃗x′ ) = φD

Bajo condiciones geométricas favorables (simetría) es posible infrerir que un número pequeño
de cargas puntuales, de magnitud apropiada, y ubicadas adecuadamente en la región externa
V4 , pueden simular las condiciones de contorno requeridas, estas son las cargas imágenes
Sean
V : región interior
V4 : región externa (conductor)
qi′ = qi′ (q, ⃗x′ ) = carga imagen
⃗x′i = ⃗x′i (q, ⃗x′ )= posición de la imagen

---

### Página 218

Además debe tenerse que
⃗x′i (q, ⃗x′ ) ∈ V4

Las cargas imágenes deben ser externas a la región de interés V , de manera que su potencial
sea una solución de la ecuación de Laplace en V . En efecto
′

⃗ 2 φ(⃗x, ⃗x′ ) = − qδ(⃗x − ⃗x )
∇
ϵ0
)
1 ) ′⃗ 2
qi′
⃗2 1
∇
qi ∇
=
′
4πϵ0 i | ⃗x − ⃗xi |
4πϵ0 i
| ⃗x − ⃗x′i |
=−
Luego

1 )
qi δ(⃗x − ⃗x′i ) = 0
ϵ0 i

δ(⃗x − ⃗x′i ) = 0, ∀⃗x ∈ V

Carga puntual q ubicada frente a un conductor plano a potencial cero, y de
extensión infinita

9.2.

Funciones Ortogonales y Expansiones

Una técnica muy poderosa de la física matemática es la representación de soluciones físicas
mediante expansiones en términos de funciones ortogonales. En cada problema se elige un
particular conjunto de funciones ort
ogonales adaptadas a la simetría del sistema. Revisemos las propiedades más generales de
las funciones ortogonales y veamos su uso en la representación de funciones mediante series
Sea ξ una variable real independiente, de rango
a≤ξ≤b
y {un (ξ)} un conjunto infinito numerable de funciones complejas definidas en (a, b), con
n = 1, 2, ... tales que
1. Todas ellas son de cuadrado integrable en (a, b)
ˆ b
a

dξ | un (ξ) |2 ≤ ∞

donde
| un (ξ) |2 = u∗n (ξ)un (ξ)

2. Además satisfacen la condición de ortogonalidad en (a, b)
m ̸= n →

ˆ b
a

dξu∗m (ξ)un (ξ) = 0

---

### Página 219

Normalización
Sea
Nn =

ˆ b
a

dξ | un (ξ) |2

0 < Nn < ∞
Definamos

ûn (ξ) = √ un (ξ)
Nn

Entonces el conjunto
{ûn (ξ), n = 1, 2, ..}
es un conjunto de funciones ortonormales en (a, b). La condición de ortonormalidad es
ˆ b
a

dξ û∗n (ξ)ûn (ξ) = δmn

Expansión
Sea f (ξ) una función arbitraria, en general compleja, de cuadrado integrable en (a, b)
ˆ b
a

dξ | f (ξ) |2 < ∞

Supongamos que, dado el número natural N , la serie finita
fN (ξ) =

N
)

an ûn (ξ)

n=1

sea una representación aproximada de la función f (ξ) en (a, b). Si modificamos los coeficientes an , n = 1, 2, ...N , modificamos la bondad de la aproximación. Surge entonces el problema
de ajustar los coeficientes de tal manera que la aproximación sea óptima. Luego requerimos que
el error cuadrático medio MN sea mínimo
MN =

ˆ b
a

dξ | f (ξ) − fN (ξ) |2

Se tiene
MN =

ˆ b
a

MN =

ˆ b
a

MN =

ˆ b
a

dξ | f (ξ) | −

N
)

m=1

dξ | f (ξ) −

dξ f ∗ (ξ) −

am

ˆ b
a

N
)

N
)
n=1

an ûn (ξ) |2

a∗n û∗n (ξ)

n=1

f (ξ) −

N
)

m=1

am û∗m (ξ)

ˆ b
ˆ b
N
N )
N
)
)
∗
∗
∗
dξf (ξ)ûm (ξ)−
an
dξf (ξ)ûn (ξ)+
an am
dξ û∗n (ξ)ûm (ξ)
∗

n=1

Utilizando la ortonormalidad

a

n=1 m=1

a

---

### Página 220

MN =

ˆ b
a

dξ | f (ξ) | −

N
)

am

ˆ b
a

m=1

∗

dξf (ξ)ûm (ξ) −

N
)

a∗n

n=1

ˆ b

dξf (ξ)ûn (ξ) +

a

N
)

a∗n an

n=1

Entonces, la condición para el mínimo es
ˆ b
∂MN
=−
dξ û∗k (ξ)f (ξ) + ak = 0
∂a∗k
a
ˆ b
∂MN
=−
dξ ûk (ξ)f ∗ (ξ) + a∗k = 0
∂ak
a
Luego, los mejores coeficientes de la representación aproximada son
ˆ b
an =
dξ û∗n (ξ)f (ξ)
a

se llaman los coeficientes de Fourier de la expansión
Completitud
El conjunto de funciones ortonormales {ûn (ξ)} es completo en (a, b) si, para cualquier función
f (ξ) de cuadrado integrable en (a, b), existe un número natural N0 [f ] tal que, dado ϵ > 0
arbitrario, se tiene
N > N0 [f ] → MN [f ] < ϵ
o sea que
lím MN [f ] = 0, ∀f

N →∞

siendo MN el error cuadrático medio mínimo
Convergencia en la media
Si el conjunto de funciones ortonormales {ûn (ξ)} es completo en (a, b) entonces se puede demostrar que la representación en serie
∞
)

an ûn (ξ) = S [f ]

n=1

con

an =

ˆ b
a

S [f ] =

∞
)
n=1

dξ û∗n (ξ)f (ξ)

un (ξ)

ˆ b
a

dξ ′ û∗n (ξ ′ )f (ξ ′ )

converge en la media a f (ξ) en (a, b). Vale decir que siendo f (ξ) una función acotada y
continua a trazos en (a, b) (por lo tanto de cuadrado integrabe) se tiene
1. En todo punto de continuidad
S [f ] = f (ξ)

---

### Página 221

2. En un punto de discontinuidad ordinaria
f (ξ + 0) + f (ξ − 0)

S [f ] =

Para todos los conjuntos de fnciones ortonormales que suelen usarse en física se ha demostrado su completitud
Relación de completitud
f (ξ) =

∞
)

an ûn (ξ)

n=1

f (ξ) =

∞
)

ûn (ξ)

a

n=1

f (ξ) =

ˆ b

ˆ b

′

∞
)

′

dξ f (ξ )

a

f (ξ) =

a

û∗n (ξ ′ )ûn (ξ)

n=1

por otro lado
ˆ b

dξ ′ û∗n (ξ ′ )f (ξ ′ )

dξ ′ f (ξ ′ )δ(ξ ′ − ξ), ∀f

Luego, la suma total de los términos bilineales û∗n (ξ)ûn (ξ) debe darnos una representación
de la delta de Dirac
∞
)
n=1

û∗n (ξ ′ )ûn (ξ) = δ(ξ ′ − ξ)

También vemos que, necesariamente
N
)

û∗n (ξ ′ )ûn (ξ) =

n=1

N
)

û∗n (ξ)ûn (ξ ′ )

n=1

es real, y que
N
)
n=1

û∗n (a)ûn (b) = 0, a ̸= b

Luego, un conjunto de funciones ortonormales completo queda caracterizado por
ˆ b
dξ û∗m (ξ)ûn (ξ) = δmn
a

---

### Página 222

∞
)

û∗n (ξ)ûn (ξ ′ ) = δ(ξ − ξ ′ )

n=1

Identidad de Parseval
Sea
f (ξ) =

∞
)

an ûn (ξ)

n=1

Consideremos

ˆ b
a

dξ | f (ξ) | =
=

ˆ b

∞
∞ )
)

dξ

a∗m û∗m (ξ)

a

m=1

a∗m an

ˆ b

m=1 n=1

∞ )
∞
)

=

∞
)

a

ˆ b
a

an ûn (ξ)

n=1

dξ û∗m (ξ)ûn (ξ)

a∗m an δmn =

m=1 n=1

Luego

∞
)

∞
)

a∗m an

n=1

dξ | f (ξ) | =

Teorema de Multiplicación
Sean
f (ξ) =

∞
)

∞
)
n=1

| an |2

an ûn (ξ)

n=1

g(ξ) =

∞
)

bn ûn (ξ)

n=1

ˆ b

∗

dξf (ξ)g(ξ) =

a

ˆ b

dξ

a

=

∞
∞ )
)

m=1 n=1

=

a∗m û∗m (ξ)

m=1

a∗m bn

∞
∞ )
)

∞
)

ˆ b
a

(f, g) =

ˆ b

bn ûn (ξ)

n=1

dξ û∗m (ξ)ûn (ξ)

a∗m bn δmn =

m=1 n=1

Con esto

∞
)

∞
)

a∗n bn

n=1

∗

dξf (ξ)g(ξ) =

a

∞
)
n=1

Caso bidimensional
Sea
f = f (ξ, η)
a ≤ ξ ≤ b, c ≤ η ≤ d

a∗n bn

---

### Página 223

Elegimos dos conjuntos completos ortonormales
/ ´b
dξ û∗ (ξ)ûn (ξ) = δmn
{ûn (ξ)} → 7∞a ∗ m
′
′
n=1 ûn (ξ)ûn (ξ ) = δ(ξ − ξ )
/ ´d
dηv̂ ∗ (η)v̂n (η) = δmn
{v̂n (η)} → 7∞c ∗ m
′
′
n=1 v̂n (η)v̂n (η ) = δ(η − η )

entonces el conjunto (producto tensorial)

{ûm (ξ)v̂n (η)} = {ŵm,n (ξ, η)}
satisface
ˆ bˆ d
a

c

∞ )
∞
)

m=1 n=1

dξdηû∗k (ξ)v̂l∗ (η)ûm (ξ)v̂n (η) = δkm δln

û∗m (ξ)v̂n∗ (η)ûm (ξ ′ )v̂n (η ′ ) = δ(ξ − ξ ′ )δ(η − η ′ )

Luego cualquier función f (ξ, η) de cuadrado integrable en (a, b) × (c, d) se puede representar
como
f (ξ, η) =

∞
∞ )
)

amn ûm (ξ)v̂n (η)

m=1 n=1

amn =

ˆ bˆ d
a

c

dξdηû∗m (ξ)v̂n∗ (η)f (ξ, η)

9.3.

Series de Fourier

9.3.1.

Condiciones de Dirichlet

Sea la función f (x) que satisface las siguientes condiciones (de Dirichlet)
(1) f (x) está definida en a < x < a + T
(2) f (x) y f ′ (x) son continuas a trazos (seccionalmente continuas) en a < x < a + T
(3) f (x) es periódica con período T en −∞ < x < ∞
f (x) = f (x + T )
Observación: la función f (x) se puede definir a partir de una función acotada F (x) definida
en −∞ < x < ∞ siendo F (x) y F ′ (x) continuas a trazos en a < x < a + T . En efecto
f (x) =

/

F (x)
si a < x < a + T
f (x + T ) si − ∞ < x < ∞

Teorema de la serie de Fourier
Si f (x) satisface las condiciones de Dirichlet en a < x < T entonces

---

### Página 224

(1) En todo punto de continuidad
"
""
!
!
∞ !
A0 )
2πnx
2πnx
f (x) =
+
An cos
+ Bn sin
T
T
n=1
(2) En un punto de discontinuidad ordinaria

donde

!
!
"
""
∞ !
f (x + 0) + f (x − 0)
2πnx
2πnx
A0 )
=
+
+ Bn sin
An cos
T
T
n=1
An =
T

ˆ a+T

Bn =
T

ˆ a+T

dx cos

a

dx sin

a

!

!

n2πx
T
n2πx
T

"

"

f (x)
f (x)

para n = 0, 1, 2, 3, .... Las condiciones de Dirichlet son suficientes (pero no necesarias) para
la convergencia en la media de la serie de Fourier. Sin perder generalidad, si f (x) satisface las
condiciones de Dirichlet en −T /2 < x < T /2 se tiene
!
!
"
""
∞ !
A0 )
2πnx
2πnx
f (x) =
+
An cos
+ Bn sin
T
T
n=1
!
"
ˆ
2 T /2
2πnx
dx cos
f (x)
An =
T −T /2
T
!
"
ˆ
2 T /2
2πnx
dx sin
Bn =
f (x)
T −T /2
T

Relaciones de ortogonalidad
!

"
2πnx
T
dx cos
cos
= δmn
T
−T /2
"
!
"
!
ˆ T /2
2πnx
T
2πmx
sin
= δmn
dx sin
T
T
−T /2
!
"
!
"
ˆ T /2
2πmx
2πnx
dx sin
cos
=0
T
T
−T /2
!
!
" ˆ T /2
"
ˆ T /2
2πmx
2πnx
dx cos
dx sin
=
=0
T
T
−T /2
−T /2
ˆ T /2

2πmx
T

"

!

---

### Página 225

9.4.

Ecuación de Laplace en Coordenadas Rectangulares
!

∂2
∂2
∂2
∇ φ(⃗x) =
+
+
∂x2 ∂y 2 ∂z 2
utilizamos el método de separación de variables
⃗2

"

φ(x, y, z) = 0

φ(x, y, z) = X(x)Y (y)Z(z)
Se tiene entonces

1⃗2
1 d2 X
1 d2 Y
1 d2 Z
∇ φ=
+
+
=0
φ
X dx2
Y dy 2
Z dz 2

luego
1 d2 X
1 d2 Y
1 d2 Z
=−
−
= −α2
X dx
Y dy
Z dz
1 d2 Y
1 d2 Z
=
α
−
= −β 2
Y dy 2
Z dz 2
1 d2 Z
= α2 + β 2 = −γ 2
Z dz 2
Resulta
d2 X
+ α2 X = 0
dx
d2 Y
+ β 2Y = 0
dy 2
d2 Z
+ γ2Z = 0
dz

con

α2 + β 2 + γ 2 = 0
Consideremos
X(x) = e±iαx
Y (y) = e±iβy
Z(z) = e±iγz
pero

γ 2 = − α 2 + β 2 = i2 α 2 + β 2 )
γ = ±i α2 + β 2

φαβ (x, y, z) = e±iαx±iβy±

√

α2 +β 2 z

es un conjunto de soluciones linealmente independientes de la ecuación de Laplace. La
ecuación de Laplace es lineal y homogénea, luego, por superposición
√
√
))
))
− i(αx+βy)− α2 +β 2 z
+ i(αx+βy)+ α2 +β 2 z
φ(x, y, z) =
Aαβ e
+
Aαβ e
α

α

β

β

−
es también una solución de la ecuación de Laplace. Las constantes α, β, A+
αβ , Aαβ están a
nuestra disposición. Ellas se determinan mediante las condiciones de contorno

---

### Página 226

9.4.1.

Problema en 2 dimensiones

En ciertos problemas, la simetría permite establecer que el potencial es sólo función de dos
variables, digamos x e y. En este caso se debe resolver
! 2
"
∂
∂
⃗ φ(⃗x) =
+
φ(x, y) = 0
∇
∂x2 ∂y 2
La lógica es la misma, utilizando el método de separación de variables
φ(x, y, z) = X(x)Y (y)
Se tiene entonces

1⃗2
1 d2 X
1 d2 Y
∇ φ=
+
=0
φ
X dx2
Y dy 2

luego
1 d2 X
1 d2 Y
=
−
= −α2
X dx2
Y dy 2
1 d2 Y
= α2
Y dy 2
Resulta
d2 X
+ α2 X = 0
dx
d2 Y
− α2 Y = 0
dy 2
Las soluciones son de la forma
X(x) = e±iαx
Y (y) = e±αy

La solución general de la ecuación de Laplace está dada por la familia de funciones
X(x) = Aα cos (αx) + Bα sin (αx)
Y (y) = Cα eαy + Dα e−αy
con Aα , Bα , Cα , Dα constantes reales.

---

### Página 227

Problema
Potencial en una Caja

Resolver

⃗ 2 φ(⃗x) = 0
⃗x ∈ V : ∇
⎧
⎪
⎪
⎪
⎪
⎪
⎪
⎨

φ(0, y, z) = 0
φ(a, y, z) = 0
φ(x, 0, z) = 0
⃗x ∈ S(V ) :
φ(x, b, z) = 0
⎪
⎪
⎪
⎪
φ(x, y, 0) = 0
⎪
⎪
⎩
φ(x, y, c) = φD (x, y)
#### Solución
φ(x, y, z) =

))'
α

β

(
√
√
− − α2 +β 2 z
α2 +β 2 z
A+
ei(αx+βy)
e
+
A
e
αβ
αβ

Esto se puede reescribir como
φ(x, y, z) =

))2
α≥0

β

3 √α2 +β 2 z iβy 2 − iα
3 −√α2 +β 2 z iβy
+
−
iαx
−iαx
−iα
A+
e
e
e
+
A
e
e
+
A
e
+
A
e
e
αβ
−αβ
αβ
−αβ

Se tiene
±
φ(0, y, z) = 0 → A±
αβ + A−αβ = 0

Luego
φ(x, y, z) =

))2
α≥0

β

2 iαx
33 √α2 +β 2 z iβy 2 − 2 iαx
33 −√α2 +β 2 z iβy
−iαx
−iαx
−
e
e
+
A
−
e
e
A+
e
e
e
e
αβ
αβ

---

### Página 228

Además
φ(a, y, z) = 0 → eiαa − e−iαa = 2i sin αa = 0
Esto limita los valores posibles que puede tomar α
aα = mπ → m = 0, ±1, ±2, ...
α=

mπ
→ m = 0, ±1, ±2, ...
a

2i sin

' mπ (
'
(
√
√
−
α2 +β 2 z
− α2 +β 2 z
e
+
A
e
x eiβy A+
mβ
mβ
a

Así
∞ )
)

φ(x, y, z) =

m=1

β

y se puede escribir como

φ(x, y, z) =

∞ )
)

2i sin

m=1 β≥0

' mπ ( '2
3 −√α2 +β 2 z (
3 √α2 +β 2 z 2 − iβy
+
−
iβy
−iβy
−iβy
x
A+
e
e
+
A
e
e
+
A
e
+
A
e
mβ
m−β
mβ
m−β
a

Se cumple además
±
φ(x, 0, z) = 0 → A±
αβ + Aα−β = 0

' mπ ( '
(
√
√
+
−
α2 +β 2 z
− α2 +β 2 z
2i sin
+ Amβ 2i sin(βy)e
φ(x, y, z) =
x Amβ 2i sin(βy)e
a
m=1 β≥0
∞ )
)

y
φ(x, b, z) = 0 → 2i sin βb = 0
Esto limita los valores posibles que puede tomar β
bβ = nπ → n = 0, ±1, ±2, ...
β=

nπ
→ n = 0, ±1, ±2, ...
b

En resumen, α y β satisfacen
nπ
mπ
,β =
a
b
:' (
m 2 ' n (2
α2 + β 2 = π
+
= γmn
a
a
α=

m, n = 0, ±1, ±2, ...
y la solución general queda
φ(x, y, z) =

' nπy (
' πmx (
γmn z
−
−γmn z
(2i)2 A+
e
+
A
e
sin
sin
mn
mn
a
b
m=1 n=1
∞ )
∞
)

El potencial también debe ser nulo en z = 0

---

### Página 229

(2i)

Sea

−
A+
mn + Amn

sin

' πmx (

sin

a

' πny (
b

=0

−
A+
mn + Amn = 0

2 −
Amn = (2i)2 A+
mn = −(2i) Amn

luego
3 1
2 γmn z
γmn z
−
−γmn z
−γmn z
(2i)2 A+
A
=
e
+
A
e
e
−
e
mn
mn
mn
= Amn sinh γmn z
Con todo esto, la solución toma la forma
φ(x, y, z) =

∞ )
∞
)

Amn sin

m=1 n=1

Por último, la condición en z = c entrega
φ(x, y, c) = φD (x, y) =

∞ )
∞
)

' πmx (
a

sin

' nπy (
b

(Amn sinh γmn ) sin

m=1 n=1

Esta es una doble serie de Fourier

sinh γmn z

' πmx (
a

sin

' nπy (
b

"
πnξ
f (ξ) =
Bn sin
L
n=1
!
"
ˆ
2 L
πnξ
dξ sin
Bn =
f (ξ)
L 0
L
!

∞
)

Luego la solución del problema es
φ(x, y, z) =

∞
∞ )
)

Amn sin

m=1 n=1

con

Amn =
ab sinh γmn c

ˆ a

dx

ˆ b

γmn = π

' πmx (
a

dy sin

:' (
m 2
a

sin

' nπy (

' πmx (
a

+

' n (2
b

b

sin

sinh γmn z

' πny (
b

φD (x, y)

c

---

### Página 230

Problema
Determinar el potencial en la región que comprende el interior de una caja rectangular de
longitud infinita, cuya sección transversal se aprecia en la figura

#### Solución
Dado que la longitud de la caja es muy larga, el potencial tendrá la misma forma para cualquier
sección transversal. Se debe resolver entonces la ecuación de Laplace
⃗ 2 φ(x, y) = 0
∇
con las condiciones de borde
⎧
φ(0, y) = 0
⎪
⎪
⎨
φ(b, y) = 0
⃗x ∈ S(V ) :
φ(x,
0) = 0
⎪
⎪
⎩
φ(x, a) = V0
La solución general de la ecuación de Laplace es
φ(x, y) = X(x)Y (y)
donde X(x) e Y (y) pertenecen a las familias de funciones
X(x) = Aα cos (αx) + Bα sin (αx)
Y (y) = Cα eαy + Dα e−αy
Para cualquier α real, φ(x, y) es solución de la ecuación de Laplace. Sin embargo, las condiciones de borde limitarán los valores posibles de α. En efecto, debe cumplirse que

de forma que

φ(0, y) = 0 → X(0) = 0
Aα = 0

es decir
X(x) = Bα sin (αx)
Además, debe tenerse
es decir

φ(b, y) = 0 → Bα sin (αb) = 0
αb = nπ, n = 0, 1, 2, ...

---

### Página 231

luego

nπ
, n = 0, 1, 2, ...
b
Es decir, la familia de funciones que satisfacen la ecuación de Laplace y cumplen con
φ(0, y) = φ(b, y) = 0 está dada por
α=

φ(x, y) = X(x)Y (y)
' nπ (
x , n = 0, 1, 2, ...
X(x) = sin
b
nπ

nπ

Y (y) = An e b y + Bn e− b y , n = 0, 1, 2, ...
La solución general toma la forma
φ(x, y) =

∞
)

sin

n=1

' nπ ( 2
nπ
nπ 3
x An e b y + Bn e− b y
b

además se tiene φ(x, 0) = 0
φ(x, 0) =

∞
)

sin

n=1

Luego

' nπ (
x (An + Bn ) = 0
b

An = −Bn
y entonces
φ(x, y) =

∞
)

sin

n=1

φ(x, y) =

∞
)

sin

n=1

φ(x, y) =

' nπ (
2 nπ
nπ 3
x An e b y − e− b y
b

∞
)

' nπ (
' nπ (
x 2An sinh
y
b
b

Cn sin

n=1

' nπ (
' nπ (
x sinh
y
b
b

Donde Cn = 2An . Por último, la condición de borde φ(x, a) = V0 entrega
φ(x, a) =

∞
)

Cn sin

n=0

V0 =

∞
)
n=0

' nπ (
' nπ (
x sinh
a = V0
b
b

Cn sin

' nπ (
' nπ (
x sinh
a
b
b

¿Cómo podemos encontrar los Cn ?. La clave está en notar que esta es una expansión en
series de Fourier. Si F : [−b, b] → R es una función de cuadrado integrable en [-b,b], admite
una expansión en series
' nπ ( )
' nπ (
a0 )
F (x) =
An cos
Bn sin
+
x +
x
b
b
n=1
n=1
con

Bn =
b

ˆ b

−b

dxF (x) sin

' nπ (
x , n = 0, 1, 2...
b

---

### Página 232

' nπ (
x , n = 0, 1, 2...
dxF (x) cos
b
−b

ˆ b

An =
b

En particular, si F es una función impar sobre [−b, b], An = 0 ∀n, y entonces
' nπ (
)
x
F (x) =
Bn sin
b
n=1
con

Bn =
b

ˆ b

dxF (x) sin

' nπ (
x , n = 0, 1, 2...
b

Interpretemos ahora el resultado que hemos obtenido
∞
' nπ ( )
' nπ (
' nπ (
V0 =
x sinh
a =
x
Cn sin
Bn sin
b
b
b
n=0
n=0
∞
)

Es justamente la expansión en serie de Fourier de V0 . Entonces
ˆ
' nπ ( 2V ˆ b
' nπ (
2 b
Bn =
dxV0 sin
dx sin
x =
x
b 0
b
b 0
b
' nπ ( &b
2V0 b
V0
&
cos
x & =2
(1 − cos (nπ))
Bn = −
b nπ
b
nπ
V0
para n impar. Además,
Notar que Bn = 0 para n impar, mientras que Bn = 4 nπ
Bn = Cn sinh
Luego

' nπ (
Bn
a → Cn =
b
sinh nπ
a
b
Cn = 0, n par

Cn =

4V0
3 , n impar
nπ sinh nπ
a
b

y la solución para el potencial queda
∞

4V0 )
( sin
'
φ(x, y) =
π n=1 (2n − 1) sinh (2n−1)πa
b

!

(2n − 1)πx
b

"

sinh

!

(2n − 1)πy
b

"

---

### Página 233

La siguiente figura es un gráfico de las curvas de nivel para a = b = 5 y V0 = 1 [V]

---

### Página 234

Problema
Encuentre el potencial para la región 0 ≤ x ≤ a, y ≥ 0, con las condiciones de borde de Dirichlet
⎧
φ(0, y) = 0
⎪
⎪
⎨
φ(a, y) = 0
⃗x ∈ S(V ) :
límy→∞ φ(x, y) = 0
⎪
⎪
⎩
φ(x, 0) = V (x)

#### Solución
El potencial en V satisface la ecuación de Laplace
⃗ 2 φ(x, y) = 0
∇
cuya solución está dada por
φ(x, y) = X(x)Y (y)
donde
X(x) = Aα cos (αx) + Bα sin (αx)
Y (y) = Bα eαy + Cα e−αy
La condición de borde φ(0, y) = 0 implica

Además, debe tenerse

X(0) = Aα = 0 → X(x) = Bα sin (αx)
φ(a, y) = 0 → X(a) = 0
sin (αa) = 0

Entonces
α=

nπ
, n = 0, 1, 2, ...
a

Entonces la solución toma la forma
' nπ ( 2
nπ
nπ 3
sin
x An e a y + Bn e− a y
φ(x, y) =
a
n=1
∞
)

---

### Página 235

La condición en el infinito es
lím φ(x, y) = 0

y→∞

de forma que An = 0, ∀n = 0, 1, 2, ...
φ(x, y) =

∞
)

Bn sin

n=1

Por último, la condición φ(x, 0) = V (x) es
φ(x, 0) =

∞
)

Bn sin

n=1

' nπ ( nπ
x e− a y
a

' nπ (
x = V (x)
a

Ahora, consideremos F (x), −a ≤ x ≤ x. Si F (x) es cuadrado integrable en [−a, a], entonces
existe su serie de Fourier

donde

∞
∞
' nπ ( )
' πn (
a0 )
F (x) =
+
x +
x
An cos
Cn sin
a
a
n=1
n=1

' nπ (
x , n = 0, 1, 2, ...
a
−a
ˆ
' nπ (
1 a
Cn =
dxF (x) sin
x , n = 0, 1, 2, ...
a −a
a

An =
a

ˆ a

dxF (x) cos

Si F (x) es impar, entonces An = 0 ∀n, de forma que
F (x) =

∞
)

Cn sin

n=1

con

Cn =
a

Con esto,

' πn (
x
a

' nπ (
x , n = 1, 2, ...
dxF (x) sin
a

ˆ a

φ(x, 0) =

∞
)

Bn sin

n=1

' nπ (
x = V (x)
a

corresponde a la expansión en serie de Fourier de V (x), −a < x < a, con V (−x) = −V (x)
(por supuesto que físicamente sólo interesa V (x) para 0 ≤ x ≤ a). Así, la solución del problema
es

con

' nπ ( nπ
φ(x, y) =
Bn sin
x e− a y
a
n=1
∞
)

Bn =
a

ˆ a

dxV (x) sin

' nπ (
x , n = 1, 2, ...
a

Supongamos que φ(x, 0) = V (x) = V0 (constante). Luego
ˆ
' nπ (
' nπ ( &a
2V0 a
2V0 a
&
dx sin
x =−
cos
x & , n = 1, 2, 3...
Bn =
a 0
a
a nπ
a

---

### Página 236

Bn =

Finalmente

2V0
(1 − cos (nπ)) , n = 1, 2, 3...
nπ
/
0 si n par
Bn = 4V0
si n impar
nπ

∞
)

4V0
φ(x, y) =
sin
(2n − 1)π
n=1

!

"
(2n−1)π
(2n − 1)π
x e− a y
a

El gráfico muestra la solución para V0 = 0,1, a = 5, y tomando 50 términos en la serie

---

### Página 237

9.5.

Ecuación de Laplace en coordenadas Cilíndricas

9.5.1.

Problema bidimensional

Supongamos un problema de Laplace plano, en donde la geometría del problema permite
que sea más favorable utilizar coordenadas polares
!
"
∂φ
1 ∂2φ
1 ∂
⃗
∇ φ=
r
+ 2 2 =0
r ∂r
∂r
r ∂ϕ
Utilizando el método de separación de variables, es decir
φ(r, ϕ) = R(r)Ψ(ϕ)
De forma que

!

1 ∂
∇ φ=Ψ
r ∂r
⃗2

∂R(r)
r
∂r

"

1 ∂ 2 Ψ(ϕ)
+ R(r) 2
=0
r ∂ϕ2

Multiplicando por rφ (si φ nunca es cero)
!
"
r ∂
∂R(r)
1 ∂ 2 Ψ(ϕ)
=0
r
+
R(r) ∂r
∂r
Ψ ∂ϕ2
o, equivalentemente

r ∂
R(r) ∂r

!

∂R(r)
r
∂r

"

=−

1 ∂ 2 Ψ(φ)
Ψ(ϕ) ∂ϕ2

La única forma de que esto último sea posible es que ambas expresiones sean una constante
!
"
r d
dR(r)
1 ∂ 2 Ψ(φ)
= α2
r
=−
R(r) dr
dr
Ψ(ϕ) ∂ϕ2
de forma que

r d
R(r) dr

!

dR(r)
r
dr

"

= α2

1 d2 Ψ(ϕ)
= −α2
Ψ(ϕ) dϕ2
1. Primer caso, α ̸= 0
La solución para Ψ es inmediata
Ψ(ϕ) = e±iαϕ
y para R(r), con α ̸= 0
r d
R(r) dr

!

dR(r)
r
dr
r

"

r
=
R(r)

!

dR(r)
d2 R(r)
+r
dr
dr2

d2 R(r)
dR(r)
= R(r)α2
+ r2
dr
dr2

"

= α2

---

### Página 238

Esta ecuación pertenece al tipo Cauchy, la solución es de la forma
R(r) = ra
En efecto, es solución si
rara−1 + r2 a(a − 1)ra−2 = ra α2
ara + a(a − 1)ra = ra α2

a + a(a − 1) = α2 → a2 = α2
Entonces
a = ±α
y la solución para R(r), con α ̸= 0 es
R(r) = Aα rα + Bα r−α

2. Segundo caso, α = 0
Aquí,
r d
R(r) dr
luego

y

!

dR(r)
r
dr

"

!

dR(r)
r
dr

"

=0

= 0 → R(r) = a0 + b0 ln r

1 d2 Ψ(ϕ)
=0
Ψ(ϕ) dϕ2

Ψ(ϕ) = A0 + B0 ϕ

Finalmente, la solución general a la ecuación de Laplace en coordenadas polares es la familia
de soluciones
φ(r, ϕ) = (a0 + b0 ln r) (A0 + B0 ϕ) + Aα rα + Bα r−α (Cα sin (αϕ) + Dα cos (αϕ))

---

### Página 239

Problema
Determine el potencial electrostático al interior de la región limitada por un conductor de
extensión infinita cuya forma se muestra en la figura. El conductor se encuentra a potencial V

#### Solución
Dada la geometría, es natural utilizar coordenadas polares para resolver este problema. Si en
la región Ω : 0 ≤ ϕ ≤ β no hay carga, entonces el potencial satisface
⃗ 2 φ = 0, enΩ
∇
La solución general de la ecuación de Laplace en coordenadas polares está dada por
φ(r, ϕ) = (a0 + b0 ln r) (A0 + B0 ϕ) + Aα rα + Bα r−α (sin (Cα αϕ) + Dα cos (αϕ))

El potencial debe ser finito en el origen r = 0, de forma que Bα = 0, ∀α, igualmente b0 = 0.
La solución que nos interesa toma la forma
φ(r, ϕ) = (A0 + B0 ϕ) + Aα rα (Cα sin (αϕ) + Dα cos (αϕ))

La condición de borde φ(r, 0) = V implica
φ(r, 0) = A0 + Aα rα Dα = V
Lo cual se cumple para todo r si A0 = V , Dα = 0. Así
φ(r, ϕ) = (V + B0 ϕ) + Aα rα sin (αϕ)
Además, la condición de borde en = β entrega
φ(r, β) = (V + B0 β) + Aα rα sin (αβ) = V

---

### Página 240

B0 β + Aα rα sin (αβ) = 0
lo cual se cumple para todo r si
B0 = 0
nπ
, n = 0, 1, 2, ...
sin (αβ) = 0 → α =
β
Finalmente, la solución queda
φ(r, ϕ) = V +

∞
)

n

An r sin

n=0

!

nπ
ϕ
β

"

---

### Página 241

9.6.

Ecuación de Laplace en Coordenadas Esféricas
⃗ 2 φ(r, ϑ, ϕ) = 0
∇
1 ∂
r2 ∂r

!

r

2 ∂φ

∂r

"

∂
+ 2
r sin ϑ ∂ϑ

Notar que
1 ∂
r2 ∂r
y

!

r

2 ∂φ

1 ∂
1 ∂2
(rφ)
=
r ∂r2
r ∂r
luego

∂r
!

"

!

∂φ
sin ϑ
∂ϑ

"

=

∂ 2 φ 2 ∂φ
+
∂r2
r ∂r

+

∂2φ
r2 sin2 ϑ ∂ϕ2

"
∂φ
∂ 2 φ 2 ∂φ
r
+φ = 2 +
∂r
∂r
r ∂r

1 ∂ 2∂
1 ∂2
r
r
=
r2 ∂r ∂r
r ∂r2

Así, la ecuación de Laplace queda de la forma
!
"
1 ∂2
∂
∂φ
1 ∂2φ
(rφ)
+
=0
sin
ϑ
+
r ∂r2
r2 sin ϑ ∂ϑ
∂ϑ
r2 sin ϑ ∂ϕ2
supongamos
R(r)
φ(r, ϑ, ϕ) =
Θ(ϑ)Φ(ϕ)
r
resulta
!
"
ΘΦ d2 R
dΘ
RΘ d2 Φ
RΦ d
sin ϑ
+ 3 2
+ 3
=0
r dr2
r sin ϑ dϑ
dϑ
r sin ϑ dϕ2

r2 sin2 ϑ d2 R sin ϑ d
+
R
dr2
Θ dϑ

!

dΘ
sin ϑ
dϑ

"

=−

1 d2 Φ
= m2
Φ dϕ2

La ecuación para Φ es inmediata
d2 Φ
+ m2 Φ = 0
dϕ2
cuya solución es
Φ(ϕ) = e±imϕ

Es evidente que esta función debe ser periódica
Φ(ϕ ± 2π) = Φ(ϕ)
es decir
e±im(ϕ+2π) = e±i2πm e±imϕ = e±imϕ

---

### Página 242

e±i2πm = cos(2πm) ± i sin(2πm) = 1
luego m = 0, ±1, ±2, ...
Φm (ϕ) = eimϕ
m = 0, ±1, ±2, ...
Con esto
r2 d2 R
d
=
−
R dr2
Θ sin ϑ dϑ
Luego

!

dΘ
sin ϑ
dϑ

"

+

m2
= l(l + 1)
Φ sin2 ϑ

d2 R l(l + 1)
−
R=0
dr2
r2

Esta ecuación pertenece al tipo Cauchy
x2 y ′′ (x) + αxy ′ (x) + βy(x) = 0
cuya solución es de la forma
y(x) = xa → y ′ (x) = axa−1 → y ′′ (x) = a(a − 1)xa−2
luego
a(a − 1)xa + αaxa + βxa = 0
a2 + (α − 1)a + β = 0
⎧
√
(1−α)+ (1−α −4β
⎨
a1 =
√2 2
a=
(1−α)− (1−α −4β
⎩
a2 =

Por superposición , tenemos que la solución general es
y(x) = Axa1 + Bxa2
En nuestro caso
R(r) = ra
a2 − a − l(l + 1) = 0

√

1 + 4l + 4l2
/
1 ± (2l + 1)2
1 ± (2l + 1)
l+1
=
=
a=
−l
a=

1±

1 + 4l(l + 1)
1±
=

---

### Página 243

Luego
Rl (r) = Al rl+1 + Bl r−l
Nos queda únicamente la ecuación para Θ
!
" !
"
dΘ
m2
1 d
sin ϑ
+ l(l + 1) −
Θ=0
sin ϑ dϑ
dϑ
sin2 ϑ
Sea µ = cos ϑ, 0 ≤ ϑ ≤ π → −1 ≤ µ ≤ 1

P (µ) = Θ(ϑ)
dΘ
dµ dP
dP
=
= − sin ϑ
dϑ
dϑ dµ
dµ
1 d
d
=−
dµ
sin ϑ dϑ
Luego la ecuación es
d
dµ

!

dP
(1 − µ )
dµ

"

!

m2
+ l(l + 1) −
1 − µ2

"

P =0

Esta es la ecuación generalizada de Legendre, sus soluciones se llaman funciones asociadas
de Legendre. Estudiaremos primero la ecuación ordinaria de Legendre
m=0
Esto equivale a resolver el problema de Laplace para casos en que existe simetría azimutal
(es decir, donde el potencial no depende de la variable ϕ). En este caso
3 dP
d 2
1 − µ2
+ l(l + 1)P (µ) = 0
dµ
dµ
Las soluciones deben ser monovalentes, finitas, y continuas en −1 ≤ µ ≤ 1. Estos son los
polinomios de Legendre

9.7.

Problemas de Contorno con Simetría Azimutal

Para problemas con simetría esférica y simetría azimutal (es decir, el potencial no depende
de ϕ)
R(r)
Θ(ϑ)
r
La solución general a la ecuación de Laplace queda en términos de potencias de r y polinomios de Legendre
φ = φ(r, ϑ) =

φ(r, ϑ) =

∞
)
l=0

Al rl + Bl r−(l+1) Pl (cos ϑ)
Al , Bl

---

### Página 244

se determinan usando las condiciones de contorno
Problema :Potencial en una esfera

El problema a resolver es
⃗x ∈ S(a) : φ(⃗x) = φD (ϑ)
⃗ 2 φ(⃗x) = 0
⃗x ∈ V : ∇

a) Problema interno (r ≤ a)
Se requiere que φ(| ⃗x |= 0) sea finito, de forma que Bl = 0 (l = 0, 1, 2, ...)
φ(r, ϑ) =

∞
)

Al rl Pl (cos ϑ)

l=0

La condición de contorno es

φ(a, ϑ) = φD (ϑ) =

∞
)

Al al Pl (cos ϑ)

l=0

es una serie de Legendre. Luego
2l + 1
Al =
2al

ˆ π

dϑ sin ϑPl (cos ϑ)φD (ϑ)

b) Problema externo (r ≥ a)
Se debe tener
lím φ(⃗x) = 0

|⃗
x|→∞

con lo que
Al = 0, l = 0, 1, 2, ...
luego
φ(r, ϑ) =

∞
)
Bl
l=0

rl+1

Pl (cos ϑ)

---

### Página 245

el potencial debe ser continuo en el contorno, por lo que
φ(a, ϑ) =

∞
)
Bl
l=0

de donde

2l + 1 l+1
Bl =
a

al+1

ˆ π

Pl (cos ϑ) = φD (ϑ)

dϑ sin ϑPl (cos ϑ)φD (ϑ)

---

### Página 246

Problema
Se tiene una esfera conductora cuyos hemisferios se encuentran a distinto potencial

/

φ0 si 0 ≤ ϑ ≤ π/2
−φ0 si π/2 ≤ ϑ ≤ π

φD (ϑ) =

Encontrar el potencial electrostático en el interior de la esfera, y la densidad superficial de cargas
#### Solución
Se trata de un problema con simetría azimutal donde el potencial satisface la ecuación de
Laplace excepto en el contorno r = a. Para el problema interno, el potencial es de la forma
φ(r, ϑ) =

∞
)

Al rl Pl cos(ϑ)

l=0

(se ha exigido que debe ser finito en r = 0). Además se cumple
φ(a, ϑ) =

∞
)

Al al Pl cos(ϑ) = φD

l=0

de donde se obtiene

2l + 1
Al =
2al

2l + 1
Al =
2al
;ˆ

2l + 1
Al = φ0
2al

ˆ π

dϑ sin ϑPl (cos ϑ)φD (ϑ)

π/2

dϑ sin ϑPl (cos ϑ)φ0

ˆ π

dϑ sin ϑPl (cos ϑ)

dµPl (µ) −

ˆ −1

*
dµPl (µ)

dµPl (µ) −

ˆ 0

dϑ sin ϑPl (cos ϑ)φ0 −

0ˆ
π/2

π/2

dϑ sin ϑPl (cos ϑ) −

2l + 1
Al = −φ0
2al
2l + 1
Al = φ0
2al

/ˆ 0

/ˆ 1

<

ˆ π

π/2

−1

*
dµPl (µ)

Si l es par, Pl (µ) = Pl (−µ), mientras que si l es impar, Pl (µ) = −Pl (−µ). Luego, Al = 0
para l par, y
ˆ
φ0 1
Al = (2l + 1) l
dµPl (µ)
a 0
para l impar. Además, se tiene que para l = 2n − 1, n = 1, 2, 3...

---

### Página 247

ˆ 1

dµP2n−1 (µ) = (−1)n+1

(2n − 3)!!
2n n!

Luego
φr,ϑ = φ0

∞
)
(−1)n+1 (4n − 1)(2n − 3)!!

a2n−1 2n n!

n=1

r2n−1 P2n−1 (cos ϑ)

Con esto es posible encontrar la densidad superficial de cargas, puesto que
&
&
⃗ ϑ) · r̂ = −ϵ0 ∇φ(r,
⃗
σ(ϑ) = ϵ0 E(a,
ϑ)&
· r̂
r=a

∂φ(r, ϑ) &&
σ(ϑ) = −ϵ0
&
∂r
r=a

∞
)
∂φ
(−1)n+1 (4n − 1)(2n − 1)!! 2n−2
P2n−1 (cos ϑ)
= φ0
r
∂r
a2n−1 2n n!
n=1

luego

∞

σ(ϑ) = ϵ0

φ0 ) (−1)n+2 (4n − 1)(2n − 1)!!
P2n−1 (cos ϑ)
a n=1
2n n!

Fig. 9.1: Equipotenciales para φ0 = 100 [V] y usando 10 términos en la expansión

---

### Página 248

Problema
Encuentre el potencial en todo el espacio de un anillo de radio R cargado con carga Q uniforme
#### Solución
El potencial en todo el espacio (excepto sobre el anillo) cumple
⃗ 2 φ(⃗x) = 0
∇

Ya fue resuelto anteriormente el valor del potencial sobre el eje z
φ(z) =

Q
√
4πϵ0 z 2 + R2

Es claro que el problema posee una simetría azimutal (el potencial no depende del ángulo
polar ϕ). Con esto
φ(r, ϑ) =

∞
)
l=0

Al rl + Bl r−(l+1) Pl (cos ϑ)

Se deben imponer las condiciones de contorno adecuadas. Como conocemos el potencial
sobre el eje z, es decir para ϑ = 0
φ(r, 0) =

φ(r, 0) =

Q
√
4πϵ0 r2 + R2

∞
∞
)
)
2 l
2 l
Q
−(l+1)
−(l+1)
A
P
A
=
r
+
B
r
(1)
=
r
+
B
r
l
l
l
l
l
4πϵ0 (r2 + R2 )1/2
l=0
l=0

pues Pl (1) = 1 para todo l = 0, 1, 2, ...
∞
)
2 l
Q
Al r + Bl r−(l+1)
φ(r, 0) =
=
1/2
4πϵ0 (r2 + R2 )
l=0

Separamos en dos casos
1) r > R

Q 1
Q
'
(1/2 =
4πϵ0
4πϵ0 r
r 1 + Rr

;

! "2 <−1/2
R
1+
r

---

### Página 249

−1/2

Como R/r < 1, la expansión en serie de potencias de (1 + (R/r)2 )
por

! "2 <−1/2
∞
& xl
)
dl
R
&
−1/2
= (1 + x)
=
1+
f (x)&
r
dx
x=0 l!
l=0

;
con

f (x) = (1 + x)−1/2

se tiene

&
&
f (x)&

&
&
f ′ (x)&

=1

=−
x=0
! "! "
&
&
f ′′ (x)&
=
x=0
"
!
"
! "
!
&
&
′′′
f (x)&
=−
x=0
! "! "! "! "
&
&
f 4 (x)&
=
x=0

En general

&
&
f (x)&
l

de forma que
;
Entonces

x=0

x=0

=

(−1)l (2l − 1)!!
2l

! "2 <−1/2 )
! "2l
∞
R
R
l (l − 1)!!
1+
=
(−1)
l
r
2 l!
r
l=0

∞
2l
Q )
Q
l (l − 1)!! R
(−1)
'
2 32 (1/2 = 4πϵ0
4πϵ0
2l l! r2l+1
l=0
r 1 + Rr
∞
)

l

Al r + Bl r

−(l+1)

l=0

∞

2l
Q )
l (l − 1)!! R
=
(−1)
4πϵ0 l=0
2l l! r2l+1

Por supuesto que debe tenerse
lím φ(⃗x) = 0

|⃗
x|→∞

por lo que
Al = 0, ∀l
∞
)
l=0

∞

Bl r

−(l+1)

(l − 1)!! R2l
Q )
=
(−1)l
4πϵ0 l=0
2l l! r2l+1

de aquí se obtiene que Bl = 0 para l impar, luego

converge, y está dada

---

### Página 250

∞
)

∞

B2l r−(2l+1) =

l=0

B2l =

Q )
(l − 1)!! R2l
(−1)l
4πϵ0 l=0
2l l! r2l+1

Q (−1)l (2l − 1)!! 2l
R
4πϵ0 2l
l!

y entonces el potencial queda, para r > R
∞
)
Q (−1)l (2l − 1)!! 2l −(2l+1)
φ(r, ϑ) =
P2l (cos ϑ)
R r
4πϵ0 2l
l!
l=0

2) caso en que r < R
Aquí el potencial será de la forma
φ(r, ϑ) =

∞
)
l=0

Cl rl + Dl r−(l+1) Pl (cos ϑ)

Se requiere que el potencial sea finito, luego Dl = 0 para todo l = 0, 1, 2... la condición de
contorno en el eje z, z > 0 entrega
φ(r, 0) =

∞
)

Cl rl =

l=0

Q
4πϵ0 R (1 + (r/R)2 )−1/2

Como r/R < 1, está garantizada la convergencia de la serie de potencias de
∞
)

1 + (r/R)2

3−1/2

∞
Q 1)
(2l − 1)!! r2l
Cl r =
(−1)l
4πϵ0 R l=0
2l l! R2l
l=0

∞
)

l

∞

Q )
(2l − 1)!! r2l
Cl r =
(−1)l
4πϵ0 l=0
2l l! R2l+1
l=0
l

de aquí es inmediato que Cl = 0 para l impar
∞
)

∞

(2l − 1)!! r2l
Q )
C2l r =
(−1)l
4πϵ0 l=0
2l l! R2l+1
l=0
2l

C2l =

(2l − 1)!!
Q
(−1)l l 2l+1
4πϵ0
2 l!R

Finalmente, el potencial está dado por
∞
)
Q
(2l − 1)!!
φ(r, ϑ) =
(−1)l l 2l+1 rl P2l (cos ϑ), r < R
4πϵ0
2 l!R
l=0

---

### Página 251

φ(r, ϑ) =

∞
)
Q (−1)l (2l − 1)!! 2l −(2l+1)
P2l (cos ϑ), r > R
R r
l
4πϵ
l!
l=0

Fig. 9.2: La figura muestra la solución para r > R, tomando 40 términos

Fig. 9.3: La figura muestra la solución para r < R

---

### Página 252

Parte III
El campo en medios materiales

---

### Página 253

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 254

#### Capítulo 10
Dieléctricos
10.1.

El campo en medios Dieléctricos

Aquí comenzamos a discutir otra de las propiedades interesantes de la materia bajo la
influencia de un campo eléctrico. Anteriormente consideramos el comportamiento de los conductores, en donde hay cargas libres para moverse en respuesta a un campo eléctrico de forma de
cancelar el campo en el interior del conductor. Ahora discutiremos qué sucede con los aislantes,
materiales que no conducen electricidad. Uno podría creer primeramente que no debería haber
efecto alguno, sin embargo, usando un condensador de placas paralelas, Faraday descubrió que
ésto no es así. Sus experimentos mostraron que la capacidad aumenta en un factor κ que depende únicamente de la naturaleza del material asilante. Éstos materiales también son llamados
dieléctricos, el factor κ es una propiedad del dieléctrico (y se llama constante dieléctrica). La
constante dieléctrica del vacío es, por supuesto, 1. A continuación se derivará el comportamiento de un dieléctrico en un campo externo y se aplicará al cálculo de capacidades con dieléctricos.
Todos los medios materiales se componen de moléculas, las que a su vez se componen de
entes cargados (núcleos atómicos y electrones), y las moléculas de los dieléctricos son, de hecho, afectadas por la prescencia de un campo eléctrico externo. El campo eléctrico produce
una fuerza que se ejerce sobre cada partícula cargada, empujando las partículas positivas en
la dirección del campo, y las negativas en sentido opuesto, de modo que las partes positivas
y negativas de cada molécula se desplazan de sus posiciones de equilibrio, sin embargo estas
cargas moleculares no están libres para moverse muy lejos o ser extraídas del material (lo que
sí ocurre en conductores).
El efecto total, desde el punto de vista macroscópico, se visualiza como un desplazamiento
de toda la carga positiva en el dieléctrico en relación a la carga negativa (Se produce una
colección de dipolos!). A esto se le llama polarización. Existen 2 tipos de dieléctricos, unos
son los dieléctricos polares, que tienen momentos dipolares permanentes. Un ejemplo de este
tipo de dieléctrico es el agua.

---

### Página 255

La orientación de las moléculas polares ante la ausencia de un campo es totalmente aleatoria.
⃗ 0 es aplicado, un torque causa que las moléculas se alinien en la dirección
Cuando un campo E
⃗ 0 . (ver último problema de ayudantía 9)
de E
El otro tipo de dieléctrico son los no polares, que no poseen momentos dipolares permanentes, pero que de igual forma se polarizan ante un campo eléctrico externo. Las moleculas
polarizadas son como dipolos y se alinean en la dirección del campo.

⃗ 0 . En
La figura ilustra la orientacion de las moléculas no polares con y sin campo externo E
ambos tipos de dieléctricos, ante la prescencia de un campo eléctrico externo, se produce una
polarización. Un dieléctrico polarizado, aun cuando sea eléctricamente neutro en promedio,
produce un campo eléctrico en los puntos exteriores e interiores al dieléctrico.

10.1.1.

Polarización

Vimos que si un medio se polariza, se efectúa una separación de cargas positivas y negativas,
y un elemento de volumen se caracterizará entonces por un momento dipolar eléctrico, ∆⃗p. Se
define P⃗ , el momento dipolar eléctrico por unidad de volumen
∆⃗p
P⃗ =
∆v
Estrictamente, P⃗ debe definirse como el límite de esta cantidad a medida que ∆v se hace muy
pequeño desde el punto de vista macroscópico. De esta forma, P⃗ se convierte en una función
puntual P⃗ (x, y, z), llamada Polarización del medio (Es, de hecho, un campo vectorial). Sus
dimensiones son carga por unidad de área.

10.1.2.

Campo de un Medio Dieléctrico

Consideremos un pedazo finito de dieléctrico polarizado, es decir, que se caracterize en
cada punto ⃗x′ por su polarización P⃗ (⃗x‘). La polarización da origen a un campo eléctrico. Para
encontrarlo, encontremos primero el potencial en un punto P .

---

### Página 256

Cada elemento de volumen d3 x′ se comporta como un dipolo microscópico, y entonces se caracteriza por un momento dipolar ∆⃗p(⃗x′ ) = P⃗ (⃗x′ )d3 x′ , y como la distancia entre ⃗x y d3 x′ es
grande comparada con las dimensiones de d3 x′ , el potencial en ⃗x será
∆⃗p(⃗x′ ) · (⃗x − ⃗x′ )
P (⃗x′ ) · (⃗x − ⃗x′ )d3 x′
=
dφ(⃗x) =
4πϵ0 |⃗x − ⃗x′ |3
4πϵ0 |⃗x − ⃗x′ |3
(Recordar el potencial de un dipolo!). El potencial en el punto ⃗x se obtiene sumando las contribuciones de todas las partes del dieléctrico, luego
φ(⃗x) =
4πϵ0

d3 x′ P⃗ (⃗x′ ) · (⃗x − ⃗x′ )
|⃗x − ⃗x′ |3
V

˚

Esta integral puede evaluarse directamente si se conoce la forma funcional de P⃗ (⃗x′ ). En la
práctica eso no se hace, resulta ventajoso desarrollar aún más esta expresión. Usando la ya
conocida identidad
⃗′
∇

⃗x − ⃗x′
=
|⃗x − ⃗x′ |
|⃗x − ⃗x′ |3

El potencial queda
φ(⃗x) =
4πϵ0

˚

⃗′
d3 x′ P⃗ (⃗x′ ) · ∇

V

|⃗x − ⃗x′ |

El siguiente paso consiste en utilizar la siguiente identidad
⃗ ′ · F⃗ + F⃗ · ∇
⃗ ′f
⃗ ′ · (f F⃗ ) = f ∇
∇
Donde f es cualquier función escalar y F⃗ un campo vectorial. Con esto, si utilizamos f =

y F⃗ = P⃗ (⃗x′ )
|⃗
x−⃗
x′ |

⃗′
P⃗ (⃗x′ ) · ∇

⃗ ′
⃗ ′ · P (⃗x ) −
⃗ ′ · P⃗ (⃗x′ )
∇
=
∇
′
′
′
|⃗x − ⃗x |
|⃗x − ⃗x | |⃗x − ⃗x |

Con esto
φ(⃗x) =
4πϵ0

˚
P⃗ (⃗x′ )
⃗ ′ · P⃗ (⃗x′ )
d x∇ ·
d3 x′
−
∇
′
′|
|⃗
x
−
⃗
x
|
4πϵ
|⃗
x
−
⃗
x
V
V

˚

3 ′⃗ ′

La primera integral puede transformarse en una integral sobre una superficie cerrada mediante el teorema de la divergencia, obteniendo

---

### Página 257

ˆˆ
˚
1 ✞☎ ⃗ ′
P⃗ (⃗x′ )
3 ′
⃗ ′ · P⃗ (⃗x′ )
φ(⃗x) =
x)·
d
x
−
∇
✝ ✆dS(⃗
′|
4πϵ0 S
|⃗x − ⃗x′ | 4πϵ0
|⃗
x
−
⃗
x
V
O, equivalentemente
ˆˆ
˚
⃗ ′ ⃗ x′ )
⃗ x′ ) · n̂(⃗x′ )
1 ✞☎
′ P (⃗
3 ′ −∇ · P (⃗
+
φ(⃗x) =
x)
d
x
✝ ✆dS(⃗
4πϵ0 S
|⃗x − ⃗x′ |
4πϵ0
|⃗x − ⃗x′ |
V
⃗ · P⃗ (⃗x) son dos funciones escalares obtenidas a partir de la
Las cantidades P⃗ (⃗x) · n̂(⃗x) y −∇
polarización P⃗ (⃗x). Es conveniente asignar a estas cantidades símbolos especiales, y como tienen
dimensiones de carga por unidad de área y carga por unidad de volumen, respectivamente,
escribiremos
σ(⃗x) = P⃗ (⃗x) · n̂(⃗x)
⃗ · P⃗ (⃗x)
ρ(⃗x) = −∇
Y llamaremos a σ y ρ densidades de carga de polarización. La densidad superficial
de carga de polarización está dada por la componente de polarización normal a la superficie,
y la densidad volumétrica de carga de polarización es una medida de la no uniformidad de la
polarización dentro del material.
En resumen, el potencial debido al material dieléctrico es, finalmente
ˆˆ
˚
1 ✞☎
σ(⃗x′ )
x′ )
′
3 ′ ρ(⃗
φ(⃗x) =
x)
d
x
+
✝ ✆dS(⃗
4πϵ0 S
|⃗x − ⃗x′ | 4πϵ0
|⃗x − ⃗x′ |
V
De esta expresión es evidente que proviene de una distribución de carga. En otras palabras,
el material dieléctrico se ha sustituido por una distribución adecuada de carga de polarización.
⃗ x) = −∇φ(⃗
⃗ x)
El campo eléctrico se obtiene usando el hecho E(⃗
ˆˆ
˚
1 ✞☎
x′ )(⃗x − ⃗x′ )
x′ )(⃗x − ⃗x′ )
′ σ(⃗
3 ′ ρ(⃗
⃗
E(⃗x) =
x)
+
d
x
✝ ✆dS(⃗
4πϵ0 S
|⃗x − ⃗x′ |3
4πϵ0
|⃗x − ⃗x′ |3
V
Notemos que la carga de polarización total de un cuerpo dieléctrico es
˚
ˆˆ
✞☎
3 ′
′ ⃗
′
⃗
Qp =
d x (−∇ · P (⃗x )) + ✝ ✆ dS(⃗x′ )P⃗ (⃗x′ ) · n̂(⃗x′ )
V

S(V )

Utilizando el teorema de la divergencia, es evidente que Qp = 0, (como debe ser!) Esto
concuerda con que un dieléctrico, como un todo, es eléctricamente neutro.

10.2.

Ley de Gauss en un Dieléctrico, Desplazamiento
Eléctrico

Es sabido que una de las leyes fundamentales de la electrostática es la ley de Gauss. Esta
ley dice que el flujo eléctrico a través de cualquier superficie cerrada es proporcional a la carga
total encerrada por la superficie. Al aplicar la ley de Gauss a una región que contiene cargas

---

### Página 258

libres dentro de un dieléctrico, hay que tener cuidado en incluír todas las cargas dentro de la
superficie gaussiana, tanto la carga de polarización como la carga libre

Consideremos una superficie S cerrada imaginaria colocada dentro de un medio dieléctrico.
Consideremos cierta cantidad de carga libre Q, contenida en el volumen limitado por S ′ . La ley
de Gauss entrega
ˆˆ
˚
ˆˆ
Q
✞
☎
✞☎ ⃗ ′
′
′
′
⃗ x)= +
d3 x′ ρ(⃗x′ )
x )σ(⃗x ) +
x ) · E(⃗
✝ ✆ dS(⃗
✝ ✆dS(⃗
ϵ
ϵ
ϵ
′
S
S
ˆˆ
˚
ˆˆ
Q
1 ✞☎ ⃗ ′ ⃗ ′
✞☎ ⃗ ′
′
⃗
⃗ ′ P⃗ (⃗x′ )
x ) · E(⃗x ) = +
d3 x′ ∇
x ) · P (⃗x ) −
✝ ✆ dS(⃗
✝ ✆dS(⃗
ϵ
ϵ
ϵ
′
S
S
ˆˆ
ˆˆ
1 ✞☎ ⃗ ′ ⃗ ′
1 ✞☎
Q
⃗ x′ ) · P⃗ (⃗x′ )
= +
x ) · P (⃗x ) −
✝ ✆ dS(⃗
✝ ✆ dS(⃗
ϵ0 ϵ0 S ′
ϵ0 S+S ′
Así

✞☎ ⃗ ′
☎ ⃗ ′
⃗ x′ ) = Q − 1 ✞
x ) · E(⃗
x ) · P⃗ (⃗x′ )
✝ ✆dS(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

ϵ0

ˆˆ

S

Equivalentemente
ˆˆ

ˆˆ

☎ ⃗ ′
✞☎ ⃗ ′
⃗ x′ ) = Q − ✞
ϵ0 ✝ ✆dS(⃗
x ) · E(⃗
x ) · P⃗ (⃗x′ )
✝ ✆dS(⃗
S

S

ˆˆ

✞☎ ⃗ ′
x)·
✝ ✆dS(⃗
S

!

"
⃗ x′ ) + P⃗ (⃗x′ ) = Q
ϵ0 E(⃗

Se define el Desplazamiento eléctrico como
⃗ x) + P⃗ (⃗x)
⃗ x) = ϵ0 E(⃗
D(⃗
⃗ queda
La ley de Gauss, en términos de D
˚
ˆˆ
✞☎ ⃗ ′
′
⃗
x ) · D(⃗x ) = Q =
✝ ✆dS(⃗
S

d3 x′ ρlibre (⃗x′ )

S(V )

Esta es la Ley de Gauss generalizada a un dieléctrico, notar que Q representa únicamente la carga libre, es decir, toda la información sobre la polarización del medio se encuen⃗ x′ ). Notar que si no hay dieléctrico (espacio vacío), se tiene P⃗ (⃗x)= 0,
tra contenida en D(⃗
⃗ x) = ϵ0 E(⃗
⃗ x) y
D(⃗
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = Q
ϵ0 ✝ ✆dS(⃗
x ) · E(⃗
S

que es la ley de Gauss usual para el vacío.

---

### Página 259

10.3.

Forma diferencial de la Ley de Gauss General

A partir de la ley de Gauss
ˆˆ

✞☎ ⃗ ′
⃗ x′ ) =
x ) · D(⃗
✝ ✆dS(⃗
S

˚

d3 x′ ρ(⃗x′ )

V (S)

Aquí, ρ(⃗x′ ) representa la densidad volumétrica de carga libre. Utilizando el teorema de la
divergencia
˚
¨
3 ′⃗
′
⃗ x)=
d x ∇ · D(⃗
d3 x′ ρ(⃗x′ )
V (S)

V (S)

De donde se obtiene la forma diferencial de la ley de Gauss general
⃗ · D(⃗
⃗ x′ ) = ρ(⃗x′ )
∇
Esta es la primera ecuación de Maxwell reescrita para un medio material. Notar que la
⃗ tiene la ventaja de conservar como fuentes únicamente las cargas lidefinición del vector D
⃗
bres. El efecto de las cargas de polarización están contenidas en D.

10.4.

Susceptibilidad Eléctrica y constante Dieléctrica

⃗ x) se anula. Como éste es
Para la mayoría de los materiales, P⃗ (⃗x) se anula cuando E(⃗
el comportamiento más común, nos limitaremos a los materiales de este tipo. Además, si el
material es isotrópico, la polarización deberá tener el mismo sentido que el campo eléctrico que
la provoca. Esto se resume en
⃗ x)
P⃗ (⃗x) = χ(E)E(⃗
Donde la cantidad escalar χ(E) se llama susceptibilidad eléctrica del material. Así, una
⃗ x) en medios isotrópicos sería
expresión para D(⃗
⃗ x) = ϵ(E)E(⃗
⃗ x)
⃗ x) = (ϵ0 + χ(E))E(⃗
D(⃗
Donde ϵ(E) = ϵ0 + χ(E) es la permitividad del material. Experimentalmente χ y ϵ son
independientes del campo eléctrico para campos no muy intensos. En otras palabras, χ y ϵ pasan
a ser constantes características del material. Materiales de este tipo se llaman dieléctricos
lineales, y se tiene
⃗ x)
P⃗ (⃗x) = χE(⃗
⃗ x) = ϵE(⃗
⃗ x)
D(⃗
Es más conveniente trabajar con una cantidad adimensional, κ, definida por
κ=

ϵ
= ϵr
ϵ0

Esta constante se llama constante dieléctrica, de manera que
⃗ x) = ϵE(⃗
⃗ x) = ϵ0 κE(⃗
⃗ x)
D(⃗

---

### Página 260

Notar que κ es siempre mayor que 1, excepto en el vacío, donde κ = 1. La primera ecuación
de Maxwell en este tipo de medios queda
⃗ · E(⃗x) = ρ(⃗x) = ρ(⃗x)
∇
ϵ
κϵ0
Eso significa que en un medio dieléctrico, el campo eléctrico es debilitado por un
factor κ.

10.5.

Condiciones de borde en la frontera

Las condiciones que deben satisfacer el campo eléctrico en una zona interfacial que separa
dos madios dieléctricos se deducen a partir de las leyes diferenciales
⃗ · D(⃗
⃗ x) = ρ(⃗x)
∇
⃗ × E(⃗
⃗ x) = 0
∇
En cualquier zona interfacial entre dos medios se puede construír una superficie cilíndrica
como se muestra en la figura

Integrando la ley de Gauss general sobre el volumen limitado por el cilindro se obtiene
˚
˚
3 ⃗
⃗
d x∇ · D(⃗x) =
d3 xρ(⃗x)
V

V

✞☎
✝✆

¨

ˆˆ

⃗ x) · D(⃗
⃗ x) =
dS(⃗

V (S)

d3 xρ(⃗x)

V

si h → 0, entonces
(D1n − D2n ) A = σA
donde A es la superficie de las tapas, y σ es la densidad superficial de carga en la frontera que
⃗ x) es discontinua al atravesar
divide a los dos medios. Así, la componente normal del campo D(⃗
una superficie cargada
D1n − D2n = σ

---

### Página 261

o, equivalentemente para medios lineales
ϵ1 E1n − ϵ2 E2n = σ

Ahora veremos que la componente tangencial del campo eléctrico es continua. A partir de
la ecuación
⃗ × E(⃗
⃗ x) = 0
∇
Integremos esta ecuación sobre una superficie plana rectangular como la de la figura

El contorno de S es el camino Γ indicado en la figura. Utilizando el teorema de Stokes
ˆˆ
!
" ˛
✞☎ ⃗
⃗ × E(⃗
⃗ x) = d⃗x · E(⃗
⃗ x) = 0
✝ ✆dS(x̂) · ∇
S

Γ

En el caso en que h1 → 0, h2 → 0

lE1t − lE2t = 0
⃗ x) debe ser continua al atravesar
De aquí se deduce que la componente tangencial de E(⃗
una interfaz entre dos medios
lE1t = lE2t

⃗ x) y D(⃗
⃗ x)
En resumen, al atravesar una interfaz entre dos medios (1 y 2), los campos E(⃗
satisfacen
E1t = E2t
D1n − D2n = σ

---

### Página 262

10.5.1.

Condensadores con Dieléctricos

Un material no conductor, ancho t, área A y constante dieléctrica κ se inserta en el espacio
entre placas de un condensador con distancia d entre placas, carga Q y área A. No es necesario
que el dieléctrico esté en la mitad del espacio entre placas

Para encontrar la capacitancia, calculemos primero la diferencia de potencial entre placas.
Ya se vió que en auscencia de dieléctrico, el campo eléctrico entre las placas está dado por
E0 = ϵσ0 = ϵ0QA , y entonces ED = Ek0 . El potencial se puede encontrar integrando el campo
eléctrico sobre una curva vertical desde la placa superior a la inferior
ˆ −
Q
Q
∆φ = −
dxE = −phi0 + phiD = −E0 (d − t) − ED t = −
(d − t) −
t
Aϵ0
Aϵ0 κ
+
∆φ = −
Con esto se obtiene
C=

Q
(d − t(1 − ))
Aϵ0
κ

Q
ϵ0 A
=
|∆V |
d − t(1 − κ1 )

Notemos algunos límites, por ejemplo cuando t → 0, es decir, cuando el ancho del dieléctrico tiende a cero, se obtiene C = ϵ0 Ad = C0 , que es la capacidad esperada para cuando no hay
dieléctrico.
Cuando κ = 1, nuevamente se obtiene C = ϵ0dA = C0 , ya que al ser κ = 1, el dieléctrico es
simplemente vacío.
En el límite cuando t → d, el espacio está totalmente lleno de dieléctrico, y se tiene
κϵ0 A
= κC0
d
Es decir, un condensador lleno de dieléctrico aumenta su capacidad en el factor κ!
C=

---

### Página 263

Problema
Calcular la capacidad del condensador de la figura

#### Solución
El problema se puede tratar como 2 condensadores en paralelo, uno formado por los dieléctricos
de constante κ1 y κ2 , y el otro formado por dieléctrico de constante κ3 y vacío.
El primer condensador (C1 ), se puede ver como 2 condensadores en serie, llenos de los dieléctricos 1 y 2, así
= ′ + ′′
C1
C1 C1
Con
κ1 ϵ0 S1
C1′ =
d1
C1′′ =

κ2 ϵ0 S1
d2

d1
d2
=
+
C1
κ1 ϵ0 S1 κ2 ϵ0 S1
De donde se obtiene
κ1 κ2 ϵ0 S1
d1 κ2 + d2 κ1
Para el condensador C2 , se procede de manera similar, esto es
C1 =

= ′ + ′′
C2
C2 C2
Donde
C2′ =
C2′′ =

ϵ 0 S2
d1

κ3 ϵ0 S2
d2

Donde se obtiene
κ3 ϵ0 S2
d1 κ3 + d2
Finalmente, como C1 y C2 están en paralelo, la capacidad total será
C2 =

C = C1 + C2 =

κ1 κ2 ϵ0 S1
κ3 ϵ0 S2
+
d1 κ2 + d2 κ1 d1 κ3 + d2

---

### Página 264

Problema
Se tiene un condensador plano de área A en el vacío, y se carga con una batería. El condensador
obtiene una carga Q. Luego, se desconecta de la batería y se llena la mitad del espacio entre
placas con un dieléctrico de permitividad ϵ2 . Calcular
a) la nueva diferencia de potencial entre las placas
b) las densidades superficiales de carga en cada placa
c) las densidades de carga de polarización del dieléctrico

#### Solución
Sea el origen en un punto sobre la placa inferior. Se define el eje z como vertical y positivo
hacia arriba. Si escogemos un camino de integración Γ como una línea recta vertical desde la
placa superior hasta la inferior

podemos obtener la diferencia de potencial entre las placas como
ˆ
ˆ 0
⃗ x) =
⃗ x)
d⃗xE(⃗
φd − φo = V = d⃗x · E(⃗
d

Γ

Despreciando efectos de borde, el campo debe ser uniforme en la región interior, y además
apunta según −k̂. Ojo con la parametrización! se tiene l = d − t, con t = 0...d. De esta forma
dl = −dt y d⃗l = dtk̂ ,luego
ˆ 0
ˆ 0
⃗
d⃗x · E(⃗x) = −E
dt = Ed
V =
d

d

Luego E = Vd

La curva Γ fue escogida de manera arbitraria,y se podría haber escogido en la mitad donde
se encuentra el dieléctrico, sin embargo la diferencia de potencial entre las placas debe ser la
misma para ambos caminos de integración. Lo que esto significa es que el campo eléctrico debe
ser igual tanto en el vacío como en la región con dieléctrico. La única forma de que esto sea
posible es que se distribuyan densidades de carga superficial en los conductores, digamos σ1 y
σ2 no necesariamente iguales entre sí.

---

### Página 265

ahora, sabemos que en la región 1
D1 = ϵ 1 E = ϵ 0

V
d

y para la región 2

V
d
Además, utilizando la ley de Gauss con las superficies S1 y S2 de la figura:
ˆˆ
✞☎ ⃗ ⃗
✝ ✆dS · D1 = D1 S = σ1 S
D2 = ϵ 2 E = ϵ

S

luego

V
d
Equivalente, para la región 2 se obtiene de forma análoga
D1 = σ1 = ϵ0

D2 = σ2 = ϵ

V
d

Además, como la carga Q en la placa superior sólo se distribuye, la ley de continuidad
establece
A
V A
= Q = (ϵ + ϵ0 )
=Q
d 2
de aquí obtenemos la diferencia de potencial entre las placas del condensador
(σ1 + σ2 )

V =

2Qd
A(ϵ + ϵ0 )

Notar que si ϵ = ϵ0 (y entonces el material dieléctrico es el vacío) el potencial es simplemente
el potencial inicial
Q
Qd
=
= Vo
V =
Aϵ0
C
b) Las densidades de carga superficial están dadas por
σ1 = ϵ0
σ2 = ϵ
Notar que
σ1

ϵ0 2Q
V
=
d
A(ϵ + ϵ0 )

ϵ2Q
V
=
d
A(ϵ + ϵ0 )

A
A
+ σ2 = Q

---

### Página 266

c) Calculemos ahora las densidades de polarización. Necesitamos encontrar σP y ρP en el
material dieléctrico. Tenemos que
⃗ · P⃗ = −χ∇
⃗ ·E
⃗
ρP = −∇
Ahora, en todos los puntos en el dieléctrico no hay densidad de carga libre, luego, de la
primera ecuación de Maxwell
⃗ ·D
⃗ =ρ=0
∇
⃗ = ϵE
⃗ →∇
⃗ ·E
⃗ =0
y como D
Esto es válido en todos los puntos interiores al dieléctrico. Con esto
ρP = 0
Ahora, para obtener la densidad de carga superficial, se tiene
σP = P⃗ · n̂
donde n̂ es la normal a la superficie del dieléctrico.
Recordar que
D = ϵE = ϵ0 E + P
Luego
(ϵ − ϵ0 )E = P
Ahora, en la superficie superior del dieléctrico se tiene n̂ = k̂ y
⃗ =−
E
Luego
σP = −

2Q
k̂
A(ϵ + ϵ0 )

2Q
(ϵ − ϵ0 )
A(ϵ + ϵ0 )

Y la densidad en la placa inferior será, simplemente
−σP =

2Q
(ϵ − ϵ0 )
A(ϵ + ϵ0 )

se verifica que la carga total de polarización es cero

---

### Página 267

Problema
Una esfera de radio R con carga libre q está sumergida en un medio dieléctrico homogéneo de
constante κ y de extensión teóricamente infinita. Calcular
a) Los vectores campo eléctrico y polarización a distancia r de la carga puntual
b) La densidad de carga de polarización
#### Solución
⃗ D
⃗ y P⃗ son todos paralelos entre sí en cada punto, y por la simetría esférica,
a) Debido a que E,
la naturaleza radial del campo no cambia por la prescencia del medio dieléctrico. Además, estos
vectores pueden depender sólo de la distancia al centro de la esfera y no de alguna coordenada
angular.
Usando la ley de gauss general, con una superficie esférica de radio r (r > R) concéntrica a la
esfera de carga q
ˆˆ

✞☎ ⃗ ′
⃗ x′ ) = q
x ) · D(⃗
✝ ✆dS(⃗
S

ˆˆ

ˆˆ

✞☎
✞☎
x′ ) = q
✝ ✆dSD(r) = q → D(r) ✝ ✆dS(⃗
S

S

Con lo que
4πr2 D(r) = q
⃗
D(r)
=

q
r̂
4πr2

⃗
El campo eléctrico y la polarización pueden evaluarse con bastante facilidad al conocer D
⃗
⃗
⃗
D(r)
= κϵ0 E(r)
→ E(r)
=
además

q
r̂
4πκϵ0 r2

⃗ x) + P⃗ (⃗x)
⃗ x) = ϵ0 E(⃗
D(⃗
⃗
P⃗ (r) = (ϵ − ϵ0 ) E(r)
=

q
q
q
r̂ − ϵ0
r̂ =
4πr
4πκϵ0 r
4πr2

#

1−
κ

$

r̂ =

q(κ − 1)
P⃗ (r) =
r̂
4πκr2
b) Claramente el dieléctrico ha debilitado la magnitud del campo eléctrico (en comparación
al espacio vacío). El campo eléctrico es originado por toda la carga, la de polarización y la
carga libre. La carga libre es sólo la carga de la esfera q. Sin embargo, la carga de polarización
⃗ · P⃗ (⃗x) y una densidad
se forma de dos contribuciones, una densidad volumétrica ρP (⃗x) = −∇
superficial σP (⃗x) = P⃗ (⃗x)·n̂(⃗x) sobre la superficie del dieléctrico en contacto con la carga puntual.
Es claro que en todos los puntos del dieléctrico
⃗ · E(⃗
⃗ x) = 0
∇
y entonces

⃗ · P⃗ (⃗x) = 0
ρP (⃗x) = −∇

---

### Página 268

Usando que
q(κ − 1)
P⃗ (r) =
r̂
4πκr2
La densidad superficial será
σ = P⃗ · n̂ = P⃗ (R) · −r̂ = −

(κ − 1)q
4πκR2

y la carga superficial es
ˆˆ

✞☎

QS = ✝ ✆dS(⃗x′ )σ(⃗x′ ) = −4πR2
S

QS = −

(κ − 1)q
4πκR2

(κ − 1)q
κ

Notar que la carga total será
(κ − 1)q
q
=
κ
κ
Otra forma de ver como campo eléctrico es menor en un factor κ, la carga se ve debilitada
por este factor de lo que sería si no hubiera un medio dieléctrico.
Q = Qlibre + QS = q −

---

### Página 269

Problema
Considere una cáscara esférica dieléctrica de radio interior a, radio exterior b y permitividad ϵ.
Se coloca una carga puntual q en su centro. Calcule el campo eléctrico en todo el espacio y las
densidades de carga de polarización

#### Solución
Tomando una superficie gaussiana esférica arbitraria de radio r > 0 concentríca con la carga
libre q, se tiene
ˆˆ
✞☎ ⃗ ′
⃗ x′ ) = 4πr2 D(r) = qin = q
x ) · D(⃗
✝ ✆dS(⃗
S

Con esto

q
r̂
4πr2
para todo r > 0. Ahora, podemos obtener el campo eléctrico como sigue. En la región r < a,
se tiene
⃗
D(r)
=

⃗ I (r) =
E

q
r̂
4πϵo r2

⃗ II (r) =
E

q
r̂
4πϵr2

para a < r < b
y para r > b

q
r̂
4πϵo r2
Notar que el campo se debilita en la región interior del cascarón dieléctrico. Ahora,
⃗ III (r) =
E

⃗ · P⃗ (⃗x) = −∇
⃗ · (ϵ − ϵo ) E
⃗r = 0
ρP = −∇

---

### Página 270

Ahora, sea σin la densidad superficial de polarización en la cáscara interior y σext la densidad
superficial de polarización en la cáscara exterior

⃗ II (a) · (−r̂) = −
σin = (ϵ − ϵ0 )E

q(ϵ − ϵ0 )
4πϵa2

⃗ II (b) · (r̂) = q(ϵ − ϵ0 )
σext = (ϵ − ϵ0 )E
4πϵb2
se verifica que la carga total de polarización es cero

---

### Página 271

Problema
Se tiene un condensador esférico de radio interno a y externo b, el cual está lleno de un dieléctrico que tiene una constante dieléctrica κ.¿Cuál es la capacitancia de este condensador? Si el
condensador está cargado con una carga Q, encuentre la energía almacenada en él

#### Solución
Supongamos que el condensador tiene almacenada una carga Q, es decir, la pared r = a
está cargada con carga Q, mientras que la pared r = b se encuentra cargada con carga −Q. Se
puede determinar la capacitancia al determinar la diferencia de potencial entre estas superficies.
Utilizando la ley de Gauss general, con una superficie esférica de radio r, con a ≤ r ≤ b

ˆˆ

✞☎ ⃗
⃗ x) = Q
x) · D(⃗
✝ ✆dS(⃗
S

⃗ x) = D(r)r̂ y entonces
dada la simetría radial, D(⃗
ˆˆ
✞☎ ⃗
⃗ x) = 4πD(r)r2 = Q
x) · D(⃗
✝ ✆dS(⃗
S

de esta forma
⃗ x) = Q r̂, a ≤ r ≤ b
D(⃗
4πr2
Si el dieléctrico es lineal, homogéneo e isotrópico, entonces
⃗ x)
⃗ x) = ϵ0 κE(⃗
D(⃗
donde κ es la constante dieléctrica del material. Luego
⃗ x) =
E(⃗

Q
r̂, a ≤ r ≤ b
4πϵ0 κr2

---

### Página 272

Ahora, la diferencia de potencial entre los extremos del condensador es
ˆ b
⃗ x)
∆V = φ(a) − φ(b) =
d⃗x · E(⃗
a

tomando un camino radial de la forma ⃗x = rr̂, ≤ ar ≤ b, entonces d⃗x = drr̂
#
$
ˆ b
drQ
Q
1 1
∆V =
=
−
4πϵ0 κ a b
a 4πϵ0 κr

Finalmente

4πϵ0 κ(b − a)
Q
=
∆V
ab
Es decir, es κ veces la capacidad de un condensador esférico en vacío
C=

C = κC0 > C0

---

### Página 273

Problema
Considere una espera conductora de radio interior a y radio exterior c. El espacio entre las 2
superficies es llenado con 2 dieléctricos distintos, de manera que la constante dieléctrica es κ1
entre a y b, y κ2 entre b y c. Determine la capacitancia del sistema

#### Solución
Para encontrar la capacitancia, podemos suponer que el condensador se encuentra cargado con
una carga Q, en este estado, habrá una cierta diferencia de potencial entre r = a y r = c. La
relación entre esta diferencial de potencial y la carga almacenada nos permitirá encontrar la
capacidad

Para encontrar ∆V = φ(a) − φ(c) necesitamos determinar el campo eléctrico en la región
Ω : a ≤ r ≤ c. Para ello, utilizamos la ley de Gauss general, para una superficie esférica de
radio r contenida en Ω
ˆˆ
✞☎ ⃗
⃗ x) = 4πr2 D(r)
x) · D(⃗
✝ ✆dS(⃗
S

esto último dada la clara simetría esférica del problema. Por la ley de Gauss
ˆˆ
✞☎ ⃗
⃗ x) = Q
x) · D(⃗
✝ ✆dS(⃗
S

De aquí es posible obtener el campo de desplazamiento eléctrico en Ω
Q
⃗
r̂, a ≤ r ≤ c
D(r)
=
4πr2
Suponiendo que los dieléctricos involucrados son lineales, homogéneos e isotrópicos, se tendrá
⃗ x)
⃗ x) = ϵ0 κE(⃗
D(⃗

donde κ es la constante dieléctrica.

---

### Página 274

Así, para la región I (a ≤ r ≤ b)
⃗ x) = Q r̂, a ≤ r ≤ b
ϵ0 κ1 E(⃗
4πr2
Despejando
⃗ x) =
E(⃗

Q
r̂, a ≤ r ≤ b
4πϵ0 κ1 r2

Análogamente, para la región II (b ≤ r ≤ c)
⃗ x) =
E(⃗

Q
r̂, b ≤ r ≤ c
4πϵ0 κ2 r2

Con esto
∆V = φ(a) − φ(c) =

ˆ c

⃗ x)
d⃗x · E(⃗

a

tomando un camino radial de la forma ⃗x = rr̂ (para algun valor del ángulo ϑ), entonces
d⃗x = drr̂
ˆ b
ˆ c
drQ
drQ
∆V =
+
a 4πϵ0 κ1 r
b 4πϵ0 κ2 r
Luego
Q
= 4πϵ0
C=
∆V

#

ab
κ2 bc
+
κ1 (b − a) c − b

$

Otra forma de resolver el sistema es notando que el condensador equivale a dos condensadores esféricos en serie. Recordando que la capacidad equivalente para un condensador esférico de radio interior r1 y radio exterior r2 , lleno de un dieléctrico lineal de constante κ está dado
por
#
$
r1 r 2
C = 4πϵ0 k
r2 − r 1
Con lo que la capacidad equivalente del sistema está dada por

(b − a)
(c − b)
κ2 c(b − a) + κ1 a(c − b)
=
+
=
C
4πϵ0 κ1 ab 4πϵ0 κ2 bc
4πϵ0 κ1 κ2 abc
Así
C=

4πϵ0 k1 k2 abc
k2 c(b − a) + k1 a(c − b)

que es el mismo resultado obtenido anteriormente

---

### Página 275

Problema
Se tiene un condensador plano con placas cuadradas de largo a, distancia d entre placas, y una
carga total Q. Calcular la fuerza que se ejerce sobre un material dieléctrico cuando se encuentra
a una distancia x del punto O

#### Solución
La energía potencial asociada a esta configuración es
1 Q2
2 C(x)
Notar que es función de x, puesto que la capacitad total del condensador es función de x.
El sistema se puede ver como dos condensadores en paralelo
U (x) =

Ceq = C1 + C2 =
Ceq =

ϵ0 ax κϵ0 a(a − x)
+
d
d

ϵ0 a(x + κ(a − x))
d

Con esto, la energía potencial eléctrica almacenada es
dQ2
U (x) =
2 ϵ0 a(x + κ(a − x))
Y la fuerza que se ejerce sobre el dieléctrico será
Fx î = −

dU
î
dx

(1 − k)
Q2 d
F⃗x =
î
2ϵ0 a (x + k(a − x)2 )
Notar que (1 − k) < 0, es decir, la fuerza apunta según - . Esto significa que la placa
dieléctrica es atraída hacia el interior del condensador.

---

### Página 276

Problema
Un condensador cilíndrico de altura l y cuyos conductores tienen radios a y b (b > a), está cargado con una carga Q, es decir, una armadura tiene carga +Q y la otra −Q. Entre ellas existe
vacío. La armadura es un cilíndro metálico macizo.
Este dispositivo se sumerge en un líquido dieléctrico de densidad constante ρ y permitividad ϵ,
a una profundidad h.
Determinar la altura x que sube el nivel del líquido que queda dentro del condensador, en
relación al líquido externo (basta llegar a la ecuación correspondiente).

#### Solución
La diferencia de nivel ∆h estará dada por el equilibrio entre la fuerza eléctrica sobre el líquido
y su peso. Como la carga es constante, entonces
U=

1 Q2
2 C(x)

La fuerza electrostática es
∂U
î
∂x
Con C(x) la capacidad del condensador cuando el agua está a una altura x.
De esta forma,el problema se traduce en determinar la capacidad del condensador en función
de la altura x.
Fx î = −

La figura muestra que el condensador puede considerarse como dos condensadores conectados
en paralelo, uno de altura l − x y otro de altura x. La capacidad total será la suma de las
capacidades C1 , C2 .
Podemos hacer esta suposición (equivalente con 2 condensadores en paralelo) si despreciamos
los efectos de borde y la deformación del campo eléctrico cerca de la superficie del líquido.
Para calcular la capacidad del condensador de altura x, supongamos que hay una carga
q2 distribuida en el conductor interno. Así, utilizando un cilindro como superficie de gauss de
radio r, concéntrico al conductor interno y contenido en la región con dieléctrico, se tiene

---

### Página 277

ˆˆ

✞☎ ⃗ ′
⃗ x′ ) = q2
x ) · D(⃗
✝ ✆dS(⃗

⃗
Si D(r)
= D(r)r̂, se tiene
⃗
D(r)
=

q2
r̂
2πrx

⃗
E(r)
=

q2
r̂
2πrxϵ

De donde

Ahora podemos obtener el potencial entre los conductores como
# $
ˆ b
q
b
⃗ · d⃗r =
∆V =
E
ln
2πϵx
a
a
Con lo que la capacidad para este condensador será
C2 =

2πϵx
% &
ln ab

Análogamente se obtiene la capacidad para el condensador superior, que estará dada por
C1 =

2πϵ0 (l − x)
% &
ln ab

La capacidad total del sistema será la suma de ambas
C = C1 + C2 =
Y la energía eléctrica será
U (x) =

2π
% & (ϵx + ϵ0 (l − x))
ln ab

1 Q2 ln(b/a)
4π x(ϵ − ϵ0 ) + ϵ0 l

Derivando se obtiene la fuerza que tiende a subir el agua
Fx î = −

dU
1 Q2 ln(b/a)(ϵ − ϵo )
î
î =
dx
4π (x(ϵ − ϵ0 ) + ϵ0 l)2

Y el peso del líquido que es elevado una altura ∆h es
W = (x − h)π(b2 − a2 )ρ
Finalmente la ecuación para determinar x es
(x − h)π(b2 − a2 )ρ =

1 Q2 ln(b/a)(ϵ0 − ϵ)
4π (x(ϵ − ϵ0 ) + ϵ0 l)2

---

### Página 278

Problema
Dos esferas concéntricas conductoras de radio interior a y exterior b, respectivamente, poseen
cargas ±Q (como se muestra en la figura). La mitad del espacio entre ellas se llena con un
dieléctrico ( de constante dieléctrica ϵ/ϵ0 )

a) Encuentre el campo eléctrico entre las esferas
b) Calcule la densidad de carga libre superficial en la esfera interior
c) Calcule la densidad de carga de polarización inducida en la superficie del dieléctrico en r = a
#### Solución
a) Sea S una esfera de radio r concéntrica a ambas esferas conductoras, con a < r < b. De la
ley de Gauss general
ˆˆ
✞☎ ⃗
⃗ x) = Q
x) · D(⃗
✝ ✆dS(⃗
S

De la simetria del problema, se deduce una dependencia y dirección radial para el campo
de desplazamiento eléctrico (y también para el campo eléctrico)
⃗ x) = D(r)r̂
D(⃗
Sean además S1 y S2 los hemisferios dados por
S1 = {⃗x ∈ S/0 ≤ ϕ ≤ π}
S2 = {⃗x ∈ S/π ≤ ϕ ≤ 2π}
'

Notar que S1 S2 = S
¨
ˆˆ
¨
✞☎ ⃗
⃗ x) · D(⃗
⃗ x) +
⃗ x) · D(⃗
⃗ x) = Q
⃗ x) =
dS(⃗
dS(⃗
x) · D(⃗
✝ ✆dS(⃗
S

ˆˆ

✞☎ ⃗
⃗ x) =
x) · D(⃗
✝ ✆dS(⃗
S

S1

¨

S2

⃗ x) +
⃗ x) · ϵ0 κE(⃗
dS(⃗

S1

¨

⃗ x) = 2πrE(r)ϵ0 (1 + κ)
⃗ x) · ϵ0 E(⃗
dS(⃗

S2

donde κ es la constante dieléctrica de la región asociada al hemisferio S1 , es decir
κ=

ϵ
ϵ0

Así
⃗ x) =
E(⃗

2Q
4πϵ0 r2 (1 + ϵ/ϵ0 )

r̂, a ≤ r ≤ b

---

### Página 279

b) Para encontrar la densidad de carga libre en la esfera r = a, utilizamos que
⃗ x) = σ(⃗x) , ∀⃗x ∈ Sa : {r = a}
D(⃗
ϵ(⃗x)

Así
σ1 = ϵ0 E(a) =

Qϵ0
2πa (ϵ + ϵ0 )

σ2 = ϵE(a) =

Qϵ
2πa2 (ϵ + ϵ0 )

c) Para encontrar la densidad de carga inducida en la superficie de dieléctrico con r = a,
utilizamos la relación
⃗ x) + P⃗ (⃗x) = ϵE(⃗
⃗ x)
⃗ x) = ϵ0 E(⃗
D(⃗
Así, el vector polarización está dado por
⃗ x)
P⃗ (⃗x) = (ϵ − ϵ0 ) E(⃗
La densidad de carga inducida de polarización en la superficie del dieléctrico con r = a es
(
(
⃗
σP = P · n̂(
⃗
x∈Sa

donde n̂ es la normal a la superficie Sa que limita al dieléctrico, es decir n̂ = −r̂
(
(
σP = − (ϵ − ϵ0 ) E(r)(
r=a

σP =

#

ϵ0 − ϵ
ϵ0 + ϵ

$

Q
2πa2

---

### Página 280

Problema
Un cascarón esférico macizo (radio interno a y externo b) está hecho de un material tal que la
polarización en su interior está dada por P⃗ (r) = kr r̂, donde k es una constante arbitraria y r la
distancia al centro. Note que no hay carga libre en este problema. Encuentre de dos maneras
distintas el campo eléctrico en todo el espacio
#### Solución
Una forma natural de resolver este problema consiste en encontrar las densidades de carga de
polarización, es decir , ρpol y σpol

La divergencia en coordenadas esféricas para una función radial de la forma f⃗ = f (r)r̂ es

En este caso

%
&
⃗ · f⃗ = 1 ∂ r2 f (r)
∇
r ∂r
#
$
∂
k
⃗ · P⃗ = −
r
ρP = −∇
r2 ∂r
r

k
ρP = − 2 , r ∈ (a, b)
r
Falta obtener además las densidades superficiales de polarización en r = a y r = b. Para
ello utilizamos que
σP = P⃗ · n̂
donde n̂ apunta hacia el exterior de la región de dieléctrico. Para la superficie r = a se tiene

en este caso, n̂ = −r̂, y entonces
(
(
σP (

r=a

=

k
k
r̂ · (−r̂) = −
a
a

---

### Página 281

En r = b, la normal exterior a la región de dieléctrico coincide con n̂ = r̂, de forma que
k
k
r̂ · r̂ =
b
b
r=b
Dividimos el espacio en dos regiones, dadas por {I : a < r < b}, {II : b < r}. Tomando una
superficie esférica S de radio r tal que r > b, e integrando el flujo del campo eléctrico a través
de ella, se tendrá por ley de Gauss
ˆˆ
✞☎ ⃗
⃗ x) = Qin = 4πr2 E(r)
x) · E(⃗
✝ ✆dS(⃗
ϵ0
S
(
(
σP (

=

donde se ha utilizado la clara simetría radial del problema. La carga encerrada por S está dada por
˚
Qin = σa 4πa + σb 4πb +
d3 xρP (⃗x)
V (S)

La integral de la densidad volumétrica de carga de polarización es como sigue
#
$
˚
ˆ 2π
ˆ π
ˆ b
−k
d xρP (⃗x) =
dϕ
dϑ sin ϑ
drr
= −4πk (b − a)
r2
V (S)
a
Entonces
k
k
Qin = − 4πa2 + 4πb2 − 4πb (b − a) = 0
a
b
(Resultado totalmente conocido a estas alturas, pues un dieléctrico es eléctricamente neutro). De esta forma, el campo eléctrico en la región II es nulo
⃗ x) = ⃗0, ∀⃗x ∈ II
E(⃗
Para la región I, nuevamente utilizando la ley de Gauss con una superficie esférica de radio
r, ahora con a < r < b
ˆˆ
✞☎ ⃗
⃗ x) = 4πr2 E(r) = Qin
x) · E(⃗
✝ ✆dS(⃗
ϵ0
S
donde ahora la carga encerrada por S es
#
$
ˆ 2π
ˆ π
ˆ b
−k
Qin = σa 4πa +
dϕ
dϑ sin ϑ
drr
r2
a
Qin = −4πka + 4πk (a − r) = −4πkr
Luego
4πr2 E(r) = −

4πkr
ϵ0

⃗ x) = − k r̂, a < r < b
E(⃗
ϵ0 r
⃗ x) = ⃗0 si r < a
Es claro, por ley de Gauss, que E(⃗

---

### Página 282

Otra forma de resolver este problema, es utilizando la ley de Gauss para el vector desplazamiento eléctrico. Utilizando una superficie S (cualquiera) contenida en la región II, se tiene
ˆˆ
✞☎ ⃗
⃗ x) = Qlibre
x) · D(⃗
✝ ✆dS(⃗
S

donde Qlibre representa la carga libre encerrada por S. En este caso, Qlibre = 0 y entonces,
por continuidad
⃗ x) = ⃗0, ∀x ∈ II
D(⃗
Además, en la región II (vacío), la polarización es nula, P⃗ (⃗x) = ⃗0, ∀x ∈ II. Utilizando
además
⃗ x) = ϵ0 E(⃗
⃗ x) + P⃗ (⃗x) = ⃗0 → E(⃗
⃗ x) = ⃗0, ∀x ∈ II
D(⃗

⃗ es nulo
Para la región I, se obtiene nuevamente que el campo D
ˆˆ
✞☎ ⃗
⃗ x) = ⃗0, ∀S ∈ I
x) · D(⃗
✝ ✆dS(⃗
S

⃗ x) = ⃗0, ∀⃗x ∈ I
D(⃗
entonces

⃗ x) + P⃗ (⃗x) = ⃗0
ϵ0 E(⃗
⃗ x) = − 1 P⃗ (⃗x) = − k r̂
E(⃗
ϵ0
ϵ0 r

⃗ x) = ⃗0 para r < a por la misma razón ( D(⃗
⃗ x) = P⃗ (⃗x) = ⃗0 en r < a)
y, por supuesto, E(⃗

---

### Página 283

Problema
Un cilindro conductor hueco sin espesor, de radio r1 , y largo l, lleva una carga q uniformemente
distribuída. Alrededor de él, otro cilindro conductor hueco sin espesor, coaxial con el anterior,
de radio r2 y mismo largo l, tal como indicado en la figura, lleva una carga -q, también uniformemente distribuída. Se llena la región entre los dos cilindros con un material cuya constante
dieléctrica es función de la distancia al eje de los cilindros, κ = κ(r). Considere l mucho mayor
que r1 y r2

a) Encuentre una expresión para κ(r) que lleva un campo electrostático radial independiente
de la distancia al eje
b) Calcule la capacidad del condensador cilíndrico correspondiente
c) Calcule la densidad superficial de cargas de polarización en la superficie del material dieléctrico a r = r1 y r = r2 , para el κ(r) calculado en el ítem a)
⃗ ·A
⃗ = 1 ∂ (rAr ), calcular la densidad
d) Considerando que, en coordenadas cilíndricas , ∇
r ∂r
volumétrica de cargas de polarización en el dieléctrico
e) Calcular la cantidad total de cargas de polarización, incluyéndose cargas en la superficie y
en el volumen del dieléctrico
f) Calcule la energía potencial electrostática almacenada en el condensador
g) Suponiendo que uno puede sacar el material dieléctrico de entre r1 y r2 deslizándolo fácilmente sin roce, a lo largo del eje del sistema, calcule el trabajo necesario para remover el
dieléctrico de entre las placas del condesador
#### Solución
Para obtener el campo electrostático en el interior, utilizamos la ley de Gauss general, con una
superficie cilíndrica de radio r, con r1 < r < r2 y largo l

⃗ es de la forma D
⃗ = D(r)r̂, con esto
Por simetría, es evidente que D
ˆˆ
ˆˆ
✞☎
✞☎ ⃗ ′
′
⃗
x ) · D(⃗x ) = ✝ ✆dS(⃗x′ )r̂ · D(r)r̂ = q
✝ ✆dS(⃗
S

S

D(r)2πrlD = q
Así
⃗ =
D

q
r̂
2πrl

---

### Página 284

⃗ se relaciona con E
⃗ según
además D
⃗ x) = ϵE(⃗
⃗ x) = κ(r)ϵ0 E(⃗
⃗ x)
D(⃗
luego
⃗
E(r)
=

q
r̂
2πlrκ(r)ϵ0

⃗ no dependa de r, κ(r) debe ser de la forma
para que E
κ(r) =

α
r

Así
⃗
E(r)
=

q
r̂
2πlαϵ0

b) Calculemos la diferencia de potencial entre las cáscaras cilíndricas

ˆ B

⃗ x) = φ(A) − φ(B) = ∆V
d⃗x · E(⃗

A

ˆ r2

q
q
drr̂ ·
r̂ =
2πlαϵ0
2πlαϵ0
r1

ˆ r2

dr =

r1

q(r2 − r1 )
2πlαϵ0

y la capacidad de este condensador es
C=

2πlαϵ0
q
=
∆V
r 2 − r1

c) La densidad superficial de cargas de polarización está dada por
σP (⃗x) = P⃗ (⃗x) · n̂(⃗x), ⃗x ∈ S
y
sobre la superficie interior

!
"
⃗ = α − 1 ϵ0 E
⃗
P⃗ = (ϵ − ϵ0 E
r

---

### Página 285

n̂ = −r̂
#
$
α
⃗
P⃗ =
− 1 ϵ0 E
r1
#
$
α
q
r̂
P⃗ (⃗x) =
−1
r1
2πlα

y entonces

(=
(
σ1 = P⃗ · n̂(

r=r1

−

#

$
q
α
−1
r1
2πlα

para la superficie exterior

P⃗ =
luego
(
(
⃗
σ2 = P · n̂(

#

n̂ = r̂
$
α
⃗
− 1 ϵ0 E
r2

r=r2

=

#

$
q
α
−1
r2
2πlα

d) La densidad volumétrica de carga de polarización es
⃗ · P⃗
ρP = −∇
como

P⃗ = P (r)r̂
"
!!
"
⃗ · P⃗ = − 1 ∂ rP (r) = − 1 ∂ r α − 1 ϵ0 E
⃗
ρP = −∇
r ∂r
r ∂r
r
) #
$
*
1 ∂
α−r
q
ρP = −
r
ϵ0
r ∂r
r
2πlαϵ0
)
*
#
$
1 ∂ (α − r) q
1 −q
ρP = −
=−
r ∂r
2πlα
r 2πlα
ρP =

q
r2πlα

e) La carga total de polarización es
˚
ˆˆ
ˆˆ
✞☎
✞☎
3 ′
′
′
′
Qp =
d x ρP (⃗x ) + ✝ ✆ dS(⃗x )σ1 (⃗x ) + ✝ ✆ dS(⃗x′ )σ2 (⃗x′ )
V

S1

S2

---

### Página 286

#

ˆˆ

✞☎
x′ )σ1 (⃗x′ ) = −
✝ ✆ dS(⃗
S1

$
#
$
ˆˆ
α
q ✞☎
α
q2πr1 l
′
x)=−
−1
−1
✝ ✆ dS(⃗
r1
2πlα S1
r1
2πlα

q
✞☎
x′ )σ1 (⃗x′ ) = − (α − r1 )
✝ ✆ dS(⃗

ˆˆ

α

S1

del mismo modo
q
✞☎
✞☎
x′ )σ2 (⃗x′ ) = σ2 ✝ ✆ dS(⃗x′ ) = (α − r2 )
✝ ✆ dS(⃗

ˆˆ

ˆˆ

S2

α

S1

por último, recordando que el elemento de volumen en coordenadas cilíndricas es d3 x′ =
rdrdϕdz
ˆ
˚
ˆ 2π
ˆ l ˆ r2
2πlq r2
q
3 ′
′
=
drr
dr
d x ρP (⃗x ) =
dϕ
dz
2πlαr
2πlα r1
V
r1
˚
q
d3 x′ ρP (⃗x′ ) = (r2 − r1 )
α
V
Así

q
q
q
(r2 − r1 ) − (α − r1 ) + (α − r2 ) = 0
α
α
α
Esto siempre se cumple, pues un dieléctrico siempre es eléctricamente neutro, en efecto
˚
ˆˆ
✞☎
3 ′
′
⃗
⃗
⃗ x′ ) · P⃗ (⃗x′ ) = 0
QP =
d x − ∇ · P (⃗x ) + ✝ ✆ dS(⃗
QP =

V

S(V )

f) La energía almacenada por el condensador es
U=
donde
C=

1 q2
2C

2πlαϵ0
(r2 − r1 )

así
U=

1 q 2 (r2 − r1 )
2 2πlαϵ0

g) Tenemos que la energía inicial es
Ui =

1 q 2 (r2 − r1 )
2 2πlαϵ0

y la final
Uf =

1 q2
2 Cf

donde Cf es la capacidad final (en vacío).

---

### Página 287

Por ley de Gauss
✞☎ ⃗ ′
⃗ x′ ) = q = E2πrl
x ) · E(⃗
✝ ✆dS(⃗

ˆˆ

ϵ0

S

⃗ =
E
y
∆V =

ˆ r2

⃗ =
d⃗x · E

r1

Así
Cf =

q
r̂
2πrlϵ0

q
2πlϵ0

ˆ r2
r1

q
dr
=
ln
r
2πlϵ0

#

r2
r1

2πlϵ0
q
= ! "
∆V
ln r2
r1

y la energía final

! "
r2

1 q2
1 q ln r1
=
Uf =
2 Cf
2 2πlϵ0

Finalmente, el trabajo necesario para remover el dieléctrico es
+
# $,
r 1 − r1
r2
1 q2
W = Uf − Ui =
− ln
2 2πlϵ0
α
r1

$

---

### Página 288

Problema
Un condensador de placas paralelas de separación d entre las placas mucho menor que su largo
L y ancho w tiene la región entre las placas llenada por un material de constante dieléctrica κ,
el que puede deslizar libremente a lo largo de la dirección dada por L, como indicado en la figura. Inicialmente, el dieléctrico llena completamente la región entre las placas, y el condensador
está cargado con una carga total Q. Se pide determinar hasta qué distancia x uno tiene que
sacar el dieléctrico para que la energía almacenada en él aumente por un factor 2 con respecto
a su valor original, si la carga almacenada en el condensador se mantiene constante en el proceso

#### Solución
Antes de mover el dieléctrico, la capacidad es
Ci =

κϵ0 wL
d

y la energía inicial es
1 Q2
1 Q2 d
Ui =
=
2 Ci
2 κϵ0 wL
Supongamos que ahora se mueve el dieléctrico hasta una distancia x. Ahora el condensador
se puede pensar como dos condensadores en paralelo

---

### Página 289

la capacidad equivalente es
Ceq = C1 + C2 =

ϵ0 w
(x + κ(L − x))
d

y la energía final queda
1 Q2
Q2 d
U (x) =
=
2 Ceq x
2 ϵ0 w (x + κ(L − x))
se pide que
U (x) = 2Ui =

Q2 d
κϵ0 wL

Así, x debe cumplir
Q2 d
Q2 d
=
2 ϵ0 w (x + κ(L − x))
κϵ0 wL
2 (x + κ(L − x)) = κL
2x − 2κx + 2κL = κL → 2x (1 − κ) = −κL
x=

κL
2 (κ − 1)

---

### Página 290

Problema
Se tienen tres esferas conductoras concéntricas de radios a, b, y c. El espacio entre las dos
primeras está lleno con un dieléctrico de constante κ. Inicialmente la esfera de radio a está descargada y las esferas de radios b y c tienen carga q1 y q2 , respectivamente. La esfera interior de
radio a se conecta con la esfera de radio c con un cable aislado delgado

a) Calcular la carga libre en cada esfera
b) Calcular la carga de polarización en la superficie externa y en la superficie interna del
dieléctrico
#### Solución
a) Definimos las siguientes regiones

Al conectar las esferas de radio a y c, se distribuirá la carga en ambas de modo que quedan
al mismo potencial, luego
q2 = qA + q C
Además, para la región I

⃗ x) = ⃗0
r < a → E(⃗

pues corresponde al interior de una esfera conductora. Para a < r < b se utiliza la ley de Gauss
con una superficie esférica de radio r
ˆˆ
✞☎
⃗ x′ ) · D(⃗
⃗ x′ ) = 4πr2 D(r) = qA
✝ ✆ dS(⃗
S(r)

⃗ = qA r̂
D
4πr2

---

### Página 291

y luego
⃗
E(r)
=

qA
r̂
4πκϵ0 r2

Para la región b < r < c
ˆˆ

⃗ x′ ) · E(⃗
⃗ x′ ) = 4πr2 E(r) = (qA + q1 )
dS(⃗
ϵ0
S(r)

✞☎
✝✆

q A + q1
⃗
E(r)
=
r̂
4πϵ0 r2
Por último, para r > c
ˆˆ

⃗ x′ ) · E(⃗
⃗ x′ ) = 4πr2 E(r) = q1 + qA + qC
dS(⃗
ϵ0
S(r)

✞☎
✝✆

En resumen
⎧
⎪
⎪
⎨

⃗0

qA
r̂
4πκϵ0 r 2
⃗ x) =
E(⃗
qA +q1
⎪
2 r̂
⎪
0r
⎩ qA4πϵ
+q1 +qC
r̂
4πϵ0 r 2

si 0 < r < a
si a < r < b
si b < r < c
si c < r

El potencial en una esfera de radio a es
ˆ ∞
ˆ b
ˆ c
ˆ ∞
⃗ =
⃗
⃗
⃗
φ(a) =
d⃗r · E
d⃗r · E(r)
+
d⃗r · E(r)
+
d⃗r · E(r)
a

a

b

c

donde la última integral corresponde a
ˆ ∞
⃗
d⃗r · E(r)
= φ(c) = φ(a)
c

qA
φ(a) =
4πκϵ0

ˆ b

dr qA + q1
+
4πϵ0
a r

ˆ c
b

dr
+ φ(a)
r2

luego
#
$
#
$
1 1
qA + q1 1 1
qA
+
=0
−
−
4πκϵ0 a b
4πϵ0
b c
#
#
$
$
c−b
b−a
qA
+ (qA + q1 )
=0
ab
bc
b−a
c−b
+ (qA + q1 )
=0
ab
cb
#
$
b
b
q1 (b − c)
b(c − a)
b−c
qA
−1+1−
=
→ qA
= q1
a
c
c
ac
c
qA

Finalmente

qA =

q1 (b − c)a
b(c − a)

---

### Página 292

qC = q2 − qA = q2 −

q1 (b − c)a
b(c − a)

b) Sobre la superficie interna del dieléctrico

σP = P⃗ · n̂
⃗
P⃗ = (ϵ − ϵ0 ) E
sobre la superficie
⃗ =
E

qA
r̂
4πκϵ0 a2

y n̂ = −r̂
σa = −

(ϵ − ϵ0 ) qA
(κ − 1) qA
=
−
4πκϵ0 a2
4πκa2

y sobre la superficie externa

⃗ =
E

qA
r̂
4πκϵ0 b2
n̂ = r̂

luego
σb = P⃗ · n̂ = (ϵ − ϵ0 )
σb =

qA
4πκϵ0 b2

(κ − 1) qA
4πκb2

---

### Página 293

Problema
Una esfera dieléctrica de radio a y permitividad ϵ se coloca en un campo eléctrico inicialmente
uniforme, como se muestra en la figura

Encuentre el potencial φ y el campo eléctrico en todo el espacio
#### Solución
Dada la simetría esférica del problema, resolveremos el problema en coordenadas esféricas, como
se muestra en la figura

Como no hay cargas libres, el potencial electrostático satisface la ecuación de Laplace
⃗ 2φ = 0
∇
Dada la simetría azimutal (el potencial no depende del ángulo polar ϕ), la solución general
para r < a y r > a toma la forma
φint =

∞

Al rl Pl (cos ϑ)

l=0

φext =

∞
%
l=0

&
Bl rl Pl + Cl r−(l+1) Pl (cos ϑ)

⃗ x) = E0 z, o, equivalentemente
Lejos de la esfera dieléctrica, E(⃗
φ∞ = −E0 z
en coordenadas esféricas
φ∞ = −E0 r cos ϑ
Es decir
lím φ(r, ϑ) = φ∞ = −E0 r cos ϑ

r→∞

---

### Página 294

lím φext =

r→∞

∞

Bl rl Pl (cos ϑ) = −E0 r cos ϑ

l=0

De aquí, es claro que

Bl = 0, l = 0, 2, 3, 4...
y
B1 r cos ϑ = −E0 r cos ϑ
B1 = −E0
con esto, el potencial exterior toma la forma
φext = −E0 r cos ϑ +

∞

Cl r−(l+1) Pl (cos ϑ)

l=0

Ahora utilizaremos las condiciones de contorno en la superficie r = a. En primer lugar, la
componente tangencial del campo eléctrico en r = a debe ser continua
(
(
(
(
⃗
⃗
= Eext · ϑ̂(
Eint · ϑ̂(
r=a

(
(
⃗
−∇φint · ϑ̂(

r=a

r=a

(
(
⃗
= −∇φext · ϑ̂(

r=a

1 ∂φint ((
1 ∂φext ((
=
−
(
(
a ∂ϑ r=a
a ∂ϑ r=a
de forma equivalente, se puede imponer
(
(
(
(
= φext (
φint (
−

r=a

∞

l

Al a Pl (cos ϑ) = −E0 a cos ϑ +

l=0

∞

Cl a−(l+1) Pl (cos ϑ)

l=0

∞
%
l=0

De aquí, se obtiene

r=a

&
Al al − Cl a−(l+1) Pl (cos ϑ) = −E0 a cos ϑ
A1 a −

C1
= −E0 a
a2

y para l ̸= 1
Al al − Cl a−(l+1) = 0, l ̸= 1

Además, si no hay densidad de carga libre en la superficie dieléctrica, la componente normal
⃗ x) es continua
del campo D(⃗
(
(
⃗ int · r̂((
⃗ ext · r̂((
D
=D
r=a

r=a

---

### Página 295

(
(
⃗
−ϵ∇φint · r̂(

r=a

(
(
⃗
= −ϵ0 ∇φext · r̂(

r=a

∂φext ((
∂φint ((
= −ϵ0
(
(
∂r r=a
∂r r=a
∞
∞
ϵ
Al lal−1 Pl (cos ϑ) = ϵ0 −E0 cos ϑ − (l + 1)
Cl a−(l+2) Pl (cos ϑ)
−ϵ

l=0

l=0

# $1
∞
∞
ϵ
l−1
Al la Pl (cos ϑ) = −E0 cos ϑ −
(l + 1)Cl a−(l+2) Pl (cos ϑ)
ϵ0 l=0
l=0
∞ ## $
ϵ
l=0

ϵ0

l−1

Al la

+ (l + 1)Cl a

−(l+2)

$

Pl (cos ϑ) = −E0 cos ϑ

de aquí se obtiene

# $
ϵ
A1 + 2C1 a−3 = −E0
ϵ0
# $
ϵ
Al lal−1 + (l + 1)Cl a−(l+2) = 0, l ̸= 1
ϵ0
En resumen
A1 a −

C1
= −E0 a
a2

Al al − Cl a−(l+1) = 0, l ̸= 1
# $
ϵ
A1 + 2C1 a−3 = −E0
ϵ0
# $
ϵ
Al lal−1 + (l + 1)Cl a−(l+2) = 0, l ̸= 1
ϵ0
de la segunda ecuación

Al = Cl 2l+1 , l ̸= 1
a

reemplazando en la cuarta
# $
ϵ
Cl 2l+1 lal−1 + (l + 1)Cl a−(l+2) = 0, l ̸= 1
ϵ0
a
# $ #
$
ϵ
l+1
l
+ l+2 = 0, l ̸= 1
Cl
ϵ0
al+2
a

Luego

Cl = Al = 0, l ̸= 1

---

### Página 296

Para l = 1, de la primera ecuación
C1
− E0
a3

A1 =

reemplazando en la tercera
# $#
$
ϵ
C1
− E0 + 2C1 a−3 = −E0
ϵ0
a3
C1
a3
Finalmente

#

#
$
$
ϵ
ϵ
+ 2 = E0
−1
ϵ0
ϵ0
2ϵ

−1

−1
ϵ0

C1 = a E0

A1 = E0

A1 = E0

ϵ0
ϵ
+2
ϵ0

2ϵ

ϵ
+2
ϵ0

2ϵ

− E0

− 1 − ϵϵ0 − 2
ϵ0

A1 = −E0

ϵ
+2
ϵ0

ϵ
+2
ϵ0

Con esto, se tiene
φint = −E0

ϵ
+2
ϵ0

ϵ
+2
ϵ0

2ϵ

r cos ϑ = −E0

φext = −E0 r cos ϑ +

a
cos ϑE0
r2

−1
ϵ0
ϵ
+2
ϵ0

Notar que el potencial interior define un campo eléctrico uniforme
⃗ int = E0
E
ẑ
ϵ
+2
ϵ0

z

---

### Página 297

La figura muestra las equipotenciales para E0 = 100 (V /m), ϵ/ϵ0 = ϵr = 5, a = 10 (m)

Notar que un dieléctrico con permitividad muy grande se compora de forma similar a un
conductor, en efecto, si ϵ → 0
⃗ · E(⃗
⃗ x) = ρ → 0
∇
ϵ
⃗
⃗
∇ × E(⃗x) = 0
y entonces el campo está forzado a ser nulo en el interior del dieléctrico / conductor. La
siguiente figura muestra la solución para ϵr = 5000

En este caso, el potencial es prácticamente constante e igual a cero dentro de la esfera

---

### Página 298

Parte IV
Corrientes Eléctricas

---

### Página 299

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 300

#### Capítulo 11
Corrientes Eléctricas
Las corrientes eléctricas son flujos de cargas eléctricas. Para ilustrar esto supongamos un
conjunto de cargas que se mueven perpendicularmente a una superficie de área A, como se
muestra en la figura

La corriente eléctrica se define como la tasa a la cual las cargas atraviesan un área transversal.
Si una cantidad de carga ∆Q pasa a través una superficie en un intervalo de tiempo ∆t, entonces la corriente promedio Iavg está dada por:
∆Q
∆t
. El rango común
La unidad en S.I. de la corriente es el ampere (A), con 1A = 1 Coulomb
seg
de corrientes va desde mega-amperes en rayos hasta nano-amperes en células nerviosas. En el
límite cuando ∆t → 0, la corriente instantánea se define como
Iavg =

dQ
dt
Ya que el flujo tiene una dirección, hemos introducido implícitamente la convención de que
la dirección de la corriente corresponde a la dirección en la cual las cargas positivas se mueven.
Las cargas que se mueven dentro de un cable son electrones cargados negativamente que se
mueven en dirección opuesta a la corriente. Corrientes eléctricas fluyen en conductores, sólidos
(metales, semiconductores), fluídos (electrolitos, ionizados) y gases (ionizados), pero el flujo no
es permitido en no conductores o aislantes.
I=

---

### Página 301

11.1.

Densidad de Corriente

Intentaremos ahora relacionar la corriente (una cantidad macroscópica) con el movimiento
microscópico de las cargas. Para ello supongamos un conductor de área transversal A, como se
muestra en la figura

Sea la corriente total a través de una superficie escrita como
¨
⃗ x′ ) · J(⃗
⃗ x′ )
I=
dS(⃗
S

⃗ x) es la densidad de corriente ( tiene unidades de A/m2 ). Si q es la carga de cada
donde J(⃗
portador, y n es el número de portadores de carga por unidad de volumen, la cantidad de carga
total en esta sección es ∆Q = q(nA∆x). Supongamos que las cargas se mueven con velocidad
vd , así, el desplazamiento en un intervalo ∆t será ∆x = vd ∆t, lo que implica
∆Q
= nqvd A
∆t
La velocidad vd a la cual el portador de carga se mueve se conoce como velocidad de deriva.
Físicamente, vd es la velocidad promedio de un portador de carga dentro de un conductor
cuando un campo eléctrico externo es aplicado. De hecho, un electrón dentro de un conductor
no viaja en línea recta, si no que su movimiento es errático, como se ve en la figura
Iavg =

Se tiene entonces que la densidad de carga se puede escribir como
J⃗ = nq⃗vd
Vemos entonces que J⃗ y ⃗vd tienen la misma dirección para portadores de carga positiva, y
tienen direcciones opuestas para los portadores de carga negativa

---

### Página 302

11.2.

Continuidad de la carga Eléctrica

Consideremos un volumen V determinado por una superficie cerrada S. La carga que entra
en el dominio V en 1 segundo será ( o equivalentemente, la corriente que ingresa a V )
ˆˆ
✞☎ ⃗ ′
⃗ x′ )
x ) · J(⃗
I = − ✝ ✆dS(⃗
S

Notar que el signo menos es consistente con la definición de flujo (Flujo es positivo cuando
las líneas de campo salen a través de la superficie ). Por otro lado, la carga total encerrada por
este volumen para cierto instante estará dada por
˚
d3 x′ ρ(⃗x′ , t)
Q(t) =
V

Con lo que la corriente será la razón de cambio de esta carga en el tiempo
˚
dQ
∂ρ(⃗x′ )
I=
d3 x′
=
dt
∂t
V
Igualando debe tenerse entonces
˚
ˆˆ
∂ρ(⃗x′ )
✞☎ ⃗ ′
′
⃗
d3 x′
− ✝ ✆dS(⃗x ) · J(⃗x ) =
∂t
S
V
Utilizando el teorema de la divergencia
˚
˚
∂ρ(⃗x′ )
3 ′⃗ ′ ⃗ ′
−
d x ∇ · J(⃗x ) =
d3 x′
∂t
V
V
#
$
˚
∂ρ(⃗x′ )
3 ′
′ ⃗
⃗
=0
d x ∇ · J(⃗x) +
∂t
V
Esta ley de conservación de la carga simplemente indica que la variación de la carga contenida en un volumen arbitrario V se debe a un flujo de carga a través de su superficie. Como
se cumple para todo V , se obtiene la ecuación de continuidad para la carga eléctrica, en su
forma diferencial
⃗ · J(⃗
⃗ x, t) + ∂ρ(⃗x) = 0
∇
∂t
Supongamos que en determinada región del espacio existe una corriente en estado estacionario, es decir, no hay dependencia temporal. Entonces se cumple
⃗ · J(⃗
⃗ x) = 0
∇

---

### Página 303

Cuando existen corrientes estacionarias, la densidad de carga en cada punto es una constante. Es decir, sobre cualquier volumen V , el flujo neto de carga a través de su superficie es
cero, lo que es consistente con
ˆˆ
˚
✞☎
⃗ x) · J(⃗
⃗ x) =
⃗ · J(⃗
⃗ x) = 0
d3 x∇
✝ ✆ dS(⃗
S(V )

11.3.

V

Ley de Ohm

Las corrientes en medios materiales surgen como una respuesta a un campo eléctrico. En
algunos materiales, la densidad de corriente depende linealmente del campo eléctrico externo
⃗ Esta relación usualmente se expresa como
E.
⃗ x) = σ E(⃗
⃗ x)
J(⃗
Donde σ es la conductividad del material. Este podría ser una matriz de coeficientes
no constantes (lo que representa a un medio no homogéneo y anisotrópico). Sin embargo,
trabajaremos con medios simples, en donde σ es una constante positiva. Esta ecuación se
conoce como la ley de Ohm diferencial. Un material que obedece esta relación se dice Ohmico.
Veamos un caso particular y muy usual de la ley de Ohm, consideremos un segmento de alambre
recto de largo l ,área A, y conductividad σ, como se muestra en la figura

Supongamos que una diferencia de potencial ∆V = φb − φa es aplicada entre los extremos del
⃗ , y como consecuencia, una corriente I. Asumiendo
alambre, generando un campo eléctrico E
⃗ uniforme en el conductor, y apuntando en la dirección longitudinal se tiene
E
∆V = φb − φa = −

ˆ b

⃗ x) = El
d⃗x · E(⃗

a

Si el medio es Ohmico, el módulo de la densidad de corriente se puede escribir como
$
#
∆V
J = σE = σ
l
Por otro lado, J = I/A, luego
l
∆V = J =
σ
Donde

#

l
σA

$

I = RI

l
∆V
=
I
σA
es la resistencia del conductor. La famosa ecuación
R=

---

### Página 304

∆V = IR
Es la version macroscópica de la ley de Ohm. La unidad de R es el Ohm (Ω), donde
1V
1A
También se suele definir la de un material como una propiedad intensiva de éste, que es
simplemente el recíproco de la conductividad
1Ω =

σ
con esto la resistencia de un conductor cilíndrico queda
ρ=

ρl
A
La mayoría de los metales, con buena conductividad y baja resistividad, son ohmicos.
R=

11.3.1.

Conexión entre conductores

Imaginemos que se tienen 2 conductores perfectos, inicialmente cargados (se encuentran
entonces a determinado potencial). La forma de estos dos conductores es absolutamente irrelevante, pero por simpleza y elegancia, en la siguiente figura se ilustran dos conductores esféricos,
cargados con carga q1 y q2 , respectivamente

Si estos conductores están en el vacío, existirá un campo electrostático. Suponiendo que el
conductor con carga q1 se encuentra a mayor potencial, las líneas de campo se verán (para el
caso de los conductores esféricos) así

Si existiera alguna carga libre, ciertamente ésta se movería debido al campo eléctrico que
generan los conductores. Sin embargo, en el vacío (ausencia de cargas), simplemente nada
ocurre. Ahora, imaginemos que ambos conductores se conectan por algún medio parcialmente
conductor (de conductividad finita). La forma puede ser cualquiera, incluso podríamos imaginar
en llenar todo el espacio de un material conductor, pero podemos imaginar como caso particular
(y simple) un alambre muy delgado

---

### Página 305

¿Qué ocurre entonces?. Ahora existe un medio entre los conductores que posee cargas libres !
Sin duda éstas se moveran siempre que exista un campo eléctrico, y entonces cargas se moverán
desde el conductor a mayor potencial hacia el conductor que está a menor potencial. Como
consecuencia de esto, el campo eléctrico en la región entre los conductores se irá debilitando,
pues este movimiento de cargas de uno al otro provocará una disminución en la diferencia de
potencial entre ambos conductores. En conclusión, la conexión entre 2 conductores mediante
un medio de conductividad finita dará origen a una corriente. Esta corriente se hará cada vez
mas débil, hasta que se alcanze un equilibrio en el cual los dos conductores quedan al mismo
potencial.
Ahora, pensemos que tenemos un solo conductor, inicialmente cargado con carga Q. Imaginemos que lo conectamos con el infinito mediante algun camino de conductividad finita, por
ejemplo un alambre infinito, esto equivale a conectarlo a otro conductor a potencial cero. Lo
que sucederá es que toda la carga contenida en el conductor se irá por este camino hacia el
infinito, de esta forma, nuestro conductor queda a potencial cero y absolutamente descargado.

---

### Página 306

11.4.

Circuitos Eléctricos

Un circuito es una malla de resistencias, fuentes, condensadores, etc, unidas por medio de
conductores perfectos. Un nodo es un punto donde convergen 2 o más conductores. Así, en un
nodo se cuple que la suma de las corrientes es cero, esta es la 1 Ley de Kirchhoff, o Ley de
Corrientes de Kirchhoff (LCK)
Ik = 0
k

Notar que esta ecuación es equivalente a la ecuación de continuidad de la carga eléctrica
para corrientes continuas (estacionarias)
⃗ · J(⃗
⃗ x) = 0
∇

.
La segunda Ley de Kirchhoff o Ley de Voltajes de Kirchhoff (LVK) dice que la suma de las
caídas de potencial en cada camino cerrado suma 0. Notar que esta ley proviene de
⃗ × E(⃗
⃗ x) = 0
∇
⃗ sobre una curva cerrada (circuito cerrado) es 0.
Debido a esto la integral de línea del campo E
Energía eléctrica y potencia
Considere un circuito consistente en una batería y una resistencia (R). Sea la diferencia de
potencial entre los puntos a y b ∆V = φb − φa > 0. Si una carga ∆q se mueve a través de
la batería, su energía potencial eléctrica aumenta ∆U = ∆q∆V . Por otro lado, si la carga se
mueve a través de la resistencia, la energía potencial decrece debido a las colisiones con los
átomos de la resistencia. Si despreciamos la resistencia interna de la batería y la de los cables
conductores, al volver al punto a, la energía de ∆q permanece invariante.

Así, la tasa a la que se disipa energía a través de la resistencia está dada por
∆U
∆q
= ( )∆V = I∆V
∆t
∆t
Esta es precisamente la potencia suministrada por la batería. Usando que ∆V = IR, se
puede reescribir como
P =

(∆V )2
R
Los circuitos eléctricos conectan fuentes de poder a cargas como resistencias, motores,
lámparas, etc. La conexión entre la fuente y la carga se hace soldando con cables conductores, tambien llamados nodos. Las distintas partes de un circuito pueden estar en serie o en
P = I 2R =

---

### Página 307

paralelo, como ya se vió en el caso de los capacitores.
Dos elementos se dicen estar en paralelo cuando son conectados a la misma diferencia de potencial.

Por otro lado,cuando los elementos son conectados uno seguido de otro, tal que la corriente
pasa a través de cada elemento sin otros caminos de por medio, los elementos están en serie.
Se pueden tener circuitos cerrados, a través de los cuales fluye corriente, o bien circuitos
abiertos en donde no existen corrientes. Usualmente por accidente, los cables pueden entrar en
contacto, causando un corto circuito, esto es, gran parte de la corriente fluirá a través del corto
circuito, mientras que una fracción muy pequeña fluirá a través de la carga.
Esto podría quemar un equipo eléctrico como un transformador. Para prevenir el daño, un
fusible se conecta en serie. Cuando hay un corto circuito, el fusible aisla la carga del resto del
circuito.
En los circuitos eléctricos, un punto (o un nodo en común) se escoge como tierra. A este punto
se le asigna arbitrariamente un voltaje, usualmente cero, y el voltaje V en cualquier otro punto
del circuito está definido como la diferencia de potencial entre el punto y la tierra.
Fuerza Electromotriz
Vimos que energía eléctrica debe ser suministrada para mantener una corriente constante en
un circuito cerrado. La fuente de energía es llamada comúnmente como la fuerza electromotriz,
o f.e.m (ε). Las baterías son ejemplos de fuentes de f.e.m. Se pueden pensar como bombas que
mueven cargas desde potenciales bajos a potenciales más altos. Matemáticamente la f.e.m se
define como
dW
ε=
(11.1)
dq
Que corresponde al trabajo hecho para mover una unidad de carga en la dirección del potencial
más alto. La unidad SI para ε es el volt (V). Considere un circuito simple que consiste en una
batería como fuente de f.e.m y una resistencia R, como se muestra en la figura

Asumiendo que la batería no posee resistencia interna, la diferencia de potencial ∆V entre los
terminales positivo y negativo de la batería es igual a la fem ε. Para establecer una corriente

---

### Página 308

alrededor del circuito, la batería efectúa un proceso de descarga que convierte energía química
en una f.e.m. La corriente I se puede encontrar notando que no hay un trabajo neto al mover
una carga q a través de un camino cerrado debido a la naturaleza conservativa de la fuerza
electrostática.

W = −q

˛

⃗ · dS
⃗=0
E

Sea a el punto de partida

Cuando se atraviesa desde el terminal negativo al positivo, el potencial aumenta en ε. Por otro
lado, cuando atravesamos la resistencia, el potencial decrece una cantidad IR, y la energía
potencial se convierte en energía térmica en la resistencia. Asumiendo que los cables conectores
no poseen resistencias, a través de un camino cerrado, la diferencia de potencial neta es cero
ε − IR = 0
Lo que implica
I=

ε
R

De todas formas, una batería real siempre posee una resistencia interna r

Ahora la diferencia de potencial a través de la batería es
∆V = ε − Ir
Ya que no hay una diferencia de potencial neta a través de un camino cerrado, tenemos
ε − Ir − IR = 0
O bien
ε
R+r
De la figura de la derecha vemos el cambio de potencial mientras atravesamos el circuito en el
sentido del reloj. Notar que la mayor diferencia de potencial está inmediatamente despues de la
I=

---

### Página 309

batería. El voltaje cae a medida que se atraviesa cada resistencia. Notar también que el voltaje
es constante en los cables. Esto se debe a que los cables poseen resistencias extremadamente
pequeñas comparadas con las resistencias del circuito.
Para una fuente de f.e.m ε, la potencia a la cual la energía se entrega es
P = Iε = I(IR + Ir) = I 2 R + I 2 r
Es decir, la potencia de la fuente es igual a la suma de la potencia disipada en ambas resistencias, la interna y la de carga. Esto es necesario debido a la conservación de la energía.

---

### Página 310

Problema
El espacio entre dos circuitos conductores de largo L y radios a y b (b > a), está lleno de
material de conductividad σ. Calcule la intensidad de la corriente por unidad de longitud y la
resistencia, cuando la diferencia de potencial entre los conductores es V0 .

#### Solución
La diferencia de potencial será responsable de un movimiento de cargas a través del material
conductor que se encuentra entre los conductores externos. La conservación de la carga implica
∂ρ(⃗x) ⃗ ⃗
+ ∇ · J(⃗x) = 0
∂t
Para corrientes estacionarias
∂ρ(⃗x)
⃗ · J(⃗
⃗ x) = 0
=0→∇
∂t
⃗ x) = σ E(⃗
⃗ x)
Si el medio es Ohmico, J(⃗
⃗ ·
∇
Si el medio además es homogéneo

#

$
1⃗
E(⃗x) = 0
σ

1⃗ ⃗
⃗ · E(⃗
⃗ x) = 0
∇ · E(⃗x) = 0 → ∇
σ
Finalmente

⃗ 2φ = 0
∇

Y entonces el potencial satisface la ecuación de Laplace en la región a < r < b. La solución
en coordenadas cilíndricas (suponiendo que ése depende únicamente de la coordenada radial r)
es
φ(r) = A ln r + B
Imponiendo la condición φ(a) − φ(b) = V0
A = V0 ln

b
a

Así, se obtiene el campo eléctrico
⃗ x) = −∇φ(⃗
⃗ x)
E(⃗
⃗ x) = V0 ln b 1 r̂
E(⃗
ar

---

### Página 311

Utilizando la ley de Ohm, se obtiene la densidad de corriente
⃗ x) = σ E(⃗
⃗ x) = σV0 ln b r̂
J(⃗
ar
La corriente por unidad de largo que fluye a través de los conductores se puede obtener
como la integral de flujo de la densidad de corriente sobre una superficie cilíndrica de radio r
(y largo unitario). Esta integral resulta simple pues la densidad de corriente tiene magnitud
constante a lo largo de esta superficie, y su dirección coincide en todo punto con la normal. El
diferencial de área sobre el cilindro es da = drdϕdz
ˆ 1 ˆ 2π
¨
σV0 b
⃗
⃗
dS(⃗x) · J(⃗x) =
dz
dϕr
I=
ln
r
a
S
b
I = 2πσV0 ln [A/m]
a
Así, la resistencia por unidad de longitud es
r=

V0
ln(b/a)
=
I
2πσ

y la resistencia total es
R = rL =

L ln(b/a)
2πσ

---

### Página 312

Problema
Dos esferas metálicas concéntricas, de radios a y b están separadas por un material conductor
de conductividad σ constante
a) Si estas esferas son mantenidas a una diferencia de potencial V constante, encuentre la
corriente que va de una a la otra
b) Encuentre la resistencia entre las esferas
c) Observe que en este caso se cumple R = ϵ0 /, donde C es la capacidad. Demuestre esta
fórmula para dos conductores cualquiera, separados por un material conductor de conductividad
σ constante

#### Solución
a) Al establecer una diferencia de potencial sobre los conductores
V = φ(a) − φ(b)
se inducirán cargas Q y −Q sobre las superficies r = a y r = b, respectivamente. El campo
eléctrico en la región interior se puede determinar a partir de la ley de Gauss debido a la simetría
esférica que éste debe tener
ˆˆ
✞☎ ⃗
⃗ x) = Q
x) · E(⃗
✝ ✆dS(⃗
ϵ0
S
Si S se escoge como una superficie esférica de radio r, se tiene
E(r)4πr2 =
⃗
E(r)
=

Q
ϵ0

Q
r̂, a < r < b
4πϵ0 r2

Por otro lado
V =

ˆ b

⃗ x) =
d⃗x · E(⃗

a

ˆ b

drQ
a 4πϵ0 r

donde se ha utilizado un camino radial para evaluar la integral de línea
#
$
1 1
Q
V =
−
4πϵ0 a b
Entonces

V 4πϵ0
Q= 1 1
−b
a

---

### Página 313

luego, para a < r < b
⃗ x) =
E(⃗

V ab
r̂
(b − a)r2

Debido a que la zona a < r < b está llena con un material conductor, el campo eléctrico
dará origen a un movimiento de cargas (corriente), en donde la densidad está relacionada con
⃗ mediante la ley de Ohm
el campo E
⃗ x) = σ E(⃗
⃗ x) =
J(⃗

V σab
r̂
(b − a)r2

La corriente que fluye entre los conductores se puede obtener integrando sobre una superficie
esférica S de radio r, a < r < b
ˆˆ
✞☎ ⃗
⃗ x) = 4πr2 J(r)
x) · J(⃗
I = ✝ ✆dS(⃗
S

Luego
I=

4πσV ab
(b − a)

b) La resistencia está dada por
V
I
#
$
1 1
−
R=
4πσ a b
R=

c) La capacidad de un condensador esférico es
C=

Q
4πϵ0 ab
=
V
b−a

Evaluando
ϵ0
ϵ0 a1 − 1b
=
=
σC
σ 4πϵ0
y entonces se tiene

ϵ0
=R
σC

%1

− 1b
4πσ

a

&

---

### Página 314

Veamos que esto se cumple en el caso general. Sean 1 y 2 dos conductores cualquiera ,
separados por un material de conductividad σ

Se tendrá un flujo de corriente dado por
ˆˆ
✞☎ ⃗
⃗ x)
I = ✝ ✆dS(⃗
x) · J(⃗
S

por ley de Ohm

⃗ x) = σ E(⃗
⃗ x)
J(⃗
ˆˆ

✞☎ ⃗
⃗ x)
I = σ ✝ ✆dS(⃗
x) · E(⃗
S

por ley de Gauss
Q
ϵ0
Por otro lado, si C es la capacidad del sistema, se cumple
I=σ

Q = CV
entonces
I=

σCV
ϵ0

V =

ϵ0
I
σC

Finalmente se demuestra la relación general
R=

ϵ0
σC

---

### Página 315

Problema
Considere un conductor perfecto, inicialmente con carga Q0 , y completamente rodeado por un
medio uniforme de conductividad σ y constante dieléctrica ϵ
a) Si el conductor es una esfera de radio a, muestre que su carga como función del tiempo es
Q(t) = Q0 e−σt/ϵ
b) Muestre que el resultado anterior es válido independientemente de la forma del conductor
#### Solución
a) Sea Q(t) la carga sobre la superficie esférica al instante t. Ésta generará un campo eléctrico
esféricamente simétrico

⃗ x, t) = Q(t) r̂
E(⃗
4πϵr2
al ser el medio circundante un conductor de conductividad σ, se tendrá una densidad de
corriente como respuesta a este campo
⃗ x, t) = σ E(⃗
⃗ x) = σQ(t) r̂
J(⃗
4πϵr2
Esta es una corriente que fluye isotrópicamente de forma radial. La corriente se obtiene de
⃗ x) sobre una superficie cerrada que contenga a la esfera conductora, en particular se
integrar J(⃗
puede evaluar tomando una esfera concéntrica de radio r > a
¨
⃗ x) · J(⃗
⃗ x, t) = σQ(t)
I(t) =
dS(⃗
ϵ
S
Por otro lado, la carga total contenida en el volumen encerrado por S es
˚
Q(t) =
d3 xρ(⃗x, t)
V

Por la continuidad de la carga
dQ(t)
= I(t)
dt
σQ(t)
dQ(t)
=
dt
ϵ

---

### Página 316

cuya solución es
Q(t) = Q0 e−tσ/ϵ

b) El resultado anterior es independiente de la forma de los conductores. En efecto, sea S
una superficie cerrada que contenga completamente al conductor. La corriente que se genera
está dada por
ˆˆ
✞☎ ⃗
⃗ x)
I = ✝ ✆dS(⃗
x) · J(⃗
S

Si el medio es ohmico
ˆˆ

✞☎ ⃗
⃗ x)
x) · E(⃗
I = σ ✝ ✆dS(⃗
S

y utilizando la ley de Gauss
I=σ

dQ(t)
Q(t)
=
ϵ
dt

y se obtiene la misma ecuación diferencial para la carga contenida en el conductor

---

### Página 317

Problema
Dos cilindros coaxiales (radios a y b) de largo L están separados por un material de conducividad
σ(r) = kr donde k es una constane arbitraria y r la distancia al eje (común) de los cilindros.
Encuentre la resistencia entre los cilindros. Observe que al ser la conductividad función de la
posición, la densidad de carga en el material conductor no es cero y el campo E no varía como
1/r. Recuerde que una corriente estacionaria I tiene el mismo valor para cualquier superficie
cilíndrica

#### Solución
Supongamos que se establece una diferencia de potencial ∆V > 0 entre los conductores r = a
y r = b. Usaremos el hecho de que la corriente que fluye entre los cilindros está dada por la
integral
¨
⃗ x)
I=
dS(⃗x)n̂(⃗x) · J(⃗
S

Donde S es un cilindro concéntrico a los conductores, de radio r y largo L. Además, por
simetría cilíndrica, J⃗ = J(r)r̂
I = 2πrLJ(r)
luego la densidad de corriente es
⃗ x) =
J(⃗

I
r̂
2πrL

⃗ = E(r)r̂ (por simetría), se tiene por ley de Ohm
Si E
⃗ x) = σ(r)E(r)
⃗
J(⃗
luego
E(r) =

r I
k 2πrL

con esto, la diferencia de potencial entre los conductores es
ˆ b
⃗ x) = I (b − a)
∆V =
d⃗x · E(⃗
2πLk
a
Entonces
R=

∆V
b−a
=
I
2πkL

---

### Página 318

Problema
Se sabe que la atmósfera tiene una conductividad (causada principalmente por los rayos cósmicos) que depende de la altura de la siguiente manera
#
$
z2
σ(z) = 3 +
10−14 [Ω]−1
donde z es la distancia vertical sobre el suelo. Se ha encontrado además, un campo eléctrico
vertical, dirigido hacia el suelo, que en la superficie de la tierra vale
⃗ = −100k̂
E
Suponga el siguiente modelo de la atmósfera: imagine una capa conductora paralela a la superficie; situada a una distancia de 15 km sobre el nivel del suelo. Entre esta capa y la tierra se
encuentra la atmósfera, con la conductividad y el campo eléctrico indicados arriba. El radio de
la tierra es RT = 6400 km.
a) Calcule el campo eléctrico y el potencial en función de la altura z
b) Calcule la corriente total que fluye entre la capa superior conductora y la tierra
#### Solución
a) Sabemos que en corriente continua (o estacionaria) se cumple que
⃗ · J(⃗
⃗ x) = 0
∇
Además, se sabe que la dirección del campo eléctrico es según z y, por razones de simetría
no debe depender de las coordenadas x e y. Eso se traduce en
⃗ · (σ(z)E(z)) = d (σ(z)E(z)) = 0
∇
dz
σ(z)E(z) = A
El valor de esta constante se puede obtener evaluando en z=0
A = σ(0)E(0) = −3 × 10−12

De esta forma, el campo eléctrico en la atmósfera es
⃗ x) = −3 × 10−12
E(⃗

(3 + z3 )10−14

k̂ =

−300
2 k̂
3 + z3

Fijando el valor del potencial en la tierra como 0, entonces
φ(z) =

ˆ ⃗x2

⃗ x)
d⃗x · E(⃗

⃗
x1

donde ⃗x2 es cualquier punto a altura z, y ⃗x1 es un punto sobre la superifice. Escogiendo una
curva vertical, se tiene
$
ˆ z #
ˆ z
!z "
φ(z) =
=
900Arctg
dz
=
dz
3 + z2
3 + z3

---

### Página 319

b) La densidad de corriente se obtiene usando la ley de Ohm, esto es
#
$
z
⃗ x) = σ(z)E(⃗
⃗ x) = − 3 +
J(⃗
10−14
k̂ = −3 × 10−12 [A/m2 ]k̂
z2
3+ 3
La corriente será
I=

¨

S

⃗ x′ ) · J(⃗
⃗ x′ ) = −3 × 10−12 S = −3 ∗ 10−12 4πRT2
dS(⃗
I = 122,88[A]

---

### Página 320

Problema
Una batería descargada se carga conectándola a la batería cargada de otro automóvil mediante
cables para corriente. Determine la corriente del motor de arranque y en la batería descargada

#### Solución
Se utiliza la Ley de Voltajes de Kirchhoff (LVK) para cada malla, esto es

Para la malla 1
−12 + 0,01I1 + 1 (I1 − I2 ) + 10 = 0
y en la malla 2
−10 + 1(I2 − I1 ) + 0,06I2 = 0

De la primera ecuación se obtiene
I2 = 1,01I1 − 2
Reemplazando
0,0706I1 − 2,02 = 10 → I1 = 170,25A
Con esto
I2 = 1,01 ∗ I1 − 2 = 169, 95A

---

### Página 321

I2 es la corriente a través del motor de arranque, mientras que la corriente a través de la
batería descargada será, según nuestra convención

I3 = I1 − I2 = 170,25 − 169,95 = 0,2975A

---

### Página 322

Problema
En el circuito de la figura la batería tiene una FEM de valor V . Encuentre la resistencia R que
debe colocarse entre los terminales A y B para que en ella se disipe la máxima potencia

#### Solución
Resolviendo el problema con mallas

Para la malla 1
−V + I1 R0 + R0 (I1 − I2 ) = 0
Para la malla 2
R0 (I2 − I1 ) + R0 I2 + RI2

De la primera ecuación se obtiene
I1 =

V + I2 R0
2R0

Reemplazando en la ecuación de la malla 2
V + I2 R0
2R0
V
(3R0 + 2R)I2 = V → I2 =
3R0 + 2R
(2R0 + R)I2 = R0 I1 = R0

Teniendo la corriente que pasa por la resistencia R, la potencia que ésta consume se puede
obtener como
P = VR IR = (IR R)IR = IR2 R

---

### Página 323

Así
P =

V2
R
(3R0 + 2R)2

Para encontrar el valor de R que maximize esta potencia consumida, bastará con resolver
dP (R)
=0
dR
Esto es
dP
4RV 2
3V 2 R0 + 2V 2 R − 4RV 2
V2
−
=
=
dR
(3R0 + 2R)2 (3R0 + 2R)3
(3R0 + 2R)3

3V 2 R0 − 2V 2 R
= 0 → 3V 2 R0 − 2V 2 R = 0
(3R0 + 2R)
Así, la resistencia R que maximiza la potencia consumida es
R = R0

---

### Página 324

Problema
La fuente V1 = 240 (V) está conectada a tres resistencias iguales según la figura

a) Determine R si la fuente de voltaje entrega 1920(W) al conjunto de resistencias
b) Si al circuito en paralelo, se le agregan más resistencias en paralelo, siguiendo una secuencia
de 3R en serie, 4R en serie, hasta llegar a N R en serie, calcule la potencia suministrada por la
fuente de voltaje cuando N tiende a Infinito

#### Solución
a) El circuito se puede reducir considerando que hay 2 resistencias en serie, cuya resistencia
equivalente será la suma de ambas, así, el circuito queda

Estas 2 resistencias ahora se encuentran en paralelo, por lo que se puede obtener un Req de
todo el circuito
= +
=
Req
R 2R
2R
Con lo que

Req = R

---

### Página 325

Con esto, el circuito equivale a

La potencia generada por este circuito será la misma que consume Req , esto es
$
#
V
= 1920W
P = VReq IReq = V IReq = V
Req
De aquí se obtiene
Req =

V2
=
= 30Ω
P

Finalmente se obtiene R usando que
Req = R → R = Req = 45Ω
b)

En este caso, se puede obtener una resistencia equivalente según
= +
+ ... +
Req
R 2R
NR
Así, se puede obtener la potencia que debe entregar la fuente para un cierto valor de N
N
V2
PN =
=V
Req
kR
k=1

Así, para obtener la potencia cuando N tiende a infinito, bastará con obtener el siguiente
límite (si existe)
PN →∞ = lím PN = V 2
N →∞

∞
k=1

kR

Pero esta serie diverge, es decir, la potencia necesaría sería infinita. Esto es lógico ya que la
fuente tendría que alimentar un número infinito de resistencias.

---

### Página 326

Problema
Una batería tiene una f.e.m ε y una resistencia interna R. Una resistencia de carga R2 se conecta
a los terminales de la batería.
a) Determine el valor de R2 tal que la diferencia de potencial aplicada a los terminales sea
máxima.
b) Determine el valor de R2 para obtener una corriente máxima en el circuito.
c) Determine el valor de R2 para que la potencia consumida por ésta sea la máxima posible

#### Solución
a) Primero determinamos la corriente a través del circuito
ε
R + R2
Así, la diferencia de potencial entre los extremos de la batería es
−ε + IR + IR2 = 0 → I =

V = IR2 =

R2 ε
ε
=
R + R2
1 + RR2

La diferencia de potencial entre los terminales será máxima cuando R2 → ∞ y valdrá ε,
que es el valor de la fem.
b) Teníamos que

ε
R + R2
Luego, la corriente será máxima si R2 = 0, y equivale a cortocircuitar los terminales de la
batería
I=

c) La potencia consumida por R2 está dada por
P =VI =

R 2 ε2
R2 ε
ε
=
R + R2 R + R2
(R + R2 )2

Para encontrar el valor de R2 que maximiza esta potencia resolvemos
ε2 (R + R2 )2 − 2(R + R2 )R2 ε2
dP
=
=0
dR2
(R + R2 )4

---

### Página 327

Así
(R + R2 )2 − 2(R + R2 )R2 = 0 → R2 + R − 2R2 = 0
Luego, la potencia será máxima si
R2 = R
es decir, se debe colocar una resistencia igual a la resistencia interna de la batería

---

### Página 328

Problema
Calcule la potencia entregada a cada resistencia en el circuito de la figura

#### Solución
Se resuelve el circuito mediante LVK

Para la malla 1
−18 + 2I1 + 3(I1 − I2 ) + 4I1 = 0 → 9I1 − 3I2 = 18
en la malla 2
3(I2 − I1 ) + 1I2 = 0 → 4I2 = 3I1

Resolviendo
9I1 − I1 = 18 → I1 = 2, 6A
I2 = I1 = 2A
Teniendo las corrientes que circulan por el circuito, podemos obtener la potencia que consume cada resistencia, usando que P = V I = I 2 R
P2Ω = 2I12 = 13, 52W
P4Ω = 4I12 = 27, 04W
P3Ω = 3(I1 − I2 )2 = 1, 08W
P1Ω = 1I22 = 4W

---

### Página 329

Problema
El circuito de la figura es llamado Puente de Wheastone y se usa para calibrar resistencias. El
dispositivo está formado por 3 resistencias, de las cuales 2 son ajustables, y un galvanómetro
(dispositivo que sirve para medir corrientes). Para realizar la medida, se ajustan las resistencias
variables R1 y R2 hasta que el galvanómetro marque cero. Exprese el valor de Rx en función
de las otras 3 resistencias. Modele el galvanómetro como una resistencia RG .

#### Solución
Definamos las corrientes que circulan por el circuito

Se obtienen las relaciones inmediatas
I = I1 + I2
I1 = I3 + Ig
I = I4 + I3
I4 = I2 + Ig
Cuando la corriente que pasa por el galvanómetro es nula, se tiene
I1 = I3
I2 = I4
Además, utilizando la ley de voltajes de Kirchhoff
−V + I2 R2 + I4 Rx = 0
−V + I1 R1 + I3 R3 = 0

---

### Página 330

I1 R1 − I2 R2 = 0
De esta última ecuación, se obtiene
I2 = I1

R1
R2

Además, igualando el valor de V
I2 R2 + I4 Rx = I1 R1 + I3 R3
I2 R2 + I2 Rx = I1 R1 + I1 R3
I1

R1
(R2 + Rx ) = I1 (R1 + R3 )
R2

Rx =

R2
R2 R3
(R1 + R3 ) − R2 =
R1
R1

Finalmente
Rx =

R2 R3
R1

---

### Página 331

Problema
En el circuito de la figura, la batería de más arriba y la de más abajo tienen la misma f.e.m
igual a ε. La del medio tiene 2ε. Las resistencias interiores de las baterías son iguales a r. Existe
una sola resistencia exterior R (ubicada como se ve en el dibujo). Designe las corrientes por I1 ,
I2 , I3 , como se ve en el dibujo

a) Calcule las tres corrientes en valor y signo.
b) Suponga que el punto a del circuito está conectado a tierra y calcule en tal caso el potencial
que tiene el punto b
#### Solución
Definimos un sentido arbitrario para las corrientes I1 ,I2 e I3 , como se ve en la figura

Resolvemos el circuito con la ley de voltajes de Kirchhoff (LVK). La ecuación para la malla
2 es
ε + rI2 − 2ε + (I2 + I1 )r = 0
−ε + 2rI2 + rI1 = 0
Para la malla 1
−2ε + (I1 + I2 )r + I1 R + ε + I1 r = 0
−ε + I2 r + I1 (R + 2r) = 0

De la primera ecuación obtenemos
I2 =

ε − rI1
2r

---

### Página 332

Así
−ε +

ε − rI1
+ I1 (R + 2r) = 0

−2ε + ε − rI1 + 2I1 (R + 2r) = 0
Finalmente
I1 =

ε
3r + 2R

y
I2 =

ε
rε
3rε + 2Rε − rε
ε(r + R)
−
=
=
2r 2r(3r + 2R)
2r(3r + 2R)
r(3r + 2R)

Por ultimo, I3 = I1 + I2
I3 =

ε
ε(2r + R)
ε(r + R)
+
=
r(3r + 2R) 3r + 2R
r(3r + 2R)

Como los valores obtenidos son todos positivos, los sentidos de las corrientes supuestos inicialmente son todos correctos.
b)

De la figura es claro que
VB − VA = I1 R + ε + I1 r = I1 (R + r) + ε

Como A está conectado a tierra, VA = 0
VB = ε + (R + r)

ε(R + 2r)
ε
=ε+
3r + 2R
2R + 3r

---

### Página 333

Problema
Considere la línea telegráfica de L metros de longitud, y de resistencia por unidad de largo
r[Ω/m]. Esta línea tiene una falla de resistencia R en un punto. Demuestre que la corriente
que lee un amperímetro ideal (de resistencia interna 0) conectado a un extremo de la línea es
mínima cuando la falla se encuentra en el medio de la distancia entre el transmisor y el receptor.
#### Solución
Supongamos que la falla está a una distancia x de uno de los extremos. El sistema queda
modelado por el siguiente circuito

Sea I1 la corriente por R1 , I2 la corriente por R2 e I la corriente por R. Es claro que
I = I1 − I2
Ahora, las ecuaciones de malla son las siguientes
−V + R1 I1 + R(I1 − I2 ) = −V + rxI1 + R(I1 − I2 ) = 0
R2 I2 + R(I2 − I1 ) = r(l − x)I2 + R(I2 − I1 ) = 0

De la primera ecuación
I1 =

V + RI2
R + rx

Reemplazando esto último
r(l − x)I2 + RI2 − R

V + RI2
=0
R + rx

RrlI2 − RxrI2 + r2 lxI2 − x2 r2 I2 + R2 I2 + RrxI2 − RV − R2 I2 = 0
I2 =

RV
Rrl + r2 lx − x2 r2

I2 =

RV
Rrl + r2 x(l − x)

---

### Página 334

Ahora veamos cuando esta corriente es mínima. Esto equivale a encontrar el x tal que el
denominador sea máximo
&
d %
Rrl + r2 xl − lr2 x2 = r2 l − 2lr2 x = 0
dx
r2 x = 2r2 l → x =

l

Es decir, la corriente medida es mínima cuando la falla se encuentra en la mitad de la línea

---

### Página 335

Problema
Obtener la resistencia equivalente entre A y B aplicando las leyes de Kirchhoff

#### Solución
La resistencia equivalente entre a y b se puede obtener al ver la relación entre el voltaje aplicado
y la corriente que circula por el circuito. Se tiene
VA − VB = IReq

LCK para el nodo A
I=

(VA − VD ) (VA − VC )
+
→ IR = 2VA − VC − VD
R
R

LCK para el nodo C
VC − VD VC − VB
VA − VC
=
+
→ VA = 3VC − VB − VD
R
R
R

Para el nodo D
VC − VD VA − VD
VD − VB
+
=
→ 3VD − VA − VC = VB
R
R
R

Y para el nodo B
VD − VB VC − VB
+
= I → IR = VC + VD − 2VB
R
R

---

### Página 336

Resolviendo
VB − VA = 3VD − VA − VC − 3VC + VB + VD
VB − VA = 4VD − VA − 4VC + VB → VD = VC
Es decir, la corriente entre D y C es cero. Así, el sistema queda
IR = 2VA − 2VC
VA = 2VC − VB
IR = 2VC − 2VB
Luego

VA + VB
= VC

Así
IR = VA − VB = IReq

Con lo que la resistencia equivalente es R

---

### Página 337

Problema
Calcular la diferencia de potencial entre los puntos a y b. Todas las fem tienen una resistencia
interna de 1 Ω

#### Solución
Para resolver este problema basta con notar que solo fluye corriente por la malla exterior, ya
que a y b forman un circuito abierto. Aplicando LVK alrededor del circuito se obtiene

2I + 2I + 12 + I + I + 2I − 8 + I = 0 → 9I = −4
I = −4/9A
Redefinamos I con su sentido correcto, es decir, el contrario al que habíamos supuesto. Así,
I = 4/9 en el sentido contrareloj.
Para obtener los potenciales en a y b, nos damos como referencia el punto c. Con esto
Va = 2I + Vc = 8/9 + Vc
Mientras que
Vc − 8 − I − 2I + 10 = Vb
+ 10 = Vc + 0, 667
Notar que no existe una caída de potencial a través de la resistencia de 3Ω ya que por ella
no pasa corriente. Finalmente
Vb = Vc − 8 −

Vb − Va = 0, 667 − 0, 888 = −0, 221V

---

### Página 338

11.5.

Circuitos RC

11.5.1.

Carga de un condensador

Considere el circuito de la figura. El condensador está conectado a una fuente de voltaje
DC (corriente continua) de fem ε. En t = 0 el interruptor S se cierra. Supongamos además que
el condensador inicialmente está descargado, q(t = 0) = 0

En particular, para t < 0, no hay voltaje entre los terminales del condensador, asi que éste
actúa como un corto circuito. Cuando t = 0, el interruptor se cierra y la corriente comienza a
fluir acorde con
ε
R
En este instante, la diferencia de potencial entre los terminales de la batería es la misma
que la diferencia de potencial a través de la resistencia. Esto inicia la carga del condensador.
Mientras éste comienza a cargarse, el voltaje a través de él aumenta en el tiempo
I0 =

q(t)
C
Para la malla utilizamos la ley de voltajes para un circuito cerrado, obteniendo
VC (t) =

−ε + VC (t) + I(t)R = 0
−ε +

q
dq
+ R=0
C
dt

Debido a que I debe ser la misma en todas las partes del circuito, la corriente a través de la
resistencia R es igual a la tasa de incremento de carga en las placas del condensador. El flujo de
corriente en el circuito irá decreciendo debido a que la carga presente en el capacitor haga cada
vez más difícil poner más carga en él. Una vez que la carga del condensador alcanza su maximo
valor Q, la corriente en el circuito caerá a cero. Esto es evidente al reescribir la ecuación de
malla como
I(t)R = ε − VC (t)

Así, el capacitor cargado satisface una ecuación diferencial de primer orden que relaciona la
tasa de cambio de carga con la carga en el condensador
dq
q"
1!
ε−
=
dt
R
C

---

### Página 339

Esta ecuación la podemos resolver con el método de separación de variables
dq
dq
dt →
=−
dt
q =
ε− C
R
q − Cε
RC
Ahora podemos integrar para obtener
ˆ q

dq
q = −
ε− C
RC

ln

#

ˆ t

dt

Lo que nos lleva a
q − Cε
−Cε

$

=−

t
RC

Finalmente, se obtiene
%
&
%
&
q(t) = Cε 1 − e−t/RC = Q 1 − e−t/RC
Donde Q = Cε es la cantidad máxima de carga almacenada por las placas. La independencia
temporal de q(t) se grafica en la figura

Teniendo la carga en el condensador, podemos determinar el voltaje a través de éste
&
%
q(t)
= ε 1 − e−t/RC
C
El gráfico del voltaje como función del tiempo tiene la misma forma que la carga a través
del condensador. De la figura, vemos que después de un tiempo suficientemente largo la carga
acumulada en el condensador tiende a
VC (t) =

lím q(t) = Cε = Q

t→∞

En el límite, el voltaje a través del condensador es igual al voltaje de la fuente y el proceso
de carga efectivamente termina
Q
q(t)
=
=ε
t→∞ C
C

lím VC (t) = lím

t→∞

La corriente en el circuito es igual a la razón de cambio de la carga en el condensador
I(t) =

dq
ε
= e−t/RC = I0 e−t/RC
dt
R

---

### Página 340

El coeficiente que acompaña a la exponencial es igual a la corriente inicial que fluye a través
del circuito cuando el interruptor fue cerrado en t = 0. El gráfico de la corriente en función del
tiempo es

La corriente en el circuito decrece exponencialmente en el tiempo. Se suele escribir de la
siguiente manera
I(t) = I0 e−t/τ
Donde τ = RC se llama constante de tiempo. En efecto, la unidad de τ en SI es el
segundo. La constante de tiempo τ es una medida del decaimiento temporal para la función
exponencial. Este decaimiento satisface la siguiente propiedad
I(t + τ ) = I(t)/e
Lo que muestra que despues de un tiempo τ la corriente cae por un factor de e−1 = 0,368,
como se ve en el gráfico. Similarmente, el voltaje a través del condensador también se puede
expresar en términos de esta constante
%
&
VC (t) = ε 1 − e−t/τ

Notar que inicialmente en t = 0, VC (t = 0) = 0. Después de un tiempo τ , la diferencia de
potencial a través del condensador ha aumentado un factor (1 − e−1 ) = 0,632 de su valor final.
&
%
VC (τ ) = ε 1 − e−1 = 0,632ε

---

### Página 341

11.5.2.

Descarga de un Condensador

Suponga ahora que el condensador ha sido cargado hasta un valor Q. Para t < 0, el interruptor está abierto y la diferencia de potencial a través del condensador está dada por VC = Q/C.
Por otro lado, la diferencia de potencial a través de la resistencia es cero por que no hay un
flujo de cargas, esto es I = 0. Ahora supongamos que en t = 0 el interruptor se cierra. El
condensador comenzará a descargarse

El condensador cargado ahora actúa como una fuente de voltaje para conducir corriente alrededor del circuito. Cuando el condensador se descarga (el flujo de electrones va desde la placa
negativa hasta la placa positiva), el voltaje entre sus extremos disminuye. Usando la ley de
Kirchhoff para un circuito cerrado
q(t)
− I(t)R = 0
C
Además se cumple
dq(t)
dt
El signo se debe al hecho de que un flujo de corriente implica una disminución en la diferencia
de polaridad de las placas del condensador. Así, la carga satisface la ecuación diferencial de
primer orden
I(t) = −

dq(t)
q(t)
+R
=0
C
dt
que también se puede resolver mediante el método de separación de variables
dq
=−
dt
q
RC
# $
ˆ q
ˆ t
q
t
dq
dt → ln
=−
=−
RC 0
Q
RC
Q q
Así
q(t) = Qe−t/RC
Y el voltaje a través del condensador es
VC (t) =

q(t)
Q
= ( )e−t/RC
C
C

---

### Página 342

El gráfico del voltaje a través del capacitor en función del tiempo

La corriente también decae exponencialmente en el circuito
I=−

Q −t/RC
dq
=
e
dt
RC

---

### Página 343

Problema
En el circuito de la figura, suponga que el interruptor ha estado abierto por un tiempo muy
largo. En t = 0 se cierra

a) Cual es la constante de tiempo antes de que se cerrara el interruptor?
b) Cual es la constante de tiempo después de que se cierra el interruptor?
c) Encuentre la corriente a través del interruptor como función del tiempo una vez que el interruptor se ha cerrado.
#### Solución
a) Antes que el interruptor se cerrara, las dos resistencias R1 y R2 están en serie con el condensador. Debido a que la resistencia equivalente es Req = R1 + R2 , la constante de tiempo
está dada por
τ = Req C = (R1 + R2 )C

Y la carga almacenada en el condensador es
&
%
q(t) = Cε 1 − e−t/τ
b) Una vez que el interruptor se cierra, el circuito cerrado a la derecha se vuelve un circuito
RC que decae con constante de tiempo τ ′ = R2 C. La carga comienza a decaer acorde a
q ′ (t) = Cεe−t/τ

c) La corriente a través del interruptor consiste en 2 fuentes, la corriente constante I1 del
circuito izquierdo, y la corriente que decae I2 del circuito RC. Las corrientes están dadas por
I1 =
I ′ (t) =

ε
R1

dq ′
ε
Cε
= − ′ e−t/τ = − e−t/R2 C
dt
τ
R2

Así, ya que I1 e I ′ van en la dirección hacia abajo a través del interruptor, la corriente total
será
I(t) = I1 + I ′ (t) =

ε
ε −t/R2 C
+
e
R1 R2

---

### Página 344

Problema
Considere el circuito de la figura. Sea ε = 40V , R1 = 8Ω, R2 = 6Ω, R3 = 4Ω y C = 4µF . El
condensador inicialmente está descargado

En t = 0 el interruptor se cierra.
a) Encuentre la corriente a través de cada resistencia inmediatamente después de que el interruptor es cerrado.
b) Encuentre la carga final del capacitor.
#### Solución
a) Inmediatamente después de que el interruptor se cierra, el condensador equivale a un corto
circuito, ya que el voltaje en t = 0 a través de éste es nulo. Es decir, en el instante justo en que
se cierra el interruptor el circuito equivale a

Para la malla 1
−ε + I1 R1 + R2 (I1 − I2 ) = 0
Para la malla 2
R2 (I2 − I1 ) + I2 R3 = 0

Reemplazando los valores numéricos, se tiene
−40 + 8I1 + 6(I1 − I2 ) = 0 → I1 =

40 + 6I2

6(I2 − I1 ) + 4I2 = 0 → I2 = I1
Resolviendo este sistema
70I1 = 200 + 18I1 → I1 = 3, 84A

---

### Página 345

con esto
I2 = 2, 3A
Finalmente la corriente por R2 será
I3 = I1 − I2 = 3, 84 − 2, 3 = 1, 54
Simulando el circuito, obtenemos las corrientes como función del tiempo

Notar que en t = 0 los valores coinciden con los obtenidos recién. Ver también como el
circuito llega a un estado estacionario en un margen de tiempo de los 120 µ s.
Por último, es claro como la corriente I3 decae rápidamente a cero a medida que el condensador
se va cargando.

b) Después de un tiempo, el condensador se carga totalmente y este pasa a comportarse
como un circuito abierto, es decir, a través del condensador no pasa corriente.(y tampoco por
R3 )

Así, es fácil notar que el voltaje final a través del condensador será igual al voltaje a través
de la resistencia R2 .
−ε + I(R1 + R2 ) = 0 → I =

=

Y el voltaje a través de R2 será
= 17, 14(V ) = VC (t = ∞)
Así, la carga final del condensador se puede obtener como
VR2 = IR2 = 6

Q(t = ∞) = CVC = 4µF ∗ 17, 14 = 6, 85 ∗ 10−5 C

---

### Página 346

El voltaje en el condensador en función del tiempo es

---

### Página 347

Problema
En el circuito de la figura, el interruptor se encuentra cerrado durante un tiempo muy largo.
a) ¿Cuál es la corriente en cada resistencia?
b) ¿Cuál es la carga en el condensador C?
c) En t=0 se abre el interruptor S. Encuentre la corriente que pasa por la resistencia R2 en
función de t.
d) ¿Cuánto tiempo debe pasar para que la carga en C disminuya hasta 4/5 del valor en t=0?

#### Solución
a) El interruptor ha estado cerrado durante un tiempo muy largo, esto significa que el condensador se ha cargado completamente. Cuando esto sucede, el condensador equivale a un circuito
abierto, es decir, no pasa corriente a través de él. Bajo estas circunstancias, sólo habrá corriente
por la malla 1, así

LVK en malla 1
−ε + I1 R2 + I1 R1 = 0 → I1 =

V
R1 + R 2

Que es la corriente por R1 y por R2 , por lo dicho anteriormente, la corriente por R3 es cero.

---

### Página 348

b) Para obtener la carga en el condensador, primero debemos obtener el voltaje a través de
él, y luego utilizar la relación que relaciona el voltaje con la carga acumulada
VC (t) = Cq(t)
Nos interesa la carga final del condensador, esto es
VC (t → ∞)
C
Como ya vimos, después de un tiempo suficientemente largo no hay corriente por la malla
derecha, así, no hay una diferencia de potencial a través de R3 . Por lo tanto el voltaje en el
condensador será igual al voltaje a través de R2
lím q(t) =

t→∞

lím VC (t) = VR2 = I1 R2

t→∞

VC (∞) =

V R2
R1 + R 2

q = CV =

V CR2
R1 + R2

y así

c) Notemos que al abrir el interruptor, no pasa corriente por la malla 1 y se inicia un proceso
de descarga en el condensador.

Si esto no parece evidente, veamos la ecuación de la malla 2
I2 R3 − VC (t) + R2 I2 = 0
q(t)
C
Notemos que I2 es positiva, es decir, el sentido que le asignamos es el correcto. Esto significa
que cargas positivas están dejando la placa positiva y están llegando a la placa negativa. Es
decir, la carga entre las placas va disminuyendo en la medida en que I2 sea positiva. Esto se
traduce en
I2 (R2 + R3 ) = VC (t) =

dq
dt
Así, obtenemos una ecuación diferencial de primer orden para q(t)
I2 = −

---

### Página 349

−

dq
q(t)
(R2 + R3 ) =
dt
C

dq
q(t)
(R2 + R3 ) +
=0
dt
C
Ecuación homogénea cuya solución es de la forma
q(t) = q0 e−t/(C(R2 +R3 ))
con q0 la carga inicial del condensador, calculada anteriormente como
q0 =

R2 V C
(R1 + R2 )

Finalmente,
I(t) = −

dq
q0
=
e−t/C(R2 +R3 )
dt
C(R2 + R3 )

d) Para determinar el tiempo que debe pasar para obtener 4/5 de la carga inicial, resolvemos
la ecuación
q0 = q0 e−t/(C(R2 +R3 ))
ln(4/5) = −

t
C(R2 + R3 )

con lo que
t = ln(5/4)(R2 + R3 )C

---

### Página 350

Problema
Dos baterías de FEM ε1 y ε2 y resistencias R1 y R2 se conectan en paralelo con una resistencia
R

a) Calcule la potencia entregada por cada batería
b) Ahora se reemplaza la resistencia R por un interruptor S y un condensador C en serie.

El interruptor se cierra en t=0
i) Calcule la carga q en el condensador como función del tiempo
ii) Calcule la corriente en cada resistencia como función del tiempo
#### Solución
a)Para obtener la potencia entregada por cada batería, debemos conocer la corriente que pasa
por cada una, y lo hacemos usando la LVK para las mallas 1 y 2, como se muestra en la figura

Para la malla 1
−ε1 + I1 R1 + R2 (I1 − I2 ) + ε2 = 0
En la malla 2
−ε2 + R2 (I2 − I1 ) + I2 R = 0

---

### Página 351

De la primera ecuación se obtiene

I1 =

R2 I2 + ε1 − ε2
R1 + R2

Reemplazando en la segunda
−ε2 + I2 (R2 + R) = I1 R2 =

R22 I2 + R2 (ε1 − ε2 )
R1 + R2

Así
−ε2 (R1 + R2 ) + I2 (R2 + R)(R1 + R2 ) = R22 I2 + R2 (ε1 − ε2 )
−ε2 (R1 + R2 ) + I2 (R2 R1 + R22 + RR1 + RR2 ) = R22 I2 + R2 (ε1 − ε2 )
I2 (R2 R1 + RR1 + RR2 ) = R2 (ε1 − ε2 ) + ε2 (R1 + R2 )
I2 =

ε1 R2 + ε2 R1
R(R1 + R2 ) + R1 R2

Y entonces, I1 está dada por
I1 =
I1 =

R2 I2 + ε1 − ε2
ε1 R22 + ε2 R1 R2 + (ε1 − ε2 )(R(R1 + R2 ) + R1 R2 )
=
R1 + R 2
(R(R1 + R2 ) + R1 R2 )(R1 + R2)

ε1 R22 + ε2 R1 R2 + ε1 RR1 + ε1 R1 R2 + ε1 RR2 − ε2 RR1 − ε2 RR2 − ε2 R1 R2
(R(R1 + R2 ) + R1 R2 )(R1 + R2)
I1 =

R(ε1 − ε2 )(R1 + R2 ) + R2 ε1 (R1 + R2 )
(R(R1 + R2 ) + R1 R2 )(R1 + R2)

Finalmente,
I1 =

R(ε1 − ε2 ) + R2 ε1
R(R1 + R2 ) + R1 R2

Y la corriente por la fem ε2 es
I3 = I1 − I2 =

R(ε1 − ε2 ) + R2 ε1 − ε1 R2 − ε2 R1
R(ε1 − ε2 ) − ε2 R1
=
R(R1 + R2 ) + R1 R2
R(R1 + R2 ) + R1 R2

Con esto, la potencia entregada por ε1 es
P1 = I1 ε1 = ε1

R(ε1 − ε2 ) + R2 ε1
R(R1 + R2 ) + R1 R2

Y la potencia entregada por ε2
P2 = −I3 ε2 = ε2

R(ε2 − ε1 ) + ε2 R1
R(R1 + R2 ) + R1 R2

---

### Página 352

b)

Aquí, la ecuación de la malla 1 es equivalente al caso anterior, donde se obtuvo
I1 =

R2 I2 + ε1 − ε2
R1 + R2

Para la malla 2
−ε2 + R2 (I2 − I1 ) + VC = 0 → −ε2 + R2 I2 − R2 I1 +

q
=0
C

Reemplazando I1

−ε2 + R2 I2 − R2 (
−ε2 +

R2 I2 + ε1 − ε2
q
)+ =0
R1 + R2
C

R22 I2 + R1 R2 I2 − R22 I2 − R2 (ε1 − ε2 )
q
+ =0
R1 + R2
C
I2

R1 R2
q
ε1 R2 + ε2 R1
+ =
R1 + R2 C
R1 + R2

Pero I2 = dq/dt
q
ε1 R2 + ε2 R1
dq R1 R2
+ =
dt R1 + R2 C
R1 + R2
ε1 R2 + ε2 R1
dq CR1 R2
+q =C
dt R1 + R2
R1 + R2
Sean
τ=

CR1 R2
ε1 R2 + ε2 R1
,A = C
R1 + R 2
R1 + R2

Entonces
dq
τ +q =A
dt
Cuya solución es
q(t) = A(1 − e−t/τ )
Con esto,
I2 (t) =
I1 (t) = (

dq(t)
A
= e−t/τ
dt
τ

R2
A
ε1 − ε2
) e−t/τ +
R1 + R2 τ
R1 + R2

---

### Página 353

Y la corriente por R2
I3 (t) = I1 (t) − I2 (t) = (

R2
A
ε1 − ε2
A
) e−t/τ +
− e−t/τ
R1 + R2 τ
R1 + R2
τ

---

### Página 354

Problema
Considere el circuito de la figura. Inicialmente el circuito ha estado abierto largo tiempo
a) Calcule la carga del condensador, con el interruptor abierto
b) Si el interruptor se cierra y transcurre mucho tiempo, encuentre la nueva carga del condensador

#### Solución
a) Antes que se cierre el interruptor, sólo se debe considerar el circuito de la derecha

Si ha pasado mucho tiempo, ha dejado de circular corriente y el condensador está cargado
completamente
Q = CV

b) Si se cierra el interruptor, el circuito es el siguiente

Como ha pasado mucho tiempo, el condensador está cargado y no hay corriente hacia él.

---

### Página 355

De esta forma, la corriente circula según

Se tiene
V1 + I(R1 + R2 ) − V2 = 0
Luego
I=

V2 − V1
R1 + R2

Con esto podemos determinar la diferencia de potencial entre los terminales del condensador

Sea
∆V = Vb − Va
−∆V + V1 + IR1 = 0
Luego
R1 V2 + R2 V1
R1 + R2
con esto, la carga almacenada en el condensador es
∆V =

Q = C∆V
Q=C

R1 V2 + R2 V1
R1 + R2

---

### Página 356

Problema
Inicialmente el condensador de capacidad C1 tiene carga Q0 , y el segundo condensador está descargado. Encuentre la pérdida de energía por calor de Joule al conectar ambos condensadores
mediante un conductor de resistencia R, como muestra la figura

#### Solución
Definimos la corriente por el circuito según se muestra en la figura

La ecuación de la malla entrega
−V1 + IR + V2 = 0
donde los voltajes entre los extremos de cada condensador se relacionan con las cargas
V1 =

Q1
C1

V2 =

Q2
C2

La ecuación a resolver es
−

Q1
Q2
+ IR +
=0
C1
C2

Pero Q1 , Q2 e I no son independientes. En efecto
I(t) =

dQ2
dQ1
=−
dt
dt

Notar que esto es consistente con
d
(Q1 + Q2 ) = 0
dt
pues por conservación de la carga
Q1 (t) + Q2 (t) = Q0

---

### Página 357

Luego, derivando una vez con respecto al tiempo
−

1 dQ1 dI(t)
1 dQ2
+
R+
=0
C1 dt
dt
C2 dt

dI(t)
I(t) +
I(t) = 0
R+
C1
dt
C2
#
$
dI(t)
+
=−
dt
R C1 C2

Finalmente

dI(t)
=−
dt
R

#

C1 + C2
C1 C2

$

I(t)

La solución de esta ecuación es
−R

I(t) = Ke

!

C1 +C2
C1 C2

"

t

donde K es una constante a determinar. Considerando que el condensador 2 está inicialmente
descargado
Q2 (0) = 0
Se tiene
Q2 (t) =

ˆ t

dτ I(τ ) = K

ˆ t

−R

dτ e

!

C1 +C2
C1 C2

"

t

KRC1 C2
Q2 (t) =
C1 + C2

#

−R

1−e

!

C1 +C2
C1 C2

" $
t

La constante K se puede determinar imponiendo que para todo t ∈ R+
−

Q1 (t)
Q2 (t)
+ I(t)R +
=0
C1
C2

Como Q1 (t) = Q0 − Q2 (t)
Q0 Q2 (t)
Q2 (t)
+
+ I(t)R +
=0
C1
C1
C2
$
#
C1 + C2
Q0
Q2 (t) + I(t)R = 0
+
−
C1
C1 C2
−

Reemplazando
#
$
#
!
" $
!
"
1 C1 +C2
1 C1 +C2
Q0
C1 + C2
C1 C2
−R
−R
t
t
C1 C2
C1 C2
−
+
=0
KR
1−e
+ RKe
C1
C1 C2
C1 + C2
−

Q0
+ KR = 0
C1

Luego

---

### Página 358

Q0
RC1
Equivalentemente uno podría haber notado que en t = 0, el condensador 2 se comporta
como un cortocircuito, y el voltaje inicial en el condensador 1 es
K=

V1 (0) =

Q0
C1

de forma que
I(0) =

V1 (0)
Q0
=
R
C1 R

La potencia disipada en la resistencia está dada por
P (t) = RI 2 (t) = R

Q20 −2 (CRC1 +CC2 ) t
1 2
e
R2 C12

y la energía perdida será
−∆E =

ˆ ∞

dt

1 +C2 ) t
Q20 − 2(C
Q20 C2
RC1 C2
e
=
RC12
2C1 (C1 + C2 )

Notar que es independiente de R! Esta pérdida de energía coincide exactamente con la diferencia de energía almacenada por el sistema antes y después de conectar ambos condensadores

---

### Página 359

Problema
Encuentre en el circuito de la figura la intensidad de corriente eléctrica por cada rama y la carga
en cada condensador al tiempo t. Asuma que inicialmente los condensadores están descargados

#### Solución
Definimos las corrientes que se indican en la figura, asi como las cargas en cada condensador

Por supuesto que debe tenerse
I(t) = I1 (t) + I2 (t)
Tomando el circuito cerrado que involucra a la fuente, la resistencia R1 y el condensador C1
se tiene
−V + I1 (t)R1 +

Q1
=0
C1

Por otro lado, considerando el circuito cerrado que contiene a V , R2 y C2
−V + I2 R2 +

Q2
=0
C2

Además se tiene
I1 (t) =

dQ1 (t)
dt

dQ2
dt
De esta forma, y derivando las ecuaciones obtenidas anteriormente
I2 (t) =

1 dQ1 (t)
dI1 (t)
+ R1
=0
C1 dt
dt
dI1 (t)
I1 (t) + R1
=0
C1
dt

---

### Página 360

luego
dI1 (t)
=−
I1 (t)
dt
R1 C1
del mismo modo

dI2 (t)
I2 (t)
=−
dt
R2 C2

Resolviendo
−

t

−

t

I1 (t) = K1 e R1 C1
I2 (t) = K2 e R2 C2
Las constantes K1 y K2 se determinan de forma inmediata al considerar que en t = 0 ambos
condensadores se comportan como un cortocircuito y entonces
V
R1
V
I2 (0) =
R2

I1 (0) =

con esto
V − R tC
e 1 1
R1
"
!
t
−
Q1 (t) = V C1 1 − e R1 C−1
I1 (t) =

V − R tC
e 2 2
R2
"
!
− R tC
Q2 (t) = V C2 1 − e
I2 (t) =

---

### Página 361

Parte V
Magnetostática. Campos variantes en
el tiempo

---

### Página 362

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 363

#### Capítulo 12
Magnetostática
El campo Magnético
Hemos visto que las cargas estáticas son fuentes de campo eléctrico. Además conocemos una ley
que nos permite saber cómo es la fuerza que un campo eléctrico ejerce sobre una carga puntual
(Ley de Coulomb). Ahora, sucede que si dos cargas se están moviendo, existe una fuerza adicional entre ellas debido a éste movimiento. Ésta fuerza se conoce como Fuerza Magnética.
Sin embargo, la fuerza magnética entre 2 cargas puntuales en movimiento relativo es muchísimo
menos intensa que la fuerza de Coulomb, por lo que se hace prácticamente imposible medir la
fuerza magnética entre 2 cargas puntuales. De todas formas, efectos magnéticos se pueden
medir al utilizar corrientes eléctricas en conductores (donde existe un número muy grande de
electrones en movimiento!)
En resumen, cargas en movimiento generan campos magnéticos (y entonces una corriente
eléctrica también), y a su vez, campos magnéticos actúan sobre cargas en movimiento (en
consecuencia, un campo magnético ejerce una fuerza sobre un conductor con corriente).

Comenzaremos por el estudio de la Magnetostática, es decir, el estudio de campos magnéticos
producidos por corrientes estacionarias. Con esto queremos decir
I=

dq
=C
dt

Recordando la ecuación de continuidad de la carga
⃗ · J(⃗
⃗ x, t) + ∂ρ(⃗x, t) = 0
∇
∂t
La condición de que las corrientes sean estacionarias entrega
∂ρ(⃗x, t)
⃗ · J(⃗
⃗ x) = 0
=0→∇
∂t
Más adelante veremos como se relacionan los campos eléctrico y magnético, y encontraremos
las leyes fundamentales de la electrodinámica.

---

### Página 364

⃗ Esto se puede verificar
Un imán permanente es una fuente natural de campo magnético B.
al mover un compás cerca de un imán, la aguja del compás se alineará en la dirección del campo
magnético producido por el imán, como se ve en la figura

Es decir, el efecto del imán sobre la aguja es el de un torque (Torque de Ampère). Una
barra magnética consiste de dos polos, que se designan como norte (N) y sur (S). Esto significa
que las líneas de campo emergen desde un polo (norte) y terminan en el opuesto (sur). Veremos
que los campos magnéticos siempre tienen esta característica, es decir, las líneas de campo
magnético siempre emergen y terminan en la misma fuente del campo. (No se han encontrado
monopolos magnéticos). Cuando se acercan 2 barras magnéticas, 2 polos iguales se repelen,
mientras que polos contrarios se atraerán

Al contrario de las cargas eléctricas, las cuales pueden estar aisladas, los 2 polos magnéticos
siempre vienen en pares. Cuando se quiebra un imán, se obtienen 2 nuevos imanes, cada uno
con polo norte y sur. En otras palabras, no existen monopolos magnéticos aislados

Se verá más adelante que éste resultado se resume en la tercera ecuación de Maxwell
⃗ · B(⃗
⃗ x) = 0
∇
Podría resultar, en principio, misterioso que un material genere campos magnéticos. Lo
único que hemos dicho es que cargas en movimiento generan campos magnéticos. Es sabido que
una de las fuerzas fundamentales que dan forma a los átomos es la fuerza eléctrica (que atrae
al electrón con el protón). El movimiento de electrones en un material genera entonces campos
magnéticos. En realidad, tener la visión de un electrón como una partícula que gira en torno al
núcleo no es muy correcto, lo que se debe usar a niveles atómicos es la Mecánica Cuántica. El
magnetismo en la materia es en general un fenómeno puramente cuántico y que tiene relación
con el espín del electron. Al igual que en electrostática vimos que las moléculas de un material
dieléctrico son levemente polarizadas ante la presencia de un campo eléctrico, y que entonces un
material se caracteriza por una suma de infinitos momentos dipolares, también se puede definir
un análogo magnético, el momento magnético. De todas formas, es algo que está presente en
todos los átomos. ¿Por qué entonces, no toda la materia presenta esta cualidad de generar un
campo magnético medible, como los objetos que hemos llamado imanes permanentes?. La respuesta es que, si bien cada átomo en un material contribuye generando un campo magnético, la

---

### Página 365

disposición de los momentos magnéticos puede ser tan aleatoria, que el efecto neto al sumarlos
es una cancelación de un campo magnético total. Los imanes son materiales cuyos momentos
magnéticos están todos alineados, y por esto es que cada uno contribuye del mismo modo a un
campo magnético total que es el que medimos en la cercanía de un imán.

12.1.

Fuerza magnética sobre una carga puntual

Aún no hemos establecido una expresión matemática para determinar el campo magnético
generado por una distribución de cargas en movimiento. Sin embargo, por el momento po⃗ x), en cierta región del espacio.
dremos asumir que simplemente existe un campo magnético, B(⃗
Estudiaremos primero cual es el efecto de un campo magnético sobre una carga puntual q en
movimiento, más adelante veremos cómo son creados los campos magnéticos. Consideremos una
partícula de carga q, que se mueve con cierta velocidad ⃗v (⃗x). Experimentalmente, se obtienen
las siguientes observaciones
1. La magnitud de la fuerza magnética F⃗B (⃗x) ejercida sobre la partícula cargada es proporcional a | ⃗v (⃗x) | y a q
⃗ x)
2. La magnitud y dirección de F⃗B (⃗x) depende de ⃗v (⃗x) y de B(⃗
⃗ x). Sin embargo, cuando
3. La fuerza magnética F⃗B (⃗x) desaparece cuando ⃗v (⃗x) es paralela a B(⃗
⃗ x), la dirección de F⃗B (⃗x) es perpendicular al plano formado por
⃗v (⃗x) forma un ángulo ϑ con B(⃗
⃗
⃗v (⃗x) y B(⃗x), y la magnitud de F⃗B (⃗x) es proporcional a sin ϑ
4. Cuando la carga cambia de signo, la dirección de la fuerza magnética se invierte

Todas las observaciones anteriores se pueden resumir en la siguiente expresión
⃗ x)
F⃗B (⃗x) = q⃗v (⃗x) × B(⃗

La magnitud de F⃗B (⃗x) está dada por

FB = |q|vB sin θ

⃗ x) es el tesla T = 1 N/Am. Notar que F⃗B (⃗x) es siempre perpenLa unidad en SI para B(⃗
⃗ x), de forma que una fuerza magnética no puede alterar la rapidez de la
dicular a ⃗v (⃗x) y B(⃗
particula. (No realiza trabajo sobre ella). En efecto
!
"
⃗ x)) · ⃗v (⃗x)dt = q(⃗v (⃗x) × ⃗v (⃗x)) · B(⃗
⃗ x) dt = 0
dW (⃗x) = F⃗B (⃗x) · d⃗x = q(⃗v (⃗x) × B(⃗

Si sobre la partícula sólo actúa una fuerza magnética, entonces el trabajo sobre ella es nulo,
y entonces su energía cinética es constante. (Luego el módulo de la velocidad es constante). Sin

---

### Página 366

embargo,la dirección de ⃗v (⃗x), sí puede ser alterada por la fuerza magnética. (De lo contrario, el
movimiento de una carga en un campo magnético sería extremadamente aburrido, simplemente
se movería en una línea recta)

12.2.

Movimiento de una carga en un campo eléctrico y
magnético uniforme

Una partícula de carga q se podría encontrar en una región del espacio en donde existen un
⃗ y un campo eléctrico E.
⃗ Así, sobre ella actuará una fuerza neta igual a
campo magnético B
!
"
⃗ + ⃗v × B
⃗
F⃗ = q E

esta es llamada fuerza de Lorentz . Ésto permite acoplar el electromagnetismo clásico con
la mecánica, en efecto, la trayectoria de la partícula es la solución de la segunda ley de Newton
!
"
d⃗p
⃗ + ⃗v × B
⃗
=q E
dt
Resolvamos el movimiento de una partícula sometida a la fuerza de Lorentz, en un caso
muy particular y sencillo, como se muestra en la siguiente figura

⃗ = E î, B
⃗ = B k̂. Se debe resolver
Es decir, se tienen dos campos uniformes y perpendiculares E
!
"
d⃗v
⃗ + ⃗v × B
⃗
=q E
dt
"
q !
d⃗v
=
E î + ⃗v × B k̂
dt
m
m

La velocidad de la partícula es, simplemente
⃗v = ẋî + ẏ ĵ + ż k̂
de forma que
"
q !
d
⃗v =
E î − ẋB ĵ + ẏB î
dt
m

---

### Página 367

De aquí se obtienen las siguientes ecuaciones diferenciales que describen el movimiento de
la partícula
z̈ = 0
qB
ÿ = − ẋ
m
$
#
qE
+ ẏB
ẍ =
m
Definiendo qB
= w0 y qE
= w1
m
m

z̈ = 0
ÿ = −w0 ẋ
ẍ = w1 + w0 ẏ

La solución de la primera de ellas es evidente, y está dada por
z(t) = z0 + voz t
es decir, la partícula describe un movimiento uniforme en la dirección z . Las ecuaciones
para la velocidad en x y en y están acopladas, y pueden ser escritas de forma matricial como
# $ #
$# $ # $
d ẏ
0 −w0
ẏ
=
+
ẋ
w
ẋ
w
dt
Es decir, se tiene un sistema de ecuaciones diferenciales no homogéneo de la forma
⃗x˙ = A⃗x + f⃗
Puede ser resuelto fácilmente de la siguiente manera
⃗x˙ − A⃗x = f⃗
e−At⃗x˙ − e−At A⃗x = e−At f⃗ =
entonces
−At

e

⃗x = ⃗x0 +

ˆ t

d % −At &
e ⃗x
dt

dτ e−Aτ f⃗(τ )

Finalmente
At

⃗x = e ⃗x0 +

ˆ t

dτ eA(t−τ ) f⃗(τ )

La solución homogénea es, simplemente
⃗xh = eAt⃗x0
donde x0 corresponde a ⃗x(t = 0). Para calcular eAt obtenemos los valores propios de A
'
'
'−λ −w0 '
' = λ2 + w02 = 0
| A − λI |= ''
w0 −λ '

---

### Página 368

Están dados por
λ1 = iw0 , λ2 = −iw0

Para encontrar eAt se puede utilizar el teorema de Caley-Hamilton ( o simplemente diagonalizar A)
eAt = a0 I + a1 A
donde a0 y a1 están dados por
eiw0 t = a0 + iw0 a1
e−iw0 t = a0 − iw0 a1
Resolviendo
a0 = cos w0 t
a1 =
sin w0 t
w0
Con esto
At

e

=

#

$ #
$
− sin w0 t
cos w0 t
+
cos w0 t
sin w0 t
$
#
cos w0 t − sin w0 t
eAt =
sin w0 t cos w0 t

y la solución homogénea queda
# $ #
$
v0y cos w0 t − v0x sin w0 t
ẏ
=
⃗xh (t) =
ẋ
v0y sin w0 t + v0x cos w0 t

Además, la solución particular toma la forma
$# $
ˆ t #
cos w0 (t − τ ) − sin w0 (t − τ )
dτ
⃗xp (t) =
sin
w
(t
−
τ
)
cos
w
(t
−
τ
)
w
$
$
#
ˆ t #
w1 cos w0 (t − τ ) ''t
w1 sin w0 (t − τ )
=
dτ
⃗xp (t) =
'
w1 cos w0 (t − τ )
w0 − sin w0 (t − τ ) 0
$
#
w1 1 − cos w0 t
⃗xp (t) =
sin w0 t
w0

Finalmente, se tiene

ẋ = v0y sin w0 t + v0x cos w0 t +
ẏ = v0y cos w0 t − v0x sin w0 t +

w1
sin w0 t
w0

w1
(1 − cos w0 t)
w0

---

### Página 369

Integrando, se obtiene la cinemática general para la partícula
v0y
v0y w1
v0x
w1
x(t) = −
cos w0 t +
sin w0 t − 2 cos w0 t +
+ 2 + x0
w0
w0
w0
w0
w0
#
$
v0y
v0x
w1
v0x
t−
y(t) =
sin w0 t +
cos w0 t +
sin w0 t −
+ y0
w0
w0
w0
w0
w0
z(t) = z0 + v0z t

12.2.1.

Trayectorias en casos particulares

Resuelta la ecuación de movimiento para la carga sometida a la fuerza de Lorentz, es posible
graficar y obtener su trayectoria para distintas condiciones iniciales y magnitudes de los campos.
La siguiente figura muestra una solución con q = 10 C, B = 110 T, E = 200 N/C, y x0 = y0 =
z0 = 0 (partícula que parte del origen)

Solución con velocidad inicial en z distinta de cero
El movimiento en la dirección vertical (eje z) es uniforme. Notar que la partícula tiene una
cierta velocidad de traslación en la dirección y, y no en la dirección x (dirección del campo
eléctrico), como se podría pensar. La razón se debe a que si bien el campo eléctrico ejerce una
fuerza según x con un incremento en la velocidad, ambos efectos se traducen en una fuerza
⃗ intensa en la dirección y. El efecto neto es una traslación general en dicha
magnética q⃗v × B
dirección

Misma solución anterior, ahora con velocidad inicial en x de 1 m/s

Trayectoria con velocidad inicial en y de 1 m/s

---

### Página 370

Ahora, ¿qué ocurre si el campo eléctrico es nulo?. Las soluciones quedan de la forma
x(t) = −
y(t) =

v0y
v0x
v0y
cos w0 t +
sin w0 t +
+ x0
w0
w0
w0

v0y
v0x
v0x
sin w0 t +
cos w0 t −
+ y0
w0
w0
w0
z(t) = z0 + v0z t

La partícula describe un movimiento circular en el plano x − y (¿cuál sería el centro?),
como se muestra en la figura

Este movimiento tiene una frecuencia angular de oscilación (constante) dada por
qB
m
En particular, si la velocidad inicial en la dirección z es nula, la trayectoria es definitivamente
una circunferencia en el espacio
w0 =

Así, una partícula en un campo magnético uniforme describe una trayectoria circular en el
plano perpendicular al campo magnético. Este movimiento circular es uniforme (frecuencia
angular constante). Esto último es evidente pues el campo magnético nunca realiza trabajo sobre
la partícula (y no modifica su energía cinética). Si v es el módulo de la velocidad, entonces se
tiene
v = w0 R
y el radio de la circunferencia descrita está dado por
R=

mv
v
=
qB
w0

El período de este movimiento circular estará dado por
T =

2π
2πm
=
w0
qB

---

### Página 371

Trayectoria general de una partícula en un campo magnético uniforme
Hay que notar que estas trayectorias han sido obtenidas a partir de campos extremadamente sencillos (uniformes). Muchísimos efectos interesantes se pueden lograr con campos que
varían en el espacio. Uno de ellos consiste en un campo magnético con curvatura en que bajo
ciertas condiciones se puede confinar a la partícula en determinadas regiones del espacio (espejos magnéticos). El confinamiento magnético parece ser la solución con más posibilidades
de permitir en el futuro la construcción de un reactor de fusión nuclear de potencia con fines
comerciales, la idea consiste en confinar un plasma a altas temperaturas lejos de las paredes
del reactor, de forma de poder replicar procesos de fusión nuclear (por ejemplo, la fusión de
Deuterio-Tritio)

Diseño de confinamiento de plasma utilizado en el International Thermonuclear Experimental
Reactor (ITER), en Francia

---

### Página 372

12.2.2.

El descubrimiento del electrón

Notar que existe una solución muy particular al movimiento de una partícula bajo la acción
de la fuerza de Lorentz cuando los campos son uniformes y perpendiculares. Resulta muy
interesante que para un determinado valor de la velocidad ⃗v una partícula cargada no siente
fuerza alguna. En efecto, supongamos una partícula cargada que ingresa a una región con
⃗ y un campo magnético B,
⃗ si la velocidad inicial de tal
prescencia de un campo eléctrico E,
partícula es
1 ⃗
⃗
⃗v = 2 E
×B
B
entonces su trayectoria será una línea recta, con velocidad constante y en la dirección de ⃗v .
Esto es fácil de demostrar, pues la fuerza de Lorentz que actúa sobre la carga es
#
$
!
"
⃗ + ⃗v × B
⃗ =q E
⃗+
⃗ × B)
⃗ ×B
⃗
F⃗ = q E
(E
B2
$
#
$
#
1 2⃗
1 ⃗
⃗
⃗
⃗
⃗
⃗
F = q E − 2 B × (E × B) = q E − 2 B E = ⃗0
B
B
Este fue el principio utilizado por JJ Thompson para medir la razón entre la carga y la
masa del electrón

Aparato de Thompson para estudiar la deflexión de partículas cargadas
La palabra átomo (que significa indivisible en Griego) fue propuesta por Demócrito, quien
vivió en Atenas (460-370 ac). El consideraba inconcebible que los objetos materiales pudiesen
ser divididos en partes cada vez más pequeñas, sin límite, y postuló la existencia de partículas
elementales, tan pequeñas que no son posibles dividirlas en partes más pequeñas. El distinguió cuatro tipos de átomos, y propuso que toda la materia está conformada por estos objetos
indivisibles. Hoy en día, la idea de Demócrito es transferida a partículas más pequeñas aún,
que constituyen la estructura interna de los átomos, y se espera que los electrones, protones, y
las demás partículas elementales sean realmente indivisibles.
Hacia el siglo 19, la atención de muchos físicos fue puesta en el paso de la electricidad a
través de los gases. Se sabía que los gases, siendo muy buenos aislantes eléctricos, a veces podían
conducir electricidad al ser sometidos a tensiones muy altas. Sin embargo, Sir Williams Crookes
mostró que el paso de la electricidad en gases tomaba una forma muy clara (en efecto, se ven
haces de luz) cuando la presión del gas es reducida a una pequeña fracción de una atmósfera

---

### Página 373

Los tubos de Crookes emitían luz de determinado color dependiendo de la naturaleza del
gas, y ellos aún brillan en las calles y ciudades de todo el mundo

Tubo de Crooke. Éste consiste de un ánodo y un cátodo entre los cuales se establece una
diferencia de potencial, al interior se tiene gas a baja presión
Al colocar un imán cerca del tubo, Crookes observó la deflección de estos rayos catódicos, tal
cual sucede con las partículas cargadas. Al mismo tiempo, Jean Perrin en Francia descubrió que
al colocar una placa metálica en el camino del haz, ésta adquiría una carga eléctrica negativa.
Todo esto parecía indicar que estos rayos se trataban de partículas cargadas negativamente
moviéndose a través del gas. Sin embargo, esta idea eran opuestas a las observaciones del físico
Philipp Lenard, quien habría encontrado que los rayos catódicos eran capaces de traspasar
varias pantallas puestas en su camino sin dejar agujeros en ellas. Lenard pensaba que sólo
ondas, y no un haz de partículas, podría hacer esto. La tarea de resolver estas contradicciones
experimentales, y probar que los rayos catódicos son en efecto un haz de partículas, y encontrar
las características físicas de éstas particulas, le fue dada a Joseph John Thompson por el Consejo
Supremo del progreso de la ciencia. Thompson fue un físico nacido en Manchester, que a los 40
años era director del famoso laboratorio de Cavendish en Cambridge. Asumiendo que los rayos
catódicos son partículas moviendose a alta velocidad, Thompson decidió medir su masa y su
carga, y una parte de esta investigación consistió en observar la deflexión de rayos catódicos en
un campo magnético

Los electrones con carga −e y masa m son emitidos del cátodo C y acelerados hacia A. Sea
la diferencia de potencial entre C y A ∆V = φa − φc . El cambio en la energía potencial del
electrón es igual al trabajo externo realizado para acelerarlo, por conservación de energía, la
energía cinética adquirida está dada por
1 2
mv = e∆V
y entonces la velocidad que adquieren los electrones al pasar por A es
v=

(

2e∆V
m

---

### Página 374

A continuación los electrones entran en una región donde existe un campo eléctrico (hacia
abajo en la figura), y un campo magnético perpendicular (hacia adentro de la hoja). Si las
partículas ingresan con velocidad
1 ⃗
⃗ = E î
E×B
B
B
se moverán en una línea recta, y pasarán por un agujero (en rojo) al final del selector de
velocidades. Así, se ajusta el valor de ∆V , E y B de forma que las partículas sean detectadas
al final del selector de velocidades. Cuando esto sucede, se obtiene
⃗v =

e
E2
=
m
2∆V B 2
Al medir E, B y ∆V , se obtiene la razón entre la carga y la masa del electrón. Esta es
aproximadamente
e
= 1,7588 × 1011 C/kg
m

Sir J.J. Thompson y sus aparatos
En esa fecha el valor de e habría sido obtenido experimentalmente gracias a los experimentos de electrólisis de líquidos de Faraday. De todas formas Thompson realizó un experimento
especial para medir la carga con gases ionizados. Este método se basó en el descubrimiento de
otro físico del laboratorio Cavendish, C.T.R Wilson. Gracias a esto Thompson logró medir el
valor de m, usando sus resultados para e/m, obteniendo
m = 9, 11 × 10−31 kg
y esta resultó ser 1840 veces más pequeña que la masa del átomo de Hidrógeno. Ésto fue un
gran descubrimiento, una partícula aproximadamente 2 mil veces más liviana que el átomo más
liviano! Thompson concluyó que las partículas que conforman los rayos catódicos eran cargas
eléctricas, y les llamó electrones. El visualizó el átomo como una esfera de un material masivo
cargado positivamente, con pequeños electrones esparcidos estáticamente a través del núcleo

---

### Página 375

Placa conmemorativa en Cambridge acerca del descubrimiento del electrón. Cortesía de mi
amigo Germán Vogel

Fig. 12.1: Joseph John Thompson
Joseph John Thompson(1856-1940) Físico Inglés. En 1870 estudió Ingeniería en la
Universidad de Manchester, y se trasladó a Trinity College de Cambridge en 1876. En 1884 se
convirtió en profesor de Física en Cavendish. Uno de sus alumnos fue Ernest Rutherford, quién
más tarde sería su sucesor en el puesto. Obtuvo el Premio Nobel en 1906, en reconocimiento
de los grandes méritos de sus investigaciones teóricas y experimentales en la conducción de la
electricidad generada por los gases. Fue nombrado caballero en 1908 y nombrado en la Orden
del Mérito en 1912. En 1918 fue nombrado Rector del Trinity College de Cambridge, donde
permaneció hasta su muerte.

---

### Página 376

12.3.

Ley de Biot-Savart

Hemos descrito rápidamente la fuerza que se ejerce sobre una partícula cargada en un campo
magnético. Experimentalmente, resulta mucho más accesible estudiar que ocurre cuando se
acercan dos conductores rígidos (es decir, son mantenidos en su posición) con corriente (dado
que en ellos hay muchísimos electrones en movimiento, los efectos magnéticos ser amplifican).
Consideremos una curva Γ en el espacio, que representa un conductor lineal que lleva una
corriente I. Vamos a recorrer esta curva en el sentido de la corriente. En el punto ⃗x ∈ Γ,
definimos un elemento de corriente infinitesimal dado por
⃗ x) = Id⃗x
dI(⃗
donde I es la magnitud de la corriente (es una constante) y d⃗x es el elemento de línea sobre la
curva Γ (Insisto en que su dirección apunta en el sentido de la corriente) .
Sean dos circuitos lineales, Γ1 y Γ2 , con corrientes I1 e I2 , respectivamente. Ambas curvas
serán parametrizadas de forma de ser recorridas en el sentido de sus respectivas corrientes

Tomamos un elemento de corriente en ⃗x′ sobre el circuito 1, y un elemento de corriente en ⃗x
sobre el circuito 2. La fuerza que ejerce el elemento de corriente 1 sobre el elemento de corriente
2 está dada por
#
$
µ0 I1 d⃗x′ × (⃗x − ⃗x′ )
⃗
dF2 (⃗x) = I2 d⃗x ×
4π
| ⃗x − ⃗x′ |3

donde µo = 4π10−7 (H/m) es la permeabilidad del vacío. Notar que esta impresionante
expresión es mucho más compleja que la ley de Coulomb, primero que nada, implica 2 productos
vectoriales. Es importante notar además que la fuerza resultante ya no apunta necesariamente
en la dirección que une ambos elementos de línea (No es una fuerza Central). Lo que sí se sigue
cumpliendo es que la magnitud de la fuerza decae según el cuadrado de la distancia. Ahora bien,
podemos obtener la fuerza que ejerce todo el circuito 1 sobre el elemento de línea 2, utilizando
el principio de superposición, e integrando como sigue
˛
µ0 I1 d⃗x′ × (⃗x − ⃗x′ )
⃗
F2 = I2 d⃗x × (
)
| ⃗x − ⃗x′ |3
Γ1 4π
Finalmente, la fuerza total sobre el circuito 2 está dada por
$
#˛
˛
′
′
I
µ
d⃗
x
×
(⃗
x
−
⃗
x
)
I2 d⃗x ×
F⃗2 =
| ⃗x − ⃗x′ |3
Γ2
Γ1 4π
µ0 I1 I2
F⃗2 =
4π

d⃗x × [d⃗x′ × (⃗x − ⃗x′ )]
| ⃗x − ⃗x′ |3
Γ1

˛ ˛
Γ2

---

### Página 377

Aparentemente esta fórmula presenta una asimetría y podría pensarse que no se satisface
la tercera ley de Newton. Sin embargo, se puede demostrar que esta ley es absolutamente
simétrica, de forma que
F⃗2 = −F⃗1
La demostración es la siguiente

[d⃗x · (⃗x − ⃗x′ )]d⃗x′ (d⃗x · d⃗x′ ) (⃗x − ⃗x′ )
d⃗x × [d⃗x′ × (⃗x − ⃗x′ )]
=
−
| ⃗x − ⃗x′ |3
| ⃗x − ⃗x′ |3
| ⃗x − ⃗x′ |3
#
$
d⃗x′ × [d⃗x × (⃗x − ⃗x′ )]
x − ⃗x′
′
′ ⃗
⃗
d⃗
x
·
∇
−
d⃗
x
·
d⃗
x
=
−d⃗
x
| ⃗x − ⃗x′ |3
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |3
El término de la izquierda es una diferencial exacta, de forma que
˛
˛
˛ ˛
µ0 I1 I2
µ0 I1 I2
x − ⃗x′
′
′ ⃗
⃗
⃗
−
d⃗x
d⃗x · ∇
d⃗
x
·
d⃗
x
F2 = −
4π
| ⃗x − ⃗x′ |
4π
| ⃗x − ⃗x′ |3
Γ1
Γ2
Γ2 Γ1
˛ ˛
µ0 I1 I2
⃗x − ⃗x′
⃗
F2 =
d⃗x · d⃗x′
4π
| ⃗x − ⃗x′ |3
Γ2 Γ1
Hemos obtenido una identidad para la fuerza que ejerce el circuito 1 sobre el circuito 2 que
es totalmente simétrica. De aquí es evidente que
F1 = −F2

12.3.1.

Campo de un circuito rígido, Biot-Savart

Hemos concluído que la fuerza sobre el circuito 2 es
#˛
$
˛
µ0 I1 d⃗x′ × (⃗x − ⃗x′ )
⃗
F2 =
I2 d⃗x ×
| ⃗x − ⃗x′ |3
Γ2
Γ1 4π

es fácil ver que la expresión entre paréntesis no depende en absoluto del circuito 2, es de
⃗ x),
hecho, un campo vectorial B(⃗
˛
⃗
⃗ x)
I2 d⃗x × B(⃗
F2 =
Γ2

⃗ ⃗x es el Campo Magnético en ⃗x debido a la corriente I1
B

Es decir

˛
I1 d⃗x′ × (⃗x − ⃗x′ )
µ0
⃗
B(⃗x) =
4π Γ1
| ⃗x − ⃗x′ |3
De esto podemos leer que el campo magnético en cualquier punto ⃗x debido a ésta corriente
⃗ x), de pequeños segmentos de
se puede calcular al sumar las contribuciones infinitesimales dB(⃗
conductor d⃗x

---

### Página 378

Esta es la ley de Biot-Savart, y da una expresión para la contribución al campo magnético
de un elemento de corriente Id⃗x
⃗ x) =
dB(⃗

µ0 I d⃗x′ × (⃗x − ⃗x′ )
4π
|⃗x − ⃗x′ |3

Fig. 12.2: Jean Baptiste Biot
Jean Baptiste Biot (1774-1862) Físico y matemático Francés. Estudió la polarización
de la luz cuando pasaba a través de soluciones químicas, y las relaciones entre la corriente
eléctrica y el magnetismo. La Ley de Biot-Savart describe como se genera el campo magnético
mediante una corriente estacionaria y se proporcionó el nombre gracias a su colaboración con
Félix Savart. Un cráter en la luna lleva su nombre en honor a sus contribuciones

12.4.

Fuerza sobre conductores de corriente

Habíamos obtenido que la fuerza sobre un circuito con corriente I2 es
F⃗2 =

˛

Γ2

⃗ x)
I2 d⃗x × B(⃗

⃗ x) es cualquier campo magnético externo
Donde B(⃗
Esto nos dice que para un conductor de forma arbitraria, la fuerza magnética se puede
obtener al sumar sobre las fuerzas actuando sobre pequeños segmentos que constituyen al
conductor. Sea un segmento diferencial denotado por d⃗x

---

### Página 379

Fig. 12.3: La figura ilustra el efecto de la fuerza magnética sobre conductores

Entonces la fuerza sobre un elemento infinitesimal de un conductor de carga es
⃗ x)
dF⃗B (⃗x) = Id⃗x × B(⃗
Anteriormente calculamos la fuerza sobre un conductor definido por una curva cerrada. Si
se desea encontrar la fuerza sobre un segmento de conductor entonces
ˆ b
⃗
⃗ x)
FB = I
d⃗x × B(⃗
a

donde a y b representan los extremos del conductor. Como ejemplo, consideremos un conductor
⃗ como se muestra
curvo que lleva corriente I y sumergido en un campo magnético uniforme B,
en la figura

Tenemos entonces que la fuerza sobre este conductor está dada por
ˆ b
⃗ x) = I (⃗xb − ⃗xa ) × B(⃗
⃗ x)
d⃗x) × B(⃗
F⃗B = I(
a

Notar que esto se debe a que el campo magnético es uniforme (sólo en este caso!). Sea ⃗l = ⃗xb −⃗xa
el vector dirigido desde a hacia b. Con esta notación
⃗
F⃗B = Id⃗l × B

---

### Página 380

Ahora veamos que sucede si el conductor constituye un circuito cerrado de forma arbitraria,
entonces la fuerza será
#˛
$
⃗
⃗
FB = I
d⃗x × B
Γ

Pero

˛

d⃗x = ⃗0

Γ

La fuerza magnética neta sobre un circuito cerrado en un campo magnético uniforme es
⃗
FB = ⃗0

12.5.

Torque sobre una espira

Veamos qué sucede cuando colocamos una espira rectangular que lleva corriente estacionaria
⃗ x) = B î paralelo al
I en el plano XY , ante la prescencia de un campo magnético uniforme B(⃗
plano de la espira

Vemos que las fuerzas magnéticas actuando en los segmentos 1 y 3 son nulas debido a que los
⃗ . Por otro lado, las fuerzas
vectores ⃗l1 = −bî y ⃗l3 = bî son paralelos al campo magnético B
magnéticas actuando en los segmentos 2 y 4 son
!
"
F⃗2 = I −aĵ × B î = IaB k̂
! "
⃗
F4 = I aĵ × B î = −IaB k̂

De aquí es claro que la fuerza neta es 0, algo que era de esperar por lo visto anteriormente.
Sin embargo, aun cuando la fuerza neta sobre la espira es nula, las fuerzas F⃗2 y F⃗4 producirán
un torque que genera una rotación de la espira con respecto al eje y. El torque con respecto al
centro de la espira es
!
"
!
"
!
"
!
"
⃗τc = −b/2î × F⃗2 + b/2î × F⃗4 = (−b/2)î × IaB k̂ + (b/2î) × −IaB k̂

---

### Página 381

#

$
IabB IabB
⃗τc =
+
ĵ = IabB ĵ = IAB ĵ
Donde A = ab representa el área de la espira. Es conveniente introducir el vector de área,
en este caso constante sobre la superficie limitada por la espira
⃗ = An̂
S
con n̂ el vector unitario en la dirección normal al plano de la espira. En este caso, tenemos
n̂ = k̂. La expresión para el torque se puede reescribir entonces como
⃗×B
⃗
⃗τ = I A

⃗ forma un
Consideremos ahora el caso más general donde la espira (o el vector de area S)
ángulo ϑ con respecto al campo magnético

De la figura

y el torque neto es

"
b!
− sin ϑî + cos ϑk̂ = −⃗r4
⃗r2 =

"
b!
τ̂c = ⃗r2 × F⃗2 + ⃗r4 × F⃗4 = 2⃗r2 × F⃗2 = 2 − sin ϑî + cos ϑk̂ × (IaB k̂)
⃗×B
⃗
τ̂c = IabB sin ϑĵ = I A

Se obtiene la misma expresión obtenida anteriormente. Notar que la magnitud del torque es
máxima cuando el vector normal a la espira es perpendicular al campo magnético. El torque es
nulo cuando la normal a la espira está orientada en la dirección paralela al campo magnético.
⃗ es, por definición, el momento magnético de la espira
El vector I A
⃗
⃗µ = I A

---

### Página 382

⃗ (perpendicular al plano de la espira).
La dirección de ⃗µ es la misma que el vector de área S
Con esto, el torque sobre una espira de corriente es
⃗
⃗τc = ⃗µ × B
Una espira en un campo magnético uniforme experimenta un torque hasta que su momento magnético esté completamente alineado con el campo magnético. Notar la analogía con el
torque que ejerce un campo eléctrico sobre un dipolo. En efecto, es posible definir un momento
magnético para una distribución general de corriente en el espacio. Así, cada átomo en un material estará caracterizado por un momento magnético, y el efecto de un campo magnético sobre
el material será el de alinear los momentos magnéticos de forma paralela al campo. Estos momentos magnéticos alineados (como sucede en un imán) también generarán un campo magnético

---

### Página 383

Problema
Considere el circuito cerrado de la figura que lleva una corriente I en el sentido contrario al
reloj. Un campo magnético uniforme apuntando en la dirección ĵ es aplicado. Encuentre la
fuerza magnética que actúa sobre el elemento rígido y el arco semicircular.

#### Solución
⃗ = B ĵ , llamemos F⃗1 y F⃗2 a las fuerzas actuando sobre
Tenemos un campo uniforme dado por B
el segmento rígido y la parte semicircular, respectivamente. La fuerza sobre el segmento rígido
es
#ˆ R $
#ˆ R $
⃗ × B ĵ = I
F⃗1 = I
dx
dx î × B ĵ = I2Rî × B ĵ = 2IRB k̂
−R

−R

Ahora, para calcular F⃗2 , notamos que elemento infinitesimal d⃗x en el semicírculo se puede
escribir como
d⃗x = dxêϕ = Rdϕ(− sin ϕî + cos ϕĵ)

⃗ es
La fuerza que actúa sobre un elemento dx
!
"
⃗ = IRdϕ − sin ϕî + cos ϕĵ × (B ĵ) = −IBRdϕ sin ϕk̂
dF⃗2 = Id⃗x × B

Integrando sobre el arco semicircular, tenemos
ˆ π
dϕ sin ϕ = −2IBRk̂
F⃗2 = −IBRk̂

Así, la fuerza neta que actúa sobre el circuito completo es

---

### Página 384

F⃗net = F⃗1 + F⃗2 = ⃗0
Consistente con el hecho de que la fuerza sobre un circuito cerrado en un campo magnético
uniforme es siempre nula

---

### Página 385

Problema
Un alambre delgado y rígido que lleva una corriente I es colocado a lo largo del eje x. Calcular
el campo magnético en el punto P . Analice el caso particular en que el alambre es simétrico
con respecto al eje y
¿Qué sucede cuando L → ∞?

#### Solución
Consideremos un elemento diferencial d⃗x′ = dxî que lleva una corriente I en la dirección x

Para calcular el campo magnético en el punto P utilizamos la ley de Biot-Savart. Según nuestra
elección del origen, se tiene ⃗x = a⃗j y ⃗x′ = xî. Así
⃗ x) =
dB(⃗

µ0 d⃗x′ × (⃗x − ⃗x′ )
I
4π
|⃗x − ⃗x′ |3

⃗x − ⃗x′ = aĵ − xî
y su magnitud es
|⃗x − ⃗x′ | =

√

a2 + x 2

Con esto, la contribución al campo queda
⃗ x) =
dB(⃗

µ0
I
4π

⃗ x) =
dB(⃗

!
"
dxî × aĵ − xî
(a2 + x2 )3/2

µ0
adxk̂
I 2
4π (a + x2 )3/2

Y el campo total en P será
⃗ ) = µ0 I
B(P
4π

ˆ L2

adxk̂
2 3/2
−L1 (a + x )

---

### Página 386

Notar además que
tan ϑ1 =

a
a
→ tan(−ϑ1 ) = −
→ −L1 = acot(−ϑ1 )
L1
L1

a
→ L2 = aϑ2
L2
Para resolver esta integral, utilizamos el siguiente gambito
tan ϑ2 =

x = actgϑ → dx = −a csc2 ϑdϑ
y la integral queda
⃗ = µ0 I
B
4π

ˆ ϑ2

dϑa(−a csc2 ϑ)k̂
2 3/2
−ϑ1 (a + a ctg ϑ)

Ahora nos comemos a la reina
ˆ ϑ2
ˆ ϑ2
µ0
−dϑ csc2 ϑk̂
µ0
⃗
B=
I
I
dϑ sin ϑk̂
=−
4πa −ϑ1 (1 + ctg 2 ϑ)3/2
4πa −ϑ1
⃗ = µ0 I (cos ϑ1 + cos ϑ2 ) k̂
B
4πa
En el caso simétrico en que ϑ2 = ϑ1 , y digamos que el largo total es 2L, entonces
cosϑ1 = √

L
L 2 + a2

y el campo es
⃗ = µ0 I √ L
B
k̂
2πa L2 + a2
De aquí es claro que si L → ∞, o , equivalentemente, θ1 → 0, θ2 → 0, el campo magnético
a una distancia a del conductor es
⃗ = µ0 I k̂
B
2πa
Notemos que en este límite, el sistema posee simetría cilíndrica, y las líneas de campo
magnético son circulares. Este resultado se comprobará más adelante con la ley de Ampère

---

### Página 387

Problema
Se lanza un electrón (carga -e) con velocidad inicial ⃗v en el medio de dos placas entre las cuales
⃗ constante (entrando a la hoja). Ignore todo efecto gravitacional
existe un campo mangético B
a) ¿Hacia dónde se deflecta la trayectoria?
b) ¿Cuál es la magnitud de la velocidad si la partícula choca exactamente con el fin de la placa?

#### Solución
La fuerza de Lorentz es la unión entre el electromagnetismo y la mecánica, y en general una
⃗ yB
⃗ está sometida a una fuerza
partícula de carga q en prescencia de campos E
!
"
⃗ + ⃗v × B
⃗
F⃗ = q E
donde ⃗v es la velocidad de la partícula. En este caso, q = −e, y el campo eléctrico es nulo.
De esta forma
⃗
F⃗ = −e⃗v × B
Dado que la velocidad inicial con que incide el electrón es perpendicular al campo magnético,
la trayectoria será una circunferencia en el plano x − y (siempre y cuando la partícula esté contenida en la región donde existe campo magnético)

Para analizar hacia donde se deflectará la partícula, basta con analizar que ocurre en el
instante inicial t = 0
⃗ = v î × −B k̂ = vB ĵ
⃗v (0) × B
Luego en t = 0 la fuerza es

F⃗ (0) = −evB ĵ

Es decir, la partícula se deflecta hacia abajo

---

### Página 388

b) Dado que el electrón impacta con el extremo derecho de la placa inferior, la trayectoria
de la partícula es la siguiente

La magnitud de la fuerza magnética sobre el electrón es constante y dada por
| F⃗ |= evB
y su dirección es radial (apuntando hacia el centro de curvatura). Por dinámica circular, se
tendrá
evB =

mv 2
R

R=

mv
eB

luego

por otro lado, se tiene
#

d
l + R−

$2

l2 + R2 − Rd +
R=

= R2

d2
= R2

l2 d
+
d

entonces
l2 d
mv
= +
eB
d
y el módulo de la velocidad del electrón resulta ser
#
$
eB l2 d
v=
+
m d

---

### Página 389

Problema
En la figura se muestran los componentes escenciales de un espectrómetro de masas. Éste es
utilizado para medir la masa de partículas cargadas. En una fuente se produce un ión de masa m
y carga q, el cual parte del reposo y es acelerado por una diferencia de potencial ∆V , entrando
⃗ uniforme (entrando a la hoja), y
a un proceso de selección, donde hay un campo magnético B
⃗ Sólo partículas con velocidad ⃗v constante abandonan el selector
un campo eléctrico deflector E.
(es un selector de velocidades). Las partículas emergentes entran a una segunda región donde
⃗ 0 (entrando a la hoja), la partícula sigue una trayectoria circular
existe otro campo magnético B
y se estrella en un detector a distancia 2r del punto de entrada

a) Encuentre la velocidad ⃗v
⃗
b) Encuentre el campo B
c) Finalmente, encuentre la masa m de la partícula
#### Solución
a) La velocidad v con que el ión entra al selector se obtiene por conservación de energía
1 2
mv = q∆V
donde el cambio en energía potencial se traduce en un aumento en la energía cinética
(
2q∆V
⃗v =
ĵ
m
b) Para que la velocidad de la partícula permaneza constante y salga a través del selector,
se requiere que la fuerza de Lorentz actuando sobre ella sea nula. Se tiene
"
!
⃗
⃗
⃗
F = q E + ⃗v × B
⃗ = E î, B
⃗ = −B k̂, ⃗v = v ĵ
donde E

qE î − qv ĵ × B k̂ = 0
qE î − qvB î = 0 → qE = qvB

---

### Página 390

y entonces
E
B=
=E
v

(

m
2q∆V

⃗ 0 , la partícula describe una circunc) Luego de ingresar a la región de campo magnético B
ferencia de radio r. La magnitud de la fuerza magnética es qvB0 . Por dinámica circular
qvB0 = m
m
qB0 =
r
Finalmente

(

v2
r

2q∆V
m

qB02 r2
m=
2∆V

---

### Página 391

Problema
Considere una espira circular que lleva corriente I en el sentido indicado por la figura. Calcule
el campo magnético a una distancia z en el eje de simetría de la espira

#### Solución
Utilizando la ley de Biot-Savart para un elemento infinitesimal de la espira
⃗ x) =
dB(⃗
en este caso, tenemos

µ0 I d⃗x′ × (⃗x − ⃗x′ )
4π
|⃗x − ⃗x′ |3

!
"
⃗x′ = R cos φî + sin φĵ = Rr̂(φ)
!
"
d⃗x′ = Rdφ −î sen φ + ĵ cos φ = Rdφφ̂

y

!
"
⃗x − ⃗x′ = z k̂ − R cos φî + R sin φĵ = −îR cos φ − ĵR sin φ + k̂z
|⃗x − ⃗x′ | = (R2 + z 2 )1/2

Así
⃗ x) =
dB(⃗

!
" !
"
Rdφ
−
î
sin
φ
+
ĵ
cos
φ
×
−
îR
cos
φ
−
ĵR
sin
φ
+
k̂z
µI

(R2 + z 2 )3/2

4π

⃗ x) = dφ
dB(⃗

µ0 I (R2 sin φ2 k̂ + Rz sin φĵ + R2 cos φ2 k̂ + Rz cos φî)
4π
(R2 + z 2 )3/2

⃗ x) = dφ
dB(⃗

µ0 I (R2 k̂ + Rz sin φĵ + Rz cos φî)
4π
(R2 + z 2 )3/2

---

### Página 392

Con esto
⃗ x) = µ0 I
B(⃗
4π

ˆ 2π

dφ

(R2 k̂ + Rz sin φĵ + Rz cos φî)
(R2 + z 2 )3/2

Las integrales según î y ĵ son cero, como era de esperarse por argumentos de simetría.
Finalmente el campo magnético a una distancia z del anillo es
⃗ x) = µ0 I
B(⃗
4π

ˆ 2π

dφ

µ0 I
R2
R2
k̂
=
k̂
(R2 + z 2 )3/2
2 (R2 + z 2 )3/2

---

### Página 393

Problema
Considere un disco muy delgado que tiene una densidad de carga superficial σ uniformemente
distribuída. El disco se pone a girar a velocidad angular w en torno a su eje. Encuentre el campo
magnético en el eje del disco

#### Solución
Se tiene una distribución de carga en movimiento (en efecto es una distribución de corriente), de
forma que ésta generará sin duda un campo magnético. Anteriormente se determinó el campo
magnético en el eje de un anillo de radio r con corriente I, esto es
⃗
B(z)
=

µ0 Ir2
2(z 2 + r2 )3/2

Podemos ver el disco como una superposición de anillos con corriente de ancho infinitesimal
dr, de esta forma por el principio de superposición el campo magnético total será la suma de
las contribuciones de estos anillos. Veamos que ocurre en la porción de disco comprendida entre
r y r + dr, con r ∈ (0, R)

La carga contenida en este anillo es
dq = σ2πrdr
la rotación le asocia a este anillo una corriente.

---

### Página 394

La carga dq da una vuelta completa en un tiempo
∆t =

2π
w

luego la corriente asociada es
dI =

dq
wσ2πrdr
=
= σwrdr
∆t
2π

el campo magnético a una distancia z sobre el eje del disco generado por este anillo es
⃗
dB(z)
=

drµ0 wσr3
µ0 dIr2
k̂ =
k̂
2(z 2 + r2 )3/2
2(z 2 + r2 )3/2

Entonces el campo total es
ˆ R
ˆ
µ0 wσ R
drµ0 wr3 σ
drr3
⃗
B(z) =
k̂
=
k̂
2 3/2
2 3/2
0 2(z + r )
0 (z + r )
Realizando el cambio de variable
u2 = z 2 + r2 , 2udu = 2rdr
ˆ

De esta forma

$
#
ˆ
ˆ
drr3
duu(u2 − z 2 )
z2
=
= du 1 − 2
(z 2 + r2 )3/2
u3
u
ˆ
drr3
z2 √ 2
z2
2+ √
=
=
u
+
z
+
r
(z 2 + r2 )3/2
u
z 2 + r2

#
$'
z2
µ0 wσ √ 2
'R
⃗
z +r + √
B(z) =
' k̂
z 2 + r2 0
#
$
√
z2
z2
µ0 wσ √ 2
⃗
z +R + √
− z −√
B(z) =
k̂
z 2 + R2
z2

µ0 wσ
⃗
B(z)
=

#

√

z 2 + R2 + √

µ0 wσ
⃗
B(z)
=

#

$
z2
− 2 | z | k̂
z 2 + R2

$
2z 2 + R2
√
− 2 | z | k̂
z 2 + R2

---

### Página 395

Problema
Considere dos bobinas de N vueltas de radio R, cada una perpendicular al eje de simetría, con
sus centros localizados en z = l/2 y z = −l/2. Existe una corriente constante I en el mismo
sentido en cada bobina, como se muestra en la figura. Encuentre el campo magnético en el eje
a una distancia z del centro de una de las bobinas. Verifique que la primera derivada del campo
en el punto medio es nula.

#### Solución
Del problema anterior, tenemos que para una espira circular con corriente I, radio R y a una
distancia z de su centro, el campo en el eje de simetría es
R2
µ0 I
⃗
k̂
B(⃗x) =
2 (R2 + z 2 )3/2
Como una bobina consta de N espiras circulares separadas por una distancia despreciable
con respecto a z, podemos utilizar el principio de superposición y obtener el campo provocado
por una bobina de N vueltas
R2
⃗ x) = µ0 N I
B(⃗
k̂
2 (R2 + z 2 )3/2
Ahora, sea un punto en el eje, a una distancia z del origen, el campo provocado por la
bobina de abajo es
R2
⃗ 1 (z k̂) = µ0 N I
k̂
B
2 (R2 + (z + l/2)2 )3/2
y el campo generado por la bobina de arriba
R2
⃗ 2 (z k̂) = µ0 N I
B
k̂
2 (R2 + (z − l/2)2 )3/2
Y el campo magnético total, por el principio de superposición
#
$
µ0 N IR2
⃗
k̂
B(z k̂) =
+
(R2 + (z − l/2)2 )3/2 (R2 + (z + l/2)2 )3/2

---

### Página 396

Notemos que la primera derivada con respecto a z está dada por
#
$
dB
µ0 N IR2
3(z − l/2)
3(z + l/2)
=
−
−
dz
((z − l/2)2 + R2 )5/2 ((z + l/2)2 + R2 )5/2
Se puede notar de inmediato que en el punto medio z = 0 se tiene
dB ''
=0
'
dz z=0

También se puede demostrar que si la distancia l entre ambas bobinas es R (radio de las
espiras), se obtiene que
d2 B ''
=0
'
dz 2 z=0
Esta configuración se conoce como Helmhotz coils (bobinas de Helmhotz). La gracia es que
el campo es aproximadamente uniforme en una pequeña región cercana a z = 0. Si se expande
en torno a este punto
1 ′′
B (0)z 2 + B ′′′ (0)z 3 + ...
2!
3!
B(z) = B(0) + B ′′′ (0)z 3 + ...
3!
Incluso se puede demostrar que la tercera derivada también es cero en z = 0, es decir, el
cambio en el campo en el punto medio para pequeñas variaciones de z es del orden de z 4 !!
B(z) = B(0) + B ′ (0)z +

---

### Página 397

Problema
Calcule el campo magnético en el centro de la circunferencia de la figura

#### Solución
Este problema se soluciona fácilmente utilizando el principio de superposición.
En el problema 2 ya se vió que la magnitud del campo eléctrico debido a un alambre rectilíneo
muy largo a una distancia a de él es
B1 =

µ0 I
2πa

En este caso, según el sentido de la corriente
⃗ 1 = µ0 I ĵ
B
2πR
Es decir, apunta hacia el fondo de la hoja. Ahora, del problema 3 obtuvimos el campo magnético
de un anillo a una distancia z del centro en el eje de simetría está dado por
R2 k̂
⃗ 2 = µ0 I
B
k̂
2 (R2 + z 2 )3/2
Como interesa el campo en el centro del anillo, z=0
⃗ 2 = µ0 I k̂
B
2R
Finalmente, por el principio de superposición, el campo resultante en el centro del anillo es
⃗ =B
⃗1 + B
⃗ 2 = µ0 I ĵ + µ0 I k̂
B
2πR
2R
#
$
µ0 I
⃗
B=
ĵ + k̂
2R
π

---

### Página 398

Problema
Una partícula de carga q y masa m entra con velocidad v en un campo magnético uniforme B
como se muestra en la figura. ¿Cuánto tiempo transcurre entre que la carga ingresa al campo
magnético y sale?

#### Solución
Es sabido que la fuerza magnética sobre una carga en movimiento q está dada por la fuerza de
Lorentz
⃗
F⃗ = q⃗v × B

Ésta fuerza es siempre perpendicular a ⃗v , luego, se sigue que ésta fuerza no ejerce trabajo.
Con esto, la energía cinética de la partícula es constante y entonces su rapidez también. La
trayectoria que sigue la partícula bajo este campo magnético uniforme es una hélice

Si se observa el movimiento proyectado en un plano perpendicular al campo magnético, la
trayectoria describe una semicircunferencia, hasta volver a salir de la región donde se encuentra
el campo magnético. Sea R el radio de ésta semicircunferencia, luego podemos determinar el
tiempo que demora en salir como
πR
2πR
=
T =
2v ′
v′
′
donde v es la componente de la velocidad que es perpendicular al campo magnético. Ahora
debemos determinar R. De la segunda ley de Newton

---

### Página 399

mv ′2
=F
R
donde F es la magnitud de la fuerza magnética que se ejerce sobre la partícula.
F = qvB sin(π/4) = qv ′ B
de esta forma

mv ′2
= qv ′ B
R
R=

Finalmente
T =

mv ′
qB

πm
π mv ′
=
v ′ qB
qB

---

### Página 400

Problema
Considere dos alambres paralelos separados por una dstancia a y que llevan corrientes I1 e I2
en la dirección x. Calcule la fuerza entre ambos conductores.

#### Solución
La fuerza magnética F⃗1 , que ejerce el alambre 2 sobre el alambre 1, se puede obtener como
F⃗1 = I1

ˆ

⃗
d⃗l1 × B

⃗ es el campo magnético creado por el conductor 2. Usando el resultado del problema
donde B
2, para alambres suficientemente largos, las líneas del campo magnético debido a I2 son círculos
⃗ 2 apuntando en la dirección tangencial. Así, en
concéntricos con el alambre 2, con el campo B
un punto arbitrario P sobre el alambre 1, tenemos
⃗ 2 = µ0 k̂
B
2πa
que apunta en dirección perpendicular al alambre 1, como se ve en la figura

Al ser este campo uniforme a lo largo del conductor 1, y siendo éste un alambre rectilíneo, la
fuerza que experimenta está dada por
⃗ 2 = I1 lĵ ×
F⃗1 = I1⃗l × B

#

µ0 I2
2πa

$

k̂ =

µ0 I1 I2 l
î
2πa

Claramente esta fuerza apunta hacia el conductor 2. Resulta evidente que F⃗2 = −F⃗1 . De
esta forma, 2 cables paralelos que llevan corriente en la misma dirección se atraerán. Por otro
lado, si las corrientes fluyen en direcciones opuestas, la fuerza resultante será repulsiva.

---

### Página 401

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 402

Problema
Calcular la fuerza resultante sobre la espira con corriente I2

#### Solución
Para obtener la fuerza total sobre la espira, sumamos las fuerzas sobre las secciones 1,2,3 y 4.

Tenemos
F⃗1 = I2

ˆ c

⃗1
d⃗l1 × B

el campo en la sección 1 es uniforme y está dado por
⃗ 1 = − µ0 I1 k̂
B
2πa
Así
F⃗1 = I2

ˆ c

dy ĵ × −

µ0 I1
k̂
2πa

µ0 cI1 I2
F⃗1 = −
ĵ × k̂
2πa
µ0 cI1 I2
F⃗1 = −
î
2πa

---

### Página 403

Ahora, para la sección 3
F⃗3 = I2

ˆ c

⃗3
d⃗l3 × B

con
⃗3 = −
B

µ0 I1
k̂
2π(a + b)

y entonces
F⃗3 = I2

ˆ 0
c

dy ĵ × −

µ0 I1
k̂
2π(a + b)

y obtenemos
µ0 cI1 I2
î
F⃗3 =
2π(a + b)
La fuerza sobre la sección 2 será
F⃗2 = I2

ˆ b

F⃗2 = −I2
Notemos que
F⃗4 = I2

ˆ 0
b

ˆ b

⃗2
d⃗l2 × B

dxî ×

−dxî ×

µ0 I1
k̂
2π(a + x)

−µ0 I1
k̂ = −F⃗2
2π(a + x)

F2 y F4 se cancelan, luego, la fuerza total sobre la espira es
#
$
µ0 cI1 I2
µ0 cI1 I2
−
î
2π(a + b)
2πa

Notar que en signo es negativo, es decir, la fuerza es atractiva.

---

### Página 404

Problema
Un circuito cuadrado rígido de lado L y masa M está pivoteado en torno a uno de sus ejes en
⃗ uniforme, y el campo gravitatorio. El circuito lleva una
prescencia de un campo magnético B
corriente I que es capaz de mantenerlo en equilibrio en un ángulo ϑ. Encuentre el sentido y
magnitud de dicha corriente

#### Solución
Para el equilibrio, se requiere que el torque neto sobre la espira con respecto a algún punto de
aceleración nula sea cero. Se escoge como origen el punto O ubicado en una de las esquinas de
la espira, como se muestra en la figura

Para el torque que ejerce el peso, usamos que la fuerza de gravedad se puede concentrar en
el centro de masa

"
l!
⃗
⃗τ = ⃗r × F =
sin ϑî − cos ϑĵ × −M g ĵ
⃗τ = −

M gl
sin ϑk̂

---

### Página 405

Por otro lado, el torque que ejerce la fuerza magnética es
⃗
⃗τ = m
⃗ ×B
donde m
⃗ es el momento magnético de la espira
m
⃗ = IAn̂ = Il2 n̂
Requerimos en primer lugar que este torque tenga dirección k̂. Luego n̂ debe tener la dirección de m
⃗ en el dibujo

⃗ = Il2 B cos ϑk̂
⃗τ = m
⃗ ×B
El equilibrio exige entonces
l
M g sin ϑk̂ − Il2 B cos ϑk̂ = 0
Luego, la corriente I debe ser
M g tan ϑ
2lB
La dirección debe ser acorde con la dirección del momento magnético, la cual se muestra en
la siguiente figura
I=

---

### Página 406

Problema
Un circuito cuadrado de lado a está suspendido en el centro de un enorme anillo fijo de radio
R, con R >> a por un hilo que ejerce un torque restaurador de magnitud τ = kϑ, con ϑ el
ángulo de torsión que forman los planos de ambos circuitos. Si por el circuito pequeño circula
una corriente i y por el grande I, encuentre en forma aproximada el valor de la constante k de
modo que ϑ = π/2 sea posición de equilibrio

#### Solución
⃗ que la corriente I produce en el centro del anillo (coinciEncontramos el campo magnético B
dente con el centro de la espira cuadrada). Como a << R, podemos considerar que el campo
es aproximadamente uniforme en una región que contenga a la espira cuadrada. El campo en
el centro es fácil de obtener con la ley de Biot-Savart
ˆ
µ0 I
⃗x − ⃗x′
⃗
B(⃗x) =
d⃗x′ ×
4π Γ
| ⃗x − ⃗x′ |
donde Γ es la curva que parametriza al anillo. Se tiene

⃗x = ⃗0, ⃗x′ = Rr̂(ϕ), d⃗x′ = Rdϕϕ̂, | ⃗x − ⃗x′ |= R
⃗ ⃗0) = µ0 I
B(
4π

ˆ 2π

dϕRϕ̂ ×

−Rr̂(ϕ)
R3

⃗ ⃗0) = µ0 I 2π k̂ = µ0 I k̂
B(
4πR
2R
El torque del campo magnético sobre la espira está dado por
⃗
⃗ ×B
⃗τ1 = m

El cual dependerá del ángulo que formen los planos de ambos circuitos

---

### Página 407

De acuerdo a la figura, en tal posición se tendrá un torque magnético dado por
⃗ = ia2 µ0 I sin ϑĵ
⃗τ1 = m
⃗ ×B
2R
En ϑ = π/2
⃗τ1 =

iIa2 µ0
ĵ
2R

Por otro lado, se tendrá un torque restaurador
⃗τ2 = −kϑĵ
en ϑ = π/2

π
⃗τ2 = −k ĵ

Para que ϑ = π/2 sea una posición de equilibrio
π
iIa2 µ0
−k =0
2R
Luego
k=

µ0 Iia2
πR

---

### Página 408

Problema
Considere la espira de corriente formada por segmentos radiales y arcos de circunferencia como
⃗ en el punto P.
se muestra en la figura. Obtenga el campo magnético B

#### Solución
Para obtener el campo magnético en P, utilizaremos el principio de superposición, notando que
el campo total en P será la suma de las contribuciones de las secciones 1,2,3,4 y 5

Si fijamos el origen en P , notamos inmediatamente que las contribuciones de los segmentos 1
y 5 son nulas, ya que en ambos casos el vector d⃗x′ es paralelo al vector ⃗x − ⃗x′ , con ⃗x = ⃗0
Para el sector 2

Tenemos
⃗2 =
dB
Utilizando coordenadas polares

µ0 d⃗x′ × (⃗x − ⃗x′ )
I
4π
|⃗x − ⃗x′ |3

---

### Página 409

′

!

d⃗x = bdφ − sin φî + cos φĵ

"

ya que P es el origen, ⃗x = 0, y por último el vector que va desde el origen al elemento diferencial
de corriente tiene magnitud b y la dirección del vector unitario radial en polares
!
"
′
⃗x = b cos φî + sin φĵ
Notar que

|⃗x − ⃗x′ |3 = | − ⃗x′ |3 = b3
con esto
!

"

µ0 dφ − sin φî + cos φĵ × −b(cos φî + sin φĵ)
Ib
4π
b3
"
!
dφ sin φk̂ + cos φ
µ0
⃗ 2 = µ0 I
dB
k̂ =
Idφk̂
4π
b
4πb

⃗2 =
dB

Así, el campo total en P debido al arco exterior es
ˆ φ
µ0
µ0 φ
⃗
dφk̂ =
I
k̂
B2 =
4πb 0
4πb
Ahora, para el arco interior (sección 4) el procedimiento es totalmente análogo, con la
diferencia de que la distancia ahora es a, y que la corriente va en el sentido opuesto al del arco
exterior
⃗ 4 = − µ0 φ k̂
B
4πa
Por último, para la sección 3, es fácil notar que su contribución es nula, ya que en este caso,
el vector d⃗x′ apunta en la dirección contraria al vector unitario radial en coordenadas polares,
y a su vez ⃗x′ apunta en la dirección radial, de esta forma, el producto vectorial d⃗x′ × (⃗x − ⃗x′ )
es 0 en todo el segmento 3. Resumiendo, solo los segmentos 2 y 4 contribuyen al campo en P,
y el campo total será la suma de ambas contribuciones
#
$
µ0 φ 1 1
⃗
⃗
⃗
B = B2 + B4 =
−
k̂
4π b a

---

### Página 410

Problema
Un conductor rectilíneo con corriente I baja por el eje y hasta el origen, y luego continua en
dirección horizontal. Muestre que el campo magnético en algún punto (x, y) con x > 0, y > 0
está dado por
+
)
µ
x
I
y
⃗
B(x,
y) =
k̂
+ + *
+ *
4π x y y x2 + y 2 x x2 + y 2

#### Solución
Sea P un punto sobre el plano (x,y) con x > 0, y > 0. El campo magnético en P será la
superposición del campo creado por la sección vertical y el de la sección horizontal. Sea Γ1 la
curva descrita por
Γ1 : ⃗x′ = ⃗x′ (t) = (0, −t) , t ∈ (−∞, 0)

Así d⃗x′ (t) = dt(0, −1) .Es fácil ver que esta curva representa el segmento vertical de conductor,
y es recorrido en el sentido de la corriente. El campo magnético en P se obtiene a partir de la
ley de Biot-Savart
ˆ
µ0
⃗x − ⃗x′
⃗
B1 (x, y) =
d⃗x′ I ×
4π Γ1
| ⃗x − ⃗x′ |3
⃗ 1 (x, y) = µ0 I
B
4π

ˆ 0

(x, y) − (0, −t)
µ0 I
−dtĵ ×
=
| (x, y) − (0, −t) |3
4π
−∞

⃗ 1 (x, y) = µ0 I
B
4π

ˆ 0

ˆ 0

−∞

µ0 Ix
dt %
=
k̂
&
3/2
4π
−∞
x2 + (y − t)2
xk̂

ˆ 0

−dtĵ × %
dt

−∞

La función a integrar es par, luego

⃗ 1 (x, y) = µ0 I k̂
B
4πx2

ˆ ∞

dt !

xî + (y − t) ĵ
&3/2
x2 + (y − t)2

!

x3 1 + (y−t)
x2

"3/2

1 + (y−t)
x

"3/2

Ahora se utiliza la sustitución tan ϑ = (y−t)
, sec2 ϑdϑ = − dt
, y entonces
x
x
ˆ

dt !

1 + (y−t)
x2

"3/2 = −x

ˆ

sec2 ϑdϑ
3/2

(1 + tan2 ϑ)

= −x

ˆ

sec2 ϑdϑ
= −x
sec3 ϑ

ˆ

dϑ cos ϑ = −x sin ϑ

---

### Página 411

Ahora, como tan ϑ = (y−t)
, es fácil ver que (es cosa de construír un triángulo rectángulo,
x
con un lado igual a (y − t), y otro igual a x)
(y − t)
sin ϑ = ,
x2 + (y − t)2

de forma que
⎛

⎞

)
+
'∞
I
(y
−
t)
I
y
µ
µ
'
⃗ 1 (x, y) = −
⎠' = −
k̂ ⎝ ,
k̂ −1 − *
B
4πx
4πx
x2 + y 2
x + (y − t)
+
)
µ
y
I
⃗ 1 (x, y) = 0
k̂
+ *
B
4π x x x2 + y 2
Ahora, el segmento horizontal está caracterizado por la curva
Γ2 : ⃗x′ (t) = (t, 0)
d⃗x′ = (1, 0)dt, t ∈ (0, ∞)
De la ley de Biot-Savart, obtenemos el campo magnético generado por esta sección
˛
ˆ
µ0 I
⃗x − ⃗x′
µ0 I ∞
(x − t, y)
′
⃗
B2 (x, y) =
d⃗x ×
=
dtî ×
′
4π Γ2
| ⃗x − ⃗x |
4π 0
((x − t)2 + y 2 )3/2
ˆ ∞
I
µ
y
⃗ 2 (x, y) =
B
dt
k̂
4π
((x − t)2 + y 2 )3/2
Esta integral es idéntica a la calculada anteriormente, sólo que intercambiando el rol de x e
y
⃗ 2 (x, y) = µ0 I
B
4π
Finalmente
µ0 I
⃗
B(x,
y) =
4π

)

)

x
+ *
y y x2 + y 2

+

k̂

y
1 1
x
+ *
+ + *
x y y x2 + y 2 x x2 + y 2

+

k̂

---

### Página 412

Problema
Un cilindro de radio a y largo h tiene una corriente superficial I uniformemente distribuída en
el manto. Calcule el campo magnético producido sobre su eje

#### Solución
El sistema se puede ver como un conjunto de espiras por las cuales circula una corriente infinitesimal dada por
Idz ′
h
puestas una al lado de la otra. Determinemos inicialmente el campo asociado a una espira
ubicada a una distancia z ′ del origen por la cual circula una corriente I. Por la ley de Biot Savart, el campo magnético originado por un elemento de corriente I es
⃗ z′ =
dB

µ0 dz ′ Id⃗l × (⃗r − ⃗r′ )
4πh | ⃗r − ⃗r′ |3

En este caso ⃗r = z k̂, ⃗r′ = ar̂ + z ′ k̂, d⃗l = adϑϑ̂
⃗ z′ =
dB

µ0 dz ′ Iadϑϑ̂ × (−ar̂ + (z − z ′ )k̂)
4πh
(a2 + (z − z ′ )2 )3/2

Integrando la componente según k̂ tiene que
′
⃗ z′ = µ0 dz
B
4πh

ˆ 2π
o

dϑIa2 k̂
(a2 + (z − z ′ )2 )3/2

Notar que existe una componente según r̂, sin embargo su integral es cero, como se podría
esperar por simetría.
Ia2 k̂
µ0 dz ′
⃗
′
Bz =
2h (a2 + (z − z ′ )2 )3/2

Este es el aporte de una sola espira, y por lo tanto, puede considerarse como un elemento
diferencial de campo magnético. El campo magnético total es
ˆ h
µ
Ia2
⃗ =
B
dz ′ 2
k̂
2h o
(a + (z − z ′ )2 )3/2
Usando el cambio z − z ′ = atanx, −dz ′ = asec2 x
ˆ
ˆ
µ0 x2 −dxIa2 asec2 x
µ o I x2
⃗
dxcosxk̂
B=
k̂ = −
2h x1 (a2 + a2 tan2 x)3/2
2 x1

---

### Página 413

⃗ = − µ0 I (sinx2 − sinx1 )k̂
B
2h
donde
sinx2 = *

z−h

a2 + (z − h)2
z
sinx1 = √
z + a2

Finalmente
µo I
z
⃗ = − µo I * z − h
√
B
k̂ +
k̂
2h a + (z − h)
z + a2

---

### Página 414

12.6.

Corrientes estacionarias extensas localizadas

Vamos a generalizar la ley de Biot-Savart para una distribución de corrientes localizadas en
un volumen V , como se muestra en la figura

Para calcular el campo magnético en ⃗x, se utiliza un modelo de anillos Biot-Savart. Sea
⃗x′ ∈ V , y Γ(⃗x′ ) una curva cerrada de corriente estacionaria, luego
˛
⃗x − ⃗x′′
µ
′
⃗ x) =
d⃗x′′ ×
dI(⃗x )
dB(⃗
4π
| ⃗x − ⃗x′′ |3
Γ(⃗
x′ )
Además

⃗ x′ ) = dI(⃗x ) ˆl(⃗x′ )
J(⃗
dS(⃗x′ )
′

luego
⃗ x)=
J(⃗
′

#

dI
dS

$'
'
' ′ t̂(⃗x′ )
⃗
x

⃗ x′ )
dI(⃗x′ ) = dS(⃗x′ )t̂(⃗x′ ) · J(⃗
con t̂(⃗x′ ) el vector unitario tangente a la curva Γ(⃗x′ ). Así
⃗x′ ∈ Γ(⃗x′ ) : dI(⃗x′ ) = dS(⃗x′ )J(⃗x′ )
Pero
⃗x′′ ∈ Γ(⃗x′ ) → dI(⃗x′′ ) = dI(⃗x′ ) = C
ya que es un elemento de corriente estacionaria. Luego
˛
⃗x − ⃗x′′
µ
⃗ x) =
dB(⃗
d⃗x′′ ×
dI(⃗x′′ )
4π Γ(⃗x′ )
| ⃗x − ⃗x′′ |3
˛
⃗x − ⃗x′′
µ0
ds′′ t̂(⃗x′′ ) ×
dS(⃗x′′ )J(⃗x′′ )
=
4π Γ(⃗x′ )
| ⃗x − ⃗x′′ |3
˛
′′
µ0
⃗ x′′ ) × ⃗x − ⃗x dS(⃗x′′ )
ds′′ J(⃗
=
4π Γ(⃗x′ )
| ⃗x − ⃗x′′ |3
El campo magnético total en ⃗x será
¨
˛
⃗x − ⃗x′′
µ0
′′
′′ ⃗ ′′
⃗
dS(⃗x ) ds J(⃗x ) ×
B(⃗x) =
4π
| ⃗x − ⃗x′′ |3

---

### Página 415

⃗ x) = µ0
B(⃗
4π

˚

⃗ x) = µ0
B(⃗
4π

˚

⃗ x′′ ) ×
d3 x′′ J(⃗

V

⃗x − ⃗x′′
| ⃗x − ⃗x′′ |3

⃗x − ⃗x′
d x J(⃗x ) ×
| ⃗x − ⃗x′ |3
V
3 ′

′

Este es el campo magnético generado por una distribución de corriente localizada dentro de un
volumen V

12.7.

Las dos leyes fundamentales de la magnetostática

Hemos obtenido, a partir de la ley de Biot-Savart y el principio de superposición la forma
general del campo magnético generado por una distribución de corriente localizada dentro de
un volumen V
˚
′
µ0
⃗
⃗ x′ ) × ⃗x − ⃗x
B(⃗x) =
d3 x′ J(⃗
4π
| ⃗x − ⃗x′ |3
V
Ahora utilizamos el lema

⃗
∇
entonces

⃗x − ⃗x′
=
−
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |3

⃗ x) = − µ0
B(⃗
4π

˚

V

⃗ x′ ) × ∇
⃗
d3 x′ J(⃗

⃗ x) = µ0 ∇
⃗ ×
B(⃗
4π

˚

d3 x′

V

| ⃗x − ⃗x′ |

⃗ x′ )
J(⃗
| ⃗x − ⃗x′ |

de forma que el campo magnetostático es el rotor de un campo vectorial, que llamaremos
potencial magnético vectorial
⃗ x) =
A(⃗

˚

d3 x′

V

y

⃗ x′ )
J(⃗
| ⃗x − ⃗x′ |

⃗ x) = ∇
⃗ × A(⃗
⃗ x)
B(⃗

De esta forma, la divergencia del campo magnético es siempre nula
⃗ · B(⃗
⃗ x) = 0
∇
Además, se tiene
˚
⃗ x′ )
J(⃗
µ0 ⃗
′
⃗
⃗
⃗
d3 x′
∇ × B(⃗x ) =
∇×∇×
4π
| ⃗x − ⃗x′ |
V
˚
˚
⃗ x′ )
⃗ x′ )
µ0 ⃗ 2
µ0 ⃗ ⃗
′
3 ′ J(⃗
3 ′ J(⃗
⃗
⃗
∇∇ ·
−
∇
∇ × B(⃗x ) =
dx
d
x
4π
| ⃗x − ⃗x′ | 4π
| ⃗x − ⃗x′ |
V
V
˚
˚
µ0 ⃗
3 ′⃗ ′
⃗ x′ )δ(⃗x − ⃗x′ )
⃗
=
+ µ0
d x J(⃗x ) · ∇
d3 x′ J(⃗
∇
′
4π
| ⃗x − ⃗x |
V
V

---

### Página 416

Si ⃗x ∈ V
˚
µ0 ⃗
′
⃗
⃗
⃗ x′ ) · ∇
⃗′
∇ × B(⃗x ) = − ∇
+ µ0 J(⃗x)
d3 x′ J(⃗
4π
| ⃗x − ⃗x′ |
V
˚
˚
⃗ ′ ⃗ x′ )
⃗ x′ )
J(⃗
µ0 ⃗
µ0
3 ′⃗ ′
3 ′ ∇ · J(⃗
⃗ x)
d x∇ ·
d
x
=− ∇
+
+ µ0 J(⃗
4π
| ⃗x − ⃗x′ | 4π
| ⃗x − ⃗x′ |
V
V
˚
⃗ ′ ⃗ x′ ) µ0 ˆ✞ˆ ☎ dS(⃗
⃗ x′ ) · J(⃗
⃗ x′ )
µ0
3 ′ ∇ · J(⃗
⃗
⃗ ✝✆
dx
= µ0 J(⃗x) +
∇
−
4π
| ⃗x − ⃗x′ |
4π
| ⃗x − ⃗x′ |
V
δV

Pero, si la distribución corriente está localizada dentro de V , no hay flujo de corriente a
través de δV , es decir
⃗ x) = 0, ⃗x ∈ δV
n̂(⃗x) · J(⃗
Además, la condición de corriente estacionaria significa
⃗ · J(⃗
⃗ x) = 0, ⃗x ∈ V
∇
De forma que
⃗ × B(⃗
⃗ x) = µ0 J(⃗
⃗ x)
∇

12.8.

Leyes fundamentales, forma diferencial

Hemos obtenido las siguientes ecuaciones diferenciales para el campo magnetostático
⃗ · B(⃗
⃗ x) = 0
∇
⃗ × B(⃗
⃗ x) = µ0 J(⃗
⃗ x)
∇
Recordar el teorema de Helmholtz! La teoría magnetostática es completa. La primera de
ellas contiene la información de que nunca han sido observados monopolos magnéticos. Se puede
obtener una forma integral, integrando sobre un volumen V
˚
⃗ · B(⃗
⃗ x) = 0
d3 x∇
V

utilizando el teorema de la divergencia
ˆˆ
✞☎ ⃗
⃗ x) = 0
x) · B(⃗
✝ ✆dS(⃗
S

Es decir, el flujo magnético sobre cualquier superficie cerrada es siempre nulo. La segunda
ecuación para el rotor
⃗ x)
⃗ × B(⃗
⃗ x) = µ0 J(⃗
∇
es la ley de Ampère, cuya forma integral y aplicaciones serán estudiadas en detalle en el
siguiente capítulo

---

### Página 417

#### Capítulo 13
Ley de Ampére
Se vió que cargas en movimiento son fuentes de campo magnético. En particular, corrientes
estacionarias en un conductor son fuentes de campos magnéticos estáticos (no varían en el
tiempo). Tal cual la ley de Gauss en electrostática puede ser muy util en problemas de geometría
simple, para campos magnéticos existe un equivalente, que es la ley integral de Ampère.
⃗ x)
Ésta se obtiene a partir de la ecuación para el rotor de B(⃗
⃗ × B(⃗
⃗ x) = µ0 J(⃗
⃗ x)
∇
Podemos integrar esta ecuación sobre una superficie S arbitraria
¨
¨
"
!
⃗ × B(⃗
⃗ x) = µ0
⃗ x) · ∇
⃗ x) · J(⃗
⃗ x)
dS(⃗
dS(⃗
S

S

Y utilizando el teorema de Stokes
˛
¨
⃗ x) = µ0
⃗ x) · J(⃗
⃗ x)
d⃗x · B(⃗
dS(⃗
Γ(S)

S

La integral de línea del campo magnético sobre una curva cerrada Γ (circulación), es proporcional al flujo de corriente sobre cualquier superficie cuyo contorno sea (Γ). Definiendo IΓ
como la corriente que cruza a S, entonces
˛
⃗ x) = µ0 IΓ
d⃗x · B(⃗
Γ

Ejemplo conocido es el campo magnético exterior de una distribución cilíndrica de corriente
(muy larga), como se ve en la figura. Debido a la simetría, la magnitud del campo magnético
debe ser constante a una distancia r del centro del conductor, y su dirección siempre tangente
a curvas circulares concéntricas con el conductor. De esta forma

---

### Página 418

˛

Γ

⃗ x) = 2πrB(r) = µ0 I
d⃗x · B(⃗

de donde

µ0 I
2πr
Problemas con simetría cilíndrica son muy sencillos de resolver con la ley de Ampère. El
campo interior al conductor se obtiene de la misma forma, pero teniendo en cuenta que en ese
caso la corriente encerrada por una trayectoria circular no es I, sino una fracción de ésta
B=

---

### Página 419

Problema
Considere un conductor cilíndrico de radio R y de extensión infinita, que lleva una corriente I
con una densidad de corriente no uniforme
J = αr
donde α es una constante (desconocida), y r es la distancia de un punto interior al conductor
al eje de simetría. Encuentre el campo magnético en todo el espacio

#### Solución
Dada la clara simetría cilíndrica, utilizamos la ley de Ampère para resolverlo. Sea Γ una curva
circular de radio r, con 0 < r < R concéntrica al eje de simetría del conductor. Es claro que
la magnitud del campo magnético sólo puede ser función de r, y su dirección tangente en todo
punto a la curva Γ. Así, veamos que ocurre con la circulación del campo
˛
⃗ x)
d⃗x · B(⃗
Γ

!

"

con ⃗x = r cos ϑî, sin ϑĵ , d⃗x = rdϑϑ̂, ϑ ∈ [0, 2π]
˛

Γ

⃗ x) =
d⃗x · B(⃗

ˆ 2π

⃗
dϑrϑ̂ · B(r)
= 2πrB(r)

Por la ley de Ampère, la circulación sobre Γ es igual a µ0 I(Γ) donde I(Γ) es la corriente que
atraviesa la superficie limitada por Γ.(Escogemos la superficie plana encerrada por Γ). Sea k̂ la
dirección del eje de simetría del cilindo (coindidente con el sentido de la corriente). Entonces
I(Γ) =

¨

Γ

⃗ x) · J(⃗
⃗ x) =
dS(⃗

ˆ 2π

ˆ r

dϑ

ˆ r

⃗ k̂
drrk̂ · J(r)

2παr3
drr =
I(Γ) = 2πα

De esta forma
2πrB(r) = µ0

2παr3

µ0 αr
⃗
ϑ̂
B(r)
=
Para encontrar el campo magnético exterior, se utilizan los mismos argumentos de simetría,
y se utiliza una nueva curva Γ circular de radio r > R. La ley de Ampère en este caso entrega
˛
⃗ x) = 2πr = µ0 I(Γ)
d⃗x · B(⃗
Γ

---

### Página 420

donde I(Γ) es la corriente que atraviesa cualquier superficie de contorno Γ. Por supuesto,
escogemos la superficie plana limitada por Γ
¨
ˆ 2π ˆ r
⃗
⃗
I(Γ) =
dS(⃗x) · J(⃗x) =
dϑ
drrk̂ · J(r)k̂
S

drr2 =

2παR3

pero J(r) = 0, r > R, luego
I(Γ) = 2πα

ˆ R

pero es claro que I(Γ) = I, luego
α=

3I
2πR3

y se tiene
2πrB(r) = µ0 I
µ0 I
⃗
B(r)
=
ϑ̂, r > R
2πr
µ0 Ir2
⃗
B(r)
=
ϑ̂, r < R
2πR3

---

### Página 421

Problema
Considere un conductor plano de ancho w e infinitamente largo, en el plano xy. Éste lleva una
corriente I en el sentido de eje x, como se muestra en la figura. Encuentre el campo magnético
en un punto P en el plano del conductor, a una distancia s de él

#### Solución
Considere una sección de conductor de ancho dr, paralela a la dirección de la corriente y a una
distancia r de P , como se ilustra en la siguiente figura

La cantidad de corriente contenida en este elemento diferencial está dada por
# $
dr
dI = I
w
Utilizando la ley de Ampère para este elemento de conductor (similar al de un conductor
lineal) se obtiene el ya conocido resultado
⃗ )=
dB(P

µ0 dI
k̂
2πr

µ0 Idr
k̂
2πrw
Por el principio de superposición, el campo magnético total se obtiene al integrar sobre el
conductor
⃗ )=
dB(P

ˆ s+w
µ0 I
µ0 I
dr
dr
k̂ =
k̂
2πrw
2πw s
r
s
#
$
µ0 I
s+w
⃗
ln
k̂
B(P ) =
2πw
s

⃗ )=
B(P

ˆ s+w

Notar que en el límite cuando w << s
ln

!
s+w
w" 1
≈ w
= ln 1 +
s
s
s

---

### Página 422

y entonces

⃗ ) ≈ µ0 I k̂
B(P
2πs
que es el campo a distancia s de un conductor rectilíneo de ancho despreciable, con corriente

I

---

### Página 423

Problema
Calcule el campo magnético dentro de un solenoide ideal de largo l, N vueltas y que lleva una
corriente estacionaria I.
#### Solución
Un solenoide es una bobina enrollada en forma helicoidal. La figura muestra las lineas de campo
magnético de un solenoide con corriente constante I

Vemos que si las vueltas están muy cercanas espacialmente, el campo magnético resultante
dentro del solenoide es parcialmente uniforme, siempre que la longitud del solenoide sea mucho
mas grande que su diámetro. Para un solenoide ideal, que es infinitamente largo con vueltas
infinitamente cercanas, el campo magnético dentro es uniforme y paralelo al eje x, y es nulo
fuera del solenoide. Podemos utlizar la ley de Ampère para calcular el campo magnético dentro
de un solenoide ideal. Una vista transversal de un solenoide ideal se muestra en la figura

Consideremos el camino rectangular de largo l y ancho w y en sentido contrareloj. La integral
⃗ x) a través de este camino es
de línea de B(⃗
ˆ
ˆ
ˆ
ˆ
˛
⃗
⃗
⃗
⃗
⃗ x)
d⃗x · B(⃗x) = d⃗x · B(⃗x) + d⃗x · B(⃗x) + d⃗x · B(⃗x) + d⃗x · B(⃗

Ahora, la integral sobre 1 es 0, ya que el campo es nulo en el exterior del solenoide. Las
integrales sobre 2 y 4 también son nulas, ya que el campo a lo largo de estas trayectorias es
perpendicular a d⃗x. Con esto, podemos estirar el camino cerrado de manera que encierre todo el
solenoide,notando que la corriente total que atraviesa la superficie encerrada por la trayectoria
es N I, con N el número de vueltas del solenoide
˛
⃗ x) = Bl = µ0 N I
d⃗x · B(⃗

Finalmente
B=

µ0 N I
l

---

### Página 424

Problema
Considere dos planos infinitos paralelos separados por una distancia b en el plano xy. En la
región interior existe una densidad de corriente uniforme J⃗ = J0⃗i. Encuentre el campo magnético
en todo el espacio

#### Solución
Podemos pensar la región de corriente como una superposición de conductores paralelos que
llevan corrientes en la direccion +x. De la figura, y por un argumento de simetría vemos que el
campo magnético en un punto P sobre la región apunta en la direccion −y

La componente z desaparece después de sumar todas las contribuciones debidas a todos los
conductores. Similarmente, se puede mostrar que el campo magnético en un punto dentro de la
región apunta en la dirección +y, y en un punto inferior a la región también según la dirección
+y.

---

### Página 425

Ahora podemos utilizar la ley de Ampère para encontrar el campo magnético debido a esta
distribución de corriente. Tomaremos las curvas cerradas que aparecen en la figura. Para el
campo exterior, integramos sobre la curva Γ1 . La corriente que atraviesa la superficie limitada
por Γ1 es
¨
⃗ x) = J0 (bl)
I(Γ1 ) =
.S(⃗x) · J(⃗
Notando que en la integral de línea los segmentos verticales no contribuyen (d⃗x perpendicular
⃗ x))
al campo B(⃗
˛
⃗ x) = B2l = µ0 I(Γ1 ) = µ0 J0 bl
d⃗x · B(⃗
Γ1

de donde
B = µ0 J0 b/2
Notamos que el campo magnético fuera es uniforme, independiente de la distancia a la
región entre ambos planos. Ahora encontremos el campo magnético interior. La corriente total
encerrada por el camino cerrado Γ2 es
¨
⃗ x) · J(⃗
⃗ x) = J0 2zl
I(Γ2 ) =
dS(⃗
Usando la ley de Ampère,
˛
⃗ x) · B(⃗
⃗ x) = B2l = µ0 I(Γ2 ) = µ0 J0 2zl
dS(⃗
Γ2

de donde
B = µ0 J 0 z
Notemos que en z=0 el campo magnético es nulo, como se requiere por simetría. Resumiendo
⃗ = − µ0 J0 b ĵ, z > b/2
B
⃗ = −µ0 J0 z ĵ, −b/2 < z < b/2
B
⃗ = µ0 J0 b ĵ, z < −b/2
B

---

### Página 426

Problema
Se tiene dos corrientes, ambas con igual sentido (en el dibujo, saliendo de la hoja). Una de
ellas es una corriente plana e infinita de densidad
lineal
Js , y la otra es una corriente cilíndrica
%
&
r
infinitamente larga cuya densidad es J = J0 1 − R . Encuentre el valor de J0 en función de Js ,
que hace que el campo magnético resultante en el punto P ubicado a distancia R/2 del centro
del cilindro sea nulo

#### Solución
El campo de la distribución plana de corriente fue obtenido en el problema anterior. De la
simetría es claro que su dirección es como se muestra en la figura

y entonces para encontrar su magnitud se utiliza la ley de Ampère, con una curva plana de
ancho l

˛

Γ

⃗ 1 (⃗x) = 2lB1 = µ0 Js lb
d⃗x · B

---

### Página 427

Luego, en la región superior a la distribución plana
⃗ 1 (⃗x) = − µ0 Js b ĵ
B
Para el cilindro, utilizamos nuevamente la ley de Ampère. Dada su extensión infinita, por
simetría el campo magnético en su interior debe ser función únicamente de la coordenada radial
r, y su dirección es tal que es tangente en todo punto a una curva circular concéntrica al cilindro

˛

Γ

⃗ 2 (⃗x) = µ0 Ienc
d⃗x · B

luego

ˆ 2π

ˆ r

!
r"
drrJ0 1 −
R
$
# 2
r3
r
2πrB2 (r) = µ0 J0 2π
−
3R
#
$
r
r2
⃗
B2 (⃗x) = µ0 J0
−
ϕ̂
2 3R

2πrB2 (r) = µ0

dϕ

En el punto P , se tendrá la superposición de ambos campos. Notar que en dicho punto, ϕ̂
coincide con la dirección ĵ, y entonces
#
#
$
$
R
R2
µ0 bJs
⃗
B(P ) = µ0 J0
−
−
ĵ
12R
para tener un campo magnético nulo, debe tenerse entonces
J0

bJs
R
=

Finalmente
J0 =

3bJs
R

---

### Página 428

Problema
Un cable de radio R lleva una densidad de corriente J⃗ = J0 k̂. El cable tiene un hoyo cilíndrico
de radio α paralelo al eje del cable, a distancia b de él. Muestre que el campo magnético dentro
de la cavidad es uniforme

#### Solución
Resolvemos el problema por superposición de dos corrientes, una del cilindro completo con
densidad de corriente J0 k̂, y otra en la cavidad con densidad −J0 k̂. El campo magnético al
interior de un cable con densidad de corriente J⃗ = J0 k̂ se puede obtener fácilmente con la ley
de Ampère

Tomando la curva circular de radio r, y dada la simetría cilíndrica de la distribución de corriente,
el campo magnético es constante y tangente sobre la curva. Así
˛
¨
⃗
d⃗x · B(⃗x) = B(r)2πr = µ0
dS(⃗x)k̂ · J0 k̂
Γ

S(Γ)

B(r)2πr = µ0 J0 πr2
µ0 J 0 r
⃗
ϑ̂(r)
B(r)
=

---

### Página 429

Sea entonces un punto arbitrario al interior de la cavidad, como muestra la figura

La superposición de los campos magnéticos es la siguiente

⃗ = µ0 J0 r1 ϑ̂1 − µ0 J0 r2 ϑ̂2
B
pero
ϑ1 = k̂ × r̂1
ϑ2 = k̂ × r̂2
luego
"
!
⃗ = µ0 J0 r1 k̂ × r̂1 − r2 k̂ × r̂2
B
"
!
⃗ = µ0 J0 k̂ × ⃗r1 − k̂ × ⃗r2 = µ0 J0 k̂ × (⃗r1 − ⃗r2 )
B
⃗ = µ0 J0 k̂ × ⃗b
B
el cual es un campo uniforme

---

### Página 430

Problema
Se tiene un conductor cilíndrico de radio R, muy largo, con corriente I, y un conductor plano
también muy largo con corriente superficial I ′ . Se supone que ambos conductores son paralelos
y que el conductor plano y el eje de la corriente cilíndrica son coplanares. Si el plano conductor
tiene ancho a, y el eje del cilindro se encuentra a distancia b del origen, encuentre
a) El campo magnético sobre el eje x, para x > a
b) La fuerza de interacción entre ambos conductores por unidad de largo

#### Solución
Resolvemos el problema por superposición. El plano de corriente puede ser visto como una
superposición de corrientes lineales muy delgadas, de ancho diferencial dx′ , como se muestra en
la figura

Nos concentramos entonces en la porción de plano contenida entre x y x + dx. Este alambre
lleva una corriente
dx
dI = I ′
a

---

### Página 431

El campo magnético sobre el eje a distancia x del origen (con x > a) se puede obtener mediante
la ley de Ampère, integrando sobre la curva circular Γ centrada en x′ y de radio x − x′ . La
magnitud del campo magnético alrededor de la curva es constante e igual a la magnitud del
campo en x
˛
′
⃗ x) = B(x)2π(x − x′ ) = µ0 I ′ dx
d⃗x · B(⃗
a
Γ
⃗
B(x)
=−

µ0 I ′ dx′
k̂
2πa(x − x′ )

Entonces el campo magnético en x debido a la distribución plana es
ˆ
'a
µ0 I ′ a dx′
µ0 I ′
′ '
⃗
B(x)1 = −
)
k̂
=
−
ln(x
−
x
' k̂
2πa 0 x − x′
2πa
Así, para x > a

′
⃗ 1 = − µ0 I ln
B(x)
2πa

#

x
x−a

$

k̂

Para el cilindro de radio R, distinguimos dos regiones: dentro y fuera del cilindro. El campo
magnético exterior se obtiene de una aplicación inmediata de la ley de Ampère

⃗ consistente con la dirección de la corriente, se indica en la figura
El sentido de B,
˛
⃗ x) = µ0 I
d⃗x · B(⃗
Γ

2πrB(r) = µ0 I
µ0 I
2πr
donde r es la distancia radial con respecto al centro del cilindro. De esta forma, en el punto
x, con a < x < b − R
B(r) =

⃗ 2 (x) =
B

µ0 I
k̂
2π(b − x)

---

### Página 432

Para x > b + R
⃗ 2 (x) = −
B

µ0 I
k̂
2π(x − b)

Ahora, para el campo al interior del conductor cilíndrico, nuevamente se utiliza la ley de
Ampère

˛

Γ

⃗ x) = B(r)2πr = µ0
d⃗x · B(⃗

B(r)2πr = µ0

¨

S(Γ)

¨

S(Γ)

⃗ x)
dS(⃗x)n̂(⃗x) · J(⃗

dS(⃗x)ĵ · J ĵ = µ0 Jπr2

donde
JπR2 = I → J =
B(r)2πr = µ0
B(r) = µ0

I
πR2

Ir2
R2

Ir
2πR2

---

### Página 433

Finalmente, tenemos lo siguiente. Para a < x < b − R
#
$
′
µ
I
I
µ
x
⃗
B(x)
=
−
ln
k̂
2π(b − x) 2πa x − a
Para b − R < x < b

⃗
B(x)
=
Para b < x < b + R

⃗
B(x)
=−
Para b + R < x

x
µ0 I(b − x) µ0 I ′
−
ln
2πR
2πa x − a

$

#

µ0 I(x − b) µ0 I ′
x
+
ln
2πR
2πa x − a

$

#

k̂

#

⃗
B(x)
=−

µ0 I
µ0 I ′
x
+
ln
2π(x − b) 2πa x − a

k̂

$

k̂

b) Para calcular la fuerza por unidad de largo que ejerce el cilindro sobre la distribución
plana de corriente, calculemos la fuerza que se ejerce sobre el segmento lineal de largo 1, y
ancho dx′ en la posición x′

La fuerza que actúa sobre este segmento es
dF⃗ (x′ ) =

µ0 I
I ′ dx′
I ′ dx′
ĵ × B2 (x′ )k̂ =
ĵ × k̂
a
a 2π(b − x)
dF⃗ (x′ ) =

I ′ µ0 Idx′
î
2πa(b − x)

Por superposición, la fuerza neta por unidad de largo que se ejerce sobre el plano es
ˆ a
µ0 II ′
î
dx′
F⃗ =
2πa(b − x)
#
$
′
II
µ
b
F⃗ =
ln
î
2πa
b−a

---

### Página 434

Problema
Suponga que tiene dos cables infinitamente largos con densidad lineal de carga λ, separados
por una distancia d, moviéndose a velocidad v constante. Encuentre el valor de v para que la
atracción magnética se compense con la repulsión eléctrica. ¿Es razonable este resultado?

#### Solución
El campo eléctrico generado por el cable izquierdo sobre el cable derecho está dado por
λ
ĵ
2πϵ0 d
De esta forma, la fuerza eléctrica por unidad de largo será
⃗ =
E

F⃗Le = λ

λ
λ2
ĵ =
ĵ
2πϵ0 d
2πϵ0 d

Por otro lado, los alambres en movimiento equivalen a una corriente
dq
λdx
=
= λv
dt
dt
El campo magnético generado por el cable izquierdo sobre el derecho es
I=

⃗ = − µ0 I k̂ = − µ0 λv k̂
B
2πd
2πd
En este caso, la fuerza magnética por unidad de largo sobre el cable derecho será
#
$
λv
µ
m
F⃗L = −I î × −
k̂
2πd
2 2

µ0 λ v
ĵ
F⃗Lm = −
2πd
Para que éstas fuerzas se anulen

F⃗Le + F⃗Lm = 0
λ2
µ0 λ 2 v 2
=
2πϵ0 d
2πd
= µ0 v 2
ϵ0

---

### Página 435

La velocidad debe ser
v=√

µ0 ϵ 0

Evaluando
v=*
= 3 × 108
−12
8,85 × 10
× 4π10−7
Esta es la velocidad de la luz en el vacío!. Claramente este curioso resultado no es razonable,
ya que para tratar problemas con velocidades altas se debe usar la electrodinámica relativista

---

### Página 436

13.1.

Potencial Vectorial

A partir de la ley de Biot-Savart se demostró que el campo magnético satisface la siguiente
relación integro-diferencial
⃗ x) = µ0 ∇
⃗ ×
B(⃗
4π

˚

d3 x′

V

⃗ x′ )
J(⃗
| ⃗x − ⃗x′ |

Es decir, el campo magnético es el rotor de un campo vectorial, cuya forma más general es
⃗ x) = µ0
A(⃗
4π

˚

V

d3 x′

⃗ x′ )
J(⃗
⃗ x)
+ ∇ψ(⃗
| ⃗x − ⃗x′ |

donde ψ es un campo escalar arbitrario(función de Gauge). Sea cual sea el campo ψ, el
⃗ x) = ∇
⃗ × A(⃗
⃗ x) es siempre el mismo. Veamos que
campo magnético obtenido a partir de B(⃗
ocurre con
⃗ · A(⃗
⃗ x) = µ0
∇
4π

˚

V

3 ′⃗

⃗
d x J(⃗x ) · ∇

⃗ · A(⃗
⃗ x) = − µ0
∇
4π

′

⃗ 2 ψ = − µ0
+∇
′
| ⃗x − ⃗x |
4π

˚

V

⃗ x′ ) · ∇
⃗′
d3 x′ J(⃗

⃗ 2ψ
+∇
| ⃗x − ⃗x′ |

˚
⃗ x′ )
⃗ ′ ⃗ x′ )
J(⃗
µ0
3 ′ ∇ · J(⃗
⃗ 2ψ
d x∇
d
x
+
+∇
′ |
′ |
|
⃗
x
−
⃗
x
4π
|
⃗
x
−
⃗
x
V
V

˚

3 ′⃗ ′

la condición de corriente estacionaria entrega
˚
⃗ ′
µ
⃗ ′ J(⃗x ) + ∇
⃗ · A(⃗
⃗ x) = −
⃗ 2ψ
d3 x′ ∇
∇
′ |
4π
|
⃗
x
−
⃗
x
V
y del teorema de la divergencia
ˆˆ
⃗ x′ )
µ
J(⃗
✞ ☎⃗ ′
⃗ · A(⃗
⃗ x) = −
⃗ 2ψ
∇
d
S(⃗
x
+∇
)
·
✝✆
4π
| ⃗x − ⃗x′ |
La condición de corriente localizada da
⃗ · A(⃗
⃗ x) = ∇
⃗ 2ψ
∇

Para todo ψ. De esta forma, podemos perfectamente escoger un Gauge tal que
⃗ · A(⃗
⃗ x) = 0
∇

Este es llamado Gauge de Coulomb.

13.2.

Ecuación de Poisson y Laplace

⃗ x) tal que
Como el campo magnético es de divergencia nula, existe un campo vectorial A(⃗
⃗ x) = ∇
⃗ × A(⃗
⃗ x)
B(⃗
Luego

⃗ × B(⃗
⃗ x) = ∇
⃗∇
⃗ × A(⃗
⃗ x) − ∇
⃗ 2 A(⃗
⃗ x)
∇

El potencial puede ser escogido como un campo de divergencia nula (Gauge de Coulomb),
luego

---

### Página 437

⃗ × B(⃗
⃗ x) = −∇
⃗ 2 A(⃗
⃗ x)
∇
Además, de la forma diferencial de la ley de Ampère
⃗ × B(⃗
⃗ x) = µ0 J(⃗
⃗ x)
∇
De esta forma, el potencial vectorial bajo el gauge de Coulomb satisface la ecuación de
Poisson
⃗ 2 A(⃗
⃗ x) = −µ0 J(⃗
⃗ x)
∇
en regiones del espacio libre de corrientes, se obtiene la ecuación de Laplace
⃗ x) = 0
⃗ 2 A(⃗
∇

---

### Página 438

13.3.

Expansión Multipolar del campo magnético

Sea una distribución localizada de corriente dentro de un volumen V . El potencial vectorial
está dado por
⃗ x) = µ0
A(⃗
4π

˚

d3 x′

V

⃗ x′ )
J(⃗
| ⃗x − ⃗x′ |

Veamos que ocurre muy lejos de las fuentes, es decir, analizaremos el caso | ⃗x′ |<<| ⃗x |
′ −1

%

&
′ −1/2

′ 2

| ⃗x − ⃗x | = | ⃗x | + | ⃗x | −2⃗x · ⃗x

La expansión en taylor a primer orden entrega

=
| ⃗x |

#

| ⃗x′ |2 2⃗x · ⃗x′
−
1+
| ⃗x |2
| ⃗x |2

$−1/2

⃗x · ⃗x′ 1 | ⃗x′ |2
≈
+
−
+ ...
| ⃗x − ⃗x′ |
| ⃗x | | ⃗x |3 2 | ⃗x |3

Luego, el potencial vectorial lejos de las fuentes tiene la forma
˚
˚
µ0
µ0
3 ′⃗ ′
⃗ x′ )⃗x′ · ⃗x + ...
⃗
d x J(⃗x ) +
d3 x′ J(⃗
A(⃗x) =
4π | ⃗x |
4π
|
⃗
x
|
V
V

Ahora, la primera integral es nula, para ello demostraremos el siguiente lema: ∀f, g
˚
⃗ x) · [f (⃗x)∇g(⃗
⃗ x) + g(⃗x)∇f
⃗ (⃗x)] = 0
d3 xJ(⃗
V

la demostración es la siguiente
˚
" ˚
" ˚
!
!
⃗ x) · ∇f
⃗ g =
⃗ g −
⃗ · Jf
⃗ · J(⃗
⃗ x)
d x J(⃗
d x∇
d3 xf g ∇
V

V

V

Usando la condición de corriente estacionaria y el teorema de la divergencia
˚
!
" ˆˆ
☎ ⃗
⃗ x) · ∇f
⃗ g = ✞
⃗ x)f g = 0
d x J(⃗
x) · J(⃗
✝ ✆ dS(⃗
V

δV

Tomando f (⃗x) = 1, g(⃗x) = x
˚
V

⃗ x) · ∇x
⃗ =
d xJ(⃗

˚

d3 xJx (⃗x) = 0

V

Del mismo modo se puede demostrar que la integral de las componentes en y e z es nula.
Así
˚
⃗ x) = ⃗0
d3 xJ(⃗
V

En otras palabras, corrientes estacionarias localizadas no generan monopolos magnéticos!.
Mas aún, utilizando el mismo teorema , podemos encontrar una nueva expresión para la segunda
integral de la expansión. Tenemos
˚
⃗ x) · [f (⃗x)∇g(⃗
⃗ x) + g(⃗x)∇f
⃗ (⃗x)] = 0, ∀f, g
d3 xJ(⃗
V

tomando la componente a-ésima
˚

V

⃗ a (f g) = 0
d3 xJ⃗a (⃗x)∇

---

### Página 439

tomando f g = xb xc
˚

V

⃗
d xJ⃗a ∇a(x
b xc ) =

=

˚

˚

d3 xJ⃗a (xb δac + xcab )

V

d3 x (Jc xb + Jb⃗xc ) = 0

V

luego
˚

d3 x[xa Jb (⃗x) + xb Ja (⃗x)] = 0

V

De esta forma, tomando la componente a-ésima de la siguente integral
$
#˚
˚
˚
3 ′⃗ ′ ′
3 ′ ′ ′
d x J(⃗x )⃗x · ⃗x =
d x Ja x b x b =
d3 x′ (Ja′ x′b − Jb′ x′a ) xb
V
V
V
a
y es fácil verificar que
#˚
$
# ˚
!
"$
3 ′⃗ ′ ′
3 ′
′
′
⃗
d x J(⃗x )⃗x · ⃗x =
d x [⃗x × J(⃗x ) × ⃗x ]
V
V
a
a
Así, se obtiene

⃗ x) ≈ µ0 ⃗x ×
A(⃗
4π | ⃗x |3

˚

V

⃗ x′ ) × ⃗x′
d3 x′ J(⃗

Se define el momento magnético de una distribución de corriente localizada en V como
˚
⃗ x′ )
d3 x′⃗x′ × J(⃗
µ=
V

⃗ x) = µ0 ⃗µ × ⃗x
A(⃗
4π | ⃗x |3

Es decir, el potencial vectorial (y por lo tanto el campo magnético) muy lejos de la fuente
está completamente determinado (a primer orden) por el momeno magnético de la distribución
de carga.

---

### Página 440

13.4.

Magnetismo en la materia

13.4.1.

Magnetización

La materia consiste en de una colección de momentos magnéticos. En los materiales no
magnéticos, estos momentos están alineados de forma arbitraria, así se cancelan unos a otros y
no hay un efecto neto de campo magnético debido a este material. Sin embargo, como hemos
visto, ante la prescencia de un campo magnético externo, los momentos magnéticos en el interior
del material se alinearán en la dirección paralela al campo

Fig. 13.1: Momentos magnéticos en un material se alinearán en la dirección paralela al campo
externo
Estos momentos magnéticos crearán a su vez un campo magnético. Para obtener el efecto
de esta magnetización, consideremos un elemento de volumen ∆V (⃗x′ ) ubicado en algún punto interior de material ⃗x′ . Este elemento de volumen estará caracterizado por un momento
magnético

∆⃗µ(⃗x) =

m
⃗a

a∈∆V (⃗
x′ )

donde la suma se realiza sobre cada átomo contenido en ∆V (⃗x′ ). Definimos la magnetización del material como la densidad de momento magnético por unidad de volumen, esto
es
#
$
∆µ ''
′
⃗
M (⃗x ) =
'′
∆V
⃗
x

Veamos que ocurre con el campo magnético en un punto ⃗x fuera del material. El potencial
estará dado por
⃗ x) = A
⃗ L (⃗x) + A
⃗ M (⃗x)
A(⃗

⃗ M (⃗x) el potencial debido a la
⃗ L (⃗x) es el potencial magnético del campo externo y A
donde A
magnetización del medio.

---

### Página 441

En ⃗x′ ∈ V hay un momento magnético dado por
⃗ (⃗x′ )∆V (⃗x′ )
µ(⃗x′ ) = M

El potencial en ⃗x debido a este momento magnético puntual está dado por
⃗ M (⃗x) =
∆A

µ0 ∆µ(⃗x′ ) × (⃗x − ⃗x′ )
4π
| ⃗x − ⃗x′ |3

El potencial total en ⃗x debido al material se obtiene al integrar sobre V
⃗ M (⃗x) = µ0
A
4π

˚

d3 x′

V

Ahora, se tiene

⃗ (⃗x′ ) × (⃗x − ⃗x′ )
M
| ⃗x − ⃗x′ |3

⃗ ′
⃗′×M
⃗ (⃗x′ ) × (⃗x − ⃗x′ )
⃗ (⃗x′ )
∇
M
⃗ (⃗x′ ) × ∇
⃗′
⃗ ′ × M (⃗x )
=
M
=
−
∇
| ⃗x − ⃗x′ |3
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |
| ⃗x − ⃗x′ |

de forma que

⃗ M (⃗x) = µ0
A
4π

⃗′
⃗ x′ ) µ0 ˚
3 ′ ∇ × M (⃗
⃗′×
−
dx
d3 x′ ∇
′
| ⃗x − ⃗x |
4π
V
V

¨

)

⃗ (⃗x′ )
M
| ⃗x − ⃗x′ |

+

Finalmente
⃗ M (⃗x) = µ0
A
4π

⃗′
⃗ x′ ) µ0 ˆ✞ˆ ☎ dS(⃗
⃗ x′ ) × M
⃗ (⃗x′ )
3 ′ ∇ × M (⃗
dx
−
✝
✆
| ⃗x − ⃗x′ |
4π δV
| ⃗x − ⃗x′ |
V

˚

Recordando que el potencial magnético de una distribución de corriente libre en un volumen
V está dado por
˚
⃗ x′ )
J(⃗
⃗
A(⃗x) =
d3 x′
| ⃗x − ⃗x′ |
V
es inmediato notar que todo sucede como si dentro del material existiera una densidad de
corriente estacionaria
⃗ ×M
⃗ (⃗x)
J⃗M (⃗x) = ∇

y como si en el contorno del material hubiera una densidad de corriente superficial
⃗ (⃗x)
⃗σM (⃗x) = −n̂(⃗x) × M
Notar que

⃗ × J⃗M (⃗x) = 0
∇

---

### Página 442

(como debe ser para una corriente estacionaria), y
n̂(⃗x) · σM (⃗x) = 0
(como debe ocurrir para una corriente localizada). Luego, el efecto de un campo magnético
externo sobre un medio material se puede resumir en una distribución de corriente estacionaria y
localizada dentro del medio, el potencial en ⃗x debido a esta corriente de magnetización está dado
por
⃗ M (⃗x) = µ0
A
4π

13.5.

ˆˆ
J⃗M (⃗x′ )
µ0 ✞ ☎
x′ )
′ σM (⃗
dx
x)
+
✝ ✆ dS(⃗
| ⃗x − ⃗x′ | 4π δV
| ⃗x − ⃗x′ |
V

˚

3 ′

Leyes fundamentales en un medio magnetizado

Queremos ver como se pueden reescribir las leyes fundamentales del campo magnético en el
interior de un medio material. En todo punto dentro del material, se tendrán una densidad de
corriente de carga libre, J⃗L (⃗x), y una densidad de corriente de magnetización J⃗M (⃗x). Es decir
⃗ x) = J⃗L (⃗x) + J⃗M (⃗x)
J(⃗
Escribiendo la ecuación rotacional para el campo magnético, se debe incluír por supuesto
la densidad de corriente total
!
"
⃗ x) = µ0 J⃗L (⃗x) + ∇
⃗ ×M
⃗ (⃗x)
⃗ × B(⃗
⃗ x) = µ0 J(⃗
∇
Equivalentemente

⃗ ×
∇

)

+
⃗ x)
B(⃗
⃗ (⃗x) = J⃗L (⃗x)
−M
µ0

⃗ x)
⃗ x) = B(⃗
⃗ (⃗x), y entonces
Definimos el campo H(⃗
−M
µ0

⃗ × H(⃗
⃗ x) = J⃗L (⃗x)
∇
La gracia es que al lado derecho aparece únicamente la densidad de corriente libre. To⃗ x) a través de la densidad
do el efecto del medio magnetizado se encuentra contenido en H(⃗
⃗ (⃗x). Las ecuaciones fundamentales en un medio magnetizado son,
de momento magnético M
entonces
⃗ · B(⃗
⃗ x) = 0
∇
⃗ × H(⃗
⃗ x) = J⃗L (⃗x)
∇
Notar la total analogía con las leyes fundamentales de la electrostática en un medio
⃗ · D(⃗x) = ρL (⃗x)
∇
⃗ × E(⃗
⃗ x) = 0
∇

donde ρL (⃗x) es la densidad de carga libre. Recordar además que en ciertos materiales lineales,
homogéneos e isotrópicos

---

### Página 443

⃗ x) = ϵE(⃗
⃗ x), ϵ > 0
D(⃗
Esto se obtuvo de suponer que los momentos dipolares se alineaban en la dirección del campo
eléctrico y que la respuesta era lineal en el campo eléctrico. De esta forma las dos ecuaciones
fundamentales de la electrostática podían ser escritas como
⃗ · E(⃗x) = ρL (⃗x)
∇
ϵ
⃗ × E(⃗
⃗ x) = 0
∇
donde la única diferencia con las leyes en el vacío es la permitividad ϵ, no necesariamente
igual a ϵ0 . (de hecho, siempre es mayor o igual). Notar que esto implica que el efecto de un
medio dieléctrico es el de disminuír la magnitud del campo eléctrico en su interior. En cambio,
con el campo magnético, podría suceder que el material aumentara la magnitud del campo
magnético total, lo que veremos a continuación

13.6.

Relaciones constitutivas del material

Se tiene

⃗
⃗ x) = B(⃗x) − M
⃗ (⃗x)
H(⃗
µ0

⃗ (⃗x) es, por supuesto, una función del campo magnético
La magnetización M
⃗ (⃗x) = G(
⃗ B(⃗
⃗ x))
M
En consecuencia
o equivalentemente

⃗ x) = B(⃗
⃗ x) − G(
⃗ B(⃗
⃗ x))
H(⃗
⃗ x) = F (H(⃗
⃗ x))
B(⃗

⃗ y cada componente de H
⃗ es
Si el medio es lineal, la relación entre cada componente de B
lineal
⃗ b (⃗x)
⃗ a (⃗x) = Fab (⃗x)H
B
⃗ x) y H(⃗
⃗ x) es la misma en cada
Si el medio es homogéneo, entonces la relación entre B(⃗
punto
⃗ a (⃗x) = Fab H(⃗
⃗ x)b
B
Por último, si el medio es isotrópico, Fab = µδab , o simplemente
⃗ x) = µH(⃗
⃗ x)
B(⃗
donde µ es una constante llamada permeabilidad magnética del material.
Con esto las leyes fundamentales quedan de la siguiente manera
⃗ · B(⃗
⃗ x) = 0
∇
⃗ × B(⃗
⃗ x) = µJ⃗L (⃗x)
∇

---

### Página 444

Es decir, la ley de Ampère es exactamente la misma, exceptuando que ahora la permeabilidad no es necesariamente igual a la del vacío. Lo interesante es que para ciertos medios,
llamados paramagnéticos, µ > µ0 , y el material magnetizado tiende a aumentar la magnitud
del campo magnético. Por el contrario, para medios llamados diamagnéticos µ < µ0 , y la
magnitud del campo magnético es debilitada

13.7.

Ferromagnetismo

Existe otro tipo de materiales, llamados ferromagnéticos. En ellos existe una interacción
fuerte entre momentos magnéticos cercanos. Este tipo de materiales está constituído por dominios, como se ilustra en la figura . Un campo magnético externo tiende a alinear los momentos magnéticos en la dirección paralela al campo externo. La interacción entre los momentos
magnéticos vecinos causa un alineamiento mucho más fuerte

El aumento en la magnitud del campo magnético puede ser considerable, de hecho la magnitud el campo magnético en el interior de un material ferromagnético puede ser 103 o 104
veces mas grande que la del campo externo aplicado. El comportamiento de un material ferromagnético es no lineal, de forma que no podemos caracterizarlo por una permeabilidad
⃗ = F (H)
⃗ no es monovalente, o dicho de otra formagnética constante. De hecho, la relación B
ma, depende de la historia previa del material. Este fenómeno es conocido como histéresis. En
la figura se muestra la variación de la magnetización ante la prescencia de un campo magnético
externo, partiendo desde a

Fig. 13.2: Curva de histéresis
Notar que cuando el campo magnético externo vuelve a ser nulo (c), una magnetización sigue
presente. Es decir, la fuerte interacción entre momentos magnéticos cercanos puede mantenerlos alineados, incluso cuando un campo magnético externo se reduce a cero. Estos momentos

---

### Página 445

alineados puede producir campos magnéticos fuertes, sin la necesidad de un campo magnético
externo, este es el origen de los imagnes permanentes.

---

### Página 446

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 447

#### Capítulo 14
Ley de Inducción de Faraday
Los campos eléctricos y magnéticos que hemos considerado hasta ahora han sido producidos por cargas y corrientes estacionarias. A principios del siglo XIX ya era bien sabido que
imponiendo una diferencia de potencial entre dos conductores, el campo eléctrico en el interior
originaba una corriente de electrones, que a su vez crea un campo magnético a su alrededor.
Era válido entonces preguntarse si un campo eléctrico podía o no ser producido por un campo
magnético. Diversos intentos se realizaron, hasta que en 1831, Michael Faraday descubrió que
una corriente eléctrica se genera en un conductor cuando éste se mueve en la cercanía de
un imán. Pero, en su época, tal fenómeno, conocido ahora como inducción magnética, no
parecía ser más que una simple curiosidad.
El notable físico Richard Feynman contaba en sus cursos de Física en Caltech, que cuando Faraday presentó su descubrimiento a la comunidad científica, alguien le preguntó para
qué servía, a lo cual Faraday respondió con otra pregunta: ¿para qué sirve un recién nacido?
Medio siglo después, Tomás Edison tuvo la idea de utilizar el descubrimiento de Faraday para
generar corriente eléctrica y distribuirla a través de cables por la ciudad de Nueva York. La
primera planta eléctrica de la historia fue inaugurada en 1881, y consistía en unas enormes
turbinas de vapor que hacían girar unas grandes bobinas de alambre conductor alrededor de
imanes. Debido al efecto Faraday se generaba una corriente eléctrica que se podía transmitir
por toda la ciudad. La energía térmica se convertía, así, en energía eléctrica. Pocos meses
después se inauguró la primera planta hidroeléctrica, en la que el agua de un río hacía girar las
bobinas.
Toda la electricidad que consumimos hoy en día se genera gracias al efecto Faraday. Lo único que
varía es el mecanismo utilizado para hacer girar una bobina alrededor de un imán: este mecanismo puede ser el flujo del agua en una presa, el funcionamiento de un motor de combustión de
petróleo, la presión del vapor de agua calentada por el uranio en una planta nuclear, en otras
palabras, Faraday descubrió el principio fundamental de la conversión electromecánica de
la energía (el recién nacido creció espectacularmente, como diría Feynman).

---

### Página 448

El experimento de Faraday consiste en una espira conductora y un imán.

Faraday mostró que el galvanómetro no mide ninguna corriente cuando el imán está estacionario
con respecto a la espira. Sin embargo, se induce una corriente cuando existe un movimiento
relativo entre el imán y la espira, en particular, el galvanómetro marca en una dirección cuando
el imán se acerca, y en la dirección opuesta cuando el imán se aleja.

14.1.

Ley de Inducción

La descripción formal es la siguiente, sea Γ una curva que describe la forma del conductor,
entonces
˛
⃗ x, t)
εΓ (t) =
d⃗x · E(⃗
Γ[t]

Es la fuerza electromotriz inducida en Γ. Notar que es una cantidad dinámica que puede
evolucionar en el tiempo, ya que ahora aceptaremos que los campos eléctricos y magnéticos
puedan variar con el tiempo. Del mismo modo
¨
⃗ x) · B(⃗
⃗ x, t)
ΦB (t) =
dS(⃗
SΓ (t)

es el flujo magnético a través de SΓ
El experimento de Faraday muestra que una corriente eléctrica es inducida en la espira al
cambiar el flujo magnético que la atraviesa. Se comporta entonces como si estuviera conectada
a una fuente de f.e.m. Experimentalmente se encuentra que esta f.e.m inducida depende de la
tasa a la que varía el flujo magnético a través de la espira, esto es
εΓ = −

dΦB
dt

---

### Página 449

La unidad SI del flujo magnético es el Weber (W b) = 1 T m2
La ley de Faraday se puede enunciar como sigue: La f.e.m inducida en un circuito cerrado es
igual a la tasa negativa de cambio del flujo magnético a través del área encerrada por la espira
El signo menos indica que la corriente inducida en la espira tiende a oponerse a este cambio
de flujo. Existen muchas formas de inducir una fem en una espira. Por ejemplo si consideramos
un caso particular en donde el campo magnético es uniforme (espacialmente), la espira es plana
y su normal forma un ángulo ϑ con el campo magnético, se tiene
#
$
# $
# $
d(BS cos ϑ)
dB
dS
dϑ
ε=−
=−
S cos ϑ − B
cos ϑ + BS sin ϑ
dt
dt
dt
dt
A partir de esto, vemos que una f.e.m inducida se puede producir de las siguientes formas
⃗ en el tiempo (por ejemplo ocurre cuando en un circuito
1. Al variar la magnitud de B
cercano la corriente varía)

⃗ es decir, el área encerrada por la espira en el tiempo
2. Al variar la magnitud de S,

⃗ y el vector de superficie S
⃗ en el tiempo
3. Al variar el ángulo entre B

Este último es el principio más utilizado en centrales de generación
Es fácil obtener el sentido de la corriente inducida, ya que ésta produce un campo magnético
que tiene a oponerse al cambio del flujo magnético que induce dicha corriente. Ésta se conoce
como Ley de Lenz. (aunque se deduce completamente de la ley de Inducción!)

---

### Página 450

⃗ x, t) y B(⃗
⃗ x, t), variables en
Esta ley, que introduce una relación dinámica distante entre E(⃗
⃗ yB
⃗ son objetos físicos reales. No son intermediarios puramente
el tiempo, sugiere que E
matemáticos introducidos para facilitar los cálculos 1

14.2.

Forma diferencial de la ley de Inducción

Consideremos un circuito de prueba Γ fijo, es decir Γ(t) = Γ
˛
¨
d
⃗ x, t) = −
⃗ x) · B(x,
⃗
dS(⃗
t)
εΓ(t) = dx · E(⃗
dt S(Γ)
Γ
˛

Γ

⃗ x, t) = −
dx · E(⃗

¨

S(Γ)

⃗ x) ·
dS(⃗

Por el teorema de Stokes
¨
¨
!
"
⃗ × E(⃗
⃗ x, t) = −
dS(⃗x) · ∇
S(Γ)

S(Γ)

∂ ⃗
B(x, t)
∂t

⃗ x) ·
dS(⃗

∂ ⃗
B(x, t)
∂t

válido para todo S(fijo), luego se obtiene la ley diferencial de Faraday
⃗ × E(⃗
⃗ x, t) + ∂ B(⃗
⃗ x, t) = 0
∇
∂t

Esta es una de las ecuaciones de Maxwell para campos que varían en el tiempo, y es una
⃗ x), en donde sólo para casos estáticos (la primera parte
generalización para el rotor de E(⃗
del curso)
⃗ × E(⃗
⃗ x) = 0
∇
⃗ es conservativo.
Notar, que sólo en ése caso el campo E

Hypothesis non fingo de Newton se viene abajo en Electromagnetismo

---

### Página 451

Problema
La espira rectangular de la figura se encuentra sumergida en un campo magnético uniforme
⃗ = B x̂. Si la espira gira con velocidad angular w utilizando el eje z como eje de rotación, y
B
asumiendo que en t = 0 la espira se encuentra en el plano y-z, determine la fuerza electromotriz
inducida y la corriente inducida en la espira

#### Solución
Definiendo la normal a la espira rectangular como en la figura

Según ésta definición, la normal es en todo instante igual a −êφ , es decir
n̂ = −(− sin φx̂ + cos φŷ) = sin φx̂ − cos φŷ

De esta forma, y dado que el campo magnético es uniforme, el flujo a través de la espira es
¨
⃗ x) · B(⃗
⃗ x) = B
⃗ ·S
⃗=B
⃗ · S n̂ = BS sin φ
dS(⃗
ΦB =
S

Es decir
ΦB = Bab sin φ
Tenemos una expresión del flujo magnético a través de la espira en función del ángulo polar
φ. La idea es obtener el flujo en función del tiempo, para ello observamos que
dφ
= w → φ(t) = wt + C
dt
La constante C es fácil de determinar, considerando que en t = 0, la espira se ubica en el
eje y-z, es decir, φ0 = π/2. Así
ΦB = Bab sin(wt + π/2)

---

### Página 452

A partir de la ley de inducción de Faraday, podemos obtener la magnitud de la fem inducida
en la espira
dΦB
= −Babw cos(wt + π/2)
dt
Vemos que la fem es alterna y varía de forma sinusoidal, como se aprecia en la figura
ε=−

Esta es la forma típica de generación alterna. La tensión que llega a nuestras casas también
varía de forma sinusoidal, a una frecuencia de 50 Hz y valor efectivo de 220 Volts.
La magnitud de la corriente es, simplemente
I=

|ε|
Babw
=
cos(wt + π/2)
R
R

---

### Página 453

Problema
Considere la disposición que se muestra en la figura. Suponga que R = 6Ω, l = 1, 2 m y un
campo magnético uniforme de 2, 5 T está dirigido hacia el interior de la página.
a) ¿A qué rapidez deberá moverse la barra para producir una corriente de 0,5 A en la resistencia?
b) Calcule la fuerza que se debe ejercer sobre la barra en este caso

#### Solución
a) Consideremos el circuito cerrado formado por la barra y los rieles.

⃗ = −S k̂. (Hacia dentro del papel) Supongamos que la
Definamos al vector de superficie como S
barra se encuentra a una distancia x del riel izquierdo, según esto, el flujo magnético sobre la
superficie plana encerrada por este circuito es
ΦB = BA = Blx
Ahora, utilizando la ley de Faraday obtenemos que la fem inducida en el circuito
ε=−

dΦ
d
dx
= − (Blx) = −Bl
dt
dt
dt

Pero dx/dt es simplemente la velocidad de la barra, así
ε = −Blv

---

### Página 454

La correspondiente corriente inducida es
|ε|
Blv
=
R
R
Y el sentido de ésta se deduce de la ley de Lenz. Notemos que mientras la velocidad de la barra
sea positiva (y entonces se mueve hacia la derecha) el flujo magnético aumenta. Le ley de Lenz
dice que la corriente inducida intentará siempre oponerse al cambio de flujo magnético que la
origina. Es decir, el sentido de la corriente será tal que intentará frenar a la barra.
I=

Notar que en la figura anterior se ha supuesto un sentido para la corriente. Éste podría
ser correcto o no. Según el sentido de la corriente que aparece en la figura, habrá una fuerza
magnética sobre la barra en la direccion −î, que justamente intentará frenar a la barra, por lo
tanto ese será el verdadero sentido de la corriente. Despejando
v=

RI
Bl

reemplazando los valores numéricos
v=

6 × 0,5
= = 1m/s
2,5 × 1,2

b) Vemos que sobre la barra actúan dos fuerzas

La fuerza externa es la fuerza que se debe ejercer sobre la barra para que se mueva a velocidad
v. La fuerza magnética tiene relación con la corriente inducida que circula por el circuito, cuyo
equivalente es

La fuerza magnética que experimenta la barra es simplemente
⃗ ×B
⃗ = I(lĵ) × (−B k̂)
F⃗B = I L
2 2

B l v
F⃗B = −IlB î = −
î
R
que apunta en la dirección opuesta a ⃗v . Para que la barra se mueva a velocidad constante, la
fuerza neta actuando sobre ella debe ser igual a cero. Así
2 2

B l v
î
F⃗ext = −F⃗B =
R

---

### Página 455

Notar que la potencia entregada por F⃗ext es igual a la potencia disipada en la resistencia
(consecuencia de la conservación de la energía)
2 2 2

B l v
P = F⃗ext · ⃗v = Fext v =
R
P =

ε2
(Blv)2
=
= I 2R
R
R

---

### Página 456

Problema
Una barra conductora de masa m y resistencia R desliza entre 2 rieles conductores sin fricción que forman un ángulo ϑ con la horizontal. y están separados una distancia l. Un campo
⃗ es aplicado verticalmente. La barra se suelta del reposo y desliza habia
magnético uniforme B
abajo.

a) La corriente inducida en la barra. ¿En qué dirección fluye, de a hacia b o de b hacia a ?
b) La velocidad terminal de la barra
Una vez alcanzada la velocidad terminal
c) Cual es la corriente inducida?
d) A qué tasa se disipa energía en la resistencia?
e) Cual es la tasa de trabajo ejercido por la gravedad?
#### Solución
a) Supongamos que en un instante dado la barra se encuentra a una distancia x del extremo,
como se ve en la figura

El circuito formado por los rieles y la barra que desliza encierra una superficie plana cuya
normal es
n̂ = sinϑx̂ + cosϑŷ
Y el flujo a través de esta superficie es
¨
⃗ x) · B(⃗
⃗ x) = B
⃗ · S n̂ = BS cos ϑ = Bxl cos ϑ
ΦB =
dS(⃗
S

Con esto, la fem inducida en los extremos de la barra es
ε=−

dx
dΦB
= −Bl cos ϑ
dt
dt

---

### Página 457

Así, la corriente inducida está dada por
I=

|ε|
Bl
dx
=
cos ϑ
R
R
dt

La magnitud de la corriente es tal que se opone al cambio de flujo, es decir, debe ser tal que
sobre la barra actúa una fuerza magnética en la dirección -x̂.
⃗ ×B
⃗ = IL
⃗ × B ĵ
F⃗B = I L
De aquí es claro que la corriente debe ir en la dirección k̂ (es decir de b hacia a), de forma que
F⃗B = IlB k̂ × ĵ = −IlB x̂
b)

Se tiene además que

d2 x
mg sin ϑ − FB cosϑ = m 2
dt
d2 x
mg sin ϑ − IlBcosϑ = m 2
dt

Recordando que
I=

Bl
dx
cos ϑ
R
dt

se tiene
l2 B 2 2 dx
d2 x
cos ϑ
=m 2
R
dt
dt
2 2
dx
l B
dx
cos2 ϑ
= 2
g sin ϑ −
mR
dt
dt

mg sin ϑ −

A − Bv =
dt =

dv
dt

dv
(A − Bv)

t − t0 = −

ln(A − Bv)
B

−B(t − t0 ) = ln(A − Bv)
Finalmente
e−B(t−t0 ) = A − Bv

---

### Página 458

A
− e−B(t−t0 ) = v
B B
Si t0 = 0

l2 B 2
mR
mRg sin ϑ
v(t) = 2 2 2 − 2 2 2 e− mR cos ϑt
l B cos ϑ l B cos ϑ
Para encontrar la velocidad terminal, simplemente vemos que ocurre en el límite cuando
t→∞

vt =

mgRtgϑsecϑ
l2 B 2

c) La corriente terminal está dada por
Bl
mgtgϑ
cos ϑvt =
R
lB
d) El módulo de la fem inducida en esta situación es
I=

| ε |=

mgRtgϑ
lB

la tasa a la cual se disipa energía en la resistencia es la potencia que consume, esta es
P =| ε | I =

m2 g 2 Rtg 2 ϑ
l2 B 2

e) La tasa de trabajo ejercida por la gravedad es
Pg = Fg vt
donde Fg es la componente de la fuerza gravitacional en la dirección del desplazamiento
m2 g 2 Rtg 2 ϑ
l2 B 2
que es lo mismo que la potencia que disipa la resistencia. Esto debe tenerse por el principio
de conservación de la energía
Pg = mg sin ϑvt =

---

### Página 459

Problema
Una espira de alambre en forma de rectángulo de largo l y ancho w, y un alambre recto paralelo
al lado l y que lleva una corriente I, yacen sobre una mesa.
La distancia entre el alambre largo y el lado izquiero de la espira es h.
a) Determine el flujo magnético que atraviesa la espira.
b) Suponga que la corriente es una función del tiempo con I(t) = a + bt, con a y b constantes
positivas. ¿Cuál es la f.e.m inducida en la espira y la dirección de la corriente inducida?
#### Solución

Usando la ley de Ampère para el alambre recto se obtiene que el campo a una distancia r
de éste está dado por
⃗ = − µ0 I k̂
B
2πr
⃗ = −S k̂ de modo
Es decir, apunta hacia dentro del papel. Definimos el vector de área como S
que ΦB > 0. Para obtener el flujo total, simplemente debemos sumar los flujos sobre todos los
pequeños elementos de área de largo l y ancho dr encerrados por la espira
¨
¨
⃗ · dS
⃗
ΦB =
dΦB =
B
S

ΦB =

µ0 Il
2π

Finalmente

ˆ h+w
h

S

µ0 Il
dr
=
(ln(h + w) − ln(h))
r
2π

µ0 Il !
w"
ΦB =
ln 1 +
2π
h

b)Utilizando la ley de Faraday
d
dΦB
=−
ε=−
dt
dt

#

µ0 Il !
w"
ln 1 +
2π
h

$

Como las dimensiones de la espira permanecen constantes, lo único que varía en el tiempo
es la corriente, y entonces
w " dI
µ0 l !
ε = − ln 1 +
2π
h dt
y sabemos que dI/dt = b, así
µ0 lb !
w"
ε=−
ln 1 +
2π
h
Ahora, notemos que el alambre recto de corriente I produce un flujo magnético a través de la
espira entrando a la pagina. Por la ley de Lenz, la corriente inducida en la espira debe fluír
en el sentido contrareloj para así producir un campo magnético saliendo a través de la página
para contrarrestar el incremento del flujo hacia adentro.

---

### Página 460

Problema
Una espira rectangular de dimensiones l y w se mueve con velocidad constante ⃗v alejándose de
un alambre recto infinitamente largo que lleva corriente I en el mismo plano de la espira. Sea
la resistencia total de la espira R. ¿Cuál es la corriente en la espira en el instante en que el lado
más cercano está a una distancia r del alambre?
#### Solución

Sabemos que el campo magnético a una distancia x del alambre recto está dado por
⃗ = − µ0 I k̂
B
2πx
Apuntando hacia dentro del papel debido a la dirección de la corriente. Ahora, el flujo magnético
sobre un elemento diferencial de área de largo l y ancho dx en la espira es
⃗ · dS
⃗ = µ0 I ldx
dΦB = B
2πx
donde hemos escogido el vector de superficie apuntando hacia dentro de la página, para que
ΦB > 0. Integrando sobre toda la espira
ˆ
µ0 Il r+w dx
ΦB =
2π r
x
µ0 Il !
w"
ΦB =
ln 1 +
2π
r
el mismo resultado del problema anterior. Derivando con respecto a t, obtenemos la fem inducida
#
$
#
$
dΦB
µ0 Il d
µ0 Il
1 dr
r+w
ε=−
=−
ln
=−
−
dt
2π dt
r
2π
r + w r dt
donde dr/dt es simplemente el módulo de la velocidad de la espira
#
$
#
$
µ0 Ilv r − r − w
µ0 Ilv
−
=−
ε=−
2π
r+w r
2π
r(r + w)
µ0 Ilv
w
2π r(r + w)
Y la corriente inducida será simplemente
ε=

I=

w
µ0 Ilv
|ε|
=
R
2πR r(r + w)

---

### Página 461

Problema
Una barra conductora de masa m y resistencia R es empujada en la dirección horizontal a través
de dos rieles sin fricción apartados una distancia l, mediante un hilo de masa despreciable que
pasa a través de una polea ideal y que está conectada a un bloque de masa M . Un campo
magnético uniforme es aplicado verticalmente hacia arriba. La barra parte del reposo.

a) Sea la velocidad de la barra en algún instante igual a v. Encuentre una expresión para la
corriente inducida. En qué dirección fluye, de a hacia b o de b hacia a?
b) Resuelva la ecuación diferencial para la velocidad de la barra en función del tiempo.
#### Solución
a) Sea nuestro origen de coordenadas la esquina inferior del sistema como se aprecia en la figura

⃗ = S k̂,
Es una situación muy similar a la del problema 2, si escogemos el vector de superficie S
entonces el flujo a través del circuito será positivo.
Supongamos que cuando la velocidad es v, la barra está a una distancia horizontal x del origen,
así
ΦB = Bxl
y la fem inducida es
ε=−

dΦB
dx
= −Bl
= −Blv
dt
dt

La corriente inducida será

Blv
|ε|
=
R
R
b) Sea x la coordenada x del centro de masa de la barra en el instante t. El equilibrio de
fuerzas para la barra es
I=

⃗ = T î − Il⃗j × B k̂ = (T − IlB)î = m dx î
F⃗ = T î − I⃗l × B
dt2

---

### Página 462

Para la masa M

dy
F⃗ = M g − T = M 2
dt
Debemos notar que dx /dt = dy /dt , así

Mg − M

dy 2
dx2
=
M
g
−
M
=T
dt2
dt2

Así, el equilibrio de fuerzas para la barra queda
(M g − M

dx2
dx2
−
IlB)
=
m
dt2
dt2

dx2
l2 B 2
v = (m + M ) 2
Mg −
R
dt
Por último, hay que notar que v = dx/dt, y obtenemos una ecuación diferencial para v
l2 B 2
Mg
dv
+
v−
=0
dt R(M + m)
M +m
la solución es de la forma
B 2 l2

v(t) = Ce− R(M +m) t +

M gR
l2 B 2

y la condición inicial es que v(0) = 0, así
C+
Finalmente

M gR
M gR
=0→C=− 2 2
l B
l B

M gR
v(t) = 2 2
l B

#

2 2

B l
− R(M
t
+m)

1−e

$

---

### Página 463

Problema
Un disco en cuyo borde se encuentra una carga uniformemente distribuída q, pende de un hilo
vertical. En la región r < a existe un campo magnético uniforme B k̂.
Se desconecta la fuente de campo magnético, disminuyendo éste uniformemente a 0 en un intervalo corto de tiempo. Si el momento de inercia del disco es I, calcule la velocidad angular
final de éste.

#### Solución
Inicialmente, se tiene un flujo constante a través de la región r < a dado por
ΦBi = Bπa2
donde hemos elegido la normal a la superficie según la dirección k̂, de manera que ΦB > 0.
Ahora, tomemos la curva C que coincide con el borde del disco, y utilizando la ley de Faraday
˛
⃗ · d⃗l = − dΦB
E
dt
E2πb = −

dΦB
dt

lo que se puede reescribir como
E2πbdt = −dΦB
E=−

1 dΦB
2πb dt

Este campo eléctrico genera una fuerza sobre cada elemento de carga en el borde del disco

---

### Página 464

⃗ = Eλbdϑϑ̂
dF
En consecuencia, se produce un diferencial de torque dado por
⃗ = Eλb2 dϑk̂
d⃗τ = br̂ × dF
d⃗τ = −

1 dΦB 2
λb dϑk̂
2πb dt

λb dΦB
dϑk̂
2π dt
El torque total a un tiempo t estará dado por
ˆ 2π
λb dΦB (t)
⃗τ = −
dϑ
2π dt
d⃗τ = −

⃗τ = −λR

dΦ(t)
dt

⃗ es el momento angular del disco con respecto al centro, entonces
Si L
⃗τ =

⃗
dL
dτ

dΦB (t)
dL
=
dt
dt
ˆ tf
ˆ tf
dΦB (t)
dL
dtλb
dt
−
=
dt
dt
−λb

−λb (ΦB (tf ) − ΦB (0)) = Lf − Li
si el disco parte del reposo, Li = 0, y además ΦB (tf ) = 0
λbπa2 B = Iwf
wf =

λRπa2 B
I

---

### Página 465

Problema
Se considera una bobina con N espiras cuadradas de lado a sin un medio material en el interior.
Cada espira está a distancia b de un alambre recto y muy largo que lleva una corriente I =
I0 sin wt, con w constante. Además, todas las espiras cuadradas son coplanares con el alambre
recto. Calcule, en función de los datos I0 , w, a, b, la fem inducida entre los terminales de la
bobina

#### Solución
El campo magnético del alambre recto se obtiene fácilmente por la ley de Ampère, pues por
la extensión infinita del alambre el campo debe tener una simetría cilíndrica radial, y debe ser
tangente a trayectorias que son circunferencias concéntricas al alambre. De esta forma
˛
⃗ x) = 2πrB(r) = µo I(t)
d⃗x · B(⃗
Γ

donde Γ es una circunferencia concéntrica al alambre, de radio r

Calculemos ahora el flujo por una sola espira, como se muestra en la figura

Se tiene
Φ=

¨

S

⃗ x) · B(⃗
⃗ x)
dS(⃗

---

### Página 466

donde S es la superficie plana encerrada por la espira cuadrada. El campo magnético en el
plano de la espira está dado por
⃗ x) = − µ0 I(t) k̂
B(⃗
2πx
Escogiendo la normal unitaria en el sentido −k̂, el flujo magnético queda
$
#
ˆ a ˆ a
µ0 I(t)a
a+b
µ0 I(t)
=
ln
Φ(t) =
dy
dx
2πx
2π
b
El flujo será el mismo sobre cada una de las N espiras, de forma que el flujo total sobre la
bobina es
#
$
a+b
N µ0 I(t)a
ΦT (t) = N Φ(t) =
ln
2π
b
por la ley de Faraday, se inducirá una fem sobre la bobina dada por
dΦT (t)
dt
#
$
a+b
N µ0 wa
ln
cos wt
ε(t) = −
2π
b
ε(t) = −

---

### Página 467

Problema
Una bobina circular plana de N vueltas tiene diámetro D y resistencia R. La bobina se orienta
⃗ = B k̂ uniforme, y los extremos de la bobina se
con su eje paralelo a un campo magnético B
conectan a un dispositivo capaz de medir la carga que pasa a través de él. Si la bobina se gira
en 180 grados sobre un eje perpendicular al campo magnético, el dispositivo mide una carga
Q. Encuentre el valor de B en términos de N, D, R y Q

#### Solución
En la situación inicial, el flujo magnético a través de la bobina es constante y está dado por
¨
⃗ x)
Φ=N
dS(⃗x)n̂(⃗x) · B(⃗
S

orientando la normal a la espira según n̂ = k̂, se tiene
¨
¨
dS(⃗x)k̂ · B k̂ = N B
dS(⃗x) = N Bπ (D/2)2
Φ=N
S

S

La espira se gira en 180 grados, de forma que la situación final es la siguiente

Mientras la espira gira, se induce una fem ε entre sus extremos, ya que el flujo magnético
Φ varía. Si se induce una fem, se induce una corriente
I(t) =

ε(t)
R

ε(t) = −

dΦ(t)
dt

y

---

### Página 468

Supongamos que la espira demora un tiempo T en girar en 180 grados, luego la carga que
pasará por el detector es
ˆ T
ˆ T
ε(t)
Q=
dtI(t) =
dt
R
ˆ
1 T dΦ(t)
= − (Φ(T ) − Φ(0))
Q=−
dt
R 0
dt
R
donde

Φ(0) = N Bπ (D/2)2

mientras que
Φ(T ) = −N Bπ (D/2)2
luego

N BπD2
Q=
2R

Finalmente
B=

2QR
πN D2

---

### Página 469

Problema
Un tren de masa m se desplaza inicialmente con velocidad v0 î. Ingresa a una región de frenado
electromagnético para disminuír la velocidad del tren, en donde existe un campo magnético
uniforme, en el sentido que se muestra en la figura. Encuentre la velocidad del tren en función
del tiempo. El largo del tren es L

#### Solución
Analizamos un instante cualquiera cuando el tren ha entrado x(t) < L a la región de campo B

Sea Γ la curva que encierra al área que ha ingresado a la zona de campo magnético, en el
sentido indicado por la figura. Así, la normal exterior está dirigida según k, y el flujo a través
de la espira es
¨
¨
⃗
⃗
Φ(t) =
dS(⃗x) · B(⃗x) =
dS(⃗x)B = aBx(t)
S(Γ)

S(Γ

por la ley de inducción, habrá una fem inducida en el circuito Γ
dΦ(t)
= −aB ẋ(t)
dt
El signo menos da el sentido de la corriente inducida, como muestra la figura
ε(t) = −

Por ley de mallas, la corriente del circuito en el sentido de la figura está dada por
IR = aB ẋ(t)
aB
ẋ(t)
R
Por otro lado, en cada segmento del circuito hay una fuerza por unidad de largo dada por
⃗
⃗ De la figura es claro que las fuerzas sobre las secciones horizontales se cancelan
I × B.
I=

---

### Página 470

F⃗ = −Iaĵ × B k̂ = −IaB î
De esta forma, la segunda ley de Newton para el tren entrega
−IaB = m

d2 x
dt2

pero
I(t) =

aB ẋ(t)
R

−(aB)2 ẋ(t)
= mẍ(t), x(t) < L
R
−(aB)2 dx(t)
d2 x(t)
, x(t) < L
=m
R
dt
dt2
Resolviendo para v(t)
−(aB)2
dv(t)
v(t) =
mR
dt
La solución es
(aB)2

v(t) = v0 e− mR t , t < t∗
con x(t∗) < L. Este tiempo puede ser obtenido mediante x(t)
#
$
(aB)2
v0 mR
− mR t
1−e
x(t) =
(aB)2
la solución es válida para todo t tal que x(t) < L . Una vez que el tren ha ingresado
completamente a la región de campo magnético, el flujo se mantiene constante, luego no hay
fuerzas sobre el tren y se mantendrá con velocidad constante igual a v(t∗ )

---

### Página 471

Problema
Considere un generador que consta de un electroimán que genera un campo magnético constante. Una espira de área A gira con velocidad angular constante w como se ve en la figura. Si
los terminales de la espira se conectan a una resistencia R, calcule la potencia consumida por
ésta. Calcule además la potencia necesaria para producir el movimiento rotatorio de la espira.

#### Solución
El flujo magnético que atraviesa la espira es, dado que el campo magnético es uniforme
⃗ · dS
⃗ = BAcos(ϑ)
ΦB = B
ΦB = BAcos(wt)
Así, la tasa a la que varía el flujo magnético es
dΦB
= −BAwsin(wt)
dt
Utilizando la ley de Faraday, obtenemos la f.e.m inducida en el circuito
ε=−

dΦB
= BAwsinwt
dt

Si el circuito se conecta a una resistencia R, la corriente a través de ésta será
I=

BAw
|ε|
=
sinwt
R
R

Notemos que es una corriente alterna, cuya amplitud máxima es
I0 =

BAw
R

Ahora, la potencia suministrada al circuito eléctrico es
P = |ε|I =

(BAw)2
sin2 wt
R

Por otro lado, el torque necesario para producir el movimiento rotatorio de la espira es
τ = µBsinθ = µBsinwt
donde µ es la magnitud del momento magnético de la espira
µ = IA → τ = IABsinwt

---

### Página 472

B 2 A2 w
sin2 wt
R
Por último, la potencia mecánica necesaria está dada por
τ=

Pm = τ w =

B 2 A2 w2
sin2 wt
R

Como era de esperarse, la potencia mecánica entregada es igual a la potencia consumida
por el circuito.

---

### Página 473

Problema
Considere una espira rectangular de lado a y masa m, en el plano y-z, sumergida en un campo
⃗ = (B0 − αz)x̂, con α > 0. La espira cae en la dirección vertical debido a la
magnético B
gravedad. Encontrar la fem y corriente inducida en función de la velocidad ⃗v de la espira. ¿Cuál
es la velocidad terminal?

#### Solución
Definiendo la normal a la espira rectangular según n̂ = x̂, y suponiendo que el extremo inferior
se encuentra a una altura z, el flujo mangético a través de la espira está dado por
¨
¨
ˆ a ˆ z+a
⃗
⃗
ΦB =
dS · B =
dydzB(z) =
dy
dz(B0 − αz)
S

S

z

α 2 z+a
aα 2
z )z = a2 Bo −
(z + 2az + a2 − z 2 )
α
αa3
ΦB = a2 Bo − (2za2 + a3 ) = a2 (B0 − αz) −
Con esto, y utilizando la ley de inducción de Faraday, podemos determinar la fem inducida
en la espira
dΦB dz
dΦB
=−
= −ż(−αa2 )
ε=−
dt
dz dt
ΦB = a(B0 z −

ε = vαa2
Donde v es la rapidez con que cae la espira. Podemos distinguir dos casos, si la espira sube,
entonces v > 0 y ε > 0, lo que nos dice que la corriente inducida irá en el sentido contrareloj,
como se aprecia en la figura

Otra forma de verlo, es notando que el campo magnético se hace más débil en la medida
que aumenta la altura z, de forma que si la espira sube, el flujo disminuye. Así, la corriente
inducida debe ir en una dirección tal que el flujo que ésta genere se sume al flujo magnético

---

### Página 474

externo e intente evitar que el flujo total disminuya
Ahora, el caso de interés (la espira cae por gravedad), implica v < 0, de forma que ε < 0 y
esto significa que la corriente va en el sentido indicado por la siguiente figura. Otra forma de
verlo es notando que si la espira cae, el flujo magnético aumenta, luego la corriente inducida
debe generar un flujo magnético opuesto de manera de oponerse a este aumento.

La magnitud de la corriente está dada por
I=

αa2 | v |
|ε|
=
R
R

Ahora, para encontrar la velocidad terminal de la espira, necesitamos encontrar la ecuación
de movimiento. Calculemos la fuerza magnética que actúa sobre la espira. Podemos descomponer la fuerza total como la suma de las fuerzas sobre 4 segmentos

Es fácil notar que sobre los segmentos verticales 2 y 4, las fuerzas se anulan (el campo no
depende de la coordenada y y la corriente tiene sentido inverso en ambos segmentos). Ahora,
la fuerza sobre el segmento 1 es
F⃗1 = IaB(z + a)(−ŷ × x̂) = IaB(z + a)k̂
Y para el segmento 2

F⃗2 = IaB(z)(ŷ × x̂) = −IaB(z)k̂

La fuerza total es
F⃗ = Ia(Bo − α(z + a) − B0 + αz)k̂ = −Ia2 αk̂
2 4

α av
F⃗ = −
k̂
R

---

### Página 475

Notar nuevamente que si v > 0 (sube), entonces la fuerza intenta hacer caer a la espira. Si
por otro lado, la espira cae v < 0 y entonces la fuerza magnética es hacia arriba. Finalmente,
la ecuación de movimiento es
dv
α 2 a4 v
=−
− mg
dt
R
Para encontrar la velocidad terminal, imponemos dv
=0
dt
m

mg
α2 a4
El signo menos indica que finalmente la espira cae con velocidad constante dada por | vt |
vt = −R

---

### Página 476

Parte VI
Inductancia y Corriente Alterna

---

### Página 477

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 478

#### Capítulo 13
Inductancia
A continuación veremos un fenómeno de acoplamiento magnético. Supongamos que tenemos
2 bobinas, cerca una de otra, como se muestra en la figura

La primera de ellas tiene N1 vueltas y lleva una corriente I1 , la que da origen a un campo
⃗ 1 . Debido a que ambas bobinas están cerca, algunas líneas de campo magnético a
magnético B
través de la bobina 1 también pasarán a través de la bobina 2, como se aprecia claramente en
la figura. Denotemos por Φ21 el flujo magnético total a través de la bobina 2 (que será N2 veces
el flujo a través de una sola vuelta) debido a la corriente I1 .
Ahora, al variar I1 en el tiempo, habrá una fem inducida en la bobina 2 debido al cambio de
flujo magnético en ella
ˆ ˆ
dΦ21
d
⃗ ·B
⃗1
dS
ε21 = −
=−
dt
dt
S2
Ahora, por regla de la cadena
dI1
dΦ21
dΦ21 dI1
=
= M21
dt
dI1 dt
dt

---

### Página 479

Notar que aquí hemos establecido que el flujo sobre 2 es proporcional a la corriente I1 , es decir, dφ21 /dI1 = M21 donde la constante de proporcionalidad M21 se llama inductancia mutua,
y depende únicamente de la geometría y es una medida de que tan bueno es el acoplamiento
magnético.
Vemos que es igual a
dΦ21
Φ21
M21 =
=
dI1
I1
esto último se debe a que los flujos siempre dependen linealmente de las corrientes que los
originan. La unidad S.I de la inductancia mutua es el Henry (H).
Análogamente, ahora suponga que existe una corriente I2 en la segunda bobina y que varía
en el tiempo. Así, se induce una fem en la bobina 1 dada por
ˆ ˆ
dΦ12
d
⃗1
⃗ 2 · dS
ε12 = −
=−
B
dt
dt

Este flujo variable en la bobina 1 es proporcional al cambio de corriente en la bobina 2
dI2
dΦ12
dΦ12 dI2
=
= M12
dt
dI2 dt
dt
donde

dΦ12
Φ12
=
dI2
I2
Utilizando la ley de Ampere y la de Biot-Savart se puede deducir la fórmula de Neumann,
y se puede demostrar que ámbas inductancias mutuas son iguales (muy útil!)
M12 =

M21 = M12 = M
Esto es claro al ver la expresión de la fórmula de Neumann para dos circuitos
˛ ˛
d⃗l1 · d⃗l2
µ0
M21 =
4π C2 C1 |⃗r2 − ⃗r1 |
la cual es totalmente simétrica, de manera que el intercambiar los índices por M12 no altera
el resultado.

Autoinductancia
Considere nuevamente una bobina de N vueltas que lleva una corriente I en el sentido contrareloj. Si la corriente es constante, entonces el flujo magnético a través de cada vuelta permanecerá constante. Ahora considere que la corriente I varía en el tiempo, luego, de acuerdo a
la ley de Faraday-Lenz, una fem inducida aparecerá para oponerse al cambio de flujo.

---

### Página 480

La corriente inducida irá en el sentido del reloj si dI/dt > 0 y contrareloj si dI/dt < 0. (Recordar
Ley de Lenz!). La propiedad de que su propio campo magnético se opone a cualquier cambio
en la corriente es lo que se llama inductancia propia o autoinductancia, y la fem generada
entre sus terminales se llama fem autoinducida, que se denota por εL . Todo elemento de este
tipo se denomina Indutancia. Matemáticamente, se tiene
ˆ ˆ
dΦB
d
⃗ · dS
⃗
εL = −
B
=−
dt
dt
dΦB dI
dI
dΦB
=
=L
dt
dI dt
dt
de manera que
εL = −L
donde L es la autoinductancia,

dI
dt

ΦB
I
Físicamente, la autoinductancia es una medida de la resitencia de una inductancia al cambio
de corriente, así, mientras más grande es el valor de L, más lenta será la tasa a la cual varía la
corriente.
La autoinductancia también se puede pensar (de hecho es equivalente en términos de la fórmula
de Neumann) como la indutancia mutua del circuito consigo mismo, es decir, L = M11 .
L=

---

### Página 481

Energía almacenada en campos magnéticos
Debido a que una inductancia en un circuito se opone a cualquier cambio en la corriente a través
de ella, debe realizarse un trabajo por un agente externo (como una batería) para establecer
una corriente en la inductancia. La energía entonces se puede almacenar en ella!. El rol que
juega una inductancia en el caso magnético es análogo al de un condensador en el caso eléctrico.
La potencia, o tasa a la cual una fem externa trabaja para superar la fem autoinducida en la
inductancia (εL ) y lograr que pase una corriente I a través de ésta es
P =

dWext
= Iεext
dt

Si solo una fem externa y la indutancia están presentes, entonces ε = −εL , esto es
P = −IεL = IL

dI
dt

Si la corriente aumenta con dI/dt > 0, entonces P > 0 lo que significa que la fuente externa
está haciendo un trabajo positivo para transferir energía a la inductancia. Entonces, la energía
interna UB de la inductancia aumenta.
Por otro lado, si la corriente decrece dI/dt < 0, la fuente externa toma energía de la inductancia,
causando una disminución en la energía interna de ésta.
El trabajo total hecho por la fuente externa para aumentar la corriente desde 0 hasta I es
ˆ
ˆ I
LIdI = LI 2
Wext = dWext =
Esto es igual a la energía magnética almacenada en la inductancia
UB = LI 2
ésta expresión es análoga a la energía eléctrica almacenada en un condensador
1 Q2
UE =
2C
Existe una distinción importante entre una inductancia y una resistencia, desde el punto de
vista de la energía. Cuando una corriente I pasa a través de una resistencia, energía fluye a
través de la resistencia y se disipa en forma de calor, independiente si la corriente es constante
o dependiente del tiempo.
Por otro lado, energía fluye en una inductancia solo cuando existe una corriente que varía en
el tiempo , con dI/dt > 0. La energía no es disipada pero sí almacenada, y es liberada después
cuando dI/dt < 0

---

### Página 482

Circuitos RL
Considere el circuito RL que se muestra en la figura. En t=0, el interruptor es cerrado. Veremos
que la corriente no alcanza inmediatamente su máximo valor ε/R. Ésto se debe a la presencia
de una fem autoinducida en la inductancia.

Utilizando la ley de voltajes de Kirchhoff
−ε + IR + |εL | = −ε + IR + L

dI
=0
dt

se obtiene entonces una ecuación diferencial para la corriente
L

dI
= ε − IR
dt

la que se puede resolver por el método de separación de variables
LdI = dt(ε − IR) →

dI
dt
=
(ε − IR)
L

dt
dI
=
(ε/R − I)
L/R

Integrando a ambos lados de la ecuación

ln(I − ε/R) = −t

R
+ C1
L

así

R

I − ε/R = Ce−t L

I(t) = Ce−tR/L + ε/R
Imponiendo la condición I(0) = 0, se tiene C = −ε/R
I(t) =

ε
(1 − e−tR/L )
R

---

### Página 483

Se define entonces la constante de tiempo de este circuito como τ = L/R, así
I(t) =

ε
(1 − e−t/τ )
R

Notar que despues de un tiempo suficientemente largo, la corriente llega a su valor de
equilibrio ε/R. El hecho de que no alcanze este valor de forma inmediata se debe justamente a
que la inductancia tiende a oponerse a que la corriente varié de forma brusca. La constante de
tiempo τ es una medida de qué tan rápido se llega al estado de equilibrio, mientras mayor es
el valor de L, más tiempo le toma al circuito a llegar a éste estado.
Similarmente, la magnitud de la fem autoinducida se puede obtener como
|εL | = | − L

dI
| = εe−t/τ
dt

La cual es máxima cuando t=0 y desaparece cuando t tiende a infinito. Esto implica que
despues de un largo tiempo desde que el interruptor es cerrado, la autoinducción desaparece y
la inductancia siplemente actúa como un alambre conductor conectando 2 partes del circuito.
Para verificar que la energía se conserva, basta multiplicar la ecuación de Kirchhoff por I, para
obtener
dI
Iε = I 2 R + LI
dt
Notar que el lado izquierdo representa la potencia entregada por la batería, parte de ésta se
disipa en la resistencia (I 2 R) y el resto se almacena en la inductancia. La energía disipada por la
resistencia es irrecuperable, mientras que la almacenada por la inductancia se puede reutilizar
después

---

### Página 484

Para verificar esto último, considere ahora el circuito RL que se muestra en la figura. El
interruptor S1 ha estado cerrado por un tiempo muy largo tal que la corriente está en equilibrio
con valor ε/R. Que ocurre cuando en t=0 el interruptor S1 se cierra y el S2 se abre?

Sumando las caídas de potencial obtenemos que
−|εL | + IR = −L
L

dI
+ IR = 0
dt

dI
dI
dt
= −IR →
=−
dt
I
L/R

Integrando ambos lados de la ecuación
I(t) = Ce−t/τ
Imponiendo la condición I(0) = ε/R
I(t) =

ε −t/τ
e
R

Es decir, una vez que se desconecta la fuente de energía (batería), la energía almacenada
por la inductancia es liberada y entregada a la resistencia, quien disipa esta energía en forma
de calor

---

### Página 485

Circuitos de Corriente Alterna
En ayudantías anteriores vimos que un flujo magnético que cambia en el tiempo puede inducir
una fem de acuerdo a la ley de Faraday. En particular, si una espira rota con velocidad angular
w en la presencia de un campo magnético, la fem inducida varía sinusoidalmente en el tiempo
(con frecuencia w) y produce una corriente alterna (AC). Este es el caso típico de generación
de energía y de los grandes sistemas de potencia. El símbolo para una fuente de voltaje alterna
es

Un ejemplo de fuente AC es
V (t) = V0 cos wt
donde el valor máximo V0 se llama amplitud. El voltaje varía entre V0 y −V0 . Un gráfico
del voltaje como función del tiempo se muestra en la siguiente figura

Es una función periódica en el tiempo. La frecuencia f , definida como 1/T donde T es el
período, tiene unidades de 1/seg (hertz).
√ Se relaciona con la frecuencia angular según w = 2πf .
En nuestras casas obtenemos V0 = 220 2 y f = 50 Hz
Cuando una fuente de voltaje se conecta a un circuito RLC, después de un tiempo transiente,
una corriente alterna comenzará a fluír por el circuito como respuesta a la fuente de voltaje
forzante. La corriente será de la forma
I(t) = I0 cos(wt − φ)
Es decir,oscilará con la misma frecuencia de la fuente (esta es una propiedad de los sistemas
lineales), con amplitud I0 y fase φ que dependerán de la frecuencia forzante de la fuente
Antes de examinar circuitos RLC complejos, primero consideremos casos simples donde sólo un
elemento se conecta a una fuente de voltaje sinusoidal

---

### Página 486

Carga puramente resistiva
Considere un circuito puramente resistivo con una resistencia conectada a un generador AC,
como se muestra en la figura

Sumando las caídas de potencial, obtenemos
V (t) − VR (t) = V (t) − I(t)R = 0
donde VR (t) = I(t)R es el voltaje instantáneo a través de la resistencia. La corriente instantánea en la resistencia (y en el circuito) está dada por
VR (t)
V0 coswt
=
= IR0 cos wt
R
R
Notamos que φ = 0, lo que significa que I(t) y V (t) están en fase, es decir, alcanzan sus
valores máximos y mínimos al mismo tiempo.
I(t) =

Ahora, podemos representar voltajes y corrientes con números complejos, así, la fuente que
representamos como V (t) = V0 cos(wt) en forma compleja es, simplemente
V (t)∗ = V0 eiwt = Vo (cos wt + i sin wt) = V̂ eiwt
donde V̂ es el voltaje en forma de fasor. En este caso V̂ = Vo , pero en otras circunstancias
podría ser un número complejo. Por supuesto lo que entendemos aquí por voltaje es la parte
real de V ∗ (t). Similarmente las corrientes también las podemos escribir en forma fasorial.

---

### Página 487

Definimos la Impedancia de una resistencia por el número complejo
Ẑ = R
Esto corresponde a la resistencia expresado como fasor. En el caso de una resistencia es por
supuesto un número real. De esta forma
V̂

= Iˆ
Ẑ
Esto se cumple de forma general, de modo que al tratar estos problemas con fasores, siempre
se cumple que V̂ = IˆẐ, lo que simplifica enormemente los cálculos. En este caso en particular
V̂
= Iˆ
R
V̂
V0
=
Iˆ =
R
R
y entonces la corriente es
ˆ iwt = V0 eiwt
I(t)∗ = Ie
R
I(t) =

V0
cos wt
R

Carga puramente inductiva
Considere ahora una carga inductiva que consiste de una inductancia conectada a una fuente
AC

Se tiene
V (t) − VL (t) = V (t) − L

dI
=0
dt

lo que implica
dI
V (t)
Vo
=
=
cos wt
dt
L
L
Integrando
IL =

ˆ

Vo
dIL =
L

ˆ

dt cos wt =

V0
V0
sin wt =
cos(wt − π/2)
wL
wL

V0
de aquí vemos que la amplitud del voltaje en la inductancia es wL
= XV0L , donde XL = wL
se llama reactancia inductiva. Tiene unidades de Ohm (Ω), igual que las resistencias. Sin
embargo, a diferencia de una resistencia común, la reactancia depende de la frecuencia. Esto
se debe al hecho de que a frecuencias más altas la corriente varía de forma más rapida que
a frecuencias bajas. Por otro lado, esta reactancia se anula cuando w tiende a cero. También
, es decir, la corriente está en atraso con respecto al voltaje, como se
notamos que φ = −π
aprecia en la figura

---

### Página 488

Veamos como se obtiene este resultado de forma inmediata utilizando fasores, todo lo que
hay que saber es que la inductancia equivale a una impedancia igual a
ZL = iXL = iwL
De esta forma, el voltaje en la inductancia se relaciona con la corriente a través de ella según
V̂L = ẐL Iˆ
es decir, trabajando con fasores es una simple ley de Ohm (entre comillas). Como el voltaje
en la inductancia aquí es igual al voltaje de la fuente
V̂ = V̂L = iwLIˆ
Despejando la corriente
Iˆ =

i
1 −iπ/2
V̂ = −
V̂ =
e
V̂
jwL
wL
wL

En este caso, V̂ = Vo , con lo que la corriente en función del tiempo queda
ˆ iwt =
I(t)∗ = Ie
tomando la parte real
I(t) =

Vo i(wt−π/2)
e
wL

V0
cos(wt − π/2)
wL

---

### Página 489

Carga puramente capacitiva

Aquí, nuevamente tenemos
V (t) − VC (t) = V (t) −

Q(t)
=0
C

Q(t) = CV (t) = CVc (t) = CV0 cos wt
además, la corriente en el circuito está dada por
dQ
= −CwV0 sin wt = CwV0 cos(wt + π/2) = CwV (t)
dt
de aquí encontramos la relación entre la amplitud del voltaje y la amplitud de la corriente
a través del condensador
I(t) =

I0 = XC I0
Cw
donde Xc es la reactancia capacitiva del condensador. Vemos que en este caso la corriente
está desfasada en φ = −π/2 con respecto al voltaje (es decir, está en adelanto con respecto a
este)
V0 =

En términos de fasores, simplemente consideramos la impedancia de un condensador
ẐC =
de forma que

jwC

V̂ = ẐC Iˆ

despejando la corriente
V̂
Iˆ =
= iwC V̂ = iwCVo = wCVo eiπ/2
ẐC
Así

ˆ iwt = wCVo ei(wt+π/2)
I(t)∗ = Ie

---

### Página 490

tomando la parte real
I(t) = wCVo cos(wt + π/2)
Fácil fácil con fasores!
El circuito resonante RLC
Consideremos ahora el circuito RLC de la figura

Aquí tenemos
V (t) − VR (t) − VL (t) − VC = V (t) − IR − L

Q
dI
− =0
dt
C

lo que nos lleva a la siguiente ecuación diferencial
L

dI
Q
+ IR + = Vo cos wt
dt
C

Asumiendo que el condensador está inicialmente descargado, y considerando I = dQ
, podedt
mos reescribirla como
d2 Q
dQ Q
+R
+ = Vo cos wt
dt
dt
C
Una solución posible es (en régimen permanente)
L

Q(t) = Q0 sin(wt + φ)
donde la amplitud y la fase son, respectivamente
V0 /L
V0
Q0 = !
= "
1 2
w R2 + (wL − 1/wC)2
(Rw/L)2 + (w2 − LC
)
Q0 =
y
tanφ =

V0
"
w R + (XL − XC )2

XL − XR
(wL −
)=
R
wC
R

la correspondiente corriente es
I(t) =
con amplitud

dQ
= Io cos(wt + φ)
dt

V0
I0 = Q0 w = "
R2 + (XL − XC )2

---

### Página 491

Notar que la corriente tiene la misma amplitud y fase en todos los puntos del circuito RLC.
Por otro lado, el voltaje instantáneo a través de cada uno de los 3 elementos tiene diferente
amplitud y fase con respecto a la corriente. Habrán notado que resolver los problemas mediante
esta forma puede resultar complicado, de forma que indicaré una solución con fasores, y sacarán
sus propias conclusiones.
En términos de fasores, podemos ver el circuito como una sola impedancia equivalente, como
la resistencia, la inductancia y el condensador se encuentran en serie, tenemos
Ẑeq = R + iwL +

= R + i(wL −
)
iwC
wC

la amplitud de este número complejo es, simplemente
mod Z

mod =

#

R2 + (wL −

1 2
)
wC

y la fase
wL − wC
φ = arctan(
)
R

de esta forma, si el voltaje de la fuente es
V̂ = V0 ∠0
entonces la corriente a través del circuito es
wL − wC
V̂
V0
ˆ
I=
)
=!
∠arctan(
R
1 2
Ẑ
R2 + (wL − wC
)

Por último, recordando que
ˆ iwt =| I | ei(wt+φ)
I(t)∗ = Ie
V0
I(t) = !
cos(wt + φ)
1 2
R2 + (wL − wC
)
wL− 1

donde φ = arctan( R wC )
Notar que la amplitud de la corriente I0 = VZ0 alcanza un máximo cuando Z es mínimo.
Esto ocurre cuando XL = XC , o wL = wC
, llevando a
w0 = √

LC

Este fenomeno en que I0 alcanza su máximo se llama Resonancia, y la frecuencia a la cual
ocurre, w0 , se llama frecuencia de resonancia. En resonancia, la impedancia se transforma en
Z = R (puramente resistiva), y la amplitud de la corriente es
I0 =

V0
R

y la fase φ = 0

---

### Página 492

El circuito resonante es últil en varias aplicaciones, como sintonizadores y tarjetas electrónicas, donde se desea que el circuito responda a señales de un rango de frecuencias limitado.

---

### Página 493

El transformador
Un transformador es un dispositivo utilizado para aumentar o disminuír el voltaje AC en un
circuito. Una típica configuración consiste de 2 bobinas, (primaria y secundaria), enrolladas en
un núcleo de hierro, como se muestra en la figura

La bobina primaria, con N1 vueltas, es conectada a una fuente alterna V1 (t). La secundaria
tiene N2 vueltas y se conecta a una resistencia de carga R2 . La forma en que funcionan los
transformadres se basa en la ley de Faraday, la corriente alterna en el primario induce una fem
alterna en la segunda bobina, debido a su inductancia mutua.
En el circuito primario, despreciando la resistencia de la bobina, la ley de Faraday implica
V1 = −N1

dΦB
dt

donde ΦB es el flujo magnético a través de la bobina primaria. El nucleo de hierro sirve para
incrementar el flujo magnético producido por la bobina 1 (el hierro tiene permeabilidad µ mucho
mayor a la del vacío) y para asegurar que prácticamente todo el flujo magnético por el primario
también atraviese la bobina secundaria. Así, el voltaje inducido en el secundario es
V2 = −N2

dΦB
dt

En un transformador ideal, la pérdida de potencia debida al efecto Joule se puede despreciar,
de manera que la potencia administrada a la bobina primaria es transferida completamente a
la secundaria
I1 V1 = I2 V2
También estamos suponiendo que no hay flujo magnético que escape afuera del núcleo de
hierro. Combinando esto obtenemos
N2
V2
=
V1
N1
I2
N1
=
I1
N2
vemos que la razón para los voltajes está completamende determinada por la razón entre el
número de vueltas entre el primario y el secundario. El transformador tiene una infinidad de
aplicaciones, todos los equipos elécticos utilizan uno para transformar los 220 V efectivos en el
voltaje deseado de operación. Notar que con corriente continua un transformador simplemente
no funciona (Es una de las razones de las porqué no se genera en corriente continua).

---

### Página 494

#### Problema 1
Considere dos espiras coplanares y concéntricas, de radios R1 y R2 con R1 ≫ R2 . Encuentre la
inductancia mutua entre ambas espiras.

#### Solución
La inductancia mutua se puede obtener suponiendo que por el anillo más grande circula una
corriente I1 , como muestra la figura:

Anteriormente vimos que el campo magnético en el centro de un anillo que lleva corriente
I1 está dado por
⃗ 1 = µ0 I1 k̂
B
2R1
Debido a que R1 ≫ R2 , aproximamos el campo magnético sobre toda la espira interior por
⃗
B1 . Así, el flujo a través de la espira interior es
⃗1 · S
⃗
Φ21 = B
Si definimos la normal a la superficie encerrada por el anillo interior según el eje k̂
µ0 I1 2 µ0 I1 πR22
πR2 =
2R1
2R1
Finalmente, la inductancia mutua está dada por
Φ21 = B1 S =

M=

Φ21
µ0 πR22
=
I1
2R1

---

### Página 495

#### Problema 2
Considere un toroide de N vueltas y de sección rectangular de lado h, radio interior a y radio
exterior b.

a) Calcule la autoinductancia y discuta que ocurre cuando a ≫ b − a
b) Calcule la energía magnética almacenada en el toroide
#### Solución
Utilizando la ley de Ampere, el campo magnético se obtiene como
˛
˛
˛
⃗ · d⃗l = Bdl = B dl = B(2πr) = µ0 N I
B
donde se ha integrado el campo sobre una circunferencia de radio r ubicada en el centro del
toroide
µ0 N I
B=
2πr
El flujo magnético sobre una vuelta del toroide se puede obtener al integrar sobre todas las
secciones rectangulares, con dA = hdr como elemento diferencial de área

ˆ b

µ0 N Ih
µ0 N I
hdr =
ln(b/a)
2πr
2π
a
y el flujo total sobre el toroide será N ΦB . Con esto, la autoinductancia es
ΦB =

ˆ ˆ

⃗ · dS
⃗=
B

N ΦB
µ0 N 2 h
L=
=
ln(b/a)
I
2π
cuando a ≫ b − a, se tiene
ln(b/a) = ln(1 +
y la autoinductancia es
L=

b−a
b−a
)≈
a
a

µ0 N 2 h b − a
2π
a

---

### Página 496

recordando que el área de una sección del toroide es A = h(b − a)
µ0 N 2 A
L=
2πa
y con l = 2πa

µ0 N 2 A
l
que es justamente la autoinductancia de un solenoide.
L=

b) La energía almacenada en el toroide es simplemente
µ0 N 2 I 2 h
U = LI 2 =
ln(b/a)
4π

---

### Página 497

#### Problema 3
Considere el siguiente circuito LC. Suponga que el condensador tiene una carga inicial Q0 . En
t=0, el interruptor se cierra.

a) Encuentre la ecuación diferencial para la carga en el condensador mediante consideraciones
energéticas.
b) Utilizando las leyes de Kirchhoff encuentre I(t) y Q(t)

#### Solución
a) En ausencia de una resistencia, la energía total se transforma constantemente en energía
eléctrica y magnética, esto se llama osilación electromagnética.
Le energía total del circuito LC en un instante arbitrario es
U = UC + UL =

1 Q2 1 2
+ LI
2C

Por el principio de conservación de la energía
dU
d 1 Q2 1 2
= (
+ LI ) = 0
dt
dt 2 C
dI
Q dQ
+ LI
=0
C dt
dt
Además, hay que notar que I = −dQ/dt
Q
dI
Q
d2 Q
− I + LI
=0→− −L 2 =0
C
dt
C
dt
Finalmente la ecuación diferencial para la carga en el condensador es
Q
d2 Q
+L 2 =0
C
dt
b)Utilizando la ley de voltajes de Kirchhoff,
−VC + VL = −

Q
dI
+L =0
C
dt

y relacionando la corriente con la carga en el condensador
Q
dQ2
+L 2 =0
C
dt

---

### Página 498

dQ2
Q
=0
+
dt
LC
la solución general es de la forma
Q(t) = Q0 cos(w0 t + φ)
donde la frecuencia angular w0 está dada por
w0 = √

LC

La corriente por la inductancia es
I(t) = −

dQ
= w0 Q0 sin(w0 t + φ) = I0 sin(w0 t + φ)
dt

donde I0 = w0 Q0 . De las condiciones iniciales Q(0) = Q0 e I(0) = 0, la fase φ es simplemente
0.
Con esto, las soluciones para la carga y la corriente en el circuito LC es
Q(t) = Q0 cos(w0 t)
I(t) = I0 sin(w0 t)
la dependencia de Q(t) e I(t) se muestra en la figura:

La energía eléctrica y magnética están dadas por
UE =

Q2
Q2 (t)
= ( 0 )cos2 (w0 t)
C
2C

LI 2
Q2
UL = LI 2 (t) = 0 sin2 (w0 t) = 0 sin2 (w0 t)
2C
Se ve fácilmente que la energía permanece constante
Q2
Q2
Q20
)cos2 (w0 t) + 0 sin2 (w0 t) = 0
2C
2C
2C
La oscilación de energía magnética y eléctrica en el tiempo se ve en la figura
U =(

---

### Página 499

El análogo mecánico de este circuito LC es el sistema masa-resorte

---

### Página 500

#### Problema 4
Considere el circuito RLC en serie, que consta de una resistencia, una inductancia, y un condensador

Mediante consideraciones energéticas encuentre la ecuación diferencial para la carga en el condensador
#### Solución
La energía en un instante arbitrario t está dada por
U = UE + UL =

1 Q2 1 2
+ LI
2C

A diferencia del circuito LC, parte de la energía del circuito será disipada por la resistencia.
Esto es, la tasa a la cual la energía es disipada es
dU
= −I 2 R
dt
donde el signo negativo implica que la energía total disminuye en el tiempo. Así
Q dQ
dI
dU
=
+ LI
= −I 2 R
dt
C dt
dt
Aquí, nuevamente se tiene I = −dQ/dt
dI
Q
= −I 2 R
− I + LI
C
dt
−

dI
Q
+ L = −IR
C
dt

dQ
Q
dQ2
−L 2 =
R
C
dt
dt
Finalmente, la ecuación diferencial para Q es
−

L

dQ2 dQ
Q
+
R+ =0
dt
dt
C

---

### Página 501

#### Problema 5
Considere el circuito de la figura

Determine la corriente por cada resistencia
a) inmediatamente después de cerrar el interruptor
b) después de que ha pasado mucho de tiempo de cerrado el interruptor
Suponga que el interruptor es reabierto después de que ha estado mucho tiempo cerrado, encuentre nuevamente las corrientes:
d) inmediatamente después de que es abierto
e) después de un largo tiempo
#### Solución
a) Inmediatamente después de que el interruptor es cerrado, la corriente a través de la inductancia es cero ya que la fem autoinducida evita que la corriente crezca abruptamente.
Así, I3 = 0.
Debido a que I1 = I2 + I3 , se tiene que I1 = I2

Utilizando las leyes de Kirchhoff a la malla 1, se tiene
−ε + I1 R1 + I1 R2 = 0
ε
R1 + R2
b) Después de un largo tiempo, no hay fem autoinducida en la inductancia y las corrientes
pasan a ser constantes. Para la malla 1, se tiene ahora
I1 = I2 =

−ε + I1 R1 + I2 R2 = 0
y para la malla 2

---

### Página 502

I3 R3 − I2 R2 = 0
por último, por la ley de nodos, I1 = I2 + I3 . Resolviendo, se obtiene
I1 =

(R2 + R3 )ε
R1 R2 + R1 R3 + R2 R3

I2 =

R3 ε
R1 R2 + R1 R3 + R2 R3

I3 =

R2 ε
R1 R2 + R1 R3 + R2 R3

c) Inmediatamente después de que el interruptor es abierto nuevamente, la corriente a través
de R1 es 0, I1 = 0. Esto implica que I2 + I3 = 0.
La malla 2 ahora forma un circuito RL que decae e I3 comienza a decaer. Así
I3 = −I2 =

R3 ε
R1 R2 + R1 R3 + R2 R3

d)Después de mucho tiempo , todas las corrientes son cero, esto es, I1 = I2 = I3 = 0

---

### Página 503

#### Problema 6
Considere el circuito de la figura, donde V (t) = Vo cos wt. Si S1 y S2 se cierran inicialmente,
encuentre (Datos son R, L, Vo y w)

a) La corriente en función del tiempo
b) La potencia promedio entregada al circuito
c) La corriente en función del tiempo largo tiempo después de que S1 se abre
d) La capacidad C si S1 y S2 se abren y después de un tiempo largo, la corriente y el voltaje
están en fase
e) La impedancia cuando S1 y S2 se abren
f) La energía máxima almacenada en el condensador y la inductancia
g) La diferencia de fase entre voltaje y corriente si se dobla la frecuencia w
h) La frecuencia para la cual la reactancia inductiva es igual a un medio de la reactancia capacitiva
#### Solución
a) Al cerrar ambos interruptores, no circulará corriente ni por la inductancia ni por el condensador. La impedancia equivalente en este caso es Zeq = R de modo que la corriente es,
simplemente
Vo
I(t) =
cos wt
R

b) La potencia instantánea consumida por la resistencia es
P (t) = V (t)I(t) =

Vo2
cos2 wt
R

Claramente una función periódica, el promedio temporal es entonces
< P (t) >=
T

ˆ T
o

dtP (t) =

Vo2
2R

c) Cuando se abre S1 , se conecta la inductancia al circuito. La impedancia equivalente en
este caso es
Zeq = R + iwL =

√

wL

R2 + w2 L2 eiarctan( R )

Luego, la corriente es
wL
V̂
Vo
Iˆ =
=√
e−iarctan( R )
Zeq
R 2 + w 2 L2

---

### Página 504

Así,
ˆ iwt ) = √
I(t) = Re(Ie

Vo
cos(wt − tan−1 (wL/R))
R +w L

d) Ahora se conecta además el condensador, de modo que la impedancia equivalente en este
caso es
Zeq = R + iwL +

= R + i(wL −
) =| Z | eiφ
iwC
wC

donde está dado por
(wL − wC
)
R
como no hay desfase entre voltaje y corriente, φ = 0 (el circuito está en resonancia!), esto
quiere decir que w = wo

φ = tan−1

φ = 0 → tan−1 = 0
wo L =
C=

wo C

wo2 L

e) El circuito está en resonancia, luego
#
| Z |=

R2 + (wL −

1 2
) =R
wC

f) La energía máxima en el condensador es (Vc representa la amplitud del voltaje en el
condensador)
Io 2
)
UEmax = CVc2 = C(
2 wC
1 Vo 2 1
V02 L
UEmax = C
=
2 R wo2 C 2
2R2
En el√último paso se ha usado que la frecuencia es igual a la frecuencia de resonancia
w0 = 1/( LC) Ahora, la energía máxima almacenada por la inductancia
LVo2
ULmax = LIo2 =
2R2

g) Si la frecuencia es ahora
w = 2wo = √

LC

el ángulo de desfase entre voltaje y corriente queda

---

### Página 505

√
√
wL − 1/(wC)
−1 2/( LC)L − ( LC/(2C))
φ = tan (
) = tan (
)
R
R
#
L
)
φ = tan−1 (
2R C
−1

h) Finalmente, la frecuencia para que XL = 12 XC debe cumplir
wL =
luego
w=√

1 1
2 wC

wo
=√
2LC

---

### Página 506

#### Problema 7
Una antena FM tiene una inductancia L = 10−6 H, una capacidad C = 10−12 F, y una
resistencia R = 100 Ω. Una señal de radio induce una fem sinusoidal en la antena con amplitud
10−5 V

a) A que frecuencia angular w0 de la señal incidente el circuito estará sintonizado, esto es, para
que w0 la corriente en el circuito será máxima?
b) Asumiendo que la onda incidente está sintonizada, cual será la amplitud de la corriente en
el circuito a esta frecuencia?
c) Cuál es la amplitud de la diferencia de potencial a través del condensador a esta frecuencia?
#### Solución
a) La antena estará sintonizada con la señal incidente a la frecuencia de resonancia, esto es, la
señal debe tener una velocidad angular dada por
#
#
w0 =
= 109
=
−6
LC
10 10−12
y la frecuencia asociada es
f=

w0
1 9
=
10 = 0, 159 ∗ 109
2π
2π

Equivalentemente f = 0, 159Ghz.
b) A la frecuencia de resonancia, la corriente máxima es
10−5
V0
=
= 0, 1µA
R
c)La amplitud del voltaje en la inductancia
I0 =

VL = I0 XL = I0 w0 L = 0, 1 ∗ 10−6 2π ∗ 0, 159 ∗ 109 ∗ 10−6 = 9, 99 ∗ 10−5 V

---

### Página 507

#### Problema 1
Dado el circuito de la figura, suponer que el interruptor S se ha cerrado durante un largo tiempo,
de modo que existen corrientes estacionarias en el inductor de L = 2H y que su resistencia es
despreciable. Además R1 = 10 Ω, ε = 10 V
(a) Determinar la intensidad de corriente suministrada por la batería, la corriente que circula
por la resistencia R2 = 100 Ω y la intensidad que circula por el inductor
(b) Determinar el voltaje inicial entre los extremos del inductor cuando se abre el interruptor
S

#### Problema 2
El circuito de la figura se denomina filtro RC pasa-altos porque transmite con mayor amplitud
las señales de alta frecuencia que las de baja. Si la tensión de entrada es Vin = V0 cos wt,
demostrar que la de salida es Vsal = VR cos(wt − φ), donde
V0
VR = !
1 + ( wRC
)2

#### Solución problema 1

Cuando el interruptor S ha estado cerrado por largo tiempo, las corrientes llegan a un estado
de regimen permanente. Si IL (t) denota la corriente a través de la inductancia, se tiene que el
voltaje a través de ésta es

---

### Página 508

vL (t) = L

dIL
dt

En régimen estacionario

dIL
=0
dt
Así, no hay diferencia de potencial entre los extremos de la inductancia. Esto significa que
en régimen permanente la inductancia se comporta como un cortocircuito

En esta situación, toda la corriente se irá por la inductancia, de esta forma
IR100Ω = 0
Para obtener la intensidad que circula por el circuito, simplemente sumamos las caídas de
potencial y se obtiene
−ε + IR1 = 0
I=

ε
=
= 1A
R1

b) En el instante en que se abre nuevamente el interruptor, circula corriente a través de la
inductancia y la resistencia de 100Ω

Sea I(t) la corriente que fluye en este caso. Por continuidad, I(0) = 1A, con esto
IR2 + VL = 0
VL = −IR2 = −1 ∗ 100 = −100V

---

### Página 509

#### Solución Problema 2
El circuito consiste en un condensador en serie con una resistencia

La impedancia equivalente está dada por
=R−i
iwC
wC
Conviene expresar esta impedancia en su forma polar
#
Ẑ = R2 + 2 2 eiφ
w C
donde φ está dado por
)
φ = tan−1 (
wRC
De esta forma, se tiene
Ẑ = R +

V̂in = Ẑ Iˆ
V̂in
Vo
Iˆ =
=!
Ẑ
R2 + w21C 2 eiφ
Vo
e−iφ
Iˆ = !
R2 + w21C 2

Finalmente, Vout es el voltaje entre los extremos de la resistencia
RVo
V̂out = Ẑr Iˆ = RIˆ = !
e−iφ
R2 + w21C 2

Con esto

Vo
V̂out = !
e−iφ
1 + R2 w 2 C 2
Vo
cos(wt − φ)
Vout (t) = Re(V̂out eiwt ) = !
1 + R2 w12 C 2

---

### Página 510

Parte VII
Ecuaciones de Maxwell y sus bases
empíricas

---

### Página 511

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 512

#### Capítulo 14
Ecuaciones de Maxwell
14.1.

Corriente de Desplazamiento

Habíamos visto anteriormente que si un conductor con corriente posee cierta simetría favorable, el campo magnético se podía obtener fácilmente mediante la ley de Ampère
˛
⃗ x) = µ0 Ienc
d⃗x · B(⃗
Γ

Esta ecuación indica que la circulación del campo magnético sobre cualquier curva cerrada
es siempre µ0 Ienc , donde Ienc es la corriente que atraviesa una superficie cuyo contorno es la
curva de integración.
Ahora, en un medio material la ley de Ampère es
˛
⃗ x) = I
d⃗x · H(⃗
Γ

Esta ley se puede llevar a su forma diferencial mediante el teorema de Stokes
⃗ × H(⃗
⃗ x) = J(⃗x)
∇
Sin embargo, esta ley es inconsistente en algunas ocasiones y encontraremos entonces una
generalización válida, que fue propuesta por Maxwell. Consideremos el circuito eléctrico de
la figura, que consiste de un condensador de placas paralelas, que se está cargando con una
corriente de magnitud constante I

Utilizando la ley de Ampère al contorno C y a la superficie S1
˛
¨
⃗ x) =
⃗ x) · J(⃗
⃗ x) = I
d⃗x · H(⃗
dS(⃗
C

S1

---

### Página 513

Si, por otra parte, se utiliza la ley de Ampère al contorno C y a la superficie S2 , entonces
J(⃗x) es cero para todo ⃗x ∈ S2
˛

C

⃗ x) =
d⃗x · H(⃗

¨

S2

⃗ x) · J(⃗
⃗ x) = 0
dS(⃗

Vemos que existe entonces una ambiguedad fundamental en la ley de Ampère al escoger dos
superficies de integración distintas. El error es fácil de ver al mirar su forma diferencial
⃗ × H(⃗
⃗ x) = J(⃗
⃗ x)
∇
Utilizamos ahora el hecho de que la divergencia de un rotor es nulo
⃗ ·∇
⃗ × H(⃗
⃗ x) = ∇
⃗ · J(⃗
⃗ x) = 0
∇
⃗ · J⃗ = 0 es inconsistente con la conservación de la carga en la presente
Es inmediato que ∇
situación, por que de hecho, en el volumen encerrado por ambas superficies, hay un ∂ρ/∂t
distinto de cero ( se está acumulando carga en el condensador).
Maxwell corrigió la ley de Ampère al agregar un término tal que de ella se desprenda
⃗ · J(⃗
⃗ x) = − ∂ρ(⃗x)
∇
∂t
De la primera ecuación de Maxwell
⃗ · D(⃗
⃗ x) = ρ(⃗x)
∇
y sustituyendo en la ecuación de continuidad
⃗
⃗ · J(⃗
⃗ x) + ∂ ∇
⃗ · D(⃗
⃗ x) = ∇
⃗ · (J(⃗
⃗ x) + ∂ D(⃗x) ) = 0
∇
∂t
∂t
⃗

de manera que la corrección de Maxwell está en agregar el término ∂∂tD a la forma diferencial
de la ley de Ampère, y entonces se obtiene la ley de Ampère-Maxwell
⃗
⃗ × H(⃗
⃗ x) = J(⃗
⃗ x) + ∂ D(⃗x)
∇
∂t
es evidente que en el caso de campos que no dependen del tiempo, esta ley es igual a la ley de
Ampère. La introducción del segundo término , llamado densidad de corriente de desplazamiento, representa una de las más grandes contribuciones de Maxwell a la teoría electromagnética.
Veremos que al modificar ésta ley, las ecuaciones de Maxwell predicen la propagación de ondas
electromagnéticas.
Por último, la forma integral de la ley de Ampère-Maxwell queda de la forma
˛

Γ

⃗ x) =
d⃗x · H(⃗

⃗ x) · J(⃗
⃗ x) + d
dS(⃗
dt
S(Γ)

¨

¨

S(Γ)

⃗ x) · D(⃗
⃗ x)
dS(⃗

En el ejemplo, al integrar en la superficie S2 , el segundo término no es nulo, debido a que
⃗ a través de S2 que está variando en el tiempo, de hecho la magnitud
hay un flujo del campo D
del campo crece cuando se acumula carga en el condensador.

---

### Página 514

14.2.

Ecuaciones de Maxwell

Las ecuaciones de Maxwell resumen toda la teoría electromagnética. Éstas establecen la
⃗ ⃗x)) con los
relación entre las fuentes (densidad de carga ρ(t, ⃗x), y densidad de corriente J(t,
⃗
⃗
⃗
⃗
campos E(t, ⃗x), B(t, ⃗x), D(t, ⃗x), H(t, ⃗x))
⃗ · D(t,
⃗ ⃗x) = ρ(⃗x)
∇
⃗
⃗ × E(t,
⃗ ⃗x) = − ∂ B(t, ⃗x)
∇
∂t
⃗ · B(t,
⃗ ⃗x) = 0
∇
⃗
⃗ × H(⃗
⃗ x) = J(⃗
⃗ x) + ∂ D(⃗x)
∇
∂t
⃗ ·D
⃗ = ρ es la ley de Gauss, cuya forma integral es
La primera ecuación ∇
ˆˆ
˚
✞☎ ⃗
⃗
x) · D(t, ⃗x) =
d3 xρ(t, ⃗x)
✝ ✆dS(⃗
S

V (S)

⃗ ×E
⃗ = − ∂ B⃗ es la forma diferencial de la ley de inducción de Faraday, ésta
La ecuación ∇
∂t
dice que un campo magnético variable en el tiempo induce un campo eléctrico, en su forma
integral
˛
ˆˆ
d ✞☎
⃗
⃗ x) · B(t,
⃗ ⃗x)
d⃗x · E(t, ⃗x) = −
✝ ✆ dS(⃗
dt
Γ
S(Γ)
⃗ ·B
⃗ = 0 es la ley de Gauss magnética, y representa el hecho de que los
La ecuación ∇
monopolos magnéticos nunca han sido observados. Es decir, las líneas de campo magnético son
cerradas, consecuencia de esto es que el flujo magnético sobre una superficie cerrada es siempre
cero. En su forma integral
ˆˆ
✞☎ ⃗
⃗ ⃗x) = 0
x) · B(t,
✝ ✆dS(⃗
S

⃗ ×H
⃗ = J⃗ + ∂ D⃗ es una extensión de la ley de Ampère, mencionada
Por último, la ecuación ∇
∂t
anteriormente. Hay que notar que ésta implica la ecuación de continuidad.
Es claro que las ecuaciones de Maxwell representan expresiones matemáticas de ciertos resultados experimentales. Resulta evidente entonces que no pueden demostrarse, sin embargo,
la aplicabilidad para cualquier situación puede verificarse.
⃗ + ⃗v × B),
⃗ que describe la acción de
Junto con la ecuación de la fuerza de Lorentz, F⃗ = q(E
los campos sobre partículas cargadas, este conjunto de leyes nos da una descripción clásica
completa de las partículas que actúan electromagnéticamente.

---

### Página 515

14.2.1.

Vector de Poynting- Conservación de la Energía

Las ecuaciones de Maxwell son consistentes con la ley de conservación de la carga eléctrica
⃗ · J(t,
⃗ ⃗x) + ∂ρ(t, ⃗x) = 0
∇
∂t
o, en su forma integral
⃗ x) · J(⃗
⃗ x) = − d
dS(⃗
dt
S(V )

ˆˆ

✞☎
✝✆

˚

d3 xρ(⃗x)

V

intentemos establecer una ley equivalente para la Conservación de la energía. Podemos
comenzar el análisis definiendo una densidad de energía electromagnética ϵ(t, ⃗x). Del mismo
⃗ ⃗x), donde
modo, definimos el vector de Poynting S(t,
⃗ ⃗x) · dS(⃗
⃗ x)
S(t,

⃗ x) por unidad de tiemes la energía electromagnética de campo cruzando una superficie dS(⃗
⃗ ⃗x) están claramente inspiradas en ρ(t, ⃗x)
po. Notar que nuestras definiciones de ϵ(t, ⃗x) y S(t,
⃗ ⃗x). Uno podría pensar entonces que la ley de conservación de la energía se escribe en la
y J(t,
forma
ˆˆ
˚
d
✞☎
⃗ x) · S(t,
⃗ ⃗x)
−
d xϵ(t, ⃗x) = ✝ ✆ dS(⃗
dt
V
S(V )
Sin embargo, esto no está correcto, pues falta incluir un término que involucre el trabajo
realizado por los campos sobre las cargas presentes en la región V (por unidad de tiempo). La
fuerza neta que actúa sobre un elemento de carga por unidad de volumen es (de acuerdo a la
fuerza de Lorentz)
⃗ + J⃗ × B
⃗ = ρ(E
⃗ + ⃗v × B)
⃗
f⃗ = ρE
de forma que el trabajo realizado sobre las cargas por unidad de tiempo es
˚
˚
!
" ˚
3 ⃗
⃗
⃗ x) · E(⃗
⃗ x)
W =
d xf · ⃗v =
d xρ(⃗x) E(⃗x) · ⃗v (⃗x) =
d3 x′ J(⃗
V

V

V

Luego, la ley de conservación de la energía debe ser como sigue
ˆˆ
˚
˚
d
✞☎
⃗
⃗
⃗ x) · E(⃗
⃗ x)
−
d xϵ(t, ⃗x) = ✝ ✆ dS(⃗x) · S(t, ⃗x) +
d3 xJ(⃗
dt
V
S(V )
V
La interpretación es bien clara: la disminución de energía por unidad de tiempo en un
volumen V es igual al flujo de energía electromagnética por unidad de tiempo a través del
contorno de V más el trabajo reaizado sobre las cargas en V por unidad de tiempo. En su
forma diferencial
∂ϵ(t, ⃗x) ⃗ ⃗
⃗ ⃗x) · E(t,
⃗ ⃗x)
+ ∇ · S(t, ⃗x) = −J(t,
∂t
Veamos que una expresión de este tipo se obtiene a partir de las ecuaciones de Maxwell
⃗
1 ⃗
⃗ ⃗x) − ϵ0 ∂ E(t, ⃗x)
J⃗ = ∇
× B(t,
µ0
∂t

---

### Página 516

⃗ ⃗x) · E(t,
⃗ ⃗x) = −
−J(t,
Además
y

!
"
⃗
1 ⃗
⃗ × B(t,
⃗ ⃗x) + ϵ0 E(t,
⃗ ⃗x) · ∂ E(t, ⃗x)
E(t, ⃗x) · ∇
µ0
∂t

⃗
⃗ × E(t,
⃗ ⃗x) = − ∂ B(t, ⃗x)
∇
∂t
!
"
!
"
!
"
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
⃗
E(t, ⃗x) · ∇ × B(t, ⃗x) = B(t, ⃗x) · ∇ × E(t, ⃗x) − ∇ · E(t, ⃗x) × B(t, ⃗x)

!
!
"
!
""
⃗
⃗ ⃗x) · ∇
⃗ × E(t,
⃗ ⃗x) − ∇
⃗ · E(t,
⃗ ⃗x) × B(t,
⃗ ⃗x) +ϵ0 E(t,
⃗ ⃗x) ∂ E(t, ⃗x)
⃗ ⃗x)·E(t,
⃗ ⃗x) = − 1 B(t,
−J(t,
µ0
∂t
⃗
⃗
⃗ ⃗x) · E(t,
⃗ ⃗x) = 1 B(t,
⃗ ⃗x) · ∂ B(t, ⃗x) + ϵ0 E(t,
⃗ ⃗x) ∂ E(t, ⃗x) + ∇
⃗ ·
−J(t,
µ0
∂t
∂t

⃗ ⃗x) · E(t,
⃗ ⃗x) = ∂
−J(t,
∂t

%

#

⃗
⃗ ⃗x) × B(t, ⃗x)
E(t,
µ0

$

#
$
&
⃗ ⃗x)
1 ⃗2
B(t,
1 ⃗2
⃗ · E(t,
⃗ ⃗x) ×
B (t, ⃗x) + ∇
ϵ0 E (t, ⃗x) +
2µ0
µ0

⃗
Comparando con nuestra expresión anterior, obtenemos fórmulas explícitas para ϵ y S
1 ⃗2
1 ⃗2
(t, ⃗x) +
B (t, ⃗x)
ϵ(t, ⃗x) = ϵ0 E
2µ0
⃗ ⃗x) = 1 E(t,
⃗ ⃗x) × B(t,
⃗ ⃗x)
S(t,
µ0

---

### Página 517

14.3.

Ecuaciones de Maxwell en un Medio Lineal, Homogéneo e Isotrópico

⃗ yE
⃗ en general está dada por
Es bien sabido que la relación entre los campos D
!
"
⃗
⃗ ⃗x)
⃗
D(t, ⃗x) = ϵ0 P + E(t,

Sin embargo, en ciertos medios, la polarización depende linealmente del campo eléctrico
(medios lineales), de forma que
⃗ ⃗x) = ϵE(t,
⃗ ⃗x)
D(t,
donde ϵ es la permitividad del medio, y no depende de ⃗x para medios homogéneos e isotrópicos.
⃗ está relacionado con B
⃗
Del mismo modo, en este tipo de medios simples, el campo H
mediante
⃗ ⃗x) = 1 B(t,
⃗ ⃗x)
H(t,
µ
donde µ es la permeabilidad del medio. De esta forma las ecuaciones de Maxwell se pueden
escribir como
⃗ · E(t,
⃗ ⃗x) = ρ(t, ⃗x)
∇
ϵ
⃗ ⃗x)
⃗ × E(t,
⃗ ⃗x) = − ∂ B(t,
∇
∂t
⃗ · B(t,
⃗ ⃗x) = 0
∇

⃗ ⃗x)
⃗ × B(t,
⃗ ⃗x) = µJ(t,
⃗ ⃗x) + µϵ ∂ E(t,
∇
∂t
⃗ y B,
⃗ donde propiedades del medio
Es un sistema de ecuaciones diferenciales acoplado para E
se incluyen en ϵ y µ

---

### Página 518

Problema
Un cable coaxial consiste de dos conductores cilíndricos concéntricos , el interior de radio a y
el exterior de radio b (ambos con resistencia nula). La longitud de ambos cables l es tal que
l >> b. El cable transmite energía en DC desde una batería a una carga. La batería provee
una fem ε entre ambos conductores en un extremo del cable , y la carga es una resistencia R
conectada entre los conductores al otro extremo del cable. Una corriente I fluye a través del
conductor interior y regresa por el conductor exterior. La batería carga el conductor interno
con carga −Q y el externo con +Q

a) Encuentre el campo eléctrico en todas partes
⃗ en todas partes
b) Encuentre la dirección y magnitud de B
c) Calcule el vector de Poynting al interior del cable
⃗ sobre una superficie apropiada, encuentre la potencia que fluye en el cable
d) Al integrar S
coaxial
#### Solución
a) Despreciando efectos de borde, se puede calcular el campo eléctrico mediante la ley de Gauss,
utilizando como superficie de integración un cilindro de largo h y radio r, con a < r < b, como
se muestra en la figura

ˆˆ

ˆˆ

ˆˆ

☎
☎
✞☎ ⃗ ′
⃗ x′ ) = ✞
⃗ x′ ) = ✞
x ) · E(⃗
x′ )n̂(⃗x′ ) · E(⃗
✝ ✆dS(⃗
✝ ✆dS(ϕ, z)r̂ · E(r)r̂
✝ ✆dS(⃗
S

S

ˆˆ

S

ˆˆ

✞☎ ⃗ ′
☎
⃗ x′ ) = E(r) ✞
x ) · E(⃗
✝ ✆dS(⃗
✝ ✆dS(r, ϕ, z) = E(r)2πrh
S

S

la carga encerrada por S es
qint = 2πahσ

---

### Página 519

donde σ es la densidad de carga (homogénea) en el conductor interno
σ=

−Q
2πaL

con esto
2πah
E(r)2πrh =
ϵ0
E(r) =

'

−Q
2πaL

(

−Q
2πrLϵ0

de forma que el campo eléctrico entre ambos conductores está dado por
⃗
E(r)
=

−Q
r̂
2πrLϵ0

Además, se sabe
ε = φ(b) − φ(a) = −

ˆ b
a

⃗ x′ )
d⃗x′ · E(⃗

tomando una curva parametrizada por ⃗x = rr̂, con r̂ alguna dirección radial fija, y a < r < b,
se obtiene
′

ˆ b

ˆ b

−Q
Q
ε=−
drE(r) = −
dr
=
2πrLϵ0
2πLϵ0
a
a
ε=

ˆ b

dr
a r

Q
ln(b/a)
2πLϵ0

luego
Q = ε2πLϵ0 ln(a/b)
y
−ε ln (a/b)
⃗
r̂
E(r)
=
r
por supuesto, que el campo eléctrico para r < a es nulo (interior de un conductor), y lo
mismo ocurre para r > b, pues el cable coaxial es eléctricamente neutro.
b) El campo magnético para a < r < b puede se obtenido mediante la ley de Ampère,
utilizando como contorno una curva circular Γ concéntrica al conductor interno y de radio r.

---

### Página 520

Notar que el sentido de la corriente por el conductor interno es según ẑ. Por simetría, el
campo magnético sólo dependerá de la variable r, y será tangente a la curva Γ en todos sus
puntos
˛
ˆ 2π
⃗
⃗ ϕ̂ = 2πrB(r)
d⃗x · B(⃗x) =
dϕrϕ̂ · B(r)

Γ

la corriente encerrada por Γ es simplemente I, luego
˛
⃗ x) = µ0 I
d⃗x · B(⃗
Γ

2πrB(r) = µ0 I
µ0 I
⃗
B(r)
=
ϕ̂
2πr
El campo magnético es nulo para r > a (Cualquier curva encierra una corriente nula, pues
ambos conductores llevan I en sentidos opuestos).
c) El vector de Poynting al interior del cable (a < r < b) está dado por
'
('
(
1 −ε ln (a/b)
1 ⃗
µ0 I
⃗
⃗
S(r) = E(r) × B(r) =
r̂ × ϕ̂
µ0
µ0
r
2πr
−Iε ln (a/b)
⃗
ẑ
S(r)
=
2πr2
El vector de Poynting representa un flujo de energía por unidad de tiempo y área en dirección
−ẑ (es decir, desde la fem hacia la resistencia). Para calcular la potencia que se transmite a
través de la línea se debe calcular el flujo del vector Poynting sobre una sección transversal
entre ambos conductores, esto es

P =

¨

S

⃗ x) · S(⃗
⃗ x) =
dS(⃗

ˆ 2π

ˆ b

−Iε ln (a/b)
dϕ
drr(−ẑ) ·
ẑ = Iε ln (a/b)
2πr2
a

ˆ b
a

dr

r

P = εI
que es efectivamente la potencia que se disipa en la resistencia. Con este ejemplo se ilustra
como los campos realmente son los que transportan la energía desde la fuente a la carga

---

### Página 521

Problema
Un condensador de placas paralelas circulares se está cargando de modo que entre las placas
⃗
existe un campo eléctrico E(t)
aproximadamente uniforme. Obtenga el campo magnético entre
las placas del condensador en función de la distancia r al eje del mismo.

#### Solución
De la cuarta ecuación de Maxwell, tenemos que
⃗
⃗ ×H
⃗ = J⃗ + ∂ D
∇
∂t
en este caso, para la región entre placas
J⃗ = ⃗0
⃗ = ϵ0 E,
⃗ yH
⃗ = B/µ
⃗ 0 , con lo que
Además, en el vacío se tiene D
⃗
⃗
⃗ ×B
⃗ = ϵ 0 µ0 ∂ E = 1 ∂ E
∇
∂t
c ∂t
Ahora, integrando sobre una circunferencia a distancia r del eje de las placas, y utilizando
el teorema de Stokes
˛

C

!
" ¨
⃗
⃗
⃗
⃗
⃗ x) · 1 ∂ E(⃗x)
dS(⃗x) · ∇ × B(⃗x) =
dS(⃗
c2 ∂t
S
S
¨
˛
1 d
⃗
⃗ x) · E(⃗
⃗ x) = 1 d (Eπr2 )
d⃗x · B = 2
dS(⃗
c dt S
c2 dt
C

⃗ =
d⃗x · B

¨

˛

C

⃗ = B2πr =
d⃗x · B

Finalmente
B=

r dE
2c2 dt

πr2 dE
c2 dt

---

### Página 522

Parte VIII
Ondas Electromagnéticas

---

### Página 523

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 524

#### Capítulo 15
Ondas Planas Monocromáticas
Una de las consecuencias importantes de las ecuaciones de Maxwell, es la predicción de la
existencia de ondas electromagnéticas que se propagan a la velocidad de la luz (La luz es, en
efecto, una onda electromagnética)
c= √
µϵ
La razón es que un campo eléctrico variable en el tiempo produce un campo magnético y vice
versa. El acoplamiento entre estos dos campos lleva a la generación de ondas electromagnéticas.
Esta predicción fue confirmada por Hertz en 1887

Fig. 15.1: Heinrich Hertz
Heinrich Hertz (1857-1894) Físico Alemán. Clarificó y expandió la teoría electromagnética
de la luz que fue propuesta por Maxwell. Fue el primero en demostrar de forma satisfactoria la
existencia de ondas electromagnéticas al construír un aparato para producir y detectar ondas
de radio.

15.1.

Ondas electromagnéticas planas en medios no conductores y libres de fuentes

Sabemos que cargas y corrientes son fuentes de campos electromagnéticos. Más adelante
veremos exactamente como son creados estos campos a partir de cierta distribución de fuentes.
Por el momento, mostraremos algunas soluciones particulares a las ecuaciones de Maxwell, en
primer lugar, las ondas planas. Supongamos que se quiere estudiar el comportamiento de los
campos en una región del espacio libre de fuentes (Es evidente que para que existan campos,
deben existir fuentes en algun lugar del espacio). Lo que quiero decir con esto es que encontraremos un tipo de solución para regiones que están lejos de las fuentes (es decir ρ(t, ⃗x) = 0 en
la zona de interés). También asumiremos que el medio en el cual se propagan las ondas no es

---

### Página 525

⃗ ⃗x) en respuesta
buen conductor, en ese caso tampoco existirá una densidad de corriente J(t,
al campo eléctrico. En este caso las ecuaciones de Maxwell son
⃗ · E(t,
⃗ ⃗x) = 0
∇

⃗ × E(t,
⃗ ⃗x) = − ∂ B(t,
⃗ ⃗x)
∇
∂t
⃗ · B(t,
⃗ ⃗x) = 0
∇

⃗ × B(t,
⃗ ⃗x) = µϵ ∂ E(t,
⃗ ⃗x)
∇
∂t
Utilizaremos ahora la conocida identidad

De esta forma

"
!
⃗
⃗
⃗
⃗
⃗
⃗
⃗ 2 f⃗
∇×∇×f =∇ ∇·f −∇
!
"
⃗ ⃗x)
⃗ ×∇
⃗ × E(t,
⃗ ⃗x) = ∇
⃗ ∇
⃗ · E(t,
⃗ ⃗x) − ∇
⃗ 2 E(t,
∇

pero en regiones libre de fuentes

⃗ · E(t,
⃗ ⃗x) = 0
∇
como indica la primera ecuación de Maxwell. Así
⃗ ×∇
⃗ × E(t,
⃗ ⃗x) = −∇
⃗ 2 E(t,
⃗ ⃗x)
∇
por otro lado

de forma que

!
"
⃗ ×∇
⃗ × E(t,
⃗ ⃗x) = −∇
⃗ × ∂ B(t,
⃗ ⃗x) = − ∂ ∇
⃗ × B(t,
⃗ ⃗x)
∇
∂t
∂t
(
'
∂2 ⃗
∂ ⃗
∂
⃗
⃗
⃗
µϵ E(t, ⃗x) = −µϵ 2 E(t,
⃗x)
∇ × ∇ × E(t, ⃗x) = −
∂t
∂t
∂t
⃗ ⃗x) − µϵ ∂ E(t,
⃗ ⃗x) = 0
⃗ 2 E(t,
∇
∂t2

definiendo

c= √
µϵ

⃗ 2 E(t,
⃗ ⃗x) − 1 ∂ E(t,
⃗ ⃗x) = 0
∇
c2 ∂t2
Esta es la conocida Ecuación de Onda. Es decir, hemos llegado a que en un medio libre
de cargas y no conductor, el campo eléctrico satisface la ecuación de onda. Las soluciones
son ondas que se propagan a velocidad c. Es fácil verificar que el campo magnético satisface
exactamente la misma ecuación, en efecto
!
"
⃗ ⃗x) = −∇
⃗ 2 B(t,
⃗ ⃗x)
⃗ ×∇
⃗ × B(t,
⃗ ⃗x) = ∇
⃗ ∇
⃗ · B(t,
⃗ ⃗x) − ∇
⃗ 2 B(t,
∇

---

### Página 526

por otro lado
'

(
∂
⃗ ×∇
⃗ × B(t,
⃗ ⃗x) = ∇
⃗ × µϵ E(t,
⃗ ⃗x)
∇
∂t

⃗ ⃗x)
⃗ ×∇
⃗ × B(t,
⃗ ⃗x) = µϵ ∂ ∇
⃗ × E(t,
⃗ ⃗x) = −µϵ ∂ B(t,
∇
∂t
∂t2
En resumen

⃗ 2 E(t,
⃗ ⃗x) − 1 ∂ E(t,
⃗ ⃗x) = 0
∇
c2 ∂t2

⃗ ⃗x) − 1 ∂ B(t,
⃗ ⃗x) = 0
⃗ 2 B(t,
∇
c2 ∂t2
⃗ ⃗x) y B(t,
⃗ ⃗x).
son las ecuaciones desacopladas para los campos E(t,
Ecuación de Onda en una dimensión
La forma general de la ecuación de onda en una dimensión es
' 2
(
∂
1 ∂2
ψ(x, t) = 0
−
∂x2 c2 ∂t2
Resulta inmediato verificar que cualquier función de la forma ψ(x ± ct) satisface la ecuación
′
de onda en una dimensión. La demostración es la siguiente: Sea x′ = x ± ct, con esto ∂x
=1y
∂x
∂x′
= ±c. Usando la regla de la cadena
∂t
∂ψ(x′ ) ∂x′
∂ψ(x′ )
∂ψ(x′ )
=
=
∂x
∂x′ ∂x
∂x′
'
(
∂ 2 ψ(x′ ) ∂x
∂ 2 ψ(x′ )
∂ ∂ψ(x′ )
∂ 2 ψ(x′ )
=
=
=
∂ 2 x′
∂x
∂x′
∂x′2 ∂x′
∂x′2

Similarmente, las derivadas parciales con respecto a t son
∂ψ
∂ψ ∂x′
∂ψ
=
= ±c ′
′
∂t
∂x ∂t
∂x
∂
∂2ψ
=
∂t
∂t
Luego

'

∂ψ
± ′
∂x

(

=±

∂ 2 ψ ∂x′
2∂ ψ
=
c
∂x′2 ∂t
∂x′2

∂2ψ
∂2ψ
2∂ ψ
=
=
c
∂x′2
∂x2
∂t2
lo cual muestra que ψ(x ± ct) es solución de la ecuación de onda en una dimensión. La
ecuación de onda es un ecuación diferencial lineal, lo que impica que si ψ1 (x, t) y ψ2 (x, t) son
soluciones de la ecuación de onda, entonces ψ1 (x, t) ± ψ2 (x, t) también es solución .vLas ondas
electromagnéticas obedecen entonces el principio de superposición

---

### Página 527

Solución a la ecuación de Onda
Para resolver la ecuación de onda que satisfacen los campos electromagnéticos, supondremos que
la variación temporal de éstos es de la forma eiwt ( es decir, tienen una dependencia oscilatoria
en el tiempo a una frecuencia bien determinada, w). A este tipo de ondas las llamaremos
monocromáticas
⃗ ⃗x) = E(⃗
⃗ x)eiwt
E(t,
⃗ ⃗x) = B(⃗
⃗ x)eiwt
B(t,
de forma que
∂2 ⃗
⃗ x)
E(t, ⃗x) = −w2 E(⃗
∂t2
⃗ x) satisface
Entonces la parte espacial E(⃗

⃗ 2 E(⃗
⃗ x) + w E(t,
⃗ ⃗x) = 0
∇
c2
busquemos una solución de la forma
⃗ x) = E
⃗ 0 e−i⃗k·⃗x
E(⃗
⃗ 0 es un vector constante
donde ⃗k =| ⃗k | k̂ y E
⃗ 2 E(⃗
⃗ x) = ∇
⃗ 2E
⃗ 0 e−i(kx x+ky y+kz z) = −k 2 E
⃗ 0 ei⃗k·⃗x
∇
donde k =| ⃗k |, de forma que
⃗

⃗ 0 e−ik·⃗x +
−k 2 E

w2 ⃗ −i⃗k·⃗x
E0 e
=0
c2

En efecto, es solución si
k=

)

w
c

Finalmente, hemos encontrado que una solución de la ecuación de onda en medios no conductores y libres de cargas son campos de la forma
⃗ ⃗x) = E
⃗ 0 ei(wt−⃗k·⃗x)
E(t,
⃗ ⃗x) = B
⃗ 0 ei(wt−⃗k·⃗x)
B(t,
con | ⃗k |= wc . Sin embargo, los campos deben tener divergencia nula, de forma que
del mismo modo

⃗ · E(t,
⃗ ⃗x) = 0 → ⃗k · E
⃗0 = 0
∇
⃗ · B(t,
⃗ ⃗x) = 0 → ⃗k · B
⃗0 = 0
∇

Ambos campos deben ser transversales (perpendiculares a la dirección de propagación)
Propagación en el eje z
Supongamos ahora que la dirección de propagación de los campos es en la dirección del eje z,
es decir
⃗k = β k̂ = w k̂
c

---

### Página 528

y

⃗k · ⃗x = βz
entonces

⃗ z) = E
⃗ 0 ei(wt−βz)
E(t,
⃗ z) = B
⃗ 0 ei(wt−βz)
B(t,

además, ambos campos deben ser perpendiculares al eje z. Por ejemplo, si escogemos
⃗ z) = E0 ei(wt−βz) î
E(t,
de la ecuación
se obtiene

⃗ × E(t,
⃗ z) = − ∂ B(t,
⃗ z)
∇
∂t
∂
⃗ 0 ei(wt−βz)
E0 ei(wt−βz) ĵ = −iβE0 ei(wt−βz) ĵ = −iwB
∂z

entonces
y se desprende que

⃗ 0 ei(wt−βz)
iβE0 ei(wt−βz) ĵ = iwB
⃗ 0 = E0 ĵ
B
c

Finalmente
⃗ z) = E0 ei(wt−βz) î
E(t,
⃗ z) = B0 ei(wt−βz) ĵ
B(t,
B0
=
E0
c
w
β=
c

⃗ yB
⃗ están siempre en fase, es decir, alcanzan sus máximos y mínimos al mismo
Vemos que E
tiempo.
Nota
Por supuesto que los campos físicos se obtienen al tomar la parte real de las soluciones encontradas
⃗ z) = E0 cos (wt − βz) î
E(t,
⃗ z) = E0 cos (wt − βz) ĵ
B(t,
c

---

### Página 529

Resumen
⃗ y B
⃗ son perpendiculares a la dirección de
1. Las ondas son transversales ya que tanto E
⃗ ×B
⃗
propagación, que coincide con la dirección del producto E
⃗
⃗
⃗
⃗ =0
2. Los campos E y B son perpendiculares entre sí. Es decir E · B
3. La razón entre las magnitudes de los campos es
E0
w
= =c= √
B0
β
µ0 ϵ 0
4. La velocidad de propagación es igual a la velocidad de la luz en el medio c = √1µϵ
5. Las ondas electromagnéticas obedecen el principio de superposición
Vector Poynting
En general, el flujo de Energía por unidad de área (y tiempo) está descrito por el vector de
Poynting
⃗ ⃗x) = 1 E(t,
⃗ ⃗x) × B(t,
⃗ ⃗x) = E(t,
⃗ ⃗x) × H(t,
⃗ ⃗x)
S(t,
µ
Debido a que los campos son perpendiculares
⃗ ⃗x) |=
| S(t,

1 ⃗
⃗ ⃗x) |= 1 | E(t,
⃗ ⃗x) || B(t,
⃗ ⃗x) |
| E(t, ⃗x) × B(t,
µ
µ

En el caso de las ondas planas monocromáticas recién visto
⃗ ⃗x) = 1 E0 B0 cos2 (wt − βx) k̂
S(t,
µ c
Como es de esperar, el vector de Poynting apunta en la dirección de propagación

⃗ | es
La intensidad de la onda I, definida como el promedio temporal de | S
I=
donde hemos usado

+ E0 B0
E0 B0 * 2
E2
cB02
cos (wt − βx) =
= 0 =
µ
2µ
2cµ
2µ
*

+
cos2 (wt − βx) = 1/2

Notar que la magnitud de la intensidad es constante. Por supuesto que esto no es muy realista, pues es bien sabido de la vida diaria que la energía de la radiación decae con la distancia.
Veremos más adelante que los campos electromagnéticos tienen en general la forma de ondas
esféricas, cuya amplitud decae como el inverso de la distancia 1/r, de forma que la magnitud
del vector poynting decae como 1/r2 . Por supuesto que las ondas planas, si bien son soluciones

---

### Página 530

de las ecuaciones de Maxwell, constituyen sólo un estudio aproximado de los campos electromagnéticos muy distantes de las fuentes. (Por ejemplo, de la radiación producida por el Sol en
la tierra, se puede suponer que la magnitud de los campos es constante). Veremos también que
es posible generar ondas planas teóricamente, pero en la práctica no

---

### Página 531

Ejemplo
En la superficie de la atmósfera terrestre, la magnitud del vector Poynting (en promedio temporal) es ⟨S⟩ = 1,35 × 103 (W/m2 ).
a) Asumiendo que la radiación solar en la superficie de la atmósfera consiste en una onda sinusoidal plana, ¿Cuáles son las magnitudes del campo eléctrico y magnético ?
b) ¿Cual es el promedio temporal de la potencial radiada por el Sol? La distancia media entre
el Sol y la Tierra es R = 1,5 × 1011 m
#### Solución
a) El promedio temporal del vector Poynting esta relacionado con la magnitud del campo
eléctrico según
ϵ0 cE02
⟨S⟩ =
La amplitud del campo eléctrico es entonces
,
,
2 ⟨S⟩
2 (1,35 × 103 W/m2 )
E0 =
=
= 1,01 × 103 V /m
cϵ0
(3 × 108 m/s) (8,85 × 10−12 C 2 /N m2 )
La magnitud del campo magnético es
B0 =

E0
1,01 × 103 V /m
=
= 3,4 × 10−6 T = 3,4µT
c
3 × 108 m/s

Notar que este campo magnético es menor que el campo magnético terrestre, que varía entre
30 y 60 µ T
b) La potencia total irradiada por el Sol a una distancia R es (en promedio)
. .2
⟨P ⟩ = ⟨S⟩ 4πR2 = 1,35 × 103 W/m2 4π 1,5 × 1011 m = 3,8 × 1026 W

Por supuesto que aquí hemos supuesto que la radiación emitida por el sol corresponde a
ondas esféricas. La intensidad a una distancia r del Sol es
I = ⟨S⟩ =

⟨P ⟩
4πr2

la cual decrece como 1/r2

Fig. 15.2: Como veremos más adelante, los campos de radiación en general son ondas esféricas

---

### Página 532

15.2.

Ondas Planas en medios conductores

Veremos que las soluciones para las ondas electromagnéticas planas en medios conductores
difieren bastante en su comportamiento con respecto al caso de un medio dieléctrico perfecto (no
conductor) que vimos anteriormente. Aceptaremos ahora que el medio tenga una conductividad
σ, de forma que existirá una corriente eléctrica en el medio en respuesta al campo eléctrico. Si
el medio es ohmico
⃗ ⃗x) = σ E(t,
⃗ ⃗x)
J(t,
Claramente seguiremos suponiendo que el medio es lineal, homogéneo e isotrópico, de forma
que las ecuaciones de Maxwell quedan
⃗ · E(t,
⃗ ⃗x) = 0
∇
⃗
⃗ × E(t,
⃗ ⃗x) = − ∂ B(t, ⃗x)
∇
∂t
⃗ · B(t,
⃗ ⃗x) = 0
∇
⃗ × B(t,
⃗ ⃗x) = µσ E(t,
⃗ ⃗x) + µϵ ∂ E(t,
⃗ ⃗x)
∇
∂t

Al igual que antes, evaluamos

Además

"
!
⃗ ×∇
⃗ × E(t,
⃗ ⃗x) = ∇
⃗ ∇
⃗ · E(t,
⃗ ⃗x) − ∇
⃗ 2 E(t,
⃗ ⃗x) = −∇
⃗ 2 E(t,
⃗ ⃗x)
∇
⃗ ×∇
⃗ × E(t,
⃗ ⃗x) = −∇
⃗ × ∂ B(t,
⃗ ⃗x) = − ∂ ∇
⃗ × B(t,
⃗ ⃗x)
∇
∂t
∂t

⃗ ×∇
⃗ × E(t,
⃗ ⃗x) = − ∂
∇
∂t

'

(
∂ ⃗
∂ ⃗
∂2 ⃗
⃗
⃗x)
µσ E(t, ⃗x) + µϵ E(t, ⃗x) = −µσ E(t,
⃗x) − µϵ 2 E(t,
∂t
∂t
∂t

con esto,la ecuación para el campo eléctrico es
⃗ ⃗x) − µϵ ∂ E(t,
⃗ ⃗x) − µσ ∂ E(t,
⃗ 2 E(t,
⃗ ⃗x) = 0
∇
∂t
∂t

Es fácil verificar, siguiendo los mismos pasos, que el campo magnético satisface la misma
ecuación
⃗ 2 B(t,
⃗ ⃗x) = 0
⃗ ⃗x) − µϵ ∂ B(t,
⃗ ⃗x) − µσ ∂ B(t,
∇
∂t
∂t
La única diferencia con el caso anterior (propagación en medios dieléctricos perfectos) la
∂ ⃗
constituye el término µσ ∂t
E(t, ⃗x). Veremos que la conductividad del medio tendrá como efecto
una atenuación de las ondas a medida que penetra en el material. Nuevamente supondremos
que los campos son de la forma

⃗ ⃗x) = E(⃗
⃗ x)eiwt
E(t,

---

### Página 533

luego
Definimos

!

"
⃗
⃗ x)eiwt = 0
∇ + µϵw − iµσw E(⃗
k 2 = w2 µϵ − iµσw

y la ecuación queda de la forma
!

"
⃗ 2 + k 2 E(⃗
⃗ x) = 0
∇

Si la propagación es en el eje z, entonces la ecuación a resolver es
(
' 2
∂
⃗ x) = 0
+ k E(⃗
∂z 2
cuya solución es, por supuesto
⃗ x) = E
⃗ 0 e−ikz
E(⃗
y entonces la solución completa queda
⃗ ⃗x) = E
⃗ 0 ei(wt−kz)
E(t,
Así

Hay que recordar que k es un número complejo, que escribiremos en la forma k = β − iα.
k 2 = µϵw2 − iµσw = β 2 − α2 − 2iαβ
se debe resolver
2αβ = µσw → α =
β 2 − α2 = µϵw2 → β 2 −
β2 −

β =

µ2 σ 2 w 2
= w2 µϵ
4β

µ2 σ 2 w 2
= w2 µϵ
4β

β 4 − β 2 w2 µϵ −

µσw
2β

µ2 σ 2 w 2
=0

/
w 4 µ2 ϵ 2 + µ2 σ 2 w 2
w µϵ ± w µϵ 1 + wσ2 ϵ2

w2 µϵ ±

β2 =

Obviamente la solución correcta es con el signo positivo, pues β es real
#)
$
! σ "2
µϵ
β 2 = w2
1+
+1
wϵ
1# #
$
)
! σ "2
2 µϵ
1+
+1
β = w3
wϵ

---

### Página 534

y como
α2 = β 2 − w2 µϵ
µϵ
α2 = w 2

#)

1+

! σ "2
wϵ

$

+1

− w2 µϵ

#)
$
! σ "2
µϵ
α2 = w 2
1+
−1
wϵ
1# #
$
)
! σ "2
2 µϵ
1+
−1
α = w3
wϵ
#### Solución
Se concluye que las ondas planas monocromáticas en un medio con conductividad σ son de la
forma
⃗ z) = E
⃗ 0 e−αz ei(wt−βz)
E(t,
⃗ 0 debe
donde hemos asumido que la propagación es en la dirección z, y al igual que antes E
ser un vector perpendicular a z. Notar que la amplitud de la onda es atenuada por un factor
exponencial e−iαz , por lo que α es llamada Constante de atenuación
1# #
$
)
! σ "2
2 µϵ
β = w3
1+
+1
wϵ
1# #
$
)
! σ "2
2 µϵ
α = w3
1+
−1
wϵ

Ésta es la solución exacta para ondas planas monocromáticas en un medio lineal y de conductividad σ. Notar que para un dieléctrico perfecto, la constante de atenuación es cero y se
recupera el caso visto anteriormente
Observación
Este factor exponencial atenuante es el que explica que en ciertos materiales las ondas no se
propaguen correctamente. Por ejemplo, para el agua de mar (que constituye un medio conductor), dentro de un gran rango de frecuencias el factor α es grande, de forma que las ondas
decaen bastante rápido. (Esto explica en parte por qué los submarinos no se comunican mediante ondas electromagnéticas)
La razón física de este factor atenuante radica en la naturaleza misma del medio. Por ser
conductor, existe una gran cantidad de cargas libres que son aceleradas por la prescencia del
campo eléctrico (principalmente, pues ya es sabido que su magnitud es muchísimo mayor a
la del campo magnético). De esta forma, parte de la energía electromagnética que se propaga
es utilizada en trabajo para mover las cargas libres presentes en el medio. Con esto, resulta
natural que la onda electromagnética pierda energía a medida que avanza en el material

---

### Página 535

⃗ 0 = E0 î. Nuevamente, de la ley de Faraday podemos determinar
Supongamos ahora que E
la relación entre las magnitudes de los campos
⃗ × E(t,
⃗ ⃗x) = − ∂ B(t,
⃗ ⃗x)
∇
∂t
∂
⃗ 0 e−αz ei(wt−βz)
k̂ × E0 e−αz ei(wt−βz) î = −iwB
∂z
⃗ 0 e−αz ei(wt−βz)
(iβ + α) × E0 e−αz ei(wt−βz) ĵ = iwB

⃗ 0 = B0 ĵ con
Se obtiene B

B0 =

iβ + α
E0
iw

β − iα
k
E0 = E0
w
w
/
k = w2 µϵ − iµσw

B0 =
con

B0 =
y entonces

)

iµσ
E0 =
µϵ −
w
E0
=
B0

o
E0
=
H0

,

)

)

µσ + iwµϵ
E0
iw

iw
σµ + iwµϵ

iwµ
=η
σ + iwϵ

Esta razón, que depende de las características del medio (µ, ϵ, σ) y de la frecuencia w, se
conoce como impedancia característica del medio. Notar que en general (σ ̸= 0) es un
número complejo, esto quiere decir que para medios con conductividad, el campo eléctrico y
magnético no están en fase
La impedancia característica en representación polar es
η =| η | eiϑ
donde
| η |=
y

#

w
µ

/

(σ 2 + w2 ϵ2 )

$1/2

ϑ=

=

#

µ/ϵ
/ σ
( ϵw )2 + 1)

$1/2

(π/2 − Arctan(wϵ/σ))
σ
tan 2ϑ =
wϵ

/
µ/ϵ
=!
- σ .2 "1/4
1 + wϵ

---

### Página 536

Con esto, la solución general para ondas planas que se propagan en dirección z queda
⃗ t) = E0 e−αz ei(wt−βz) ê1
E(z,
E0 −αz i(wt−βz−ϑ)
⃗
H(z,
t) =
ê2
e e
|η|
e1 × e2 = k̂

La velocidad de propagación es

w
=,
β

(
'0
- σ .2
µϵ
1 + wϵ + 1

2π
=
β

2π
'0
(
- σ .2
µϵ
1 + wϵ + 1

c=

y la longitud de onda
λ=

w

15.3.

,

Solución para buenos conductores

Si la conductividad es grande en el sentido σ >> wϵ, entonces
1# #
$$
)
)
! σ "2
2 µϵ
µσ
β = w3
1+
+1
≈w
wϵ
2w

1# #
$$
)
)
! σ "2
2 µϵ
µσ
α=w
1+
−1
≈w
wϵ
2w

Es decir, aproximadamente se tiene
α=β=

)

wµσ

w
En términos de la frecuencia en Hertz f = 2π

α=β=

/
πf σ

En este caso los campos son atenuados rápidamente. Se define la profundidad de penetración como la distancia dentro del material a la cual los campos han decaido en un factor
1/e (aproximadamente al 30 % de su valor original)
δ=

=√
α
πf σ

Además, en este caso la impedancia característica queda
)
wµ iπ/4
E0
η=
=
e
σ
H0

Es decir, los campos se encuentran en un desfase de ϑ = π/4

---

### Página 537

⃗ t) = E0 e−αz ei(wt−βz) ê1
E(z,
E0 −αz i(wt−βz−π/4)
⃗
e e
H(z,
t) =
ê2
|η|
e1 × e2 = k̂

La velocidad de propagación es

w
c= =
β
y la longitud de onda
λ=

)

2w
= wδ
σµ

2π
2π
= 2πδ
=√
β
πf µσ

Nota: Notar que aquí, la definición de un buen conductor no es una propiedad única del
material, puesto que debe tenerse σ >> wϵ. Es decir, un material se considera buen conductor
en determinado rango de frecuencias.

15.4.

Resumen sobre las ondas planas monocromáticas

Hemos visto que las ecuaciones de Maxwell aceptan como solución campos electromagnéticos
que están descritos matemáticamente por ondas planas. Para una propagación según el eje z,
los campos son de la forma
⃗ t) = E0 e−αz ei(wt−βz) ê1
E(z,
E0 −αz i(wt−βz−ϑ)
⃗
H(z,
t) =
ê2
e e
|η|
e1 × e2 = k̂
1. En un dieléctrico perfecto (conductividad nula), la constante de atenuación es cero, y la
impedancia intrínseca es un número real puro
)
E0
E0
µ
η=
=
= √ =c
→
H0
ϵ
B0
µϵ
En el espacio vacío, la impedancia intrínseca es
)
µ0
≈ 120π
η=
ϵ0
En este caso

⃗ t) = E0 ei(wt−βz) ê1
E(z,
⃗ t) = E0 ei(wt−βz) ê2
B(z,
c
e1 × e2 = k̂

---

### Página 538

Con
β=

w
√
= w µϵ
c

2. En un buen conductor (σ >> wϵ), los campos son fuertemente atenuados a medida que
se propagan en el medio. Aquí, en un análisis aproximado
)
wµσ /
α=β=
= πf σ
la impedancia intrínseca es un complejo con fase π/4 y su magnitud es
)
wµ
| η |=
σ

Los campos son atenuados por un factor 1/e al ingresar una distancia igual a la profundidad
de penetración
δ= = =√
α
β
πf µσ

---

### Página 539

Problema
⃗ ⃗x) = Em sin (wt − βz) ĵ en el espacio libre, encuentre D(t,
⃗ ⃗x), B(t,
⃗ ⃗x) y H(t,
⃗ ⃗x). DibuDado E(t,
⃗ yH
⃗ en t = 0
je E
#### Solución
Se tiene

⃗ ⃗x) = Em sin (wt − βz) ĵ
E(t,

de aquí es inmediato que
⃗ ⃗x) = ϵ0 E(t,
⃗ ⃗x) = ϵ0 Em sin (wt − βz) ĵ
D(t,
Además, de la ecuación de Maxwell
⃗
⃗ × E(t,
⃗ ⃗x) = − ∂ B(t, ⃗x)
∇
∂t
como la propagación es en z, la única derivada parcial espacial para el campo eléctrico que
no es nula es la que involucra z, es decir
⃗
∂
⃗ ⃗x) = − ∂ B(t, ⃗x)
k̂ × E(t,
∂z
∂t
⃗
∂
⃗ ⃗x) = − ∂ Em sin (wt − βz) î = βEm cos (wt − βz) î = − ∂ B(t, ⃗x)
k̂ × E(t,
∂z
∂z
∂t
Luego

⃗ ⃗x) = − β Em sin (wt − βz) î = − Em sin (wt − βz) î
B(t,
w
c
⃗ ⃗x) es, simplemente
Por último, el campo H(t,
⃗ ⃗x) = − Em sin (wt − βz) î
⃗ ⃗x) = 1 B(t,
H(t,
µ0
µ0 c

⃗ yH
⃗ están dados por
En t = 0, los campos E
⃗ ⃗x) = −Em sin (βz) ĵ
E(0,
Em
⃗
H(0,
⃗x) =
sin (βz) î
µ0 c

---

### Página 540

Problema
⃗ = Hm ei(wt+βz) î en el espacio libre, encuentre E
⃗
Dado H
#### Solución
⃗ representa una onda plana que se
Una forma de resolver este problema es notando que H
propaga en dirección −ẑ. Luego, debe tenerse que el vector poynting tenga esta dirección, lo
cual se logra con un campo eléctrico polarizado según ĵ, en efecto
⃗=E
⃗ ×H
⃗ = E ĵ × H î = −EH k̂
S
Además, se cumple que

E
=√
B
µ0 ϵ 0

o, equivalentemente
E
=
H
y entonces

)

µ0
βµ0
=
ϵ0
w

⃗ = wµ0 Hm ei(wt+βz) ĵ
E
β

Otra forma, es recordando que el espacio vacío tiene conductividad nula y entonces
⃗
⃗ × H = ∂D
∇
∂t
⃗ × H = ∂ k̂ × H
⃗ = βHm ei(wt+βz) ĵ
∇
∂z
entonces

⃗
∂D
= βHm ei(wt+βz) ĵ
∂t
⃗ = β Hm ei(wt+βz) ĵ
D
w

⃗ = β Hm ei(wt+βz) ĵ
E
wϵ0
En efecto, es el mismo resultado anterior
√
⃗ = µ0 ϵ0 Hm ei(wt+βz) ĵ = √µ0 Hm ei(wt+βz) ĵ
E
ϵ0
µ0 ϵ 0
⃗ = wµ0 Hm ei(wt+βz) ĵ
E
β

---

### Página 541

Problema
Dados

⃗ = 30πei(108 t+βz) î, H
⃗ = Hm ei(108 t+βz) ĵ
E

en el espacio libre, encontrar Hm y β (β > 0)
#### Solución
Estas son ondas planas que satisfacen las ecuaciones de Maxwell en el vacío, de forma que
w
=√
= 3 × 108 (m/s)
β
µ0 ϵ 0
Luego
β=
Además

Luego

w
=
=
c
3 × 108

|E|
|E|
=c→
=
|B|
|H|
| Hm |=

)

µ0
= 120π
ϵ0

30π
=
120π

Además, las ondas se propagan en la dirección −k̂, por lo que
⃗ ×H
⃗ = −k̂
E
entonces
Hm = −

y
⃗ = 30πei(108 t+ 13 z) î
E
⃗ = − 1 ei(108 t+ 13 ) ĵ
H

---

### Página 542

Problema
En un medio homogéneo no conductor donde µr = 1, encuentre ϵr y w si
⃗ = 30πei(wt−(4/3)y) ẑ, H
⃗ = 1,0πei(wt−(4/3)y) î
E
¿Cuál es la velocidad de la luz en esta región?
#### Solución
Se trata de ondas planas con β = 4/3. Luego
3 × 108
w
= √
=√ =√
β
µϵ
µ0 ϵ r ϵ 0
ϵr
Además

E
= 30π =
H

)

Así

Resolviendo

µ
=
ϵ

)

µ0
= 120π
ϵr ϵ0

)

w
3 × 108
= √
4/3
ϵr
)
30π = 120π
ϵr
ϵr = 16
w = 108 (rad/s)

la velocidad de la luz en este medio es
3 × 108
c= √ = √
=
µϵ
µ0 16ϵ0
es un cuarto de la velocidad de la luz en el vacío

ϵr

---

### Página 543

Problema
⃗ = e−αz ei(wt−βz) î (V /m) con f = 100 Mhz, en la superficie de un conductor de cobre,
Suponga E
σ = 58 M S/m, localizado en z > 0 . Examine la atenuación a medida que la onda se propaga
en el interior del conductor

#### Solución
A una profundidad z, la magnitud del campo eléctrico es
⃗ |= e−αz = e−z/δ
|E
donde δ = 1/α es la profundidad de penetración
δ=√

= 6,61µm
πf µσ

Es decir, después de 6,61 micrómetros dentro del conductor, el campo es atenuado en 1e , a
un 36,8 % de su valor inicial. A 5δ o 33 micrómetros, la magnitud es 0,67 % de su valor inicial

---

### Página 544

Problema
Para agua de mar con µ = µ0 y conductividad σ ≈ 4,3 (S/m), ¿a qué frecuencia la profundidad
de penetración es de un metro?
#### Solución
Supongamos un rango de frecuencias en el que el agua de mar es considerado un buen conductor,
es decir
σ >> wϵ
(notar que la permitividad del vacío es del orden de 10−12 , y la constante dieléctrica ϵr en
general no es muy grande). La profundidad de penetración está dada por
)
)
δ=
=
µwσ
µ0 wσ
δ2 =

→w=
µ0 wσ
σµ0 δ 2

Se desea δ = 1 (m), entonces
w=
o, en Hertz

= 3,7 × 105
4,3 × 4π × 10−7 12
f=

w
= 58,6 × 103
2π

o sea, una frecuencia de aproximadamente 60 kHz para una profundidad de un metro. Si un
submarino está equipado con un receptor de muy alta sensibilidad y si se utiliza un transmisor
de muy alta potencia, es posible comunicarse con otro submarino sumergido. Sin embargo, debe
utilizarse una frecuencia muy baja, y aún en este caso se produce una atenuación muy fuerte
de la señal. En efecto, a 5 profundidades de penetración (5 metros), la magnitud de los campos
se reduce al 1 % del valor original, y por consiguiente la potencia se reduce al 0,01 % de la
potencia incidente

---

### Página 545

Problema
Una onda plana uniforme que se propaga en un medio determinado, tiene un campo eléctrico
⃗ z) = 5e−γz ei108 t ĵ
E(t,
Si el medio se caracteriza por
σ = 3,5S/m
ϵr = 1
µr = 18
⃗ , η y la profundidad de penetración para el medio. ¿Después de recorrer
Determine γ, H
qué distancia la onda se atenúa al 10 % de su valor inicial? ¿Cuál es la velocidad de propagación
en este medio?
#### Solución
Las ondas planas que son solución de las ecuaciones de Maxwell son de la forma
⃗ z) = E
⃗ 0 e−ikz eiwt
E(t,
donde
k = β − iα
⃗ z) = E
⃗ 0 e−iβz−αz eiwt
E(t,
comparando con
⃗ z) = 5e−γz ei108 t ĵ
E(t,
se aprecia que se trata de una onda plana a frecuencia w = 108 Hertz, polarizada según ĵ y
con
γ = α + iβ
Notemos que

Se aprecia que

σ
3,5
3,5
=
= 3953,02
=
wϵ
ϵ0 × 10
8,854 × 10−12 × 108
σ >> wϵ

de forma que el medio se puede considerar un buen conductor. En este caso
)
108 × 18 ∗ 4π × 10−7 × 3,5
wµσ
α≈β≈
=
= 62,9159
Con esto
γ = 62,9159 + i62,9159 =

62,9159 iπ/4
√
e

La profundidad de penetración es
δ=

= 0,0158942
α

---

### Página 546

La impedancia característica del medio es (en una muy buena aproximación)
,
)
wµ iπ/4
108 × 18 × 4π10−7 iπ/4
η=
e
e
=
= 25,4219eiπ/4
σ
3,5
⃗ z) está dado por
El campo H(t,
H(t, z) = −

5 −γz i108 t −iπ/4
5 −αz i(108 t−βz −π/4)
e e
î = −
e e
î
e
|η|
|η|

H(t, z) = −0,196681e−62,9159z ei(10 t−62,9159z −π/4) î

La velocidad de propagación está relacionada con la constante de propagación β
β=

w
→c=
= 1, 5895 × 108
c
62,9159

un poco más de la mitad de la velocidad de la luz en el vacío. Por último, para determinar
a que distancia dentro del material la onda se ha atenuado hasta un 10 % de su valor original,
se debe resolver
0,1 = e−αx = e−62,9159x
−2,30258 = −62,9159x
x = 3,65978 × 10−2 = 3,65978cm

---

### Página 547

*(Página sin texto extraíble; contiene solo figuras o contenido escaneado)*

---

### Página 548

#### Capítulo 16
Condiciones de borde en la frontera
Las condiciones que deben satisfacer los campos electromagnéticos en una zona interfacial
que separa dos madios se deducen, por supuesto, de las ecuaciones de Maxwell. La más simple
de obtener es la que cumple la componente normal del campo magnético, y se obtiene a partir
de la ecuación
⃗ · B(t,
⃗ ⃗x) = 0
∇
En cualquier zona interfacial entre dos medios se puede construír una superficie cilíndrica
como se muestra en la figura

Integrando la ecuación de Maxwell sobre el volumen limitado por el cilindro se obtiene
ˆˆ
˚
✞☎
3 ⃗
⃗
⃗
⃗ ⃗x) = 0
d x∇ · B(t, ⃗x) = ✝ ✆ dS(x̂)
· B(t,
V

¨

S1

S(V )

⃗ ⃗x) +
dS1 n̂1 · B(t,

¨

S2

⃗ ⃗x) +
dS2 n̂2 · B(t,

¨

S3

⃗ ⃗x) = 0
dS3 n̂3 · B(t,

⃗ ⃗x) es finito, el último
donde S3 es el manto del cilindro, mientras S1 y S2 las tapas. Si B(t,
término se puede anular si h → 0. Además, en este límite (h → 0) las superficies S1 y S2 son
prácticamente las mismas, S1 → S2 , con n̂1 = −n̂2 y entonces
¨
ˆˆ
"
!
✞☎
⃗
⃗
⃗
⃗
dS
d
S(x̂)
·
B(t,
⃗
x
)
=
·
B(t,
⃗
x
)
−
n̂
·
B(t,
⃗
x
)
=0
n̂
✝✆
S(V )

S1

⃗ ⃗x) − n̂1 · B(t,
⃗ ⃗x) = 0
n̂1 · B(t,
Es decir, la componente normal del campo magnético es continua al atravesar un medio

---

### Página 549

B1n = B2n
Ahora veremos que la componente tangencial del campo eléctrico es continua. A partir de
la ecuación
⃗
⃗ × E(t,
⃗ ⃗x) + ∂ B(t, ⃗x) = 0
∇
∂t
Integremos esta ecuación sobre una superficie plana rectangular como la de la figura

El contorno de S es el camino Γ indicado en la figura. Utilizando el teorema de Stokes
ˆˆ

✞☎ ⃗
✝ ✆dS(x̂) ·
S

!

ˆˆ
" ˛
⃗ ⃗x)
∂ B(t,
☎ ⃗
⃗ × E(t,
⃗ ⃗x) = d⃗x · E(t,
⃗ ⃗x) = − ✞
∇
x) ·
✝ ✆dS(⃗
∂t
Γ
S

En el caso en que h1 → 0, h2 →

lE1t − lE2t = 0
la integral de superficie por supuesto es nula ya que la superficie total tiende a cero
S →(suponemos que la derivada temporal del campo magnético es finita). De aquí se deduce
⃗ ⃗x) debe ser continua al atravesar una interfaz entre dos
que la componente tangencial de E(t,
medios
lE1t = lE2t
Utilizando ahora la primera ecuación de Maxwell
⃗ · D(t,
⃗ ⃗x) = ρ(t, ⃗x)
∇
y utilizando la misma superficie para el caso del campo magnético (cilindro de altura h) se
obtiene
˚
˚
3 ⃗
⃗
d x∇ · D(t, ⃗x) =
d3 xρ(⃗x)
V

V

✞☎
✝✆

¨

ˆˆ

V (S)

⃗ x) · D(t,
⃗ ⃗x) =
dS(⃗

d3 xρ(⃗x)

V

si h → 0, entonces
(D1n − D2n ) A = σA
donde A es la superficie de las tapas, y σ es la densidad superficial de carga en la frontera
⃗ ⃗x) es discontinua al
que divide a los dos medios. Así, la componente normal del campo D(t,
atravesar una superficie cargada

---

### Página 550

D1n − D2n = σ
o, equivalentemente para medios lineales
ϵ1 E1n − ϵ2 E2n = σ
Por último, de la ecuación
⃗ × H(t, ⃗x) = J(t,
⃗ ⃗x) + ∂D(t, ⃗x)
∇
∂t
y utilizando la misma superficie de integración que el caso del campo eléctrico, se obtiene
ˆˆ
ˆˆ
!
" ˆˆ
∂D(t, ⃗x)
✞☎ ⃗
✞☎ ⃗
✞☎ ⃗
⃗
x) · ∇ × H(t, ⃗x) = ✝ ✆dS(⃗x) · J(t, ⃗x) + ✝ ✆dS(⃗
x) ·
✝ ✆dS(⃗
∂t
S
S
S
ˆˆ
ˆˆ
˛
∂D(t, ⃗x)
✞☎ ⃗
✞☎ ⃗
d⃗x · ×H(t, ⃗x) = ✝ ✆dS(⃗x) · J(t, ⃗x) + ✝ ✆dS(⃗
x) ·
∂t
Γ
S
S
⃗ es finita
Si nuevamente h1 y h2 tienden a cero, y la derivada temporal del campo D
⃗ ⃗x) · n̂
H1t − H2t = J(t,

⃗ ⃗x)
donde n es la perpendicular a la superficie S. Es decir, la componente tangencial de H(t,
es discontinua al atravesar un medio con densidad de carga superficial en la interfaz.
Resumen
Al atravesar una interfaz entre dos medios (1 y 2), los campos electromagnéticos satisfacen
B1n = B2n
E1t = E2t
D1n − D2n = σ
H1n − H2n = J⃗ · n̂

---

### Página 551

16.1.

Condiciones de Borde para incidencia normal

Las ondas electromagnéticas que se propagan en materiales generalmente entran en el material a través de una frontera entre éste y otro medio, que puede ser aire o vacío. Aquí utilizaremos
las condiciones de borde que satisfacen los campos para el caso de ondas que inciden normalmente sobre una interfaz. (Esto significa que la dirección de propagación es perpendicular a
la frontera). Veremos que la onda incidente será acompañada por una onda reflejada y una
transmitida. Consideremos el caso que se muestra en la figura

⃗ i (x, z), H
⃗ i (y, z)) que se desplaza en el sentido positivo de z,
Se aprecia una onda incidente (E
⃗ r (y, z) describen la onda reflejada que se desplaza en el sentido negativo
⃗ r (x, z), H
los campos E
⃗ t (x, z), H
⃗ t (y, z) describen la onda transmitida. La interfaz es el plano z = 0, con el
de z, y E
medio 1 a la izquierda y el medio 2 a la derecha. Más concretamente
⃗ i (t, z) = E i e−ikz eiwt î
E
⃗ r (t, z) = E r eikz eiwt î
E
⃗ t (t, z) = E t e−ikz eiwt î
E
⃗ i (t, z) = H i e−ikz eiwt ĵ
H
⃗ r (t, z) = −H r eikz eiwt ĵ
H
⃗ t (t, z) = H t e−ikz eiwt ĵ
H

Estas son ondas planas que se propagan en dirección z. Son soluciones a las Ecuaciones de
Maxwell si
k = β − iα
Con α y β encontrados anteriormente (Son propiedad de la frecuencia y del medio en el cual
se propagan las ondas). Interesa determinar que relación se cumple entre las magnitudes de
los campos incidentes, reflejados y transmitidos. Para ello, usaremos el hecho de que el campo
eléctrico debe ser continuo en z = 0 (es completamente transversal a la interfaz). Esto significa
⃗ r (t, 0) = E
⃗ t (t, 0)
⃗ i (t, 0) + E
E
o bien
Ei + Er = Et
⃗ z) es también
Además, si no hay una corriente superficial en la interfaz, el campo H(t,
continuo en z = 0
⃗ r (t, 0) = H
⃗ t (t, 0)
⃗ i (t, 0) + H
H

---

### Página 552

o bien
Hi − Hr = Ht
⃗ y H
⃗ están dadas por las impedancias
Además, para cada onda las magnitudes entre E
intrínsecas del medio. En resumen, se debe resolver lo siguiente
Ei + Er = Et
Hi − Hr = Ht
Ei
Er
=
η
=
Hi
Hr
Et
= η2
Ht

Utilizando la última junto a las dos primeras se obtiene lo siguiente
Ei + Er
Et
=
η
=
Ht
Hi − Hr
Ei + Er
(E i − E r )
η1

η2 = 1
η2 = η 1

Ei + Er
→ E i (η2 − η1 ) = E r (η1 + η2 )
Ei − Er

Finalmente
r

E =E

i

'

η2 − η 1
η1 + η 2

(

(
2η2
E =E
η 1 + η2
'
(
η 2 − η1
r
i
H =H
η 1 + η2
'
(
2η1
t
i
H =H
η1 + η 2
t

i

'

⃗ r = 0, H
⃗ r = 0, lo cual es evidente pues en este caso
Es inmediato que si η1 = η2 , entonces E
no existe ninguna interfaz. Recordar que la impedancia de un medio está dada en general por
)
iwµ
η=
σ + iwϵ0
Para un buen conductor
)
wµ iπ/4
η≈
e
σ
Para un medio dieléctrico perfecto (conductividad nula)
)
µ
η=
ϵ

---

### Página 553

Para el espacio vacío
η=

16.1.1.

)

µ0
= 120π
ϵ0

Incidencia Normal en un conductor perfecto: Ondas estacionarias

Un caso particular interesante de la ley de reflexión y transmisión en una interfaz para
ondas que inciden normalmente es cuando el medio 2 es un conductor perfecto. En este medio,
la impedancia intrínseca tiende a cero
)
iwµ
lím η2 = lím
=0
σ→∞
σ→∞
σ + iwϵ0
Luego, se cumple
r

E =E

i

'

−η1
η1

(

= −E i

Et = 0
'
(
−η1
r
i
= −H i
H =H
η1
Ht = 0

Es decir, la onda es completamente reflejada. Veremos que esta condición da origen a la
creación de una onda estacionaria. El campo eléctrico total queda
⃗ z) = E
⃗ i (t, z) + E
⃗ r (t, z)
E(t,
⃗ z) = E i e−ikz eiwt î − E i eikz eiwt î
E(t,
.
⃗ z) = E i eiwt î e−ikz − eikz
E(t,

Si el medio 1 es un dieléctrico perfecto, entonces k = β (α = 0)
.
⃗ z) = E i eiwt î e−iβz − eiβz = −2i sin(βz)E i eiwt î
E(t,

Tomando la parte real

⃗ z) = 2E i sin(βz) sin(wt)î
E(t,

Esta es una onda que se anula para valores determinados de z (∀t), dados por
z=

wnπ
fn
nπ
=
=
β
c
2λf

n
, n = 0, ±1, ±2, ...
2λ
donde λ es la longitud de onda en el medio 1. Por otra parte, el campo eléctrico se anula
para todo t tal que
z=

---

### Página 554

nπ
, n = 0, ±1, ±2, ...
w
Esta onda es llamada estacionaria puesto que no se propaga, sino que simplemente oscila
en el espacio y el tiempo.
sin wt = 0 → t =

Para el campo magnético se tiene
⃗ z) = H
⃗ i (t, z) + H
⃗ r (t, z)
H(t,
⃗ z) = H i e−iβz eiwt ĵ + H i eiβz eiwt ĵ
H(t,
.
⃗ z) = H i eiwt ĵ e−iβz + eiβz = 2H i eiwt cos(βz)ĵ
H(t,

tomando la parte real

⃗ z) = 2H i cos(βz) cos wtĵ
H(t,
Se anula para
'
(
π
1 π
βz = + nπ → z = n +
2 β
'
(
n 1
z=
+
λ, n = 0, ±1, ±2, ...
2 4
Además, se aprecia que se anula para todo t tal que
cos wt = 0
Se aprecia que para ondas estacionarias, el campo eléctrico y magnético están en un desfase
de π/2

Fig. 16.1: Ondas estacionarias se pueden lograr al confinar ondas electromagnéticas entre dos
planos perfectamente conductores

---

### Página 555

Problema
⃗ 1 = 1,2î + 0,8ĵ + 0,4k̂ (T). Encuentre H
⃗ 2 (H
⃗ en z = +0) y los
En la región 1 de la figura, B
ángulos entre los campos y una tangente a la superficie

#### Solución
Se tiene

⃗ 1 = 1,2î + 0,8ĵ + 0,4k̂
B

la componente normal del campo magnético a una superficie es siempre continua, es decir
⃗ 2 · ẑ
⃗ 1 · ẑ = B
B
se desprende que el campo magnético en z = 0+ es de la forma
⃗ 2 = B2x î + B2y ĵ + 0,4k̂
B
Además, en la regiòn 1 la permeabilidad está dada por
µ1 = µr1 µ0 = 15µ0
⃗ en z = 0− es
de forma que el campo H
⃗1 =
H

"
1 ⃗
1 !
1,2î + 0,8ĵ + 0,4k̂
B1 =
15µ0
15µ0

⃗ es continua al atravesar una superficie sin densidad de
La componente tangencial de H
⃗ en z = 0+ es de la forma
carga superficial. Suponiendo que éste es el caso, el campo H
"
1 !
⃗
H2 =
1,2î + 0,8ĵ + H2z k̂
15µ0
En resumen

Además

⃗ 2 = B2x î + B2y ĵ + 0,4k̂
B
!
"
⃗2 = 1
H
1,2î + 0,8ĵ + H2z k̂
15µ0
⃗2 = 1 B
⃗2
⃗2 = 1 B
H
µ2
µ0

luego
B2x = µ0 H2x =

1,2

---

### Página 556

B2y = µ0 H2y =

0,8

B2z = µ0 H2z = 0,4 → H2z =
Finalmente
⃗2 =
H

0,4
µ0

" 0,4
1 !
1,2î + 0,8ĵ +
k̂
15µ0
µ0

---

### Página 557

Problema
⃗ de 500 Mhz viaja por el espacio libre e incide perpendicularmente sobre un medio
Un campo E
parcialmente conductor como se ilustra en la figura. Si la amplitud del campo incidente es
⃗ i0 = 100 V /m, determine
E
a) Las amplitudes de las ondas una vez atravesado completamente el medio (Et0 , Ht0 )
b) La potencia temporal que porta la onda incidente
c) La potencia temporal que porta la onda transmitida nuevamente al espacio

#### Solución
Definimos el eje ẑ como se indica en la figura, donde el origen coincide con el extremo izquierdo
del medio parcialmente conductor

La onda incidente está descrita por
⃗ i = Ei0 ei(5×108 t−βz) î, z < 0
E
donde la constante de propagación en el vacío está dada por
β=

w
√
= 5 × 108 µ0 ϵ0
c

Al incidir normalmente sobre el medio conductor, parte de la onda se refleja, y otra es
transmitida hacia el medio. Si Em0 es la amplitud de la onda transmitida en la interfaz (z = 0),
entonces se cumple
'
(
2ηm
Em0 = Ei0
η0 + η m

---

### Página 558

donde ηm es la impedancia intrínseca del medio conductor
,
)
iwµ
i5 × 108 µ0
η2 =
=
σ + iwϵ
1 + i5 × 108 55ϵ0
η2 = 44,5594 + i13,2865
El que sea un número complejo implica que existirá un desfase entre la onda incidente y la
onda transmitida al medio. η0 es la impedancia intrínseca del vacío
)
µ0
η0 =
= 120π
ϵ0
Así, para Ei0 = 100
Em0 = 21,3182 + i5,63173i = 22,0495ei0,258274
Con esto, la onda transmitida al medio parcialmente conductor está descrita por
⃗ m (t, z) = Em0 e−αm z ei(wt−βm z) , 0 < z < 30 × 10−3
E
⃗ m (t, z) = 22,0495e−αm z ei(5×108 t−βm z+0,258274) , 0 < z < 30 × 10−3
E
donde la constante de atenuación (αm ) en este medio está dada por
1# #
$
)
! σ "2
2 µϵ
αm = w3
1+
−1
wϵ

Así

1⎛
⎞
⎛,
'
(2
2 µ0 55ϵ0 ⎝
1+
− 1⎠ = 24,26005
αm = 5 × 108 3⎝
5 × 108 55ϵ0

⃗ m (t, z) = 22,0495e−24,26005z ei(5×108 t−βm z+0,258274) , 0 < z < 30 × 10−3
E

La magnitud del campo en z = 30 × 10−3 es
Emt = 22,0495e−24,26005×30×10

−3

= 10,6491

Si Et0 es la amplitud del campo eléctrico transmitido nuevamente al vacío, se cumple
'
(
2η0
Et0 = Emt |
|= 19,0375
η0 + η m

⃗ se relaciona con la del campo eléctrico según
la amplitud del campo H
Et0
= η0
Ht0
Ht0 =

η0
= 0,0504984
Et0

---

### Página 559

b) El promedio temporal del vector Poynting de la onda incidente es
8 9
⃗i = Ei0 k̂ = 13,2629k̂(W/m2 )
S
2cµ0
c) Para la onda transmitida nuevamente al vacío
8 9
⃗t = Et0 k̂ = 0,480681k̂(W/m2 )
S
2cµ0

---

### Página 560

Problema
Se requiere que Ud. haga una estimación de la intensidad de campo eléctrico, en V /m, que
requerirría generar un radar de 2 Ghz de penetración de suelo, con el objeto de detectar piezas
metálicas de gran tamaño, enterradas a una profundidad de hasta 2 metros. Dependiendo de
la composición y la humedad del terreno, este puede tener el siguiente rango de parámetros
10−4 ≤ σ ≤ 10−2
3 ≤ ϵrt ≤ 8
µrt = 1
Por otra parte se estima que las piezas enterradas tienen el siguiente rango de parámetros
107 ≤ σm ≤ 6 × 107
1 ≤ µrm ≤ 7000
ϵrm = 1
Se requiere saber que intensidad de campo eléctrico en V /m se requiere en el aire, sobre
la superficie del terreno, para detectar en el aire sobre la superficie del terreno, un rebote del
objeto metálico que tenga una amplitud de 1V /m, asumiendo incidencia normal
#### Solución
Para estimar la intensidad mínima de campo eléctrico que debe generar el radar, debemos
suponer la peor situación posible. Supondremos que hay una pieza metálica situada a 2 m de
profundidad en la tierra. El caso menos favorable para la propagación en la tierra es cuando ésta
presenta su máxima conductividad (mayor atenuación). Más aún, para que ésta se comporte
como un buen conductor (atenuante) debe tenerse σt >> wϵt , de forma que consideramos el
caso de mayor conductividad y menor constante dieléctrica.
La reflexión en la placa metálica será buena en la medida que ηm (impedancia intrínseca del
metal) sea lo más pequeña posible. De esta forma, el peor de los casos para la reflexión en la
pieza metálica ocurre cuando ηm toma su máximo valor posible, y entonces cuando posee la
menor conductividad y la mayor permeabilidad magnética.

⃗ i (campo emitido por el radar en la
En la figura de arriba se aprecia una onda incidente E
⃗ ti , que se propaga en dirección −z, esta onda
superficie), y una onda transmitida en la tierra E
será reflejada por la pieza metálica en z = 0

---

### Página 561

En esta figura se muestra el campo que se ha reflejado en el metal y se propaga hacia la
⃗ rm , y la onda recibida finalmente en la superficie, llamada E
⃗ t.
superficie, que llamaremos E
Sabemos que esta última tiene una magnitud de Et = 1 (V /m). La magnitud de la onda
reflejada en el metal se describe por
Erm (z) = Er0 e−αz
donde α es el coeficiente de atenuación en la tierra
1⎛
⎛,
⎞
(2
'
σt
2 µt ϵ t ⎝
α = w3⎝
1+
− 1⎠
wϵt

con w = 2 × 109 Hz, σt = 10−2 (S/m), µt = 4π10−7 = µ0 , ϵt = ϵrt ϵ0 = 3 × 8,854 × 10−12 .
Reemplazando estos valores
α = 1,08742
Debido a las condiciones de contorno en la interfaz (z = 2), se cumple
Et = 1 = E |

2η0
|
η0 + ηt

⃗ rm en z = 2, y η0 es la impedancia intrínseca del aire,
donde E es la magnitud del campo E
considerada igual a la del vacío.
)
µ0
η0 =
= 120π
ϵ0
y la impedancia intrínseca de la tierra
)
iwµ0
= 217,434 + i3,2564
ηt =
σt + iwϵ0 ϵrt
con esto se obtiene
E=|

η0 + η t
|= 0,788393V /m
2η0

Además
E = Erm (z = 2) = Er0 e−α2 = Er0 e−1,08742×2
de donde la magnitud de la onda reflejada en el metal en z = 0 es
Er0 = Ee1,08742×2 = 6,93842V /m

---

### Página 562

⃗ ti que fue transmitida a la
Ahora, esta onda reflejada en el metal proviene de la onda E
tierra. La magnitud de esta última se puede expresar como
Eti = E0 eαz
donde E0 (magnitud en z = 0) está relacionada con Er0 mediante
Er0 = E0 |

ηm − ηt
|
η m + ηt

donde la impedancia intrínseca de la pieza de metal es
)
iwµ0 µm
ηm =
σm + iwϵ0 ϵm
con w = 2 × 109 Hz, σm = 107 (S/m), µm = 700, ϵm = 1 resulta
ηm = 2,35095 + i2,35095
Notar que es un complejo con fase π/4, que es lo que se obtiene para un buen conductor.
Con todo esto
E0 = Er0 |

ηm + η t
|= 7,09235
ηm − ηt

Justo en z = 2, la magnitud de la onda transmitida a la tierra es
Eti (2) = E0 eαz = 7,09235e1,08742×2 = 62,4177V /m
Si Ei es la magnitud de la onda que emite el radar en la superficie, entonces se cumple
Eti (2) = Ei |

2ηt
|
ηt + η0

Ei = 62,4177 |

ηt + η 0
|
2ηt

Ei = 85,3109
Es decir, se requiere emitir un campo de magnitud aproximadamente Ei = 85, 3 (V /m)

---

### Página 563

16.2.

Reflexión y Refracción en la frontera de dos medios
dieléctricos. Incidencia Oblicua

Un caso más general que el discutido en la sección de incidencia normal es el de la reflexión
y refracción de una onda plana que incide oblicuamente por el plano de una zona interfacial de
un dieléctrico. La situación está descrita por la siguiente figura

El sistema de coordenadas que utilizaremos se ilustra en la figura. Los medios sobre y bajo
el plano z = 0 están caracterizados por permitividades y permeabilidades {ϵ1 , µ1 } y {ϵ2 , µ2 }
respectivamente. Una onda plana con vector de onda ⃗ki y frecuencia w incide desde el medio
1. La onda refractada y reflejada tienen vectores de onda ⃗kt y ⃗kr , respectivamente, y ûn es
un vector unitario normal dirigo desde el medio 1 al medio 2. (En el dibujo, concide con la
dirección z). La onda incidente está descrita por
⃗ i (t, ⃗x) = E
⃗ 0 ei(wt−⃗ki ·⃗x)
E
#
$
⃗ki × E
⃗i
⃗ i (t, ⃗x) =
H
η1
β1
donde ⃗ki es la dirección de propagación de la onda incidente, cuya magnitud es ki = β1 =
√
w
⃗ 0 debe tener una dirección perpendicular a ⃗ki (las ondas electro= µ1 ϵ1 w. Además E
c1
magnéticas son transversales). Para la onda refractada

con kt = β2 = cw2 =

√

⃗ t (t, ⃗x) = E
⃗ t ei(wt−⃗kt ·⃗x)
E
#
$
⃗kt × E
⃗t
⃗ t (t, ⃗x) =
H
η2
β2
ϵ2 µ2 w. Por último, la onda reflejada está descrita por
⃗ r (t, ⃗x) = E
⃗ 0 ei(wt−⃗kr ·⃗x)
E
#
$
⃗kr × E
⃗r
⃗ r (t, ⃗x) =
H
η1
β1

notar que la magnitud del vector de onda reflejada es igual al de la incidente, kr = β1 .
La existencia de condiciones de borde en la interfaz z = 0, que se deben satisfacer para
todos los puntos en el plano en todo instante, implica que la variación espacial (y temporal) de

---

### Página 564

los campos debe ser la misma en z = 0. De esta forma, las ondas reflejadas y refractadas deben
tener la misma frecuencia w que la incidente si las condiciones en la frontera se satisfacen para
todo t. Además, debe tenerse que las 3 ondas deben tener la misma fase en z = 0
!
":
!
":
!
":
:
:
⃗ki · ⃗x ::
⃗
⃗
= kt · ⃗x :
= kr · ⃗x :
z=0

z=0

z=0

De aquí se aprecia que los tres vectores de onda deben permanecer en un plano, llamado
plano de incidencia. En la figura, corresponde al plano x − z. Esta condición se puede
reescribir en términos de los ángulos de incidencia ϑi , de reflexión ϑr y de refracción ϑt . Notar
que ningún vector de onda tiene componente según j, luego
:
!
"
⃗ki · ⃗x = (kix x + kiz z) ::
= kix x = ki sin ϑi x
z=0

análogo para el resto, así

ki sin ϑi x = kr sin ϑr x = kt sin ϑt x
ki sin ϑi = kr sin ϑr = kt sin ϑt
Como ki = kr , se obtiene que el ángulo de incidencia es igual al ángulo de reflexión
sin ϑi = sin ϑr
Además, se obtiene la ley de Snell
ki sin ϑi = kt sin ϑt
)
sin ϑi
ϵ 2 µ2
kt
=
=
sin ϑt
ki
ϵ 1 µ1
)
sin ϑi
ϵ 2 µ2
c1
=
=
sin ϑt
ϵ 1 µ1
c2

16.2.1.

Polarización paralela y perpendicular
ϑi , ϑr , ϑt
⃗ki , ⃗kr , ⃗kt
⃗ i, H
⃗ i, E
⃗ r, H
⃗ r, E
⃗ t, H
⃗t
E
