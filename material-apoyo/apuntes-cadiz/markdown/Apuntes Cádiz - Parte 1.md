---
title: "Parte 1"
source_pdf: "Electro/material-apoyo/apuntes-cadiz/Apuntes Cádiz - Parte 1.pdf"
pages: 136
pdf_kind: "PDF (texto)"
extraction_mode: "pdftotext_cleaned"
---
# Parte 1

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
~·B
~ = Ax Bx + Ay By + Az Bz
A
~×B
~ = (Ay Bz − Az By ) î + (Az Bx − Ax Bz ) ĵ + (Ax By − Ay Bz ) k̂
A
~×A
~=0
A


~· A
~×B
~ =0
A


 

~
~
~
~
~
~
A· B×C = A×B ·C


 



~× B
~ ×C
~ = A
~·C
~ B
~− A
~·B
~ C
~
A

1.2.

Cálculo diferencial en R3

Sea f : [R3 ] → R una función real. También es llamada campo escalar, pues a cada punto
del espacio (R3 ) le asocia un número real (un escalar). Ejemplo de un campo escalar puede ser
la temperatura en cierta región del espacio T : [Ω ⊆ R3 → R]

Fig. 1.1: T (x, y, z) representa un campo escalar sobre Ω
Además de la existencia de campos escalares, también existen campos vectoriales. La
idea es bien simple, a cada punto del espacio se le asocia un vector. En R3 , el tipo de campos
vectoriales que nos interesarán son de la forma F~ : [Ω ⊆ R3 ] → R3 .

---

### Página 6

Fig. 1.2: La velocidad de los átomos de un objeto que rota es un ejemplo de campo vectorial

1.2.1.

Derivadas de un campo escalar

Si f es un campo escalar diferenciable (y por lo tanto una función continua) sobre un
dominio D ⊆ R3 , entonces está definido el Gradiente de f


∂f (x, y, z) ∂f (x, y, z) ∂f (x, y, z)
~
+
+
∇f (x, y, z) =
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
∂f 0
∂f 0
∂f 0
x (t) +
y (t) +
z (t) = 0
∂x
∂y
∂z


∂f (x, y, z) ∂f (x, y, z) ∂f (x, y, z)
+
+
∂x
∂y
∂y



· (x0 (t), y 0 (t), z 0 (t)) = 0

y entonces el gradiente es perpendicular a la dirección tangente a la curva. Más aún, si û es
un vector unitario, se define la derivada direccional de f en la dirección û como
~ (x, y, z) · û
Dû f (x, y, z) = ∇f
Se puede demostrar que la derivada direccional se maximiza en la dirección del gradiente,
es decir, el gradiente entrega la dirección de máxima variación de f .

---

### Página 7

1.3.

~ como un operador
∇

Conviene considerar al gradiente como algo independiende de que función se está derivando.
~ al operador
Llamamos ∇


∂
∂
∂
~ =
∇
, ,
∂x ∂y ∂z
~ debe operar
Por supuesto que este operador así escrito no significa nada. El operador ∇
sobre una función, por ejemplo


∂f ∂f ∂f
~
,
,
∇f =
∂x ∂y ∂z

Tiene completo sentido en este caso. Hemos ”multiplicado” al operador por una cantidad
escalar. Hay que tener ciertas precauciones con este tipo de notación, por ejemplo, del álgebra
de vectores es sabido que si α es un escalar
~ = Aα
~
αA
~ no tiene sentido por si mismo, en efecto, es un nuevo operador
sin embargo, f ∇


∂
∂
∂
~
f∇ = f , f , f
∂x ∂y ∂z

1.3.1.

Divergencia y Rotor

Si F~ es un campo vectorial, entonces
~ · F~
∇
~ como un
debe ser un escalar, y por lo tanto puede tener un sentido físico. Entendiendo ∇
operador vectorial, se tiene


∂ ∂ ∂
~
~
∇·F =
, ,
· (Fx , Fy , Fz )
∂x ∂y ∂z
~ · F~ = ∂ Fx + ∂ Fy + ∂ Fz
∇
∂x
∂y
∂z
A esta cantidad escalar asociada a un campo vectorial se le llama divergencia de F~ .
~ × F~ ?.
Veamos que más es posible definir a partir del operador gradiente. ¿Qué ocurre con ∇
Por supuesto que el resultado debe ser un campo vectorial, de hecho, muy útil en el análisis de
funciones vectoriales. Desarrollando este producto cruz según el álgebra de vectores


~ × F~
∇





~ × F~
∇





~ × F~
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


=

---

### Página 8

~ → Vector
∇f
~ · F~ → Escalar
∇

~ × F~ → Vector
∇

---

### Página 9

1.3.2.

Segundas derivadas

Hasta ahora hemos definido cantidades que involucran únicamente primeras derivadas.
Veamos que ocurre con las siguientes combinaciones
 
~ · ∇f
~
(a)∇
 
~ × ∇f
~
(b)∇


~ ∇
~ · F~
(c)∇


~ · ∇
~ × F~
(d)∇



~
~
~
(e)∇ × ∇ × F
Veamos la primera de ellas, es claro que debe obtenerse un campo escalar. Desarrollando


 
∂f ∂f ∂f
~
~
~
∇ · ∇f = ∇ ·
,
,
∂x ∂y ∂z
  ∂2f
∂2f
∂2f
~
~ · ∇f
=
∇
+
+
∂x2
∂y 2
∂z 2
Se ve que esto se puede reescribir como
 


~
~
~
~
~
~
~ 2f
∇ · ∇f = ∇ · ∇f = ∇ · ∇ f = ∇

~ 2 como un nuevo operador, y como aparece mucho en física, tiene un nombre. Es
Vemos a ∇
llamado Laplaciano
∂2
∂2
∂2
+
+
∂x2 ∂y 2 ∂z 2
debido a que el Laplaciano es un operador escalar, podría aplicarse sobre un vector
~2=
Laplaciano → ∇

~ 2 F~
∇
por supuesto esto significa que el operador Laplaciano opera sobre cada componente de F~


~ 2 Fy , ∇
~ 2 Fz
~ 2 Fx , ∇
~ 2 F~ = ∇
∇
Veamos que ocurre con la expresión (b). Notemos que tiene la siguiente forma

  
~×A
~ f =0
~
~ × Af
= A
A
Esperamos que

 
~
~ × ∇f
∇

sea cero para cualquier campo escalar f . Podemos verificarlo tomando alguna de las componentes

---

### Página 10

 
 
~
~
~
~
~
~
[∇ × ∇f ]x = ∇z ∇f − ∇y ∇f
y

~ × ∇f
~ ]x =
[∇

∂
∂z



∂f
∂y



−

∂
∂y



∂f
∂z

Del mismo modo se muestra para las demás componentes



z

=0

La expresión (c) es por supuesto un campo vectorial


~ ∇
~ · F~
∇

Sin embargo, no hay nada muy especial que decir acerca de él. Es simplemente un campo
vectorial que podría aparecer en el futuro
La expresión (d) tiene la forma

Es decir, esperamos que



~· A
~×B
~ =0
A


~ · ∇
~ × F~ = 0
∇

Para cualquier campo vectorial F~ . Es así, y es fácil de verificar
Por último, veamos que sucede con la expresión (e)


~ × F~
~ × ∇
∇

Ésta tiene la forma de


 



~
~
~
~
~
~
~
~
~
A× B×C =B A·C − A·B C

Podríamos seguir utilizando esta expresión y escribir



 

~
~
~
~
~
~
~
~
∇ × ∇ × F = ∇ ∇ · F − ∇ · ∇ F~
El último término es el Laplaciano




~
~
~
~
~
~
~ 2 F~
∇× ∇×F =∇ ∇·F −∇

En resumen, hemos encontrado
 
~
~
~ 2 f → Laplaciano sobre f, campo escalar
∇ · ∇f
=∇

 
~
~
∇ × ∇f
=0


~ · F~ → Campo vectorial
~ ∇
∇


~ · ∇
~ × F~ = 0
∇




~ × F~ = ∇
~ · F~ − ∇
~ × ∇
~ ∇
~ 2 F~ → campo vectorial
∇

---

### Página 11

1.3.3.

Dos teoremas adicionales

En muchos problemas físicos, sucede que un determinado campo vectorial F~ tiene rotor
nulo. Es decir
~ × F~ = 0
∇

Hemos visto que el rotor de un gradiente es siempre cero. Podría ser ciento entonces, que
F~ fuera el gradiente de algún campo escalar, de esta forma su rotor sería siempre nulo. Lo
interesante es que esto es siempre así, y enunciaremos el siguente teorema
Si
Existe un campo escalar ψ, tal que

~ × F~ = 0
∇
~
F~ = ∇ψ

Del mismo modo, hemos visto que la divergencia de un rotor es siempre cero. Luego, si la
divergencia de un campo vectorial F~ es nula, podria tenerse que F~ fuera el rotor de un campo
vectorial. De ser así, estaría garantizado que su divergencia sea nula. En efecto, enunciamos el
segundo teorema
Si
~ tal que
Existe un campo vectorial A,

~ · F~ = 0
∇
~ ×A
~
F~ = ∇

1.4.

Cálculo Integral en R3

1.4.1.

Integral de línea de un campo vectorial

Sea F~ : [Ω ⊆ R3 ] → R3
Consideremos una curva Γ contenida en Ω. Sea ~x0 , ~x1 , ...~xn una partición de Γ, (xk , yk ) un
punto en el trazo de Γ que va de ~xk−1 a ~xk , y ∆~xk = ~xk − ~xk−1 . Se define la integral de línea
de F~ (~x) por
ˆ
d~x · F~ (~x) = lím F~ (xk , yk ) · ∆~xk
n→∞

Γ

Esto se puede reescribir como
ˆ
ˆ
∆~xk
~
~
d~x · F (~x) = lím F (xk , yk ) ·
| ∆~xk |= dsT̂ (~x) · F~ (~x)
n→∞
| ∆~xk |
Γ
Γ
donde T̂ (~x) es la tangente unitaria a la curva Γ en ~x. Así
ˆ
ˆ
~
d~x · F (~x) = dsT̂ (~x) · F~ (~x)
Γ

Γ

La integral de línea de un campo vectorial sobre una curva Γ corresponde a sumar las
proyeccciones de F~ (~x) en la dirección tangente a la curva en todo punto.

---

### Página 12

1.4.2.

Integral de superficie de un campo vectorial

Sea F~ : [Ω ⊆ R3 ] → R3 y S una superficie contenida en Ω. Se define la integral de flujo del
campo F~ sobre S como
¨
¨
~ x) · F~ (~x) =
dS(~
dS(~x)n̂(~x) · F~ (~x)
S

S

corresponde a sumar la proyección del campo F~ sobre la normal a la superficie S en cada
punto.

1.4.3.

Teorema de la Divergencia

Sea Ω ⊆ R3 una región. Sea F~ un campo vectorial continuo y diferenciable en Ω. Entonces
ˆˆ
˚
 ~
3 ~
~
x) · F~ (~x)
d x∇ · F =   dS(~
δΩ

Ω

1.4.4.

Teorema de Stokes

Sea S una superficie en R3 . Sea F~ un campo vectorial continuo y diferenciable en una región
que contiene a S. Entonces
¨

 ˛
~
~
~
dS(~x) · ∇ × F (~x) =
d~x · F~ (~x)
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
~ y magnético B.
~
mediante la introducción del campo eléctrico E

A Dynamical Theory of the Electromagnetic Field, James Clerk Maxwell

---

### Página 14

Primeramente estudiaremos el caso estático, en donde los campos no tienen dependencia
temporal. En este caso las ecuaciones de Maxwell se transforman en:
~ ·E
~ = ρ
∇
o
~ ×E
~ =0
∇

~ ·B
~ =0
∇
~ ×B
~ = µo J~
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
La fuerza que ejerce q 0 sobre q está dada por la ley de Coulomb
F~q =

qq 0
(~x − ~x0 )
4π0 | ~x − ~x0 |3

---

### Página 16

Es decir, la fuerza electrostática es proporcional al producto de las cargas e inversamente
proporcional al cuadrado de la distancia entre ellas. Notar que la dirección
(~x − ~x0 )
| ~x − ~x0 |
va siempre desde la carga q 0 hacia la carga q. El signo de la fuerza estará determinado entonces
por el producto de las cargas, así, si ambas son iguales, la fuerza será repulsiva, mientras que
si son de signo opuesto, la fuerza será atractiva.
En el sistema S.I., la constante de proporcionalidad está dada por
= 8, 9875 × 109 N m2 /C 2
4πo
Donde 0 se conoce como la permitividad del vacío.
K=

Similarmente, la fuerza sobre q 0 debido a q está dada por F~q0 = −F~q , como debe ser por la
tercera ley de Newton. La ley de Coulomb describe perfectamente las fuerzas entre 2 cargas
puntuales, luego, resulta de interés estudiar qué sucede cuando hay más de dos cargas presentes.
Supongamos que existen N cargas qj con j = 1, 2, ...N . Supongamos que hay una carga q en
la posición ~x y que la posición de la carga qj es ~xj . La fuerza que ejercen las N cargas sobre q
está dada por el principio de superposición
F~q =

N
X
qqj
(~x − ~xj )
4π
|
~
x
−
~
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
~ se define formalmente como
El campo eléctrico E
~
~ = lím Fq0
E
q0 →0 q0
Es decir, el campo existe en todo el espacio y es independiente de la carga de prueba. La
sutileza de elegir una carga de prueba infinitamente pequeña es para que el campo producido
por q0 no altere de ninguna forma a la fuente del campo que queremos cuantificar.

Diremos entonces con este nuevo enfoque que la carga q es una fuente (crea) un campo
~ que ejerce una fuerza F~q0 = q0 E(~
~ x) sobre una carga q0 ubicada en ~x
eléctrico E
Usando la definición de Campo Eléctrico y la Ley de Coulomb, se obtiene que el campo eléctrico
a una distancia r de la carga puntual q está dado por
1 q
r̂
4π0 r2
donde r̂ es la dirección radial desde la carga q
~ =
E

~ para una carga positiva(izq) y negativa
Fig. 3.3: Representación gráfica del campo vectorial E
(der)

---

### Página 18

Lógicamente, el principio de superposición es también válido para el campo eléctrico, bajo
las mismas condiciones mencionadas anteriormente. Así, el campo en ~x de una distribución
discreta de N cargas puntuales ubicadas en qj ,j = 1, 2, ...N está dado por
~ x) =
E(~

N
X
qj
(~x − ~xj )
4π0 | ~x − ~xj |3
j=1

(3.1)

La ley de Coulomb y el principio de superposición son las leyes empíricas fundamentales
de la Electrostática. Más adelante, veremos que las ecuaciones de Maxwell para el campo
Electrostático
~ · E(~
~ x) = ρ
∇
0
~ × E(~
~ x) = 0
∇
contienen exactamente la misma información que acabamos de presentar (y por supuesto, contienen muchísima información adicional!), pero de una forma mucho más general, simple y
elegante.

3.2.

Distribuciones continuas de carga - Integrales de
Coulomb

Se pueden extender estas ideas para cuando se tiene una gran cantidad de cargas distribuídas
en una región del espacio. Supongamos una distribución continua de carga encerrada en un
volumen V , por ésto entendemos una región del espacio en donde se puede definir una densidad
volumétrica de carga en cada punto, digamos ρ(~x) (C / m3 )

En el caso de obtener una distribución continua de carga, se utiliza una partición del volumen
V en celdas de volumen infinitesimal d3 x0 . En la posición ~x0 , se encuentra un pequeño volumen
con carga dada por
dq(~x0 ) = d3 x0 ρ(~x0 )
Como esta es una carga infinitesimal, el campo que genera en ~x será el de una carga puntual
~ x0 ) =
dE(~

d3 x0 ρ(~x0 ) ~x − ~x0
4πε0 | ~x − ~x0 |3

---

### Página 19

Para obtener el campo generado por toda la distribución de carga, basta con sumar (integrar)
sobre el volumen V las contribuciones individuales de cada elemento de volumen, luego
~ x) = 1
E(~
4π0

d3 x0 ρ(~x0 )
(~x − ~x0 )
0 |3
|
~
x
−
~
x
V

˚

En el caso de obtener una superficie S de carga, en donde para cada ~x0 en S se tiene
una densidad superficial de carga (que denotaremos σ(~x0 ) para diferenciarla de una densidad
volumétrica), se obtiene
¨
ds0 σ(~x0 )
~
E(~x) =
(~x − ~x0 )
4π0 S | ~x − ~x0 |3
Por último, para una distribución lineal Γ, en donde para cada ~x0 en Γ se tiene una densidad
lineal de carga, denotada λ(~x0 ) entonces el campo en ~x está dado por
ˆ
dx0 λ(~x0 )
~
E(~x) =
(~x − ~x0 )
4π0 Γ | ~x − ~x |
Éstas son las integrales de Coulomb y son una extensión al caso de una distribución discreta
de cargas, a distribuciones continuas en el espacio
Ejemplo: Campo de un anillo de carga
Consideremos un anillo con densidad lineal de carga constante y dada por λ. El objetivo es
calcular el campo eléctrico generado por esta distribución de carga en un punto sobre el eje de
simetría a distancia z del origen

Un elemento diferencial de longitud sobre el anillo está dado por dl = Rdφ donde φ es el
ángulo polar. Este elemento posee una carga dq = λdl = λRdφ, de forma que el campo eléctrico
en un punto ~x debido a esta carga infinitesimal está dado por la ley de Coulomb
~ x) = dq ~x − ~x = dφRλ ~x − ~x
E(~
4π0 | ~x − ~x0 |3
4π0 | ~x − ~x0 |3

donde ~x0 es la posición del elemento de carga, en este caso


~x0 = Rr̂ = R cos φî + sin φj

---

### Página 20

de forma que el campo total se obtiene integrando sobre todo el anillo (abarcando todo el
rango de φ)
~ x) = R
E(~
4π0

ˆ 2π

dφ

~x − Rr̂
| ~x − Rr̂ |3

ahora, se desea el campo en un punto sobre el eje simetría del anillo, a distancia z del origen,
de forma que
~x = z k̂
y queda
~ k̂) = R
E(z
4π0

ˆ 2π

dφ

por supuesto que

z k̂ − Rr̂

| z k̂ − Rr̂ |3

| z k̂ − Rr̂ |= z 2 + R2
~ k̂) = R
E(z
4π0

ˆ 2π

1/2

z k̂ − R cos φî − R sin φĵ

dφ

(z 2 + R2 )3/2

De estas tres integrales (en î, ĵ, k̂), la única que no es nula es la según k̂. Esto es fácil de
ver apelando a la simetría de la distribución de carga

~ k̂) = Rz
E(z
4π0

ˆ 2π

dφ

(z 2 + R2 )3/2

k̂

z
~ k̂) = 2πR
E(z
k̂
4π0 (z 2 + R2 )3/2
esto se puede escribir de otra forma considerando que Q = 2πRλ es la carga total del anillo
z
~ k̂) = Q
k̂
E(z
4π0 (z 2 + R2 )3/2

---

### Página 21

Si z es suficientemente grande en comparación con las dimensiones del anillo (z >> R),
entonces
~ k̂) ≈ Q k̂
E(z
4π0 z 2
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

p
4πε0 T sin ϑ

---

### Página 23

Del equilibrio de fuerzas para el eje vertical obtenemos
T =

mg
cosθ

Y además, r = 2l sin ϑ. Finalmente se obtiene
qeq = ±2lsinϑ

p
p
4πε0 mgtgϑ = ±4lsinϑ π0 mgtanϑ

---

### Página 24

Problema
Se tiene una línea homogénea de carga con densidad lineal λ, y de longitud finita a. Calcular
el campo eléctrico en el punto P a distancia x del extremo

#### Solución
Tomamos un pequeño elemento dµ de la línea de carga, situado a una distancia µ del punto A,
y obtenemos el campo eléctrico en el punto P debido a este elemento diferencial
~ )=
dE(P

λdµ
î
4π0 (a + x − µ)2

Y el campo eléctrico total se obtiene integrando para toda la línea de carga. Esto es

~ )=
E(P

4π0

ˆ a

λdµ
î
(a + x − µ)2

Sea z = a + x − µ, así, dz = −dµ y el campo queda
~ = −λ
E
4π0

ˆ x

dz
λ 1 x
î
=
î =
4π0 z a+x
a+x z



λ
λ
−
4π0 x 4π0 (a + x)

λa
Q
~ = λ(x + a) − λx î =
î =
î
E
4π0 x(x + a)
4π0 x(x + a)
4π0 x(x + a)
Con Q la carga total de la línea.
Notar que si x
a

~ ≈
E

Q
î
4πε0 x2

que concuerda con el campo de una carga puntual



î

---

### Página 25

Problema
Una barra delgada con densidad de carga uniforme λ se dobla con la forma de un arco de
círculo de radio R. El arco subiende un ángulo total 2ϑ0 , simétrico con respecto al eje x, como
~ en el origen O?. Vea que sucede cuando
se muestra en la figura. ¿Cuál es el campo eléctrico E
ϑ0 → π

#### Solución
Considere un elemento diferencial de longitud dl = Rdϑ, que forma un ángulo ϑ con respecto
al eje x. La cantidad de carga que contiene este elemento es dq = λdl = λRdθ

Su contribución al campo eléctrico en O es
~ =−
dE

1 dq
1 dq
1 λdϑ
(− cos ϑî − sin ϑĵ)
r̂ =
(− cos ϑî − sin ϑĵ) =
4π0 r
4π0 R
4π0 R

Integrando para ϑ entre −ϑ0 y ϑ0 , se obtiene
ˆ
1 λ ϑ0
~
dϑ(− cos ϑî − sin ϑĵ)
E=
4π0 R −ϑ0

~ =
E

ϑ0
1 λ
1 2λ sin ϑ0
(− sin ϑî + cos ϑĵ)
î
=−
4π0 R
4π0
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
~ ≈ − 1 2λθ0 î = − 1 2λϑ0 R î = − 1 Q î
E
4π0 R
4π0 R2
4π0 R2
Donde la carga total del arco es Q = λl = λ(2Rϑ0 )

---

### Página 27

Problema
Un recipiente hemisférico no conductor de radio interior a tiene una carga total Q repartida
uniformemente en su superficie interior. Encuentre el campo eléctrico en el centro de curvatura

#### Solución
Tomamos como origen el centro de curvatura de la semiesfera. A partir de esto podemos determinar la contribución de un elemento diferencial de carga en la superficie al campo eléctrico
~ por
en el eje que pasa por el centro de curvatura, que coincide con la direccion k̂ (El campo E,
simetría, solo tendrá componente en k̂).

~ x) =
dE(~

1 (~x − ~x0 )
σds0
4π0 |~x − ~x0 |3

Un elemento diferencial de superficie sobre la esfera está dado por
ds = a2 sin ϑdϑdφ
y como la carga está distribuída uniformemente, la densidad superficial es simplemente
σ=

Q
2πa2

Con esto, podemos determinar el campo total integrando sobre toda la superficie
ˆ π
ˆ
Q (~x − ~x0 )
1 2 2π
~
a
dφ
dϑ sin ϑ
E(~x) =
4π0
2πa2 |~x − ~x0 |3
π/2
Evaluando en ~x= 0 obtenemos el campo en el centro de curvatura
ˆ 2π ˆ π
Q
−~x0 2
~
E(0) =
a sin ϑdθdφ
4π0 0
x0 |3
π/2 2πa | − ~

~
E(0)
=

4π0

ˆ 2π

Q
2πa2

ˆ π

−~x0 2
a sin ϑdθdφ
x0 |3
π/2 | − ~

El vector ~x0 que recorre la superficie está dado por
~x0 = a cos ϑk̂ + a sin ϑ cos φî + a sin ϑ sin φĵ

---

### Página 28

Por el argumento de simetría, solo interesa la componente según k̂. De todas formas se
puede verificar calculando explícitamente las integrales en î y ĵ . Con esto
ˆ π
Q
−a cos ϑ 2
~
E(0) =
a sin ϑdϑk̂
40 πa π/2
a3
ˆ π
ˆ π
Q
Q
~
− cos ϑ sin ϑdϑk̂ =
− sin(2ϑ)dϑk̂
E(0) =
40 πa2 π/2
80 πa2 π/2
Finalmente el campo en el centro de curvatura es
~
E(0)
=

Q
k̂
80 πa2

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

Un elemento de longitud dx0 a distancia x0 del origen genera una contribución al campo en
P dada por
~ ) = dx λ ~x − ~x
dE(P
4πε0 | ~x − ~x0 |3
donde ~x = Rĵ es el vector posición del punto P , y ~x0 = x0 î el vector que recorre la distribución
de carga (parámetro x0 ). Por el principio de superposición, el campo eléctrico en P se obtiene
sumando sobre toda la distribución
~ )=
E(P

λ
4πε0

ˆ ∞

dx0

Rĵ − x0 î

(x02 + R2 )3/2
ˆ ∞
ˆ ∞
λ
Rλ
x0
dx0
~
dx
E(P ) = −
î
+
ĵ
4πε0 0
4πε0 0 (x02 + R2 )3/2
(x02 + R2 )3/2

Calculemos primero la integral
I1 =

ˆ ∞

dx0 x0
(x02 + R2 )3/2

con el trivial cambio de variable u = x02 , du = 2x0 dx0

---

### Página 30

I1 =

ˆ ∞

=
3/2
(u + R2 )
du

ˆ ∞

∞
du(u + R2 )−3/2 = −2 ∗ (u + R2 )−1/2

I1 =
Ahora, obtenemos
I2 =

ˆ ∞

R

dx0
(x02 + R2 )3/2

y utilizamos la conocida sustitución x0 = R tan ϑ, dx0 = Rsec2 ϑdϑ. Con esto la integral
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

Utilizando que x0 /R = tan ϑ
sin ϑ = √

x0
x02 + R2

de forma que
I2 =

∞
x0
x0
√
√
=
lím
R2 x02 + R2 0
R2 x0 →∞ x02 + R2

I2 =

q
lím
= 2
R x →∞
R
12 + (R/x0 )2

Luego el campo eléctrico debido al alambre en el punto P es
~ 1 (P ) =
E

4πε0



λ
−λ
î + ĵ
R
R



√ 

λ
~ 1 (P ) =
√ (−î + ĵ)
E
4πε0 R

La contribución del sector de arco de círculo ya fue obtenida en un problema anterior, uego
es inmediato que
~ 2 (P ) =
E

2λ
sin
4πε0 R



3π



î

---

### Página 31

Finalmente, el campo total en P se obtiene por superposición. Veamos que ocurre con el
campo que produce el segmento rectilíneo superior

~ 1 en P forma un ángulo de 3π/8 con la horizontal. De esta forma, la superposición
El campo E
de los 3 campos es como sigue

~ )=
E(P

~ )= 1
E(P
4πε0

~ )=
E(P





~ 1 | cos
~ 2 | −2 | E
|E



3π









sin

3π

3π



λ√
2 cos
−2
R

2λ
sin
R

λ
2πε0 R



−

√

2 cos



î



3π

3π





î

î

---

### Página 32

Problema
Se pide calcular el campo eléctrico a distancia r del centro de una distribución uniforme de
carga ρ0 localizada dentro de una esfera de radio R, mediante la integral de Coulomb, o sea,
calcule
˚
~x − ~x0
ρ
~ x) =
E(~
d3 x0
4πε0
| ~x − ~x0 |3
V
puesto que

ρ0 si | ~x0 |≤ R
ρ(~x ) =
0 si | ~x0 |> R
para r > R

#### Solución
Ubiquemos el centro de la esfera en el origen

Sea ~x un punto a distancia r del origen
~x = rr̂
y ~x0 un punto dentro de la distribución de carga
~r0 = r0 r̂0
El campo eléctrico está dado por la integral de Coulomb sobre la distribución de carga
˚
˚
x − ~x0
~x − ~x0
ρ0
3 0
3 0 ~
~
E(~x) =
d x ρ(~x )
=
d
x
4πε0
| ~x − ~x0 |3
4πε0
| ~x − ~x0 |3
V
V

~ x) = ρ0
E(~
4πε0

ˆ 2π

dφ

ˆ π

dϑ sin ϑ

ˆ R

dr0 r02

r̂r − r̂0 r
| r̂r − r̂0 r0 |3

De la simetría de la distribución de carga, es claro que el campo eléctrico será sólo función
de la distancia r y su dirección será radial, es decir
~ x) = E(r)r̂
E(~
esto nos permite además orientar el vector ~x según la dirección k̂, de forma que
| r̂r − r̂0 r0 |= r2 + r02 − 2rr0 cos ϑ0
~ x) = ρ0
E(~
4πε0

ˆ 2π

dφ

ˆ π

dϑ sin ϑ

ˆ R

dr0 r02

1/2

r̂r − r̂0 r

(r2 + r02 − 2rr0 cos ϑ0 )3/2

= E(r)r̂

---

### Página 33

~ = 2πρ0
E(r) = r̂ · E
4πε0

ˆ π

dϑ sin ϑ

ˆ R

dr0 r02

r − r0 cos ϑ0

(r2 + r02 − 2rr0 cos ϑ0 )3/2

Hasta ahora, esta expresión es absolutamente general. Sin embargo, el valor de la integral
dependerá si el punto ~x se encuentra dentro o fuera de la distribución
Campo externo, r > R

se tiene
r = r0 cos ϑ0 + | ~x − ~x0 | cos α

Sea s =| ~x − ~x0 |, luego

r − r0 cos ϑ0

0 3/2

(r2 + r02 − 2rr0 cos ϑ )

=

s cos α
cos α
=
s3
s2

de la relación

se puede obtener para cos ϑ0

r2 + r02 − 2rr0 cos ϑ0 = s2
cos ϑ0 =

r2 + r02 − s2
2rr0

y utilizando el teorema del coseno para r0
r2 + s2 − 2rs cos α = r02
de aquí obtenemos que
cos α =

Por último

r2 + s2 − r02
2rs

∂
s
2s
dϑ0
=
−
cos ϑ0 = − sin ϑ0
=−
∂s
ds
2rr0
rr0

---

### Página 34

Luego

ˆ R

dr

=

ˆ R

ˆ π

dϑ0 sin ϑ0 r02

r − r0 cos ϑ0

(r2 + r02 − 2rr0 cos ϑ0 )3/2

ˆ r+r0

s
r2 + s2 − r02
ds 0 r02
dr
=
rr
2rs3
r−r 0

ˆ R

ˆ r+r0



= 2
2r

ˆ R

ˆ r+r0

r0
ds 2
dr
2r
r−r0

r2 − r02
dr r
ds 1 +
s2
r−r0
0 0



r2 − r02
1+
s2





y
ˆ r+r0

r2 − r02
ds 1 +
s2
r−r0




=

ˆ r+r0
r−r 0

ds + (r − r )

r2 − r02
= (r + r ) − (r − r ) +
−2 + 1

= 2r0 − (r2 − r02 )
Así
2r2

ˆ R

ˆ r+r0



de forma que
2πρ0
E(r) =
4πε0

ˆ π

dϑ sin ϑ

ˆ R



ˆ r+r0
r−r0

−
r + r0 r − r0

ds
s2



(r − r0 ) − (r + r0 )
= 4r0
r2 − r02

r2 − r02
dr r
ds 1 +
s2
r−r0
0 0

dr0 r02



= 2
r

ˆ R

dr0 r02 =

2R3
3r2

r − r0 cos ϑ0

ρR3
=
3ε0 r2
(r2 + r02 − 2rr0 cos ϑ0 )3/2

Así, para r > R

~ x) = ρR r̂
E(~
3ε0 r2
si Q = 43 πR3 ρ0 es la carga total de la esfera, entonces
~ x) =
E(~

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
δ(x) = 0, x 6= 0
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


x < −1/n
0
δn (x) = n/2 −1/n < x < 1/n


x > 1/n

Fig. 3.4: Primeras 3 funciones dadas por la sucesión δn (x)
Notar que a medida que aumenta n, la función se asemeja a un rectángulo cada vez más
angosto en torno al origen y de mayor amplitud. Sin embargo, siempre el área bajo δn (x) es
uno. Físicamente usaremos la delta de Dirac para modelar distribuciones de carga que son nulas
excepto en un punto del espacio
Veamos que en efecto δn (x) define una sucesión de funciones de cuadrado integrable
ˆ ∞
ˆ 1/n
 n 2  n  2  2  n
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

δ(x) = 0, x 6= 0

Del mismo modo, podemos interpretar δ(x − xo ) en base a
ˆ ∞
dxδ(x − x0 ) = 1
−∞

ˆ ∞

−∞

dxδ(x − x0 )f (x) = f (xo )

δ(x − x0 ) = 0, x 6= x0

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

dxδ 0 (x)f (x) = −f 0 (0)

δ(x − x0 ) = 0, x 6= x
ˆ b
a

dx0 δ(x − x0 ) = 1, a < x < b
δ(x − x0 ) = δ(x0 − x)

ˆ ∞

−∞

ˆ ∞

−∞

dx0 δ(x − x0 )f (x0 ) = f (x)

dx00 δ(x00 − x0 )δ(x00 − x) = δ(x0 − x)
N
X
δ(x − xi )
δ(f (x)) =
| f 0 (x) |x=xi
i=1

donde xi son los ceros simples de f (x)

Delta de Dirac en 3 dimensiones
Se define
δ(~x − ~x0 ) = δ(x − x0 )δ(y − y 0 )δ(z − z 0 )
la cual cumple
˚

3 0

d x δ(~x − ~x ) =

V

˚

R3

˚

R3



1 si ~x ∈ V
0 si ~x ∈
/V

d3 x0 δ(~x − ~x0 ) = 1

d3 x0 δ(~x − ~x0 )f (~x0 ) = f (~x)

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
Muestre que una distribución discreta de cargas qi , i = 1, 2, ...N ubicada en los puntos ~xi ,
i = 1, 2, ...N es consistente con una distribución volumétrica de carga
N
X

ρ(~x) =

qi δ(~x − ~xi )

i=1

#### Solución
Para ver que la distribución de carga se puede escribir de esta forma, se debe verificar que el
campo eléctrico que genera es el correcto. En efecto
˚
~x − ~x0
~
d3 x0 ρ(~x0 )
E(~x) =
| ~x − ~x0 |3
R3

~ x) =
E(~

˚

3 0

dx

R3

N
X
i=1

qi δ(~x − ~xi )

~x − ~x0
| ~x − ~x0 |3

Si la distribución es finita (N es un número finito) podemos intercambiar la integral con la
suma (y nos aseguramos que no se espante ningún matemático)
~ x) =
E(~

N
X
i=1

qi

˚

~ x) =
E(~

3 0

R3

d x δ(~x − ~x0i )

N
X

qi

i=1

~x − ~x0
| ~x − ~x0 |3

~x − ~xi
| ~x − ~xi |3

que es el campo correcto generado por la distribución de carga

---

### Página 43

Problema
Demuestre la propiedad
δ(f (x)) =
donde xi son los ceros simples de f (x)

X δ(x − xi )
| f 0 (x) |x=xi
i

#### Solución
Sea la sucesión de funciones de cuadrado integrable


x < −1/n
0
δn (x) = n/2 −1/n < x < 1/n


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

X δ(x − xi )
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

X δn (x − xi )

(x)
| dfdx
|x=xi

i

Sea y(x) una función de prueba
ˆ ∞
ˆ ∞
X δn (x − xi )
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

Xˆ ∞
i

−∞

dx

δn (x − xi )

(x)
| dfdx
|x=xi

Por el teorema del valor medio integral
ˆ ∞
X
dxgn (x)y(x) =
−∞

i

y(x) =

X ˆ xi +1/n
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
X
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


f (x) < −1/n
0
hn (x) = n/2 −1/n ≤ f (x) ≤ 1/n


f (x) > 1/n

sea Ij = [x1j , x2j ], j = 1, 2, ... tal que ∀x ∈ Ij , −1/n ≤ f (x) ≤ 1/n (x2j ≥ x1j ) y tal que
\
Ij
Ii = φ

∀i 6= j (intervalos disjuntos). Así, por el teorema del valor medio integral
ˆ ∞
Xn
X ˆ x2i n
y(x∗i ) (x2i − x1i )
dxhn (x)y(x) =
dx y(x) =
x1i
−∞
i
i
con x∗i ∈ Ii . Además, está garantizada la existencia de un x0i ∈ Ii tal que
|
Luego

df (x)
| 2/n |
2/n
|x=x0i =
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
|x=x0i

Si n → ∞, Ij = xj tal que f (xj ) = 0. Así
ˆ ∞
dxh(x)y(x) =
lím dxhn (x)y(x) =
n→∞

−∞

y(xi )
df (x)
| dx |x = xi

Por lo tanto, se ha demostrado la igualdad entre las funciones generalizadas
δ[f (x)] =

X δ(x − xi )
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
en un punto ~x se obtiene evaluando la integral de Coulomb
˚ 3 0 0
d x ρ(~x )(~x − ~x0 )
~
E(~x) =
4π0
| ~x − ~x0 |3
V
Más adelante no utlizaremos demasiado ésta fórmula, la escribimos sólo para enfatizar el
hecho de que hemos resuelto completamente el problema de la electrostática en que conocemos
exactamente la distribución espacial de todas las cargas. Es decir, conocemos ρ(~x0 ) en todo el
espacio.

---

### Página 46

Problema que hemos resuelto: Dadas las cargas, ¿cómo son los campos?
Nuestra respuesta es : Resuelva esta integral
˚ 3 0 0
d x ρ(~x )(~x − ~x0 )
~
E(~x) =
4π0
| ~x − ~x0 |3
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

~ = S n̂ como el vector de área, cuya
Considere la superficie plana de la figura. Se define S
magnitud es el área de la superficie, S, y apunta en la dirección normal n̂ (perpendicular en
todo punto a la superficie). Si la superficie se encuentra sumergida en un campo eléctrico
~ que apunta siempre en la misma dirección de n̂ (perpendicular a la superficie S),
uniforme E
~ sobre el vector S
~
el flujo sobre la superficie es la proyección de E
~ ·S
~=E
~ · n̂S = ES
ΦE = E
Ahora, si el campo eléctrico sigue siendo uniforme pero forma un ángulo ϑ con n̂, el flujo
será

---

### Página 47

~ ·S
~ = EScosϑ
ΦE = E

Es decir, el flujo de un campo vectorial sobre una superficie mide en cierta forma la componente
normal a la superficie. Notar que según la definición del vector normal n̂, el flujo eléctrico es
positivo si las líneas de campo eléctrico están saliendo a través de la superficie, y será negativo
si las líneas entran a través de la superficie.
Generalización
Hemos definido el flujo del campo eléctrico sobre una superficie muy simple (plana). Además
hemos supuesto que el campo es uniforme (magnitud y dirección constantes). En general,una
~ puede variar sobre la superficie (tanto en
superficie S puede ser curva, y el campo eléctrico E
magnitud como en dirección).
Nos resultará de particular interés aquellas superficies que son cerradas. Una superficie
cerrada es aquella que envuelve completamente a un volumen (es el contorno de un volumen).
Para calcular el flujo del campo sobre una superficie cerrada, se divide la superficie en una
~i = ∆Si n̂i , como se ve en la figura.
suma de elementos de área infinitesimales, ∆S

~i es
El flujo a través de ∆S
~ i · ∆S
~i = Ei ∆Si cosθ
∆ΦE = E
El flujo total a través de la superficie se obtiene sumando sobre todos los elementos de
superficie. (A la Riemann) Tomando el límite cuando ∆Si → 0 se obtiene la integral de flujo
ˆˆ
X
 ~
~ i · dS
~i = 
~ x)
∆ΦE = lím
E
x) · E(~
 dS(~
∆Si →0

S

Le ley de Gauss establece que el flujo eléctrico a través de una superficie cerrada es
proporcional a la carga encerrada por ella. Más concretamente
ˆˆ
 ~ 0
~ x0 ) = qenc
x ) · E(~
ΦE =  dS(~
0
S

---

### Página 48

o, escribiendo de forma explícita la carga encerrada por S
ˆˆ
˚
 ~ 0
~
x ) · E(~x ) =
d3 x0 ρ(~x0 )
 dS(~
ε0
S
V (S)
Esta ley es consecuencia directa de la Ley de Coulomb y la geometría Euclídea. Notar que
campos eléctricos creados por cargas fuera de la superficie no contribuyen al flujo total. Es
decir, el flujo sobre una superficie cerrada sólo depende de la carga encerrada por ella.
La forma de la superficie puede ser elegida arbitrariamente. Para las superficies de la figura,
el mismo resultado se obtiene para el flujo eléctrico (ΦE = Q/0 ).

La ley de Gauss es extremadamente útil en muchos casos. Hay que notar, que a partir de
la Ley de Gauss es posible recuper la Ley de Coulomb, es decir, conociendo la ley de Gauss
uno podría determinar la forma de los campos. Hay que notar además, que hay casos en los
cuales esta ley no es práctica, es útil sólo en problemas donde la integral de flujo es simple
de calcular.
Ejemplo: Campo de una distribución esférica homogénea de carga
Tal como en el capítulo 1, se desea obtener el campo eléctrico de una distribución de carga

ρ0 si | ~x0 |≤ R
ρ(~x ) =
0 si | ~x0 |> R

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
 ~ 0


~
Φ =  dS(~x ) · E(~x ) =  dS r̂ · E(r)r̂ = E(r)  dS
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
~ = E(r)r̂ =
E

Q = πR3 ρ0

~ = E(r)r̂ = ρ0 R r̂
E
3ε0 r2
Mismo resultado obtenido en el capítulo anterior (ahora de forma mucho más simple). Ahora,
para el campo interno, nuevamente escogemos una superficie Gaussiana de radio r < R

Nuevamente el flujo es
 ~ 0
~ x0 ) = E(r)4πr2 = qin
x ) · E(~
Φ =  dS(~
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
(
rρ0
r̂ si | ~x |≤ R
~
E(~x) = ρ3ε
0R
r̂ si | ~x |> R
3ε0 r2
E(r) =

---

### Página 50

Notar que el campo es continuo en | x |= R

pero no es diferenciable en dicho punto!
Ejemplo: Plano infinito de carga
Consideremos un plano infinito en X − Y con densidad superficial de carga uniforme σ. Se
desea determinar el campo eléctrico en todo el espacio

~
Debido a que la carga está distribuída uniformemente en la superficie, el campo eléctrico E
~ = E k̂. Además, la magnitud del campo es constante en
debe ser perpendicular al plano , E
planos paralelos al plano de carga. Elegimos como superficie Gaussiana un cilindro (llamado
por muchos autores como caja de píldoras)

el flujo sobre esta superficie es
ˆˆ
¨
¨
¨
 ~ 0
~
~
~
~
~
~3 · E
~3
Φ =  dS(~x ) · E(~x ) =
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
 ~ ~
~
~
~2 · E
~2
Φ =  dS · E =
dS1 · E1 +
dS
S

---

### Página 51

S1 y S2 están a la misma distancia del plano infinito, luego, en ambas superficies la magnitud
del campo debe ser la misma, digamos, E, luego
¨

ˆˆ
¨
 ~ ~
Φ =  dS · E = E
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
~ x) =
E(~

(

σ
k̂
2ε0
σ
− 2ε0 k̂

si z > 0
si z < 0

notar que el campo tiene una discontinuidad en z = 0
σ
~
~
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
~ = E(r)r̂
E
Para r < a, elegimos una superficie Gaussiana esférica de radio r, como se muestra en la
figura

de la ley de Gauss
qin
 ~ ~
 dS · E =

ˆˆ

ε0

S

Es claro que en este caso no hay carga encerrada por la superficie, de forma que
ˆˆ

 ~ 0
~ x0 ) = E(r)4πr2 = 0 → E(r) = 0
x ) · E(~
 dS(~
S

Para r > a, nuevamente elegimos una superficie Gaussiana esférica de radio r

 ~ 0
~ x0 ) = 4πr2 E(r) = Q
x ) · E(~
 dS(~

ˆˆ

ε0

S

~ = E(r)r̂ =
E

Q
r̂
4πε0 r2

es decir, para r > a el campo es igual al de una carga puntual Q en el origen.

---

### Página 53

~ x) =
E(~



~0
Q
r̂
4πε0 r2

si | ~x |< a
si | ~x |> a

El campo es discontinuo en r = a (siempre lo es al atravesar una superficie cargada)

Notar que

Q
σ
=
r→a+
r→a−
4πε0 a
0
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
 ~ 0
~ x0 ) = 1 Qint
x ) · E(~
 dS(~

ˆˆ

0

S

donde S es cualquier superficie cerrada y Qint la carga encerrada por ésta
Qint =

˚

d3 x0 ρ(~x0 )

V (S)

~ x0 )//n̂(~x0 ) y | E(~
~ x0 ) |
Debemos encontrar una superficie con las siguientes características: E(~
constante ∀~x ∈ S . Dada la simetría del problema usamos como superficie un cilindro de radio
r > b y altura h S

---

### Página 55

Luego
¨

ˆˆ

 ~ 0
~ x) =
x ) · E(~
 dS(~
S

M anto

~ x0 ) · E(~
~ x0 ) +
dS(~

¨

T apas

~ x0 ) · E(~
~ x0 )
dS(~

~ x0 ) = dS(~x0 )n̂(~x0 ) = rdϕdzr̂(ϕ), y E(~
~ x0 ) = E(r)r̂(ϕ), de forma
Para todo ~x0 en el manto, dS(~
que
¨

M anto

~ x0 ) · E(~
~ x0 ) = E(r)
dS(~

¨

dS(~x0 ) = 2πrhE(r)

M anto

~ x0 ) = rdϕdrẑ, y en la tapa inferior
Por otro lado, para todo ~x0 en las tapa superior, dS(~
~ x0 ) = E(r)r̂(ϕ)⊥dS(~
~ x0 ), luego
~ x0 ) = −rdϕdrẑ , mientras que E(~
dS(~
¨

T apas

~ x0 ) · E(~
~ x0 ) = 0
dS(~

con esto
ˆˆ

 ~ 0
~ x) = E(r)2πrh
x ) · E(~
 dS(~
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

 ~ 0
~ x) = 1 Qint
x ) · E(~
 dS(~

ˆˆ

0
Por los mismos argumentos utilizados anteriormente, la integral de flujo se reduce a
ˆˆ
 ~ 0
~ x) = E(r)2πrh
x ) · E(~
 dS(~
S

S

y
Qint =

˚

3 0

d x ρ(~x ) = ρ

V (S)

entonces

˚

d3 x0 = ρπa2 h

V (S)

πa2 h
E(r)2πrh = ρ
0

~ x) = a ρ r̂
E(~
20 r
si r ∈ [a, b]
Por último, para la región III: r < a, se escoge nuevamente un cilindro de radio r y altura
h. Los mismos argumentos de simetría son válidos aquí para determinar el campo eléctrico.
Resulta
ˆˆ
 ~ 0
~ x) = 1 Qint
x ) · E(~
 dS(~
0
S
y
ˆˆ
 ~ 0
~ x) = E(r)2πrh
x ) · E(~
 dS(~
S
˚
˚
3 0
Qint =
d x ρ(~x ) = ρ
d3 x0 = ρπr2 h
V (S)

V (S)

entonces
E(r)2πrh = ρ

πr2 h
0

~ x) = ρr r̂
E(~
20
En resumen (notar discontinuidad al atravesar la superficie cargada r = b)
 ρr
 20 si 0 ≤ r < a
~ x) = a2 ρ si a < r < b
E(~
 20 r
si b < r

---

### Página 57

Problema
Considere dos esferas no concéntricas de radio R. La primera de ellas lleva una densidad
volumétrica de carga ρ y la segunda −ρ. Los centros de las esferas están a distancia menor
que 2R. si d~ es el vector que va del centro de la esfera positiva al centro de la negativa, demuestre que el campo eléctrico en la intersección de las esferas es constante, y encuentre su
valor

#### Solución
Este problema se resuelve por superposición y recordando la forma del campo eléctrico generado
por una distribución homogénea y esférica de carga (resuelto anteriormente)

~ x) =
E(~

(

ρr
r̂
30
ρR3
r̂
30 r2

si r ≤ R
si r > R

donde r es la distancia al centro de la distribución. Ahora, sea P un punto arbitrario dentro
de la región de la intersección

---

### Página 58

El campo en P producido por la distribución de carga positiva es
~ 1 = ρ ~r
E
30
y el de la distribución de carga negativa
~ 2 = −ρ ~r0
E
30
Por el principio de superposición, el campo eléctrico en P está dado por
~ )=E
~1 + E
~ 2 = ρ ~r + −ρ ~r0
E(P
30
30
Pero
de forma que

d~ + ~r0 = ~r
~r0 = ~r − d~


~ ) = ρ ~r + −ρ ~r − d~
E(P
30
30

~ ) = ρ d~
E(P
30
P fue escogido de manera arbitraria, luego, para todo ~x dentro de la distribución, el campo
eléctrico es uniforme y está dado por
~ x) = ρ d~
E(~
30
notar que es paralelo a la dirección que une ambos centros

---

### Página 59

Problema
Se tiene un cilindro de radio R muy largo y con densidad de carga homogénea ρ. Se ha suprimido
un cilindro con eje paralelo con el mismo largo y radio R/2. El vector que une el centro del
cilindro con el centro de la cavidad es ~a para una sección transversal. Se pide obtener la expresión
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
 ~ 0
~ x0 ) = Qin
x ) · E(~
 dS(~

ˆˆ

0

S

Ahora, notemos que el cilindro lo podemos dividir en 3 superficies

---

### Página 60

Luego la ley de Gauss queda
ˆˆ
¨
¨
¨
 ~ 0
~
~
~
~
~
~3 · E
~3
x ) · E(~x ) =
dS1 · E1 +
dS2 · E2 +
dS
 dS(~
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
 ~ 0
~
~
~
x ) · E(~x ) =
dS3 · E3 =
Er r̂ · dS3 r̂
 dS(~
S

S

E(r)

¨

S

dS3 = E(r)2πrL

S

Ahora, la carga encerrada por la superficie de Gauss es
˚
d3 x0 ρ(~x0 )
Qin =
V (S)

donde V (S) es el volumen encerrado por S. Como ρ es constante,
˚
Qin = ρ
d3 x0 = ρπr2 L
V

Luego la ley de Gauss queda
E(r)2πrL = ρπr2 L
ρr
E(r) =
Ahora, eligiendo un punto P dentro de la cavidad, tendremos que el campo total será la
suma vectorial del campo eléctrico debido a un cilindro homogéneo de carga y del campo debido
a un cilindro homogéneo de carga negativa, tal como indica la figura

~ 1 = ρr r̂
E
~ 2 = − ρx r̂0
E
donde
r̂0 =

(rr̂ − ~a)
(~r − ~a)
=
x
x

Sumando ambos campos

---

### Página 61

~ = ρr r̂ − ρx (rr̂ − ~a)
E
x
~ = ρr r̂ − ρrr̂ + ρ~a
E
~ = ρ~a
E
El campo en todo punto de la cavidad es uniforme y paralelo al vector ~a

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
~ 1 = σ k̂
E
20
Ahora, para calcular el campo en el eje de un disco, de radio R y densidad σ

Un elemento de superficie del disco está dado por dA = rdrdφ, que tiene asociado un
elemento diferencial de carga, dado por dq = σdA = σrdrdφ.
Así, el campo eléctrico en P debido a este elemento de superficie será
~2 =
dE

1 dq(~x − ~x0 )
4π0 | ~x − ~x0 |3

donde ~x = xk̂, ~x0 = r(cos φî + sin φĵ) así

---

### Página 63

| ~x − ~x0 |= (r2 + x2 )1/2
~x − ~x0 = xk̂ − r(cos φî + sin φĵ)
Con esto la contribución al campo total en P debido al elemento de superficie es
~2 =
dE

1 σrdrdφ(xk̂ − rr̂)
4π0 (r2 + x2 )3/2

Así, el campo eléctrico total en P debido al disco completo será
~ 2 = σx
E
4π0

ˆ 2π

dφ

ˆ R

r
σ
dr 2
k̂ −
3/2
(r + x )
4π0

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

~ 2 = 2π σx
E
4π0

x2

du
k̂
2u3/2

Donde el factor 2π sale de integrar dφ entre 0 y 2π. Finalmente
x2 +R2

~ 2 = σx − 2u−1/2
E
40
x2

k̂ = −

σx
σx 1
√
+
k̂
20 R + x
20 x

√
−σx
+
σ
R 2 + x2
~2 =
√
k̂
E
20 R2 + x2
~2 = σ
E
20



x
1− √
R 2 + x2



k̂

Notar que si R → ∞ se recupera el campo de un plano infinito
~ = σ k̂
E
2o
~ 2 , ya que el disco tiene
~ 1 y -E
Finalmente el campo eléctrico total en P , será la suma de E
densidad de carga −σ
~ )= σ + σ
E(P
20 20




x
√
− 1 k̂
R 2 + x2

~ )= σ √ x
k̂
E(P
20 R2 + x2

b)

---

### Página 64

Para calcular la fuerza sobre el alambre de carga, bastará con tomar un elemento diferencial
de longitud dx y obtener la fuerza electrostática que actúa sobre éste
~
~
dF~ = dq E(x)
= λdxE(x)
=

σx
λ
√
dxk̂
20 R2 + x2

Con lo que la fuerza total sobre la línea de carga será

ˆ µ+a 
σx
λ
√
dx
F =
k̂
20 R2 + x2
µ
Sea z = R2 + x2 , con lo que dz = 2xdx. Finalmente
λσ
F~ =
40

ˆ R2 +(µ+a)2
R2 +µ


p
dz
σλ p 2
√ î =
R + (µ + a)2 − R2 + µ2 k̂
20
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
ρ0 =

k0
,0 ≤ r ≤ R
r2

Sea la región del espacio en que r > R. Dada la simetría esférica de la distribución, escogemos
como superficie Gaussiana S una esfera concéntrica al origen y de radio r > R

---

### Página 66

El flujo a través de S será
ˆˆ

 ~ 0
~ x0 ) = 4πr2
x ) · E(~
 dS(~
S

La carga encerrada por esta superficie es
˚
ˆ 2π
ˆ π
ˆ R
k0
3 0
Qint =
d x ρ(~x ) =
dϕ
dϑ sin ϑ
drr2 2 = 4πRk 0
r
V (S)
Por ley de Gauss
E(r)4πr2 =

4πRk 0
0

Rk
~
r̂, r > R
E(r)
=
0 r 2
Ahora, para r < R, nuevamente se utiliza una superficie esférica de radio r y se resuelve en
forma análoga a la anterior, lo único que varía es la carga encerrada
ˆˆ
 ~ 0
~ x0 ) = 4πr2
x ) · E(~
 dS(~
S

esta vez la carga encerrada es la carga contenida en todo el volumen de la superficie de
Gauss
˚
Q=
d3 x0 ρ(~x0 ) = 4πrk 0
S(V )

entonces

4πrk 0
E(r)4πr =
0

k
~
E(r)
=
r̂
0 r
Ahora, superponemos los campos generados por ρ1 y ρ2 . Si r > b > a
~ = bk r̂ + (−k)a r̂
E
0 r 2
0 r 2
~ = k(b − a) r̂
E
0 r 2
Si a < r < b

(−k)a
k
~
r̂
r̂ +
E(r)
=
0 r
0 r 2


k
ak
~
E(r) =
r̂
−
0 r 0 r 2

Por último, para
r<a


k
k
~
E(r) =
−
r̂
0 r 0 r
~
E(r)
=0

---

### Página 67

En resumen
~
E(r)
=







si r < a

k
− ak
0 r
0r
k(b−a)
r̂
0 r 2



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
~ solo tendrá componente en la dirección î.
simetría el campo E
Notar además, que para x > 0, el campo tendrá dirección x̂, mientras que si x < 0, el campo
tendrá dirección −x̂. Utilizando un cilindro como superficie de Gauss, de radio x , se tiene
ˆˆ
 ~ 0
~ x0 ) = qin
x ) · E(~
 dS(~
0
S
En este caso sólo habrá flujo a través de las tapas del cilindro, puesto que el campo es
horizontal y perpendicular a la normal del cilindro sobre el manto. Luego
ˆˆ
 ~ 0
~ x0 ) = E(x)2S
x ) · E(~
 dS(~
S

---

### Página 69

donde S es el área de cada tapa. Ahora, la carga encerrada por este cilindro será simplemente
qin = ρV = ρ2xS
Con esto
2SE(x) =

ρ2xS
0

E(x) =

ρx
0

Finalmente, para | x |< a/2

~ = ρx î
E
0

Ahora, para obtener el campo en un punto exterior a distancia r > a/2 del plano central,
volvemos a utilizar la ley de Gauss, como se aprecia en la figura

Nuevamente sólo habrá flujo por S1 y S2 , luego
¨

¨
ˆˆ
 ~ 0
~
x ) · dE(~x ) = E(r)
dS1 +
dS2
 dS(~
S

S1

S2

ˆˆ

 ~ ~
 dS · E = E(r)2S
S

la carga encerrada por el cilindro será
qin = ρaS
Luego
E(r)2S =

ρaS
0

de donde se obtiene, para | r |> a/2
~ = ρa î
E
20
Notar que no depende de la distancia al plano central.
b) Por el principio de superposición, este problema equivale a considerar la distribución de
carga de la parte a) más una esfera de densidad volumétrica de carga −2ρ.
El campo en el centro de la esfera, debido a la esfera misma es nulo, por simetría. Así, el
~
~ es el campo interior creado por la
campo total en el centro será, simplemente E(a/4)
donde E
distribución entre planos calculado anteriormente.

---

### Página 70

~ centro = ρa î
E
40
Ahora, para obtener el campo en el punto P, calculemos primero el campo debido a la esfera
de carga usando la Ley de Gauss,

 ~ 0
~ x0 ) = qin
x ) · E(~
 dS(~

ˆˆ

0

S

ˆˆ

ˆˆ

ˆˆ



 ~ 0
~ x0 ) = 
x ) · E(~
 dS r̂ · E(r)r̂ = E(r)  dS
 dS(~
S

S

S

ˆˆ

 ~ 0
~ x0 ) = E(r)4πr2
x ) · E(~
 dS(~
S

y la carga encerrada por la superficie de Gauss es
qin = −2ρ

πa3
4π(a/4)3
= −ρ

Con esto
E(r) = −

ρa3
96r2 0

Esto corresponde al campo debido a la esfera, donde r es la distancia entre el punto P y el
centro de la esfera. En este caso, el centro de la esfera se encuentra en x = a/4, con lo que el
campo total en P sera

con | x |> a/2

ρa3
~ ) = ρa î −
E(P
î
20
960 (x − a/4)2

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
 ~ 0
~ x)=
~
x ) · E(~
dϕr
dzr̂(ϕ) · E(r)r̂(ϕ)
= 2πrhE(r) =
 dS(~
0
S
y entonces
~
E(r)
=

λ
r̂
2π0 r

De esta forma, en el plano que contiene a ambas distribuciones, y definiendo las direcciones
î, ĵ (como se indica en la figura)

---

### Página 72

el campo eléctrico generado por la distribución lineal tiene la forma
λ
ĵ
2π0 r
donde r es la distancia vertical entre ~x y el alambre. Fijando el origen de coordenadas según
lo indicado en la figura, calculemos la fuerza que se ejerce sobre una porción de largo L de la
distribución plana de carga con densidad σ. Un elemento de área de coordenadas (x, y) posee
una carga dada por
~ x) =
E(~

dq(x, y) = σdxdy
y el campo eléctrico en dicho punto debido a la distribución lineal es
~
E(x,
y) =

λ
ĵ
2π0 (d + y)

Luego, la fuerza que se ejerce sobre este elemento de área es
dF~ (x, y) = dxdyσ

λ
ĵ
2π0 (d + y)

consideremos la distribución dada por 0 ≤ x ≤ L, 0 ≤ y ≤ b. La fuerza neta sobre esta
porción es
ˆ L ˆ b
σλ
~
F =
ĵ
dx
0 2π0 (d + y)
ˆ b
b
σλL
σλL
ln(d + y) ĵ
ĵ =
F~ =
2π0 0 d + y
2π0


σλL
d+b
~
ĵ
F =
ln
2π0
d
y la fuerza por unidad de largo es



F~
σλ
d+b
ĵ
=
ln
L
2π0
d

---

### Página 73

#### Capítulo 5
El potencial Electrostático
Vimos anteriormente que el campo Electrostático generado por una distribución de carga
se escribe en su forma más general como una integral de Coulomb
˚
(~x − ~x0 )
~
E(~x) =
d3 x0 ρ(~x0 )
4π0
|~x − ~x0 |3
R3
Hemos establecido además una relación interesante entre el flujo del campo sobre una superficie cerrada y la carga encerrada por ésta (Ley de Gauss). Esta relación es consistente con
la ley de Coulomb y establece que el flujo del campo eléctrico sobre cualquier superficie cerrada
S es
ˆˆ
˚
  ~0 ~ 0
x)=
d3 x0 ρ(~x0 )
 dS · E(~
ε
S
V (S)
Ahora, veremos una segunda ley muy importante en electrostática, y para enunciarla demostraremos el siguiente lema
~
∇
Demostración
Esta es trivial considerando que

~x − ~x0
=
−
| ~x − ~x0 |
|~x − ~x0 |3

| ~x − ~x0 |= (x − x0 )2 + (y − y 0 )2 + (z − z 0 )2
y
~
∇

1/2

∂
∂
∂
=
k̂
î +
ĵ +
| ~x − ~x |
∂x | ~x − ~x |
∂y | ~x − ~x |
∂z | ~x − ~x0 |

veamos que ocurre con la componente según î
∂
∂
| ~x − ~x0 | î
î
=
−
∂x | ~x − ~x0 |
| ~x − ~x0 |2 ∂x
−1/2
∂
2(x − x0 )î
î = −
(x − x0 )2 + (y − y 0 )2 + (z − z 0 )2
∂x | ~x − ~x |
| ~x − ~x | 2
∂
x − x0
î
î = −
∂x | ~x − ~x0 |
| x − x0 |3

---

### Página 74

El cálculo es análogo para las demás componentes, y se demuestra que
~
∇

~x − ~x0
=
−
| ~x − ~x0 |
|~x − ~x0 |3

¿Qué tendrá que ver esto con electrostática? No es difícil reconocer el parecido del campo
vectorial
~x − ~x0
|~x − ~x0 |3
con el campo electrostático, puesto que en su forma más general puede ser escrito como
˚
(~x − ~x0 )
~ x) =
d3 x0 ρ(~x0 )
E(~
4π0
|~x − ~x0 |3
R3
Utilizando el lema recién demostrado, esto se reescribe como
˚
~
~
d3 x0 ρ(~x0 )∇
E(~x) = −
4π0
| ~x − ~x0 |
R3
~ x) = −∇
~ 1
E(~
4π0

˚

d3 x0 ρ(~x0 )

R3

| ~x − ~x0 |

Se obtiene que el campo eléctrico es menos el gradiente de un campo escalar. Se define el
potencial electrostático de una distribución de cargas como
˚
ρ(~x0 )
φ(~x) =
d3 x0
4π0
| ~x − ~x0 |
R3
y el campo eléctrico cumple

~ x) = −∇φ(~
~ x)
E(~

Notar que es inmediato que el potencial de una carga puntual ubicada en ~x0 estará dado
por
φ(~x) =

q
4π0 | ~x − ~x0 |

Potencial de una distribución discreta
Supongamos que se tiene una distribución discreta de cargas qj , j = 1, 2, ...N ubicadas en las
posiciones ~xj , j = 1, 2, ...N . El potencial de ésta distribución se puede obtener fácilmente a
partir del potencial de una sola carga utilizando el principio de superposición
N

φ(~x) =

1 X
qj
4π0 i=1 | ~x − ~xi |

por supuesto, esto es consistente con la densidad de carga en términos de la delta de Dirac
ρ(~x) =

N
X
i=1

qi δ(~x − ~xi )

---

### Página 75

en efecto, de la definición para el potencial
φ(~x) =
4π0

ρ(~x0 )
=
dx
| ~x − ~x0 |
4π0
R3

˚

3 0

N

1 X
φ(~x) =
qi
4π0 i=1

˚

d3 x0

R3

N
X
qi δ(~x0 − ~xi )
| ~x − ~x0 | i=1

N

x0 − ~xi )
3 0 δ(~

1 X
qi
=
dx
| ~x − ~xi |
4π0 i=1 | ~x − ~xi |
R3

˚

N

1 X
qj
φ(~x) =
4π0 i=1 | ~x − ~xi |

5.1.

Interpretación Física del Potencial

Supongamos que se tiene una distribución de carga en el espacio, ésta generará un campo
~ x). Consideremos el trabajo efectuado contra las fuerzas del campo al trasladar
eléctrico E(~
cuasiestáticamente una carga puntual q desde un punto ~x1 hasta el punto ~x2 , siguiendo una
trayectoria cualquiera Γ. Por cuasiestáticamente, se entiende que no se altera la energía cinética
al mover a la carga. Esto se puede lograr exclusivamente si la fuerza neta sobre la carga es cero
(recordar Teorema del Trabajo). De esta forma, debemos ejercer una fuerza de igual magnitud
y contraria a la fuerza electrostática que actúa sobre la carga. Esto es
ˆ ~x2
~ x)
d~x · q E(~
W =−
~
x1

Podría ser que este trabajo dependiera de la trayectoria utilizada para ir desde ~x1 hasta ~x2 .
Sin embargo, como
~ x) = −∇φ(~
~ x)
E(~
W =−

ˆ ~x2
~
x1

~ x) = q
d~x · q E(~

ˆ ~x2
~
x1

~ x)
d~x · ∇φ(~

Utilizando la parametrización de la curva Γ: ~x = ~x(l0 ), donde l ∈ [0, l]
ˆ l
d~x ~
W =q
dl0 0 · ∇φ(~
x(l0 ))
dl

---

### Página 76

W =q

ˆ l

ˆ φ2
x(l0 ))
0 dφ(~
dφ = q (φ2 − φ1 )
dl
=q
dl0
φ1

Finalmente hemos obtenido
W = −q

ˆ ~x2
~
x1

~ x) = q (φ2 − φ1 )
d~x · E(~

Independiente de la curva Γ!
Si tomamos una carga unitaria, q = 1, la interpretación de éste resultado es como sigue:
El trabajo necesario para mover una carga unitaria cuasiestáticamente desde el punto x1 hasta
el punto x2 contra el campo eléctrico es igual a la diferencia de potencial entre x2 y x1
Ahora, notemos que
ˆ ~x2
~
x1

~ x) = − (φ2 − φ1 )
d~x · E(~

Por lo tanto, sobre una trayectoria cerrada
˛
~ x) = 0
d~x · E(~
el campo eléctrico es conservativo. Obsérvese que este resultado físico es consecuencia de
Coulomb y la geometría Euclídea
Notar que U (~x) = qφ(~x) es la Energía Potencial de una carga q en la posicion ~x. En
efecto, la fuerza asociada a esta interacción es
~ (~x) = q E(~
~ x)
F~ = −∇U

Otro enfoque para la electrostática
La introducción del campo escalar φ presenta muchas ventajas para resolver matemáticamente
el problema de la electrostática. Como vimos, si conocemos la distribución de carga, es decir, conocemos explícitamente ρ(~x), podemos calcular el campo resolviendo las integrales de
Coulomb. Sin embargo, como ya se dijo anteriormente, éstas integrales pueden ser complicadas,
un método alternativo sería resolver las integrales de Coulomb para el potencial
˚
d3 x0 ρ(~x0 )
φ(~x) =
4π0
x − ~x0 |
R3 | ~

Notar que calcular esta integral es notoriamente más simple que calcular la integral para
el campo eléctrico. En primer lugar, no aparece ninguna cantidad vectorial. En segundo lugar,
el potencial sólo depende del inverso de la distancia a la fuente, en cambio el campo eléctrico
depende del cuadrado de la distancia. Notemos que una vez obtenido el potencial en todo el
~ x) = −∇φ(~
~ x),
espacio, determinar el campo eléctrico es muy sencillo, sólo basta con evaluar E(~
y todos sabemos que derivar es mucho más sencillo que integrar.
Ahora, aún no hemos dicho nada sobre qué hacer cuándo la distribución de carga no es
conocida, eso lo veremos más adelante, pero justamente el potencial electrostático es una herramienta muy poderosa a la hora de resolver ese tipo de problemas más complejos.

---

### Página 77

5.2.

Energía Potencial de una distribución de carga discreta

El trabajo necesario para traer una carga q cuasiestáticamente desde el infinito hasta un
punto ~x es, simplemente
W = qφ(~x)
suponiendo que el potencial en el infinito es cero (Esto se cumple si, por ejemplo, toda la
carga está localizada dentro de un volumen finito). Luego, esta carga ha adquirido una energía
potencial igual a U (~x) = qφ(~x). De la misma forma, una distribución de carga tiene una energía
potencial asociada, ya que un trabajo se debe realizar para mantener la distribución en su lugar.
Calculemos la energía potencial de un sistema electrostático de cargas puntuales. Para ello
inicialmente traemos una carga q1 hasta un punto cualquiera ~x1 . El trabajo necesario para esto
es nulo, ya que inicialmente no existe un campo eléctrico alguno que ejerza una fuerza sobre
q1 . Con esto
W1 = 0
y el sistema en este estado posee una energía potencial igual a
U = W1 = 0
Ahora, para traer una carga q2 hasta un punto ~x2 , como se aprecia en la figura

se requiere hacer un trabajo igual a
W2 = φ(x2 )q2 =

q1
q2
4π0 | ~x1 − ~x2 |

Con esta configuración, el sistema tiene asociada una energía potencial dada por
U = W1 + W 2 =

q1
q2
4π0 | ~x1 − ~x2 |

Ahora, para traer una tercera carga q3 , como se ve en la figura

---

### Página 78

el trabajo necesario será
W3 = q3 φ(~x3 ) =



q1
q2
+
4π0 | ~x1 − ~x3 | 4π0 | ~x2 − ~x3 |



q3

En síntesis, el trabajo necesario para formar esta configuración de 3 cargas a distancias r12 ,
r13 , r23 es
1 q1
1 q2
1 q1
q3 +
q3 +
q2
4π0 r13
4π0 r23
4π0 r12
Y es igual a la energía potencial total de esta configuración, que se puede reescribir como
U = W 1 + W2 + W3 =

U=

U=



1 1 q1 q 2 q2 q1 q1 q3 q 3 q1 q 2 q3 q3 q2
(
+
+
+
+
+
)
2 4π0 r12
r21
r13
r31
r23
r32

1 q2
1 q3
+
4π0 r21 4π0 r31



q1 +



1 q1
1 q3
+
4π0 r12 4π0 r32



q2 +



1 q1
1 q2
+
4π0 r13 4π0 r23

 
q3

(φ(~x1 )q1 + φ(~x2 )q2 + φ(~x3 )q3 )
Donde φ(~xi ) no es más que el potencial en la posición de la carga i debido a las demás
cargas. En general, para un sistema de N cargas, se tiene que la energía potencial asociada al
sistema es
N
1X
U=
qi φ(~xi )
2 i=1
U=

Esto se puede extender al caso continuo, donde la energía potencial de una distribución
continua de carga es, equivalentemente
˚
˚
U=
φ(~x )dq(~x ) =
d3 x0 ρ(~x0 )φ(~x0 )
V
V

---

### Página 79

5.3.

El dipolo Eléctrico

Definiremos una cantidad absolutamente general asociada con una distribución de cargas
ρ(~x), llamada Momento Dipolar
˚
p~ =
d3 x0~x0 ρ(~x0 )
V

donde V es un volumen que contiene todas las cargas. Notar en primer lugar que p~ es
un vector constante que dependerá de la forma en que están distribuídas las cargas. De cierta
forma, es una suma de las posiciones ponderadas por sus respectivas cargas. El momento dipolar
de una distribución discreta de N cargas es, por supuesto
p~ =

N
X

~xi qi

i=1

Dipolo Eléctrico
Estudiemos ahora un cierto tipo muy particular de distribución de carga. Primeramente, imaginemos 2 cargas cualquiera q1 , q2 separadas una distancia a, como muestra la figura

El momento dipolar está dado por
p~ = q1~x1 + q2~x2
Definamos además, el vector ~x como el vector posición del punto medio entre q1 y q2 , y la
dirección k̂ que apunta desde q1 hacia q2 . De esta forma, es claro que
a
~x1 = ~x − k̂
a
~x2 = ~x + k̂
luego

a
a
p~ = q1 (~x − k̂) + q2 (~x + k̂)

a(q2 − q1 )
k̂
Ahora, consideremos que ambas cargas son iguales en magnitud, pero de signo opuesto.
Digamos q2 = q, q1 = −q. Esto es lo que se conoce como dipolo eléctrico y entonces
p~ = (q1 + q2 ) ~x +

p~ = qak̂

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


q
q
φ(P ) =
−
4π0 r + r−

Donde, por el teorema del coseno

= r2 + d2 − 2dr cos ϑ
r+
r−
= r2 + d2 + 2dr cos ϑ

r+ = r

p
1 + (d/r)2 − 2(d/r) cos ϑ

Para el límite en que d << r, se puede desarrollar en series de Taylor


−1/2 1
1 − (d/r) + (d/r) cos ϑ + ...
1 + (d/r) − 2(d/r) cos ϑ)
=
=
r+
r
r

Conservaremos los términos hasta segundo orden en d/r, como en la expansión (1 + x)n ≈
1 + nx + n(n − 1)/2x2 , cuando x


1 − (d/r) + (d/r) cos ϑ
≈
r+
r
De forma análoga

≈
r−
r



1 − (d/r)2 − (d/r) cos ϑ



---

### Página 81

Con esto, el potencial en P puede aproximarse por
q 2d cos ϑ
4π0 r
r
Si a = 2d es la separación entre las cargas del dipolo
φ(P ) ≈

φ(P ) ≈

p cos ϑ
q a cos ϑ
=
4π0 r r
4π0 r2

Donde p~ = aq ĵ es justamente el momento dipolar eléctrico. Notar entonces que el potencial
eléctrico debido a un dipolo microscópico (a << r) queda absolutamente determinado por
su momento dipolar p~ y disminuye según el cuadrado de la distancia (es un potencial más débil
que el de una carga puntual). Escribiendolo en su forma más general posible
φ(~x) =

p~ · r̂
p~ · ~x
=
4π0 r
4π0 | ~x |3

Notar que existe una clara simetría azimutal, pues el potencial no depende del ángulo polar ϕ

Fig. 5.1: Un dipolo eléctrico y sus líneas de campo eléctrico
Podemos obtener el campo eléctrico como el antigradiente del potencial
~ = ∂f r̂ + 1 ∂f ϑ̂ + 1 ∂f φ̂
∇f
∂r
r ∂ϑ
r sin φ ∂φ
El campo eléctrico sólo tendrá componentes en las direcciones r̂ y θ̂.
p cos ϑ
∂φ
=
∂r
2π0 r3
1 ∂φ
p sin ϑ
Eϑ = −
=
r ∂ϑ
4π0 r3
Er = −

Así
p
(2 cos ϑr̂ + sin ϑϑ̂)
4π0 r3
El campo eléctrico debido a un dipolo microscópico disminuye según el inverso del cubo
de la distancia. Notar que un dipolo microscópico corresponde a un dipolo visto desde muy
lejos. Lo interesante es que si bien es eléctricamente neutro, produce un campo eléctrico, y
también interactúa con campos eléctricos externos. La explicación de ésto es que, si bien un
~ =
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
U = −qφ(~x) + qφ(~x + ~a)
Podemos desarrollar φ(~x + ~a) en serie de Taylor (hasta primer orden)
φ(~x + ~a) = φ(x, y, z) +

∂φ(x, y, z)
∂φ(x, y, z)
∂φ(x, y, z)
ax +
ay +
az
∂x
∂y
∂z

~ x) · ~a
φ(~x + ~a) = φ(~x) + ∇φ(~
de forma que
~ x)
U = q~a · ∇φ(~
U = p~ · ∇φ(~x)
o, equivalentemente
~ x)
U = −~p · E(~

5.6.

Fuerza sobre un dipolo situado en un campo externo

El hecho de que el campo electrostático (y por lo tanto, la fuerza electrostática) sea conservativo, nos permite obtener la fuerza que siente un dipolo inmerso en un campo eléctrico
~ como el antigradiente de la energía potencial, esto es
externo E,

---

### Página 83

~
F~ = −∇U


~
~
~
F = ∇ p~ · E(~x)
~ E(~
~ x)
F~ = (~p · ∇)

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

~ 1 (~x) =
E

(

σ
î
20
σ
− 20 î

si x > 0
si x < 0

Ahora, para el plano cargado negativamente
(
σ
~ 2 (~x) = − 20 î si x > d
E
σ
î si x < d
20
El campo eléctrico total se obtiene de la suma de ambos campos, luego, es fácil ver que
~ = σ î
E
0
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
~ = mgtgϑ î
E
q
Igualando, se obtiene que

mgtgϑ
σ
=
0
q

de donde la densidad superficial de carga está dada por
σ=

mg0 tgϑ
q

b) La diferencia de potencial entre los planos se puede obtener integrando el campo eléctrico
sobre una trayectoria cualquiera entre la placa izquierda y la placa derecha. Por supuesto,
elegimos una trayectoria horizontal, de manera que el campo es paralelo en todo instante a la
curva
ˆ 0
ˆ d
mgtgϑd
mgtgϑ
~
dx =
φ(0) − φ(d) = −
d~x · E =
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
Tomemos un elemento infinitesimal de longitud en el anillo dl = Rdφ0 , como se aprecia en la
figura

Este elemento posee una carga
dq = dφ0 Rλ
Su contribución al potencial en P es
dφ0 Rλ
1 dq
√
=
dφ(P ) =
4π0 r
4π0 R2 + z 2
Luego, el potencial debido al anillo completo está dado por
ˆ 2π
dφ0
Rλ
√
φ(P ) =
4π0 R2 + z 2
φ(P ) =

2πRλ
√
4π0 R2 + z 2

notar que Q = 2πRλ es la carga total del anillo, luego
V (P ) =

Q
√
4π0 R + z 2

---

### Página 87

Es fácil ver que si z >> R, se tiene el potencial de una carga puntual
1 Q
V (P ) =
4π0 | z |
Ahora, el campo eléctrico en el punto P se puede obtener a partir del potencial como
~ ) = −∇φ(P
~
E(P
)

~ es necesario conocer φ(x, y, z). Aún así, veamos que sucede
Sin embargo, para evaluar ∇φ
con
−

∂φ
k̂
∂z

2zπRλ
~ )
k̂ = E(P
4π0 (R2 + z 2 )3/2
y se recupera el resultado obtenido anteriormente para el campo en el eje. ¿Qué nos dice
esto acerca de las derivadas parciales con respecto a x e y del potencial en un punto de la forma
(0, 0, z)?
Ahora, para obtener el potencial de un disco de radios a y b, simplemente se considera la
superposición de anillos inifintesimales

Tomamos un anillo de radio r y ancho infinitesimal dr, sabemos que el potencial en el eje
está dado por
dQ
√
4π0 r2 + z 2
donde dQ = σ2πrdr es la carga que contiene ese anillo
Luego
dφ(P ) =

dφ(P ) =

2πσ
drr
√
4π0 r2 + z 2

Y el potencial es

ˆ b
drr
σ
√
φ(P ) =
20 a
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

√
σ √ 2
φ(P ) =
b +z − a +z
20

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

~ x)
d~x · E(~

~ x) y elegir un camino desde a a
Para evaluar la integral, claramente debemos encontrar E(~
b . Utilizamos una superficie Gaussiana S esférica de radio r, con a < r < b, como muestra la
figura

Por ley de Gauss

 ~ 0
~ x0 ) = E(r)4πr2 = Q
x ) · E(~
 dS(~

ˆˆ

0

S

Luego, en la región entre los dos cascarones
~ x) =
E(~

Q
r̂
4π0 r2

---

### Página 89

Dada la forma del campo, resulta inteligente elegir un camino radial
Γ : ~x = rr̂
r:a→b
Luego
d~x = drr̂
y
~ x) = dr
d~x · E(~
Entonces

Q
4π0 r2

ˆ b

ˆ b
drQ
dr
Q
=−
φ(b) − φ(a) = −
4π0 a r2
a 4π0 r
ˆ b
Q
Q 1 a
dr
φ(b) − φ(a) =
=
−
4π0 a r2
4π0 r b

Q
∆V =
4π0
Notar que



1 1
−
b a



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

 ~ 0
~ x0 ) = 4πr2 = Qint
x ) · E(~
 dS(~

ˆˆ

0

S

la carga encerrada por S está dada por la siguiente integral
˚
ˆ 2π
ˆ π ˆ a
3 0
d x ρ(~x ) =
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
4π0 r2
Si ahora se utiliza una superficie esférica de radio r < a, la carga interior será
~
E(r)
=

qint =

4πC λ+3
r
λ+3

Luego, el campo interior tiene la forma
~
E(r)
=

C λ+1
r r̂
λ+3

Para evaluar φ(r) debemos calcular
φ(r) = −

ˆ ∞
r

~ x)
d~x · E(~

Hay que tener cuidado al realizar este cálculo si r > a o r < a.

---

### Página 91

i) Potencial exterior r > a

φ(r) = −

ˆ ∞
r

~ x) =
d~x · E(~

ˆ ∞
r

~ x)
d~x · E(~

Por comodidad elegimos un camino radial
~x = r0 r̂
r0 : r → ∞
d~x = dr0 r̂

Luego
~ x) = dr0
d~x · E(~

φ(r) =

ˆ ∞
r

Q
4π0 r02

Q
dr0 Q
=
4π0 r02
4π0

entonces
φ(r) =



− 0
r



∞
r

Q
,r ≥ a
4π0 r

Caλ+3
,r ≥ a
φ(r) =
(λ + 3) 0 r
ii) Si r < a

φ(r) =

ˆ ∞
r

~ x) =
d~x · E(~

ˆ a
r

la segunda integral se obtiene al evaluar φ(r)

~+
d~x · E
r=a

ˆ ∞
a

~ x)
d~x · E(~

con φ(r) el potencial exterior encontrado

anteriormente. La primera integral resulta (tomando un camino radial)
~x = r0 r̂
r0 : r → a
d~x = dr0 r̂

~ · ~x = dr0 C r0λ+1
E
λ+3
ˆ a
ˆ a
C
C r0λ+2 a
~
d~x · E(~x) =
dr0 r0λ+1 =
λ+3 r
λ+3λ+2 r
r
ˆ a
r

~ x) =
d~x · E(~


Caλ+2
Crλ+2
C
−
= 2
aλ+2 − rλ+2
(λ + 3)(λ + 2) (λ + 3)(λ + 2)
λ + 5λ + 6

---

### Página 92

la segunda integral es
ˆ ∞
a

~ x) =
d~x · E(~

Caλ+1
C aλ+2
=
0 a λ + 3
0 (λ + 3)

Finalmente, para r < a
φ(r) =


Caλ+1
C
aλ+2 − rλ+2
+ 2
0 (λ + 3) λ + 5λ + 6

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
 ~ 0
~ x0 ) = 2πrhE(r) = qin
x ) · E(~
 dS(~
0
S
donde la carga encerrada por la superficie S es
qin = σ2πha
σ es la densidad superficial de carga sobre el cilindro de radio a. De aquí
2πrhE(r) =

σh2πa
0

σa
~
E(r)
=
r̂
0 r
En particular

~ 0 ) = σa r̂
E(r
 0 r0

Este campo es por supuesto el responsable de la fuerza que siente un ión (en dirección
radial), y que permite la trayectoria circular. El equilibrio de fuerzas en la dirección radial
sobre un Ión de carga q es
~ 0) = q
q E(r

σa
v2
r̂ = −m r̂
 0 r0
r0

de donde
σa
2qV0
= −m
 0 r0
mr0
la densidad superficial de carga sobre el cilindro A resulta ser
q

σ=−

20 V0
a

y el campo eléctrico queda, para r, a < r < b
20 V0 a
σa
~
r̂ = −
r̂
E(r)
=
0 r
a 0 r
V0
~
E(r)
= −2 r̂
r
La diferencia de potencial entre los cilindros es
ˆ b
~ x)
∆V = φ(b) − φ(a) = −
d~x · E(~
a

tomando un camino radial

ˆ b
ˆ b 
ˆ b
dr
2V0
~
∆V = −
d~r · E(r) = −
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
~ 1 el campo eléctrico debido al plano
éste se puede obtener fácilmente por superposición. Sea E
infinito, sabemos que éste es uniforme y no depende de la distancia al plano. Para x > 0 es
~ 1 (x) = σ î
E
20
Podemos obtener el potencial asociado al plano integrando el campo eléctrico sobre una
trayectoria horizontal que pasa por Ox, entre ~x1 = xî y ~x2 = Rî (R > x)
φ1 (x) − φ1 (R) =

ˆ ~x2
~
x1

~ x0 ) =
d~x · E(~

ˆ R
x

dx0

σ
20

σ
σ
R−
x
20
20
El potencial en un punto x debido a la carga puntual −q está dado por
φ1 (x) = φ1 (R) +

φ2 (x) =
por el principio de superposición
φ(x) =

−q
4π0 | a − x |

−q
σ
σ
+ φ1 (R) +
R−
x
4π0 | a − x |
20
20

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



2e
(φ(0) − φ(a/2))
m

1 −2q
σ
1 −q
−
+
a
4π0 a
4π0 a
40

2e
vf2 =
m



q
σa
+
4π0 a 40





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

p
(x − l)2 + y 2 . Con esto

φ(P ) =
4π0

1 dlλ
4π0 r

ˆ L

dlλ
p
(x − l)2 + y 2

Sea t = x − l, con lo que dt = −dl, así
λ
φ(P ) = −
4π0

ˆ x−L
x

dtλ
p
t2 + y 2

Aquí es inmediato que se usa la sustitución t = y tan ϑ, luego dt = ysec2 ϑdϑ. Con esto
tenemos
ˆ
ˆ
ˆ
dϑsec2 ϑy
dt
p
p
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

p
x−L
λ
(ln(t + t2 + y 2 ))
4π0
x


p
p
λ 
ln(x + x2 + y 2 ) − ln(x − L + (x − L)2 + y 2 )
4π0

λ
φ(P ) = −
ln
4π0
y llamando

!
p
x + x2 + y 2
p
(x − L + (x − L2 ) + y 2 )

p
a = x2 + y 2
p
b = (x − L)2 + y 2

λ
φ(P ) = −
ln
4π0



x+a
(x − L + b)



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
 ~ ~
r) =
 dS · E(~
0
S
~ = E(r)r̂ y dS
~ = dS r̂, luego la integral de flujo del campo eléctrico es, simplemente
donde E
ˆˆ
ˆˆ
ˆˆ


 ~ ~
r) =  dSE(r)r̂ · r̂ =  dSE(r)
 dS · E(~
S

S

S

Como en la superficie S el radio r es constante
ˆˆ
ˆˆ


 dSE(r) = E(r)  dS = E(r)4πr
S

S

Por otra parte, la carga encerrada por la superficie de Gauss es
˚
d3 x0 ρ(~x0 )
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

De esta forma, y considerando d3 x0 = r2 sinϑdrdϑdφ
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
0 R 3

E(r)4πr2 =
de donde, para r < R
E(r) =

Qr
4π0 R3

Campo exterior
Ahora, para obtener el campo exterior, se construye una superficie de Gauss esférica y ahora
de radio r > R

El flujo eléctrico sobre esta superficie es, de manera análoga al caso anterior
ˆˆ

 ~ ~
 dS · E· = E(r)4πr
S

mientras que la carga encerrada en este caso está dada por
qin = Q
Con esto
E(r)4πr2 =

E(r) =

Q
0

Q
4π0 r2

En resumen, se tiene
~ x) =
E(~

(

Qr
r̂
4π0 R3
Q
r̂
4π0 r2

si | ~x |≤ R
si | ~x |> R

---

### Página 101

Notar que el campo es continuo al atravesar un volumen cargado, pero no es diferenciable
Potencial exterior
Ahora, para obtener el potencial electrostático, calculamos la integral de línea
ˆ r
~
~ · dr
φ(r) = −
E
∞

~ = drr̂, así, para r > R
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
4π0 r
4π0
∞
φ(r) =

ˆ r

dr 2
r
∞

Q
4π0 r

Potencial interior
Ahora, para r < R, tenemos
drE(r) −

ˆ r

drE(r)

Q
dr
−
φ(r) = −
4π0 r2
∞

ˆ r

dr

Qr
4π0 R3

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
4π0 R 4π0 R3
φ(r) =

Q(R2 − r2 )
Q
+
4π0 R
8π0 R3

φ(r) =

φ(r) =

R

(

Q(3R2 − r2 )
8π0 R3

Q(3R2 −r2 )
8π0 R3
Q
4π0 r

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
4π0 (z − l)

dφ(z) =

dq
4π0 (z − l)

donde dq = dlλ

dφ(z) =
con esto, el potencial total está dado por

dlλ
4π0 (z − l)

λ
φ(z) =
4π0

ˆ d

dl
−d (z − l)

sea u = z − l, luego du = −dl
λ
φ(z) = −
4π0

ˆ z−d

du
u

λ
φ(z) =
ln
4π0





z+d

z+d
z−d

---

### Página 103

b) Un electrón se mueve desde z = 4d hasta z = 3d, luego, su cambio en energía potencial
está dado por
∆U = U (4d) − U (3d) = −e (φ(4d) − φ(3d)) = eφ(3d) − eφ(4d)



λ
λ
ln2 −
ln( )
∆U = e
4π0
4π0
 
λ
∆U = e
ln
4π0
c) Por conservación de la energía
U (4d) + K(4d) = U (3d) + K(3d)
como el electrón parte del reposo, K(4d) = 0, luego
U (4d) = U (3d) + K(3d)
U (4d) − U (3d) = K(3d)
luego, el cambio de energía potencial calculado en la parte b) es equivalente a la energía
cinética que adquiere el electrón
 
λ
K(3d) = ∆U = e
ln
4π0


λ
mv 2
ln
=e
4π0
s
 
2λ
v= e
ln
4π0 m

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
1 dq(~x − ~x0 )
~
dE(P ) =
4π0 | ~x − ~x0 |3

---

### Página 105

En este caso, tenemos
~x = rr̂
donde r̂ es el vector radial en coordenadas cilíndricas que apunta desde el origen hasta el
punto P . Además
~x0 = lk̂
Luego
~x − ~x0 = rr̂ − lk̂
| ~r − ~r0 |=

√

r2 + l2

De esta forma , la contribución del elemento diferencial al campo es
~ )=
dE(P

1 λdl(rr̂ − lk̂)
4π0 (r2 + l2 )3/2

Utilizando el principio de superposición, el campo total en P será la suma de todas las
contribuciones infinitesimales de la distribución, esto es
~ )=
E(P

λ
4π0



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



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


l1
l1
l
λ
~
E(P ) =
+ k̂ √
rr̂ 2 √
4π0
r r2 + l2 −l2
r2 + l2 −l2
~ )= λ
E(P
4π0

r̂
r

l2

l1

p
+p
r2 + l12
r2 + l22

!

+ k̂

p
−p
r2 + l12
r2 + l22

!!

b) En el límite cuando r >> l1 y r >> l2 , se tiene que ( a cero orden)
q
q
r + l1 ≈ r2 + l22 ≈ r
Luego el campo queda

~ )≈ λ
E(P
4π0



r̂
r



~ )≈
E(P

l1 l2
+
r
r



+ k̂



1 1
−
r r



λ l1 + l2
r̂
4π0 r r

pero λ(l1 + l2 ) no es más que la carga total contenida en la distribución, digamos, q, luego
el campo toma la forma
q
~ ≈
r̂
E
4π0 r2
que es el campo de una carga puntual
c) Ahora, en el límite cuando l1 >> r y l2 >> r, se tiene que
q
r2 + l12 ≈ l1
q
r2 + l22 ≈ l2

y el campo queda
~ )≈
E(P

λ 2
( r̂ + k̂( − ))
4π0 r
l1 l2

y si l1 → ∞, l2 → ∞, se tiene
λ
r̂
2π0 r
que es el campo eléctrico de un alambre infinito de carga.
~ )≈
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
 ~
~
dS r̂E(r)r̂ = E(r)
dS = E(r)2πrl
 dS · dE =
S

manto

manto

la carga encerrada por este cilindro es qin = λl, luego
E(r)2πrl =
E(r) =

λl
0

λ
2πr0

El mismo resultado obtenido anteriormente
d) El campo del alambre infinito está dado por
~
E(r)
=

λ
r̂
2πr0

Sabemos que en electrostática se cumple
~
~
E(r)
= −∇φ(r)
Debido a la simetría, el potencial será sólo función de r, luego
dφ
~
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
2π0

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
2π0

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
2π0
y el potencial debido al alambre de densidad −λ es
φ1 (P ) =

λ
ln s− + C2
2π0

Ahora, como nos piden que la referencia sea el origen, las constantes C1 y C2 deben satisfacer
φ1 (a) = 0 = φ2 (a)
Con esto
φ1 (a) = −
φ2 (a) =

λ
λ
ln a + C1 = 0 → C1 =
ln a
2π0
2π0

λ
λ
ln a + C2 = 0 → C2 = −
ln a
2π0
2π0

Notar que C1 + C2 = 0.

---

### Página 110

El potencial en el punto P es
φ(P ) = φ1 (P ) + φ2 (P ) = −

λ
λ
ln s+ +
ln s−
2π0
2π0

Si P = (x, y, z), entonces
p
(y − a)2 + z 2
p
s+ = (y + a)2 + z 2

s+ =
Finalmente, el potencial es
φ(P ) = +

p
p
λ
λ
ln( (y + a)2 + z 2 ) −
ln( (y − a)2 + z 2 )
2π0
2π0
!
p
(y
+
a)
+
z
λ
φ(P ) =
ln p
2π0
(y − a)2 + z 2
λ
ln
φ(P ) =
4π0



(y + a)2 + z 2
(y − a)2 + z 2



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
Un dipolo con momento dipolar p~ se localiza a una distancia r de una barra muy delgada con
largo infinito y homogéneamente cargada con densidad lineal de carga λ > 0. Asuma que el
dipolo está orientado con el campo eléctrico debido a la barra cargada como muestra la figura

a) Suponiendo que la separación fija l entre las cargas que conforman el dipolo es tal que
l << r, determine la fuerza sobre el dipolo, a primer orden en l/r
b) Partiendo de la respuesta del inciso anterior, demuestre que la fuerza sobre el dipolo puede
ser escrita como


~
~
~ x)
F (~x) = p~ · ∇ E(~
(válido para un dipolo puntual)

#### Solución
Ya fue obtenido anteriormente el campo eléctrico de una distribución lineal de carga muy larga
y de densidad λ. Definiendo un sistema de coordenadas cilíndricas, donde el eje z coincide con
el eje de la barra, como se ve en la figura

El campo eléctrico creado por la barra está dado por
~
E(r)
=

λ
r̂
2π0 r

La fuerza sobre el dipolo está dada por
~ + l/2) − q E(r
~ − l/2) = q (E(r + l/2) − E(r − l/2)) r̂
F~ = q E(r

r̂
−
r + l/2 r − l/2
!
qλ
r̂
F~ =
−
2π0 r 1 + 2rl
1 − 2rl

qλ
F~ =
2π0



---

### Página 113

qλ
F~ =
2π0 r



l
1+
2r

−1



l
− 1−
2r

−1 !

r̂

Recordar la expansión a primer orden de (1 + x)n , buena aproximación cuando x << 1
(1 + x)n ≈ 1 + nx
De esta forma, la fuerza se puede aproximar (en primer orden de l/r)



qλ
l
l
~
F ≈
1−
r̂
− 1+
2π0 r
2r
2r
 
l
qλ
~
−
r̂
F ≈
2π0 r
r
−qlλ
−pλ
F~ ≈
r̂
=
r̂
2π0 r2
2π0 r2
donde p es la magnitud del momento dipolar del dipolo
b) Notar que si l << r, se espera obtener para la fuerza el resultado que se obtuvo para el
dipolo puntual


~ E(~
~ x)
F~ (~x) = p~ · ∇
Utilizando coordenadas cilíndricas, y recordando la naturaleza radial del campo eléctrico




∂
~
~
~
~
F (r) = p~ · ∇ E(r) = pr̂ · r̂ E(r)
∂r




λ
∂
∂ ~
~
r̂
E(r) = p
F (r) = p
∂r
∂r 2π0 r

λ
r̂
2π0 r2
que es el mismo resultado que se obtuvo en la parte anterior
F~ (r) = −p

---

### Página 114

Problema
Considere un dipolo de momento dipolar p~ formando un ángulo ϑ con la horizontal. Suponga
~ = E x̂.
que existe un campo eléctrico externo uniforme dado por E
a) Calcule la fuerza total y explícitamente el torque que se ejerce sobre el dipolo
b) ¿Qué ocurre si el campo no es uniforme?

#### Solución
Como se aprecia en la figura, se tiene que la fuerza total sobre el dipolo será
F~ = F~+ + F~−
F~ = qE î − qE î = ~0
La fuerza neta sobre el dipolo en un campo externo uniforme es nula. Calculemos ahora el
torque que se ejerce sobre el dipolo, con respecto a su centro de masa(origen)
~τ = ~r+ × F~+ + ~r− × F~−
~τ = (a cos ϑî + a sin ϑĵ) × qE î + (−acosϑî − a sin ϑĵ) × −qE î
~τ = a sin ϑĵ × qE î + a sin ϑĵ × qE î
~τ = 2a sin ϑĵ × qE î = −2aqsinϑE k̂
Existe un torque sobre el dipolo, a pesar que la fuerza neta sobre él es nula! La dirección del
torque es según −k̂ (hacia dentro de la página). Es decir, el dipolo tiende a girar en el sentido
del reloj de forma que el dipolo se alinea con respecto al campo. (Deja de haber torque cuando
p~ y Ê son paralelos). Ahora, la magnitud del momento dipolar es
p = 2aq
Luego, se puede reescribir
~τ = −pEsinϑk̂
Escrito en forma más general, se tiene
~
~τ = p~ × E
que es consistente con la expresión general para el torque sobre un dipolo de momento dipo~
lar p~ situado en un campo eléctrico E.

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
φ(~x) =
4π0

dx0 λ
x − ~x0 |
Γ |~

˛

interesa obtener el potencial para ~x = z k̂. La parametrización de la distribución de carga
está dada por
~x0 = Rr̂(ϑ)
r̂(ϑ) = cos ϑî + sin ϑĵ
dx = Rdϑ
Luego
φ(z) =
4π0
y la densidad lineal es

ϑ : 0 → 2π
ˆ 2π

dϑ √

λR
z 2 + R2

=

λR
√
20 z 2 + R2

q
2πR
q
√
φ(z) =
4π0 z 2 + R2
λ=

Consideremos ahora dos anillos separados una distancia 2a

---

### Página 117

El potencial sobre un punto a distancia z del origen es
φ(z) =
donde

q
q
p1
p2
+
4π0 z12 + R2 4π0 z22 + R2
z2 = z

z1 = z − 2a
φ(z) =
Además se tiene

q
q1
p
√2
+
4π0 (z − 2a)2 + R2 4π0 z 2 + R2


q2
q1
√
+
W1 = qφ(2a) = q
4π0 R 4π0 4a2 + R2


q1
q2
√
W2 = qφ(0) = q
+
4π0 4a2 + R2 4π0 R


De aquí se puede resolver para q1 y q2
√
√

π0 R 4a2 + R2 W1 4a2 + R2 − W2 R
q1 =
qa2
√
√

π0 R 4a2 + R2 W2 4a2 + R2 − W1 R
q2 =
qa2

---

### Página 118

Problema
Muestre que la energía potencial almacendada en una esfera sólida cargada uniformemente con
carga Q y de radio R es


Q2
U=
5 4π0 R
#### Solución
De la forma general para la energía potencial de una distribución de carga
˚
U=
d3 x0 ρ(~x0 )φ(~x0 )
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
8π0 R3

ˆ R
3Q
2 Q(3R − r )
drr
U = 4π
8πR3 0
8π0 R3


ˆ R
3Q2
3Q2
R5
R −
U=
drr (3R − r ) =
16π0 R6 0
16π0 R6

U=

4 5 3 Q2
3Q2
×
R =
16π0 R6 5
5 4π0 R

---

### Página 119

Problema
Una distribución de fuentes localizadas en un volumen V se define como

ρ(~x) si ~x ∈ V
ρ=
si ~x ∈
/V
Demuestre que en primera aproximación en la magnitud de V (diámetro máximo), el campo
eléctrico distante debido a fuentes localizadas en V , puede descomponerse en
~ x) =
E(~

 ~x
~x
1 
~
q(V )
−
p
~
(V
)
·
∇
4π0
| ~x |3 4π0
| ~x |3

donde

˚

d3 x0 ρ(~x0 )

˚

d3 x0 ρ(~x0 )~x0

q(V ) =

V

es la carga total de la distribución, y
p~(V ) =

V

es el momento dipolar de la distribución
#### Solución
Pondremos el origen ~0 ∈ V , con lo que por campo distante estamos pensando en
| ~x |>>| ~x0 |, ~x0 ∈ V
es decir, la distancia a la distribución es mucho mayor que las dimensiones de ésta

El campo está dado por la integral de Coulomb
˚
˚
~x − ~x0
~x − ~x0
3 0
3 0
~
=
E(~x) =
d x ρ(~x )
d
x
ρ(~
x
)
4π0
| ~x − ~x0 |
4π0
| ~x − ~x0 |
R3
V
Ahora, utilizaremos la siguiente expansión en Taylor


~ f~(~x) + O(2)
f~(~x − ~x0 ) = f~(~x) − ~x0 · ∇

de forma que


 ~x
~x − ~x0
~x
0 ~
=
−
~
x
·
∇
+ O(2)
| ~x − ~x0 |
| ~x |3
| ~x |3

---

### Página 120

Así
~ x) =
E(~

~ x) ≈ 1
E(~
4π0

4π0

˚

~x − ~x0
d x ρ(~x )
| ~x − ~x0 |3
V

˚

3 0




 ~x
~x
0 ~
− ~x · ∇
| ~x |3
| ~x |3

3 0

q(V ) =

˚

d3 x0 ρ(~x0 )

˚

d3 x0 ρ(~x0 )~x0

d x ρ(~x )

V

definiendo



V

p~(V ) =

V

queda
~ x) ≈
E(~

 ~x
~x
1 
~
p
~
(V
)
·
∇
q(V )
−
4π0
| ~x |3 4π0
| ~x |3

Notar que el primer término corresponde al campo creado por una carga puntual q(V ) en
el origen. Por supuesto ésta sería la aproximación a cero orden del campo, en donde esperamos
obtener la ley de Coulomb. El segundo término de esta expansión, equivale al campo eléctrico
generado por un dipolo puntual p~(V ) en el origen.
Esta expansión del campo se conoce como Expansión Multipolar, y se verá con más detalle
un poco más adelante (de hecho, en la próxima página).

---

### Página 121

5.7.

Expansión Multipolar

Consideraremos una fuente localizada caracterizada por la siguiente densidad de carga

ρ(~x) si ~x ∈ V
ρ=
si ~x ∈
/V
El potencial está dado por
φ(~x) =
4π0

˚

d3 x0

V

donde

ρ(~x0 )
| ~x − ~x0 |


1/2
| ~x − ~x0 |= ~x2 + ~x02 − 2~x · ~x0

entonces

=
| ~x − ~x |
| ~x |

−1/2

~x · ~x0
~x02
1+ 2 −2 2
~x
~x

Recordando la expansión en taylor

13 2
(1 + z)−1/2 = 1 − z +
z + O(3)
y la expansión hasta segundo orden es
≈
| ~x − ~x |
| ~x |

{1 −


2 )
 02

~x · ~x0
~x · ~x0
3 ~x02
~x
−2 2
−2 2
+
~x2
~x
8 ~x2
~x

#)
" 

2
(~x · ~x0 )~x02
~x · ~x0
~x · ~x0 1 ~x02 3
~x02
+
+4
−4
1+ 2 −
~x
2 ~x2
~x2
~x2
~x4
(
"

2
3 #)
~x · ~x0 1 ~x02 3 ~x · ~x0
| ~x0 |
1+ 2 −
=
+
+O
| ~x |
~x
2 ~x2
~x2
| ~x |

=
| ~x |

(

Con esto, la expansión del potencial electrostático a segundo orden es
˚
˚
~x
1 1
3 0
φ(~x) =
d x ρ(~x ) +
·
d3 x0 ρ(~x0 )~x0
4π0 | ~x |
4π0 | ~x |
V
V
˚
 0 0
1 1 xi xj
3 0
3xi xj − δij | ~x0 |2 ρ(~x0 ) + ...
+
d
x
4π0 2 | ~x |
V
Se define el momento monopolar (escalar)
˚
d3 x0 ρ(~x0 )
q=
V

que es la carga total de la distribución. Además
˚
p~ =
d3 x0 ρ(~x0 )~x0
V

es el momento dipolar (vector) de la distribución.

---

### Página 122

~ =
Q

˚

V

n
o
d3 x0 ρ(~x0 ) 3~x0 · ~x0T − I~ ~x0T · ~x0

es el momento cuadripolar (tensor)
˚

d3 x0 ρ(~x0 ) 3x0i x0j − δij | ~x0 |2
Qij =
V

la expansión queda

φ(~x) =
4π0

!
~ · ~x
p~ · ~x
1 ~xT · Q
q
+
+
+ ...
| ~x | | ~x |3 2 | ~x |5

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
 ~
~
x) · E(~x) =
d3 xρ(~x)
 dS(~

S
V
y la ley de circulación del campo eléctrico
˛
~ x) = 0
d~x · E(~
Γ

Éstas dos ecuaciones integrales entregan información global acerca del campo. Sin embargo,
es posible llevarlas a su forma más simple en un par de ecuaciones diferenciales para el campo
electrostático.
A partir de la ley de Gauss, y utilizando el teorema de la divergencia, se obtiene
ˆˆ
˚
˚
 ~ ~
3 ~
~
x) =
d x∇ · E(~x) =
d3 xρ(~x)
 dS · E(~

S
V
V


~ · E(~
~ x) − ρ(~x)
dx ∇
0
V

˚



=0

esto es independiente del volumen V de integración. Consecuencia de esto es que
~ · E(~
~ x) = ρ(~x)
∇
0
Del mismo modo, a partir de la ley de circulación y utilizando el teorema de Stokes
¨
˛


~ × E(~
~ x) = 0
~
~ x) · ∇
d~x · E(~x) =
dS(~
Γ

S(Γ)

para cualquier superficie cuyo contorno sea Γ. De aquí se desprende que
~ × E(~
~ x) = 0
∇

---

### Página 124

En resumen, las dos leyes integrales fundamentales del campo electrostático tienen una
formulación equivalente en dos ecuaciones diferenciales para el campo
~ · E(~
~ x) = ρ(~x)
∇
0
~ × E(~
~ x) = 0
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
~2
∇

= −4πδ(~x − ~x0 )
| ~x − ~x |

#### Solución
Sea V (S) un volumen en R3 y S = δV su contorno. Sea además una carga puntual q en el
punto ~x0 , es sabido que el campo electrostático creado por esta carga es
~ x) =
E(~

~x − ~x0
q
4π0 | ~x − ~x0 |3

La ley de Gauss establece
ˆˆ
˚
q  ~
~x − ~x0
x) ·
=
d3 xqδ(~x − ~x0 )
 dS(~
4π0 S
| ~x − ~x0 |3
0
V
o equivalentemente

~x − ~x0
= 4π
| ~x − ~x0 |3

ˆˆ

 ~
x) ·
 dS(~
S

˚

V

d3 xδ(~x − ~x0 )

Utilizando el teorema de la divergencia
˚
ˆˆ
~x − ~x0
~x − ~x0
 ~
3 ~
d
S(~
x
)
·
=
d
x
∇
·

| ~x − ~x0 |3
| ~x − ~x0 |3
S
V
y recordando que

~x − ~x0
=−
| ~x − ~x0 |
| ~x − ~x0 |3
ˆˆ
˚
~x − ~x0
 ~
~ ·∇
~
x) ·
=−
d3 x∇
 dS(~
| ~x − ~x |
| ~x − ~x0 |
S
V
ˆˆ
˚
˚
~x − ~x0
 ~
3 ~2
x) ·
=−
d x∇
d3 xδ(~x − ~x0 )
= 4π
 dS(~
0 |3
0 |
|
~
x
−
~
x
|
~
x
−
~
x
S
V
V
~
∇

luego

˚

V



~2
dx ∇

Finalmente
~2
∇


+ 4πδ(~x − ~x )
| ~x − ~x0 |

= −4πδ(~x − ~x0 )
| ~x − ~x0 |

---

### Página 126

6.1.

Completitud de la teoría Electrostática

6.1.1.

Descomposición de Helmhotz

~ x) un campo vectorial tal que
Sea A(~
ˆˆ




S(∞)

~ x0 ) ·
dS(~

~ x0 )
A(~
=0
| ~x0 − ~x |

definamos los campos
~ L (~x) = − 1 ∇
~
A
4π

˚

d3 x0

R3

~ T (~x) = 1 ∇
~ ×∇
~ ×
A
4π

˚

~ x0 )
~ 0 · A(~
∇
| ~x − ~x0 |

d3 x0

R3

entonces se cumple

~ x0 )
A(~
| ~x − ~x0 |

~ T (~x)
~ x) = A
~ L (~x) + A
1)A(~
~ ×A
~ L (~x) = 0
2)∇
~ ·A
~ T (~x) = 0
3)∇

~
~ L (~x) se llama parte longitudinal (irrotacional) de A
A
~ T (~x) se lama parte transversal (solenoidal) de A
~
A
Demostración del teorema de Helmhotz
1) Utilizando la identidad
~ · (f~g) = g ∇
~ · f~ + f~ · ∇g
~
∇
se tiene
~0·
∇
de forma que

~ x0 )
~ 0 · A(~
~ x0 )
A(~
∇
~0
~ x0 ) · ∇
=
+ A(~
| ~x − ~x |
| ~x − ~x |
| ~x − ~x0 |

˚
~ 0 ~ x0 ) ˚
~ x0 )
A(~
3 0 ∇ · A(~
3 0~ 0
~0
~ x0 ) · ∇
dx
d x∇ ·
d3 x0 A(~
=
−
| ~x − ~x |
| ~x − ~x |
| ~x − ~x0 |
R3
R3
R3

˚

˚
~ 0 ~ x0 ) ˆˆ 
~ x0 )
A(~
3 0 ∇ · A(~
~
~
~ x0 ) · ∇
=   dS(~x ) ·
+
dx
d3 x0 A(~
| ~x − ~x |
| ~x − ~x |
| ~x − ~x0 |
R3
S(∞)
R3

˚

en este último paso hemos utilizado el teorema de la divergencia y el hecho que
~0
∇

~
= −∇
| ~x − ~x |
| ~x − ~x0 |

utilizando la hipótesis del teorema
˚
~ 0 ~ x0 ) ˚
~ x0 )
3 0 ∇ · A(~
3 0~ 0
3 0 A(~
~
~
dx
d x A(~x ) · ∇
dx
=
=∇·
| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
R3
R3
R3

˚

---

### Página 127

por lo tanto
~ x0 )
A(~
| ~x − ~x0 |
R3
Ahora ocupamos la siguiente identidad (muy utilizada en teoría electromagnética)
~ L (~x) = −∇
~∇
~ ·
4π A

˚

d3 x0

~ ×∇
~ × f~ = ∇
~∇
~ · f~ − ∇
~ 2 f~
∇
˚
~ x0 )
~ x0 )
A(~
3 0 A(~
~
x
−
∇
dx
d
| ~x − ~x0 |
| ~x − ~x0 |
R3
R3
˚
~
~
~2
~ x0 )∇
4π AL (~x) = −4π AT (~x) −
d3 x0 A(~
| ~x − ~x0 |
R3
por último, utilizando el teorema
~ ×∇
~ ×
~ L (~x) = −∇
4π A

˚

3 0

= −4πδ(~x − ~x0 )
| ~x − ~x0 |
˚


~ x0 )δ(~x − ~x0 )
~
~
d3 x0 A(~
4π AL (~x) + AT (~x) = 4π
~2
∇

R3

y se demuestra que

~ T (~x)
~ x) = A
~ L (~x) + A
A(~

~ ×∇
~
~ ×A
~ L (~x) = ∇
b) − 4π ∇

˚

R

~ 0 ~ x0 )
3 0 ∇ · A(~
= ~0
dx
| ~x − ~x0 |

~ ×A
~ L (~x) = 0
∇

~ ·A
~ T (~x) = ∇
~ ·∇
~ ×∇
~ ×
c)4π ∇

˚

R3

d3 x0

~ x0 )
A(~
=0
| ~x − ~x0 |

~ ·A
~ T (~x) = 0
∇
Observación
La validez del teorema de Helmhotz es
ˆˆ



S(∞)

~ x0 ) ·
dS(~

~ x0 )
A(~
=0
| ~x − ~x0 |

Podemos escoger esta superficie como una esfera centrada en ~x y de radio a, con a → ∞
ˆˆ
ˆˆ
~ x0 )
~ x0 )
x0 ) · A(~
A(~


0 n̂(~
~
x)·
dS(~
x
)
=
lím


  dS(~
| ~x − ~x0 | a→∞ S(~x,a)
| ~x − ~x0 |
S(∞)
sobre la superficie

---

### Página 128

~x0 − ~x = an̂(~x0 )
| ~x − ~x0 |= a

dS(~x0 ) = a2 dΩ(~x)
donde dΩ(~x) = sin2 ϑdϑdφ es el elemento de ángulo sólido con vértice en ~x
ˆ 4π
~ x0 )
~ x0 ) |
A(~
x0 ) · A(~
2 | n̂(~
~
dS(~x ) ·
dΩ(~x) lím a
≤
a→∞
| ~x − ~x0 |
a
S(∞)

ˆˆ




ˆˆ




S(∞)

~ x0 ) ·
dS(~

ˆ 4π
ˆ 4π
~ x0 )
A(~
~
~ x0 ) |
≤
dΩ(~x) lím a | n̂(~x ) · A(~x ) |=
dΩ lím
| ~x − ~x0 || A(~
0 |→∞
a→∞
|~
x
| ~x − ~x0 |
=

ˆ 4π

~ x0 ) |
dΩ lím | ~x0 || A(~
|~
x|→∞

por lo tanto
ˆˆ

~
lím | ~x || A(~x) |= 0 →  

|~
x|→∞

S(∞)

~ x0 ) ·
dS(~

~ x0 )
A(~
=0
| ~x − ~x0 |

A continuación, demostraremos dos teoremas que nos permitirán escribir el teorema de
Helmhotz de una forma más conveniente
Teorema 1
˚
ˆˆ

3 ~
~ x)ψ(~x)
d x∇ψ(~x) =   dS(~
V

S(V )

Demostración
Ustamos el teorema de la divergencia
ˆˆ
˚

3 ~
~ x) = 
d x∇ · A(~

V

S(V )

~ x) · A(~
~ x)
dS(~

~ x) = Bψ(~
~ x), con B
~ un vector constante arbitrario
con A(~
˚
˚
˚
3 ~
3 ~ ~
~
~
~ x)
d x∇ · Bψ(~x) =
d xB · ∇ψ(~x) = B ·
d3 x∇ψ(~
V

˚

V

V

ˆˆ


~ · Bψ(~
~ x) = 
d3 x∇


S(V )

~·
B

˚

V

V

ˆˆ


~ x) · Bψ(~
~ x) = B
~· 
dS(~


~ x)ψ(~x)
dS(~

S(V )

ˆˆ

~
d x∇ψ(~x) −  

S(V )


~
dS(~x)ψ(~x) = 0

---

### Página 129

~ fue escogido de forma arbitraria
como B
˚
ˆˆ

3 ~
d x∇ψ(~x) =  
V

~ x)ψ(~x)
dS(~

S(V )

Teorema 2
˚

~ × A(~
~ x) =  
d x∇

V

Demostración
˚


S(V )

~ x) × A(~
~ x)
dS(~

˚
˚

~
~
~ b Ac
~
d x ∇×A =
d xabc ∇b Ac = abc
d3 x∇


V

ˆˆ

a

V

V

pero del teorema anterior

~ aψ =  
d x∇

˚





ˆˆ

~ ×A
~
dx ∇

V



V

así

ˆˆ

˚

a

dSa ψ

S(V )


= abc  

=

S(V )

ˆˆ




S(V )



ˆˆ



dSb Ac =  

abc dSb Ac

S(V )

~ ×A
~
dS



a

~ x) como
Con este teorema, podemos escribir la parte transversal de A(~
~ ×
~ T (~x) = 1 ∇
A
4π

˚

d3 x0

R3

En efecto, consideremos
~ ×
∇
˚

R3

˚
~ x0 )
A(~
3 0~ 0
~
x
)
×
∇
A(~
x
=
−
dx
d
| ~x − ~x0 |
| ~x − ~x0 |
R3
R3

˚

~0
d x A(~x ) × ∇
3 0~

~ x0 )
~ 0 × A(~
∇
| ~x − ~x0 |

3 0

=
| ~x − ~x0 |

~ x0 )
~ 0 ~ x0 ) ˚
A(~
3 0 ∇ × A(~
3 0~ 0
x
×
∇
−
dx
d
| ~x − ~x0 |
| ~x − ~x0 |
R3
R3

˚

~ 0 ~ x0 ) ˆˆ 
~ x0 )
A(~
3 0 ∇ × A(~
~
−
dx
d
S(~
x
)
×

| ~x − ~x0 |
| ~x − ~x0 |
R3
S(∞)

˚

pero si se cumple la hipótesis del teorema de Helmhotz
ˆˆ

~ x) |= 0 →  
lím | ~x || A(~


|~
x|→∞

luego
~ ×
∇

S(∞)

~ x0 ) ×
dS(~

~ x0 )
A(~
= ~0
| ~x − ~x0 |

˚
~ x0 )
~ 0 ~ x0 )
A(~
3 0 ∇ × A(~
dx
dx
=
| ~x − ~x0 |
| ~x − ~x0 |
R3
R3

˚

3 0

---

### Página 130

y entonces

6.1.2.

˚
~ x0 )
1 ~
A(~
~
~
AT (~x) =
∇×∇×
d3 x0
4π
| ~x − ~x0 |
R3
˚
~ x0 )
~ 0 × A(~
1 ~
∇
~
∇×
d3 x0
AT (~x) =
4π
| ~x − ~x0 |
R3

Teorema de Helmhotz, segunda forma

~ es un campo vectorial tal que
Si A
~ x) |= 0
lím | ~x || A(~

|x|→∞

entonces

~ T (~x)
~ x) = A
~ L (~x) + A
A(~

con
~ L (~x) = − 1 ∇
~
A
4π

˚

d3 x0

~ x0 )
~ 0 · A(~
∇
| ~x − ~x0 |

~ T (~x) = 1 ∇
~ ×
A
4π

˚

d3 x0

~ x0 )
~ 0 × A(~
∇
| ~x − ~x0 |

donde

R3

R3

~ ×A
~ L (~x) = 0
∇
~ ·A
~ T (~x) = 0
∇

6.1.3.

Corolario del Teorema de Helmhotz

Dadas la divergencia

~ · A(~
~ x) = 4πD(~x)
∇

y el rotor

~ × A(~
~ x) = 4π R(~
~ x)
∇

~ x), sobre todo el espacio, entonces ese campo vectorial está comde un campo vectorial A(~
pletamente determinado en todos los puntos del espacio mediante la siguiente representación
integral- diferencial
~ x) = −∇
~
A(~

D(~x0 )
~ ×
+∇
dx
0 |
|
~
x
−
~
x
R

˚

3 0

˚

R3

d3 x0

~ x)
R(~
| ~x − ~x0 |

~ x) y R(~
~ x) nos son dadas, son las fuentes del campo A(~
~ x).
Observación: las funciones D(~
Pero
n
o
~ = {D, Rx , Ry , Rz }
D, R
son 4 funciones, mientras que

n o
~ = {Ax , Ay , Az }
A

---

### Página 131

son 3 funciones. Sin embargo, no hay sobredeterminación pues


~ ×A
~ = 4π ∇
~ ·R
~ =0
~ · ∇
∇
~ debe ser solenoidal
luego R

~ · R(~
~ x) = 0
∇

esto agrega 1 condición. Con esto, la construcción de Helmhotz define un problema bien
determinado

6.2.

Completitud de la Electrostática

Hemos encontrado que
~ · E(~
~ x) = ρ(~x)
∇
0
~ × E(~
~ x) = ~0
∇
El teorema de Helmhotz nos dice que , dadas la divergencia y el rotor del campo eléctrico,
este esta absolutamente determinado por la forma integral
˚
1 ~
ρ(~x0 )
~
E(~x) = −
d3 x0
∇
4π0
| ~x − ~x0 |
R3
y la electrostática es una teoría completa: el conjunto de ecuaciones diferenciales que representan las leyes fundamentales de la teoría es suficiente para determinar completamente el
campo electrostático

---

### Página 132

Problema
La descomposición de Helmholtz requiere que
~ x) |= 0
lím | ~x || A(~

|~
x|→∞

demuestre que
˚

R3

n
o
~ x) | < ∞
d3 x | D(~x) | + | R(~

es condición suficiente para la validez de la representación integro-diferencial de Helmholtz
#### Solución
~ x) = −∇
~
A(~
Entonces

≤| ~x |
≤| ~x |

˚

R3

R3

~
d x D(~x )∇
3 0

~ x0 )
R(~
| ~x − ~x0 |

D(~x0 )
~ ×
+∇
dx
0 |
|
~
x
−
~
x
R

˚

d3 x0

˚

R3

3 0

+ | ~x |
| ~x − ~x0 |

˚

R3

R3

~ x0 )
R(~
| ~x − ~x0 |

~
~ x0 ) × ∇
d3 x0 R(~

| ~x − ~x0 |

~x − ~x0
3 0
~ x0 ) || ~x − ~x |
|
+
|
~
x
|
x
|
R(~
d
| ~x − ~x0 |3
| ~x − ~x0 |3
R3
˚
o
| ~x | n
~ x0 ) |
d3 x0
|
D(~
x
=
)
|
+
|
R(~
| ~x − ~x0 |2
R3

˚

d3 x0 | D(~x0 ) ||

Luego

˚

~ x) |≤ lím
lím | ~x || A(~

|~
x|→∞

|~
x|→∞

=

˚

R3

si

d3 x0

3 0

~
~ x) |=| ~x | −∇
| ~x || A(~
˚

˚

D(~x0 )
~ ×
+∇
dx
0 |
|
~
x
−
~
x
R

˚

o
| ~x | n
~ x0 ) |
|
D(~
x
)
|
+
|
R(~
| ~x − ~x0 |2

| ~x |
|~
x|→∞ | ~
x − ~x0 |2
n
o
3 0
~
d x | D(~x ) | + | R(~x ) | = 0

n
o
~ x0 ) | lím
d3 x0 | D(~x0 ) | + | R(~

= lím
|~
x|→∞ | ~
x|
0<

R3

d3 x0

˚

˚

R3

R3

o
n
~
d x | D(~x ) | + | R(~x ) | < ∞
3 0

---

### Página 133

Problema
Demuestre que si
lím | ~x || D(~x) |= 0

|~
x|→∞

y

~ x) |= 0
lím | ~x || R(~

|~
x|→∞

entonces la representación de Helmholtz puede escribirse
~ x) = −
A(~

˚

d3 x0

R3

~ 0 × R(~
~ x0 )
~ 0 D(~x0 ) − ∇
∇
| ~x − ~x0 |

#### Solución
De la representación de Helmholtz
~ x) = −∇
~
A(~
~ x) =
A(~

˚

3 0

+
| ~x − ~x0 |

~0
d x D(~x )∇
3 0

R3

D(~x0 )
~
+∇
dx
0 |
|
~
x
−
~
x
R

˚

˚

˚

R3

d3 x0

R3

~ x0 )
R(~
| ~x − ~x0 |

~0
~ x0 ) × ∇
d3 x0 R(~

| ~x − ~x0 |

˚
~ 0 x0 ) ˚
~ 0 ~ x0 ) ˚
~ x0 )
x0 )
R(~
3 0 ∇ D(~
3 0 ~ 0 D(~
3 0 ∇ × R(~
3 0~ 0
+
+
−
dx
d
d
d
x
x
x
×
∇
∇
| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
R3
R3
R3
R3

~ x) = −
A(~

˚

~ x) = −
A(~

˚

ˆˆ
˚
~ x0 )
~0
~ 0 ~ x0 ) ˆˆ 
D(~x0 )
R(~
x0 )  
3 0 ∇ · D(~
3 0 ∇ × R(~
~
~
d
S(~
x
)
x
d
S(~
x
)×
+
+
−
dx
d


| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
R3
S(∞)
R3
S(∞)
~ x) = −
A(~

En efecto

˚

R3

d3 x0

~ 0 × R(~
~ x0 )
~ 0 D(~x0 ) − ∇
∇
| ~x − ~x0 |
D(~x0 )
=0
| ~x − ~x0 |

ˆˆ

lím | ~x || D(~x) |= 0 →  

~ x0 )
dS(~

ˆˆ

~
lím | ~x || R(~x) |= 0 →  

~ x0 ) ×
dS(~



|~
x|→∞

|~
x|→∞

S(∞)

S(∞)

~ x0 )
R(~
=0
| ~x − ~x0 |

---

### Página 134

6.3.

Apendice: Descomposición de Helmholtz en un volumen finito

~ x) satisface idénticamente la siguiente relación
Se demuestra que cualquier campo vectorial A(~
~ x) = − 1 ∇
~
A(~
4π

˚
~ 0 ~ x0 )
~ 0 ~ x0 )
1 ~
3 0 ∇ · A(~
3 0 ∇ × A(~
dx
d
x
∇
×
+
| ~x − ~x0 |
4π
| ~x − ~x0 |
V
V

˚





ˆˆ
ˆˆ
~x0 − ~x
1 
~x0 − ~x
1 
~
~
~ x0 )
~
+
dS(~x ) · 0
dS(~x ) × 0
× A(~
A(~x ) +


4π S(V )
| ~x − ~x |3
4π S(V )
| ~x − ~x |3
donde V es cualquier región cerrada, δV = S(V ) es su frontera, y ~x ∈ V
Demostración
Tenemos
˚
˚
˚
~ 0 ~ x0 )
~ x0 )
A(~
3 0 ∇ · A(~
3 0~ 0
3 0~ 0
~
=
−
+
dx
d
x
)
·
∇
d
x
·
A(~
x
∇
| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
V
V
V
ˆˆ
~ 0 ~ x0 ) ˚
~ 0

3 0 ∇ · A(~
3 0~ 0
~
~ x0 ) · A(~x )
=
+
dx
d
x
)
·
∇
d
S(~
A(~
x


| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
V
V
S(V )

˚

˚
ˆˆ
~ x0 )
~ 0 ~ x0 )
~ 0

3 0 ∇ · A(~
3 0 A(~
~
~ x0 ) · A(~x )
=
∇
·
+
dx
d
x
d
S(~


| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
V
V
S(V )

˚
con esto
~
∇

˚
ˆˆ
~ 0 ~ x0 )
~ x0 )
~ 0

3 0 ∇ · A(~
3 0 A(~
~
~
~
~ x0 ) · A(~x )
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
S(~


| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
V
V
S(V )

˚

y utilizando la identidad



~ ∇
~ ·A
~ =∇
~ ×∇
~ ×A
~+∇
~ 2A
~
∇
~
∇

˚
˚
ˆˆ
~ x0 )
~ x0 )
~ 0 ~ x0 )
A(~
A(~

3 0 ∇ · A(~
~ x0 )·A(~
~ x0 )∇
~ ∇×
~
~
dx
dx
dx
= ∇×
+∇
+   dS(~
| ~x − ~x |
| ~x − ~x |
| ~x − ~x |
| ~x − ~x0 |
V
V
V
S(V )

˚

˚
ˆˆ
~ x0 )
A(~

3 0~ 0 ~2
~ x0 ) · A(~
~ x0 ) ~x − ~x
dx
d
x
)
∇
d
S(~
A(~
x
+
−


| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |3
V
V
S(V )

~ ×∇
~ ×
=∇

˚

~ ×∇
~ ×
=∇

˚

3 0

˚
ˆˆ
~ x0 )
A(~

3 0~ 0
~ x0 ) · A(~
~ x0 ) ~x − ~x
−
4π
dx
d
x
)δ(~
x
−
~
x
)
+
d
S(~
A(~
x


| ~x − ~x0 |
| ~x0 − ~x |3
V
V
S(V )
3 0

Luego si ~x ∈ V
~
~ x) = − 1 ∇
A(~
4π

ˆˆ
˚
~ 0 ~ x0 ) 1
~ x0 )
1 
3 0 ∇ · A(~
3 0 A(~
~ x0 )·A(~
~ x0 ) ~x − ~x
~
~
dx
d
x
d
S(~
∇×
∇×
+
+


| ~x − ~x0 | 4π
| ~x − ~x0 | 4π S(V )
| ~x − ~x0 |3
V
V

˚

---

### Página 135

Ahora bien

~ ×
∇

˚
˚
~ x0 )
A(~
3 0~ 0
~
~0
~ x0 ) × ∇
dx
d x A(~x ) × ∇
d3 x0 A(~
=−
=
| ~x − ~x |
| ~x − ~x |
| ~x − ~x0 |
V
V
V

˚

3 0

˚
~ x0 )
~ 0 ~ x0 ) ˚
~ x0 )
A(~
A(~
3 0 ∇ × A(~
3 0~ 0
=
−
dx
d
x
d
x
×
∇
| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
V
V
V
˚
˚
~ x0 )
~ 0 ~ x0 ) ˆˆ 
~ 0
3 0 A(~
3 0 ∇ × A(~
~
~ x0 ) × A(~x )
∇×
=
−
dx
d
x
d
S(~


| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
V
V
S(V )
˚

~ ×
∇

3 0

Luego
˚
ˆˆ
~ x0 )
~ 0 ~ x0 )
~ 0
A(~

3 0 ∇ × A(~
~
~
~ x0 ) × A(~x )
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
S(~


| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
V
V
S(V )

˚

~ ×∇
~ ×
∇

~ ×∇
~×
∇

˚

~ x0 )
~ 0 ~ x0 ) ˆˆ  
A(~
3 0 ∇ × A(~
~
~
~
~
= ∇×
+ 
dS(~x ) × A(~x ) × ∇
dx
dx
| ~x − ~x |
| ~x − ~x |
| ~x − ~x0 |
V
V
S(V )

˚

~ ×∇
~ ×
∇

3 0

3 0

˚

~ x0 )
~ 0 ~ x0 ) ˆˆ  
A(~
~x0 − ~x
3 0 ∇ × A(~
~
~
~
d
S(~
x
dx
d
x
)
×
A(~
x
)
×
=
∇
×
+


| ~x − ~x0 |
| ~x − ~x0 |
| ~x − ~x0 |
V
V
S(V )

˚

3 0

Así
~
~ x) = − 1 ∇
A(~
4π

˚
~ 0 ~ x0 )
~ 0 ~ x0 )
1 ~
3 0 ∇ · A(~
3 0 ∇ × A(~
dx
d
x
∇
×
+
| ~x − ~x0 |
4π
| ~x − ~x0 |
V
V

˚

ˆˆ
ˆˆ

1    ~ 0 ~ 0  ~x − ~x0
1   ~ 0
~ x0 ) × ~x − ~x
+
dS(~x ) · A(~x )
d
S(~
x
+
)
×
A(~



4π S(V )
| ~x − ~x0 |3 4π S(V )
| ~x0 − ~x |3
Por otra parte


luego








~·B
~ C
~+ A
~×B
~ ×C
~ = A
~·B
~ C
~ −C
~× A
~×B
~
A












~·B
~ C
~+ A
~×B
~ ×C
~ = A
~ C
~·B
~− C
~ ·B
~ A
~+ C
~ ·A
~ B
~
A












~·B
~ C
~+ A
~×B
~ ×C
~ = B
~ ·A
~ C
~− B
~ ·C
~ A
~+ C
~ ·A
~ B
~
A






 

~·B
~ C
~+ A
~×B
~ ×C
~ =B
~× C
~ ×A
~ + C
~ ·A
~ B
~
A










~·B
~ C
~+ A
~×B
~ ×C
~ = A
~×C
~ ×B
~+ A
~·C
~ B
~
A

---

### Página 136

Finalmente










~
~
~
~
~
~
~
~
~
~
~
~
A·B C + A×B ×C = A·C B+ A×C ×B

~
~ x) = − 1 ∇
A(~
4π

˚
~ 0 ~ x0 )
~ 0 ~ x0 )
1 ~
3 0 ∇ · A(~
3 0 ∇ × A(~
+
∇
×
dx
d
x
| ~x − ~x0 |
4π
| ~x − ~x0 |
V
V

˚





ˆˆ
ˆˆ
1 
~x0 − ~x
1 
~x0 − ~x
~
~
~ x0 )
~
dS(~x ) · 0
dS(~x ) × 0
× A(~
A(~x ) +
+


4π S(V )
| ~x − ~x |3
4π S(V )
| ~x − ~x |3
~ x) está determinado por
Vemos que A(~
~ · A(~
~ x) = 4πD(~x)
∇

~ × A(~
~ x) = 4π R(~
~ x)
∇
para ~x ∈ V
~ x) = A
~ H (~x)
A(~
para ~x ∈ S(V )
